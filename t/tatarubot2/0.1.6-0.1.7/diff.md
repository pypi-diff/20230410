# Comparing `tmp/tatarubot2-0.1.6.tar.gz` & `tmp/tatarubot2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tatarubot2-0.1.6.tar", max compression
+gzip compressed data, was "tatarubot2-0.1.7.tar", max compression
```

## Comparing `tatarubot2-0.1.6.tar` & `tatarubot2-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,44 @@
--rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.6/LICENSE
--rw-r--r--   0        0        0     2734 2023-03-14 01:51:48.000000 tatarubot2-0.1.6/README.md
--rw-r--r--   0        0        0      424 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.6/tatarubot2/__init__.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.6/tatarubot2/data/boss.json
--rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.6/tatarubot2/data/item_dict.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.6/tatarubot2/data/job.json
--rw-r--r--   0        0        0     1525 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/tatarubot2/plugins/__init__.py
--rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.6/tatarubot2/plugins/auto_response.py
--rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/plugins/bot_help.py
--rw-r--r--   0        0        0     1211 2023-04-07 02:28:25.000000 tatarubot2-0.1.6/tatarubot2/plugins/chat_ai.py
--rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.6/tatarubot2/plugins/ff_weibo.py
--rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/house.py
--rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.6/tatarubot2/plugins/item.py
--rw-r--r--   0        0        0    17442 2023-04-10 14:32:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/item_new.py
--rw-r--r--   0        0        0     7150 2023-04-10 14:58:41.000000 tatarubot2-0.1.6/tatarubot2/plugins/logs_dps.py
--rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.6/tatarubot2/plugins/lottery.py
--rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.6/tatarubot2/plugins/market.py
--rw-r--r--   0        0        0     8327 2023-04-10 14:32:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/market_new.py
--rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.6/tatarubot2/plugins/nuannuan.py
--rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.6/tatarubot2/plugins/precious.py
--rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.6/tatarubot2/plugins/weather.py
--rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.6/tatarubot2/tools/__init__.py
--rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.6/tatarubot2/tools/data.json
--rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/tools/download_boss.py
--rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.6/tatarubot2/tools/download_item2id.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.6/tatarubot2/tools/new_boss.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.6/tatarubot2/tools/new_job.json
--rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.6/tatarubot2/tools/normal_data.py
--rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 tatarubot2-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3600 2023-04-10 16:38:02.000000 tatarubot2-0.1.7/README_PIP.md
+-rw-r--r--   0        0        0      420 2023-04-10 16:38:02.000000 tatarubot2-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.7/tatarubot2/__init__.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.7/tatarubot2/data/boss.json
+-rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.7/tatarubot2/data/item_dict.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.7/tatarubot2/data/job.json
+-rw-r--r--   0        0        0     1680 2023-04-10 15:34:49.000000 tatarubot2-0.1.7/tatarubot2/plugins/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-10 15:35:48.501998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1759 2023-04-10 15:35:49.525995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/bot_help.cpython-37.pyc
+-rw-r--r--   0        0        0     1259 2023-04-10 15:42:09.704827 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/chat_ai.cpython-37.pyc
+-rw-r--r--   0        0        0     1878 2023-04-10 15:35:48.501998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/ff_weibo.cpython-37.pyc
+-rw-r--r--   0        0        0     4186 2023-04-10 15:35:48.565998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/house.cpython-37.pyc
+-rw-r--r--   0        0        0    11706 2023-04-10 15:35:48.629998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item.cpython-37.pyc
+-rw-r--r--   0        0        0    11717 2023-04-10 15:35:48.697997 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item_new.cpython-37.pyc
+-rw-r--r--   0        0        0     6049 2023-04-10 15:35:48.985997 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/logs_dps.cpython-37.pyc
+-rw-r--r--   0        0        0     1298 2023-04-10 15:35:49.049996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/lottery.cpython-37.pyc
+-rw-r--r--   0        0        0     6464 2023-04-10 15:35:49.113996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market.cpython-37.pyc
+-rw-r--r--   0        0        0     6614 2023-04-10 15:35:49.177996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market_new.cpython-37.pyc
+-rw-r--r--   0        0        0     2737 2023-04-10 15:35:49.401995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/nuannuan.cpython-37.pyc
+-rw-r--r--   0        0        0     1167 2023-04-10 15:35:49.465995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/precious.cpython-37.pyc
+-rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.7/tatarubot2/plugins/auto_response.py
+-rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/plugins/bot_help.py
+-rw-r--r--   0        0        0     1249 2023-04-10 15:47:26.000000 tatarubot2-0.1.7/tatarubot2/plugins/chat_ai.py
+-rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.7/tatarubot2/plugins/ff_weibo.py
+-rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/house.py
+-rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.7/tatarubot2/plugins/item.py
+-rw-r--r--   0        0        0    17442 2023-04-10 14:32:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/item_new.py
+-rw-r--r--   0        0        0     7150 2023-04-10 14:58:41.000000 tatarubot2-0.1.7/tatarubot2/plugins/logs_dps.py
+-rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.7/tatarubot2/plugins/lottery.py
+-rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.7/tatarubot2/plugins/market.py
+-rw-r--r--   0        0        0     8327 2023-04-10 14:32:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/market_new.py
+-rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.7/tatarubot2/plugins/nuannuan.py
+-rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/precious.py
+-rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.7/tatarubot2/plugins/weather.py
+-rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.7/tatarubot2/tools/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 15:35:49.585995 tatarubot2-0.1.7/tatarubot2/tools/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.7/tatarubot2/tools/data.json
+-rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/tools/download_boss.py
+-rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.7/tatarubot2/tools/download_item2id.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.7/tatarubot2/tools/new_boss.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.7/tatarubot2/tools/new_job.json
+-rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/tools/normal_data.py
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 tatarubot2-0.1.7/PKG-INFO
```

### Comparing `tatarubot2-0.1.6/LICENSE` & `tatarubot2-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/README.md` & `tatarubot2-0.1.7/README_PIP.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # TataruBot2
 
 基于NoneBot2的FF14机器人塔塔露
 
+这里是塔塔露功能作为nonebot2插件安装的指南
+
 ## 当前功能
 
+0. 塔塔露帮帮忙：显示所有功能
 1. 暖暖：本周时尚品鉴作业
 2. 选门：帮你选藏宝洞的门
 3. 仙人彩：帮你选每周仙人仙彩数字
 4. 物品 物品名：查询物品信息，例：`物品 铁矿`
 5. 价格 大区 物品名：查询板子物价，大区不写默认豆豆柴，例：`价格 陆行鸟 铁矿`、`价格 叶小妖`
 6. 看看微博：获取FF微博新闻
 7. 新物品 物品名：查物品异常时可以尝试这个版本
@@ -18,58 +21,81 @@
 
 ## chatgpt聊天功能
 
 前提：该电脑或服务器科学上网(才能连接上chatgpt_api)，有chatgpt账号。
 
 指令：`塔塔露问问 你想说的话`，例如`塔塔露问问 武士是ff14里的最强职业吗`
 
-设置：代码见`src/plugins/chat_ai.py`，将`on_chat`改为`True`开启该功能，将`openai.api_key`替换为自己的chatgpt key。`max_tokens`为最长回复字数，
-防止烧钱过快。其他设定见chatgpt_api的官方文档或者网上的调教文章。
+设置：配置文件`tatarubot2_conf.json`里开启该插件功能后，`"api_key"`改为自己的chatgpt api key。
 
 chatgpt_api官方文档：https://platform.openai.com/docs/api-reference/chat
 
 ## 依赖
 
 1. python >= 3.7.3
 2. 如果有NoneBot v1则卸载 `pip uninstall nonebot`
 3. 本代码测试使用的NoneBot版本是 nonebot2==2.0.0b4
 
+↑↑↑ 既然是作为nonebot2的插件，上面的1.2.3.你应该都已经达到了，姑且放在这里提一下
+
+4. 如果要用chatgpt则多安装一个`pip install openai`
+
 ## 使用
 
-1. 安装脚手架nb-cli
+1. 安装塔塔露机器人插件包
 
    ```shell
-   pip install nb-cli
-   
-   # 国内速度慢可以用阿里源加速，或者别的源，命令如下
-   pip install nb-cli -i https://mirrors.aliyun.com/pypi/simple/
+   # 为了防止出啥意外先把旧的删了吧
+   pip uninstall tatarubot2
+   # 安装最新插件
+   pip install -U tatarubot2
    ```
 
-2. 安装适配器
+2. 进入你的机器人文件夹，根据需要修改配置文件`.env.dev`，更多信息见NoneBot2官方文档
 
-   ```
-   nb adapter install nonebot-adapter-onebot
+   ```shell
+   # 注意配置命令起始字符
+   # 我的习惯是直接纯中文作为命令，所以添加了一个空 ""，如下所示
+   COMMAND_START=["/", ""]  
    ```
 
-3. 下载本项目代码，并进入文件夹
+3. 在`bot.py`中加载插件
 
+   ```python
+   nonebot.load_builtin_plugins("tatarubot2")
    ```
-   git clone https://github.com/aaron-lii/TataruBot2.git
-   cd TataruBot2
-   ```
+   
+5. 首次启动机器人，会自动在机器人文件夹内生成一个插件的配置文件`tatarubot2_conf.json`
 
-4. 根据需要修改配置文件`.env.dev`，更多信息见NoneBot2官方文档
+   ```shell
+   nb run
+   ```
 
-5. 启动机器人
+6. 根据需要选择开启哪些插件，修改`tatarubot2_conf.json`，下面是插件对应的配置词条名
 
    ```
+   1. 暖暖：nuannuan
+   2. 选门：precious
+   3. 仙人彩：lottery
+   4. 物品 物品名：item
+   5. 价格 大区 物品名：market
+   6. 看看微博：ff_weibo
+   7. 新物品 物品名：item_new
+   8. 新价格 大区 物品名：market_new
+   9. 房子 服务器名 主城名 房子大小：house
+   10. 输出 boss名 职业名 (国服) (rdps) (day2)：logs_dps
+   ```
+
+7. 启动机器人
+
+   ```shell
    nb run
    ```
 
-6. 使用go-cqhttp连接机器人，该部分参考go-cqhttp官方文档。需要注意的是配置中反向websocket设置参考文档https://adapter-onebot.netlify.app/docs/guide/setup
+8. 使用go-cqhttp连接机器人，该部分参考go-cqhttp官方文档。需要注意的是配置中反向websocket设置参考文档https://adapter-onebot.netlify.app/docs/guide/setup
 
 ## 备注
 
 NoneBot2官方文档：https://v2.nonebot.dev/
 
 NoneBot2 github：https://github.com/nonebot/nonebot2
```

### Comparing `tatarubot2-0.1.6/tatarubot2/data/boss.json` & `tatarubot2-0.1.7/tatarubot2/data/boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/data/item_dict.json` & `tatarubot2-0.1.7/tatarubot2/data/item_dict.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/data/job.json` & `tatarubot2-0.1.7/tatarubot2/data/job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/__init__.py` & `tatarubot2-0.1.7/tatarubot2/plugins/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 """
 json_path = "./tatarubot2_conf.json"
 
 if os.path.exists(json_path):
     with open(json_path, "r", encoding="utf-8") as f_r:
         plugins_dict = json.load(f_r)
 else:
-    plugins_dict = {"chat_ai": False,
+    plugins_dict = {
+                "chat_ai": False,
+                "api_key": "这里填你自己的chatgpt账号aip key，需要魔法上网",
                 "ff_weibo": True,
                 "house": True,
                 "item": True,
                 "item_new": True,
                 "logs_dps": True,
                 "lottery": True,
                 "market": True,
@@ -26,14 +28,15 @@
         json.dump(plugins_dict, f_w, ensure_ascii=False, indent=2)
 
 """
 加载指定插件
 """
 if plugins_dict["chat_ai"]:
     from .chat_ai import *
+    openai.api_key = plugins_dict["api_key"]
 if plugins_dict["ff_weibo"]:
     from .ff_weibo import *
 if plugins_dict["house"]:
     from .house import *
 if plugins_dict["item"]:
     from .item import *
 if plugins_dict["item_new"]:
```

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/auto_response.py` & `tatarubot2-0.1.7/tatarubot2/plugins/auto_response.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/bot_help.py` & `tatarubot2-0.1.7/tatarubot2/plugins/bot_help.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/chat_ai.py` & `tatarubot2-0.1.7/tatarubot2/plugins/chat_ai.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,44 @@
 from nonebot.rule import to_me
 from nonebot.typing import T_State
 from nonebot.adapters import Bot, Event
 
 import openai
 
 # 控制是否开启该功能
-on_chat = False
+# on_chat = False
 
 this_command = "问问 "
 chat_ai = on_command(this_command, rule=to_me(), priority=5)
 
-openai.api_key = "这里填你自己的chatgpt账号aip key"
+# openai.api_key = "这里填你自己的chatgpt账号aip key"
 
 async def chat_run(args):
+    # print(openai.api_key)
 
     completion = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "system", "content": "你是FF14里面的角色塔塔露.也是我的小助手,请简洁地回答我的问题,不需要复杂的解释."},
             {"role": "user", "content": args}
         ],
-        max_tokens=200
+        # max_tokens=200
     )
     res = completion.choices[0].message
     if "content" in res:
         res = res["content"].strip()
     else:
         res = "不懂呢！"
     return res
 
 
 @chat_ai.handle()
 async def handle_first_receive(bot: Bot, event: Event, state: T_State):
-    if not on_chat:
-        return
+    # if not on_chat:
+    #     return
     args = str(event.get_message()).strip().split(this_command, 1)
     if len(args) < 2:
         return
 
     return_str = await chat_run(args[1])
     await chat_ai.finish(return_str)
```

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/ff_weibo.py` & `tatarubot2-0.1.7/tatarubot2/plugins/ff_weibo.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/house.py` & `tatarubot2-0.1.7/tatarubot2/plugins/house.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/item.py` & `tatarubot2-0.1.7/tatarubot2/plugins/item.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/item_new.py` & `tatarubot2-0.1.7/tatarubot2/plugins/item_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/logs_dps.py` & `tatarubot2-0.1.7/tatarubot2/plugins/logs_dps.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/lottery.py` & `tatarubot2-0.1.7/tatarubot2/plugins/lottery.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/market.py` & `tatarubot2-0.1.7/tatarubot2/plugins/market.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/market_new.py` & `tatarubot2-0.1.7/tatarubot2/plugins/market_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/nuannuan.py` & `tatarubot2-0.1.7/tatarubot2/plugins/nuannuan.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/precious.py` & `tatarubot2-0.1.7/tatarubot2/plugins/precious.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/plugins/weather.py` & `tatarubot2-0.1.7/tatarubot2/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/data.json` & `tatarubot2-0.1.7/tatarubot2/tools/data.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/download_boss.py` & `tatarubot2-0.1.7/tatarubot2/tools/download_boss.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/download_item2id.py` & `tatarubot2-0.1.7/tatarubot2/tools/download_item2id.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/new_boss.json` & `tatarubot2-0.1.7/tatarubot2/tools/new_boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/new_job.json` & `tatarubot2-0.1.7/tatarubot2/tools/new_job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.6/tatarubot2/tools/normal_data.py` & `tatarubot2-0.1.7/tatarubot2/tools/normal_data.py`

 * *Files identical despite different names*

