# Comparing `tmp/nonebot-plugin-SDGPT-0.1.1.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.1.1.tar", last modified: Mon Apr 10 12:47:53 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.1.2.tar", last modified: Mon Apr 10 14:09:40 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.1.1.tar` & `nonebot-plugin-SDGPT-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.276173 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     9257 2023-04-10 12:45:26.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-10 12:47:53.000000 nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 12:47:53.291799 nonebot-plugin-SDGPT-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-10 12:47:13.000000 nonebot-plugin-SDGPT-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:09:40.341599 nonebot-plugin-SDGPT-0.1.2/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-10 14:09:40.341599 nonebot-plugin-SDGPT-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-04-09 01:25:35.000000 nonebot-plugin-SDGPT-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:09:40.325972 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3339 2023-04-10 14:07:48.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     9775 2023-04-10 14:02:21.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:09:40.341599 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-10 14:09:40.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-10 14:09:40.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:09:40.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-10 14:09:40.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-10 14:09:40.000000 nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 14:09:40.341599 nonebot-plugin-SDGPT-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-10 14:09:25.000000 nonebot-plugin-SDGPT-0.1.2/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.1.1/LICENSE` & `nonebot-plugin-SDGPT-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.1/README.md` & `nonebot-plugin-SDGPT-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from nonebot import get_driver, require
 
 
-from .bot import info,error,warn
+from .bot import info,error,warn,err
 from nonebot.plugin import on_command , on_message , on
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 from nonebot.adapters import Message
 from nonebot.plugin import PluginMetadata
 
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
 from nonebot.params import CommandArg
 from nonebot.rule import to_me
-from .bot import Chat,Bing,text2image,startup,Chat_api
+from .bot import Chat,Bing,text2image,startup,Chat_api,AIcheck
 
 from dotenv import dotenv_values, load_dotenv
 config =dotenv_values(".cfg")
 
 __plugin_meta__ = PluginMetadata(
     name="ChatBot",
     description="ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion",
@@ -27,28 +27,36 @@
 driver = get_driver()
 
 @driver.on_startup
 async def do_something():
     global Presets
     global botList  
     global cfg
+    global ChatUse
     info('fthxbot','startup')
     CFGdata = await startup()
     Presets = CFGdata['Presets']
     botList = CFGdata['botList']
     cfg = CFGdata['cfg']
+    ChatUse = CFGdata['ChatUse']
+
     
 
 chat = on_command('chat')
 @chat.handle()
 async def _(event:GuildMessageEvent|GroupMessageEvent,args: Message = CommandArg()):
+    global ChatUse
     message = args.extract_plain_text()
-    await Chat(chat,message)
-    if type(event) == GuildMessageEvent:await Bing(bing,message)
-    elif type(event) == GroupMessageEvent:await Bing(bing,message,0)
+    if ChatUse == Bing:
+        if await AIcheck(Chat_api):
+            ChatUse = Chat_api
+        elif await AIcheck(Chat):
+            ChatUse = Chat
+    if type(event) == GuildMessageEvent:await ChatUse(bing,message) # type: ignore
+    elif type(event) == GroupMessageEvent:await ChatUse(bing,message,0) # type: ignore
 
 bing = on_command('bing')
 @bing.handle()
 async def _(event:GuildMessageEvent|GroupMessageEvent,args: Message = CommandArg()):
     message = args.extract_plain_text()
     if type(event) == GuildMessageEvent:await Bing(bing,message)
     elif type(event) == GroupMessageEvent:await Bing(bing,message,0)
@@ -56,61 +64,44 @@
 
 
 msg = on_message(rule=to_me())
 @msg.handle()
 async def _(event:GuildMessageEvent|GroupMessageEvent):
     global ChatUse
     message = str(event.message)
-    All = {
-        'ChatGPT' : Chat,
-        'Bing' : Bing,
-        'ChatGPT_api' : Chat_api,
-    }
-    if cfg['defaultAI'] and type(cfg['defaultAI'])==str:  
-        if cfg.defaultAI in botList:
-            try : not ChatUse # type: ignore
-            except : ChatUse  = All[cfg['defaultAI']]
-        else: 
-            return error('Config','你配置的 defaultAI 没有被接入')
-    else: 
-        return error('Config','你没有配置 defaultAI')
-
     if type(event) == GuildMessageEvent:await ChatUse(msg,message) # type: ignore
     elif type(event) == GroupMessageEvent:await ChatUse(msg,message,0) # type: ignore
 
 
 tag = on_command('tag')
 @tag.handle()
 async def _(args: Message = CommandArg()):
     message = args.extract_plain_text()
-    await Chat(tag,Presets['PromptGenerator'] + message,0)
+    global ChatUse
+    await ChatUse(tag,Presets['PromptGenerator'] + message,0) # type: ignore
 
 
 ai = on_command('ai')
 @ai.handle()
 async def _(args: Message = CommandArg()):
     message = args.extract_plain_text()
-    text = await Chat(tag,Presets['PromptGenerator'] + message,2)
+    global ChatUse
+    text = await ChatUse(tag,Presets['PromptGenerator'] + message,2) # type: ignore
     img_bytes = await text2image(ai,text)
     await ai.reject(MessageSegment.image(file=img_bytes,cache=False))
 
-test = on_command('test')
-@test.handle()
-async def _():
-    await test.send('test')
-
 chatC = on_command('切换AI')
 @chatC.handle()
 async def _(args: Message = CommandArg()):
     All = {
         'ChatGPT' : Chat,
         'Bing' : Bing,
         'ChatGPT_api' : Chat_api,
     }
-    global chatUse
     message = args.extract_plain_text()
-    if message in botList:
-        chatUse = All[message]
-        await chatC.send(f'已切换到 {message}')
-    else: 
-        await chatC.send('AI没有配置 或 AI不存在')
+    global ChatUse
+    ChatUse = All[message]
+    if not await AIcheck(ChatUse) :
+        err('ChatUse','AI不存在')
+        return await chatC.send('AI不存在')
+    await chatC.send(f'已切换到 {message}')
```

### Comparing `nonebot-plugin-SDGPT-0.1.1/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.1.2/nonebot_plugin_SDGPT/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,19 @@
     if len(out_text) < len(text) or mode == 0:
         outText = text.replace(out_text,'')
         success('Bing', outText)
         await func.send(outText)
     if mode ==2:
         return text.replace(r'.*\.AIP','')
 
+AllAI = {
+        'ChatGPT' : Chat,
+        'Bing' : Bing,
+        'ChatGPT_api' : Chat_api,
+    }
 async def text2image(func,prompt):
     ip = cfg['text2img_proxy'].split(':')
     info('Stable-Diffusion','开始询问 api'+cfg['text2img_proxy'])
     api = webuiapi.WebUIApi(host=ip[0], port=ip[1]) # type: ignore
     
     result1 = api.txt2img(
         prompt=prompt,
@@ -203,15 +208,15 @@
         else:raise Exception()
         cfg.update(cfg_)
     except:
         err('Config','配置文件 config.cfg 未配置')
         # raise Exception('配置文件 config.cfg 未配置')
 
 
-    botList  = []
+    botList = []
 
     info('Presets Load','开始加载预设')
     Presets = {}
     for file_path in glob.glob(os.path.join(cfg['presets_dir'], '*.txt')):
         with open(file_path, 'r', encoding='utf-8') as file:
             content = file.read()
         fileName = os.path.basename(file_path).replace('.txt', '')
@@ -245,9 +250,26 @@
             warn('ChatGPT api','apikey 无效,将无法使用ChatGPT api模式')
             raise Exception
         chatbot_api = chatGPT_api(cfg['api_key'])
         botList.append('ChatGPT_api')
         suc('ChatGPT api','接入 ChatGPT_api 成功')
     except:pass
     CFGdata['botList']=botList
+    suc('所有AI',str(botList))
+    if cfg['defaultAI'] in botList:
+        ChatUse = AllAI[cfg['defaultAI']]
+        CFGdata['ChatUse']=ChatUse
+    else: 
+        error('Config','你配置的 defaultAI 错误')
+        print(botList)
+        raise Exception('ChatUse error')
+    
     CFGdata['cfg']=cfg
     return CFGdata
+
+
+async def AIcheck(fuc) -> bool:
+    All = AllAI
+    for i in botList:
+        if All[i] == fuc:
+            return True
+    return False
```

### Comparing `nonebot-plugin-SDGPT-0.1.1/setup.py` & `nonebot-plugin-SDGPT-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="nonebot-plugin-SDGPT",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.1.1",  # 程序版本
+    version="0.1.2",  # 程序版本
     author="F_thx",  # 项目作者
     author_email="thx1140093097@gmail.com",  # 作者邮件
     url="https://github.com/thx114/SDGPT",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     license="MIT Licence",
     install_requires=[
         'nonebot2',
```

