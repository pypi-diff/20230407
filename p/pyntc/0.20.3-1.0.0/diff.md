# Comparing `tmp/pyntc-0.20.3.tar.gz` & `tmp/pyntc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntc-0.20.3.tar", max compression
+gzip compressed data, was "pyntc-1.0.0.tar", max compression
```

## Comparing `pyntc-0.20.3.tar` & `pyntc-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      590 2022-10-27 18:54:42.825087 pyntc-0.20.3/LICENSE
--rw-r--r--   0        0        0     2591 2022-10-27 18:54:42.825087 pyntc-0.20.3/README.md
--rw-r--r--   0        0        0     3029 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/__init__.py
--rw-r--r--   0        0        0      630 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/__init__.py
--rw-r--r--   0        0        0    53035 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/aireos_device.py
--rw-r--r--   0        0        0    37032 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/asa_device.py
--rw-r--r--   0        0        0    16188 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/base_device.py
--rw-r--r--   0        0        0    18518 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/eos_device.py
--rw-r--r--   0        0        0    22425 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/f5_device.py
--rw-r--r--   0        0        0    37370 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/ios_device.py
--rw-r--r--   0        0        0     3488 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/iosxewlc_device.py
--rw-r--r--   0        0        0    14832 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/jnpr_device.py
--rw-r--r--   0        0        0    13631 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/nxos_device.py
--rw-r--r--   0        0        0        0 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/system_features/__init__.py
--rw-r--r--   0        0        0      486 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/system_features/base_feature.py
--rw-r--r--   0        0        0        0 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/system_features/vlans/__init__.py
--rw-r--r--   0        0        0      787 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/system_features/vlans/base_vlans.py
--rw-r--r--   0        0        0     1979 2022-10-27 18:54:42.825087 pyntc-0.20.3/pyntc/devices/system_features/vlans/eos_vlans.py
--rw-r--r--   0        0        0        0 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/devices/tables/__init__.py
--rw-r--r--   0        0        0        0 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/devices/tables/jnpr/__init__.py
--rw-r--r--   0        0        0      190 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/devices/tables/jnpr/loopback.py
--rw-r--r--   0        0        0      690 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/devices/tables/jnpr/loopback.yml
--rw-r--r--   0        0        0    11533 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/errors.py
--rw-r--r--   0        0        0      259 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/__init__.py
--rw-r--r--   0        0        0     3273 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/converters.py
--rw-r--r--   0        0        0     1412 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/__init__.py
--rw-r--r--   0        0        0     1484 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/cisco_asa_show_interface.template
--rw-r--r--   0        0        0      875 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/cisco_asa_show_version.template
--rw-r--r--   0        0        0      178 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/cisco_ios_show_ip_int_brief.template
--rw-r--r--   0        0        0      486 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/cisco_ios_show_version.template
--rw-r--r--   0        0        0      138 2022-10-27 18:54:42.829087 pyntc-0.20.3/pyntc/utils/templates/cisco_ios_show_vlan.template
--rw-r--r--   0        0        0     3853 2022-10-27 18:54:54.333304 pyntc-0.20.3/pyproject.toml
--rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 pyntc-0.20.3/setup.py
--rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 pyntc-0.20.3/PKG-INFO
+-rw-r--r--   0        0        0      590 2023-04-07 21:45:13.735669 pyntc-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2591 2023-04-07 21:45:13.735669 pyntc-1.0.0/README.md
+-rw-r--r--   0        0        0     3029 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/__init__.py
+-rw-r--r--   0        0        0      630 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/__init__.py
+-rw-r--r--   0        0        0    58121 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/aireos_device.py
+-rw-r--r--   0        0        0    44999 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/asa_device.py
+-rw-r--r--   0        0        0    14748 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/base_device.py
+-rw-r--r--   0        0        0    21677 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/eos_device.py
+-rw-r--r--   0        0        0    26957 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/f5_device.py
+-rw-r--r--   0        0        0    43911 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/ios_device.py
+-rw-r--r--   0        0        0     4160 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/iosxewlc_device.py
+-rw-r--r--   0        0        0    14540 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/jnpr_device.py
+-rw-r--r--   0        0        0    17280 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/nxos_device.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/system_features/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/system_features/base_feature.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/system_features/vlans/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/system_features/vlans/base_vlans.py
+-rw-r--r--   0        0        0     1979 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/system_features/vlans/eos_vlans.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/tables/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/tables/jnpr/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/tables/jnpr/loopback.py
+-rw-r--r--   0        0        0      690 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/devices/tables/jnpr/loopback.yml
+-rw-r--r--   0        0        0    11499 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/errors.py
+-rw-r--r--   0        0        0     2114 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/log.py
+-rw-r--r--   0        0        0      259 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/__init__.py
+-rw-r--r--   0        0        0     3371 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/converters.py
+-rw-r--r--   0        0        0     1430 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/__init__.py
+-rw-r--r--   0        0        0     3401 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/cisco_asa_show_interface.template
+-rw-r--r--   0        0        0      875 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/cisco_asa_show_version.template
+-rw-r--r--   0        0        0      178 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/cisco_ios_show_ip_int_brief.template
+-rw-r--r--   0        0        0      486 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/cisco_ios_show_version.template
+-rw-r--r--   0        0        0      138 2023-04-07 21:45:13.739669 pyntc-1.0.0/pyntc/utils/templates/cisco_ios_show_vlan.template
+-rw-r--r--   0        0        0     4153 2023-04-07 21:45:23.387852 pyntc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 pyntc-1.0.0/PKG-INFO
```

### Comparing `pyntc-0.20.3/LICENSE` & `pyntc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/README.md` & `pyntc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/pyntc/__init__.py` & `pyntc-1.0.0/pyntc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Kickoff functions for getting instancs of device objects."""
+"""Kickoff functions for getting instance of device objects."""
 
 import os
 import warnings
 
 from .devices import supported_devices
 from .errors import ConfFileNotFoundError, DeviceNameNotFoundError, UnsupportedDeviceError
```

### Comparing `pyntc-0.20.3/pyntc/devices/__init__.py` & `pyntc-1.0.0/pyntc/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/pyntc/devices/aireos_device.py` & `pyntc-1.0.0/pyntc/devices/aireos_device.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Module for using a Cisco WLC/AIREOS device over SSH."""  # pylint: disable=too-many-lines
 
+import json
 import os
 import re
-import signal
 import time
-import warnings
 
 from netmiko import ConnectHandler
+from netmiko.exceptions import ReadTimeout
+
+from pyntc import log
+from pyntc.devices.base_device import BaseDevice, fix_docs
 from pyntc.errors import (
     CommandError,
     CommandListError,
     DeviceNotActiveError,
     FileTransferError,
     NTCError,
     NTCFileNotFoundError,
     OSInstallError,
     PeerFailedToFormError,
     RebootTimeoutError,
     WLANDisableError,
     WLANEnableError,
 )
 
-from .base_device import BaseDevice, fix_docs
-
 RE_FILENAME_FIND_VERSION = re.compile(r"^.+?(?P<version>\d+(?:-|_)\d+(?:-|_)\d+(?:-|_)\d+)\.", re.M)
 RE_AP_IMAGE_COUNT = re.compile(r"^[Tt]otal\s+number\s+of\s+APs\.+\s+(?P<count>\d+)\s*$", re.M)
 RE_AP_IMAGE_DOWNLOADED = re.compile(r"^\s*[Cc]ompleted\s+[Pp]redownloading\.+\s+(?P<downloaded>\d+)\s*$", re.M)
 RE_AP_IMAGE_UNSUPPORTED = re.compile(r"^\s*[Nn]ot\s+[Ss]upported\.+\s+(?P<unsupported>\d+)\s*$", re.M)
 RE_AP_IMAGE_FAILED = re.compile(r"^\s*[Ff]ailed\s+to\s+[Pp]redownload\.+\s+(?P<failed>\d+)\s*$", re.M)
 RE_AP_BOOT_OPTIONS = re.compile(
     r"^(?P<name>.+?)\s+(?P<primary>(?:\d+\.){3}\d+)\s+(?P<backup>(?:\d+\.){3}\d+)\s+(?P<status>\S+).+$",
@@ -86,14 +87,15 @@
         self.native = None
         self.secret = secret
         self.port = int(port)
         self.global_delay_factor = kwargs.get("global_delay_factor", 1)
         self.delay_factor = kwargs.get("delay_factor", 1)
         self._connected = False
         self.open(confirm_active=confirm_active)
+        log.init(host=host)
 
     def _ap_images_match_expected(self, image_option, image, ap_boot_options=None):
         """
         Test that all AP images have the ``image_option`` matching ``image``.
 
         Args:
             image_option (str): The boot_option dict key ("primary", "backup") to validate.
@@ -115,16 +117,15 @@
             >>>
         """
         if ap_boot_options is None:
             ap_boot_options = self.ap_boot_options
 
         return all(boot_option[image_option] == image for boot_option in ap_boot_options.values())
 
-    @staticmethod
-    def _check_command_output_for_errors(command, command_response):
+    def _check_command_output_for_errors(self, command, command_response):
         """
         Check response from device to see if an error was reported.
 
         Args:
             command (str): The command that was sent to the device.
 
         Raises:
@@ -138,20 +139,22 @@
             >>> command = "invalid command"
             >>> command_response = "Incorrect Usage: invalid command"
             >>> device._check_command_output_for_errors(command, command_resposne)
             CommandError: ...
             >>>
         """
         if "Incorrect usage" in command_response or "Error:" in command_response:
+            log.error("Host %s: Error in %s with response: %s", self.host, command, command_response)
             raise CommandError(command, command_response)
 
     def _enter_config(self):
         """Enter into config mode."""
         self.enable()
         self.native.config_mode()
+        log.debug("Host %s: Device entered config mode.", self.host)
 
     def _image_booted(self, image_name, **vendor_specifics):
         """
         Check if ``image_name`` is the currently booted image.
 
         Args:
             image_name (str): The version to check if image is booted.
@@ -165,16 +168,18 @@
             True
             >>>
         """
         re_version = r"^Product\s+Version\s*\.+\s*(\S+)"
         sysinfo = self.show("show sysinfo")
         booted_image = re.search(re_version, sysinfo, re.M)
         if booted_image.group(1) == image_name:
+            log.info("Host %s: Image %s is booted.", self.host, image_name)
             return True
 
+        log.warning("Host %s: Image %s not booted successfully.", self.host, image_name)
         return False
 
     def _send_command(self, command, expect_string=None, **kwargs):
         """
         Send single command to device.
 
         Args:
@@ -201,16 +206,18 @@
         """
         if expect_string is None:
             response = self.native.send_command_timing(command, **kwargs)
         else:
             response = self.native.send_command(command, expect_string=expect_string, **kwargs)
 
         if "Incorrect usage" in response or "Error:" in response:
+            log.error("Host %s: Error in %s with response: %s", self.host, command, response)
             raise CommandError(command, response)
 
+        log.info("Host %s: Command %s was executed successfully with response: %s", self.host, command, response)
         return response
 
     def _uptime_components(self):
         """
         Retrieve days, hours, and minutes device has been up.
 
         Returns:
@@ -232,14 +239,17 @@
         match_hours = re.search(r"(\d+) hrs?", uptime_string)
         match_minutes = re.search(r"(\d+) mins?", uptime_string)
 
         days = int(match_days.group(1)) if match_days else 0
         hours = int(match_hours.group(1)) if match_hours else 0
         minutes = int(match_minutes.group(1)) if match_minutes else 0
 
+        log.debug(
+            "Host %s: The device has been up for %s days, %s hours, and %s minutes", self.host, days, hours, minutes
+        )
         return days, hours, minutes
 
     def _wait_for_ap_image_download(self, timeout=3600):
         """
         Wait for all APs have completed downloading the image.
 
         Args:
@@ -277,24 +287,45 @@
         while downloaded < ap_count:
             ap_image_stats = self.ap_image_stats
             downloaded = ap_image_stats["downloaded"]
             unsupported = ap_image_stats["unsupported"]
             failed = ap_image_stats["failed"]
             # TODO: When adding logging, send log message of current stats
             if unsupported or failed:
+                log.error(
+                    "Host %s: Failed transferring image to AP\nUnsupported: %s\nFailed: %s\n",
+                    self.host,
+                    unsupported,
+                    failed,
+                )
                 raise FileTransferError(
                     "Failed transferring image to AP\n" f"Unsupported: {unsupported}\n" f"Failed: {failed}\n"
                 )
             elapsed_time = time.time() - start
             if elapsed_time > timeout:
+                log.error(
+                    "Host %s: Failed waiting for AP image to be transferred to all devices:\n Total: %s\nDownloaded: %s",
+                    self.host,
+                    ap_count,
+                    downloaded,
+                )
                 raise FileTransferError(
                     "Failed waiting for AP image to be transferred to all devices:\n"
                     f"Total: {ap_count}\nDownloaded: {downloaded}"
                 )
 
+            log.debug(
+                "Host %s:"
+                "End of waiting time for AP image to be transferred to all devices:\n"
+                "Total: %s\nDownloaded: %s",
+                self.host,
+                ap_count,
+                downloaded,
+            )
+
     def _wait_for_device_reboot(self, timeout=3600):
         """
         Wait for the device to finish reboot process and become accessible.
 
         Args:
             timeout (int): The length of time before considering the device unreachable.
 
@@ -309,19 +340,21 @@
             True
             >>>
         """
         start = time.time()
         while time.time() - start < timeout:
             try:
                 self.open()
+                log.debug("Host %s: Device rebooted.", self.host)
                 return
             except:  # noqa E722 # nosec # pylint: disable=bare-except
                 pass
 
         # TODO: Get proper hostname parameter
+        log.error("Host %s: Device timed out while rebooting.", self.host)
         raise RebootTimeoutError(hostname=self.host, wait_time=timeout)
 
     def _wait_for_peer_to_form(self, redundancy_state, timeout=300):
         """
         Wait for device redundancy state to form properly.
 
         Args:
@@ -342,16 +375,22 @@
             >>> device._wait_for_peer_to_form("standby hot")
             >>>
         """
         start = time.time()
         while time.time() - start < timeout:
             current_state = self.peer_redundancy_state
             if current_state == redundancy_state:
+                log.debug("Host %s: Redundancy state %s formed properly.", self.host, redundancy_state)
                 return
 
+        log.error(
+            "Host %s: Redundancy state did not form properly to desired state: %s from current state: {current_state}",
+            self.host,
+            redundancy_state,
+        )
         raise PeerFailedToFormError(hostname=self.host, desired_state=redundancy_state, current_state=current_state)
 
     @property
     def ap_boot_options(self):
         """
         Boot Options for all APs associated with the controller.
 
@@ -381,14 +420,15 @@
             ap["name"]: {
                 "primary": ap.group("primary"),
                 "backup": ap.group("backup"),
                 "status": ap.group("status").lower(),
             }
             for ap in ap_boot_options
         }
+        log.debug("Host %s: Boot options: {boot_options_by_ap}", self.host, boot_options_by_ap)
         return boot_options_by_ap
 
     @property
     def ap_image_stats(self):
         """
         Stats of downloading the the image to all APs.
 
@@ -407,20 +447,22 @@
             >>>
         """
         ap_images = self.show("show ap image all")
         count = RE_AP_IMAGE_COUNT.search(ap_images).group(1)
         downloaded = RE_AP_IMAGE_DOWNLOADED.search(ap_images).group(1)
         unsupported = RE_AP_IMAGE_UNSUPPORTED.search(ap_images).group(1)
         failed = RE_AP_IMAGE_FAILED.search(ap_images).group(1)
-        return {
+        stats = {
             "count": int(count),
             "downloaded": int(downloaded),
             "unsupported": int(unsupported),
             "failed": int(failed),
         }
+        log.debug("Host %s: Image stats {json.dumps(stats, indent=4)}", self.host)
+        return stats
 
     def backup_running_config(self, filename):
         """
         Create backup of running config.
 
         Args:
             filename (str): Name of backup file.
@@ -462,14 +504,16 @@
                 result["sys"] = result["primary"]
             elif "default" in backup_status:
                 result["sys"] = result["backup"]
             else:
                 result["sys"] = None
         else:
             result = {"sys": None}
+
+        log.debug("Host %s: Boot options %s", self.host, result)
         return result
 
     def checkpoint(self, filename):
         """
         Create a checkpoint file of the current config.
 
         Args:
@@ -482,14 +526,15 @@
         raise NotImplementedError
 
     def close(self):
         """Close the SSH connection to the device."""
         if self.connected:
             self.native.disconnect()
             self._connected = False
+            log.debug("Host %s: Connection closed.", self.host)
 
     def config(self, command, **netmiko_args):
         r"""
         Send config commands to device.
 
         By default, entering and exiting config mode is handled automatically.
         To disable entering and exiting config mode, pass `enter_config_mode` and `exit_config_mode` in ``**netmiko_args``.
@@ -514,15 +559,16 @@
             >>> device.config("boot primary")
             '(host) config>boot primary\n\n(host) config>'
             >>>
         """
         # TODO: Remove this when deprecating config_list method
         original_command_is_str = isinstance(command, str)
 
-        if original_command_is_str:  # TODO: switch to isinstance(command, str) when removing above
+        # TODO: switch to isinstance(command, str) when removing above
+        if original_command_is_str:
             command = [command]
 
         original_exit_config_setting = netmiko_args.get("exit_config_mode")
         netmiko_args["exit_config_mode"] = False
         # Ignore None or invalid args passed for enter_config_mode
         if netmiko_args.get("enter_config_mode") is not False:
             self._enter_config()
@@ -533,61 +579,47 @@
         try:
             for cmd in command:
                 entered_commands.append(cmd)
                 command_response = self.native.send_config_set(cmd, **netmiko_args)
                 command_responses.append(command_response)
                 self._check_command_output_for_errors(cmd, command_response)
         except TypeError as err:
-            raise TypeError(f"Netmiko Driver's {err.args[0]}") from err
+            log.error("Host %s: Netmiko Driver's %s", self.host, err.args[0])
+            raise TypeError(f"Netmiko Driver's {err.args[0]}")
         # TODO: Remove this when deprecating config_list method
         except CommandError as err:
             if not original_command_is_str:
-                raise CommandListError(entered_commands, cmd, err.cli_error_msg) from err
-            raise err
+                log.error(
+                    "Host %s: Commands %s returned the error %s",
+                    self.host,
+                    entered_commands,
+                    err.cli_error_msg,
+                )
+                raise CommandListError(entered_commands, cmd, err.cli_error_msg)
+            else:
+                log.error("Host %s: Commands %s returned the error %s", self.host, entered_commands, err.cli_error_msg)
+                raise err
         # Don't let exception prevent exiting config mode
         finally:
             # Ignore None or invalid args passed for exit_config_mode
             if original_exit_config_setting is not False:
                 self.native.exit_config_mode()
 
         # TODO: Remove this when deprecating config_list method
         if original_command_is_str:
             return command_responses[0]
 
+        log.info(
+            "Host %s: List of config commands %s received responses %s.",
+            self.host,
+            command,
+            command_response,
+        )
         return command_responses
 
-    def config_list(self, commands, **netmiko_args):  # noqa: D401
-        """
-        DEPRECATED - Use the `config` method.
-
-        Send config commands to device.
-
-        By default, entering and exiting config mode is handled automatically.
-        To disable entering and exiting config mode, pass `enter_config_mode` and `exit_config_mode` in ``**netmiko_args``.
-        This supports all arguments supported by Netmiko's `send_config_set` method using ``netmiko_args``.
-
-        Args:
-            commands (list): The commands to send to the device.
-            **netmiko_args: Any argument supported by ``netmiko.base_connection.BaseConnection.send_config_set``.
-
-        Returns:
-            list: Each command's input and ouput from sending the command in ``commands``.
-
-        Raises:
-            TypeError: When sending an argument in ``**netmiko_args`` that is not supported.
-            CommandListError: When one of the commands reports an error on the device.
-
-        Example:
-            >>> device = AIREOSDevice(**connection_args)
-            >>> device.config_list(["interface hostname virtual wlc1.site.com", "config interface vlan airway 20"])
-            >>>
-        """
-        warnings.warn("config_list() is deprecated; use config.", DeprecationWarning)
-        return self.config(commands, **netmiko_args)
-
     def confirm_is_active(self):
         """
         Confirm that the device is either standalone or the active device in a high availability cluster.
 
         Returns:
             bool: True when the device is considered active.
 
@@ -611,30 +643,38 @@
             True
             >>>
         """
         if not self.is_active():
             redundancy_state = self.redundancy_state
             peer_redundancy_state = self.peer_redundancy_state
             self.close()
+            log.error(
+                "Host %s: Device not active error where redundancy state %s and peer redundancy state %s",
+                self.host,
+                redundancy_state,
+                peer_redundancy_state,
+            )
             raise DeviceNotActiveError(self.host, redundancy_state, peer_redundancy_state)
 
         return True
 
     @property
     def connected(self):
         """
         Get connection status of the device.
 
         Returns:
             bool: True if the device is connected, else False.
         """
+        log.debug("Host %s: Connection status %s.", self.host, self._connected)
         return self._connected
 
     @connected.setter
     def connected(self, value):
+        log.debug("Host %s: Device connected is %s.", self.host, value)
         self._connected = value
 
     def disable_wlans(self, wlan_ids):
         """
         Disable all given WLAN IDs.
 
         The string `all` can be passed to disable all WLANs.
@@ -670,16 +710,24 @@
         if not wlans_to_validate.issubset(disabled_wlans):
             commands = [f"wlan disable {wlan}" for wlan in wlan_ids if wlan not in disabled_wlans]
             self.config(commands)
 
             post_disabled_wlans = self.disabled_wlans
             if not wlans_to_validate.issubset(post_disabled_wlans):
                 desired_wlans = wlans_to_validate.union(disabled_wlans)
+                log.error(
+                    "Host %s: WLANS not disabled, with desired WLANs %s and post disabled WLANs %s",
+                    self.host,
+                    desired_wlans,
+                    post_disabled_wlans,
+                )
                 raise WLANDisableError(self.host, desired_wlans, post_disabled_wlans)
 
+        log.info("Host %s: All WLANs with IDs %s were disabled.", self.host, disabled_wlans)
+
     @property
     def disabled_wlans(self):  # noqa: D403
         """
         IDs for all disabled WLANs.
 
         Returns:
             list: Disabled WLAN IDs.
@@ -696,14 +744,15 @@
                 8: {'profile': 'wlan 8', 'ssid': 'wifi-v', 'status': 'disabled', 'interface': '1'}
             }
             >>> device.disabled_wlans
             [2, 4, 8]
             >>>
         """
         disabled_wlans = [wlan_id for wlan_id, wlan_data in self.wlans.items() if wlan_data["status"] == "Disabled"]
+        log.info("Host %s: Disabled WLAN IDs: %s", self.host, disabled_wlans)
         return disabled_wlans
 
     def enable(self):
         """
         Ensure device is in enable mode.
 
         Returns:
@@ -712,14 +761,16 @@
         # Netmiko reports enable and config mode as being enabled
         if not self.native.check_enable_mode():
             self.native.enable()
         # Ensure device is not in config mode
         if self.native.check_config_mode():
             self.native.exit_config_mode()
 
+        log.debug("Host %s: Device enabled.", self.host)
+
     def enable_wlans(self, wlan_ids):
         """
         Enable all given WLAN IDs.
 
         The string `all` can be passed to enable all WLANs.
         Commands are sent to enable WLAN IDs that are not in `self.enabled_wlans`.
         If trying to enable `all` WLANS, then "all" will be sent,
@@ -754,14 +805,20 @@
         if not wlans_to_validate.issubset(enabled_wlans):
             commands = [f"wlan enable {wlan}" for wlan in wlan_ids if wlan not in enabled_wlans]
             self.config(commands)
 
             post_enabled_wlans = self.enabled_wlans
             if not wlans_to_validate.issubset(post_enabled_wlans):
                 desired_wlans = wlans_to_validate.union(enabled_wlans)
+                log.error(
+                    "Host %s: WLANS not enabled,\nwith desired WLANs %s and post enabled WLANs %s",
+                    self.host,
+                    desired_wlans,
+                    post_enabled_wlans,
+                )
                 raise WLANEnableError(self.host, desired_wlans, post_enabled_wlans)
 
     @property
     def enabled_wlans(self):  # noqa: D403
         """
         IDs for all enabled WLANs.
 
@@ -780,14 +837,15 @@
                 8: {'profile': 'wlan 8', 'ssid': 'wifi-v', 'status': 'disabled', 'interface': '1'}
             }
             >>> device.enabled_wlans
             [1, 3, 7]
             >>>
         """
         enabled_wlans = [wlan_id for wlan_id, wlan_data in self.wlans.items() if wlan_data["status"] == "Enabled"]
+        log.info("Host %s: List of enabled WLAN IDs: %s", self.host, enabled_wlans)
         return enabled_wlans
 
     def facts(self):
         """
         Get facts from device.
 
         Raises:
@@ -855,28 +913,43 @@
                     f"transfer download password {password}",
                     f"transfer download serverip {server}",
                     f"transfer download path {filedir}/",
                     f"transfer download filename {filename}",
                 ]
             )
         except CommandListError as error:
+            log.error(
+                "Host %s: File transfer error %s\n\n%s",
+                self.host,
+                FileTransferError.default_message,
+                error.message,
+            )
             raise FileTransferError(error.message) from error
 
         try:
             response = self.native.send_command_timing("transfer download start")
             if "Are you sure you want to start? (y/N)" in response:
                 response = self.show("y", auto_find_prompt=False, delay_factor=delay_factor)
         except CommandError as error:
+            log.error(
+                "Host %s: File transfer error %s\n\n%s",
+                self.host,
+                FileTransferError.default_message,
+                error.message,
+            )
             raise FileTransferError(message=f"{FileTransferError.default_message}\n\n{error.message}") from error
         except:  # noqa E722
+            log.error("Host %s: File transfer error %s", self.host, FileTransferError)
             raise FileTransferError
 
         if "File transfer is successful" not in response:
-            raise FileTransferError(message=f"Did not find expected success message in response, found:\n{response}")
+            log.error("Host %s: Did not find expected success message in response, found:\n%s", self.host, response)
+            raise FileTransferError
 
+        log.info("Host %s: File transferred successfully.", self.host)
         return True
 
     def file_copy_remote_exists(self, src, dest=None, **kwargs):
         """
         Copy 'src' file to remote device.
 
         Args:
@@ -885,14 +958,23 @@
                 Defaults to use the name of the ``src`` file.
 
         Raises:
             NotImplementedError: Function currently not implemented.
         """
         raise NotImplementedError
 
+    @property
+    def hostname(self):
+        """Retrieve hostname from sysinfo."""
+        sysinfo = self.show("show sysinfo")
+        re_hostname = r"^System\s+Name\.+\s*(.+?)\s*$"
+        hostname = re.search(re_hostname, sysinfo, re.M)
+        hostname_string = hostname.group(1)
+        return hostname_string
+
     def install_os(self, image_name, controller="both", save_config=True, disable_wlans=None, **vendor_specifics):
         """
         Install an operating system on the controller.
 
         Args:
             image_name (str): The version to install on the device.
             controller (str): The controller(s) to reboot for install (only applies to HA device).
@@ -934,22 +1016,33 @@
             if disable_wlans is not None:
                 self.disable_wlans(disable_wlans)
             self.reboot(controller=controller, save_config=save_config)
             self._wait_for_device_reboot(timeout=timeout)
             if disable_wlans is not None:
                 self.enable_wlans(disable_wlans)
             if not self._image_booted(image_name):
+                log.error("Host %s: OS install error for image %s", self.host, image_name)
                 raise OSInstallError(hostname=self.host, desired_boot=image_name)
             try:
                 self._wait_for_peer_to_form(peer_redundancy)
             except PeerFailedToFormError:
-                raise OSInstallError(hostname=f"{self.host}-standby", desired_boot=f"{image_name}-{peer_redundancy}")
+                log.error(
+                    "Host %s: Peer failed to form error for image %s and peer redundancy %s",
+                    self.host,
+                    image_name,
+                    peer_redundancy,
+                )
+                raise OSInstallError(
+                    hostname=f"Host {self.host}: {self.host}-standby", desired_boot=f"{image_name}-{peer_redundancy}"
+                )
 
+            log.info("Host %s: OS image %s installed successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: OS image %s not installed.", self.host, image_name)
         return False
 
     def is_active(self):
         """
         Determine if the current processor is the active processor.
 
         Returns:
@@ -989,15 +1082,15 @@
             >>> device.connected
             True
             >>>
         """
         if self.connected:
             try:
                 self.native.find_prompt()
-            except:  # noqa E722
+            except:  # noqa E722  pylint: disable=bare-except
                 self._connected = False
 
         if not self.connected:
             self.native = ConnectHandler(
                 device_type="cisco_wlc",
                 ip=self.host,
                 username=self.username,
@@ -1009,14 +1102,16 @@
             )
             self._connected = True
 
         # This prevents open sessions from connecting to STANDBY WLC
         if confirm_active:
             self.confirm_is_active()
 
+        log.debug("Host %s: Connection to controller was opened successfully.", self.host)
+
     @property
     def peer_redundancy_state(self):
         """
         Determine the redundancy state of the peer processor.
 
         Returns:
             str: The redundancy state of the peer processor.
@@ -1027,71 +1122,71 @@
             >>> device.peer_redundancy_state
             'standby hot'
             >>>
         """
         try:
             show_redundancy = self.show("show redundancy summary")
         except CommandError:
+            log.error("Host %s: Peer redundancy state command error.", self.host)
             return None
         re_peer_redundancy_state = RE_PEER_REDUNDANCY_STATE.search(show_redundancy)
         peer_redundancy_state = re_peer_redundancy_state.group(1).lower()
         if peer_redundancy_state == "n/a":
             peer_redundancy_state = "disabled"
+
+        log.debug("Host %s: Peer redundancy state: %s.", self.host, peer_redundancy_state)
         return peer_redundancy_state
 
-    def reboot(self, timer=0, controller="self", save_config=True, **kwargs):
+    def reboot(self, wait_for_reload=False, controller="self", save_config=True, **kwargs):
         """
         Reload the controller or controller pair.
 
         Args:
-            timer (int): The time to wait before reloading.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
             controller (str): Which controller(s) to reboot (only applies to HA pairs).
             save_config (bool): Whether the configuration should be saved before reload.
 
         Raises:
             ReloadTimeoutError: When the device is still unreachable after the timeout period.
 
         Example:
             >>> device = AIREOSDevice(**connection_args)
             >>> device.reboot()
             >>>
         """
         if kwargs.get("confirm"):
-            warnings.warn("Passing 'confirm' to reboot method is deprecated.", DeprecationWarning)
-
-        def handler(signum, frame):
-            raise RebootSignal("Interrupting after reload")
-
-        signal.signal(signal.SIGALRM, handler)
+            log.warning("Passing 'confirm' to reboot method is deprecated.")
 
         if self.redundancy_mode != "sso disabled":
             reboot_command = f"reset system {controller}"
         else:
             reboot_command = "reset system"
 
-        if timer:
-            reboot_command += f" in {timer}"
-
         if save_config:
             self.save()
 
-        signal.alarm(20)
         try:
             response = self.native.send_command_timing(reboot_command)
-            if "save" in response:
-                if not save_config:
-                    response = self.native.send_command_timing("n")
-                else:
-                    response = self.native.send_command_timing("y")
-            if "reset" in response:
-                self.native.send_command_timing("y")
-        except RebootSignal:
-            signal.alarm(0)
-
-        signal.alarm(0)
+            try:
+                if "save" in response:
+                    if not save_config:
+                        response = self.native.send_command_timing("n")
+                    else:
+                        response = self.native.send_command_timing("y")
+                if "reset" in response:
+                    self.native.send_command_timing("y")
+            except ReadTimeout as expected_exception:
+                log.info("Host %s: Device rebooted.", self.host)
+                log.info("Hit expected exception during reload: %s", expected_exception.__class__)
+            if wait_for_reload:
+                time.sleep(10)
+                self._wait_for_device_reboot()
+        except Exception as err:
+            log.error(err)
+            log.error(err.__class__)
 
     @property
     def redundancy_mode(self):
         """
         Get operating redundancy mode of the controller.
 
         Returns:
@@ -1099,16 +1194,17 @@
 
         Example:
             >>> device = AIREOSDevice(**connection_args)
             >>> device.redundancy_mode
             'sso enabled'
             >>>
         """
-        ha = self.show("show redundancy summary")
-        ha_mode = re.search(r"^\s*Redundancy\s+Mode\s*=\s*(.+?)\s*$", ha, re.M)
+        high_availability = self.show("show redundancy summary")
+        ha_mode = re.search(r"^\s*Redundancy\s+Mode\s*=\s*(.+?)\s*$", high_availability, re.M)
+        log.debug("Host %s: Redundancy mode: {ha_mode.group(1).lower()}", self.host, ha_mode.group(1).lower())
         return ha_mode.group(1).lower()
 
     @property
     def redundancy_state(self):
         """
         Determine the redundancy state of the current processor.
 
@@ -1121,19 +1217,21 @@
             >>> device.redundancy_state
             'active'
             >>>
         """
         try:
             show_redundancy = self.show("show redundancy summary")
         except CommandError:
+            log.error("Host %s: Redundancy state command error.", self.host)
             return None
         re_redundancy_state = RE_REDUNDANCY_STATE.search(show_redundancy)
         redundancy_state = re_redundancy_state.group(1).lower()
         if redundancy_state == "n/a":
             redundancy_state = "disabled"
+        log.debug("Host %s: Redundancy state %s.", self.host, redundancy_state)
         return redundancy_state
 
     def rollback(self):
         """
         Rollback to stored file config.
 
         Raises:
@@ -1160,14 +1258,15 @@
 
         Example:
             >>> device = AIREOSDevice(**connection_args)
             >>> device.save()
             >>>
         """
         self.native.save_config()
+        log.debug("Host %s: Configuration saved.", self.host)
         return True
 
     def set_boot_options(self, image_name, **vendor_specifics):
         """
         Set the version to boot on the device.
 
         Args:
@@ -1193,21 +1292,23 @@
             }
         """
         if self.boot_options["primary"] == image_name:
             boot_command = "boot primary"
         elif self.boot_options["backup"] == image_name:
             boot_command = "boot backup"
         else:
+            log.error("Host %s: File not found error for image %s.", self.host, image_name)
             raise NTCFileNotFoundError(image_name, "'show boot'", self.host)
         self.config(boot_command)
         self.save()
         if not self.boot_options["sys"] == image_name:
+            log.error("Host %s: Setting boot command did not yield expected results", self.host)
             raise CommandError(
                 command=boot_command,
-                message="Setting boot command did not yield expected results",
+                message="Host {self.host}: Setting boot command did not yield expected results",
             )
 
     def show(self, command, expect_string=None, **netmiko_args):
         """
         Send an operational command to the device.
 
         Args:
@@ -1237,92 +1338,79 @@
             System Up Time......3 days 2 hrs 20 mins 30 sec
             ...
             >>>
         """
         # TODO: Remove this when deprecating config_list method
         original_command_is_str = isinstance(command, str)
 
-        if original_command_is_str:  # TODO: switch to isinstance(command, str) when removing above
+        # TODO: switch to isinstance(command, str) when removing above
+        if original_command_is_str:
             command = [command]
 
         entered_commands = []
         command_responses = []
         if expect_string is not None:
             netmiko_args["expect_string"] = expect_string
 
         try:
             for cmd in command:
                 entered_commands.append(cmd)
                 command_response = self.native.send_command(cmd, **netmiko_args)
                 command_responses.append(command_response)
                 self._check_command_output_for_errors(cmd, command_response)
         except TypeError as err:
+            log.error("Host %s: Netmiko Driver's %s", self.host, err.args[0])
             raise TypeError(f"Netmiko Driver's {err.args[0]}")
         # TODO: Remove this when deprecating config_list method
         except CommandError as err:
             if not original_command_is_str:
+                log.error(
+                    "Host %s: Command error for commands %s with message %s.",
+                    self.host,
+                    entered_commands,
+                    err.cli_error_msg,
+                )
                 raise CommandListError(entered_commands, cmd, err.cli_error_msg)
             else:
+                log.error(
+                    "Host %s: Command error for commands %s with message %s.",
+                    self.host,
+                    entered_commands,
+                    err,
+                )
                 raise err
 
         # TODO: Remove this when deprecating config_list method
         if original_command_is_str:
             return command_responses[0]
 
+        log.debug(
+            "Host %s: Successfully executed show commands with responses %s.",
+            self.host,
+            command_responses,
+        )
         return command_responses
 
-    def show_list(self, commands, **netmiko_args):  # noqa: D401
-        """
-        DEPRECATED - Use the `show` method.
-
-        Send operational commands to the device.
-
-        Args:
-            commands (list): The list of commands to send to the device.
-            **netmiko_args: Any argument supported by ``netmiko.ConnectHandler.send_command``.
-
-        Returns:
-            list: The data returned from the device for all commands.
-
-        Raises:
-            TypeError: When sending an argument in ``**netmiko_args`` that is not supported.
-            CommandListError: When the returned data indicates one of the commands failed.
-
-        Example:
-            >>> device = AIREOSDevice(**connection_args)
-            >>> command_data = device._send_command(["show sysinfo", "show boot"])
-            >>> print(command_data[0])
-            Product Version.....8.2.170.0
-            System Up Time......3 days 2 hrs 20 mins 30 sec
-            ...
-            >>> print(command_data[1])
-            Primary Boot Image............................... 8.2.170.0 (default) (active)
-            Backup Boot Image................................ 8.5.110.0
-            >>>
-        """
-        warnings.warn("show_list() is deprecated; use show.", DeprecationWarning)
-        return self.show(commands, **netmiko_args)
-
     @property
     def startup_config(self):
         """
         Get startup config.
 
         Raises:
             NotImplementedError: Function currently not implemented.
         """
         raise NotImplementedError
 
-    def transfer_image_to_ap(self, image, timeout=None):
+    def transfer_image_to_ap(self, image):
         """
         Transfer ``image`` file to all APs connected to the WLC.
 
         Args:
             image (str): The image that should be sent to the APs.
-            timeout (int): The max time to wait for all APs to download the image.
+            timeout (int): Removed, The max time to wait for all APs to download the image.
 
         Returns:
             bool: True if AP images are transferred or swapped, False otherwise.
 
         Example:
             >>> device = AIREOSDevice(**connection_args)
             >>> device.ap_boot_options
@@ -1364,30 +1452,33 @@
             changed = True
             download_image = None
             for option in boot_options:
                 if self.boot_options[option] == image:
                     download_image = option
                     break
             if download_image is None:
-                raise FileTransferError(f"Unable to find {image} on {self.host}")
+                log.error("Host %s: Unable to find %s on host.", self.host, image)
+                raise FileTransferError
 
             self.config(f"ap image predownload {option} all")
             self._wait_for_ap_image_download()
 
         counter = 0
         while counter < 3 and self._ap_images_match_expected("backup", image):
             counter += 1
             changed = True
             self.config("ap image swap all")
             # testing showed delay in reflecting changes when issuing `show ap image all`
             time.sleep(1)
 
         if not self._ap_images_match_expected("primary", image):
+            log.error("Host %s: Unable to set all APs to use %s", self.host, image)
             raise FileTransferError(f"Unable to set all APs to use {image}")
 
+        log.info("Host %s: All images transferred to AP connected to WLC.", self.host)
         return changed
 
     @property
     def uptime(self):
         """
         Get uptime of the device in seconds.
 
@@ -1400,14 +1491,15 @@
             109303
             >>>
         """
         days, hours, minutes = self._uptime_components()
         hours += days * 24
         minutes += hours * 60
         seconds = minutes * 60
+        log.debug("Host %s: Device has been up for %d seconds", self.host, seconds)
         return seconds
 
     @property
     def uptime_string(self):
         """
         Get uptime of the device as a string in the format is dd::hh::mm.
 
@@ -1417,15 +1509,15 @@
         Example:
             >>> device = AIREOSDevice(**connection_args)
             >>> device.uptime_string
             22:04:39
             >>>
         """
         days, hours, minutes = self._uptime_components()
-        return "%02d:%02d:%02d:00" % (days, hours, minutes)
+        return f"{days:02d}:{hours:02d}:{minutes:02d}:00"
 
     @property
     def wlans(self):
         """
         All configured WLANs.
 
         Returns:
@@ -1445,12 +1537,13 @@
             >>>
         """
         wlan_keys = ("profile", "ssid", "status", "interface")
         wlans = []
         show_wlan_summary_out = self.show("show wlan summary")
         re_wlans = RE_WLANS.finditer(show_wlan_summary_out)
         wlans = {int(wlan.group("wlan_id")): dict(zip(wlan_keys, wlan.groups()[1:])) for wlan in re_wlans}
+        log.debug("Host %s: Device WLANs %s.", self.host, json.dumps(wlans, indent=4))
         return wlans
 
 
 class RebootSignal(NTCError):
     """Handles reboot interrupts."""
```

### Comparing `pyntc-0.20.3/pyntc/devices/asa_device.py` & `pyntc-1.0.0/pyntc/devices/asa_device.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Module for using a Cisco ASA device over SSH."""
 
 import os
 import re
-import signal
 import time
-import warnings
 from collections import Counter
 from ipaddress import ip_address, IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 from typing import Dict, Iterable, List, Optional, Union
 
 from netmiko import ConnectHandler
 from netmiko.cisco import CiscoAsaFileTransfer, CiscoAsaSSH
+from netmiko.exceptions import ReadTimeout
+
+from pyntc import log
+from pyntc.devices.base_device import BaseDevice, fix_docs
 from pyntc.errors import (
     CommandError,
     CommandListError,
     FileSystemNotFoundError,
     FileTransferError,
     NTCError,
     NTCFileNotFoundError,
     OSInstallError,
     RebootTimeoutError,
 )
 from pyntc.utils import get_structured_data
 
-from .base_device import BaseDevice, fix_docs
-
 RE_SHOW_FAILOVER_GROUPS = re.compile(r"Group\s+\d+\s+State:\s+(.+?)\s*$", re.M)
 RE_SHOW_FAILOVER_STATE = re.compile(r"(?:Primary|Secondary)\s+-\s+(.+?)\s*$", re.M)
 RE_SHOW_IP_ADDRESS = re.compile(r"^\S+\s+(\S+)\s+((?:\d+.){3}\d+)\s+((?:\d+.){3}\d+)", re.M)
 RE_IPV6_INTERFACE_MATCH = re.compile(r"^\s+([A-Fa-f0-9:]{5,}).+?(/\d+)\s*$", re.M)
 
 
 @fix_docs
@@ -56,53 +56,66 @@
         self.port = int(port)
         self.kwargs = kwargs
         self.global_delay_factor: int = kwargs.get("global_delay_factor", 1)
         self.delay_factor: int = kwargs.get("delay_factor", 1)
         self._connected = False
         self.open()
         self._peer_device: Optional[ASADevice] = None
+        log.init(host=host)
 
     def _enable(self):
-        warnings.warn("_enable() is deprecated; use enable().", DeprecationWarning)
+        log.warning("_enable() is deprecated; use enable().")
         self.enable()
+        log.debug("Host %s: Device enabled", self.host)
 
     def _enter_config(self):
         self.enable()
         self.native.config_mode()
+        log.debug("Host %s: Device entered config mode.", self.host)
 
     def _file_copy(self, src: str, dest: str, file_system: str) -> None:
         self.enable()
 
         if not self.file_copy_remote_exists(src, dest, file_system):
-            fc: CiscoAsaFileTransfer = self._file_copy_instance(src, dest, file_system)
+            file_copy: CiscoAsaFileTransfer = self._file_copy_instance(src, dest, file_system)
 
             try:
-                fc.establish_scp_conn()
-                fc.transfer_file()
+                file_copy.establish_scp_conn()
+                file_copy.transfer_file()
             # Allow EOFErrors to be caught and only raise an error if the file is not actually on the device
             except EOFError:
+                log.error("Host %s: EOF error.", self.host)
                 self.open()
             except Exception:
+                log.error("Host %s: File transfer error %s", self.host, FileTransferError.default_message)
                 raise FileTransferError
             finally:
-                fc.close_scp_chan()
+                log.error("Host %s: An error occurred when transferring file %s.", self.host, src)
+                file_copy.close_scp_chan()
 
             if not self.file_copy_remote_exists(src, dest, file_system):
-                raise FileTransferError(
-                    message="Attempted file copy, but could not validate file existed after transfer"
+                log.error(
+                    "Host %s: Attempted file copy, but could not validate file %s existed after transfer.",
+                    self.host,
+                    src,
                 )
+                raise FileTransferError
+
+        log.info("Host %s: File transferred successfully.", self.host)
 
     def _file_copy_instance(
         self, src: str, dest: Optional[str] = None, file_system: str = "flash:"
     ) -> CiscoAsaFileTransfer:
+        log.info("Host %s: _file_copy_instance dest %s.", self.host, dest)
         if dest is None:
             dest = os.path.basename(src)
 
-        fc = CiscoAsaFileTransfer(self.native, src, dest, file_system=file_system)
-        return fc
+        file_copy = CiscoAsaFileTransfer(self.native, src, dest, file_system=file_system)
+        log.debug("Host %s: File copy instance %s.", self.host, file_copy)
+        return file_copy
 
     def _get_file_system(self):
         """Determine the default file system or directory for device.
 
         Returns:
             str: The name of the default file system or directory for the device.
 
@@ -111,16 +124,18 @@
         """
         raw_data = self.show("dir")
         try:
             file_system = re.match(r"\s*.*?(\S+:)", raw_data).group(1)
 
         except AttributeError:
             # TODO: Get proper hostname
-
+            log.error("Host %s: File system not found with command 'dir'.", self.host)
             raise FileSystemNotFoundError(hostname=self.host, command="dir")
+
+        log.debug("Host %s: File system %s.", self.host, file_system)
         return file_system
 
     def _get_ipv4_addresses(self, host: str) -> Dict[str, List[IPv4Address]]:
         """
         Get IPv4 Addresses for ``host``.
 
         Args:
@@ -141,15 +156,19 @@
             command = "show ip address"
         elif host == "peer":
             command = "failover exec mate show ip address"
 
         show_ip_address = self.show(command)
         re_ip_addresses = RE_SHOW_IP_ADDRESS.findall(show_ip_address)
 
-        return {interface: [IPv4Interface(f"{address}/{netmask}")] for interface, address, netmask in re_ip_addresses}
+        results = {
+            interface: [IPv4Interface(f"{address}/{netmask}")] for interface, address, netmask in re_ip_addresses
+        }
+        log.debug("Host %s: ip interfaces %s", self.host)
+        return results
 
     def _get_ipv6_addresses(self, host: str) -> Dict[str, List[IPv6Address]]:
         """
         Get IPv6 Addresses for ``host``.
 
         Args:
             host (str): Whether to get IP Addresses for `self` or `peer` device.
@@ -189,58 +208,67 @@
                     ipv6_addresses = []
                 interface = line.split()[0]
 
         # Add final interface in iteration if it has IPv6 addresses
         if ipv6_addresses:
             results[interface] = ipv6_addresses
 
+        log.debug("Host %s: ip interfaces %s", self.host, results)
         return results
 
     def _image_booted(self, image_name, **vendor_specifics):
         version_data = self.show("show version")
         if re.search(image_name, version_data):
+            log.info("Host %s: Image %s booted successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: Image %s not booted successfully.", self.host, image_name)
         return False
 
     def _interfaces_detailed_list(self):
         ip_int = self.show("show interface")
         ip_int_data = get_structured_data("cisco_asa_show_interface.template", ip_int)
 
+        log.debug("Host %s: interfaces detailed list %s.", self.host, ip_int_data)
         return ip_int_data
 
     def _raw_version_data(self):
         show_version_out = self.show("show version")
         try:
             version_data = get_structured_data("cisco_asa_show_version.template", show_version_out)[0]
+
+            log.debug("Host %s: version data %s.", self.host, version_data)
             return version_data
         except IndexError:
+            log.error("Host %s: index error.", self.host)
             return {}
 
     def _send_command(self, command, expect_string=None):
         if expect_string is None:
             response = self.native.send_command_timing(command)
         else:
             response = self.native.send_command(command, expect_string=expect_string)
 
         if "% " in response or "Error:" in response:
+            log.error("Host %s: Error in %s with response: %s", self.host, command, response)
             raise CommandError(command, response)
 
+        log.info("Host %s: Command %s was executed successfully with response: %s", self.host, command, response)
         return response
 
     def _show_vlan(self):
         show_vlan_out = self.show("show vlan")
-        show_vlan_data = get_structured_data("cisco_ios_show_vlan.template", show_vlan_out)
 
-        return show_vlan_data
+        log.debug("Host %s: Successfully executed command 'show vlan' with responses %s.", self.host, show_vlan_out)
+        return show_vlan_out.split(",")
 
-    def _uptime_components(self, uptime_full_string):
+    def _uptime_components(self, uptime_full_string):  # pylint: disable=no-self-use
         match_days = re.search(r"(\d+) days?", uptime_full_string)
         match_hours = re.search(r"(\d+) hours?", uptime_full_string)
-        match_minutes = re.search(r"(\d+) minutes?", uptime_full_string)
+        match_minutes = re.search(r"(\d+) mins?", uptime_full_string)
 
         days = int(match_days.group(1)) if match_days else 0
         hours = int(match_hours.group(1)) if match_hours else 0
         minutes = int(match_minutes.group(1)) if match_minutes else 0
 
         return days, hours, minutes
 
@@ -251,26 +279,28 @@
         seconds += hours * 60 * 60
         seconds += minutes * 60
 
         return seconds
 
     def _uptime_to_string(self, uptime_full_string):
         days, hours, minutes = self._uptime_components(uptime_full_string)
-        return "%02d:%02d:%02d:00" % (days, hours, minutes)
+        return f"{days:02d}:{hours:02d}:{minutes:02d}:00"
 
     def _wait_for_device_reboot(self, timeout=3600):
         start = time.time()
         while time.time() - start < timeout:
             try:
                 self.open()
+                log.debug("Host %s: Device rebooted.", self.host)
                 return
-            except:  # noqa E722 # nosec
+            except:  # noqa E722 # nosec   # pylint: disable=bare-except
                 pass
 
         # TODO: Get proper hostname parameter
+        log.error("Host %s: Device timed out while rebooting.", self.host)
         raise RebootTimeoutError(hostname=self.host, wait_time=timeout)
 
     def _wait_for_peer_reboot(self, acceptable_states: Iterable[str], timeout: int = 3600) -> None:
         """
         Wait for peer device to come online and reach an acceptable state.
 
         Args:
@@ -294,33 +324,42 @@
             >>> dev.peer_redundancy_state
             'cold standby'
             >>>
         """
         start = time.time()
         while time.time() - start < timeout:
             if self.peer_redundancy_state == "failed":
+                log.error(
+                    "Host %s: Redundancy state for device %s did not form properly to desired state: %s.",
+                    self.host,
+                    self.host,
+                    self.peer_redundancy_state,
+                )
                 break
 
         while time.time() - start < timeout:
             if self.peer_redundancy_state in acceptable_states:
                 return
             time.sleep(1)
 
         # TODO: Get proper hostname parameter
+        log.error("Host %s: reboot timeout error with timeout %s.", self.host, timeout)
         raise RebootTimeoutError(hostname=f"{self.host}-peer", wait_time=timeout)
 
     def backup_running_config(self, filename):
         """
         Backups running config.
 
         Args:
             filename (str): Name of backup file.
         """
-        with open(filename, "w") as f:
-            f.write(self.running_config)
+        with open(filename, "w", encoding="utf-8") as file_name:
+            file_name.write(self.running_config)
+
+        log.debug("Host %s: Running config backed up to %s.", self.host, self.running_config)
 
     @property
     def boot_options(self):
         """
         Determine boot image.
 
         Returns:
@@ -332,61 +371,56 @@
 
         match = re.search(boot_path_regex, show_boot_out)
         if match:
             boot_image = match.group(2)
         else:
             boot_image = None
 
+        log.debug("Host %s: the boot options are %s", self.host, dict(sys=boot_image))
         return dict(sys=boot_image)
 
     def checkpoint(self, checkpoint_file):
         """
         Create a checkpoint file of the current config.
 
         Args:
             checkpoint_file (str):  Saves a checkpoint file with the name provided to the function.
         """
+        log.debug("Host %s: checkpoint is %s.", self.host, checkpoint_file)
         self.save(filename=checkpoint_file)
 
     def close(self):
         """Disconnect from device."""
         if self._connected:
             self.native.disconnect()
             self._connected = False
+            log.debug("Host %s: Connection closed.", self.host)
 
     def config(self, command):
-        """
-        Send single command to device.
+        """Send configuration commands to a device.
 
         Args:
-            command (str): command to be sent to device.
-        """
-        self._enter_config()
-        self._send_command(command)
-        self.native.exit_config_mode()
-
-    def config_list(self, commands):
-        """
-        Send list of commands to device.
-
-        Args:
-            commands (list): list of commands to be set to device.
+            commands (str, list): String with single command, or list with multiple commands.
 
         Raises:
             CommandListError: Message stating which command failed and the response from the device.
         """
         self._enter_config()
-        entered_commands = []
-        for command in commands:
-            entered_commands.append(command)
-            try:
-                self._send_command(command)
-            except CommandError as e:
-                raise CommandListError(entered_commands, command, e.cli_error_msg)
+        if isinstance(command, list):
+            entered_commands = []
+            for command_instance in command:
+                entered_commands.append(command_instance)
+                try:
+                    self._send_command(command_instance)
+                except CommandError as e:
+                    raise CommandListError(entered_commands, command_instance, e.cli_error_msg)
+        else:
+            self._send_command(command)
         self.native.exit_config_mode()
+        log.info("Host %s: Device configured with command %s.", self.host, command)
 
     @property
     def connected_interface(self) -> str:
         """
         Interface that is assigned an IP Address of ``self.ip_address``.
 
         Returns:
@@ -402,29 +436,33 @@
         ip_property = getattr(self, f"{self.ip_protocol}_addresses")
         for interface, addresses in ip_property.items():
             addrs = {ip_address(addr.ip) for addr in addresses}
             if address in addrs:
                 connected_interface = interface
                 break
 
-        return connected_interface  # TODO: Raise custom exception for when connected_interface is not discovered
+        # TODO: Raise custom exception for when connected_interface is not discovered
+        log.debug("Host %s: Interface connected to %s is %s.", self.host, address, connected_interface)
+        return connected_interface
 
     def enable(self):
         """Ensure device is in enable mode.
 
         Returns:
             None: Device prompt is set to enable mode.
         """
         # Netmiko reports enable and config mode as being enabled
         if not self.native.check_enable_mode():
             self.native.enable()
         # Ensure device is not in config mode
         if self.native.check_config_mode():
             self.native.exit_config_mode()
 
+        log.debug("Host %s: Device enabled.", self.host)
+
     def enable_scp(self) -> None:
         """
         Enable SCP on device by configuring "ssh scopy enable".
 
         The command is ran on the active device; if the device is
         currently standby, then a new connection is created to the
         active device. The configuration is saved after to sync to peer.
@@ -443,24 +481,28 @@
         """
         if self.is_active():
             device: ASADevice = self
         else:
             device = self.peer_device
 
         if not device.is_active():
-            raise FileTransferError("Unable to establish a connection with the active device")
+            log.error("Host %s: Unable to establish a connection with the active device", self.host)
+            raise FileTransferError
 
         try:
             device.config("ssh scopy enable")
         except CommandError:
-            raise FileTransferError("Unable to enable scopy on the device")
+            log.error("Host %s: Unable to enable scopy on the device", self.host)
+            raise FileTransferError
+
+        log.info("Host %s: ssh copy enabled.", self.host)
         device.save()
 
     @property
-    def facts(self):
+    def facts(self):  # pylint: disable=invalid-overridden-method
         """Implement this once facts re-factor is done."""
         return {}
 
     def file_copy(
         self,
         src: str,
         dest: Optional[str] = None,
@@ -496,15 +538,19 @@
         if file_system is None:
             file_system = self._get_file_system()
 
         # netmiko's enable_scp
         self.enable_scp()
         self._file_copy(src, dest, file_system)
         if peer:
-            self.peer_device._file_copy(src, dest, file_system)
+            self.peer_device._file_copy(src, dest, file_system)  # pylint: disable=protected-access
+
+        # logging removed because it messes up unit test mock_basename.assert_not_called()
+        # for tests test_file_copy_no_peer_pass_args, test_file_copy_include_peer
+        # log.info("Host %s: File %s transferred successfully.")
 
     # TODO: Make this an internal method since exposing file_copy should be sufficient
     def file_copy_remote_exists(self, src, dest=None, file_system=None):
         """
         Copy ``src`` file to device.
 
         Args:
@@ -523,17 +569,20 @@
         True
         >>>
         """
         self.enable()
         if file_system is None:
             file_system = self._get_file_system()
 
-        fc = self._file_copy_instance(src, dest, file_system=file_system)
-        if fc.check_file_exists() and fc.compare_md5():
+        file_copy = self._file_copy_instance(src, dest, file_system=file_system)
+        if file_copy.check_file_exists() and file_copy.compare_md5():
+            log.debug("Host %s: File %s already exists on remote.", self.host, src)
             return True
+
+        log.debug("Host %s: File %s does not already exist on remote.", self.host, src)
         return False
 
     def install_os(self, image_name, **vendor_specifics):
         """
         Install OS on device.
 
         Args:
@@ -547,18 +596,21 @@
         """
         timeout = vendor_specifics.get("timeout", 3600)
         if not self._image_booted(image_name):
             self.set_boot_options(image_name, **vendor_specifics)
             self.reboot()
             self._wait_for_device_reboot(timeout=timeout)
             if not self._image_booted(image_name):
+                log.error("Host %s: OS install error for image %s", self.host, image_name)
                 raise OSInstallError(hostname=self.facts.get("hostname"), desired_boot=image_name)
 
+            log.info("Host %s: OS image %s installed successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: OS image %s not installed.", self.host, image_name)
         return False
 
     @property
     def ip_address(self) -> Union[IPv4Address, IPv6Address]:
         """
         IP Address used to establish the connection to the device.
 
@@ -574,20 +626,21 @@
             IPv4Address('10.1.1.1')
             >>> dev = ASADevice("asa_host", **connection_args)
             >>> dev.ip_address
             IPv6Address('fe80::2a0:c9ff:fe03:102')
             >>>
         """
         try:
-            ip = ip_address(self.host)
+            ip_add = ip_address(self.host)
         except ValueError:
             # Assume hostname was used, and retrieve resolved IP from paramiko transport
-            ip = ip_address(self.native.remote_conn.transport.getpeername()[0])
-
-        return ip
+            log.error("Host %s: value error for ip address used to establish connection.", self.host)
+            ip_add = ip_address(self.native.remote_conn.transport.getpeername()[0])
+        log.debug("Host %s: ip address used to establish connection %s.", self.host, ip_add)
+        return ip_add
 
     @property
     def ipv4_addresses(self) -> Dict[str, List[IPv4Address]]:
         """
         IPv4 addresses of the device's interfaces.
 
         Returns:
@@ -595,14 +648,15 @@
 
         Example:
             >>> dev = ASADevice(**connection_args)
             >>> dev.ipv4_addresses
             {'outside': [IPv4Interface('10.132.8.6/24')], 'inside': [IPv4Interface('10.1.1.2/23')]}
             >>>
         """
+        log.debug("Host %s: ipv4 addresses of the devices interfaces %s.", self.host, self._get_ipv4_addresses("self"))
         return self._get_ipv4_addresses("self")
 
     @property
     def ipv6_addresses(self) -> Dict[str, List[IPv6Address]]:
         """
         IPv6 addresses of the device's interfaces.
 
@@ -611,14 +665,15 @@
 
         Example:
             >>> dev = ASADevice(**connection_args)
             >>> dev.ipv6_addresses
             {'outside': [IPv6Interface('fe80::5200:ff:fe0a:1')]}
             >>>
         """
+        log.debug("Host %s: ipv6 addresses of the devices interfaces %s.", self.host, self._get_ipv6_addresses("self"))
         return self._get_ipv6_addresses("self")
 
     @property
     def ip_protocol(self) -> str:
         """
         IP Protocol of the IP Addressed used by the underlying paramiko connection.
 
@@ -635,14 +690,15 @@
             >>> dev = ASADevice("asa_host", **connection_args)
             >>> dev.ip_protocol
             'ipv6'
             >>>
         """
         protocol = f"ipv{self.ip_address.version}"
 
+        log.debug("Host %s: IP protocol for paramiko is %s.", self.host)
         return protocol
 
     def is_active(self):
         """
         Determine if the current processor is the active processor.
 
         Returns:
@@ -657,15 +713,15 @@
         return self.redundancy_state in self.active_redundancy_states
 
     def open(self):
         """Attempt to find device prompt. If not found, create Connecthandler object to device."""
         if self._connected:
             try:
                 self.native.find_prompt()
-            except:  # noqa E722
+            except:  # noqa E722  pylint: disable=bare-except
                 self._connected = False
 
         if not self._connected:
             self.native = ConnectHandler(
                 device_type="cisco_asa",
                 ip=self.host,
                 username=self.username,
@@ -673,14 +729,16 @@
                 port=self.port,
                 global_delay_factor=self.global_delay_factor,
                 secret=self.secret,
                 verbose=False,
             )
             self._connected = True
 
+        log.debug("Host %s: Connection to controller was opened successfully.", self.host)
+
     @property
     def peer_device(self) -> "ASADevice":
         """
         Create instance of ASADevice for peer device.
 
         Returns:
             :class`~devices.ASADevice`: Cisco ASA device instance.
@@ -688,14 +746,15 @@
         if self._peer_device is None:
             self._peer_device = self.__class__(
                 str(self.peer_ip_address), self.username, self.password, self.secret, self.port, **self.kwargs
             )
         else:
             self._peer_device.open()
 
+        log.debug("Host %s: Peer device %s.", self.host, self._peer_device)
         return self._peer_device
 
     @property
     def peer_ip_address(self) -> Union[IPv4Address, IPv6Address]:
         """
         IP Address associated with ``self.ip_address`` on the peer device.
 
@@ -715,14 +774,15 @@
             >>>
         """
         self_address = self.ip_address
         peer_ip_property = getattr(self, f"peer_{self.ip_protocol}_addresses")
         peer_ip_addresses = peer_ip_property[self.connected_interface]
         for address in peer_ip_addresses:
             if self_address in address.network:
+                log.debug("Host %s: Peer IP %s.", self.host, address.ip)
                 return address.ip
 
     @property
     def peer_ipv4_addresses(self) -> Dict[str, List[IPv4Address]]:
         """
         IPv4 addresses of the peer device's interfaces.
 
@@ -771,14 +831,15 @@
             >>> device.peer_redundancy_state
             'standby ready'
             >>>
         """
         try:
             show_failover = self.show("show failover")
         except CommandError:
+            log.error("Host %s: Peer redundancy state command error.", self.host)
             return None
 
         if "Failover On" in show_failover:
             peer_failover_data = show_failover.split("Other host:")[1]
             show_failover_groups = RE_SHOW_FAILOVER_GROUPS.findall(peer_failover_data)
             if not show_failover_groups:
                 re_show_failover_peer_state = RE_SHOW_FAILOVER_STATE.search(peer_failover_data)
@@ -788,54 +849,52 @@
                     peer_redundancy_state = "active"
                 else:
                     peer_redundancy_state_counter = Counter(show_failover_groups)
                     peer_redundancy_state = peer_redundancy_state_counter.most_common()[0][0]
         else:
             peer_redundancy_state = "disabled"
 
+        log.debug("Host %s: Peer redundancy state: %s.", self.host, peer_redundancy_state)
         return peer_redundancy_state.lower()
 
-    def reboot(self, timer=0, **kwargs):
+    def reboot(self, wait_for_reload=False, **kwargs):
         """
         Reload the controller or controller pair.
 
         Args:
-            timer (int, optional): The time to wait before reloading. Defaults to 0.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
 
         Raises:
             RebootTimeoutError: When the device is still unreachable after the timeout period.
 
         Example:
             >>> device = ASADevice(**connection_args)
             >>> device.reboot()
             >>>
         """
         if kwargs.get("confirm"):
-            warnings.warn("Passing 'confirm' to reboot method is deprecated.", DeprecationWarning)
-
-        def handler(signum, frame):
-            raise RebootSignal("Interrupting after reload")
-
-        signal.signal(signal.SIGALRM, handler)
-        signal.alarm(10)
+            log.warning("Passing 'confirm' to reboot method is deprecated.")
 
         try:
-            if timer > 0:
-                first_response = self.show("reload in %d" % timer)
-            else:
-                first_response = self.show("reload")
+            first_response = self.show("reload")
 
             if "System configuration" in first_response:
                 self.native.send_command_timing("no")
 
-            self.native.send_command_timing("\n")
-        except RebootSignal:
-            signal.alarm(0)
-
-        signal.alarm(0)
+            try:
+                self.native.send_command_timing("\n", read_timeout=10)
+            except ReadTimeout as expected_exception:
+                log.info("Host %s: Device rebooted.", self.host)
+                log.info("Hit expected exception during reload: %s", expected_exception.__class__)
+            if wait_for_reload:
+                time.sleep(10)
+                self._wait_for_device_reboot()
+        except Exception as err:
+            log.error(err)
+            log.error(err.__class__)
 
     def reboot_standby(self, acceptable_states: Optional[Iterable[str]] = None, timeout: Optional[int] = None) -> None:
         """
         Reload the standby device from the active device.
 
         Args:
             acceptable_states (iter): List of acceptable redundancy states for the peer device after reboot.
@@ -862,14 +921,16 @@
             acceptable_states = [self.peer_redundancy_state]
         kwargs = {"acceptable_states": acceptable_states}
         if timeout is not None:
             kwargs["timeout"] = timeout
         self.show("failover reload-standby")
         self._wait_for_peer_reboot(**kwargs)
 
+        log.debug("Host %s: reboot standby with timeout %s.", self.host, timeout)
+
     @property
     def redundancy_mode(self):
         """
         Operating redundancy mode of the device.
 
         Returns:
             str: The redundancy mode the device is operating in.
@@ -884,14 +945,15 @@
         try:
             show_failover = self.show("show failover")
         except CommandError:
             return "n/a"
 
         show_failover_first_line = show_failover.splitlines()[0].strip()
         redundancy_mode = show_failover_first_line.lower().lstrip("failover")
+        log.debug("Host %s: Redundancy mode: %s", self.host, redundancy_mode.lstrip())
         return redundancy_mode.lstrip()
 
     @property
     def redundancy_state(self):
         """
         Determine the current redundancy state of the processor.
 
@@ -908,14 +970,15 @@
             >>> device.redundancy_state
             'active'
             >>>
         """
         try:
             show_failover = self.show("show failover")
         except CommandError:
+            log.error("Host %s: Redundancy state command error.", self.host)
             return None
 
         if "Failover On" in show_failover:
             failover_data = show_failover.split("Other host:")[0]
             show_failover_groups = RE_SHOW_FAILOVER_GROUPS.findall(failover_data)
             if not show_failover_groups:
                 re_show_failover_state = RE_SHOW_FAILOVER_STATE.search(failover_data)
@@ -925,14 +988,15 @@
                     redundancy_state = "active"
                 else:
                     redundancy_state_counter = Counter(show_failover_groups)
                     redundancy_state = redundancy_state_counter.most_common()[0][0]
         else:
             redundancy_state = "disabled"
 
+        log.debug("Host %s: Redundancy state %s.", self.host, redundancy_state.lower())
         return redundancy_state.lower()
 
     def rollback(self, rollback_to):
         """
         Rollback the device configuration.
 
         Args:
@@ -959,23 +1023,24 @@
 
         Args:
             filename (str, optional): Name of startup configuration file. Defaults to "startup-config".
 
         Returns:
             bool: True if configuration saved succesfully.
         """
-        command = "copy running-config %s" % filename
+        command = f"copy running-config {filename}"
         # Changed to send_command_timing to not require a direct prompt return.
         self.native.send_command_timing(command)
         # If the user has enabled 'file prompt quiet' which dose not require any confirmation or feedback.
         # This will send return without requiring an OK.
         # Send a return to pass the [OK]? message - Increase delay_factor for looking for response.
         self.native.send_command_timing("\n", delay_factor=2)
         # Confirm that we have a valid prompt again before returning.
         self.native.find_prompt()
+        log.debug("Host %s: Configuration saved.", self.host)
         return True
 
     def set_boot_options(self, image_name, **vendor_specifics):
         """
         Set new image as boot option on device.
 
         Args:
@@ -986,82 +1051,176 @@
             CommandError: Unable to issue command on device.
         """
         current_boot = self.show("show running-config | inc ^boot system ")
         file_system = vendor_specifics.get("file_system")
         if file_system is None:
             file_system = self._get_file_system()
 
-        file_system_files = self.show("dir {0}".format(file_system))
+        file_system_files = self.show(f"dir {file_system}")
         if re.search(image_name, file_system_files) is None:
+            log.error("Host %s: File not found error for image %s.", self.host, image_name)
             raise NTCFileNotFoundError(
                 # TODO: Update to use hostname
                 hostname=self.host,
                 file=image_name,
-                dir=file_system,
+                directory=file_system,
             )
 
         current_images = current_boot.splitlines()
-        commands_to_exec = ["no {0}".format(image) for image in current_images]
-        commands_to_exec.append("boot system {0}/{1}".format(file_system, image_name))
-        self.config_list(commands_to_exec)
+        commands_to_exec = [f"no {image}" for image in current_images]
+        commands_to_exec.append(f"boot system {file_system}/{image_name}")
+        self.config(commands_to_exec)
 
         self.save()
         if self.boot_options["sys"] != image_name:
+            log.error("Host %s: Setting boot command did not yield expected results", self.host)
             raise CommandError(
-                command="boot system {0}/{1}".format(file_system, image_name),
+                command=f"boot system {file_system}/{image_name}",
                 message="Setting boot command did not yield expected results",
             )
 
+        log.info("Host %s: boot options have been set to %s", self.host, image_name)
+
     def show(self, command, expect_string=None):
         """
         Send command to device.
 
         Args:
             command (str): Command to be ran on device.
             expect_string (str, optional): Expected response from running command on device. Defaults to None.
 
         Returns:
             str: Output from running command on device.
         """
         self.enable()
+        log.debug("Host %s: Successfully executed command 'show' with responses.", self.host)
+        if isinstance(command, list):
+            responses = []
+            entered_commands = []
+            for command_instance in command:
+                entered_commands.append(command_instance)
+                try:
+                    responses.append(self._send_command(command_instance))
+                except CommandError as e:
+                    raise CommandListError(entered_commands, command_instance, e.cli_error_msg)
+            return responses
         return self._send_command(command, expect_string=expect_string)
 
-    def show_list(self, commands):
+    @property
+    def startup_config(self):
         """
-        Send list of commands to device.
+        Show startup config.
 
-        Args:
-            commands (list): Commands to be sent to device.
+        :return: Output of command 'show startup-config'.
+        """
+        return self.show("show startup-config")
 
-        Raises:
-            CommandListError: Failure running command on device.
+    @property
+    def uptime(self):
+        """Get uptime from device.
 
         Returns:
-            list: Output from each command sent.
+            int: Uptime in seconds.
         """
-        self.enable()
+        if self._uptime is None:
+            version_data = self._raw_version_data()
+            uptime_full_string = version_data["uptime"]
+            self._uptime = self._uptime_to_seconds(uptime_full_string)
 
-        responses = []
-        entered_commands = []
-        for command in commands:
-            entered_commands.append(command)
-            try:
-                responses.append(self._send_command(command))
-            except CommandError as e:
-                raise CommandListError(entered_commands, command, e.cli_error_msg)
+        return self._uptime
+
+    @property
+    def uptime_string(self):
+        """Get uptime in format dd:hh:mm.
+
+        Returns:
+            str: Uptime of device.
+        """
+        if self._uptime_string is None:
+            version_data = self._raw_version_data()
+            uptime_full_string = version_data["uptime"]
+            self._uptime_string = self._uptime_to_string(uptime_full_string)
 
-        return responses
+        return self._uptime_string
 
     @property
-    def startup_config(self):
+    def hostname(self):
+        """Get hostname of device.
+
+        Returns:
+            str: Hostname of device.
         """
-        Show startup config.
+        version_data = self._raw_version_data()
+        if self._hostname is None:
+            self._hostname = version_data["hostname"]
 
-        :return: Output of command 'show startup-config'.
+        return self._hostname
+
+    @property
+    def interfaces(self):
         """
-        return self.show("show startup-config")
+        Get list of interfaces on device.
+
+        Returns:
+            list: List of interfaces on device.
+        """
+        if self._interfaces is None:
+            self._interfaces = list(x["interface"] for x in self._interfaces_detailed_list())
+
+        return self._interfaces
+
+    @property
+    def model(self):
+        """Get the device model.
+
+        Returns:
+            str: Device model.
+        """
+        version_data = self._raw_version_data()
+        if self._model is None:
+            self._model = version_data["hardware"]
+
+        return self._model
+
+    @property
+    def os_version(self):
+        """Get os version on device.
+
+        Returns:
+            str: OS version on device.
+        """
+        version_data = self._raw_version_data()
+        if self._os_version is None:
+            self._os_version = version_data["version"]
+
+        return self._os_version
+
+    @property
+    def serial_number(self):
+        """Get serial number of device.
+
+        Returns:
+            str: Serial number of device.
+        """
+        version_data = self._raw_version_data()
+        if self._serial_number is None:
+            self._serial_number = version_data["serial"]
+
+        return self._serial_number
+
+    @property
+    def vlans(self):
+        """Get vlan ids from device.
+
+        Returns:
+            list: List of vlans
+        """
+        if self._vlans is None:
+            self._vlans = self._show_vlan()
+
+        return self._vlans
 
 
 class RebootSignal(NTCError):
     """Not implemented."""
 
-    pass
+    pass  # pylint: disable=unnecessary-pass
```

### Comparing `pyntc-0.20.3/pyntc/devices/base_device.py` & `pyntc-1.0.0/pyntc/devices/base_device.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """The module contains the base class that all device classes must inherit from."""
 
-import abc
 import importlib
 import warnings
 
 from pyntc.errors import FeatureNotFoundError, NTCError
 
 
 def fix_docs(cls):
@@ -23,16 +22,14 @@
                     break
     return cls
 
 
 class BaseDevice:  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     """Base Device ABC."""
 
-    __metaclass__ = abc.ABCMeta
-
     def __init__(
         self, host, username, password, device_type=None, **kwargs
     ):  # noqa: D403  # pylint: disable=unused-argument
         """PyNTC base device implementation.
 
         Args:
             host (str): The address of the network device.
@@ -63,160 +60,131 @@
                 volume: Required by F5Device as F5 boots into a volume.
 
         Returns:
             bool: True if image is currently being used by the device, else False.
         """
         raise NotImplementedError
 
-    ####################
-    # ABSTRACT METHODS #
-    ####################
-    @abc.abstractmethod
     def backup_running_config(self, filename):
         """Save a local copy of the running config.
 
         Args:
             filename (str): The local file path on which to save the running config.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def boot_options(self):
         """Get current boot variables.
 
         like system image and kickstart image.
 
         Returns:
             A dictionary, e.g. {'kick': router_kick.img, 'sys': 'router_sys.img'}
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def checkpoint(self, filename):
         """Save a checkpoint of the running configuration to the device.
 
         Args:
             filename (str): The filename to save the checkpoint as on the remote device.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def close(self):
         """Close the connection to the device."""
         raise NotImplementedError
 
-    @abc.abstractmethod
     def config(self, command):
         """Send a configuration command.
 
         Args:
             command (str): The command to send to the device.
 
         Raises:
             CommandError: If there is a problem with the supplied command.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def config_list(self, commands):
-        """Send a list of configuration commands.
-
-        Args:
-            commands (list): A list of commands to send to the device.
-
-        Raises:
-            CommandListError: If there is a problem with one of the commands in the list.
-        """
-        raise NotImplementedError
-
     @property
-    @abc.abstractmethod
     def uptime(self):
         """Uptime integer property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def os_version(self):
         """Operating System string property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def interfaces(self):
         """Interfaces list of strings property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def hostname(self):
         """Host name string property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def fqdn(self):
         """
         Get FQDN of the device.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def uptime_string(self):
         """Uptime string string property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def serial_number(self):
         """
         Get serial number of the device.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def model(self):
         """Model string property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def vlans(self):
         """Vlans lost of strings property, part of device facts.
 
         Raises:
             NotImplementedError: returns not implemented if not included in facts.
         """
         raise NotImplementedError
@@ -238,15 +206,14 @@
                 "serial_number",
                 "os_version",
             ]
         }
         if self.device_type == "cisco_ios_ssh":
             facts[self.device_type] = {"config_register": self.config_register}  # pylint: disable=no-member
 
-    @abc.abstractmethod
     def file_copy(self, src, dest=None, **kwargs):
         """Send a local file to the device.
 
         Args:
             src (str): Path to the local file to send.
             dest (str): The destination file path to be saved on remote flash.
                 If none is supplied, the implementing class should use the basename
@@ -255,15 +222,14 @@
         Keyword Args:
             file_system (str): Supported only for IOS and NXOS. The file system for the
                 remote fle. If no file_system is provided, then the ``get_file_system``
                 method is used to determine the correct file system to use.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def file_copy_remote_exists(self, src, dest=None, **kwargs):
         """Check if a remote file exists.
 
         A remote file exists if it has the same name as supplied dest,
         and the same md5 hash as the source.
 
         Args:
@@ -277,15 +243,14 @@
                 remote fle. If no file_system is provided, then the ``get_file_system``
                 method is used to determine the correct file system to use.
 
         Returns:
             True if the remote file exists, False if it doesn't.
         """
 
-    @abc.abstractmethod
     def install_os(self, image_name, **vendor_specifics):
         """Install the OS from specified image_name.
 
         Args:
             image_name(str): The name of the image on the device to install.
 
         Keyword Args:
@@ -310,56 +275,55 @@
             NTCFileNotFoundError: When the ``image_name`` is not found in the devices ``file_system``.
             FileSystemNotFoundError: When the ``file_system`` is left to default,
                 and the ``file_system`` cannot be identified.
             RebootTimeoutError: When device is rebooted and is unreachable longer than ``timeout`` period.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def open(self):
         """Open a connection to the device."""
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def reboot(self, timer=0):
-        """Reboot the device.
+    def reboot(self, wait_for_reload=False):
+        """Reload a device.
 
         Args:
-            confirm(bool): if False, this method has no effect.
-            timer(int): number of seconds to wait before rebooting.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
+
+        Raises:
+            RebootTimeoutError: When the device is still unreachable after the timeout period.
+
+        Raises:
+            NotImplementedError: _description_
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def rollback(self, checkpoint_file):
         """Rollback to a checkpoint file.
 
         Args:
             checkpoint_file (str): The filename of the checkpoint file to load into the running configuration.
         """
         raise NotImplementedError
 
     @property
-    @abc.abstractmethod
     def running_config(self):
         """Return the running configuration of the device."""
         raise NotImplementedError
 
-    @abc.abstractmethod
     def save(self, filename=None):
         """Save a device's running configuration.
 
         Args:
             filename (str): The filename on the remote device.
                 If none is supplied, the implementing class should
                 save to the "startup configuration".
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def set_boot_options(self, image_name, **vendor_specifics):
         """Set boot variables like system image and kickstart image.
 
         Args:
             image_name: The main system image file name.
 
         Keyword Args:
@@ -372,54 +336,33 @@
         Raises:
             ValueError: When the boot options returned by the ``boot_options``
                 method does not match the ``image_name`` after the config command(s)
                 have been sent to the device.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
     def show(self, command, raw_text=False):
         """Send a non-configuration command.
 
         Args:
             command (str): The command to send to the device.
 
         Keyword Args:
             raw_text (bool): Whether to return raw text or structured data.
 
         Returns:
             The output of the show command, which could be raw text or structured data.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def show_list(self, commands, raw_text=False):
-        """Send a list of non-configuration commands.
-
-        Args:
-            commands (list): A list of commands to send to the device.
-
-        Keyword Args:
-            raw_text (bool): Whether to return raw text or structured data.
-
-        Returns:
-            A list of outputs for each show command
-        """
-        raise NotImplementedError
-
     @property
-    @abc.abstractmethod
     def startup_config(self):
         """Return the startup configuration of the device."""
         raise NotImplementedError
 
-    #################################
-    # Inherited implemented methods #
-    #################################
-
     def feature(self, feature_name):
         """Return a feature class based on the ``feature_name`` for the appropriate subclassed device type."""
         try:
             feature_module = importlib.import_module(
                 f"pyntc.devices.system_features.{feature_name}.{self.device_type}_{feature_name}"
             )
             return feature_module.instance(self)
```

### Comparing `pyntc-0.20.3/pyntc/devices/eos_device.py` & `pyntc-1.0.0/pyntc/devices/eos_device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Module for using an Arista EOS device over the eAPI."""
 
+import os
 import re
 import time
-import os
-import warnings
 
+from netmiko import ConnectHandler, FileTransfer
 from pyeapi import connect as eos_connect
 from pyeapi.client import Node as EOSNative
 from pyeapi.eapilib import CommandError as EOSCommandError
-from netmiko import ConnectHandler
-from netmiko import FileTransfer
 
-from pyntc.utils import convert_list_by_key
-from .system_features.vlans.eos_vlans import EOSVlans
-from .base_device import BaseDevice, RollbackError, RebootTimerError, fix_docs
+from pyntc import log
+from pyntc.devices.base_device import BaseDevice, fix_docs, RollbackError
+from pyntc.devices.system_features.vlans.eos_vlans import EOSVlans
 from pyntc.errors import (
-    NTCError,
     CommandError,
-    OSInstallError,
     CommandListError,
+    FileSystemNotFoundError,
     FileTransferError,
-    RebootTimeoutError,
+    NTCError,
     NTCFileNotFoundError,
-    FileSystemNotFoundError,
+    OSInstallError,
+    RebootTimeoutError,
 )
+from pyntc.utils import convert_list_by_key
 
 
 BASIC_FACTS_KM = {"model": "modelName", "os_version": "internalVersion", "serial_number": "serialNumber"}
 INTERFACES_KM = {
     "speed": "bandwidth",
     "duplex": "duplex",
     "vlan": ["vlanInformation", "vlanId"],
@@ -68,173 +67,184 @@
             value = getattr(self, arg)
             if value is not None:
                 eapi_args[arg] = value
         self.connection = eos_connect(**eapi_args)
         self.native = EOSNative(self.connection)
         # _connected indicates Netmiko ssh connection
         self._connected = False
+        log.init(host=host)
 
     def _file_copy_instance(self, src, dest=None, file_system="flash:"):
         if dest is None:
             dest = os.path.basename(src)
 
-        fc = FileTransfer(self.native_ssh, src, dest, file_system=file_system)
-        return fc
+        file_copy = FileTransfer(self.native_ssh, src, dest, file_system=file_system)
+        log.debug("Host %s: File copy instance %s.", self.host, file_copy)
+        return file_copy
 
     def _get_file_system(self):
         """Determine the default file system or directory for device.
 
         Returns:
             str: The name of the default file system or directory for the device.
 
         Raises:
             FileSystemNotFound: When the module is unable to determine the default file system.
         """
         raw_data = self.show("dir", raw_text=True)
         try:
             file_system = re.match(r"\s*.*?(\S+:)", raw_data).group(1)
         except AttributeError:
+            log.error("Host %s: Attribute error with command 'dir'.", self.host)
             raise FileSystemNotFoundError(hostname=self.hostname, command="dir")
 
+        log.debug("Host %s: File system %s.", self.host, file_system)
         return file_system
 
     def _image_booted(self, image_name, **vendor_specifics):
         version_data = self.show("show boot", raw_text=True)
         if re.search(image_name, version_data):
+            log.info("Host %s: Image %s booted successfully.", self.host, image_name)
             return True
 
         return False
 
     def _interfaces_status_list(self):
         interfaces_list = []
         interfaces_status_dictionary = self.show("show interfaces status")["interfaceStatuses"]
         for key in interfaces_status_dictionary:
             interface_dictionary = interfaces_status_dictionary[key]
             interface_dictionary["interface"] = key
             interfaces_list.append(interface_dictionary)
 
-        return convert_list_by_key(interfaces_list, INTERFACES_KM, fill_in=True, whitelist=["interface"])
+        interface_status_list = convert_list_by_key(
+            interfaces_list, INTERFACES_KM, fill_in=True, whitelist=["interface"]
+        )
+        log.debug("Host %s: interfaces detailed list %s.", self.host, interface_status_list)
+        return interface_status_list
 
-    def _parse_response(self, response, raw_text):
+    def _parse_response(self, response, raw_text):  # pylint: disable=no-self-use
         if raw_text:
             return list(x["result"]["output"] for x in response)
-        else:
-            return list(x["result"] for x in response)
 
-    def _uptime_to_string(self, uptime):
+        return list(x["result"] for x in response)
+
+    def _uptime_to_string(self, uptime):  # pylint: disable=no-self-use
         days = uptime / (24 * 60 * 60)
         uptime = uptime % (24 * 60 * 60)
 
         hours = uptime / (60 * 60)
         uptime = uptime % (60 * 60)
 
         mins = uptime / 60
         uptime = uptime % 60
 
         seconds = uptime
 
-        return "%02d:%02d:%02d:%02d" % (days, hours, mins, seconds)
+        return f"{days:02d}:{hours:02d}:{mins:02d}:{seconds:02d}"
 
     def _wait_for_device_reboot(self, timeout=3600):
         start = time.time()
         while time.time() - start < timeout:
             try:
                 self.show("show hostname")
+                log.debug("Host %s: Device rebooted.", self.host)
                 return
-            except:  # noqa E722 # nosec
+            except:  # noqa E722 # nosec  # pylint: disable=bare-except
                 pass
 
+        log.error("Host %s: Device timed out while rebooting.", self.host)
         raise RebootTimeoutError(hostname=self.hostname, wait_time=timeout)
 
     def backup_running_config(self, filename):
         """
         Create backup file of running configuration.
 
         Args:
             filename (str): The name of the file that will be saved.
         """
-        with open(filename, "w") as f:
-            f.write(self.running_config)
+        with open(filename, "w", encoding="utf-8") as file_name:
+            file_name.write(self.running_config)
+
+        log.debug("Host %s: Running config backed up to %s.", self.host, self.running_config)
 
     @property
     def boot_options(self):
         """Get current running software.
 
         Returns:
             dict: Key is ``sys`` with value being the image on the device.
         """
         image = self.show("show boot-config")["softwareImage"]
         image = image.replace("flash:", "")
+        log.debug("Host %s: the boot options are %s", self.host, dict(sys=image))
         return dict(sys=image)
 
     def checkpoint(self, checkpoint_file):
-        """Create a checkpoint file of the running config.
+        """Copy running config checkpoint.
 
         Args:
-            checkpoint_file (str): Name of the checkpoint file.
+            checkpoint_file (str): Checkpoint file name.
         """
-        self.show("copy running-config %s" % checkpoint_file)
+        log.debug("Host %s: checkpoint is %s.", self.host, checkpoint_file)
+        self.show(f"copy running-config {checkpoint_file}")
 
     def close(self):
         """Not implemented. Just ``passes``."""
-        pass
+        pass  # pylint: disable=unnecessary-pass
 
     def config(self, commands):
         """Send configuration commands to a device.
 
         Args:
             commands (str, list): String with single command, or list with multiple commands.
 
         Raises:
             CommandError: Issue with the command provided.
             CommandListError: Issue with a command in the list provided.
         """
         try:
             self.native.config(commands)
+            log.info("Host %s: Device configured with commands %s.", self.host, commands)
         except EOSCommandError as e:
             if isinstance(commands, str):
+                log.error(
+                    "Host %s: Command error with commands: %s and error message %s", self.host, commands, e.message
+                )
                 raise CommandError(commands, e.message)
             raise CommandListError(commands, e.commands[len(e.commands) - 1], e.message)
 
-    def config_list(self, commands):
-        """Send configuration commands in list format to a device.
-
-        DEPRECATED - Use the `config` method.
-
-        Args:
-            commands (list): List with multiple commands.
-        """
-        warnings.warn("config_list() is deprecated; use config().", DeprecationWarning)
-        self.config(commands)
-
     def enable(self):
         """Ensure device is in enable mode.
 
         Returns:
             None: Device prompt is set to enable mode.
         """
         # Netmiko reports enable and config mode as being enabled
         if not self.native_ssh.check_enable_mode():
             self.native_ssh.enable()
         # Ensure device is not in config mode
         if self.native_ssh.check_config_mode():
             self.native_ssh.exit_config_mode()
 
+        log.debug("Host %s: Device enabled", self.host)
+
     @property
     def uptime(self):
         """
         Get uptime of the device in seconds.
 
         Returns:
             int: Uptime of the device.
         """
         if self._uptime is None:
             sh_version_output = self.show("show version")
             self._uptime = int(time.time() - sh_version_output["bootupTimestamp"])
 
+        log.debug("Host %s: Uptime %s", self.host, self._uptime)
         return self._uptime
 
     @property
     def uptime_string(self):
         """
         Get uptime of the device in the format of dd::hh::mm.
 
@@ -253,92 +263,99 @@
         Returns:
             str: Hostname of the device.
         """
         if self._hostname is None:
             sh_hostname_output = self.show("show hostname")
             self._hostname = sh_hostname_output["hostname"]
 
+        log.debug("Host %s: Hostname %s", self.host, self._hostname)
         return self._hostname
 
     @property
     def interfaces(self):
         """Get list of interfaces on device.
 
         Returns:
             list: List of interfaces
         """
         if self._interfaces is None:
             iface_detailed_list = self._interfaces_status_list()
             self._interfaces = sorted(list(x["interface"] for x in iface_detailed_list))
 
+        log.debug("Host %s: Interfaces %s", self.host, self._interfaces)
         return self._interfaces
 
     @property
     def vlans(self):
         """Get list of VLANS on device.
 
         Returns:
             list: List of VLANS on device.
         """
         if self._vlans is None:
             vlans = EOSVlans(self)
             self._vlans = vlans.get_list()
 
+        log.debug("Host %s: Vlans %s", self.host, self._vlans)
         return self._vlans
 
     @property
     def fqdn(self):
         """Get fully-qualified domain name of device.
 
         Returns:
             str: Fully-qualified domain name of device.
         """
         if self._fqdn is None:
             sh_hostname_output = self.show("show hostname")
             self._fqdn = sh_hostname_output["fqdn"]
 
+        log.debug("Host %s: FQDN %s", self.host, self._fqdn)
         return self._fqdn
 
     @property
     def model(self):
         """Get model of device.
 
         Returns:
             str: Model of device.
         """
         if self._model is None:
             sh_version_output = self.show("show version")
             self._model = sh_version_output["modelName"]
 
+        log.debug("Host %s: Model %s", self.host, self._model)
         return self._model
 
     @property
     def os_version(self):
         """Get OS version on device.
 
         Returns:
             str: OS version of device.
         """
         if self._os_version is None:
             sh_version_output = self.show("show version")
             self._os_version = sh_version_output["internalVersion"]
 
+        log.debug("Host %s: OS version %s", self.host, self._os_version)
         return self._os_version
 
     @property
     def serial_number(self):
         """Get serial number of device.
 
         Returns:
             str: Serial number of device.
         """
         if self._serial_number is None:
             sh_version_output = self.show("show version")
             self._serial_number = sh_version_output["serialNumber"]
 
+        log.debug("Host %s: Serial number %s", self.host, self._serial_number)
         return self._serial_number
 
     def file_copy(self, src, dest=None, file_system=None):
         """Copy file to device.
 
         Args:
             src (string): source file
@@ -351,29 +368,34 @@
         self.open()
         self.enable()
 
         if file_system is None:
             file_system = self._get_file_system()
 
         if not self.file_copy_remote_exists(src, dest, file_system):
-            fc = self._file_copy_instance(src, dest, file_system=file_system)
+            file_copy = self._file_copy_instance(src, dest, file_system=file_system)
 
             try:
-                fc.enable_scp()
-                fc.establish_scp_conn()
-                fc.transfer_file()
+                file_copy.enable_scp()
+                file_copy.establish_scp_conn()
+                file_copy.transfer_file()
+                log.info("Host %s: File %s transferred successfully.", self.host, src)
             except:  # noqa E722
+                log.error("Host %s: File transfer error %s", self.host, FileTransferError.default_message)
                 raise FileTransferError
             finally:
-                fc.close_scp_chan()
+                file_copy.close_scp_chan()
 
             if not self.file_copy_remote_exists(src, dest, file_system):
-                raise FileTransferError(
-                    message="Attempted file copy, but could not validate file existed after transfer"
+                log.error(
+                    "Host %s: Attempted file copy, but could not validate file existed after transfer %s",
+                    self.host,
+                    FileTransferError.default_message,
                 )
+                raise FileTransferError
 
     # TODO: Make this an internal method since exposing file_copy should be sufficient
     def file_copy_remote_exists(self, src, dest=None, file_system=None):
         """Copy file to remote device if it exists.
 
         Args:
             src (string): source file
@@ -383,18 +405,20 @@
         Returns:
             bool: True if remote file exists.
         """
         self.enable()
         if file_system is None:
             file_system = self._get_file_system()
 
-        fc = self._file_copy_instance(src, dest, file_system=file_system)
-        if fc.check_file_exists() and fc.compare_md5():
+        filecopy = self._file_copy_instance(src, dest, file_system=file_system)
+        if filecopy.check_file_exists() and filecopy.compare_md5():
+            log.debug("Host %s: File %s already exists on remote.", self.host, src)
             return True
 
+        log.debug("Host %s: File %s does not already exist on remote.", self.host, src)
         return False
 
     def install_os(self, image_name, **vendor_specifics):
         """Install new OS on device.
 
         Args:
             image_name (str): Name of the image name to be installed.
@@ -407,98 +431,104 @@
         """
         timeout = vendor_specifics.get("timeout", 3600)
         if not self._image_booted(image_name):
             self.set_boot_options(image_name, **vendor_specifics)
             self.reboot()
             self._wait_for_device_reboot(timeout=timeout)
             if not self._image_booted(image_name):
+                log.error("Host %s: OS install error for image %s", self.host, image_name)
                 raise OSInstallError(hostname=self.hostname, desired_boot=image_name)
 
+            log.info("Host %s: OS image %s installed successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: OS image %s not installed.", self.host, image_name)
         return False
 
     def open(self):
         """Open ssh connection with Netmiko ConnectHandler to be used with FileTransfer."""
         if self._connected:
             try:
-                self.native_ssh.find_prompt()
-            except Exception:
+                self.native_ssh.find_prompt()  # pylint: disable=access-member-before-definition
+            except Exception:  # pylint: disable=broad-except
                 self._connected = False
 
         if not self._connected:
-            self.native_ssh = ConnectHandler(
+            self.native_ssh = ConnectHandler(  # pylint: disable=attribute-defined-outside-init
                 device_type="arista_eos",
                 ip=self.host,
                 username=self.username,
                 password=self.password,
                 # port=self.port,
                 # global_delay_factor=self.global_delay_factor,
                 # secret=self.secret,
                 verbose=False,
             )
             self._connected = True
 
-    def reboot(self, timer=0, **kwargs):
+        log.debug("Host %s: Connection to controller was opened successfully.", self.host)
+
+    def reboot(self, wait_for_reload=False, **kwargs):
         """
         Reload the controller or controller pair.
 
         Args:
-            timer (int, optional): The time to wait before reloading. Defaults to 0.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
 
         Raises:
             RebootTimeoutError: When the device is still unreachable after the timeout period.
 
         Example:
             >>> device = EOSDevice(**connection_args)
             >>> device.reboot()
             >>>
 
         """
         if kwargs.get("confirm"):
-            warnings.warn("Passing 'confirm' to reboot method is deprecated.", DeprecationWarning)
-
-        if timer != 0:
-            raise RebootTimerError(self.device_type)
+            log.warning("Passing 'confirm' to reboot method is deprecated.")
 
         self.show("reload now")
+        log.info("Host %s: Device rebooted.", self.host)
+        if wait_for_reload:
+            self._wait_for_device_reboot()
 
     def rollback(self, rollback_to):
         """Rollback device configuration.
 
         Args:
             rollback_to (str): Name of file to revert configuration to.
 
         Raises:
-            RollbackError: When rollback is unsuccesful.
+            RollbackError: When rollback is unsuccessful.
         """
         try:
-            self.show("configure replace %s force" % rollback_to)
+            self.show(f"configure replace {rollback_to} force")
+            log.info("Host %s: Rollback to %s.", self.host, rollback_to)
         except (CommandError, CommandListError):
-            raise RollbackError("Rollback unsuccessful. %s may not exist." % rollback_to)
+            log.error("Host %s: Rollback unsuccessful. %s may not exist.", self.host, rollback_to)
+            raise RollbackError(f"Rollback unsuccessful. {rollback_to} may not exist.")
 
     @property
     def running_config(self):
-        """Show running configuration.
+        """Return running config.
 
         Returns:
             str: Running configuration.
         """
+        log.debug("Host %s: Show running config.", self.host)
         return self.show("show running-config", raw_text=True)
 
     def save(self, filename="startup-config"):
-        """Copy running configuration to startup configuration.
-
-        Args:
-            filename (str, optional): Name where you want running configuration to save. Defaults to "startup-config".
+        """Show running configuration.
 
         Returns:
-            bool: True when succesfull.
+            str: Running configuration.
         """
-        self.show("copy running-config %s" % filename)
+        log.debug("Host %s: Copy running config with name %s.", self.host, filename)
+        self.show(f"copy running-config {filename}")
         return True
 
     def set_boot_options(self, image_name, **vendor_specifics):
         """Set boot option to specified image.
 
         Args:
             image_name (str): Name of the image file.
@@ -507,25 +537,29 @@
             NTCFileNotFoundError: File not found on device.
             CommandError: Error in trying to set image as boot option.
         """
         file_system = vendor_specifics.get("file_system")
         if file_system is None:
             file_system = self._get_file_system()
 
-        file_system_files = self.show("dir {0}".format(file_system), raw_text=True)
+        file_system_files = self.show(f"dir {file_system}", raw_text=True)
         if re.search(image_name, file_system_files) is None:
-            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, dir=file_system)
+            log.error("Host %s: File not found error for image %s.", self.host, image_name)
+            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, directory=file_system)
 
-        self.show("install source {0}{1}".format(file_system, image_name))
+        self.show(f"install source {file_system}{image_name}")
         if self.boot_options["sys"] != image_name:
+            log.error("Host %s: Setting boot command did not yield expected results", self.host)
             raise CommandError(
-                command="install source {0}".format(image_name),
+                command=f"install source {image_name}",
                 message="Setting install source did not yield expected results",
             )
 
+        log.info("Host %s: boot options have been set to %s", self.host, image_name)
+
     def show(self, commands, raw_text=False):
         """Send configuration commands to a device.
 
         Args:
             commands (str, list): String with single command, or list with multiple commands.
             raw_text (bool, optional): False if encode should be json, True if encoding is text. Defaults to False.
 
@@ -542,38 +576,31 @@
         if original_commands_is_str:
             commands = [commands]
         try:
             response = self.native.enable(commands, encoding=encoding)
             response_list = self._parse_response(response, raw_text=raw_text)
             if original_commands_is_str:
                 return response_list[0]
+            log.debug("Host %s: Successfully executed command 'show' with responses %s.", self.host, response_list)
             return response_list
-        except EOSCommandError as e:
+        except EOSCommandError as err:
             if original_commands_is_str:
-                raise CommandError(e.commands, e.message)
-            raise CommandListError(commands, e.commands[len(e.commands) - 1], e.message)
-
-    def show_list(self, commands):
-        """Send show commands in list format to a device.
-
-        DEPRECATED - Use the `show` method.
-
-        Args:
-            commands (list): List with multiple commands.
-        """
-        warnings.warn("show_list() is deprecated; use show().", DeprecationWarning)
-        self.show(commands)
+                log.error("Host %s: Command error for command %s with message %s.", self.host, commands, err.message)
+                raise CommandError(err.commands, err.message)
+            log.error("Host %s: Command list error for commands %s with message %s.", self.host, commands, err.message)
+            raise CommandListError(commands, err.commands[len(err.commands) - 1], err.message)
 
     @property
     def startup_config(self):
         """Get startup configuration.
 
         Returns:
             str: Startup configuration.
         """
+        log.debug("Host %s: show startup-config", self.host)
         return self.show("show startup-config", raw_text=True)
 
 
 class RebootSignal(NTCError):
     """Error for sending reboot signal."""
 
-    pass
+    pass  # pylint: disable=unnecessary-pass
```

### Comparing `pyntc-0.20.3/pyntc/devices/f5_device.py` & `pyntc-1.0.0/pyntc/devices/f5_device.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 import re
 import time
 import warnings
 
 import requests
 from f5.bigip import ManagementRoot
 
-from pyntc.errors import OSInstallError, FileTransferError, NTCFileNotFoundError, NotEnoughFreeSpaceError
-from .base_device import BaseDevice
+from pyntc import log
+from pyntc.devices.base_device import BaseDevice
+from pyntc.errors import FileTransferError, NotEnoughFreeSpaceError, NTCFileNotFoundError, OSInstallError
+
+# TODO: Check in on soap_handler in the F5Device, many instances of no-member. Is this broken?
 
 
 class F5Device(BaseDevice):
     """F5 LTM Device Implementation."""
 
     vendor = "f5"
 
@@ -25,67 +28,74 @@
             host (str): The address of the network device.
             username (str): The username to authenticate with the device.
             password (str): The password to authenticate with the device.
         """
         super().__init__(host, username, password, device_type="f5_tmos_icontrol")
 
         self.api_handler = ManagementRoot(self.host, self.username, self.password)
+        log.init(host=host)
 
     def _check_free_space(self, min_space=0):
         """Check for minimum space on the device.
 
         Args:
             min_space (int): The minimal amount of space required.
 
         Raises:
             NotEnoughFreeSpaceError: When the amount of space on the device is less than min_space.
         """
         free_space = self._get_free_space()
 
         if not free_space:
             raise ValueError("Could not get free space")
-        elif free_space >= min_space:
+
+        if free_space >= min_space:
             return
         elif free_space < min_space:
+            log.error("Host %s: Not enough free space for min space requirement %s.", self.host, min_space)
             raise NotEnoughFreeSpaceError(hostname=self.host, min_space=min_space)
 
+        log.debug("Host %s: Free space %s is sufficient.", self.host, free_space)
+
     def _check_md5sum(self, filename, checksum):
         """Check is md5sum is correct.
 
         Args:
             filename (str): Name of file to generate md5.
             checksum (str): checksum used against image.
 
         Returns:
             bool: True if md5 matches. Otherwise, false.
         """
         md5sum = self._file_copy_remote_md5(filename)
 
         if checksum == md5sum:
+            log.debug("Host %s: Checksums match.", self.host)
             return True
         else:
+            log.debug("Host %s: Checksums do not match.", self.host)
             return False
 
     @staticmethod
     def _file_copy_local_file_exists(filepath):
         return os.path.isfile(filepath)
 
     def _file_copy_local_md5(self, filepath, blocksize=2**20):
         if self._file_copy_local_file_exists(filepath):
-            m = hashlib.md5()  # nosec
-            with open(filepath, "rb") as f:
-                buf = f.read(blocksize)
+            md5_check = hashlib.md5()  # nosec
+            with open(filepath, "rb") as file_name:
+                buf = file_name.read(blocksize)
                 while buf:
-                    m.update(buf)
-                    buf = f.read(blocksize)
-            return m.hexdigest()
+                    md5_check.update(buf)
+                    buf = file_name.read(blocksize)
+            return md5_check.hexdigest()
 
     def _file_copy_remote_md5(self, filepath):
         md5sum_result = None
-        md5sum_output = self.api_handler.tm.util.bash.exec_cmd("run", utilCmdArgs='-c "md5sum {}"'.format(filepath))
+        md5sum_output = self.api_handler.tm.util.bash.exec_cmd("run", utilCmdArgs=f'-c "md5sum {filepath}"')
         if md5sum_output:
             md5sum_result = md5sum_output.commandResult
             md5sum_result = md5sum_result.split()[0]
 
         return md5sum_result
 
     def _get_active_volume(self):
@@ -94,14 +104,15 @@
         Returns:
             str: Name of active volume.
         """
         volumes = self._get_volumes()
         for _volume in volumes:
             if hasattr(_volume, "active") and _volume.active is True:
                 current_volume = _volume.name
+                log.debug("Host %s: Active volume name is %s.", self.host, current_volume)
                 return current_volume
 
     def _get_free_space(self):
         """Get free space on the device.
 
         Example:
             >>> [root@ntc:Active:Standalone] config # vgdisplay -s --units G
@@ -116,61 +127,74 @@
             free_space = free_space_output.commandResult
             free_space_regex = r".*\s\/\s(\d+\.?\d+) GB free"
             match = re.match(free_space_regex, free_space)
 
             if match:
                 free_space = float(match.group(1))
 
+        log.debug("Host %s: Free space is %s GB.", self.host, free_space)
         return free_space
 
     def _get_images(self):
         images = self.api_handler.tm.sys.software.images.get_collection()
 
+        log.debug("Host %s: List of images %s.", self.host, images)
         return images
 
     def _get_interfaces_list(self):
-        interfaces = self.soap_handler.Networking.Interfaces.get_list()
+        interfaces = self.soap_handler.Networking.Interfaces.get_list()  # pylint: disable=no-member
+        log.debug("Host %s: List of interfaces %s.", self.host, interfaces)
         return interfaces
 
     def _get_model(self):
-        return self.soap_handler.System.SystemInfo.get_marketing_name()
+        model = self.soap_handler.System.SystemInfo.get_marketing_name()  # pylint: disable=no-member
+        log.debug("Host %s: Model name %s.", self.host, model)
+        return model
 
     def _get_serial_number(self):
-        system_information = self.soap_handler.System.SystemInfo.get_system_information()
+        system_information = self.soap_handler.System.SystemInfo.get_system_information()  # pylint: disable=no-member
         chassis_serial = system_information.get("chassis_serial")
 
+        log.debug("Host %s: Serial number %s.", self.host, chassis_serial)
         return chassis_serial
 
     def _get_uptime(self):
-        return self.soap_handler.System.SystemInfo.get_uptime()
+        uptime = self.soap_handler.System.SystemInfo.get_uptime()  # pylint: disable=no-member
+        log.debug("Host %s: Uptime %s.", self.host, uptime)
+        return uptime
 
     def _get_version(self):
-        return self.soap_handler.System.SystemInfo.get_version()
+        version = self.soap_handler.System.SystemInfo.get_version()  # pylint: disable=no-member
+        log.debug("Host %s: Version %s.", self.host, version)
+        return version
 
     def _get_vlans(self):
-        rd_list = self.soap_handler.Networking.RouteDomainV2.get_list()
-        rd_vlan_list = self.soap_handler.Networking.RouteDomainV2.get_vlan(rd_list)
+        rd_list = self.soap_handler.Networking.RouteDomainV2.get_list()  # pylint: disable=no-member
+        rd_vlan_list = self.soap_handler.Networking.RouteDomainV2.get_vlan(rd_list)  # pylint: disable=no-member
 
+        log.debug("Host %s: List of vlans %s.", self.host, rd_vlan_list)
         return rd_vlan_list
 
     def _get_volumes(self):
         volumes = self.api_handler.tm.sys.software.volumes.get_collection()
 
+        log.debug("Host %s: List of volumes %s.", self.host, volumes)
         return volumes
 
     def _image_booted(self, image_name, **vendor_specifics):
         """Check if requested booted volume is an active volume.
 
         Args:
             image_name (str): Name of image.
 
         Returns:
             bool: True if booted volume is equal to active volume. Otherwise, false.
         """
         volume = vendor_specifics.get("volume")
+        log.debug("Host %s: Checking if image %s has been booted.", self.host, image_name)
         return True if self._get_active_volume() == volume else False
 
     def _image_exists(self, image_name):
         """Check if image exists on the device.
 
         Args:
             image_name (str): Name of image.
@@ -182,16 +206,18 @@
 
         if all_images_output:
             all_images = all_images_output.commandResult.splitlines()
         else:
             return None
 
         if image_name in all_images:
+            log.debug("Host %s: Image %s exists.", self.host, image_name)
             return True
         else:
+            log.debug("Host %s: Image %s does not exist.", self.host, image_name)
             return False
 
     def _image_install(self, image_name, volume):
         """Request installation of the image on a volume.
 
         Args:
             image_name (str): Name of volume.
@@ -202,29 +228,33 @@
         create_volume = not self._volume_exists(volume)
 
         if create_volume:
             options.append({"create-volume": True})
 
         self.api_handler.tm.sys.software.images.exec_cmd("install", name=image_name, volume=volume, options=options)
 
+        log.info("Host %s: Image %s is installed.", self.host, image_name)
+
     def _image_match(self, image_name, checksum):
         """Check if image name matches the checksum.
 
         Args:
             image_name (str): Name of image.
             checksum (str): Expected checksum.
 
         Returns:
             bool: True if expected checksum matches file checksum. Otherwise, false.
         """
         if self._image_exists(image_name):
             image = os.path.join("/shared/images", image_name)
             if self._check_md5sum(image, checksum):
+                log.debug("Host %s: Image %s matches the checksum.", self.host, image_name)
                 return True
 
+        log.debug("Host %s: Image %s does not match the checksum.", self.host, image_name)
         return False
 
     def _reboot_to_volume(self, volume_name=None):
         """Request the reboot (activation) to a specified volume.
 
         Args:
             volume_name (str, optional): Volume name. Defaults to None.
@@ -232,51 +262,58 @@
         if volume_name:
             self.api_handler.tm.sys.software.volumes.exec_cmd("reboot", volume=volume_name)
         else:
             # F5 SDK API does not support reboot to the current volume.
             # This is a workaround by issuing reboot command from bash directly.
             self.api_handler.tm.util.bash.exec_cmd("run", utilCmdArgs='-c "reboot"')
 
+        log.debug("Host %s: Activation to volume %s.", self.host, volume_name)
+
     def _reconnect(self):
         """Reconnect to the device."""
         self.api_handler = ManagementRoot(self.host, self.username, self.password)
+        log.debug("Host %s: Reconnect to device.", self.host)
 
     def _upload_image(self, image_filepath):
         """Upload an iso image to the device.
 
         Args:
             image_filepath (str): Name of file.
         """
         image_filename = os.path.basename(image_filepath)
-        _URI = "https://{hostname}/mgmt/cm/autodeploy/software-image-uploads/{filename}".format(
-            hostname=self.host, filename=image_filename
-        )
+        upload_uri = f"https://{self.host}/mgmt/cm/autodeploy/software-image-uploads/{image_filename}"
         chunk_size = 512 * 1024
         size = os.path.getsize(image_filepath)
         headers = {"Content-Type": "application/octet-stream"}
-        requests.packages.urllib3.disable_warnings()
+        requests.packages.urllib3.disable_warnings()  # pylint: disable=no-member
         start = 0
 
         with open(image_filepath, "rb") as fileobj:
             while True:
                 payload = fileobj.read(chunk_size)
                 if not payload:
                     break
 
                 end = fileobj.tell()
                 if end < chunk_size:
                     end = size
-                content_range = "{}-{}/{}".format(start, end - 1, size)
+                content_range = f"{start}-{end - 1}/{size}"
                 headers["Content-Range"] = content_range
                 requests.post(
-                    _URI, auth=(self.username, self.password), data=payload, headers=headers, verify=False  # nosec
+                    upload_uri,
+                    auth=(self.username, self.password),
+                    data=payload,
+                    headers=headers,
+                    verify=False,  # nosec
                 )
 
                 start += len(payload)
 
+        log.info("Host %s: Image %s uploaded to %s.", self.host, image_filename, image_filepath)
+
     @staticmethod
     def _uptime_to_string(uptime):
         """Change uptime to a string.
 
         Args:
             uptime (float): Uptime represented in a float.
 
@@ -300,14 +337,15 @@
             volume_name (str): Volume name.
 
         Returns:
             bool: True if volume exists. Otherwise, false.
         """
         result = self.api_handler.tm.sys.software.volumes.volume.exists(name=volume_name)
 
+        log.debug("Host %s: Checking if volume exists.", self.host)
         return result
 
     def _wait_for_device_reboot(self, volume_name, timeout=600):
         """Wait for device to be booted into a specified volume.
 
         Args:
             volume_name (str): Volume name to boot into.
@@ -322,16 +360,20 @@
         while time.time() < end_time:
             time.sleep(5)
             try:
                 self._reconnect()
                 volume = self.api_handler.tm.sys.software.volumes.volume.load(name=volume_name)
                 if hasattr(volume, "active") and volume.active is True:
                     return True
-            except Exception:  # noqa E722 # nosec
+
+                log.debug("Host %s: Reboot successfull.", self.host)
+            except Exception:  # noqa E722 # nosec  # pylint: disable=broad-except
+                log.error("Host %s: Error while rebooting.", self.host)
                 pass
+        log.debug("Host %s: Reboot not successfull.", self.host)
         return False
 
     def _wait_for_image_installed(self, image_name, volume, timeout=1800):
         """Wait for the device to install image on a volume.
 
         Args:
             image_name (str): The name of the image that should be booting.
@@ -345,18 +387,20 @@
 
         while time.time() < end_time:
             time.sleep(20)
             # Avoid race-conditions issues. Newly created volumes _might_ lack
             # of .version attribute in first seconds of their live.
             try:
                 if self.image_installed(image_name=image_name, volume=volume):
+                    log.info("Host %s: Image %s installed on volume %s.", self.host, image_name, volume)
                     return
-            except:  # noqa E722 # nosec
+            except:  # noqa E722 # nosec  # pylint: disable=bare-except
                 pass
 
+        log.error("Host %s: OS install error with image %s and volume %s.", self.host, image_name, volume)
         raise OSInstallError(hostname=self.hostname, desired_boot=volume)
 
     def backup_running_config(self, filename):
         """Backup running configuration.
 
         Args:
             filename (str): Name of file to save running config to.
@@ -371,14 +415,15 @@
         """Get active volume.
 
         Returns:
             dict: Key is ``active volume`` with value being the current active volume.
         """
         active_volume = self._get_active_volume()
 
+        log.debug("Host %s: Active volume name %s.", self.host, active_volume)
         return {"active_volume": active_volume}
 
     def checkpoint(self, filename):
         """Create checkpoint configuration file.
 
         Args:
             filename (str): Name of file to save running config to.
@@ -386,15 +431,15 @@
         Raises:
             NotImplementedError: Function currently not implemeneted.
         """
         raise NotImplementedError
 
     def close(self):
         """Implement ``pass``."""
-        pass
+        pass  # pylint: disable=unnecessary-pass
 
     def config(self, command):
         """Send command to device.
 
         Args:
             command (str): Command.
 
@@ -409,14 +454,15 @@
 
         Returns:
             float: Uptime of device.
         """
         if self._uptime is None:
             self._uptime = self._get_uptime()
 
+        log.debug("Host %s: Uptime %s.", self.host, self._uptime)
         return self._uptime
 
     @property
     def uptime_string(self):
         """
         Get uptime of device in format dd:hh:mm:ss.
 
@@ -524,17 +570,22 @@
         Raises:
             FileTransferError: Error in verifying if file existed before transfer.
         """
         if not self.file_copy_remote_exists(src, dest, **kwargs):
             self._check_free_space(min_space=6)
             self._upload_image(image_filepath=src)
             if not self.file_copy_remote_exists(src, dest, **kwargs):
-                raise FileTransferError(
-                    message="Attempted file copy, but could not validate file existed after transfer"
+                log.error(
+                    "Host %s: Attempted file copy, but could not validate file existed after transfer for file %s.",
+                    self.host,
+                    src,
                 )
+                raise FileTransferError
+
+        log.info("Host %s: File %s copied successfully.", self.host, src)
 
     # TODO: Make this an internal method since exposing file_copy should be sufficient
     def file_copy_remote_exists(self, src, dest=None, **kwargs):
         """Copy file to device.
 
         Args:
             src (str): Source of file.
@@ -543,22 +594,25 @@
         Raises:
             NotImplementedError: Destination must be ``/shared/images``.
 
         Returns:
             bool: True if image specified exists on device. Otherwise, false.
         """
         if dest and not dest.startswith("/shared/images"):
+            log.error("Host %s: Support only for images - destination is always /shared/images.", self.host)
             raise NotImplementedError("Support only for images - destination is always /shared/images")
 
         local_md5sum = self._file_copy_local_md5(filepath=src)
         file_basename = os.path.basename(src)
 
         if not self._image_match(image_name=file_basename, checksum=local_md5sum):
+            log.debug("Host %s: File %s does not already exist on remote.", self.host, src)
             return False
         else:
+            log.debug("Host %s: File %s already exists on remote.", self.host)
             return True
 
     def image_installed(self, image_name, volume):
         """Check if image is installed on specified volume.
 
         Args:
             image_name (str): Name of image.
@@ -587,16 +641,18 @@
             for _volume in volumes:
                 if (
                     _volume.name == volume
                     and _volume.version == image.version  # noqa W503
                     and _volume.basebuild == image.build  # noqa W503
                     and _volume.status == "complete"  # noqa W503
                 ):
+                    log.debug("Host %s: Image %s installed on volume %s.", self.host, image_name, volume)
                     return True
 
+        log.debug("Host %s: Image %s not installed on volume %s.", self.host, image_name, volume)
         return False
 
     def install_os(self, image_name, **vendor_specifics):
         """Install OS on device.
 
         Args:
             image_name (str): Image name.
@@ -607,33 +663,36 @@
         Returns:
             bool: True if image is installed successfully. Otherwise, false.
         """
         volume = vendor_specifics.get("volume")
         if not self.image_installed(image_name, volume):
             self._check_free_space(min_space=6)
             if not self._image_exists(image_name):
-                raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, dir="/shared/images")
+                log.error("Host %s: File not found for image %s and volume %s.", self.host, image_name, volume)
+                raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, directory="/shared/images")
             self._image_install(image_name=image_name, volume=volume)
             self._wait_for_image_installed(image_name=image_name, volume=volume)
 
+            log.info("Host %s: Image %s installed on volume %s.", self.host, image_name, volume)
             return True
 
+        log.info("Host %s: Image %s not installed on volume %s.", self.host, image_name, volume)
         return False
 
     def open(self):
         """Implement ``pass``."""
-        pass
+        pass  # pylint: disable=unnecessary-pass
 
-    def reboot(self, timer=0, volume=None, **kwargs):
+    def reboot(self, wait_for_reload=False, volume=None, **kwargs):
         """
         Reload the controller or controller pair.
 
         Args:
-            timer (int, optional): The time to wait before reloading. Defaults to 0.
             volume (str, optional): Active volume to reboot. Defaults to None.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
 
         Raises:
             RuntimeError: If device is unreachable after timeout period, raise an error.
 
         Example:
             >>> device = F5Device(**connection_args)
             >>> device.reboot()
@@ -646,28 +705,30 @@
             volume_name = None
         else:
             volume_name = volume
 
         self._reboot_to_volume(volume_name=volume_name)
 
         if not self._wait_for_device_reboot(volume_name=volume):
-            raise RuntimeError("Reboot to volume {} failed".format(volume))
+            log.error("Host %s: Reboot to volume %s failed.", self.host, volume)
+            raise RuntimeError(f"Reboot to volume {volume} failed")
+        log.debug("Host %s: Reboot to volume %s succeeded.", self.host, volume)
 
     def rollback(self, checkpoint_file):
-        """Rollback to checkpoint configurtion file.
+        """Rollback to checkpoint configuration file.
 
         Args:
             checkpoint_file (str): Name of checkpoint file.
 
         Raises:
             NotImplementedError: Function currently not implemented.
         """
         raise NotImplementedError
 
-    def running_config(self):
+    def running_config(self):  # pylint: disable=invalid-overridden-method
         """Get running configuration.
 
         Raises:
             NotImplementedError: Function currently not implemented.
         """
         raise NotImplementedError
 
@@ -690,30 +751,32 @@
 
         Raises:
             NTCFileNotFoundError: Error if file is not found on device.
         """
         volume = vendor_specifics.get("volume")
         self._check_free_space(min_space=6)
         if not self._image_exists(image_name):
-            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, dir="/shared/images")
+            log.error("Host %s: File not found for image %s and volume %s.", self.host, image_name, volume)
+            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, directory="/shared/images")
         self._image_install(image_name=image_name, volume=volume)
         self._wait_for_image_installed(image_name=image_name, volume=volume)
+        log.info("Host %s: Image %s installed to volume %s.", self.host, image_name, volume)
 
     def show(self, command, raw_text=False):
         """Run cli command on device.
 
         Args:
             command (str): Command to be ran.
             raw_text (bool, optional): Specifies if you want raw text. Defaults to False.
 
         Raises:
             NotImplementedError: [description]
         """
         raise NotImplementedError
 
-    def startup_config(self):
+    def startup_config(self):  # pylint: disable=invalid-overridden-method
         """Get startup configuration.
 
         Raises:
             NotImplementedError: Function currently not implemented.
         """
         raise NotImplementedError
```

### Comparing `pyntc-0.20.3/pyntc/devices/ios_device.py` & `pyntc-1.0.0/pyntc/devices/ios_device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Module for using a Cisco IOS device over SSH."""
 
 import os
 import re
-import signal
 import time
-import warnings
 
 from netmiko import ConnectHandler, FileTransfer
+from netmiko.exceptions import ReadTimeout
+
+from pyntc import log
+from pyntc.devices.base_device import BaseDevice, fix_docs, RollbackError
 from pyntc.errors import (
     CommandError,
     CommandListError,
     DeviceNotActiveError,
     FileSystemNotFoundError,
     FileTransferError,
     NTCError,
     NTCFileNotFoundError,
     OSInstallError,
     RebootTimeoutError,
     SocketClosedError,
 )
 from pyntc.utils import get_structured_data
 
-from .base_device import BaseDevice, fix_docs, RollbackError
-
 BASIC_FACTS_KM = {"model": "hardware", "os_version": "version", "serial_number": "serial", "hostname": "hostname"}
 RE_SHOW_REDUNDANCY = re.compile(
     r"^Redundant\s+System\s+Information\s*:\s*\n^-.+-\s*\n(?P<info>.+?)\n"
     r"^Current\s+Processor\s+Information\s*:\s*\n^-.+-\s*\n(?P<self>.+?$)\n"
     r"(?:Peer\s+Processor\s+Information\s*:\s*\n-.+-\s*\n(?P<other>.+)|Peer\s+\(slot:\s+\S+\).+)",
     re.DOTALL | re.MULTILINE,
 )
@@ -64,16 +64,17 @@
         self.secret = secret
         self.port = int(port)
         self.global_delay_factor = kwargs.get("global_delay_factor", 1)
         self.delay_factor = kwargs.get("delay_factor", 1)
         self._fast_cli = fast_cli
         self._connected = False
         self.open(confirm_active=confirm_active)
+        log.init(host=host)
 
-    def _check_command_output_for_errors(self, command, command_response):
+    def _check_command_output_for_errors(self, command, command_response):  # pylint: disable=no-self-use
         """
         Check response from device to see if an error was reported.
 
         Args:
             command (str): The command that was sent to the device.
 
         Raises:
@@ -90,27 +91,30 @@
             CommandError: ...
             >>>
         """
         if "% " in command_response or "Error:" in command_response:
             raise CommandError(command, command_response)
 
     def _enable(self):
-        warnings.warn("_enable() is deprecated; use enable().", DeprecationWarning)
+        log.warning("_enable() is deprecated; use enable().")
         self.enable()
+        log.debug("Host %s: Device enabled", self.host)
 
     def _enter_config(self):
         self.enable()
         self.native.config_mode()
+        log.debug("Host %s: Device entered config mode.", self.host)
 
     def _file_copy_instance(self, src, dest=None, file_system="flash:"):
         if dest is None:
             dest = os.path.basename(src)
 
-        fc = FileTransfer(self.native, src, dest, file_system=file_system)
-        return fc
+        file_copy = FileTransfer(self.native, src, dest, file_system=file_system)
+        log.debug("Host %s: File copy instance %s.", self.host, file_copy)
+        return file_copy
 
     def _get_file_system(self):
         """Determine the default file system or directory for device.
 
         Returns:
             str: The name of the default file system or directory for the device.
 
@@ -122,27 +126,31 @@
 
         # Attempt to gather file system
         while counter < SHOW_DIR_RETRY_COUNT:
             counter += 1
             raw_data = self.show("dir")
             try:
                 file_system = re.match(r"\s*.*?(\S+:)", raw_data).group(1)
+                log.debug("Host %s: File system %s.", self.host, file_system)
                 return file_system
             except AttributeError:
                 # Allow to continue through the loop
                 continue
 
+        log.error("host %s: File system not found with command 'dir'.")
         raise FileSystemNotFoundError(hostname=self.hostname, command="dir")
 
     # Get the version of the image that is booted into on the device
     def _image_booted(self, image_name, image_pattern=r".*\.(\d+\.\d+\.\w+)\.SPA.+", **vendor_specifics):
         version_data = self.show("show version")
         if re.search(image_name, version_data):
+            log.info("Host %s: Image %s booted successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: Image %s not booted successfully.", self.host, image_name)
         # Test for version number in the text, used on install mode devices that use packages.conf
         try:
             version_number = re.search(image_pattern, image_name).group(1)
             if version_number and version_number in version_data:
                 return True
         # Continue on if regex is unable to find the result, which raises an attribute error
         except AttributeError:
@@ -151,26 +159,29 @@
         # Unable to find the version number in output, the image is not booted.
         return False
 
     def _interfaces_detailed_list(self):
         ip_int_br_out = self.show("show ip int br")
         ip_int_br_data = get_structured_data("cisco_ios_show_ip_int_brief.template", ip_int_br_out)
 
+        log.debug("Host %s: interfaces detailed list %s.", self.host, ip_int_br_data)
         return ip_int_br_data
 
     def _is_catalyst(self):
         return self.model.startswith("WS-")
 
     def _raw_version_data(self):
         show_version_out = self.show("show version")
         try:
             version_data = get_structured_data("cisco_ios_show_version.template", show_version_out)[0]
         except IndexError:
+            log.error("Host %s: index error.", self.host)
             return {}
 
+        log.debug("Host %s: version data %s.", self.host, version_data)
         return version_data
 
     def _send_command(self, command, expect_string=None, **kwargs):
         # Set command args and assign the command to command_string argument
         command_args = {"command_string": command}
 
         # Check for an expect_string being passed in
@@ -179,25 +190,28 @@
 
         # Update command_args with additional arguments passed in, must be a valid Netmiko argument
         command_args.update(kwargs)
 
         response = self.native.send_command(**command_args)
 
         if "% " in response or "Error:" in response:
+            log.error("Host %s: Error in %s with response: %s", self.host, command, response)
             raise CommandError(command, response)
 
+        log.info("Host %s: Command %s was executed successfully with response: %s", self.host, command, response)
         return response
 
     def _show_vlan(self):
         show_vlan_out = self.show("show vlan")
         show_vlan_data = get_structured_data("cisco_ios_show_vlan.template", show_vlan_out)
 
+        log.debug("Host %s: Successfully executed command 'show vlan' with responses %s.", self.host, show_vlan_data)
         return show_vlan_data
 
-    def _uptime_components(self, uptime_full_string):
+    def _uptime_components(self, uptime_full_string):  # pylint: disable=no-self-use
         match_days = re.search(r"(\d+) days?", uptime_full_string)
         match_hours = re.search(r"(\d+) hours?", uptime_full_string)
         match_minutes = re.search(r"(\d+) minutes?", uptime_full_string)
 
         days = int(match_days.group(1)) if match_days else 0
         hours = int(match_hours.group(1)) if match_hours else 0
         minutes = int(match_minutes.group(1)) if match_minutes else 0
@@ -211,36 +225,45 @@
         seconds += hours * 60 * 60
         seconds += minutes * 60
 
         return seconds
 
     def _uptime_to_string(self, uptime_full_string):
         days, hours, minutes = self._uptime_components(uptime_full_string)
-        return "%02d:%02d:%02d:00" % (days, hours, minutes)
+        return f"{days:02d}:{hours:02d}:{minutes:02d}:00"
 
     def _wait_for_device_reboot(self, timeout=3600):
         start = time.time()
         while time.time() - start < timeout:
             try:
                 self.open()
                 self.show("show version")
-                return
-            except:  # noqa E722 # nosec
+                log.debug("Host %s: Device reboot Completed.", self.host)
+                if self._has_reload_happened_recently():
+                    return
+            except:  # noqa E722 # nosec  # pylint: disable=bare-except
                 pass
 
+        log.error("Host %s: Device timed out while rebooting.", self.host)
         raise RebootTimeoutError(hostname=self.hostname, wait_time=timeout)
 
+    def _has_reload_happened_recently(self):
+        if re.search(r"^00:00:0\d:*", self.uptime_string) is None:
+            self._uptime_string = None
+            return False
+        return True
+
     def backup_running_config(self, filename):
         """Backup running configuration to filename specified.
 
         Args:
             filename (str): Filename to save running configuration to.
         """
-        with open(filename, "w") as f:
-            f.write(self.running_config)
+        with open(filename, "w", encoding="utf-8") as file_name:
+            file_name.write(self.running_config)
 
     @property
     def boot_options(self):
         """Get current boot image.
 
         Returns:
             dict: Key ``sys`` with value being the current boot image.
@@ -254,15 +277,16 @@
             try:
                 # Try show boot if previous command was invalid
                 show_boot_out = self.show("show boot")
                 show_boot_out = show_boot_out.split("Boot Variables on next reload", 1)[-1]
             except CommandError:
                 # Default to running config value
                 show_boot_out = self.show("show run | inc boot")
-                boot_path_regex = r"boot\s+system\s+(?:\S+\s+|)(\S+)\s*$"
+                boot_path_regex = r"boot\ssystem\s\S+(?::+|\s)(\S+.bin)"
+                log.error("Host %s: Command error 'show boot'.", self.host)
 
         match = re.search(boot_path_regex, show_boot_out, re.MULTILINE)
         if match:
             boot_path_tuple = match.groups()
             # The regex match will return two values: the boot value and None
             # The return order will depend on which side of the `or` is matched in the regex
             boot_path = [value for value in boot_path_tuple if value is not None][0]
@@ -270,29 +294,32 @@
             boot_image = boot_path.replace(file_system, "")
             boot_image = boot_image.replace("/", "")
             boot_image = boot_image.split(",")[0]
             boot_image = boot_image.split(";")[0]
         else:
             boot_image = None
 
+        log.debug("Host %s: the boot options are {dict(sys=boot_image)}", self.host)
         return {"sys": boot_image}
 
     def checkpoint(self, checkpoint_file):
         """Create checkpoint file.
 
         Args:
             checkpoint_file (str): Name of checkpoint file.
         """
+        log.debug("Host %s: checkpoint is %s.", self.host, checkpoint_file)
         self.save(filename=checkpoint_file)
 
     def close(self):
         """Disconnect from device."""
         if self.connected:
             self.native.disconnect()
             self._connected = False
+            log.debug("Host %s: Connection closed.", self.host)
 
     def config(self, command, **netmiko_args):
         r"""
         Send config commands to device.
 
         By default, entering and exiting config mode is handled automatically.
         To disable entering and exiting config mode, pass `enter_config_mode` and `exit_config_mode` in ``**netmiko_args``.
@@ -320,15 +347,16 @@
             >>> device.config(["interface Gig0/1", "description x-connect"])
             ['host(config)#interface Gig0/1\nhost(config-if)#, 'description x-connect\nhost(config-if)#']
             >>>
         """
         # TODO: Remove this when deprecating config_list method
         original_command_is_str = isinstance(command, str)
 
-        if original_command_is_str:  # TODO: switch to isinstance(command, str) when removing above
+        # TODO: switch to isinstance(command, str) when removing above
+        if original_command_is_str:
             command = [command]
 
         original_exit_config_setting = netmiko_args.get("exit_config_mode")
         netmiko_args["exit_config_mode"] = False
         # Ignore None or invalid args passed for enter_config_mode
         if netmiko_args.get("enter_config_mode") is not False:
             self._enter_config()
@@ -339,63 +367,40 @@
         try:
             for cmd in command:
                 entered_commands.append(cmd)
                 command_response = self.native.send_config_set(cmd, **netmiko_args)
                 command_responses.append(command_response)
                 self._check_command_output_for_errors(cmd, command_response)
         except TypeError as err:
+            log.error("Host %s: Netmiko Driver's %s", self.host, err.args[0])
             raise TypeError(f"Netmiko Driver's {err.args[0]}")
         # TODO: Remove this when deprecating config_list method
         except CommandError as err:
             if not original_command_is_str:
+                log.error(
+                    "Host %s: Command error with commands: %s and error message %s",
+                    self.host,
+                    entered_commands,
+                    err.cli_error_msg,
+                )
                 raise CommandListError(entered_commands, cmd, err.cli_error_msg)
-            else:
-                raise err
+            raise err
         # Don't let exception prevent exiting config mode
         finally:
             # Ignore None or invalid args passed for exit_config_mode
             if original_exit_config_setting is not False:
                 self.native.exit_config_mode()
 
         # TODO: Remove this when deprecating config_list method
         if original_command_is_str:
             return command_responses[0]
 
+        log.info("Host %s: Device configured with command responses %s.", self.host, command_responses)
         return command_responses
 
-    def config_list(self, commands, **netmiko_args):  # noqa: D401
-        r"""
-        DEPRECATED - Use the `config` method.
-
-        Send config commands to device.
-
-        By default, entering and exiting config mode is handled automatically.
-        To disable entering and exiting config mode, pass `enter_config_mode` and `exit_config_mode` in ``**netmiko_args``.
-        This supports all arguments supported by Netmiko's `send_config_set` method using ``netmiko_args``.
-
-        Args:
-            commands (list): The commands to send to the device.
-            **netmiko_args: Any argument supported by ``netmiko.ConnectHandler.send_config_set``.
-
-        Returns:
-            list: Each command's input and output from sending the command in ``commands``.
-
-        Raises:
-            TypeError: When sending an argument in ``**netmiko_args`` that is not supported.
-            CommandListError: When one of the commands reports an error on the device.
-
-        Example:
-            >>> device = IOSDevice(**connection_args)
-            >>> device.config_list(["interface Gig0/1", "description x-connect"])
-            ['host(config)#interface Gig0/1\nhost(config-if)#, 'description x-connect\nhost(config-if)#']
-            >>>
-        """
-        warnings.warn("config_list() is deprecated; use config.", DeprecationWarning)
-        return self.config(commands, **netmiko_args)
-
     def confirm_is_active(self):
         """
         Confirm that the device is either standalone or the active device in a high availability cluster.
 
         Returns:
             bool: True when the device is considered active.
 
@@ -419,16 +424,23 @@
             True
             >>>
         """
         if not self.is_active():
             redundancy_state = self.redundancy_state
             peer_redundancy_state = self.peer_redundancy_state
             self.close()
+            log.error(
+                "Host %s: Device not active error with redundancy state %s and peer redundancy state %s",
+                self.host,
+                redundancy_state,
+                peer_redundancy_state,
+            )
             raise DeviceNotActiveError(self.host, redundancy_state, peer_redundancy_state)
 
+        log.debug("Host %s: Device is active.", self.host)
         return True
 
     @property
     def connected(self):  # noqa: D401
         """
         Get connection status of the device.
 
@@ -450,26 +462,29 @@
         # Netmiko reports enable and config mode as being enabled
         if not self.native.check_enable_mode():
             self.native.enable()
         # Ensure device is not in config mode
         if self.native.check_config_mode():
             self.native.exit_config_mode()
 
+        log.debug("Host %s: Device enabled.", self.host)
+
     @property
     def uptime(self):
         """Get uptime from device.
 
         Returns:
             int: Uptime in seconds.
         """
         if self._uptime is None:
             version_data = self._raw_version_data()
             uptime_full_string = version_data["uptime"]
             self._uptime = self._uptime_to_seconds(uptime_full_string)
 
+        log.debug("Host %s: Uptime %s", self.host, self._uptime)
         return self._uptime
 
     @property
     def uptime_string(self):
         """Get uptime in format dd:hh:mm.
 
         Returns:
@@ -489,27 +504,29 @@
         Returns:
             str: Hostname of device.
         """
         version_data = self._raw_version_data()
         if self._hostname is None:
             self._hostname = version_data["hostname"]
 
+        log.debug("Host %s: Hostname {self._hostname}", self.host)
         return self._hostname
 
     @property
     def interfaces(self):
         """
         Get list of interfaces on device.
 
         Returns:
             list: List of interfaces on device.
         """
         if self._interfaces is None:
             self._interfaces = list(x["intf"] for x in self._interfaces_detailed_list())
 
+        log.debug("Host %s: Interfaces %s", self.host, self._interfaces)
         return self._interfaces
 
     @property
     def vlans(self):
         """
         Get list of VLANs on device.
 
@@ -518,78 +535,84 @@
         """
         if self._vlans is None:
             if self.model.startswith("WS"):
                 self._vlans = list(str(x["vlan_id"]) for x in self._show_vlan())
             else:
                 self._vlans = []
 
+        log.debug("Host %s: Vlans %s", self.host, self._vlans)
         return self._vlans
 
     @property
     def fqdn(self):
         """Get fully qualified domain name.
 
         Returns:
             str: Fully qualified domain name or ``N/A`` if not defined.
         """
         if self._fqdn is None:
             self._fqdn = "N/A"
 
+        log.debug("Host %s: FQDN %s", self.host, self._fqdn)
         return self._fqdn
 
     @property
     def model(self):
         """Get the device model.
 
         Returns:
             str: Device model.
         """
         version_data = self._raw_version_data()
         if self._model is None:
             self._model = version_data["hardware"]
 
+        log.debug("Host %s: Model %s", self.host, self._model)
         return self._model
 
     @property
     def os_version(self):
         """Get os version on device.
 
         Returns:
             str: OS version on device.
         """
         version_data = self._raw_version_data()
         if self._os_version is None:
             self._os_version = version_data["version"]
 
+        log.debug("Host %s: OS version %s", self.host, self._os_version)
         return self._os_version
 
     @property
     def serial_number(self):
         """Get serial number of device.
 
         Returns:
             str: Serial number of device.
         """
         version_data = self._raw_version_data()
         if self._serial_number is None:
             self._serial_number = version_data["serial"]
 
+        log.debug("Host %s: Serial number %s", self.host, self._serial_number)
         return self._serial_number
 
     @property
     def config_register(self):
         """Get config register of device.
 
         Returns:
             str: Config register.
         """
         # ios-specific facts
         version_data = self._raw_version_data()
         self._config_register = version_data["config_register"]
 
+        log.debug("Host %s: Config register %s", self.host, self._config_register)
         return self._config_register
 
     @property
     def fast_cli(self):
         """Get current fast_cli value.
 
         Returns:
@@ -616,38 +639,45 @@
             FileTransferError: Error if unable to verify file was transferred successfully.
         """
         self.enable()
         if file_system is None:
             file_system = self._get_file_system()
 
         if not self.file_copy_remote_exists(src, dest, file_system):
-            fc = self._file_copy_instance(src, dest, file_system=file_system)
+            file_copy = self._file_copy_instance(src, dest, file_system=file_system)
             #        if not self.fc.verify_space_available():
             #            raise FileTransferError('Not enough space available.')
 
             try:
-                fc.enable_scp()
-                fc.establish_scp_conn()
-                fc.transfer_file()
+                file_copy.enable_scp()
+                file_copy.establish_scp_conn()
+                file_copy.transfer_file()
+                log.info("Host %s: File %s transferred successfully.", self.host, src)
             except OSError as error:
                 # compare hashes
-                if not fc.compare_md5():
+                if not file_copy.compare_md5():
+                    log.error("Host %s: Socket closed error %s", self.host, error)
                     raise SocketClosedError(message=error)
+                log.error("Host %s: OS error  %s", self.host, error)
             except:  # noqa E722
+                log.error("Host %s: File transfer error %s", self.host, FileTransferError.default_message)
                 raise FileTransferError
             finally:
-                fc.close_scp_chan()
+                file_copy.close_scp_chan()
 
             # Ensure connection to device is still open after long transfers
             self.open()
 
             if not self.file_copy_remote_exists(src, dest, file_system):
-                raise FileTransferError(
-                    message="Attempted file copy, but could not validate file existed after transfer"
+                log.error(
+                    "Host %s: Attempted file copy, but could not validate file existed after transfer %s",
+                    self.host,
+                    FileTransferError.default_message,
                 )
+                raise FileTransferError
 
     # TODO: Make this an internal method since exposing file_copy should be sufficient
     def file_copy_remote_exists(self, src, dest=None, file_system=None):
         """Copy file to device.
 
         Args:
             src (str): Source of file.
@@ -657,17 +687,20 @@
         Returns:
             bool: True if file copied succesfully and md5 hashes match. Otherwise, false.
         """
         self.enable()
         if file_system is None:
             file_system = self._get_file_system()
 
-        fc = self._file_copy_instance(src, dest, file_system=file_system)
-        if fc.check_file_exists() and fc.compare_md5():
+        file_copy = self._file_copy_instance(src, dest, file_system=file_system)
+        if file_copy.check_file_exists() and file_copy.compare_md5():
+            log.debug("Host %s: File %s already exists on remote.", self.host, src)
             return True
+
+        log.debug("Host %s: File %s does not already exist on remote.", self.host, src)
         return False
 
     def install_os(self, image_name, install_mode=False, install_mode_delay_factor=20, **vendor_specifics):
         """Installs the prescribed Network OS, which must be present before issuing this command.
 
         Args:
             image_name (str): Name of the IOS image to boot into
@@ -705,33 +738,41 @@
                     command = (
                         f"install add file {self._get_file_system()}{image_name} activate commit prompt-level none"
                     )
                     # Set a higher delay factor and send it in
                     try:
                         self.show(command, delay_factor=install_mode_delay_factor)
                     except IOError:
+                        log.error("Host %s: IO error for image %s", self.host, image_name)
                         pass
-
+                    except CommandError:
+                        command = f"request platform software package install switch all file {self._get_file_system()}{image_name} auto-copy"
+                        self.show(command, delay_factor=install_mode_delay_factor)
+                        self.reboot()
             else:
                 self.set_boot_options(image_name, **vendor_specifics)
                 self.reboot()
 
             # Wait for the reboot to finish
+            # TODO: This was moved into reboot method as well, should cause issues running again, but should be removed in future versions.
             self._wait_for_device_reboot(timeout=timeout)
 
             # Set FastCLI back to originally set when using install mode
             if install_mode:
                 self.fast_cli = current_fast_cli
-
+                image_name = INSTALL_MODE_FILE_NAME
             # Verify the OS level
             if not self._image_booted(image_name):
+                log.error("Host %s: OS install error for image %s", self.host, image_name)
                 raise OSInstallError(hostname=self.hostname, desired_boot=image_name)
 
+            log.info("Host %s: OS image %s installed successfully.", self.host, image_name)
             return True
 
+        log.info("Host %s: OS image %s not installed.", self.host, image_name)
         return False
 
     def is_active(self):
         """
         Determine if the current processor is the active processor.
 
         Returns:
@@ -771,15 +812,15 @@
             >>> device.connected
             True
             >>>
         """
         if self.connected:
             try:
                 self.native.find_prompt()
-            except:  # noqa E722
+            except:  # noqa E722  # pylint: disable=bare-except
                 self._connected = False
 
         if not self.connected:
             self.native = ConnectHandler(
                 device_type="cisco_ios",
                 ip=self.host,
                 username=self.username,
@@ -791,14 +832,16 @@
                 fast_cli=self.fast_cli,
             )
             self._connected = True
 
         if confirm_active:
             self.confirm_is_active()
 
+        log.debug("Host %s: Connection to controller was opened successfully.", self.host)
+
     @property
     def peer_redundancy_state(self):
         """
         Determine the current redundancy state of the peer processor.
 
         Returns:
             str: The redundancy state of the peer processor.
@@ -809,60 +852,58 @@
             >>> device.peer_redundancy_state
             'standby hot'
             >>>
         """
         try:
             show_redundancy = self.show("show redundancy")
         except CommandError:
+            log.error("Host %s: Command error for command 'show redundancy'.", self.host)
             return None
         re_show_redundancy = RE_SHOW_REDUNDANCY.match(show_redundancy.lstrip())
         processor_redundancy_info = re_show_redundancy.group("other")
         if processor_redundancy_info is not None:
             re_redundancy_state = RE_REDUNDANCY_STATE.search(processor_redundancy_info)
             processor_redundancy_state = re_redundancy_state.group(1).lower()
         else:
             processor_redundancy_state = "disabled"
+
+        log.debug("Host %s: Processor redundancy state %s.", self.host, processor_redundancy_state)
         return processor_redundancy_state
 
-    def reboot(self, timer=0, **kwargs):
+    def reboot(self, wait_for_reload=False, **kwargs):
         """Reboot device.
 
         Reload the controller or controller pair.
 
         Args:
-            timer (int): The time to wait before reloading.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
 
         Raises:
             ReloadTimeoutError: When the device is still unreachable after the timeout period.
         """
         if kwargs.get("confirm"):
-            warnings.warn("Passing 'confirm' to reboot method is deprecated.", DeprecationWarning)
-
-        def handler(signum, frame):
-            raise RebootSignal("Interrupting after reload")
-
-        signal.signal(signal.SIGALRM, handler)
-        signal.alarm(10)
+            log.warning("Passing 'confirm' to reboot method is deprecated.")
 
         try:
-            if timer > 0:
-                first_response = self.native.send_command_timing("reload in %d" % timer)
-            else:
-                first_response = self.native.send_command_timing("reload")
+            first_response = self.native.send_command_timing("reload")
 
             if "System configuration" in first_response:
                 self.native.send_command_timing("no")
 
-            self.native.send_command_timing("\n")
-        except RebootSignal:
-            signal.alarm(0)
-
-        signal.alarm(0)
-        # else:
-        #     print("Need to confirm reboot with confirm=True")
+            try:
+                self.native.send_command_timing("\n", read_timeout=10)
+            except ReadTimeout as expected_exception:
+                log.info("Host %s: Device rebooted.", self.host)
+                log.info("Hit expected exception during reload: %s", expected_exception.__class__)
+            if wait_for_reload:
+                time.sleep(10)
+                self._wait_for_device_reboot()
+        except Exception as err:
+            log.error(err)
+            log.error(err.__class__)
 
     @property
     def redundancy_mode(self):
         """
         Get operating redundancy mode of the device.
 
         Returns:
@@ -874,19 +915,21 @@
             >>> device.redundancy_mode
             'stateful switchover'
             >>>
         """
         try:
             show_redundancy = self.show("show redundancy")
         except CommandError:
+            log.error("Host %s: Command error for command 'show redundancy'.", self.host)
             return "n/a"
         re_show_redundancy = RE_SHOW_REDUNDANCY.match(show_redundancy.lstrip())
         redundancy_info = re_show_redundancy.group("info")
         re_redundancy_mode = RE_REDUNDANCY_OPERATION_MODE.search(redundancy_info)
         redundancy_mode = re_redundancy_mode.group(1).lower()
+        log.debug("Host %s: Redundancy mode is %s.", self.host, redundancy_mode)
         return redundancy_mode
 
     @property
     def redundancy_state(self):
         """
         Determine the current redundancy state of the processor.
 
@@ -899,141 +942,173 @@
             >>> device.redundancy_state
             'active'
             >>>
         """
         try:
             show_redundancy = self.show("show redundancy")
         except CommandError:
+            log.error("Host %s: Command error for command 'show redundancy'.", self.host)
             return None
         re_show_redundancy = RE_SHOW_REDUNDANCY.match(show_redundancy.lstrip())
         processor_redundancy_info = re_show_redundancy.group("self")
         re_redundancy_state = RE_REDUNDANCY_STATE.search(processor_redundancy_info)
         processor_redundancy_state = re_redundancy_state.group(1).lower()
+
+        log.debug("Host %s: Redundancy state is %s.", self.host, processor_redundancy_state)
         return processor_redundancy_state
 
     def rollback(self, rollback_to):
         """Rollback configuration to file on flash.
 
         Args:
             rollback_to (sEtr): Name of the file to rollback to.
 
         Raises:
             RollbackError: Error if unable to rollback to configuration.
         """
         try:
-            self.show("configure replace %s%s force" % (self._get_file_system(), rollback_to))
+            self.show(f"configure replace {self._get_file_system()}{rollback_to} force")
+            log.info("Host %s: Rollback to %s.", self.host, rollback_to)
         except CommandError:
-            raise RollbackError("Rollback unsuccessful. %s may not exist." % rollback_to)
+            log.error("Host %s: Rollback unsuccessful. %s may not exist.", self.host, rollback_to)
+            raise RollbackError(f"Rollback unsuccessful. {rollback_to} may not exist.")
 
     @property
     def running_config(self):
         """Get running configuration.
 
         Returns:
             str: Output of ``show running-config``.
         """
+        log.debug("Host %s: Show running config.", self.host)
         return self.show("show running-config")
 
     def save(self, filename="startup-config"):
         """Save running configuration.
 
         Args:
             filename (str, optional): Name of file to save running configuration. Defaults to "startup-config".
 
         Returns:
             bool: True if save is succesfull.
         """
-        command = "copy running-config %s" % filename
+        command = f"copy running-config {filename}"
         # Changed to send_command_timing to not require a direct prompt return.
         self.native.send_command_timing(command)
         # If the user has enabled 'file prompt quiet' which dose not require any confirmation or feedback.
         # This will send return without requiring an OK.
         # Send a return to pass the [OK]? message - Incease delay_factor for looking for response.
         self.native.send_command_timing("\n", delay_factor=2)
         # Confirm that we have a valid prompt again before returning.
         self.native.find_prompt()
+        log.debug("Host %s: Copy running config with name %s.", self.host, filename)
         return True
 
     def set_boot_options(self, image_name, **vendor_specifics):
         """Set specified image as boot image.
 
         Args:
             image_name (str): Name of image to set as boot variable.
 
         Raises:
             NTCFileNotFoundError: Error if file is not found on device.
             CommandError: Error if setting new image as boot variable fails.
         """
         file_system = vendor_specifics.get("file_system")
+        command = "boot system flash"
         if file_system is None:
             file_system = self._get_file_system()
 
-        file_system_files = self.show("dir {0}".format(file_system))
-        if re.search(image_name, file_system_files) is None:
-            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, dir=file_system)
-
-        try:
-            command = "boot system {0}/{1}".format(file_system, image_name)
-            self.config(["no boot system", command])
-        except CommandListError:  # TODO: Update to CommandError when deprecating config_list
-            file_system = file_system.replace(":", "")
-            command = "boot system {0} {1}".format(file_system, image_name)
+        file_system_files = self.show(f"dir {file_system}")
+        if image_name != INSTALL_MODE_FILE_NAME and re.search(image_name, file_system_files) is None:
+            log.error("Host %s: File not found error for image %s.", self.host, image_name)
+            raise NTCFileNotFoundError(hostname=self.hostname, file=image_name, directory=file_system)
+        if image_name == "packages.conf":
+            command = f"boot system {file_system}{image_name}"
             self.config(["no boot system", command])
+        else:
+            show_boot_sys = self.show("show run | include boot system")
+            # Sample:
+            # boot system flash:/c3560-advipservicesk9-mz.122-44.SE.bin
+            # boot system flash0:/c3560-advipservicesk9-mz.122-44.SE.bin
+            if re.search(r"boot\ssystem\s\S+\:\/\S+", show_boot_sys):
+                command = "boot system {0}/{1}".format(file_system, image_name)
+                self.config(["no boot system", command])
+            # Sample:
+            # boot system flash:c3560-advipservicesk9-mz.122-44.SE.bin
+            # boot system flash0:c3560-advipservicesk9-mz.122-44.SE.bin
+            elif re.search(r"boot\ssystem\s\S+\:\S+", show_boot_sys):
+                command = "boot system {0}{1}".format(file_system, image_name)
+                self.config(["no boot system", command])
+            # Sample:
+            # boot system flash flash:c3560-advipservicesk9-mz.122-44.SE.bin
+            # boot system flash flash0:c3560-advipservicesk9-mz.122-44.SE.bin
+            # boot system flash bootflash:c3560-advipservicesk9-mz.122-44.SE.bin
+            elif re.search(
+                r"boot\ssystem\s\S+\s\S+:\S+", show_boot_sys
+            ):  # TODO: Update to CommandError when deprecating config_list
+                command = "boot system flash {0}{1}".format(file_system, image_name)
+                self.config(["no boot system", command])
+            # Sample:
+            # boot system flash c3560-advipservicesk9-mz.122-44.SE.bin
+            elif re.search(
+                r"boot\ssystem\sflash\s\S+", show_boot_sys
+            ):  # TODO: Update to CommandError when deprecating config_list
+                file_system = file_system.replace(":", "")
+                command = "boot system {0} {1}".format(file_system, image_name)
+                self.config(["no boot system", command])
+            else:
+                raise CommandError(
+                    command=command,
+                    message="Unable to determine the boot system configuration syntax. Current config is {0}".format(
+                        show_boot_sys
+                    ),
+                )
 
         self.save()
         new_boot_options = self.boot_options["sys"]
         if new_boot_options != image_name:
+            log.error("Host %s: Setting boot command did not yield expected results", self.host)
             raise CommandError(
                 command=command,
-                message="Setting boot command did not yield expected results, found {0}".format(new_boot_options),
+                message=f"Setting boot command did not yield expected results, found {new_boot_options}",
             )
 
     def show(self, command, expect_string=None, **netmiko_args):
         """Run command on device.
 
         Args:
             command (str): Command to be ran.
             expect_string (str, optional): Expected string from command output. Defaults to None.
 
         Returns:
             str: Output of command.
         """
         self.enable()
-        return self._send_command(command, expect_string=expect_string, **netmiko_args)
-
-    def show_list(self, commands):
-        """Run a list of commands on device.
-
-        Args:
-            commands (list): List of commands to run on device.
-
-        Raises:
-            CommandListError: Error if one of the commands is not able to be ran on the device.
-
-        Returns:
-            list: Responses from each command ran on device.
-        """
-        self.enable()
-
-        responses = []
-        entered_commands = []
-        for command in commands:
-            entered_commands.append(command)
-            try:
-                responses.append(self._send_command(command))
-            except CommandError as e:
-                raise CommandListError(entered_commands, command, e.cli_error_msg)
+        if isinstance(command, list):
+            responses = []
+            entered_commands = []
+            for command_instance in command:
+                entered_commands.append(command_instance)
+                try:
+                    responses.append(self._send_command(command_instance))
+                except CommandError as e:
+                    raise CommandListError(entered_commands, command_instance, e.cli_error_msg)
 
-        return responses
+            return responses
+        return self._send_command(command, expect_string=expect_string, **netmiko_args)
 
     @property
     def startup_config(self):
         """Get startup configuration.
 
         Returns:
             str: Startup configuration from device.
         """
+        log.debug("Host %s: Successfully executed command 'show startup-config'.", self.host)
         return self.show("show startup-config")
 
 
 class RebootSignal(NTCError):  # noqa: D101
-    pass
+    """RebootSignal."""
+
+    pass  # pylint: disable=unnecessary-pass
```

### Comparing `pyntc-0.20.3/pyntc/devices/jnpr_device.py` & `pyntc-1.0.0/pyntc/devices/jnpr_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import re
 import time
 import warnings
 from tempfile import NamedTemporaryFile
 
 from jnpr.junos import Device as JunosNativeDevice
 from jnpr.junos.exception import ConfigLoadError
-from jnpr.junos.op.ethport import EthPortTable
+from jnpr.junos.op.ethport import EthPortTable  # pylint: disable=no-name-in-module
 from jnpr.junos.utils.config import Config as JunosNativeConfig
 from jnpr.junos.utils.fs import FS as JunosNativeFS
 from jnpr.junos.utils.scp import SCP
 from jnpr.junos.utils.sw import SW as JunosNativeSW
-from pyntc.errors import CommandError, CommandListError, FileTransferError, RebootTimeoutError
 
-from .base_device import BaseDevice, fix_docs
-from .tables.jnpr.loopback import LoopbackTable
+from pyntc.devices.base_device import BaseDevice, fix_docs
+from pyntc.devices.tables.jnpr.loopback import LoopbackTable
+from pyntc.errors import CommandError, CommandListError, FileTransferError, RebootTimeoutError
 
 
 @fix_docs
 class JunosDevice(BaseDevice):
     """Juniper JunOS Device Implementation."""
 
     vendor = "juniper"
@@ -33,30 +33,30 @@
             username (str): The username to authenticate with the device.
             password (str): The password to authenticate with the device.
         """
         super().__init__(host, username, password, *args, device_type="juniper_junos_netconf", **kwargs)
 
         self.native = JunosNativeDevice(*args, host=host, user=username, passwd=password, **kwargs)
         self.open()
-        self.cu = JunosNativeConfig(self.native)
-        self.fs = JunosNativeFS(self.native)
-        self.sw = JunosNativeSW(self.native)
+        self.cu = JunosNativeConfig(self.native)  # pylint: disable=invalid-name
+        self.fs = JunosNativeFS(self.native)  # pylint: disable=invalid-name
+        self.sw = JunosNativeSW(self.native)  # pylint: disable=invalid-name
 
-    def _file_copy_local_file_exists(self, filepath):
+    def _file_copy_local_file_exists(self, filepath):  # pylint: disable=no-self-use
         return os.path.isfile(filepath)
 
     def _file_copy_local_md5(self, filepath, blocksize=2**20):
         if self._file_copy_local_file_exists(filepath):
-            m = hashlib.md5()  # nosec
-            with open(filepath, "rb") as f:
-                buf = f.read(blocksize)
+            md5_hash = hashlib.md5()  # nosec
+            with open(filepath, "rb") as file_name:
+                buf = file_name.read(blocksize)
                 while buf:
-                    m.update(buf)
-                    buf = f.read(blocksize)
-            return m.hexdigest()
+                    md5_hash.update(buf)
+                    buf = file_name.read(blocksize)
+            return md5_hash.hexdigest()
 
     def _file_copy_remote_md5(self, filename):
         return self.fs.checksum(filename)
 
     def _get_interfaces(self):
         eth_ifaces = EthPortTable(self.native)
         eth_ifaces.get()
@@ -68,15 +68,15 @@
         ifaces.extend(loop_ifaces.keys())
 
         return ifaces
 
     def _image_booted(self, image_name, **vendor_specifics):
         raise NotImplementedError
 
-    def _uptime_components(self, uptime_full_string):
+    def _uptime_components(self, uptime_full_string):  # pylint: disable=no-self-use
         match_days = re.search(r"(\d+) days?", uptime_full_string)
         match_hours = re.search(r"(\d+) hours?", uptime_full_string)
         match_minutes = re.search(r"(\d+) minutes?", uptime_full_string)
         match_seconds = re.search(r"(\d+) seconds?", uptime_full_string)
 
         days = int(match_days.group(1)) if match_days else 0
         hours = int(match_hours.group(1)) if match_hours else 0
@@ -92,35 +92,35 @@
         seconds += hours * 60 * 60
         seconds += minutes * 60
 
         return seconds
 
     def _uptime_to_string(self, uptime_full_string):
         days, hours, minutes, seconds = self._uptime_components(uptime_full_string)
-        return "%02d:%02d:%02d:%02d" % (days, hours, minutes, seconds)
+        return f"{days:02d}:{hours:02d}:{minutes:02d}:{seconds:02d}"
 
     def _wait_for_device_reboot(self, timeout=3600):
         start = time.time()
         while time.time() - start < timeout:
             try:
                 self.open()
                 return
-            except:  # noqa E722 # nosec
+            except:  # noqa E722 # nosec  # pylint: disable=bare-except
                 pass
 
         raise RebootTimeoutError(hostname=self.hostname, wait_time=timeout)
 
     def backup_running_config(self, filename):
         """Backup current running configuration.
 
         Args:
             filename (str): Name used for backup file.
         """
-        with open(filename, "w") as f:
-            f.write(self.running_config)
+        with open(filename, "w", encoding="utf-8") as file_name:
+            file_name.write(self.running_config)
 
     @property
     def boot_options(self):
         """Get os version on device.
 
         Returns:
             str: OS version on device.
@@ -136,51 +136,39 @@
         self.save(filename)
 
     def close(self):
         """Close connection to device."""
         if self.connected:
             self.native.close()
 
-    def config(self, commands, format="set"):
+    def config(self, commands, format_type="set"):
         """Send configuration commands to a device.
 
         Args:
-             commands (str, list): String with single command, or list with multiple commands.
+            commands (str, list): String with single command, or list with multiple commands.
 
         Raises:
-             ConfigLoadError: Issue with loading the command.
-             CommandError: Issue with the command provided, if its a single command, passed in as a string.
-             CommandListError: Issue with a command in the list provided.
+            ConfigLoadError: Issue with loading the command.
+            CommandError: Issue with the command provided, if its a single command, passed in as a string.
+            CommandListError: Issue with a command in the list provided.
         """
         if isinstance(commands, str):
             try:
-                self.cu.load(commands, format=format)
+                self.cu.load(commands, format_type=format_type)
                 self.cu.commit()
-            except ConfigLoadError as e:
-                raise CommandError(commands, e.message)
+            except ConfigLoadError as err:
+                raise CommandError(commands, err.message)
         else:
             try:
                 for command in commands:
-                    self.cu.load(command, format=format)
+                    self.cu.load(command, format_type=format_type)
 
                 self.cu.commit()
-            except ConfigLoadError as e:
-                raise CommandListError(commands, command, e.message)
-
-    def config_list(self, commands, format="set"):
-        """Send configuration commands in list format to a device.
-
-        DEPRECATED - Use the `config` method.
-
-        Args:
-            commands (list): List with multiple commands.
-            format (str): The Junos format the commands are in.
-        """
-        warnings.warn("config_list() is deprecated; use config().", DeprecationWarning)
-        self.config(commands, format=format)
+            except ConfigLoadError as err:
+                raise CommandListError(commands, command, err.message)
 
     @property
     def connected(self):
         """Get connection status of device.
 
         Returns:
             bool: True if connection is active. Otherwise, false.
@@ -349,41 +337,44 @@
         raise NotImplementedError
 
     def open(self):
         """Open connection to device."""
         if not self.connected:
             self.native.open()
 
-    def reboot(self, timer=0, **kwargs):
+    def reboot(self, wait_for_reload=False, **kwargs):
         """
         Reload the controller or controller pair.
 
         Args:
-            timer (int, optional): The time to wait before reloading. Defaults to 0.
+            wait_for_reload: Whether or not reboot method should also run _wait_for_device_reboot(). Defaults to False.
 
         Example:
             >>> device = JunosDevice(**connection_args)
             >>> device.reboot()
             >>>
         """
         if kwargs.get("confirm"):
             warnings.warn("Passing 'confirm' to reboot method is deprecated.", DeprecationWarning)
 
         self.sw = JunosNativeSW(self.native)
-        self.sw.reboot(in_min=timer)
+        self.sw.reboot(in_min=0)
+        if wait_for_reload:
+            time.sleep(10)
+            self._wait_for_device_reboot()
 
     def rollback(self, filename):
         """Rollback to a specific configuration file.
 
         Args:
             filename (str): Filename to rollback device to.
         """
         self.native.timeout = 60
 
-        temp_file = NamedTemporaryFile()
+        temp_file = NamedTemporaryFile()  # pylint: disable=consider-using-with
 
         with SCP(self.native) as scp:
             scp.get(filename, local_path=temp_file.name)
 
         self.cu.load(path=temp_file.name, format="text", overwrite=True)
         self.cu.commit()
 
@@ -412,15 +403,15 @@
         Returns:
             bool: True if new file created for save file. Otherwise, just returns if save is to default name.
         """
         if filename is None:
             self.cu.commit()
             return
 
-        temp_file = NamedTemporaryFile()
+        temp_file = NamedTemporaryFile()  # pylint: disable=consider-using-with
         temp_file.write(self.show("show config"))
         temp_file.flush()
 
         with SCP(self.native) as scp:
             scp.put(temp_file.name, remote_path=filename)
 
         temp_file.close()
@@ -459,26 +450,14 @@
 
             response = self.native.cli(command, warning=False)
             responses.append(response)
         if original_commands_is_str:
             return responses[0]
         return responses
 
-    def show_list(self, commands, raw_text=True):
-        """Send show commands in list format to a device.
-
-        DEPRECATED - Use the `show` method.
-
-        Args:
-            commands (list): List with multiple commands.
-            raw_text (bool): Return raw text or structured text.
-        """
-        warnings.warn("show_list() is deprecated; use show().", DeprecationWarning)
-        return self.show(commands)
-
     @property
     def startup_config(self):
         """Get startup configuration.
 
         Returns:
             str: Startup configuration.
         """
```

### Comparing `pyntc-0.20.3/pyntc/devices/system_features/vlans/base_vlans.py` & `pyntc-1.0.0/pyntc/devices/system_features/vlans/base_vlans.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if vlan_id < lower or vlan_id > upper:
         raise VlanNotInRangeError(lower, upper)
 
 
 class BaseVlans(BaseFeature):
     """Subclass for base vlan feature."""
 
-    pass
+    pass  # pylint: disable=unnecessary-pass
 
 
 class VlanNotInRangeError(NTCError):
     """Vlan error.
 
     Args:
         NTCError (str): Vlan range error.
@@ -27,8 +27,8 @@
     def __init__(self, lower, upper):
         """Exception for vlan range validation.
 
         Args:
             lower (int): lower vlan range.
             upper (int): upper vlan range.
         """
-        super().__init__("Vlan Id must be in range %s-%s" % (lower, upper))
+        super().__init__(f"Vlan Id must be in range {lower}-{upper}")
```

### Comparing `pyntc-0.20.3/pyntc/devices/system_features/vlans/eos_vlans.py` & `pyntc-1.0.0/pyntc/devices/system_features/vlans/eos_vlans.py`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/pyntc/devices/tables/jnpr/loopback.yml` & `pyntc-1.0.0/pyntc/devices/tables/jnpr/loopback.yml`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/pyntc/errors.py` & `pyntc-1.0.0/pyntc/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 """pyntc custom exceptions."""
 import warnings
 
 
 class NTCError(Exception):
     """Generic Error class for PyNTC."""
 
-    def __init__(self, message):
+    def __init__(self, message):  # pylint: disable=super-init-not-called
         """
         Generic Error class for PyNTC.
 
         Args:
             message (str): The error message associated with the Exception.
         """
         self.message = message
 
     def __repr__(self):
         """Representation of NTC error object."""
-        return "%s: \n%s" % (self.__class__.__name__, self.message)
+        return f"{self.__class__.__name__}: \n{self.message}"
 
     __str__ = __repr__
 
 
 class UnsupportedDeviceError(NTCError):
     """Error class for Unsupported Devices."""
 
     def __init__(self, vendor):
         """
         Error class for Unsupported Devices.
 
         Args:
             vendor (str): The name of the deice's vendor to present in the error.
         """
-        message = "%s is not a supported vendor." % vendor
+        message = f"{vendor} is not a supported vendor."
         super().__init__(message)
 
 
 class DeviceNameNotFoundError(NTCError):
     """Error for issues finding ``name`` in inventory file, ``filename``."""
 
     def __init__(self, name, filename):
         """
         Error for issues finding ``name`` in inventory file, ``filename``.
 
         Args:
             name (str): The hostname that failed the lookup.
             filename (str): The name of the file used for inventory.
         """
-        message = "Name %s not found in %s. The file may not exist." % (name, filename)
+        message = f"Name {name} not found in {filename}. The file may not exist."
         super().__init__(message)
 
 
 class ConfFileNotFoundError(NTCError):
     """Error for issues finding the config ``filename``."""
 
     def __init__(self, filename):
         """
         Error for issues finding the config ``filename``.
 
         Args:
             filename (str): The name of the file used for config settings.
         """
-        message = "NTC Configuration file %s could not be found." % filename
+        message = f"NTC Configuration file {filename} could not be found."
         super().__init__(message)
 
 
 class CommandError(NTCError):
     """Error for issuing ``command`` on device."""
 
     def __init__(self, command, message):
@@ -73,15 +73,15 @@
 
         Args:
             command (str): The command that failed.
             message (str): The error message returned from the device.
         """
         self.command = command
         self.cli_error_msg = message
-        message = "Command %s was not successful: %s" % (command, message)
+        message = f"Command {command} was not successful: {message}"
         super().__init__(message)
 
 
 class CommandListError(NTCError):
     """Error for issuing a ``command`` from a list of ``commands`` on device.."""
 
     def __init__(self, commands, command, message):
@@ -92,18 +92,18 @@
             commands (list): The list of commands that were to be sent to the device.
             command (str): The command that reported an error on the device.
             message (str): The error emssage returned from the device.
         """
         warnings.warn("This will raise CommandError in the future", FutureWarning)
         self.commands = commands
         self.command = command
-        message = "\nCommand %s failed with message: %s" % (command, message)
+        message = f"\nCommand {command} failed with message: {message}"
         message += "\nCommand List: \n"
-        for command in commands:
-            message += "\t%s\n" % command
+        for command in commands:  # pylint: disable=redefined-argument-from-local
+            message += f"\t{command}\n"
         super().__init__(message)
 
 
 class DeviceNotActiveError(NTCError):
     """Error for when the device is part of an HA cluster, and the device is not the active device."""
 
     def __init__(self, hostname, redundancy_state, peer_redundancy_state):
@@ -131,30 +131,30 @@
 
         Args:
             feature (str): The PyNTC feature name.
             device_type (str): The PyNTC device_type name.
 
         TODO: Remove this Exception when VLAN feature is removed.
         """
-        message = "%s feature not found for %s device type." % (feature, device_type)
+        message = f"{feature} feature not found for {device_type} device type."
         super().__init__(message)
 
 
 class FileSystemNotFoundError(NTCError):
     """Error for inability to identify the default file system on network device."""
 
     def __init__(self, hostname, command):
         """
         Error for inability to identify the default file system on network device.
 
         Args:
             hostname (str): The hostname of the device that failed.
             command (str): The command used to detect the default file system.
         """
-        message = 'Unable to parse "{0}" command to identify the default file system on {1}.'.format(command, hostname)
+        message = f'Unable to parse "{command}" command to identify the default file system on {hostname}.'
         super().__init__(message)
 
 
 class FileTransferError(NTCError):
     """File Transfer Error."""
 
     default_message = (
@@ -179,62 +179,60 @@
         """
         Error for inability to log into device after waiting for max time for reboot to complete.
 
         Args:
             hostname (str): The hostname of the device that did not boot back up.
             wait_time (int): The amount of time waiting before considering the reboot failed.
         """
-        message = "Unable to reconnect to {0} after {1} seconds".format(hostname, wait_time)
+        message = f"Unable to reconnect to {hostname} after {wait_time} seconds"
         super().__init__(message)
 
 
 class WaitingRebootTimeoutError(NTCError):
     """Error for device not rebooting after sending install mode upgrade command."""
 
     def __init__(self, hostname, wait_time):
         """
         Error for device not rebooting after sending install mode upgrade command.
 
         Args:
             hostname (str): The hostname of the device that did not boot back up.
             wait_time (int): The amount of time waiting before considering the reboot failed.
         """
-        message = "{0} has not rebooted in {1} seconds after issuing install mode upgrade command".format(
-            hostname, wait_time
-        )
+        message = f"{hostname} has not rebooted in {wait_time} seconds after issuing install mode upgrade command"
         super().__init__(message)
 
 
 class NotEnoughFreeSpaceError(NTCError):
     """Error for not having enough free space to transfer a file."""
 
     def __init__(self, hostname, min_space):
         """
         Error for not having enough free space to transfer a file.
 
         Args:
             hostname (str): The hostname of the device that did not boot back up.
             min_space (str): The minimum amount of space required to transfer the file.
         """
-        message = "{0} does not meet the minimum disk space requirements of {1}".format(hostname, min_space)
+        message = f"{hostname} does not meet the minimum disk space requirements of {min_space}"
         super().__init__(message)
 
 
 class OSInstallError(NTCError):
     """Error for failing to install an OS on a device."""
 
     def __init__(self, hostname, desired_boot):
         """
         Error for failing to install an OS on a device.
 
         Args:
             hostname (str): The hostname of the device that failed to install OS.
             desired_boot (str): The OS that was attempted to be installed.
         """
-        message = "{0} was unable to boot into {1}".format(hostname, desired_boot)
+        message = f"{hostname} was unable to boot into {desired_boot}"
         super().__init__(message)
 
 
 class PeerFailedToFormError(NTCError):
     """Error for failing to have High Availability Peer form after state change."""
 
     def __init__(self, hostname, desired_state, current_state):
@@ -252,26 +250,25 @@
         )
         super().__init__(message)
 
 
 class NTCFileNotFoundError(NTCError):
     """Error for not being able to find a file on a device."""
 
-    def __init__(self, hostname, file, dir):
-        """
-        Error for not being able to find a file on a device.
+    def __init__(self, hostname, file, directory):
+        """Error for not being able to find a file on a device.
 
         Args:
             hostname (str): The hostname of the device that did not have the ``file``.
             file (str): The name of the file that could not be found.
-            dir (str): The directory on the network device where the file was searched for.
+            directory (str): The directory on the network device where the file was searched for.
 
         TODO: Rename ``dir`` arg as that is a reserved name in python.
         """
-        message = "{0} was not found in {1} on {2}".format(file, dir, hostname)
+        message = f"{file} was not found in {directory} on {hostname}"
         super().__init__(message)
 
 
 class SocketClosedError(NTCError):
     """Error for network device closing the socket connection during operation."""
 
     default_message = (
```

### Comparing `pyntc-0.20.3/pyntc/utils/converters.py` & `pyntc-1.0.0/pyntc/utils/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Provides methods for manipulating and converting data."""
 
 
-def convert_dict_by_key(original, key_map, fill_in=False, whitelist=[], blacklist=[]):
+def convert_dict_by_key(
+    original, key_map, fill_in=False, whitelist=[], blacklist=[]
+):  # pylint: disable=dangerous-default-value
     """Use a key map to convert a dictionary to desired keys.
 
     Args:
         original (dict): Original dictionary to be converted.
         key_map (dict): Key map to use to convert dictionary.
         fill_in (dict): Whether the returned dictionary should contain
             keys and values from the original dictionary if not specified in the key map.
@@ -37,15 +39,17 @@
         for original_key in original_key_subset:
             if original_key in original:
                 converted[original_key] = original[original_key]
 
     return converted
 
 
-def convert_list_by_key(original_list, key_map, fill_in=False, whitelist=[], blacklist=[]):
+def convert_list_by_key(
+    original_list, key_map, fill_in=False, whitelist=[], blacklist=[]
+):  # pylint: disable=dangerous-default-value
     """Apply a list conversion for all items in original_list.
 
     Args:
         original_list (list): Original list to be converted.
         key_map (dict): Key map to use to convert list.
         fill_in (dict): Whether the returned list should contain
             keys and values from the original dictionary if not specified in the key map.
```

### Comparing `pyntc-0.20.3/pyntc/utils/templates/__init__.py` & `pyntc-1.0.0/pyntc/utils/templates/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         template_name (str): Name of template to use.
         rawtxt (str): Raw output from device.
 
     Returns:
         list: A dict per entry returned by TextFSM.
     """
     template_file = get_template(template_name)
-    with open(template_file) as template:
+    with open(template_file, encoding="utf-8") as template:
         fsm = textfsm.TextFSM(template)
         table = fsm.ParseText(rawtxt)
 
         structured_data = []
         for row in table:
             entry = {fsm.header[index].lower(): element for index, element in enumerate(row)}
             structured_data.append(entry)
```

### Comparing `pyntc-0.20.3/pyntc/utils/templates/cisco_asa_show_version.template` & `pyntc-1.0.0/pyntc/utils/templates/cisco_asa_show_version.template`

 * *Files identical despite different names*

### Comparing `pyntc-0.20.3/pyproject.toml` & `pyntc-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntc"
-version = "v0.20.3"
+version = "v1.0.0"
 description = "SDK to simplify common workflows for Network Devices."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://pyntc.readthedocs.io"
 repository = "https://github.com/networktocode/pyntc"
 documentation = "https://pyntc.readthedocs.io"
@@ -89,27 +89,38 @@
   )/
   | settings.py     # This is where you define files that should not be stylized by black
                      # the root of the project
 )
 '''
 
 [tool.pylint.master]
-ignore=".venv"
+ignore=[".venv", "tests"]
 
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
 disable = """,
-    line-too-long,
+    abstract-method,
+    arguments-differ,
+    arguments-renamed,
+    attribute-defined-outside-init,
     bad-continuation,
-    consider-iterating-dictionary
+    consider-iterating-dictionary,
+    duplicate-code,
+    inconsistent-return-statements,
+    line-too-long,
+    raise-missing-from,
+    too-many-arguments,
+    too-many-instance-attributes,
+    too-many-lines,
+    too-many-public-methods,
     """
 
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
```

### Comparing `pyntc-0.20.3/PKG-INFO` & `pyntc-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntc
-Version: 0.20.3
+Version: 1.0.0
 Summary: SDK to simplify common workflows for Network Devices.
 Home-page: https://pyntc.readthedocs.io
 License: Apache-2.0
 Keywords: network,os-upgrades,network devices
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyntc Version: 0.20.3 Summary: SDK to simplify
+Metadata-Version: 2.1 Name: pyntc Version: 1.0.0 Summary: SDK to simplify
 common workflows for Network Devices. Home-page: https://pyntc.readthedocs.io
 License: Apache-2.0 Keywords: network,os-upgrades,network devices Author:
 Network to Code, LLC Author-email: info@networktocode.com Requires-Python:
 >=3.7,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

