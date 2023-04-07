# Comparing `tmp/MistressGPT-0.9.71.tar.gz` & `tmp/MistressGPT-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MistressGPT-0.9.71.tar", last modified: Fri Apr  7 18:35:46 2023, max compression
+gzip compressed data, was "MistressGPT-0.9.8.tar", last modified: Fri Apr  7 19:02:38 2023, max compression
```

## Comparing `MistressGPT-0.9.71.tar` & `MistressGPT-0.9.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.344758 MistressGPT-0.9.71/
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.340565 MistressGPT-0.9.71/MistressGPT.egg-info/
--rw-r--r--   0 huzi       (501) staff       (20)     1411 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)      674 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/SOURCES.txt
--rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/dependency_links.txt
--rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/entry_points.txt
--rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/requires.txt
--rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 18:35:46.000000 MistressGPT-0.9.71/MistressGPT.egg-info/top_level.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1411 2023-04-07 18:35:46.344642 MistressGPT-0.9.71/PKG-INFO
--rw-r--r--   0 huzi       (501) staff       (20)     1261 2023-04-06 00:01:40.000000 MistressGPT-0.9.71/README.md
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.342112 MistressGPT-0.9.71/chatmistress/
--rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.71/chatmistress/__init__.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.343329 MistressGPT-0.9.71/chatmistress/assets/
--rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/Kelpy-Codos.js
--rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/custom.css
--rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/custom.js
--rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.71/chatmistress/assets/favicon.ico
--rw-r--r--   0 huzi       (501) staff       (20)     4502 2023-04-07 17:58:59.000000 MistressGPT-0.9.71/chatmistress/chatmistress.py
--rw-r--r--   0 huzi       (501) staff       (20)     8925 2023-04-07 18:28:08.000000 MistressGPT-0.9.71/chatmistress/core.py
--rw-r--r--   0 huzi       (501) staff       (20)      359 2023-04-07 17:59:28.000000 MistressGPT-0.9.71/chatmistress/gui_debug.py
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.343833 MistressGPT-0.9.71/chatmistress/roles/
--rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.71/chatmistress/roles/landlady.yml
--rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.71/chatmistress/roles/wife.yml
-drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 18:35:46.344362 MistressGPT-0.9.71/chatmistress/templates/
--rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.71/chatmistress/templates/role_play_summary.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.71/chatmistress/templates/role_play_sys.txt
--rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.71/chatmistress/utils.py
--rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.71/chatmistress/webbot.py
--rw-r--r--   0 huzi       (501) staff       (20)    20828 2023-04-07 18:33:53.000000 MistressGPT-0.9.71/chatmistress/webbot2.py
--rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 18:35:46.344792 MistressGPT-0.9.71/setup.cfg
--rw-r--r--   0 huzi       (501) staff       (20)      820 2023-04-07 18:35:35.000000 MistressGPT-0.9.71/setup.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.378495 MistressGPT-0.9.8/
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.374806 MistressGPT-0.9.8/MistressGPT.egg-info/
+-rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)      674 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 huzi       (501) staff       (20)        1 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       63 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/entry_points.txt
+-rw-r--r--   0 huzi       (501) staff       (20)      102 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/requires.txt
+-rw-r--r--   0 huzi       (501) staff       (20)       13 2023-04-07 19:02:38.000000 MistressGPT-0.9.8/MistressGPT.egg-info/top_level.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1410 2023-04-07 19:02:38.378371 MistressGPT-0.9.8/PKG-INFO
+-rw-r--r--   0 huzi       (501) staff       (20)     1261 2023-04-06 00:01:40.000000 MistressGPT-0.9.8/README.md
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.376546 MistressGPT-0.9.8/chatmistress/
+-rw-r--r--   0 huzi       (501) staff       (20)        0 2023-03-30 05:12:33.000000 MistressGPT-0.9.8/chatmistress/__init__.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.377509 MistressGPT-0.9.8/chatmistress/assets/
+-rw-r--r--   0 huzi       (501) staff       (20)     2956 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/Kelpy-Codos.js
+-rw-r--r--   0 huzi       (501) staff       (20)     8644 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/custom.css
+-rw-r--r--   0 huzi       (501) staff       (20)       25 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/custom.js
+-rw-r--r--   0 huzi       (501) staff       (20)    15406 2023-04-02 06:57:10.000000 MistressGPT-0.9.8/chatmistress/assets/favicon.ico
+-rw-r--r--   0 huzi       (501) staff       (20)     4502 2023-04-07 17:58:59.000000 MistressGPT-0.9.8/chatmistress/chatmistress.py
+-rw-r--r--   0 huzi       (501) staff       (20)     8510 2023-04-07 18:40:41.000000 MistressGPT-0.9.8/chatmistress/core.py
+-rw-r--r--   0 huzi       (501) staff       (20)      359 2023-04-07 17:59:28.000000 MistressGPT-0.9.8/chatmistress/gui_debug.py
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.377914 MistressGPT-0.9.8/chatmistress/roles/
+-rw-r--r--   0 huzi       (501) staff       (20)      758 2023-03-30 00:07:04.000000 MistressGPT-0.9.8/chatmistress/roles/landlady.yml
+-rw-r--r--   0 huzi       (501) staff       (20)      964 2023-03-30 04:46:54.000000 MistressGPT-0.9.8/chatmistress/roles/wife.yml
+drwxr-xr-x   0 huzi       (501) staff       (20)        0 2023-04-07 19:02:38.378174 MistressGPT-0.9.8/chatmistress/templates/
+-rw-r--r--   0 huzi       (501) staff       (20)     1104 2023-03-30 00:08:37.000000 MistressGPT-0.9.8/chatmistress/templates/role_play_summary.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1113 2023-03-30 00:27:26.000000 MistressGPT-0.9.8/chatmistress/templates/role_play_sys.txt
+-rw-r--r--   0 huzi       (501) staff       (20)     1239 2023-04-06 02:40:08.000000 MistressGPT-0.9.8/chatmistress/utils.py
+-rw-r--r--   0 huzi       (501) staff       (20)     1876 2023-03-30 05:13:12.000000 MistressGPT-0.9.8/chatmistress/webbot.py
+-rw-r--r--   0 huzi       (501) staff       (20)    21013 2023-04-07 19:00:44.000000 MistressGPT-0.9.8/chatmistress/webbot2.py
+-rw-r--r--   0 huzi       (501) staff       (20)       38 2023-04-07 19:02:38.378534 MistressGPT-0.9.8/setup.cfg
+-rw-r--r--   0 huzi       (501) staff       (20)      819 2023-04-07 19:02:19.000000 MistressGPT-0.9.8/setup.py
```

### Comparing `MistressGPT-0.9.71/MistressGPT.egg-info/PKG-INFO` & `MistressGPT-0.9.8/MistressGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistressGPT
-Version: 0.9.71
+Version: 0.9.8
 Summary: MistressGPT: 基于GPT3.5的女王聊天室
 Description-Content-Type: text/markdown
 
 # MistressGPT: 基于 GPT3.5 的女王聊天室
 
 ## 介绍
```

### Comparing `MistressGPT-0.9.71/MistressGPT.egg-info/SOURCES.txt` & `MistressGPT-0.9.8/MistressGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/PKG-INFO` & `MistressGPT-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistressGPT
-Version: 0.9.71
+Version: 0.9.8
 Summary: MistressGPT: 基于GPT3.5的女王聊天室
 Description-Content-Type: text/markdown
 
 # MistressGPT: 基于 GPT3.5 的女王聊天室
 
 ## 介绍
```

### Comparing `MistressGPT-0.9.71/README.md` & `MistressGPT-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/assets/Kelpy-Codos.js` & `MistressGPT-0.9.8/chatmistress/assets/Kelpy-Codos.js`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/assets/custom.css` & `MistressGPT-0.9.8/chatmistress/assets/custom.css`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/assets/favicon.ico` & `MistressGPT-0.9.8/chatmistress/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/chatmistress.py` & `MistressGPT-0.9.8/chatmistress/chatmistress.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/core.py` & `MistressGPT-0.9.8/chatmistress/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 import copy
 from pathlib import Path
 from typing import Dict, List, Optional, Union
-import click
 import openai
+import logging
 import xmltodict
 import json
-import yaml
-from dotenv import load_dotenv
 from langchain.chains import ConversationChain
 from langchain.chat_models import ChatOpenAI
-from langchain.memory import (
-    ConversationSummaryBufferMemory,
-    ChatMessageHistory,
-    ConversationBufferMemory,
-    ConversationBufferWindowMemory,
-    ConversationSummaryMemory,
-    ConversationKGMemory)
+from langchain.memory import ConversationBufferWindowMemory
 from langchain.output_parsers import (OutputFixingParser, PydanticOutputParser,
                                       RetryWithErrorOutputParser)
 from langchain.schema import HumanMessage, AIMessage
 from langchain import PromptTemplate, OpenAI
-from prompt_toolkit import PromptSession
-from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
-from prompt_toolkit.completion import WordCompleter
-from prompt_toolkit.history import InMemoryHistory, FileHistory
 from langchain.chains.llm import LLMChain
 from pydantic import BaseModel, Field
 from rich.console import Console
-from .utils import fetch_template, load_roles, RoleInfo
+from .utils import RoleInfo
 
 
 class DummyConsole:
     def __init__(self):
         pass
 
     def __enter__(self):
@@ -54,25 +42,24 @@
     sum_chain: LLMChain
     llm: ChatOpenAI
     mistress_name: str
     user_role: str
     existing_summary: str = ''
     max_token_limit: int = 1000
     debug: bool = False
-    # parser: PydanticOutputParser = parser
 
     @property
     def memory_variables(self) -> List[str]:
         return [self.memory_key] + self.other_input_keys
 
     def summrize_lines(self):
         buffer = self.chat_memory.messages
         curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
         if self.debug:
-            print(
+            logging.debug(
                 f"len(buffer)={len(buffer)}, curr_buffer_length={curr_buffer_length}")
         if curr_buffer_length > self.max_token_limit:
             pruned_memory = []
             while curr_buffer_length > self.max_token_limit:
                 pruned_memory.append(buffer.pop(0))
                 curr_buffer_length = self.llm.get_num_tokens_from_messages(
                     buffer)
@@ -180,18 +167,19 @@
     fix_parser = OutputFixingParser.from_llm(parser=parser, llm=llm)
     retry_parser = RetryWithErrorOutputParser.from_llm(parser=parser, llm=llm)
     return conversation, prompt, memory, parser, fix_parser, retry_parser
 
 
 def parse_llm_output(output, parser, fix_parser, retry_parser, prompt_value: str):
     try:
-        output = json.dumps(xmltodict.parse(output)['res'], ensure_ascii=False)
-        parsed_response = parser.parse(output)
+        outputjson = json.dumps(xmltodict.parse(
+            output)['res'], ensure_ascii=False)
+        parsed_response = parser.parse(outputjson)
     except:
-        print('发生错误，再次解析')
+        logging.error(f'发生错误，再次解析. Original output: {output}')
         # avoid using retry_parser.
         # parsed_response = retry_parser.parse_with_prompt(
         #     output, prompt_value)
         parsed_response = fix_parser.parse(output)
 
     return parsed_response
 
@@ -220,15 +208,15 @@
         conversation.llm.openai_api_key = openai_api_key
         conversation.memory.sum_chain.llm.openai_api_key = openai_api_key
 
     with console.status("loading..."):
         res = conversation.predict(
             input=user_input, summary=memory.existing_summary)
         if debug:
-            print(f"original response: {res}")
+            logging.error(f"original response: {res}")
 
         prompt_value = prompt.format_prompt(
             input=user_input,
             history=memory.load_memory_variables({})['history'],
             summary=memory.existing_summary,
         )
     parsed_response = parse_llm_output(
```

### Comparing `MistressGPT-0.9.71/chatmistress/roles/landlady.yml` & `MistressGPT-0.9.8/chatmistress/roles/landlady.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/roles/wife.yml` & `MistressGPT-0.9.8/chatmistress/roles/wife.yml`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/templates/role_play_summary.txt` & `MistressGPT-0.9.8/chatmistress/templates/role_play_summary.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/templates/role_play_sys.txt` & `MistressGPT-0.9.8/chatmistress/templates/role_play_sys.txt`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/utils.py` & `MistressGPT-0.9.8/chatmistress/utils.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/webbot.py` & `MistressGPT-0.9.8/chatmistress/webbot.py`

 * *Files identical despite different names*

### Comparing `MistressGPT-0.9.71/chatmistress/webbot2.py` & `MistressGPT-0.9.8/chatmistress/webbot2.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     "gpt-4-32k",
     "gpt-4-32k-0314",
 ]  # 可选的模型
 
 TOP_P = 1.0
 TEMPERATURE = 0.9
 
+DEFAULT_USERNAME = "我"
 HISTORY_DIR = "history"
 TEMPLATES_DIR = "templates"
 
 asset_dir = Path(__file__).parent / 'assets'
 with open(asset_dir / "custom.css", "r", encoding="utf-8") as f:
     customCSS = f.read()
 
@@ -160,15 +161,15 @@
         role_cards[ri.mistress_name] = ri
     except Exception as e:
         raise gr.Error(f"格式错误! {e}")
 
     return role_cards
 
 
-def read_template_create_chat(chat_info, role_selected, temperature, top_p, role_cards, templateSelectDropdown, systemPromptTxt=None, chatbot=None, user_name=None):
+def read_template_create_chat(chat_info, role_selected, temperature, top_p, role_cards, templateSelectDropdown, systemPromptTxt=None, chatbot=None):
     """
     从模板文件中读取模板内容, 并更新系统提示文本. 如果有必要，重置对话
     """
     role_name_selected = templateSelectDropdown
     role_info = role_cards[role_name_selected] if type(
         role_cards) is dict else role_cards.value[role_name_selected]
     systemPromptTxt = yaml.dump(role_info.dict(), allow_unicode=True)
@@ -179,15 +180,15 @@
         role_info, temperature, top_p, max_token_limit, debug=False)
 
     if chatbot is None:
         return chat_info_res, systemPromptTxt
     else:
         # 重置对话
         # chat_info, systemPromptTxt, chatbot, history
-        return chat_info_res, systemPromptTxt, gr.Chatbot.update(label=role_name_selected, value=[]), []
+        return chat_info_res, systemPromptTxt, gr.Chatbot.update(label=role_name_selected, value=[]), [], role_name_selected
 
 
 def get_templates(role_cards, plain=False):
     """
     从网上或者本地文件获取模板列表.
     TODO: 默认情况下从本地和网上获取模板列表
     """
@@ -210,21 +211,26 @@
         # 选择最新的那个prompt
         return gr.Dropdown.update(choices=templates, value=templates[-1])
 
 
 def save_chat_history(saveFileName, systemPromptTxt, history, role_selected, user_name):
     """
     """
+    print(f'user_name={user_name}')
+    pwd = Path('.')
+    history_dir = pwd / HISTORY_DIR
+    history_dir.mkdir(exist_ok=True)
+
     contents = f'## 场景\n{systemPromptTxt}\n\n\n# 聊天记录:\n\n'
     for conversation in history:
         user, bot = conversation
         contents += f'{user_name}: {user}\n\n'
         contents += f'{role_selected}: {bot}\n\n'
 
-    with open(f'{saveFileName}.md', 'w', encoding='utf-8') as f:
+    with open(history_dir / f'{saveFileName}.md', 'w', encoding='utf-8') as f:
         f.write(contents)
 
 
 # def get_history_names(plain=False, user_name=""):
 #     """
 #     TODO 读取本地的历史记录文件名列表
 #     注意，这里的对话要先被解析，所以我们暂时不处理这部分内同
@@ -332,15 +338,15 @@
 
     return chatbot, history, status_display, token_count
 
 
 def creat_gui_chat(roles: Dict[str, RoleInfo], debug=False, max_token_limit=2000):
     with gr.Blocks(css=customCSS, theme=small_and_beautiful_theme) as demo:
         my_api_key = os.getenv("OPENAI_API_KEY", None)
-        user_name = gr.State("我")
+        user_name = gr.State(DEFAULT_USERNAME)
         history = gr.State([])
         token_count = gr.State([])
         role_cards = gr.State(roles)
         role_selected = gr.State('Hello')
         chat_info = gr.State("")
 
         user_api_key = gr.State(my_api_key)
@@ -358,15 +364,15 @@
 
             # https://github.com/gradio-app/gradio/pull/3296
             def create_greeting(request: gr.Request):
                 if hasattr(request, "username") and request.username:  # is not None or is not ""
                     logging.info(f"Get User Name: {request.username}")
                     return gr.Markdown.update(value=f"User: {request.username}"), request.username
                 else:
-                    return gr.Markdown.update(value=f"User: default", visible=False), ""
+                    return gr.Markdown.update(value=f"User: default", visible=False), DEFAULT_USERNAME
             demo.load(create_greeting, inputs=None,
                       outputs=[user_info, user_name])
 
         with gr.Row().style(equal_height=True):
             with gr.Column(scale=3):
                 with gr.Row():
                     chatbot = gr.Chatbot(
@@ -386,14 +392,16 @@
                     )
 
             with gr.Column(scale=1, min_width=400):
                 with gr.Column(min_width=400):
                     role_names = get_templates(role_cards, plain=True)
                     role_name_selected = role_names[0]
                     chatbot.label = role_name_selected
+                    role_selected.value = role_name_selected
+
                     chat_info.value, initial_prompt = read_template_create_chat(
                         chat_info, role_selected, temperature, top_p, role_cards, role_name_selected)
                     with gr.Tab(label="Prompt"):
                         systemPromptTxt = gr.Textbox(
                             show_label=True,
                             placeholder=f"在这里输入设定...",
                             label="故事设定",
@@ -515,15 +523,15 @@
                                                       chatgpt_predict_args).then(**end_outputing_args)
 
         submitBtn.click(**transfer_input_args).then(**
                                                     chatgpt_predict_args).then(**end_outputing_args)
 
         creat_chat_args = dict(
             fn=read_template_create_chat, inputs=[chat_info, role_selected, temperature, top_p, role_cards, templateSelectDropdown,
-                                                  systemPromptTxt, chatbot], outputs=[chat_info, systemPromptTxt, chatbot, history]
+                                                  systemPromptTxt, chatbot], outputs=[chat_info, systemPromptTxt, chatbot, history, role_selected]
         )
 
         emptyBtn.click(
             reset_state,
             outputs=[chatbot, history, token_count, status_display],
             show_progress=True,
         ).then(show_progress=True, **creat_chat_args)
@@ -584,11 +592,7 @@
 
 
 if __name__ == '__main__':
     from dotenv import load_dotenv
     load_dotenv()
     demo = creat_gui_chat()
     demo.launch()
-
-# role_selected = role_list[0]
-# demo = creat_chat(roles[role_selected])
-# demo.launch()
```

### Comparing `MistressGPT-0.9.71/setup.py` & `MistressGPT-0.9.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='MistressGPT',
     description='MistressGPT: 基于GPT3.5的女王聊天室',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.71',
+    version='0.9.8',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'mistressgpt=chatmistress.chatmistress:main'
         ]
     },
     package_data={
```

