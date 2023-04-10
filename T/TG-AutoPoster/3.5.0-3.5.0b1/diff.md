# Comparing `tmp/TG_AutoPoster-3.5.0.tar.gz` & `tmp/TG_AutoPoster-3.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TG_AutoPoster-3.5.0.tar", last modified: Mon Apr 10 09:33:19 2023, max compression
+gzip compressed data, was "TG_AutoPoster-3.5.0b1.tar", last modified: Tue Jan 17 17:22:37 2023, max compression
```

## Comparing `TG_AutoPoster-3.5.0.tar` & `TG_AutoPoster-3.5.0b1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.569603 TG_AutoPoster-3.5.0/TG_AutoPoster/
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/TG_AutoPoster.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/inline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:33:19.569603 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-10 09:33:19.000000 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-10 09:33:19.000000 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:33:19.000000 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-10 09:33:19.000000 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 09:33:19.000000 TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 09:33:19.573603 TG_AutoPoster-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-10 09:33:07.000000 TG_AutoPoster-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.525045 TG_AutoPoster-3.5.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-01-17 17:22:37.525045 TG_AutoPoster-3.5.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.517045 TG_AutoPoster-3.5.0b1/TG_AutoPoster/
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/TG_AutoPoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.521045 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/inline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.521045 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.521045 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.525045 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:22:37.517045 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-01-17 17:22:37.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-17 17:22:37.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:22:37.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-17 17:22:37.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-17 17:22:37.000000 TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 17:22:37.525045 TG_AutoPoster-3.5.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-17 17:22:25.000000 TG_AutoPoster-3.5.0b1/setup.py
```

### Comparing `TG_AutoPoster-3.5.0/LICENCE.md` & `TG_AutoPoster-3.5.0b1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/PKG-INFO` & `TG_AutoPoster-3.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TG_AutoPoster
-Version: 3.5.0
+Version: 3.5.0b1
 Summary: Telegram Bot for reposting from VK
 Home-page: https://github.com/qwertyadrian/TG_AutoPoster
 Download-URL: https://github.com/qwertyadrian/TG_AutoPoster/releases/latest
 Author: qwertyadrian
 Author-email: me@qwertyadrian.ru
 License: MIT License
 Platform: OS Independent
```

### Comparing `TG_AutoPoster-3.5.0/README.md` & `TG_AutoPoster-3.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/TG_AutoPoster.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/TG_AutoPoster.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/__main__.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/__main__.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/callback.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/callback.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/commands.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -166,96 +166,54 @@
     & pyrogram.filters.private
     & tools.is_admin
 )
 def update_stoplist(bot: AutoPoster, message: Message):
     domain = message.command[1] if len(message.command) >= 2 else "global"
     if domain != "global":
         if domain not in bot.config["domains"].keys():
-            message.reply(f"Источник `{domain}` не найден.")
+            message.reply(f"Источник {domain} не найден.")
             return
     bot.conversations.update(
         {message.from_user.id: ("stop_list", domain)}
     )
     message.reply(messages.STOPLIST_UPDATE)
 
 
 @AutoPoster.on_message(
-    pyrogram.filters.command(commands=["delete_stoplist", "delete_blacklist"])
-    & pyrogram.filters.private
-    & tools.is_admin
-)
-def delete_stoplist(bot: AutoPoster, message: Message):
-    bot.reload_config()
-    if message.command[0].split("_")[1] == "stoplist":
-        filetype = "stop_list"
-    else:
-        filetype = "blacklist"
-
-    domain = message.command[1] if len(message.command) >= 2 else "global"
-    if domain == "global":
-        if filetype in bot.config.get("settings", {}).keys():
-            os.remove(bot.config["settings"][filetype])
-            bot.config["settings"].pop(filetype)
-    else:
-        if domain in bot.config["domains"].keys():
-            if filetype in bot.config["domains"][domain].keys():
-                os.remove(bot.config["domains"][domain][filetype])
-                bot.config["domains"][domain].pop(filetype)
-        else:
-            message.reply(f"Источник `{domain}` не найден.")
-            return
-
-    message.reply(
-        getattr(messages, f"{filetype.replace('_', '').upper()}_DELETED")
-    )
-    bot.save_config()
-
-
-@AutoPoster.on_message(
     pyrogram.filters.command(commands=["update_blacklist"])
     & pyrogram.filters.private
     & tools.is_admin
 )
 def update_blacklist(bot: AutoPoster, message: Message):
     domain = message.command[1] if len(message.command) >= 2 else "global"
-    if domain != "global":
-        if domain not in bot.config["domains"].keys():
-            message.reply(f"Источник `{domain}` не найден.")
-            return
     bot.conversations.update(
         {message.from_user.id: ("blacklist", domain)}
     )
     message.reply(messages.BLACKLIST_UPDATE)
 
 
 @AutoPoster.on_message(
     pyrogram.filters.command(commands=["restart"])
     & pyrogram.filters.private
     & tools.is_admin
 )
 def restart(bot: AutoPoster, message: Message):
-    if sys.platform.startswith("win32"):
-        message.reply("Команда не доступна в Windows.")
-    else:
-        message.reply("Перезапуск бота...")
-        os.chdir(bot.config_path.parent)
-        os.execv(sys.executable, [sys.executable] + sys.argv)
+    message.reply("Перезапуск бота...")
+    os.chdir(bot.config_path.parent)
+    os.execv(sys.executable, [sys.executable] + sys.argv)
 
 
 @AutoPoster.on_message(
     pyrogram.filters.command(commands=["exit"])
     & pyrogram.filters.private
     & tools.is_admin
 )
 def exit_(_, message: Message):
-    if sys.platform.startswith("win32"):
-        message.reply("Команда не доступна в Windows.")
-    else:
-        message.reply("Завершение работы...")
-        sys.exit(0)
+    message.reply("Завершение работы...")
+    sys.exit(0)
 
 @AutoPoster.on_message(
     pyrogram.filters.command(commands=["cancel"]) & pyrogram.filters.private
 )
 def cancel(bot: AutoPoster, message: Message):
     if message.from_user.id in bot.conversations.keys():
         message.reply("Операция отменена.")
```

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/handlers.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,28 @@
     bot.reload_config()
     if domain == "global":
         global_stoplist = Path(bot.config.get("settings", {}).get(
             filetype,
             bot.config_path.parent / f"{filetype}_global.txt"
         ))
         bot.config.get("settings", {})[filetype] = str(global_stoplist)
-        with global_stoplist.open("a", encoding="utf-8") as f:
+        with global_stoplist.open("a") as f:
             f.write(message.text + "\n")
     else:
         domain_clear = re.sub(r"https://(m\.)?vk\.com/", "", domain)
         domain_stoplist = Path(bot.config["domains"][domain].get(
             filetype,
             bot.config_path.parent / f"{filetype}_{domain_clear}.txt"
         ))
         bot.config["domains"][domain][filetype] = str(domain_stoplist)
-        with domain_stoplist.open("a", encoding="utf-8") as f:
+        with domain_stoplist.open("a") as f:
             f.write(message.text + "\n")
     bot.save_config()
 
 
-@AutoPoster.on_message(pyrogram.filters.forwarded & pyrogram.filters.private)
+@AutoPoster.on_message(pyrogram.filters.forwarded)
 def get_forward_id(_, message: Message):
     if message.forward_from:
         id_ = message.forward_from.id
     else:
         id_ = message.forward_from_chat.id
     message.reply("Channel (user) ID is `{}`".format(id_))
```

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/plugins/inline.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/plugins/inline.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/messages.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 ACCESS_DENIED = (
     "Список администраторов бота не был настроен.\n"
     "Для доступа к настройкам отправьте команду /register с токеном этого бота."
 )
 
 HELP = (
-    "**Доступные команды:**\n"
+    "<b>Доступные команды:</b>\n"
     "/help - список команд\n"
     "/settings - настройка автопостинга\n"
     "/update_blacklist `[источник]` - добавить значения в черный список источника "
     "(в глобальный, если не указан источник)\n"
     "/update_stoplist `[источник]` - добавить значения в список стоп-слов источника "
     "(в глобальный, если не указан источник)\n"
-    "/delete_blacklist `[источник]` - удалить черный список источника "
-    "(глобальный, если не указан источник)\n"
-    "/delete_stoplist `[источник]` - удалить список стоп-слов источника "
-    "(глобальный, если не указан источник)\n"
     "/get_full_logs - получить полные логи\n"
     "/get_last_logs `[n]` - получить последние n строк логов (по умолчанию 15)\n"
     "/remove - удалить источник постов\n"
     "/add - добавить источник постов\n"
     "/get_config - получить файл конфигурации бота\n"
     "/restart - перезапустить бота\n"
     "/exit - выключить бота\n"
@@ -120,16 +116,12 @@
 )
 
 STOPLIST_UPDATE = (
     "Для добавления новых стоп-слов отправьте по одному значению в "
     "строке/сообщении.\nДля завершения отправьте команду /cancel"
 )
 
-STOPLIST_DELETED = "Список стоп-слов был удален."
-
 BLACKLIST_UPDATE = (
     "Для добавления новых значений черного списка отправьте по одному значению "
     "в строке/сообщении. Также поддерживаются регулярные выражения.\nДля "
     "завершения отправьте команду /cancel"
-)
-
-BLACKLIST_DELETED = "Черный список был удален."
+)
```

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tg/tools.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tg/tools.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/tools.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/tools.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/group.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,23 +97,16 @@
         if post["id"] > self.last_id or (
             is_pinned and post["id"] != self.pinned_id
         ):
             logger.info("[VK] Обнаружен новый пост с ID {}", post["id"])
             if post.get("marked_as_ads", 0):
                 logger.info("[VK] Пост рекламный. Он будет пропущен.")
                 return
-            if post.get("post_type", "post") == "suggest":
-                logger.info("[VK] Пост из предложки. Он будет пропущен")
-                return
             for word in self.stop_list:
-                if re.findall(
-                        word, post["text"], flags=re.MULTILINE | re.IGNORECASE
-                ):
-                    logger.info("[VK] В посте содержится выражение {} "
-                                "из стоп списка. Пост будет пропущен", word)
+                if word.lower() in post["text"].lower():
                     break
             else:
                 for word in self.blacklist:
                     post["text"] = re.sub(
                         word, "", post["text"], flags=re.MULTILINE
                     )
                 parsed_post = Post(
```

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/handlers.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/handlers.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/parser.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/parser.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/sender.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/sender.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster/utils/vk/tools.py` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster/utils/vk/tools.py`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/PKG-INFO` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TG-AutoPoster
-Version: 3.5.0
+Version: 3.5.0b1
 Summary: Telegram Bot for reposting from VK
 Home-page: https://github.com/qwertyadrian/TG_AutoPoster
 Download-URL: https://github.com/qwertyadrian/TG_AutoPoster/releases/latest
 Author: qwertyadrian
 Author-email: me@qwertyadrian.ru
 License: MIT License
 Platform: OS Independent
```

### Comparing `TG_AutoPoster-3.5.0/TG_AutoPoster.egg-info/SOURCES.txt` & `TG_AutoPoster-3.5.0b1/TG_AutoPoster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TG_AutoPoster-3.5.0/setup.py` & `TG_AutoPoster-3.5.0b1/setup.py`

 * *Files identical despite different names*

