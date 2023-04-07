# Comparing `tmp/MistressGPT-0.9.8.tar.gz` & `tmp/MistressGPT-0.9.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MistressGPT-0.9.8.tar", last modified: Fri Apr  7 19:02:38 2023, max compression
+gzip compressed data, was "MistressGPT-0.9.85.tar", last modified: Fri Apr  7 19:15:52 2023, max compression
```

## Comparing `MistressGPT-0.9.8.tar` & `MistressGPT-0.9.85.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.378495 MistressGPT-0.9.8/
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.374806 MistressGPT-0.9.8/MistressGPT.egg-info/
--rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)      674 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/SOURCES.txt
--rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/dependency_links.txt
--rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/entry_points.txt
--rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/requires.txt
--rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/top_level.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 19:02:38.378371 MistressGPT-0.9.8/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)     1261 2023-04-06 00:01:40.000000 MistressGPT-0.9.8/README.md
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.376546 MistressGPT-0.9.8/chatmistress/
--rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.8/chatmistress/__init__.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.377509 MistressGPT-0.9.8/chatmistress/assets/
--rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/Kelpy-Codos.js
--rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/custom.css
--rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/custom.js
--rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/favicon.ico
--rw-r--r--   0 huzi       (501) staff       (20)     4502 2023-04-07 17:58:59.000000 MistressGPT-0.9.8/chatmistress/chatmistress.py
--rw-r--r--   0 huzi       (501) staff       (20)     8510 2023-04-07 18:40:41.000000 MistressGPT-0.9.8/chatmistress/core.py
--rw-r--r--   0 huzi       (501) staff       (20)      359 2023-04-07 17:59:28.000000 MistressGPT-0.9.8/chatmistress/gui_debug.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.377914 MistressGPT-0.9.8/chatmistress/roles/
--rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.8/chatmistress/roles/landlady.yml
--rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.8/chatmistress/roles/wife.yml
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.378174 MistressGPT-0.9.8/chatmistress/templates/
--rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.8/chatmistress/templates/role_play_summary.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.8/chatmistress/templates/role_play_sys.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.8/chatmistress/utils.py
--rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.8/chatmistress/webbot.py
--rw-r--r--   0 huzi       (501) staff       (20)    21013 2023-04-07 19:00:44.000000 MistressGPT-0.9.8/chatmistress/webbot2.py
--rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 19:02:38.378534 MistressGPT-0.9.8/setup.cfg
--rw-r--r--   0 huzi       (501) staff       (20)      819 2023-04-07 19:02:19.000000 MistressGPT-0.9.8/setup.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.519818 MistressGPT-0.9.85/
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.515617 MistressGPT-0.9.85/MistressGPT.egg-info/
+-rw-r--r--   0 huzi       (501) staff       (20)     1421 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)      674 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/entry_points.txt
+-rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/requires.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 19:15:52.000000 MistressGPT-0.9.85/MistressGPT.egg-info/top_level.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1421 2023-04-07 19:15:52.519662 MistressGPT-0.9.85/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)     1266 2023-04-07 19:10:07.000000 MistressGPT-0.9.85/README.md
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.517394 MistressGPT-0.9.85/chatmistress/
+-rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.85/chatmistress/__init__.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.518355 MistressGPT-0.9.85/chatmistress/assets/
+-rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.85/chatmistress/assets/Kelpy-Codos.js
+-rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.85/chatmistress/assets/custom.css
+-rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.85/chatmistress/assets/custom.js
+-rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.85/chatmistress/assets/favicon.ico
+-rw-r--r--   0 huzi       (501) staff       (20)     4502 2023-04-07 17:58:59.000000 MistressGPT-0.9.85/chatmistress/chatmistress.py
+-rw-r--r--   0 huzi       (501) staff       (20)     8510 2023-04-07 18:40:41.000000 MistressGPT-0.9.85/chatmistress/core.py
+-rw-r--r--   0 huzi       (501) staff       (20)      359 2023-04-07 17:59:28.000000 MistressGPT-0.9.85/chatmistress/gui_debug.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.518790 MistressGPT-0.9.85/chatmistress/roles/
+-rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.85/chatmistress/roles/landlady.yml
+-rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.85/chatmistress/roles/wife.yml
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:15:52.519333 MistressGPT-0.9.85/chatmistress/templates/
+-rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.85/chatmistress/templates/role_play_summary.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.85/chatmistress/templates/role_play_sys.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.85/chatmistress/utils.py
+-rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.85/chatmistress/webbot.py
+-rw-r--r--   0 huzi       (501) staff       (20)    21223 2023-04-07 19:15:23.000000 MistressGPT-0.9.85/chatmistress/webbot2.py
+-rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 19:15:52.519863 MistressGPT-0.9.85/setup.cfg
+-rw-r--r--   0 huzi       (501) staff       (20)      825 2023-04-07 19:15:43.000000 MistressGPT-0.9.85/setup.py
```

### Comparing `MistressGPT-0.9.8/MistressGPT.egg-info/PKG-INFO` & `MistressGPT-0.9.85/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1
-Name: MistressGPT
-Version: 0.9.8
-Summary: MistressGPT: 基于GPT3.5的女王聊天室
-Description-Content-Type: text/markdown
-
-# MistressGPT: 基于 GPT3.5 的女王聊天室
+# MistressGPT: 基于 GPT3.5 的女王聊天室 👠
 
 ## 介绍
 
 安装
 
 ```
 pip install MistressGPT
```

### Comparing `MistressGPT-0.9.8/MistressGPT.egg-info/SOURCES.txt` & `MistressGPT-0.9.85/MistressGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/PKG-INFO` & `MistressGPT-0.9.85/MistressGPT.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: MistressGPT
-Version: 0.9.8
-Summary: MistressGPT: 基于GPT3.5的女王聊天室
+Version: 0.9.85
+Summary: MistressGPT: 基于GPT3.5的女王聊天室 👠
 Description-Content-Type: text/markdown
 
-# MistressGPT: 基于 GPT3.5 的女王聊天室
+# MistressGPT: 基于 GPT3.5 的女王聊天室 👠
 
 ## 介绍
 
 安装
 
 ```
 pip install MistressGPT
```

### Comparing `MistressGPT-0.9.8/README.md` & `MistressGPT-0.9.85/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# MistressGPT: 基于 GPT3.5 的女王聊天室
+Metadata-Version: 2.1
+Name: MistressGPT
+Version: 0.9.85
+Summary: MistressGPT: 基于GPT3.5的女王聊天室 👠
+Description-Content-Type: text/markdown
+
+# MistressGPT: 基于 GPT3.5 的女王聊天室 👠
 
 ## 介绍
 
 安装
 
 ```
 pip install MistressGPT
```

### Comparing `MistressGPT-0.9.8/chatmistress/assets/Kelpy-Codos.js` & `MistressGPT-0.9.85/chatmistress/assets/Kelpy-Codos.js`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/assets/custom.css` & `MistressGPT-0.9.85/chatmistress/assets/custom.css`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/assets/favicon.ico` & `MistressGPT-0.9.85/chatmistress/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/chatmistress.py` & `MistressGPT-0.9.85/chatmistress/chatmistress.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/core.py` & `MistressGPT-0.9.85/chatmistress/core.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/roles/landlady.yml` & `MistressGPT-0.9.85/chatmistress/roles/landlady.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/roles/wife.yml` & `MistressGPT-0.9.85/chatmistress/roles/wife.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/templates/role_play_summary.txt` & `MistressGPT-0.9.85/chatmistress/templates/role_play_summary.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/templates/role_play_sys.txt` & `MistressGPT-0.9.85/chatmistress/templates/role_play_sys.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/utils.py` & `MistressGPT-0.9.85/chatmistress/utils.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/webbot.py` & `MistressGPT-0.9.85/chatmistress/webbot.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.8/chatmistress/webbot2.py` & `MistressGPT-0.9.85/chatmistress/webbot2.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,16 @@
 HISTORY_DIR = "history"
 TEMPLATES_DIR = "templates"
 
 asset_dir = Path(__file__).parent / 'assets'
 with open(asset_dir / "custom.css", "r", encoding="utf-8") as f:
     customCSS = f.read()
 
-title = """<h1 align="left" style="min-width:200px; margin-top:6px; white-space: nowrap;">MistressGPT</h1>"""
+page_title = "MistressGPT 👠"
+title = f"""<h1 align="left" style="min-width:200px; margin-top:6px; white-space: nowrap;">{page_title}</h1>"""
 
 
 footer = """\
 <div class="versions">{versions}</div>
 """
 
 
@@ -179,16 +180,16 @@
     chat_info_res = wrap_init_chat_components(
         role_info, temperature, top_p, max_token_limit, debug=False)
 
     if chatbot is None:
         return chat_info_res, systemPromptTxt
     else:
         # 重置对话
-        # chat_info, systemPromptTxt, chatbot, history
-        return chat_info_res, systemPromptTxt, gr.Chatbot.update(label=role_name_selected, value=[]), [], role_name_selected
+        # chat_info, systemPromptTxt, chatbot, history, role_name_selected, status_bar_text
+        return chat_info_res, systemPromptTxt, gr.Chatbot.update(label=role_name_selected, value=[]), [], role_name_selected, f'已选择角色: {role_name_selected}'
 
 
 def get_templates(role_cards, plain=False):
     """
     从网上或者本地文件获取模板列表.
     TODO: 默认情况下从本地和网上获取模板列表
     """
@@ -249,15 +250,15 @@
 
 def load_chat_history(downloadFile, systemPromptTxt, history, chatbot, user_name):
     saveFileName = ''
     return saveFileName, systemPromptTxt, history, chatbot
 
 
 def reset_default():
-    status_display = ""
+    status_display = "默认设置已经恢复"
     return TOP_P, TEMPERATURE, status_display
 
 
 def start_outputing():
     logging.debug("显示取消按钮，隐藏发送按钮")
     return gr.Button.update(visible=False), gr.Button.update(visible=True)
 
@@ -283,15 +284,15 @@
     msg = f"API密钥更改为了{hide_middle_chars(key)}"
     logging.info(msg)
     return key, msg, gr.update(interactive=True), gr.Button.update(visible=True)
 
 
 def reset_state():
     logging.info("重置状态")
-    status_display = ""
+    status_display = "重置完成"
     return [], [], [], status_display
 
 
 def transfer_input(inputs, chatbot):
     # 一次性返回，降低延迟
     textbox = reset_textbox()
     chatbot.append([inputs, None])
@@ -329,22 +330,22 @@
         chat_info['selected_model'] = selected_model
         chat_info['openai_api_key'] = openai_api_key
 
         parsed_response = wrap_interact(chat_info, inputs)
         chatbot[-1][1] = f'({parsed_response.pose}): {parsed_response.line}'
 
     history.append(copy.deepcopy(chatbot[-1]))
-    status_display = ""
+    status_display = "返回成功"
     token_count = all_token_counts + [1]
 
     return chatbot, history, status_display, token_count
 
 
 def creat_gui_chat(roles: Dict[str, RoleInfo], debug=False, max_token_limit=2000):
-    with gr.Blocks(css=customCSS, theme=small_and_beautiful_theme) as demo:
+    with gr.Blocks(css=customCSS, theme=small_and_beautiful_theme, title=page_title) as demo:
         my_api_key = os.getenv("OPENAI_API_KEY", None)
         user_name = gr.State(DEFAULT_USERNAME)
         history = gr.State([])
         token_count = gr.State([])
         role_cards = gr.State(roles)
         role_selected = gr.State('Hello')
         chat_info = gr.State("")
@@ -522,16 +523,19 @@
         user_input.submit(**transfer_input_args).then(**
                                                       chatgpt_predict_args).then(**end_outputing_args)
 
         submitBtn.click(**transfer_input_args).then(**
                                                     chatgpt_predict_args).then(**end_outputing_args)
 
         creat_chat_args = dict(
-            fn=read_template_create_chat, inputs=[chat_info, role_selected, temperature, top_p, role_cards, templateSelectDropdown,
-                                                  systemPromptTxt, chatbot], outputs=[chat_info, systemPromptTxt, chatbot, history, role_selected]
+            fn=read_template_create_chat,
+            inputs=[chat_info, role_selected, temperature, top_p, role_cards, templateSelectDropdown,
+                    systemPromptTxt, chatbot],
+            outputs=[chat_info, systemPromptTxt,
+                     chatbot, history, role_selected, status_display]
         )
 
         emptyBtn.click(
             reset_state,
             outputs=[chatbot, history, token_count, status_display],
             show_progress=True,
         ).then(show_progress=True, **creat_chat_args)
```

### Comparing `MistressGPT-0.9.8/setup.py` & `MistressGPT-0.9.85/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='MistressGPT',
-    description='MistressGPT: 基于GPT3.5的女王聊天室',
+    description='MistressGPT: 基于GPT3.5的女王聊天室 👠',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.8',
+    version='0.9.85',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'mistressgpt=chatmistress.chatmistress:main'
         ]
     },
     package_data={
```

