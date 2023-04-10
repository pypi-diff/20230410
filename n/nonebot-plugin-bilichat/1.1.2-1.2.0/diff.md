# Comparing `tmp/nonebot_plugin_bilichat-1.1.2.tar.gz` & `tmp/nonebot_plugin_bilichat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.1.2.tar", last modified: Mon Apr 10 14:54:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.2.0.tar", last modified: Mon Apr 10 16:24:58 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.1.2.tar` & `nonebot_plugin_bilichat-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-04-10 14:54:40.221422 nonebot_plugin_bilichat-1.1.2/LICENSE
--rw-r--r--   0        0        0     5965 2023-04-10 14:54:40.221422 nonebot_plugin_bilichat-1.1.2/README.md
--rw-r--r--   0        0        0     8397 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      289 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      866 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     2212 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/content_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     1764 2023-04-10 14:54:40.229421 nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1184 2023-04-10 14:54:51.373477 nonebot_plugin_bilichat-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6953 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-10 16:24:50.045187 nonebot_plugin_bilichat-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6703 2023-04-10 16:24:50.045187 nonebot_plugin_bilichat-1.2.0/README.md
+-rw-r--r--   0        0        0     7031 2023-04-10 16:24:50.049187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4394 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      289 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0      406 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     3544 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2457 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1311 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1344 2023-04-10 16:24:58.421182 nonebot_plugin_bilichat-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7992 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.1.2/LICENSE` & `nonebot_plugin_bilichat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/README.md` & `nonebot_plugin_bilichat-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -56,20 +56,14 @@
 - 💰 如果终端机价格做到1500-2000元，竞争力还是很足的。
 - 🧪 高通自己也意识到骁龙7系列的竞争力问题，这也使其成了必须要解决的一个问题。
 - 🕹️ 7+ Gen2就是8+的CPU，旗舰规格下放，最大的受益者是大型游戏。
 ```
 
 </details>
 
-## 📝 TODO
-
-- [x] 简易的黑(白)名单系统
-- [ ] 更好的权限控制系统
-- [ ] 图片形式发送视频总结
-
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-bilichat[all]
@@ -109,30 +103,37 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置, 配置均为**非必须项**
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_block              | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
-| bilichat_enable_private     | bool      | True                 | 是否允许响应私聊 |
-| bilichat_enable_v12_channel | bool      | True                 | 是否允许响应频道消息(ob12专属) |
-| bilichat_enable_unkown_src  | bool      | False                | 是否允许响应未知来源的消息 |
-| bilichat_whitelist          | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
-| bilichat_blacklist          | list[str] | []                   | **不响应**的群聊(频道)名单 |
-| bilichat_dynamic_font       | str       | None                 | 视频信息及词云图片使用的字体 |
-| bilichat_cd_time            | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
-| bilichat_forword_msg        | set[str]  | ()                   | 对什么类型的消息开启合并转发(ob11专属),包含 `info`、`wordcloud`、`summary` 三个可选项 |
-| nickname                    | set[str]  | ("awesome-nonebot",) | 合并转发中,bot的昵称(取第一个值) |
-| bilichat_use_bcut_asr       | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
-| bilichat_word_cloud         | bool      | True                 | 是否开启词云功能 |
-| bilichat_openai_token       | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
-| bilichat_openai_proxy       | str       | None                 | 访问openai使用的代理地址 |
-| bilichat_openai_model       | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
-| bilichat_openai_token_limit | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_block               | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
+| bilichat_enable_private      | bool      | True                 | 是否允许响应私聊 |
+| bilichat_enable_v12_channel  | bool      | True                 | 是否允许响应频道消息(ob12专属) |
+| bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
+| bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
+| bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
+| bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
+| bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
+| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
+| bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
+| bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE))
+| bilichat_newbing_token_limit | int       | 0                    | 请求的文本量上限, 0为无上限 |
+
+注:
+
+1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
+2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `chatgpt` 进行总结
+3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
+4. 由于 newbing 限制较大，也不如 chatgpt 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -13,49 +13,58 @@
 ð® æ°çAdreno
 700æ¶æGPUè§æ ¼æ§è½å¼ºï¼æ¯ä¸ä¸ä»£7Gen1å¼ºäºè¶è¿ä¸åã - ð
 è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
 å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
 é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
 - ð¹ï¸ 7+
 Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
-```  ## ð TODO - [x] ç®æçé»(ç½)ååç³»ç» - [ ]
-æ´å¥½çæéæ§å¶ç³»ç» - [ ] å¾çå½¢å¼åéè§é¢æ»ç» ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat[all]
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-
-bilichat[all]   poetry poetry add nonebot-plugin-bilichat[all]   conda conda
-install nonebot-plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
+è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-bilichat[all]   pdm
+pdm add nonebot-plugin-bilichat[all]   poetry poetry add nonebot-plugin-
+bilichat[all]   conda conda install nonebot-plugin-bilichat[all]  æå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®,
+éç½®åä¸º**éå¿é¡»é¡¹** | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:----
+-:|:----:|:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_forword_msg | set[str] | () |
-å¯¹ä»ä¹ç±»åçæ¶æ¯å¼å¯åå¹¶è½¬å(ob11ä¸å±),åå«
-`info`ã`wordcloud`ã`summary` ä¸ä¸ªå¯éé¡¹ | | nickname | set[str] |
-("awesome-nonebot",) | åå¹¶è½¬åä¸­,botçæµç§°(åç¬¬ä¸ä¸ªå¼) | |
-bilichat_use_bcut_asr | bool | True |
+(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
-è®¿é®openaiä½¿ç¨çä»£çå°å | | bilichat_openai_model | str | gpt-3.5-
-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | | bilichat_openai_token_limit | int
-| 3500 | è¯·æ±çææ¬éä¸é, è®¡ç®æ¹å¼å¯åè[tiktoken](https://
-github.com/openai/tiktoken) | ## ð ä½¿ç¨ ç´æ¥åéè§é¢
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
+è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | |
+bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
+(è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
+authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) | bilichat_newbing_token_limit
+| int | 0 | è¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | æ³¨: 1.
+~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
+2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
+`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `chatgpt` è¿è¡æ»ç» 3.
+ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
+token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
+tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
+token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 4. ç±äº newbing
+éå¶è¾å¤§ï¼ä¹ä¸å¦ chatgpt
+å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
+~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
 (ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
 æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ | æä»¤ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æä»¤1 | ä¸»äºº |
 å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å | æ¯ | ç¾¤è | æä»¤è¯´æ
 | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
```

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,20 @@
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_video_basic, get_video_cache
 from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
 
-if plugin_config.bilichat_openai_token:
-    from .summary.content_summarise import openai_summarization
+if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
+    ENABLE_SUMMARY = True
+    from .summary import summarization
+else:
+    ENABLE_SUMMARY = False
+
 if plugin_config.bilichat_word_cloud:
     from .wordcloud.wordcloud import wordcloud
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="一个通过 OpenAI 来对b站视频进行总结插件",
     usage="直接发送视频链接即可",
@@ -84,99 +88,68 @@
 async def get_bili_number_b23(state: T_State):
     if matched := re.search(
         r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])  # type: ignore
     ):
         state["bili_number"] = matched.group()
 
 
-async def forword_msg_v11(bot: V11_Bot, event: V11_ME, forword_list: V11_Message):
-    msgs = [
-        {"type": "node", "data": {"name": plugin_config.nickname[0], "uin": bot.self_id, "content": msg}}
-        for msg in forword_list
-    ]
-    if isinstance(event, V11_GME):
-        await bot.send_group_forward_msg(id=str(event.group_id), messages=msgs)
-    else:
-        await bot.send_private_forward_msg(id=str(event.user_id), messages=msgs)
-    raise FinishedException
-
-
 @bili.handle()
 @b23.handle()
 async def video_info_v11(bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher):
     # sourcery skip: raise-from-previous-error
-    forword_list: V11_Message = []  # type: ignore
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg or not info:
         await matcher.finish()
     reply = V11_MS.reply(event.message_id)
     if not img:
         await matcher.finish(reply + msg)
     image = V11_MS.image(img)
-    if "info" in plugin_config.bilichat_forword_msg:
-        forword_list.append(image + msg)  # type: ignore
-        reply = ""
-    else:
-        msgid = (await matcher.send(reply + image + msg))["message_id"]
-        reply = V11_MS.reply(msgid)
+    msgid = (await matcher.send(reply + image + msg))["message_id"]
+    reply = V11_MS.reply(msgid)
 
     # furtuer fuctions
     if not plugin_config.bilichat_openai_token and not plugin_config.bilichat_word_cloud:
         raise FinishedException
 
     # get video cache
     try:
         cache = await get_video_cache(info)
     except AbortError as e:
         logger.exception(e)
-        if "info" in plugin_config.bilichat_forword_msg:
-            forword_list.append(f"视频字幕获取失败: {str(e)}")
-            await forword_msg_v11(bot, event, forword_list)
-            raise FinishedException
-        else:
-            await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
+        await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
-        if "info" in plugin_config.bilichat_forword_msg:
-            forword_list.append(f"未知错误: {e}")
-            await forword_msg_v11(bot, event, forword_list)
-            raise FinishedException
-        else:
-            await matcher.finish(f"{reply}未知错误: {e}")
+        await matcher.finish(f"{reply}未知错误: {e}")
 
     # wordcloud
+    wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-            if "wordcloud" in plugin_config.bilichat_forword_msg:
-                forword_list.append(V11_MS.image(image))
-            else:
-                await matcher.send(reply + V11_MS.image(image))
-        elif "wordcloud" in plugin_config.bilichat_forword_msg:
-            forword_list.append("视频无有效字幕")
-            await forword_msg_v11(bot, event, forword_list)
+            wc_image = V11_MS.image(image)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
     # summary
-    if plugin_config.bilichat_openai_token:
-        if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
-            if "summary" in plugin_config.bilichat_forword_msg:
-                forword_list.append(summary)
-            else:
-                await matcher.send(reply + summary)
-        elif "summary" in plugin_config.bilichat_forword_msg:
-            forword_list.append("视频无有效字幕")
-            await forword_msg_v11(bot, event, forword_list)
+    summary = ""
+    if ENABLE_SUMMARY:
+        if summary := await summarization(cache=cache, cid=str(info["cid"])):
+            if isinstance(summary, bytes):
+                summary = V11_MS.image(summary)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
-    if forword_list:
-        await forword_msg_v11(bot, event, forword_list)
+    if wc_image or summary:
+        await matcher.finish(reply + wc_image + summary)
+
+
+async def get_image_v12(bot: V12_Bot, bili_number: str, suffix: str, data):
+    fileid = await bot.upload_file(type="data", name=f"{bili_number}_{suffix}.jpg", data=data)
+    return V12_MS.image(file_id=fileid["file_id"])
 
 
 @bili.handle()
 @b23.handle()
 async def video_info_v12(bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher):
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
@@ -184,37 +157,42 @@
         await matcher.finish()
     reply = V12_MS.reply(message_id=event.message_id, user_id=event.get_user_id())
     if not img or not info:
         await matcher.finish(reply + msg)
     fileid = await bot.upload_file(type="data", name=f"{state['bili_number']}.jpg", data=img)
     image = V12_MS.image(file_id=fileid["file_id"])
     msgid = (await matcher.send(reply + image + msg))["message_id"]
+    reply = V12_MS.reply(msgid)
 
     # furtuer fuctions
-    if not (plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud):
+    if not plugin_config.bilichat_openai_token and not plugin_config.bilichat_word_cloud:
         raise FinishedException
 
-    reply = V12_MS.reply(message_id=msgid, user_id=bot.self_id)
     try:
         cache = await get_video_cache(info)
     except AbortError as e:
         logger.exception(e)
         await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {str(e)}")
 
     # wordcloud
+    wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-            fileid = await bot.upload_file(type="data", name=f"{state['bili_number']}_wc.jpg", data=image)
-            await matcher.send(reply + V12_MS.image(file_id=fileid["file_id"]))
+            wc_image = await get_image_v12(bot, state["bili_number"], "wc", data=image)
         else:
-            await matcher.finish(f"{reply}视频无有效字幕")
+            await matcher.send(f"{reply}视频无有效字幕")
 
     # summary
-    if plugin_config.bilichat_openai_token:
-        if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
-            await matcher.send(reply + summary)
+    summary = ""
+    if ENABLE_SUMMARY:
+        if summary := await summarization(cache=cache, cid=str(info["cid"])):
+            if isinstance(summary, bytes):
+                summary = await get_image_v12(bot, state["bili_number"], "summary", data=summary)
         else:
-            await matcher.finish(f"{reply}视频无有效字幕")
+            await matcher.send(f"{reply}视频无有效字幕")
+
+    if wc_image or summary:
+        await matcher.finish(reply + wc_image + summary)  # type: ignore
```

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import importlib.util
 import sys
-from typing import Literal, Optional, Sequence, Union, Set
+from typing import Literal, Optional, List, Union
+from pathlib import Path
+import json
 
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseModel, validator
 
 # get package version
 if sys.version_info < (3, 10):
@@ -20,55 +22,41 @@
 
 class Config(BaseModel):
     # general
     bilichat_block: bool = False
     bilichat_enable_private: bool = True
     bilichat_enable_v12_channel: bool = True
     bilichat_enable_unkown_src: bool = False
-    bilichat_whitelist: Sequence[str] = []
-    bilichat_blacklist: Sequence[str] = []
+    bilichat_whitelist: List[str] = []
+    bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
-    bilichat_forword_msg: Sequence[str] = []  # ("info", "wordcloud", "summary")
-    nickname: Sequence[str] = ["awesome-nonebot"]
+    nickname: List[str] = ["awesome-nonebot"]
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
 
     # AI Summary
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
     bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
-
-    @validator("bilichat_forword_msg")
-    def check_adapter_can_send_forword_msg(cls, v):
-        if not v:
-            return
-        drivers = get_driver()._adapters.keys()
-        if "OneBot V12" in drivers:
-            logger.warning(
-                "Forword_msg is not implemented by OneBot V12, events of OneBot V12 will not be sent as forword_msg!"
-            )
-        if "OneBot V11" in drivers:
-            logger.warning(
-                "Using forward_msg may cause serious risk control restrictions, please enable this feature with caution!"
-            )
-        return v
+    bilichat_newbing_cookie: Optional[str]
+    bilichat_newbing_token_limit: int = 0
 
     @validator("nickname")
     def check_nickname(cls, v):
         return list(v) or ["awesome-nonebot"]
 
     @validator("bilichat_openai_proxy")
     def check_openai_proxy(cls, v, values):
-        if values["bilichat_openai_token"] is None:
+        if not (values["bilichat_openai_token"] or values["bilichat_newbing_cookie"]):
             return v
         if v is None:
             logger.warning("you have enabled openai summary without a proxy, this may cause request failure.")
         return v
 
     @validator("bilichat_openai_token_limit")
     def check_token_limit(cls, v, values):
@@ -87,21 +75,39 @@
                 f"Model {model} has a token cap of {max_limit} instead of {v}, token will be replaced with {max_limit}"
             )
             v = max_limit
         return v
 
     @validator("bilichat_openai_token", always=True)
     def check_pypackage_openai(cls, v):
-        if importlib.util.find_spec("tiktoken_async") or not v:
+        if (importlib.util.find_spec("tiktoken_async") and importlib.util.find_spec("minidynamicrender")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction openai summary not installed, use **nb plugin install nonebot-plugin-bilichat[openai]** to install required dependencies"
             )
 
+    @validator("bilichat_newbing_cookie", always=True)
+    def check_pypackage_newbing_and_cookie(cls, v):
+        if not v:
+            return v
+        if not importlib.util.find_spec("EdgeGPT") or not importlib.util.find_spec("minidynamicrender"):
+            raise RuntimeError(
+                "Package(s) of fuction newbing summary not installed, use **nb plugin install nonebot-plugin-bilichat[newbing]** to install required dependencies"
+            )
+
+        # verify cookie file
+        try:
+            if Path(v).is_file():
+                json.loads(Path(v).read_text("utf-8"))
+        except Exception as e:
+            raise ValueError("Config bilichat_newbing_cookie got a problem occurred") from e
+
+        return v
+
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction wordcloud not installed, use **nb plugin install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
```

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class Episode(BaseModel):
     title: Optional[str]
     content: List[str]
     jieba: Optional[Dict]
     openai: Optional[str]
+    newbing: Optional[str]
 
 
 class Cache(BaseModel):
     id: str
     title: str
     episodes: Dict[str, Episode]
```

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/content_summarise.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 from typing import List
 
 from loguru import logger
 
 from .openai import get_small_size_transcripts, get_user_prompt, openai_req
+from .text_to_image import rich_text2image
 from ..model.cache import Cache
 from ..model.exception import AbortError
-from ..optional import capture_exception
+from ..optional import capture_exception  # type: ignore
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
     small_size_transcripts = get_small_size_transcripts(sub)
     prompt = get_user_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
@@ -38,16 +39,19 @@
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
             if ai_summary.summary:
                 cache.episodes[cid].openai = ai_summary.summary
                 cache.save()
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
-                return None
-        return cache.episodes[cid].openai or "视频无法总结"  # TODO: add image type output
+                return f"视频(专栏) {cache.id} 总结失败: {ai_summary.raw}"
+        if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结"):
+            return img
+        else:
+            return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].openai}"
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
     except Exception as e:
         capture_exception()
         logger.exception(f"Video(Column) {cache.id} summary failed: {e}")
         return f"视频(专栏) {cache.id} 总结失败: {e}"
```

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.1.2/pyproject.toml` & `nonebot_plugin_bilichat-1.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.1.2"
+version = "1.2.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
@@ -45,19 +45,26 @@
 ]
 wordcloud = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
 ]
 openai = [
     "tiktoken-async>=0.3.2",
+    "minidynamicrender>=1.1.9",
+]
+newbing = [
+    "EdgeGPT>=0.1.22.1",
+    "minidynamicrender>=1.1.9",
 ]
 all = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
     "tiktoken-async>=0.3.2",
+    "EdgeGPT>=0.1.22.1",
+    "minidynamicrender>=1.1.9",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_bilichat-1.1.2/PKG-INFO` & `nonebot_plugin_bilichat-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.1.2
+Version: 1.2.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -12,20 +12,26 @@
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
+Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
+Requires-Dist: EdgeGPT>=0.1.22.1; extra == "newbing"
+Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
 Requires-Dist: jieba>=0.42.1; extra == "all"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "all"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "all"
+Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all"
+Requires-Dist: minidynamicrender>=1.1.9; extra == "all"
 Provides-Extra: extra
 Provides-Extra: wordcloud
 Provides-Extra: openai
+Provides-Extra: newbing
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="docs/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="docs/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -83,20 +89,14 @@
 - 💰 如果终端机价格做到1500-2000元，竞争力还是很足的。
 - 🧪 高通自己也意识到骁龙7系列的竞争力问题，这也使其成了必须要解决的一个问题。
 - 🕹️ 7+ Gen2就是8+的CPU，旗舰规格下放，最大的受益者是大型游戏。
 ```
 
 </details>
 
-## 📝 TODO
-
-- [x] 简易的黑(白)名单系统
-- [ ] 更好的权限控制系统
-- [ ] 图片形式发送视频总结
-
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-bilichat[all]
@@ -136,30 +136,37 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置, 配置均为**非必须项**
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_block              | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
-| bilichat_enable_private     | bool      | True                 | 是否允许响应私聊 |
-| bilichat_enable_v12_channel | bool      | True                 | 是否允许响应频道消息(ob12专属) |
-| bilichat_enable_unkown_src  | bool      | False                | 是否允许响应未知来源的消息 |
-| bilichat_whitelist          | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
-| bilichat_blacklist          | list[str] | []                   | **不响应**的群聊(频道)名单 |
-| bilichat_dynamic_font       | str       | None                 | 视频信息及词云图片使用的字体 |
-| bilichat_cd_time            | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
-| bilichat_forword_msg        | set[str]  | ()                   | 对什么类型的消息开启合并转发(ob11专属),包含 `info`、`wordcloud`、`summary` 三个可选项 |
-| nickname                    | set[str]  | ("awesome-nonebot",) | 合并转发中,bot的昵称(取第一个值) |
-| bilichat_use_bcut_asr       | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
-| bilichat_word_cloud         | bool      | True                 | 是否开启词云功能 |
-| bilichat_openai_token       | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
-| bilichat_openai_proxy       | str       | None                 | 访问openai使用的代理地址 |
-| bilichat_openai_model       | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
-| bilichat_openai_token_limit | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_block               | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
+| bilichat_enable_private      | bool      | True                 | 是否允许响应私聊 |
+| bilichat_enable_v12_channel  | bool      | True                 | 是否允许响应频道消息(ob12专属) |
+| bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
+| bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
+| bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
+| bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
+| bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
+| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
+| bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
+| bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE))
+| bilichat_newbing_token_limit | int       | 0                    | 请求的文本量上限, 0为无上限 |
+
+注:
+
+1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
+2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `chatgpt` 进行总结
+3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
+4. 由于 newbing 限制较大，也不如 chatgpt 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
 jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
 "wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-
-Dist: jieba>=0.42.1; extra == "all" Requires-Dist: wordcloud>=1.8.2.2; extra ==
-"all" Requires-Dist: tiktoken-async>=0.3.2; extra == "all" Provides-Extra:
-extra Provides-Extra: wordcloud Provides-Extra: openai Provides-Extra: all
+Dist: minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
+EdgeGPT>=0.1.22.1; extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9;
+extra == "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
+wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
+== "all" Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
+minidynamicrender>=1.1.9; extra == "all" Provides-Extra: extra Provides-Extra:
+wordcloud Provides-Extra: openai Provides-Extra: newbing Provides-Extra: all
 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
                            [license] [pypi] [python]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
@@ -27,49 +31,58 @@
 ð® æ°çAdreno
 700æ¶æGPUè§æ ¼æ§è½å¼ºï¼æ¯ä¸ä¸ä»£7Gen1å¼ºäºè¶è¿ä¸åã - ð
 è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
 å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
 é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
 - ð¹ï¸ 7+
 Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
-```  ## ð TODO - [x] ç®æçé»(ç½)ååç³»ç» - [ ]
-æ´å¥½çæéæ§å¶ç³»ç» - [ ] å¾çå½¢å¼åéè§é¢æ»ç» ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat[all]
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-
-bilichat[all]   poetry poetry add nonebot-plugin-bilichat[all]   conda conda
-install nonebot-plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
+install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
+è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-bilichat[all]   pdm
+pdm add nonebot-plugin-bilichat[all]   poetry poetry add nonebot-plugin-
+bilichat[all]   conda conda install nonebot-plugin-bilichat[all]  æå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®,
+éç½®åä¸º**éå¿é¡»é¡¹** | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:----
+-:|:----:|:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_forword_msg | set[str] | () |
-å¯¹ä»ä¹ç±»åçæ¶æ¯å¼å¯åå¹¶è½¬å(ob11ä¸å±),åå«
-`info`ã`wordcloud`ã`summary` ä¸ä¸ªå¯éé¡¹ | | nickname | set[str] |
-("awesome-nonebot",) | åå¹¶è½¬åä¸­,botçæµç§°(åç¬¬ä¸ä¸ªå¼) | |
-bilichat_use_bcut_asr | bool | True |
+(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
-è®¿é®openaiä½¿ç¨çä»£çå°å | | bilichat_openai_model | str | gpt-3.5-
-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | | bilichat_openai_token_limit | int
-| 3500 | è¯·æ±çææ¬éä¸é, è®¡ç®æ¹å¼å¯åè[tiktoken](https://
-github.com/openai/tiktoken) | ## ð ä½¿ç¨ ç´æ¥åéè§é¢
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
+è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | |
+bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
+(è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
+authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) | bilichat_newbing_token_limit
+| int | 0 | è¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | æ³¨: 1.
+~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
+2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
+`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `chatgpt` è¿è¡æ»ç» 3.
+ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
+token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
+tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
+token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 4. ç±äº newbing
+éå¶è¾å¤§ï¼ä¹ä¸å¦ chatgpt
+å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
+~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
 (ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
 æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ | æä»¤ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æä»¤1 | ä¸»äºº |
 å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å | æ¯ | ç¾¤è | æä»¤è¯´æ
 | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
```

