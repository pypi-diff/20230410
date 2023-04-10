# Comparing `tmp/nonebot-plugin-SDGPT-0.1.0.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.1.0.tar", last modified: Sun Apr  9 22:13:52 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.1.1.tar", last modified: Mon Apr 10 12:47:53 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.1.0.tar` & `nonebot-plugin-SDGPT-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.437157 nonebot-plugin-SDGPT-0.1.0/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-09 22:13:52.436156 nonebot-plugin-SDGPT-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.423164 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     9410 2023-04-09 22:11:16.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:13:52.433153 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-09 22:13:52.000000 nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 22:13:52.437157 nonebot-plugin-SDGPT-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-09 22:13:43.000000 nonebot-plugin-SDGPT-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.276173 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     9257 2023-04-10 12:45:26.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-10 12:47:13.000000 nonebot-plugin-SDGPT-0.1.1/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.1.0/LICENSE` & `nonebot-plugin-SDGPT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.0/README.md` & `nonebot-plugin-SDGPT-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.0/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,254 +1,253 @@
-import glob
-from io import BytesIO
-import json
-import os
-import sys
-import time
-import re
-
-from nonebot.log import logger_id
-from nonebot.log import  default_filter
-
-from nonebot import logger
-import webuiapi
-from revChatGPT.V1 import Chatbot as chatGPT
-from revChatGPT.V3 import Chatbot as chatGPT_api
-from EdgeGPT import Chatbot as bing
-logger.remove(logger_id)
-
-def formatter(record):
-    record['message']
-    level = record['level'].name
-    add = ''
-    Dir = {
-        'INFO':'<cyan>',
-        'ERROR':'<RED>[ERROR]</RED><red>',
-        'WARNING':'<LIGHT-YELLOW><black>[WARN]</black></><light-yellow>',
-        'DEBUG':'<bold>',
-        'SUCCESS':'<green>',
-        'FBOT':'<fg #bf0060>',
-        'suc':'<GREEN>[OK]</GREEN><green>',
-        'err':'<RED>[ERROR]</RED><RED><white>'
-    }
-    color_tag=Dir[level]
-    if not color_tag:color_tag = ''
-    match = re.match(r'^\s*\[([^\]]+)\]',record['message'])
-    if match:
-        func_name = '['+match[1]+']'
-        record['message'] = record['message'].replace(func_name,'')
-    else: func_name = '['+record['name']+']'
-    if level == 'ERROR': add = "{exception}"
-    if level == 'err': add = "</>"
-    return color_tag+func_name+"</>"+'{message}'+"\n"+add
-logger.add(sys.stdout, format=formatter,level=0,filter=default_filter,diagnose=True,serialize=False)
-logger.level('suc',no=25)
-logger.level('err',no=40)
-logger.level('FBOT',no=20)
-
-def info(app:str,text:str): logger.opt(colors=True).log('FBOT',f"[{app}] {text}")
-def error(app:str,text:str): logger.opt(colors=True).error(f"[{app}] {text}")
-def success(app:str,text:str): logger.opt(colors=True).success(f"[{app}] {text}")
-def warn(app:str,text:str): logger.opt(colors=True).warning(f"[{app}] {text}")
-def debug(app:str,text:str): logger.opt(colors=True).debug(f"[{app}] {text}")
-def suc(app:str,text:str): logger.opt(colors=True).log('suc',f"[{app}] {text}")
-def err(app:str,text:str): logger.opt(colors=True).log('err',f"[{app}] {text}")
-
-from dotenv import dotenv_values, load_dotenv, set_key
-cfg = {
-'text2img_step':27,
-'text2img_negative_prompt':"(worst quality, low quality:1.4),NSFW,r18",
-'text2img_proxy':'127.0.0.1:7860',
-'presets_dir':'./presets',
-'Chat_stream_waitTime':2,
-'Chat_stream_endStr':('？','。','?','\n'),
-'defaultAI':'chatGPT',
-'access_token':'',
-'api_key':'',
-'model':'gpt-3.5-turbo',
-'cookies_file_path': "./cookies.json",
-}
-
-
-
-async def Chat(func,message:str,mode=1): 
-    if not message or len(message)<1:return
-    Rtime = int(cfg['Chat_stream_waitTime'])
-    endStr = cfg['Chat_stream_endStr']
-    text = ''
-    out_text=''
-    info('ChatGPT','开始询问 (网页)')
-    for data in chatbot.ask(message):
-        text = data["message"] # type: ignore
-        try: not now # type: ignore
-        except: now = time.time()
-        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1: # type: ignore
-            now = time.time()
-            outText = text.replace(out_text,'')
-            success('ChatGPT', outText)
-            await func.send(outText)
-            out_text = data["message"] # type: ignore
-    if len(out_text) < len(text) or mode == 0:
-        outText = text.replace(out_text,'')
-        success('ChatGPT', outText)
-        await func.send(outText)
-    if mode ==2:
-        return text.replace(r'.*\.AIP','')
-    
-async def Chat_api(func,message:str,mode=1):
-    if not message or len(message)<1:return
-    Rtime = cfg['Chat_stream_waitTime']
-    endStr = cfg['Chat_stream_endStr']
-    text = ''
-    info('ChatGPT api','开始询问 api')
-    for data in chatbot_api.ask_stream(message):
-        text += data 
-        try: not now # type: ignore
-        except: now = time.time()
-        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1: # type: ignore
-            now = time.time()
-            success('ChatGPT api', text)
-            await func.send(text)
-            text = ''
-    if len(text) > 0:
-        success('ChatGPT api', text)
-        await func.send(text)
-    if mode ==2:
-        return text.replace(r'.*\.AIP','')
-
-async def Bing(func,message,mode=1):
-    if not message or len(message)<1:return
-    Rtime = int(cfg['Chat_stream_waitTime'])
-    endStr = cfg['Chat_stream_endStr']
-    text = ''
-    out_text=''
-    info('Bing','开始询问 api')
-    async for data in bingbot.ask_stream(message):
-        istrue , string = data
-        if type(string) == str : text = string
-        try: not now # type: ignore
-        except: now = time.time()
-        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1 : # type: ignore
-            now = time.time()
-            outText = text.replace(out_text,'')
-            success('Bing', outText)
-            if len(outText.replace(' ','')) > 0:
-                await func.send(outText)
-            out_text = text # type: ignore
-    if len(out_text) < len(text) or mode == 0:
-        outText = text.replace(out_text,'')
-        success('Bing', outText)
-        await func.send(outText)
-    if mode ==2:
-        return text.replace(r'.*\.AIP','')
-
-async def text2image(func,prompt):
-    ip = cfg['text2img_proxy'].split(':')
-    info('Stable-Diffusion','开始询问 api'+cfg['text2img_proxy'])
-    api = webuiapi.WebUIApi(host=ip[0], port=ip[1]) # type: ignore
-    
-    result1 = api.txt2img(
-        prompt=prompt,
-        negative_prompt=cfg['text2img_negative_prompt'],
-        steps=cfg['text2img_step'],
-    )
-    image = result1.image
-    success('Stable-Diffusion','返回图片')
-    buffered = BytesIO()
-    image.save(buffered, format="PNG")
-    img_bytes = buffered.getvalue()
-    return img_bytes
-
-async def startup():
-    global bingbot
-    global chatbot
-    global chatbot_api
-    global botList 
-    if not os.path.exists('./config.cfg'):
-        with open('config.cfg', 'w',encoding='utf-8') as f:
-            text = """
-# "#"后面的为注释
-
-Stable-Diffusion # Stable-Diffusion 配置:
-text2img_step=27 # 文生图 渲染步数
-text2img_negative_prompt="(worst quality, low quality:1.4),NSFW,r18" #文生图 固定负面提示词
-text2img_proxy='127.0.0.1:7860' #Stable-Diffusion api地址 (SD内配置 --server-name 127.0.0.1 --port 7860 --api)
-
-chat # 聊天 api 通用设置:
-presets_dir='./presets' # 预设文件夹
-Chat_stream_waitTime=2 # 频道内 分条发送间隔 (秒)
-Chat_stream_endStr=('？','。','?','\n') # 频道内 分条发送分割依据
-defaultAI='chatGPT' # 默认 AI
-
-chatGPT # ChatGPT 配置 (网页):
-access_token="" # access_token  获取:https://chat.openai.com/api/auth/session
-
-chatGPT_api # ChatGPT api 配置:
-api_key="" # api_key 获取:https://platform.openai.com/account/api-keys
-model="gpt-3.5-turbo"
-
-bing # Bing api 配置:
-cookies_file_path="./cookies.json" # 设置:https://github.com/thx114/SDGPT/wiki/bing-cookies
-"""
-            f.write(text)
-
-
-    cfg_ =dotenv_values("config.cfg")
-
-    try : 
-        if len(cfg_['access_token']) >0:suc('Config','配置文件 有效') # type: ignore
-        elif len(cfg_['api_key']) >0:suc('Config','配置文件 有效') # type: ignore
-        elif len(cfg_['cookies_file_path'])>0: # type: ignore
-            with open(cfg_['cookies_file_path'], 'r') as f: # type: ignore
-                cookies = json.load(f)
-                suc('Config','配置文件 有效')
-        else:raise Exception()
-        cfg.update(cfg_)
-    except:
-        err('Config','配置文件 config.cfg 未配置')
-        # raise Exception('配置文件 config.cfg 未配置')
-
-
-    botList  = []
-
-    info('Presets Load','开始加载预设')
-    Presets = {}
-    for file_path in glob.glob(os.path.join(cfg['presets_dir'], '*.txt')):
-        with open(file_path, 'r', encoding='utf-8') as file:
-            content = file.read()
-        fileName = os.path.basename(file_path).replace('.txt', '')
-        Presets[fileName] = content
-        success('Presets Load','加载预设: '+fileName)
-    CFGdata = {}
-    CFGdata['Presets'] = Presets
-    try: 
-        cfg['cookies_file_path']
-        if os.path.exists(cfg['cookies_file_path']):
-            info('Bing',"发现cookies.json")
-            with open(cfg['cookies_file_path'], 'r') as f:
-                cookies = json.load(f)
-                bingbot = bing(cookies=cookies)
-            botList.append('Bing')
-            suc('Bing','接入 Bing 成功')
-        else:warn('Bing','cookies.json 不存在,将无法使用bing')
-    except:pass
-    try: 
-        cfg['access_token']
-        if len(cfg['access_token']) < 4 : 
-            warn('ChatGPT','access_token 无效,将无法使用ChatGPT 网页模式')
-            raise Exception
-        chatbot = chatGPT(config={"access_token": cfg['access_token']})
-        botList.append('ChatGPT')
-        suc('chatGPT','接入 ChatGPT 成功')
-    except:pass
-    try:
-        cfg['api_key']
-        if(len(cfg['api_key']) < 4 or 'sk-' not in cfg['api_key']): 
-            warn('ChatGPT api','apikey 无效,将无法使用ChatGPT api模式')
-            raise Exception
-        chatbot_api = chatGPT_api(cfg['api_key'])
-        botList.append('ChatGPT_api')
-        suc('ChatGPT api','接入 ChatGPT_api 成功')
-    except:pass
-    CFGdata['botList']=botList
-    CFGdata['cfg']=cfg
-    return CFGdata
+import glob
+from io import BytesIO
+import json
+import os
+import sys
+import time
+import re
+import html
+from nonebot.log import logger_id
+from nonebot.log import  default_filter
+from nonebot import logger
+import webuiapi
+from revChatGPT.V1 import Chatbot as chatGPT
+from revChatGPT.V3 import Chatbot as chatGPT_api
+from EdgeGPT import Chatbot as bing
+logger.remove(logger_id)
+
+def formatter(record):
+    record['message']
+    level = record['level'].name
+    add = ''
+    Dir = {
+        'INFO':'<cyan>',
+        'ERROR':'<RED>[ERROR]</RED><red>',
+        'WARNING':'<LIGHT-YELLOW><black>[WARN]</black></><light-yellow>',
+        'DEBUG':'<bold>',
+        'SUCCESS':'<green>',
+        'FBOT':'<fg #bf0060>',
+        'suc':'<GREEN>[OK]</GREEN><green>',
+        'err':'<RED>[ERROR]</RED><RED><white>'
+    }
+    color_tag=Dir[level]
+    if not color_tag:color_tag = ''
+    match = re.match(r'^\s*\[([^\]]+)\]',record['message'])
+    if match:
+        func_name = '['+match[1]+']'
+        record['message'] = record['message'].replace(func_name,'')
+    else: func_name = '['+record['name']+']'
+    if level == 'ERROR': add = "{exception}"
+    if level == 'err': add = "</>"
+    return color_tag+func_name+"</>"+'{message}'+"\n"+add
+logger.add(sys.stdout, format=formatter,level=0,filter=default_filter,diagnose=True,serialize=False)
+logger.level('suc',no=25)
+logger.level('err',no=40)
+logger.level('FBOT',no=20)
+
+def info(app:str,text:str): logger.opt(colors=True).log('FBOT',f"[{app}] {html.escape(text)}")
+def error(app:str,text:str): logger.opt(colors=True).error(f"[{app}] {html.escape(text)}")
+def success(app:str,text:str): logger.opt(colors=True).success(f"[{app}] {html.escape(text)}")
+def warn(app:str,text:str): logger.opt(colors=True).warning(f"[{app}] {html.escape(text)}")
+def debug(app:str,text:str): logger.opt(colors=True).debug(f"[{app}] {html.escape(text)}")
+def suc(app:str,text:str): logger.opt(colors=True).log('suc',f"[{app}] {html.escape(text)}")
+def err(app:str,text:str): logger.opt(colors=True).log('err',f"[{app}] {html.escape(text)}")
+
+from dotenv import dotenv_values, load_dotenv, set_key
+cfg = {
+'text2img_step':27,
+'text2img_negative_prompt':"(worst quality, low quality:1.4),NSFW,r18",
+'text2img_proxy':'127.0.0.1:7860',
+'presets_dir':'./presets',
+'Chat_stream_waitTime':2,
+'Chat_stream_endStr':('？','。','?','\n'),
+'defaultAI':'chatGPT',
+'access_token':'',
+'api_key':'',
+'model':'gpt-3.5-turbo',
+'cookies_file_path': "./cookies.json",
+}
+
+
+
+async def Chat(func,message:str,mode=1): 
+    if not message or len(message)<1:return
+    Rtime = int(cfg['Chat_stream_waitTime'])
+    endStr = cfg['Chat_stream_endStr']
+    text = ''
+    out_text=''
+    info('ChatGPT','开始询问 (网页)')
+    for data in chatbot.ask(message):
+        text = data["message"] # type: ignore
+        try: not now # type: ignore
+        except: now = time.time()
+        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1: # type: ignore
+            now = time.time()
+            outText = text.replace(out_text,'')
+            success('ChatGPT', outText)
+            await func.send(outText)
+            out_text = data["message"] # type: ignore
+    if len(out_text) < len(text) or mode == 0:
+        outText = text.replace(out_text,'')
+        success('ChatGPT', outText)
+        await func.send(outText)
+    if mode ==2:
+        return text.replace(r'.*\.AIP','')
+    
+async def Chat_api(func,message:str,mode=1):
+    if not message or len(message)<1:return
+    Rtime = cfg['Chat_stream_waitTime']
+    endStr = cfg['Chat_stream_endStr']
+    text = ''
+    info('ChatGPT api','开始询问 api')
+    for data in chatbot_api.ask_stream(message):
+        text += data 
+        try: not now # type: ignore
+        except: now = time.time()
+        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1: # type: ignore
+            now = time.time()
+            success('ChatGPT api', text)
+            await func.send(text)
+            text = ''
+    if len(text) > 0:
+        success('ChatGPT api', text)
+        await func.send(text)
+    if mode ==2:
+        return text.replace(r'.*\.AIP','')
+
+async def Bing(func,message,mode=1):
+    if not message or len(message)<1:return
+    Rtime = int(cfg['Chat_stream_waitTime'])
+    endStr = cfg['Chat_stream_endStr']
+    text = ''
+    out_text=''
+    info('Bing','开始询问 api')
+    async for data in bingbot.ask_stream(message):
+        istrue , string = data
+        if type(string) == str : text = string
+        try: not now # type: ignore
+        except: now = time.time()
+        if time.time() - now > Rtime and text.endswith(endStr) and mode == 1 : # type: ignore
+            now = time.time()
+            outText = text.replace(out_text,'')
+            success('Bing', outText)
+            if len(outText.replace(' ','')) > 0:
+                await func.send(outText)
+            out_text = text # type: ignore
+    if len(out_text) < len(text) or mode == 0:
+        outText = text.replace(out_text,'')
+        success('Bing', outText)
+        await func.send(outText)
+    if mode ==2:
+        return text.replace(r'.*\.AIP','')
+
+async def text2image(func,prompt):
+    ip = cfg['text2img_proxy'].split(':')
+    info('Stable-Diffusion','开始询问 api'+cfg['text2img_proxy'])
+    api = webuiapi.WebUIApi(host=ip[0], port=ip[1]) # type: ignore
+    
+    result1 = api.txt2img(
+        prompt=prompt,
+        negative_prompt=cfg['text2img_negative_prompt'],
+        steps=cfg['text2img_step'],
+    )
+    image = result1.image
+    success('Stable-Diffusion','返回图片')
+    buffered = BytesIO()
+    image.save(buffered, format="PNG")
+    img_bytes = buffered.getvalue()
+    return img_bytes
+
+async def startup():
+    global bingbot
+    global chatbot
+    global chatbot_api
+    global botList 
+    if not os.path.exists('./config.cfg'):
+        with open('config.cfg', 'w',encoding='utf-8') as f:
+            text = """
+# "#"后面的为注释
+
+Stable-Diffusion # Stable-Diffusion 配置:
+text2img_step=27 # 文生图 渲染步数
+text2img_negative_prompt="(worst quality, low quality:1.4),NSFW,r18" #文生图 固定负面提示词
+text2img_proxy='127.0.0.1:7860' #Stable-Diffusion api地址 (SD内配置 --server-name 127.0.0.1 --port 7860 --api)
+
+chat # 聊天 api 通用设置:
+presets_dir='./presets' # 预设文件夹
+Chat_stream_waitTime=2 # 频道内 分条发送间隔 (秒)
+Chat_stream_endStr=('？','。','?','\n') # 频道内 分条发送分割依据
+defaultAI='chatGPT' # 默认 AI
+
+chatGPT # ChatGPT 配置 (网页):
+access_token="" # access_token  获取:https://chat.openai.com/api/auth/session
+
+chatGPT_api # ChatGPT api 配置:
+api_key="" # api_key 获取:https://platform.openai.com/account/api-keys
+model="gpt-3.5-turbo"
+
+bing # Bing api 配置:
+cookies_file_path="./cookies.json" # 设置:https://github.com/thx114/SDGPT/wiki/bing-cookies
+"""
+            f.write(text)
+
+
+    cfg_ =dotenv_values("config.cfg")
+
+    try : 
+        if len(cfg_['access_token']) >0:suc('Config','配置文件 有效') # type: ignore
+        elif len(cfg_['api_key']) >0:suc('Config','配置文件 有效') # type: ignore
+        elif len(cfg_['cookies_file_path'])>0: # type: ignore
+            with open(cfg_['cookies_file_path'], 'r') as f: # type: ignore
+                cookies = json.load(f)
+                suc('Config','配置文件 有效')
+        else:raise Exception()
+        cfg.update(cfg_)
+    except:
+        err('Config','配置文件 config.cfg 未配置')
+        # raise Exception('配置文件 config.cfg 未配置')
+
+
+    botList  = []
+
+    info('Presets Load','开始加载预设')
+    Presets = {}
+    for file_path in glob.glob(os.path.join(cfg['presets_dir'], '*.txt')):
+        with open(file_path, 'r', encoding='utf-8') as file:
+            content = file.read()
+        fileName = os.path.basename(file_path).replace('.txt', '')
+        Presets[fileName] = content
+        success('Presets Load','加载预设: '+fileName)
+    CFGdata = {}
+    CFGdata['Presets'] = Presets
+    try: 
+        cfg['cookies_file_path']
+        if os.path.exists(cfg['cookies_file_path']):
+            info('Bing',"发现cookies.json")
+            with open(cfg['cookies_file_path'], 'r') as f:
+                cookies = json.load(f)
+                bingbot = bing(cookies=cookies)
+            botList.append('Bing')
+            suc('Bing','接入 Bing 成功')
+        else:warn('Bing','cookies.json 不存在,将无法使用bing')
+    except:pass
+    try: 
+        cfg['access_token']
+        if len(cfg['access_token']) < 4 : 
+            warn('ChatGPT','access_token 无效,将无法使用ChatGPT 网页模式')
+            raise Exception
+        chatbot = chatGPT(config={"access_token": cfg['access_token']})
+        botList.append('ChatGPT')
+        suc('chatGPT','接入 ChatGPT 成功')
+    except:pass
+    try:
+        cfg['api_key']
+        if(len(cfg['api_key']) < 4 or 'sk-' not in cfg['api_key']): 
+            warn('ChatGPT api','apikey 无效,将无法使用ChatGPT api模式')
+            raise Exception
+        chatbot_api = chatGPT_api(cfg['api_key'])
+        botList.append('ChatGPT_api')
+        suc('ChatGPT api','接入 ChatGPT_api 成功')
+    except:pass
+    CFGdata['botList']=botList
+    CFGdata['cfg']=cfg
+    return CFGdata
```

### Comparing `nonebot-plugin-SDGPT-0.1.0/setup.py` & `nonebot-plugin-SDGPT-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="nonebot-plugin-SDGPT",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.0",  # 程序版本
+    version="0.1.1",  # 程序版本
     author="F_thx",  # 项目作者
     author_email="thx1140093097@gmail.com",  # 作者邮件
     url="https://github.com/thx114/SDGPT",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     license="MIT Licence",
     install_requires=[
         'nonebot2',
```

