# Comparing `tmp/MistressGPT-0.9.7.tar.gz` & `tmp/MistressGPT-0.9.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MistressGPT-0.9.7.tar", last modified: Fri Apr  7 00:59:50 2023, max compression
+gzip compressed data, was "MistressGPT-0.9.71.tar", last modified: Fri Apr  7 18:35:46 2023, max compression
```

## Comparing `MistressGPT-0.9.7.tar` & `MistressGPT-0.9.71.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.224013 MistressGPT-0.9.7/
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.219078 MistressGPT-0.9.7/MistressGPT.egg-info/
--rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)      648 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/SOURCES.txt
--rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/dependency_links.txt
--rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/entry_points.txt
--rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/requires.txt
--rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 00:59:50.000000 MistressGPT-0.9.7/MistressGPT.egg-info/top_level.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 00:59:50.223850 MistressGPT-0.9.7/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)     1261 2023-04-06 00:01:40.000000 MistressGPT-0.9.7/README.md
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.220623 MistressGPT-0.9.7/chatmistress/
--rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.7/chatmistress/__init__.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.222474 MistressGPT-0.9.7/chatmistress/assets/
--rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.7/chatmistress/assets/Kelpy-Codos.js
--rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.7/chatmistress/assets/custom.css
--rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.7/chatmistress/assets/custom.js
--rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.7/chatmistress/assets/favicon.ico
--rw-r--r--   0 huzi       (501) staff       (20)     4508 2023-04-07 00:55:36.000000 MistressGPT-0.9.7/chatmistress/chatmistress.py
--rw-r--r--   0 huzi       (501) staff       (20)     8871 2023-04-05 23:52:03.000000 MistressGPT-0.9.7/chatmistress/core.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.222952 MistressGPT-0.9.7/chatmistress/roles/
--rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.7/chatmistress/roles/landlady.yml
--rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.7/chatmistress/roles/wife.yml
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 00:59:50.223517 MistressGPT-0.9.7/chatmistress/templates/
--rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.7/chatmistress/templates/role_play_summary.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.7/chatmistress/templates/role_play_sys.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.7/chatmistress/utils.py
--rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.7/chatmistress/webbot.py
--rw-r--r--   0 huzi       (501) staff       (20)    20647 2023-04-06 00:30:48.000000 MistressGPT-0.9.7/chatmistress/webbot2.py
--rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 00:59:50.224056 MistressGPT-0.9.7/setup.cfg
--rw-r--r--   0 huzi       (501) staff       (20)      819 2023-04-07 00:59:26.000000 MistressGPT-0.9.7/setup.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.344758 MistressGPT-0.9.71/
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.340565 MistressGPT-0.9.71/MistressGPT.egg-info/
+-rw-r--r--   0 huzi       (501) staff       (20)     1411 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)      674 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/entry_points.txt
+-rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/requires.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/top_level.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1411 2023-04-07 18:35:46.344642 MistressGPT-0.9.71/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)     1261 2023-04-06 00:01:40.000000 MistressGPT-0.9.71/README.md
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.342112 MistressGPT-0.9.71/chatmistress/
+-rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.71/chatmistress/__init__.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.343329 MistressGPT-0.9.71/chatmistress/assets/
+-rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/Kelpy-Codos.js
+-rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/custom.css
+-rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/custom.js
+-rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/favicon.ico
+-rw-r--r--   0 huzi       (501) staff       (20)     4502 2023-04-07 17:58:59.000000 MistressGPT-0.9.71/chatmistress/chatmistress.py
+-rw-r--r--   0 huzi       (501) staff       (20)     8925 2023-04-07 18:28:08.000000 MistressGPT-0.9.71/chatmistress/core.py
+-rw-r--r--   0 huzi       (501) staff       (20)      359 2023-04-07 17:59:28.000000 MistressGPT-0.9.71/chatmistress/gui_debug.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.343833 MistressGPT-0.9.71/chatmistress/roles/
+-rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.71/chatmistress/roles/landlady.yml
+-rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.71/chatmistress/roles/wife.yml
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.344362 MistressGPT-0.9.71/chatmistress/templates/
+-rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.71/chatmistress/templates/role_play_summary.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.71/chatmistress/templates/role_play_sys.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.71/chatmistress/utils.py
+-rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.71/chatmistress/webbot.py
+-rw-r--r--   0 huzi       (501) staff       (20)    20828 2023-04-07 18:33:53.000000 MistressGPT-0.9.71/chatmistress/webbot2.py
+-rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 18:35:46.344792 MistressGPT-0.9.71/setup.cfg
+-rw-r--r--   0 huzi       (501) staff       (20)      820 2023-04-07 18:35:35.000000 MistressGPT-0.9.71/setup.py
```

### Comparing `MistressGPT-0.9.7/MistressGPT.egg-info/PKG-INFO` & `MistressGPT-0.9.71/MistressGPT.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistressGPT
-Version: 0.9.7
+Version: 0.9.71
 Summary: MistressGPT: 基于GPT3.5的女王聊天室
 Description-Content-Type: text/markdown
 
 # MistressGPT: 基于 GPT3.5 的女王聊天室
 
 ## 介绍
```

### Comparing `MistressGPT-0.9.7/MistressGPT.egg-info/SOURCES.txt` & `MistressGPT-0.9.71/MistressGPT.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MistressGPT.egg-info/dependency_links.txt
 MistressGPT.egg-info/entry_points.txt
 MistressGPT.egg-info/requires.txt
 MistressGPT.egg-info/top_level.txt
 chatmistress/__init__.py
 chatmistress/chatmistress.py
 chatmistress/core.py
+chatmistress/gui_debug.py
 chatmistress/utils.py
 chatmistress/webbot.py
 chatmistress/webbot2.py
 chatmistress/assets/Kelpy-Codos.js
 chatmistress/assets/custom.css
 chatmistress/assets/custom.js
 chatmistress/assets/favicon.ico
```

### Comparing `MistressGPT-0.9.7/PKG-INFO` & `MistressGPT-0.9.71/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistressGPT
-Version: 0.9.7
+Version: 0.9.71
 Summary: MistressGPT: 基于GPT3.5的女王聊天室
 Description-Content-Type: text/markdown
 
 # MistressGPT: 基于 GPT3.5 的女王聊天室
 
 ## 介绍
```

### Comparing `MistressGPT-0.9.7/README.md` & `MistressGPT-0.9.71/README.md`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/assets/Kelpy-Codos.js` & `MistressGPT-0.9.71/chatmistress/assets/Kelpy-Codos.js`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/assets/custom.css` & `MistressGPT-0.9.71/chatmistress/assets/custom.css`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/assets/favicon.ico` & `MistressGPT-0.9.71/chatmistress/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/chatmistress.py` & `MistressGPT-0.9.71/chatmistress/chatmistress.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 @click.command()
 @click.argument('cmd', type=click.Choice(['cli', 'gui']))
 @click.option('--debug', default=False, help='Debug mode if True')
 @click.option('--max-token-limit', default=1000, help='temperature for openai')
 @click.option('--ext-url', default=None, help='外部模板URL')
-@click.option('--concurrency', default=20, help='外部模板URL')
+@click.option('--concurrency', default=20, help='并发数')
 @click.option('--inbrowser', default=True, help='是否开启浏览器')
 @click.option('--server-name', default=None, help='是否外网可用')
 def main(cmd, debug, max_token_limit, ext_url, concurrency, inbrowser, server_name):
     assert cmd in ('cli', 'gui')
 
     if 'OPENAI_API_KEY' not in os.environ:
         os.environ['OPENAI_API_KEY'] = input(
```

### Comparing `MistressGPT-0.9.7/chatmistress/core.py` & `MistressGPT-0.9.71/chatmistress/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 import click
+import openai
 import xmltodict
 import json
 import yaml
 from dotenv import load_dotenv
 from langchain.chains import ConversationChain
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import (
@@ -211,14 +212,15 @@
     if top_p is not None:
         conversation.llm.model_kwargs['top_p'] = top_p
         conversation.memory.sum_chain.llm.top_p = top_p
     if temperature is not None:
         conversation.llm.model_kwargs['temperature'] = temperature
         conversation.memory.sum_chain.llm.temperature = temperature
     if openai_api_key is not None:
+        openai.api_key = openai_api_key
         conversation.llm.openai_api_key = openai_api_key
         conversation.memory.sum_chain.llm.openai_api_key = openai_api_key
 
     with console.status("loading..."):
         res = conversation.predict(
             input=user_input, summary=memory.existing_summary)
         if debug:
```

### Comparing `MistressGPT-0.9.7/chatmistress/roles/landlady.yml` & `MistressGPT-0.9.71/chatmistress/roles/landlady.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/roles/wife.yml` & `MistressGPT-0.9.71/chatmistress/roles/wife.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/templates/role_play_summary.txt` & `MistressGPT-0.9.71/chatmistress/templates/role_play_summary.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/templates/role_play_sys.txt` & `MistressGPT-0.9.71/chatmistress/templates/role_play_sys.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/utils.py` & `MistressGPT-0.9.71/chatmistress/utils.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/webbot.py` & `MistressGPT-0.9.71/chatmistress/webbot.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.7/chatmistress/webbot2.py` & `MistressGPT-0.9.71/chatmistress/webbot2.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     pass
 
 
 def submit_key(key):
     key = key.strip()
     msg = f"API密钥更改为了{hide_middle_chars(key)}"
     logging.info(msg)
-    return key, msg
+    return key, msg, gr.update(interactive=True), gr.Button.update(visible=True)
 
 
 def reset_state():
     logging.info("重置状态")
     status_display = ""
     return [], [], [], status_display
 
@@ -307,14 +307,15 @@
     all_token_counts,
     top_p,
     temperature,
     debug=False,
     selected_model=MODELS[0],
     should_check_token_count=True,
 ):
+    logging.info(f'本次消息发送的APIKEY为{openai_api_key}')
     # outputing = start_outputing()
     debug = False
     if debug:
         time.sleep(0.1)
         chatbot[-1][1] = f'input is {inputs}'
     else:
         chat_info['temperature'] = temperature
@@ -524,16 +525,17 @@
         emptyBtn.click(
             reset_state,
             outputs=[chatbot, history, token_count, status_display],
             show_progress=True,
         ).then(show_progress=True, **creat_chat_args)
         emptyBtn.click(**reset_textbox_args)
 
-        # ChatGPT
-        keyTxt.change(submit_key, keyTxt, [user_api_key, status_display])
+        # 重置API-key
+        keyTxt.change(submit_key, keyTxt, [
+                      user_api_key, status_display, user_input, submitBtn])
 
         # 重新获取所有模板
         get_all_templates_args = dict(
             fn=get_templates, inputs=[role_cards], outputs=[
                 templateSelectDropdown]
         )
```

### Comparing `MistressGPT-0.9.7/setup.py` & `MistressGPT-0.9.71/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='MistressGPT',
     description='MistressGPT: 基于GPT3.5的女王聊天室',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.7',
+    version='0.9.71',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'mistressgpt=chatmistress.chatmistress:main'
         ]
     },
     package_data={
```

