# Comparing `tmp/discord-py-interactions-4.4.1.tar.gz` & `tmp/discord-py-interactions-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-4.4.1.tar", last modified: Mon Apr 10 15:16:12 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.0.0.tar", last modified: Mon Apr 10 11:44:03 2023, max compression
```

## Comparing `discord-py-interactions-4.4.1.tar` & `discord-py-interactions-5.0.0.tar`

### file list

```diff
@@ -1,96 +1,191 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.439875 discord-py-interactions-4.4.1/
--rw-rw-rw-   0        0        0    35823 2023-03-15 04:13:26.000000 discord-py-interactions-4.4.1/LICENSE
--rw-rw-rw-   0        0        0      194 2023-03-15 04:13:26.000000 discord-py-interactions-4.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6525 2023-04-10 15:16:12.439875 discord-py-interactions-4.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5448 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.353025 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/
--rw-rw-rw-   0        0        0     6525 2023-04-10 15:16:12.000000 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2591 2023-04-10 15:16:12.000000 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 15:16:12.000000 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-04-10 15:16:12.000000 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 15:16:12.000000 discord-py-interactions-4.4.1/discord_py_interactions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.357025 discord-py-interactions-4.4.1/interactions/
--rw-rw-rw-   0        0        0      739 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.361031 discord-py-interactions-4.4.1/interactions/api/
--rw-rw-rw-   0        0        0      320 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/__init__.py
--rw-rw-rw-   0        0        0     5449 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/cache.py
--rw-rw-rw-   0        0        0     3441 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/dispatch.py
--rw-rw-rw-   0        0        0    17935 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/error.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.366031 discord-py-interactions-4.4.1/interactions/api/gateway/
--rw-rw-rw-   0        0        0      247 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/gateway/__init__.py
--rw-rw-rw-   0        0        0    46943 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/gateway/client.py
--rw-rw-rw-   0        0        0      597 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/gateway/heartbeat.py
--rw-rw-rw-   0        0        0     2848 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/gateway/ratelimit.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.390200 discord-py-interactions-4.4.1/interactions/api/http/
--rw-rw-rw-   0        0        0      768 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/__init__.py
--rw-rw-rw-   0        0        0    15464 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/channel.py
--rw-rw-rw-   0        0        0     4782 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/client.py
--rw-rw-rw-   0        0        0     3344 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/emoji.py
--rw-rw-rw-   0        0        0    30813 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/guild.py
--rw-rw-rw-   0        0        0    13468 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/interaction.py
--rw-rw-rw-   0        0        0     1863 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/invite.py
--rw-rw-rw-   0        0        0     1381 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/limiter.py
--rw-rw-rw-   0        0        0     5851 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/member.py
--rw-rw-rw-   0        0        0     7861 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/message.py
--rw-rw-rw-   0        0        0     4870 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/reaction.py
--rw-rw-rw-   0        0        0    10777 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/api/http/request.py
--rw-rw-rw-   0        0        0     2068 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/route.py
--rw-rw-rw-   0        0        0     5551 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/api/http/scheduledEvent.py
--rw-rw-rw-   0        0        0     4162 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/sticker.py
--rw-rw-rw-   0        0        0     9644 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/thread.py
--rw-rw-rw-   0        0        0     2493 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/user.py
--rw-rw-rw-   0        0        0     8313 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/http/webhook.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.408876 discord-py-interactions-4.4.1/interactions/api/models/
--rw-rw-rw-   0        0        0      733 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/__init__.py
--rw-rw-rw-   0        0        0    14014 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/audit_log.py
--rw-rw-rw-   0        0        0    80142 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/api/models/channel.py
--rw-rw-rw-   0        0        0     6246 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/emoji.py
--rw-rw-rw-   0        0        0     7492 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/flags.py
--rw-rw-rw-   0        0        0   128536 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/guild.py
--rw-rw-rw-   0        0        0    30302 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/gw.py
--rw-rw-rw-   0        0        0    25089 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/api/models/member.py
--rw-rw-rw-   0        0        0    49572 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/api/models/message.py
--rw-rw-rw-   0        0        0    13844 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/misc.py
--rw-rw-rw-   0        0        0     7249 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/presence.py
--rw-rw-rw-   0        0        0     8069 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/role.py
--rw-rw-rw-   0        0        0     7069 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/team.py
--rw-rw-rw-   0        0        0     9111 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/user.py
--rw-rw-rw-   0        0        0    11209 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/api/models/webhook.py
--rw-rw-rw-   0        0        0      773 2023-04-10 15:15:13.000000 discord-py-interactions-4.4.1/interactions/base.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.414875 discord-py-interactions-4.4.1/interactions/client/
--rw-rw-rw-   0        0        0      315 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/__init__.py
--rw-rw-rw-   0        0        0    91974 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/client/bot.py
--rw-rw-rw-   0        0        0    32207 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/interactions/client/context.py
--rw-rw-rw-   0        0        0     4901 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/decor.py
--rw-rw-rw-   0        0        0     5207 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/enums.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.418874 discord-py-interactions-4.4.1/interactions/client/models/
--rw-rw-rw-   0        0        0      285 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/models/__init__.py
--rw-rw-rw-   0        0        0    39893 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/models/command.py
--rw-rw-rw-   0        0        0    13187 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/models/component.py
--rw-rw-rw-   0        0        0     5623 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/client/models/misc.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.425878 discord-py-interactions-4.4.1/interactions/ext/
--rw-rw-rw-   0        0        0      338 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/ext/__init__.py
--rw-rw-rw-   0        0        0     5334 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/ext/base.py
--rw-rw-rw-   0        0        0     2552 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/ext/converter.py
--rw-rw-rw-   0        0        0     2009 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/ext/error.py
--rw-rw-rw-   0        0        0     7348 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/ext/version.py
--rw-rw-rw-   0        0        0        0 2023-03-15 04:13:26.000000 discord-py-interactions-4.4.1/interactions/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.434877 discord-py-interactions-4.4.1/interactions/utils/
--rw-rw-rw-   0        0        0      256 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:16:12.438875 discord-py-interactions-4.4.1/interactions/utils/abc/
--rw-rw-rw-   0        0        0      107 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/abc/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/abc/base_context_managers.py
--rw-rw-rw-   0        0        0     3202 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/abc/base_iterators.py
--rw-rw-rw-   0        0        0     8588 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/attrs_utils.py
--rw-rw-rw-   0        0        0     2855 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/attrs_utils.pyi
--rw-rw-rw-   0        0        0     1928 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/dict_caches.py
--rw-rw-rw-   0        0        0    12086 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/get.py
--rw-rw-rw-   0        0        0     3089 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/get.pyi
--rw-rw-rw-   0        0        0      777 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/missing.py
--rw-rw-rw-   0        0        0    11229 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/interactions/utils/utils.py
--rw-rw-rw-   0        0        0      157 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       71 2023-03-15 04:13:26.000000 discord-py-interactions-4.4.1/requirements-docs.txt
--rw-rw-rw-   0        0        0       34 2023-03-15 04:13:26.000000 discord-py-interactions-4.4.1/requirements-lint.txt
--rw-rw-rw-   0        0        0       35 2023-04-10 14:53:20.000000 discord-py-interactions-4.4.1/requirements.txt
--rw-rw-rw-   0        0        0       76 2023-04-10 15:16:12.444878 discord-py-interactions-4.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1892 2023-04-10 15:10:42.000000 discord-py-interactions-4.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.259178 discord-py-interactions-5.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4478 2023-04-10 11:44:03.259178 discord-py-interactions-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3150 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.139566 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/
+-rw-rw-rw-   0        0        0     4478 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6418 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1169 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 11:44:03.000000 discord-py-interactions-5.0.0/discord_py_interactions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.141568 discord-py-interactions-5.0.0/interactions/
+-rw-rw-rw-   0        0        0    15600 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.141568 discord-py-interactions-5.0.0/interactions/api/
+-rw-rw-rw-   0        0        0       47 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.144570 discord-py-interactions-5.0.0/interactions/api/events/
+-rw-rw-rw-   0        0        0     3921 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/__init__.py
+-rw-rw-rw-   0        0        0     2844 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/base.py
+-rw-rw-rw-   0        0        0    24582 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/discord.py
+-rw-rw-rw-   0        0        0     8542 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/internal.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.156581 discord-py-interactions-5.0.0/interactions/api/events/processors/
+-rw-rw-rw-   0        0        0      811 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/_template.py
+-rw-rw-rw-   0        0        0      459 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/_template.pyi
+-rw-rw-rw-   0        0        0     1590 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/auto_mod.py
+-rw-rw-rw-   0        0        0     2135 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/channel_events.py
+-rw-rw-rw-   0        0        0     4943 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/guild_events.py
+-rw-rw-rw-   0        0        0     1337 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/integrations.py
+-rw-rw-rw-   0        0        0     1532 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/member_events.py
+-rw-rw-rw-   0        0        0     2878 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/message_events.py
+-rw-rw-rw-   0        0        0     3303 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/reaction_events.py
+-rw-rw-rw-   0        0        0     1776 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/role_events.py
+-rw-rw-rw-   0        0        0      998 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/stage_events.py
+-rw-rw-rw-   0        0        0     2335 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/thread_events.py
+-rw-rw-rw-   0        0        0     2155 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/user_events.py
+-rw-rw-rw-   0        0        0     2002 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/events/processors/voice_events.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.160585 discord-py-interactions-5.0.0/interactions/api/gateway/
+-rw-rw-rw-   0        0        0       78 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/__init__.py
+-rw-rw-rw-   0        0        0    13930 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/gateway.py
+-rw-rw-rw-   0        0        0     8445 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/state.py
+-rw-rw-rw-   0        0        0    11904 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/gateway/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.162587 discord-py-interactions-5.0.0/interactions/api/http/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/__init__.py
+-rw-rw-rw-   0        0        0    19920 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_client.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.172597 discord-py-interactions-5.0.0/interactions/api/http/http_requests/
+-rw-rw-rw-   0        0        0      835 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/bot.py
+-rw-rw-rw-   0        0        0    22688 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/channels.py
+-rw-rw-rw-   0        0        0     3188 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/emojis.py
+-rw-rw-rw-   0        0        0    35035 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/guild.py
+-rw-rw-rw-   0        0        0    10705 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/interactions.py
+-rw-rw-rw-   0        0        0     6739 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/members.py
+-rw-rw-rw-   0        0        0     5200 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/messages.py
+-rw-rw-rw-   0        0        0     4930 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/reactions.py
+-rw-rw-rw-   0        0        0     5061 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-rw-rw-   0        0        0     4202 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/stickers.py
+-rw-rw-rw-   0        0        0     8434 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/threads.py
+-rw-rw-rw-   0        0        0     4307 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/users.py
+-rw-rw-rw-   0        0        0     6995 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/http_requests/webhooks.py
+-rw-rw-rw-   0        0        0     2176 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/http/route.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.178602 discord-py-interactions-5.0.0/interactions/api/voice/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/__init__.py
+-rw-rw-rw-   0        0        0    12295 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/audio.py
+-rw-rw-rw-   0        0        0     9276 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/audio_writer.py
+-rw-rw-rw-   0        0        0     3754 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/encryption.py
+-rw-rw-rw-   0        0        0    11836 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/opus.py
+-rw-rw-rw-   0        0        0     5596 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/player.py
+-rw-rw-rw-   0        0        0     8005 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/recorder.py
+-rw-rw-rw-   0        0        0    15611 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/api/voice/voice_gateway.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.183108 discord-py-interactions-5.0.0/interactions/client/
+-rw-rw-rw-   0        0        0     1771 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/__init__.py
+-rw-rw-rw-   0        0        0     9799 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/auto_shard_client.py
+-rw-rw-rw-   0        0        0    87510 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/client.py
+-rw-rw-rw-   0        0        0     6562 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/const.py
+-rw-rw-rw-   0        0        0    13632 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.188113 discord-py-interactions-5.0.0/interactions/client/mixins/
+-rw-rw-rw-   0        0        0      118 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/__init__.py
+-rw-rw-rw-   0        0        0      891 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/modal.py
+-rw-rw-rw-   0        0        0     4313 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/send.py
+-rw-rw-rw-   0        0        0     3746 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/mixins/serialization.py
+-rw-rw-rw-   0        0        0    31016 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/smart_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.196120 discord-py-interactions-5.0.0/interactions/client/utils/
+-rw-rw-rw-   0        0        0     2159 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_converters.py
+-rw-rw-rw-   0        0        0     2285 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.py
+-rw-rw-rw-   0        0        0     1210 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/attr_utils.pyi
+-rw-rw-rw-   0        0        0     4806 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/cache.py
+-rw-rw-rw-   0        0        0     3632 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-rw-rw-   0        0        0     3189 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/formatting.py
+-rw-rw-rw-   0        0        0     3642 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/input_utils.py
+-rw-rw-rw-   0        0        0     7524 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/misc_utils.py
+-rw-rw-rw-   0        0        0     4688 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/serializer.py
+-rw-rw-rw-   0        0        0     1079 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/client/utils/text_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.199123 discord-py-interactions-5.0.0/interactions/ext/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/__init__.py
+-rw-rw-rw-   0        0        0     1883 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/console.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.203127 discord-py-interactions-5.0.0/interactions/ext/debug_extension/
+-rw-rw-rw-   0        0        0     3300 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/__init__.py
+-rw-rw-rw-   0        0        0     5112 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-rw-rw-   0        0        0     4646 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exec.py
+-rw-rw-rw-   0        0        0     1418 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/debug_exts.py
+-rw-rw-rw-   0        0        0     6234 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/debug_extension/utils.py
+-rw-rw-rw-   0        0        0     8196 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/jurigged.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.204128 discord-py-interactions-5.0.0/interactions/ext/mypy/
+-rw-rw-rw-   0        0        0     1085 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/mypy/__init__.py
+-rw-rw-rw-   0        0        0    16283 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/paginators.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.208131 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/
+-rw-rw-rw-   0        0        0      554 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/__init__.py
+-rw-rw-rw-   0        0        0    28658 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/command.py
+-rw-rw-rw-   0        0        0     3516 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/context.py
+-rw-rw-rw-   0        0        0     7778 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/help.py
+-rw-rw-rw-   0        0        0    14481 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/manager.py
+-rw-rw-rw-   0        0        0     1205 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/prefixed_commands/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/ext/sentry.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.209132 discord-py-interactions-5.0.0/interactions/models/
+-rw-rw-rw-   0        0        0    12743 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.235156 discord-py-interactions-5.0.0/interactions/models/discord/
+-rw-rw-rw-   0        0        0     8257 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/__init__.py
+-rw-rw-rw-   0        0        0     5628 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/activity.py
+-rw-rw-rw-   0        0        0     3105 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/app_perms.py
+-rw-rw-rw-   0        0        0     4829 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/application.py
+-rw-rw-rw-   0        0        0     3939 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/asset.py
+-rw-rw-rw-   0        0        0    12872 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/auto_mod.py
+-rw-rw-rw-   0        0        0     1779 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/base.py
+-rw-rw-rw-   0        0        0   104561 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/channel.py
+-rw-rw-rw-   0        0        0     8310 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/color.py
+-rw-rw-rw-   0        0        0    25482 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/components.py
+-rw-rw-rw-   0        0        0    16775 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/embed.py
+-rw-rw-rw-   0        0        0     9326 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/emoji.py
+-rw-rw-rw-   0        0        0    29369 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/enums.py
+-rw-rw-rw-   0        0        0     2323 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/file.py
+-rw-rw-rw-   0        0        0    96518 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/guild.py
+-rw-rw-rw-   0        0        0     6212 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/invite.py
+-rw-rw-rw-   0        0        0    38197 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/message.py
+-rw-rw-rw-   0        0        0     5139 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/modal.py
+-rw-rw-rw-   0        0        0     3609 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/reaction.py
+-rw-rw-rw-   0        0        0     8309 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/role.py
+-rw-rw-rw-   0        0        0     9570 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0     5353 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/snowflake.py
+-rw-rw-rw-   0        0        0     1479 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/stage_instance.py
+-rw-rw-rw-   0        0        0     5378 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/sticker.py
+-rw-rw-rw-   0        0        0     2871 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/team.py
+-rw-rw-rw-   0        0        0     5828 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/thread.py
+-rw-rw-rw-   0        0        0     4429 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/timestamp.py
+-rw-rw-rw-   0        0        0    25473 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/user.py
+-rw-rw-rw-   0        0        0     6891 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/user.pyi
+-rw-rw-rw-   0        0        0     4971 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/voice_state.py
+-rw-rw-rw-   0        0        0    12721 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/discord/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.246166 discord-py-interactions-5.0.0/interactions/models/internal/
+-rw-rw-rw-   0        0        0     4981 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/__init__.py
+-rw-rw-rw-   0        0        0    11584 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/active_voice_state.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.247167 discord-py-interactions-5.0.0/interactions/models/internal/annotations/
+-rw-rw-rw-   0        0        0      523 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/annotations/__init__.py
+-rw-rw-rw-   0        0        0     7673 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/annotations/slash.py
+-rw-rw-rw-   0        0        0    56500 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/application_commands.py
+-rw-rw-rw-   0        0        0     1470 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/auto_defer.py
+-rw-rw-rw-   0        0        0     1238 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/callback.py
+-rw-rw-rw-   0        0        0     2485 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/checks.py
+-rw-rw-rw-   0        0        0    12548 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/command.py
+-rw-rw-rw-   0        0        0    35380 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/context.py
+-rw-rw-rw-   0        0        0    19957 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/converters.py
+-rw-rw-rw-   0        0        0     8652 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/cooldowns.py
+-rw-rw-rw-   0        0        0    10438 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/extension.py
+-rw-rw-rw-   0        0        0     4671 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/listener.py
+-rw-rw-rw-   0        0        0     6168 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/localisation.py
+-rw-rw-rw-   0        0        0     1405 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/protocols.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.250170 discord-py-interactions-5.0.0/interactions/models/internal/tasks/
+-rw-rw-rw-   0        0        0      212 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5295 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/task.py
+-rw-rw-rw-   0        0        0     4194 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/tasks/triggers.py
+-rw-rw-rw-   0        0        0     1228 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/internal/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.252171 discord-py-interactions-5.0.0/interactions/models/misc/
+-rw-rw-rw-   0        0        0      115 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/__init__.py
+-rw-rw-rw-   0        0        0      996 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/context_manager.py
+-rw-rw-rw-   0        0        0     3216 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/interactions/models/misc/iterator.py
+-rw-rw-rw-   0        0        0        0 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/interactions/py.typed
+-rw-rw-rw-   0        0        0     5833 2023-04-10 11:43:08.000000 discord-py-interactions-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       71 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/requirements-docs.txt
+-rw-rw-rw-   0        0        0       34 2023-03-29 13:34:31.000000 discord-py-interactions-5.0.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0       54 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/requirements.txt
+-rw-rw-rw-   0        0        0      456 2023-04-10 11:44:03.260178 discord-py-interactions-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2483 2023-04-10 11:42:49.000000 discord-py-interactions-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:44:03.258177 discord-py-interactions-5.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4500 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/consts.py
+-rw-rw-rw-   0        0        0    17477 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_bot.py
+-rw-rw-rw-   0        0        0     1956 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_cache.py
+-rw-rw-rw-   0        0        0     2056 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_contexts.py
+-rw-rw-rw-   0        0        0     2278 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_cooldowns.py
+-rw-rw-rw-   0        0        0     3907 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/test_emoji.py
+-rw-rw-rw-   0        0        0     1081 2023-04-10 11:35:41.000000 discord-py-interactions-5.0.0/tests/utils.py
```

### Comparing `discord-py-interactions-4.4.1/LICENSE` & `discord-py-interactions-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-4.4.1/interactions/api/http/emoji.py` & `discord-py-interactions-5.0.0/interactions/api/http/http_requests/emojis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,104 @@
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, cast
 
-from ..models.emoji import Emoji
-from ..models.guild import Guild
-from ..models.misc import Snowflake
-from .request import _Request
-from .route import Route
+import discord_typings
 
-if TYPE_CHECKING:
-    from ...api.cache import Cache
+from interactions.models.internal.protocols import CanRequest
+from ..route import Route
 
-__all__ = ("EmojiRequest",)
+__all__ = ("EmojiRequests",)
 
 
-class EmojiRequest:
-    _req: _Request
-    cache: "Cache"
+if TYPE_CHECKING:
+    from interactions.models.discord.snowflake import Snowflake_Type
 
-    def __init__(self) -> None:
-        pass
 
-    async def get_all_emoji(self, guild_id: int) -> List[dict]:
+class EmojiRequests(CanRequest):
+    async def get_all_guild_emoji(self, guild_id: "Snowflake_Type") -> list[discord_typings.EmojiData]:
         """
-        Gets all emojis from a guild.
+        Get all the emoji from a guild.
+
+        Args:
+            guild_id: The ID of the guild to query.
+
+        Returns:
+            List of emoji objects
 
-        :param guild_id: Guild ID snowflake.
-        :return: A list of emojis.
         """
-        res = await self._req.request(Route("GET", f"/guilds/{guild_id}/emojis"))
-        self.cache[Guild].get(Snowflake(guild_id)).emojis = [
-            Emoji(**_res, _client=self) for _res in res
-        ]
-        return res
+        result = await self.request(Route("GET", f"/guilds/{int(guild_id)}/emojis"))
+        return cast(list[discord_typings.EmojiData], result)
 
-    async def get_guild_emoji(self, guild_id: int, emoji_id: int) -> dict:
+    async def get_guild_emoji(
+        self, guild_id: "Snowflake_Type", emoji_id: "Snowflake_Type"
+    ) -> discord_typings.EmojiData:
         """
-        Gets an emote from a guild.
+        Get a specific guild emoji object.
+
+        Args:
+            guild_id: The ID of the guild to query
+            emoji_id: The ID of the emoji to get
+
+        Returns:
+            PartialEmoji object
 
-        :param guild_id: Guild ID snowflake.
-        :param emoji_id: Emoji ID snowflake.
-        :return: Emoji object
         """
-        res = await self._req.request(Route("GET", f"/guilds/{guild_id}/emojis/{emoji_id}"))
-        emoji = Emoji(**res, _client=self)
-        guild = self.cache[Guild].get(Snowflake(guild_id))
-        if guild.emojis is None:
-            guild.emojis = [emoji]
-        else:
-            for index, _emoji in enumerate(guild.emojis):
-                if _emoji.id == emoji.id:
-                    guild.emojis[index] = emoji
-                    break
-            else:
-                guild.emojis.append(emoji)
-        self.cache[Guild].add(guild)  # yes it should just be overwritten
-        return res
+        result = await self.request(Route("GET", f"/guilds/{int(guild_id)}/emojis/{int(emoji_id)}"))
+        return cast(discord_typings.EmojiData, result)
 
     async def create_guild_emoji(
-        self, guild_id: int, payload: dict, reason: Optional[str] = None
-    ) -> dict:
+        self, payload: dict, guild_id: "Snowflake_Type", reason: str | None = None
+    ) -> discord_typings.EmojiData:
         """
-        Creates an emoji.
+        Create a guild emoji.
 
-        :param guild_id: Guild ID snowflake.
-        :param payload: Emoji parameters.
-        :param reason: Optionally, give a reason.
-        :return: An emoji object with the included parameters.
-        """
-        return await self._req.request(
-            Route("POST", f"/guilds/{guild_id}/emojis"), json=payload, reason=reason
-        )
+        Args:
+            payload: The emoji's data
+            guild_id: The ID of the guild
+            reason: The reason for this creation
 
-    async def modify_guild_emoji(
-        self, guild_id: int, emoji_id: int, payload: dict, reason: Optional[str] = None
-    ) -> dict:
-        """
-        Modifies an emoji.
+        Returns:
+            The created emoji object
 
-        :param guild_id: Guild ID snowflake.
-        :param emoji_id: Emoji ID snowflake
-        :param payload: Emoji parameters with updated attributes
-        :param reason: Optionally, give a reason.
-        :return: An emoji object with updated attributes.
         """
-        return await self._req.request(
-            Route("PATCH", f"/guilds/{guild_id}/emojis/{emoji_id}"), json=payload, reason=reason
+        result = await self.request(Route("POST", f"/guilds/{int(guild_id)}/emojis"), payload=payload, reason=reason)
+        return cast(discord_typings.EmojiData, result)
+
+    async def modify_guild_emoji(
+        self,
+        payload: dict,
+        guild_id: "Snowflake_Type",
+        emoji_id: "Snowflake_Type",
+        reason: str | None = None,
+    ) -> discord_typings.EmojiData:
+        """
+        Modify an existing guild emoji.
+
+        Args:
+            payload: The emoji's data
+            guild_id: The ID of the guild
+            emoji_id: The ID of the emoji to update
+            reason: The reason for this creation
+
+        Returns:
+            The updated emoji object
+
+        """
+        result = await self.request(
+            Route("PATCH", f"/guilds/{int(guild_id)}/emojis/{int(emoji_id)}"),
+            payload=payload,
+            reason=reason,
         )
+        return cast(discord_typings.EmojiData, result)
 
     async def delete_guild_emoji(
-        self, guild_id: int, emoji_id: int, reason: Optional[str] = None
+        self, guild_id: "Snowflake_Type", emoji_id: "Snowflake_Type", reason: str | None = None
     ) -> None:
         """
-        Deletes an emoji.
+        Delete a guild emoji.
+
+        Args:
+            guild_id: The ID of the guild
+            emoji_id: The ID of the emoji to update
+            reason: The reason for this deletion
 
-        :param guild_id: Guild ID snowflake.
-        :param emoji_id: Emoji ID snowflake
-        :param reason: Optionally, give a reason.
         """
-        await self._req.request(
-            Route("DELETE", f"/guilds/{guild_id}/emojis/{emoji_id}"), reason=reason
-        )
+        await self.request(Route("DELETE", f"/guilds/{int(guild_id)}/emojis/{int(emoji_id)}"), reason=reason)
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/http/webhook.py` & `discord-py-interactions-5.0.0/interactions/api/http/http_requests/webhooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,246 +1,208 @@
-from typing import List, Optional
+from typing import TYPE_CHECKING, Any, List, Optional
 
-from aiohttp import MultipartWriter
+import discord_typings
 
-from ...api.cache import Cache
-from ...utils.missing import MISSING
-from ..models.misc import File
-from .request import _Request
-from .route import Route
+from interactions.client.utils.serializer import dict_filter_none
+from ..route import Route
 
-__all__ = ("WebhookRequest",)
+__all__ = ("WebhookRequests",)
 
 
-class WebhookRequest:
-    _req: _Request
-    cache: Cache
+if TYPE_CHECKING:
+    from interactions.models.discord.snowflake import Snowflake_Type
+    from interactions import UPLOADABLE_TYPE
 
-    def __init__(self) -> None:
-        pass
 
-    async def create_webhook(self, channel_id: int, name: str, avatar: str = None) -> dict:
+class WebhookRequests:
+    request: Any
+
+    async def create_webhook(
+        self, channel_id: "Snowflake_Type", name: str, avatar: Any = None
+    ) -> discord_typings.WebhookData:
         """
         Create a new webhook.
 
-        :param channel_id: Channel ID snowflake.
-        :param name: Name of the webhook (1-80 characters)
-        :param avatar: The image for the default webhook avatar, if given.
+        Args:
+            channel_id: The id of the channel to add this webhook to
+            name: name of the webhook (1-80 characters)
+            avatar: The image for the default webhook avatar
 
-        :return: Webhook object
         """
-        return await self._req.request(
-            Route("POST", f"/channels/{channel_id}/webhooks"), json={"name": name, "avatar": avatar}
+        return await self.request(
+            Route("POST", f"/channels/{channel_id}/webhooks"),
+            payload={"name": name, "avatar": avatar},
         )
 
-    async def get_channel_webhooks(self, channel_id: int) -> List[dict]:
+    async def get_channel_webhooks(self, channel_id: "Snowflake_Type") -> List[discord_typings.WebhookData]:
         """
         Return a list of channel webhook objects.
 
-        :param channel_id: Channel ID snowflake.
-        :return: List of webhook objects
+        Args:
+            channel_id: The id of the channel to query
+
+        Returns:
+            List of webhook objects
+
         """
-        return await self._req.request(Route("GET", f"/channels/{channel_id}/webhooks"))
+        return await self.request(Route("GET", f"/channels/{channel_id}/webhooks"))
 
-    async def get_guild_webhooks(self, guild_id: int) -> List[dict]:
+    async def get_guild_webhooks(self, guild_id: "Snowflake_Type") -> List[discord_typings.WebhookData]:
         """
         Return a list of guild webhook objects.
 
-        :param guild_id: Guild ID snowflake
-        :return: List of webhook objects
+        Args:
+            guild_id: The id of the guild to query
+
+        Returns:
+            List of webhook objects
+
         """
-        return await self._req.request(Route("GET", f"/guilds/{guild_id}/webhooks"))
+        return await self.request(Route("GET", f"/guilds/{guild_id}/webhooks"))
 
-    async def get_webhook(self, webhook_id: int, webhook_token: str = None) -> dict:
+    async def get_webhook(self, webhook_id: "Snowflake_Type", webhook_token: str = None) -> discord_typings.WebhookData:
         """
         Return the new webhook object for the given id.
 
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: Webhook Token, if given.
+        Args:
+            webhook_id: The ID of the webhook to get
+            webhook_token: The token for the webhook
+
+        Returns:
+            Webhook object
 
-        :return:Webhook object
         """
         endpoint = f"/webhooks/{webhook_id}{f'/{webhook_token}' if webhook_token else ''}"
 
-        return await self._req.request(Route("GET", endpoint))
+        return await self.request(Route("GET", endpoint))
 
     async def modify_webhook(
         self,
-        webhook_id: int,
-        payload: dict,
+        webhook_id: "Snowflake_Type",
+        name: str,
+        avatar: Any,
+        channel_id: "Snowflake_Type",
         webhook_token: str = None,
-    ) -> dict:
+    ) -> discord_typings.WebhookData:
         """
         Modify a webhook.
 
-        :param webhook_id: Webhook ID snowflake
-        :param payload: The payload for the webhook
-        :param webhook_token: The token for the webhook, if given.
+        Args:
+            name: the default name of the webhook
+            avatar: image for the default webhook avatar
+            channel_id: the new channel id this webhook should be moved to
+            webhook_id: The ID of the webhook to modify
+            webhook_token: The token for the webhook
 
-        :return: Modified webhook object.
         """
         endpoint = f"/webhooks/{webhook_id}{f'/{webhook_token}' if webhook_token else ''}"
 
-        return await self._req.request(
+        return await self.request(
             Route("PATCH", endpoint),
-            json=payload,
+            payload={"name": name, "avatar": avatar, "channel_id": channel_id},
         )
 
-    async def delete_webhook(self, webhook_id: int, webhook_token: str = None):
+    async def delete_webhook(self, webhook_id: "Snowflake_Type", webhook_token: str = None) -> None:
         """
         Delete a webhook.
 
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: The token for the webhook, if given.
-        """
+        Args:
+            webhook_id: The ID of the webhook to delete
+            webhook_token: The token for the webhook
+
+        Returns:
+            Webhook object
 
+        """
         endpoint = f"/webhooks/{webhook_id}{f'/{webhook_token}' if webhook_token else ''}"
 
-        return await self._req.request(Route("DELETE", endpoint))
+        return await self.request(Route("DELETE", endpoint))
 
     async def execute_webhook(
         self,
-        webhook_id: int,
+        webhook_id: "Snowflake_Type",
         webhook_token: str,
         payload: dict,
-        files: Optional[List[File]] = MISSING,
-        wait: Optional[bool] = False,
-        thread_id: Optional[int] = None,
-    ) -> Optional[dict]:
-        """
-        Sends a message as a webhook.
-
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: The token for the webhook.
-        :param payload: Payload consisting of the message.
-        :param files: The files to upload to the message.
-        :param wait: A bool that signifies waiting for server confirmation of a send before responding.
-        :param thread_id: Optional, sends a message to the specified thread.
-        :return: The message sent, if wait=True, else None.
-        """
-
-        data = None
-        if files is not MISSING and len(files) > 0:
-            data = MultipartWriter("form-data")
-            part = data.append_json(payload)
-            part.set_content_disposition("form-data", name="payload_json")
-            payload = None
-
-            for id, file in enumerate(files):
-                part = data.append(
-                    file._fp,
-                )
-                part.set_content_disposition(
-                    "form-data", name=f"files[{str(id)}]", filename=file._filename
-                )
-
-        params = {"wait": "true" if wait else "false"}
-        if thread_id:
-            params["thread_id"] = thread_id
+        wait: bool = False,
+        thread_id: "Snowflake_Type" = None,
+        files: list["UPLOADABLE_TYPE"] | None = None,
+    ) -> Optional[discord_typings.MessageData]:
+        """
+        Execute a webhook. Basically send a message as the webhook.
+
+        Args:
+            webhook_id: The ID of the webhook to delete
+            webhook_token: The token for the webhook
+            payload: The JSON payload for the message
+            wait: Waits for server confirmation of message send before response
+            thread_id: Send a message to the specified thread
+            files: The files to send with this message
 
-        return await self._req.request(
-            Route("POST", f"/webhooks/{webhook_id}/{webhook_token}"),
-            params=params,
-            json=payload,
-            data=data,
-        )
-
-    async def execute_slack_webhook(
-        self, webhook_id: int, webhook_token: str, payload: dict
-    ) -> None:
-        """
-        Sends a message to a Slack-compatible webhook.
-
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: The token for the webhook.
-        :param payload: Payload consisting of the message.
+        Returns:
+            The sent `message`, if `wait` is True else None
 
-        :return: ?
-
-        .. note::
-            Payload structure is different than Discord's. See `here <https://api.slack.com/messaging/webhooks>_` for more details.
         """
-
-        return await self._req.request(
-            Route("POST", f"/webhooks/{webhook_id}/{webhook_token}/slack"), json=payload
+        return await self.request(
+            Route("POST", f"/webhooks/{webhook_id}/{webhook_token}"),
+            params=dict_filter_none({"wait": "true" if wait else "false", "thread_id": thread_id}),
+            payload=payload,
+            files=files,
         )
 
-    async def execute_github_webhook(
-        self, webhook_id: int, webhook_token: str, payload: dict
-    ) -> None:
+    async def get_webhook_message(
+        self, webhook_id: "Snowflake_Type", webhook_token: str, message_id: "Snowflake_Type"
+    ) -> discord_typings.MessageData:
         """
-        Sends a message to a Github-compatible webhook.
+        Returns a previously-sent webhook message from the same token. Returns a message object on success.
 
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: The token for the webhook.
-        :param payload: Payload consisting of the message.
+        Args:
+            webhook_id: The ID of the webhook to delete
+            webhook_token: The token for the webhook
+            message_id: The ID of a message sent by this webhook
 
-        :return: ?
+        Returns:
+            A message object on success
 
-        .. note::
-            Payload structure is different than Discord's. See `here <https://discord.com/developers/docs/resources/webhook#execute-githubcompatible-webhook>_` for more details.
         """
+        return await self.request(Route("GET", f"/webhooks/{webhook_id}/{webhook_token}/messages/{message_id}"))
 
-        return await self._req.request(
-            Route("POST", f"/webhooks/{webhook_id}/{webhook_token}/github"), json=payload
-        )
-
-    async def get_webhook_message(
-        self, webhook_id: int, webhook_token: str, message_id: int
-    ) -> dict:
-        """
-        Retrieves a message sent from a Webhook.
-
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: Webhook token.
-        :param message_id: Message ID snowflake,
-        :return: A Message object.
+    async def edit_webhook_message(
+        self,
+        webhook_id: "Snowflake_Type",
+        webhook_token: str,
+        message_id: "Snowflake_Type",
+        payload: dict,
+        files: None | list["UPLOADABLE_TYPE"] = None,
+    ) -> discord_typings.MessageData:
         """
+        Edits a previously-sent webhook message from the same token.
 
-        return await self._req.request(
-            Route("GET", f"/webhooks/{webhook_id}/{webhook_token}/messages/{message_id}")
-        )
+        Args:
+            webhook_id: The ID of the webhook to delete
+            webhook_token: The token for the webhook
+            message_id: The ID of a message sent by this webhook
+            payload: The JSON payload for the message
+            files: The files to send in this message
 
-    async def edit_webhook_message(
-        self, webhook_id: int, webhook_token: str, message_id: int, data: dict
-    ) -> dict:
-        """
-        Edits a message sent from a Webhook.
+        Returns:
+            The updated message on success
 
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: Webhook token.
-        :param message_id: Message ID snowflake.
-        :param data: A payload consisting of new message attributes.
-        :return: An updated message object.
         """
-
-        return await self._req.request(
+        return await self.request(
             Route("PATCH", f"/webhooks/{webhook_id}/{webhook_token}/messages/{message_id}"),
-            json=data,
+            payload=payload,
+            files=files,
         )
 
     async def delete_webhook_message(
-        self, webhook_id: int, webhook_token: str, message_id: int
+        self, webhook_id: "Snowflake_Type", webhook_token: str, message_id: "Snowflake_Type"
     ) -> None:
         """
-        Deletes a message object.
-
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: Webhook token.
-        :param message_id: Message ID snowflake.
-        """
+        Delete a message that was created by the same token.
 
-        return await self._req.request(
-            Route("DELETE", f"/webhooks/{webhook_id}/{webhook_token}/messages/{message_id}")
-        )
-
-    async def delete_original_webhook_message(self, webhook_id: int, webhook_token: str) -> None:
-        """
-        Deletes the original message object sent.
+        Args:
+            webhook_id: The ID of the webhook to delete
+            webhook_token: The token for the webhook
+            message_id: The ID of a message sent by this webhook
 
-        :param webhook_id: Webhook ID snowflake.
-        :param webhook_token: Webhook token.
         """
-
-        return await self._req.request(
-            Route("DELETE", f"/webhooks/{webhook_id}/{webhook_token}/messages/@original")
-        )
+        return await self.request(Route("DELETE", f"/webhooks/{webhook_id}/{webhook_token}/messages/{message_id}"))
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/emoji.py` & `discord-py-interactions-5.0.0/interactions/models/discord/invite.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,188 +1,134 @@
-from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union, Dict, Any
 
-from ...utils.attrs_utils import ClientSerializerMixin, convert_list, define, field
-from ...utils.missing import MISSING
-from ..error import LibraryException
-from .misc import Snowflake
-from .role import Role
-from .user import User
-
-if TYPE_CHECKING:
-    from ..http import HTTPClient
-    from .guild import Guild
-
-__all__ = ("Emoji",)
+import attrs
 
+from interactions.client.const import MISSING, Absent
+from interactions.client.utils.attr_converters import optional as optional_c
+from interactions.client.utils.attr_converters import timestamp_converter
+from interactions.models.discord.application import Application
+from interactions.models.discord.enums import InviteTargetType
+from interactions.models.discord.guild import GuildPreview
+from interactions.models.discord.snowflake import to_snowflake
+from interactions.models.discord.stage_instance import StageInstance
+from interactions.models.discord.timestamp import Timestamp
+from .base import ClientObject
 
-@define()
-class Emoji(ClientSerializerMixin):
-    """
-    A class objecting representing an emoji.
-
-    :ivar Optional[Snowflake] id: Emoji id
-    :ivar Optional[str] name: Emoji name.
-    :ivar Optional[List[int]] roles: Roles allowed to use this emoji
-    :ivar Optional[User] user: User that created this emoji
-    :ivar Optional[bool] require_colons: Status denoting of this emoji must be wrapped in colons
-    :ivar Optional[bool] managed: Status denoting if this emoji is managed (by an integration)
-    :ivar Optional[bool] animated: Status denoting if this emoji is animated
-    :ivar Optional[bool] available: Status denoting if this emoji can be used. (Can be false via server boosting)
-    """
-
-    id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    name: Optional[str] = field(default=None)
-    roles: Optional[List[int]] = field(converter=convert_list(int), default=None)
-    user: Optional[User] = field(converter=User, default=None)
-    require_colons: Optional[bool] = field(default=None)
-    managed: Optional[bool] = field(default=None)
-    animated: Optional[bool] = field(default=None)
-    available: Optional[bool] = field(default=None)
+if TYPE_CHECKING:
+    from interactions.client import Client
+    from interactions.models import TYPE_GUILD_CHANNEL
+    from interactions.models.discord.user import User
+    from interactions.models.discord.snowflake import Snowflake_Type
+
+__all__ = ("Invite",)
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class Invite(ClientObject):
+    code: str = attrs.field(repr=True)
+    """the invite code (unique ID)"""
+
+    # metadata
+    uses: int = attrs.field(default=0, repr=True)
+    """the guild this invite is for"""
+    max_uses: int = attrs.field(repr=False, default=0)
+    """max number of times this invite can be used"""
+    max_age: int = attrs.field(repr=False, default=0)
+    """duration (in seconds) after which the invite expires"""
+    created_at: Timestamp = attrs.field(default=MISSING, converter=optional_c(timestamp_converter), repr=True)
+    """when this invite was created"""
+    temporary: bool = attrs.field(default=False, repr=True)
+    """whether this invite only grants temporary membership"""
+
+    # target data
+    target_type: Optional[Union[InviteTargetType, int]] = attrs.field(
+        default=None, converter=optional_c(InviteTargetType), repr=True
+    )
+    """the type of target for this voice channel invite"""
+    approximate_presence_count: Optional[int] = attrs.field(repr=False, default=MISSING)
+    """approximate count of online members, returned from the `GET /invites/<code>` endpoint when `with_counts` is `True`"""
+    approximate_member_count: Optional[int] = attrs.field(repr=False, default=MISSING)
+    """approximate count of total members, returned from the `GET /invites/<code>` endpoint when `with_counts` is `True`"""
+    scheduled_event: Optional["Snowflake_Type"] = attrs.field(
+        default=None, converter=optional_c(to_snowflake), repr=True
+    )
+    """guild scheduled event data, only included if `guild_scheduled_event_id` contains a valid guild scheduled event id"""
+    expires_at: Optional[Timestamp] = attrs.field(default=None, converter=optional_c(timestamp_converter), repr=True)
+    """the expiration date of this invite, returned from the `GET /invites/<code>` endpoint when `with_expiration` is `True`"""
+    stage_instance: Optional[StageInstance] = attrs.field(repr=False, default=None)
+    """stage instance data if there is a public Stage instance in the Stage channel this invite is for (deprecated)"""
+    target_application: Optional[dict] = attrs.field(repr=False, default=None)
+    """the embedded application to open for this voice channel embedded application invite"""
+    guild_preview: Optional[GuildPreview] = attrs.field(repr=False, default=MISSING)
+    """the guild this invite is for"""
+
+    # internal for props
+    _channel_id: "Snowflake_Type" = attrs.field(converter=to_snowflake, repr=True)
+    _inviter_id: Optional["Snowflake_Type"] = attrs.field(default=None, converter=optional_c(to_snowflake), repr=True)
+    _target_user_id: Optional["Snowflake_Type"] = attrs.field(
+        repr=False, default=None, converter=optional_c(to_snowflake)
+    )
 
     @property
-    def format(self) -> str:
-        """
-        .. versionadded:: 4.4.0
-
-        Formats the emoji into a send-able form.
-
-        :rtype: str
-        """
-        return (
-            f"<{'a' if self.animated else ''}:{self.name}:{self.id}>"
-            if self.id is not None
-            else f":{self.name}:"
-            if self.require_colons
-            else self.name
-        )
+    def channel(self) -> "TYPE_GUILD_CHANNEL":
+        """The channel the invite is for."""
+        return self._client.cache.get_channel(self._channel_id)
 
     @property
-    def created_at(self) -> datetime:
-        """
-        .. versionadded:: 4.4.0
-
-        Returns when the emoji was created.
-        """
-        return self.id.timestamp
-
-    @classmethod
-    async def get(
-        cls,
-        guild_id: Union[int, Snowflake, "Guild"],
-        emoji_id: Union[int, Snowflake],
-        client: "HTTPClient",
-    ) -> "Emoji":
-        """
-        .. versionadded:: 4.2.0
-
-        Gets an emoji.
-
-        :param Union[int, Snowflake, Guild] guild_id: The id of the guild of the emoji
-        :param Union[int, Snowflake] emoji_id: The id of the emoji
-        :param HTTPClient client: The HTTPClient of your bot. Equals to ``bot._http``
-        :return: The Emoji as object
-        :rtype: Emoji
-        """
-
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
+    def inviter(self) -> Optional["User"]:
+        """The user that created the invite or None."""
+        return self._client.cache.get_user(self._inviter_id) if self._inviter_id else None
 
-        res = await client.get_guild_emoji(guild_id=_guild_id, emoji_id=int(emoji_id))
-        return cls(**res, _client=client)
+    @property
+    def target_user(self) -> Optional["User"]:
+        """The user whose stream to display for this voice channel stream invite or None."""
+        return self._client.cache.get_user(self._target_user_id) if self._target_user_id else None
 
     @classmethod
-    async def get_all_of_guild(
-        cls,
-        guild_id: Union[int, Snowflake, "Guild"],
-        client: "HTTPClient",
-    ) -> List["Emoji"]:
-        """
-        .. versionadded:: 4.2.0
-
-        Gets all emoji of a guild.
-
-        :param Union[int, Snowflake, Guild] guild_id: The id of the guild to get the emojis of
-        :param HTTPClient client: The HTTPClient of your bot. Equals to ``bot._http``
-        :return: The Emoji as list
-        :rtype: List[Emoji]
-        """
-
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
-
-        res = await client.get_all_emoji(guild_id=_guild_id)
-        return [cls(**emoji, _client=client) for emoji in res]
-
-    async def modify(
-        self,
-        guild_id: Union[int, Snowflake, "Guild"],
-        name: Optional[str] = MISSING,
-        roles: Optional[Union[List[Role], List[int]]] = MISSING,
-        reason: Optional[str] = None,
-    ) -> "Emoji":
-        """
-        .. versionadded:: 4.4.0
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if "stage_instance" in data:
+            data["stage_instance"] = StageInstance.from_dict(data, client)
 
-        Edits the Emoji in a guild.
+        if "target_application" in data:
+            data["target_application"] = Application.from_dict(data, client)
 
-        :param int guild_id: The id of the guild to edit the emoji on
-        :param Optional[str] name: The name of the emoji. If not specified, the filename will be used
-        :param Optional[Union[List[Role], List[int]]] roles: Roles allowed to use this emoji
-        :param Optional[str] reason: The reason of the modification
-        :return: The modified emoji object
-        :rtype: Emoji
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-
-        payload: dict = {}
-
-        if name is not MISSING:
-            payload["name"] = name
+        if "target_event_id" in data:
+            data["scheduled_event"] = data["target_event_id"]
 
-        if roles is not MISSING:
-            payload["roles"] = [int(role.id if isinstance(role, Role) else role) for role in roles]
+        if channel := data.pop("channel", None):
+            # invite metadata does not contain enough info to create a channel object
+            data["channel_id"] = channel["id"]
 
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
+        if guild := data.pop("guild", None):
+            data["guild_preview"] = GuildPreview.from_dict(guild, client)
 
-        res = await self._client.modify_guild_emoji(
-            guild_id=_guild_id, emoji_id=int(self.id), payload=payload, reason=reason
-        )
+        if inviter := data.pop("inviter", None):
+            inviter = client.cache.place_user_data(inviter)
+            data["inviter_id"] = inviter.id
 
-        self.update(res)
+        return data
 
-        return self
-
-    async def delete(
-        self,
-        guild_id: Union[int, Snowflake, "Guild"],
-        reason: Optional[str] = None,
-    ) -> None:
-        """
-        .. versionadded:: 4.2.0
+    def __str__(self) -> str:
+        return self.link
 
-        Deletes the emoji.
+    @property
+    def link(self) -> str:
+        """The invite link."""
+        if self.scheduled_event:
+            return f"https://discord.gg/{self.code}?event={self.scheduled_event}"
+        return f"https://discord.gg/{self.code}"
 
-        :param Union[int, Snowflake, Guild] guild_id: The guild id to delete the emoji from
-        :param Optional[str] reason: The reason for the deletion
+    async def delete(self, reason: Absent[str] = MISSING) -> None:
         """
-        if not self._client:
-            raise LibraryException(code=13)
-
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
+        Delete this invite.
 
-        return await self._client.delete_guild_emoji(
-            guild_id=_guild_id, emoji_id=int(self.id), reason=reason
-        )
+        !!! note
+            You must have the `manage_channels` permission on the channel this invite belongs to.
 
-    @property
-    def url(self) -> str:
-        """
-        .. versionadded:: 4.2.0
+        !!! note
+            With `manage_guild` permission, you can delete any invite across the guild.
 
-        Returns the emoji's URL.
+        Args:
+            reason: The reason for the deletion of invite.
 
-        :return: URL of the emoji
-        :rtype: str
         """
-        url = f"https://cdn.discordapp.com/emojis/{self.id}"
-        url += ".gif" if self.animated else ".png"
-        return url
+        await self._client.http.delete_invite(self.code, reason=reason)
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/member.py` & `discord-py-interactions-5.0.0/interactions/client/smart_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,684 +1,902 @@
-from datetime import datetime
-from typing import TYPE_CHECKING, Any, List, Optional, Union
+from contextlib import suppress
+from logging import Logger
+from typing import TYPE_CHECKING, List, Dict, Any, Optional, Union
+
+import attrs
+import discord_typings
+
+from interactions.client.const import Absent, MISSING, get_logger
+from interactions.client.errors import NotFound, Forbidden
+from interactions.client.utils.cache import TTLCache, NullCache
+from interactions.models import VoiceState
+from interactions.models.discord.channel import BaseChannel, GuildChannel, ThreadChannel
+from interactions.models.discord.emoji import CustomEmoji
+from interactions.models.discord.guild import Guild
+from interactions.models.discord.message import Message
+from interactions.models.discord.role import Role
+from interactions.models.discord.snowflake import to_snowflake, to_optional_snowflake
+from interactions.models.discord.user import Member, User
+from interactions.models.internal.active_voice_state import ActiveVoiceState
 
-from ...utils.attrs_utils import ClientSerializerMixin, convert_int, convert_list, define, field
-from ...utils.missing import MISSING
-from ...utils.utils import search_iterable
-from ..error import LibraryException
-from .channel import Channel
-from .flags import MemberFlags, Permissions
-from .misc import AllowedMentions, File, IDMixin, Snowflake
-from .role import Role
-from .user import User
+__all__ = ("GlobalCache", "create_cache")
 
-if TYPE_CHECKING:
-    from ...client.models.component import ActionRow, Button, SelectMenu
-    from .guild import Guild
-    from .gw import VoiceState
-    from .message import Attachment, Embed, Message
 
-__all__ = ("Member",)
+if TYPE_CHECKING:
+    from interactions.client import Client
+    from interactions.models.discord.channel import DM, TYPE_ALL_CHANNEL
+    from interactions.models.discord.snowflake import Snowflake_Type
 
 
-@define()
-class Member(ClientSerializerMixin, IDMixin):
+def create_cache(
+    ttl: Optional[int] = 60,
+    hard_limit: Optional[int] = 250,
+    soft_limit: Absent[Optional[int]] = MISSING,
+) -> Union[dict, TTLCache, NullCache]:
     """
-    A class object representing the user of a guild, known as a "member."
+    Create a cache object based on the parameters passed.
 
-    .. note::
-        ``pending`` and ``permissions`` only apply for members retroactively
-        requiring to verify rules via. membership screening or lack permissions
-        to speak.
-
-    :ivar User user: The user of the guild.
-    :ivar str nick: The nickname of the member.
-    :ivar Optional[str] avatar: The hash containing the user's guild avatar, if applicable.
-    :ivar List[int] roles: The list of roles of the member.
-    :ivar datetime joined_at: The timestamp the member joined the guild at.
-    :ivar datetime premium_since: The timestamp the member has been a server booster since.
-    :ivar bool deaf: Whether the member is deafened.
-    :ivar bool mute: Whether the member is muted.
-    :ivar MemberFlags flags: The guild member flags. Default to 0.
-    :ivar Optional[bool] pending: Whether the member is pending to pass membership screening.
-    :ivar Optional[Permissions] permissions: Whether the member has permissions.
-    :ivar Optional[str] communication_disabled_until: How long until they're unmuted, if any.
-    """
+    If `ttl` and `max_values` are set to None, the cache will just be a regular dict, with no culling.
 
-    user: Optional[User] = field(converter=User, default=None, add_client=True)
-    nick: Optional[str] = field(default=None)
-    _avatar: Optional[str] = field(default=None, discord_name="avatar", repr=False)
-    roles: List[int] = field(converter=convert_list(int))
-    joined_at: datetime = field(converter=datetime.fromisoformat, repr=False)
-    premium_since: Optional[datetime] = field(
-        converter=datetime.fromisoformat, default=None, repr=False
-    )
-    deaf: bool = field()
-    mute: bool = field()
-    flags: MemberFlags = field(converter=convert_int(MemberFlags), repr=False)
-    is_pending: Optional[bool] = field(default=None, repr=False)
-    pending: Optional[bool] = field(default=None, repr=False)
-    permissions: Optional[Permissions] = field(
-        converter=convert_int(Permissions), default=None, repr=False
+    Args:
+        ttl: The time to live of an object in the cache
+        hard_limit: The hard limit of values allowed to be within the cache
+        soft_limit: The amount of values allowed before objects expire due to ttl
+
+    Returns:
+        dict or TTLCache based on parameters passed
+
+    """
+    if ttl is None and hard_limit is None:
+        return {}
+    if ttl == 0 and hard_limit == 0 and soft_limit == 0:
+        return NullCache()
+    if not soft_limit:
+        soft_limit = int(hard_limit / 4) if hard_limit else 50
+    return TTLCache(
+        hard_limit=hard_limit or float("inf"),
+        soft_limit=soft_limit or 0,
+        ttl=ttl or float("inf"),
     )
-    communication_disabled_until: Optional[datetime.isoformat] = field(
-        converter=datetime.fromisoformat, default=None
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GlobalCache:
+    _client: "Client" = attrs.field(
+        repr=False,
     )
-    hoisted_role: Optional[Any] = field(
-        default=None, repr=False
-    )  # TODO: Investigate what this is for when documented by Discord.
 
-    def __getattr__(self, name):
-        # Forward any attributes the user has to make it easier for devs
-        try:
-            return getattr(self.user, name)
-        except AttributeError as e:
-            raise AttributeError(f"Neither `User` nor `Member` have attribute {name}") from e
+    # Non expiring discord objects cache
+    user_cache: dict = attrs.field(repr=False, factory=dict)  # key: user_id
+    member_cache: dict = attrs.field(repr=False, factory=dict)  # key: (guild_id, user_id)
+    channel_cache: dict = attrs.field(repr=False, factory=dict)  # key: channel_id
+    guild_cache: dict = attrs.field(repr=False, factory=dict)  # key: guild_id
+
+    # Expiring discord objects cache
+    message_cache: TTLCache = attrs.field(repr=False, factory=TTLCache)  # key: (channel_id, message_id)
+    role_cache: TTLCache = attrs.field(repr=False, factory=dict)  # key: role_id
+    voice_state_cache: TTLCache = attrs.field(repr=False, factory=dict)  # key: user_id
+    bot_voice_state_cache: dict = attrs.field(repr=False, factory=dict)  # key: guild_id
+
+    enable_emoji_cache: bool = attrs.field(repr=False, default=False)
+    """If the emoji cache should be enabled. Default: False"""
+    emoji_cache: Optional[dict] = attrs.field(repr=False, default=None, init=False)  # key: emoji_id
+
+    # Expiring id reference cache
+    dm_channels: TTLCache = attrs.field(repr=False, factory=TTLCache)  # key: user_id
+    user_guilds: TTLCache = attrs.field(repr=False, factory=dict)  # key: user_id; value: set[guild_id]
+
+    logger: Logger = attrs.field(repr=False, init=False, factory=get_logger)
+
+    def __attrs_post_init__(self) -> None:
+        if not isinstance(self.message_cache, TTLCache):
+            self.logger.warning(
+                "Disabling cache limits for message_cache is not recommended! This can result in very high memory usage"
+            )
 
-    @property
-    def voice_state(self) -> Optional["VoiceState"]:
-        """
-        .. versionadded:: 4.4.0
+        # enable emoji cache
+        if self.enable_emoji_cache:
+            self.emoji_cache = {}
 
-        Returns the current voice state of the member, if any.
+    # region User cache
 
-        :rtype: VoiceState
+    async def fetch_user(self, user_id: "Snowflake_Type") -> User:
         """
-        if not self._client:
-            raise LibraryException(code=13)
+        Fetch a user by their ID.
 
-        from .gw import VoiceState
+        Args:
+            user_id: The user's ID
 
-        return self._client.cache[VoiceState].get(self.id)
+        Returns:
+            User object if found
 
-    @property
-    def guild(self) -> Optional["Guild"]:
         """
-        .. versionadded:: 4.4.0
+        user_id = to_snowflake(user_id)
 
-        Attempts to get the guild the member is in.
-        Only works then roles or nick or joined at is present and the guild is cached.
+        user = self.user_cache.get(user_id)
+        if user is None:
+            data = await self._client.http.get_user(user_id)
+            user = self.place_user_data(data)
+        return user
 
-        :return: The guild this member belongs to.
-        :rtype: Guild
+    def get_user(self, user_id: Optional["Snowflake_Type"]) -> Optional[User]:
         """
-        _id = self.guild_id
-        from .guild import Guild
+        Get a user by their ID.
 
-        if not _id or isinstance(_id, LibraryException):
-            return
+        Args:
+            user_id: The user's ID
 
-        return self._client.cache[Guild].get(_id, None)
+        Returns:
+            User object if found
+        """
+        return self.user_cache.get(to_optional_snowflake(user_id))
 
-    @property
-    def guild_id(self) -> Optional[Union[Snowflake, LibraryException]]:
+    def place_user_data(self, data: discord_typings.UserData) -> User:
         """
-        .. versionadded:: 4.3.2
+        Take json data representing a User, process it, and cache it.
 
-        Attempts to get the guild ID the member is in.
-        Only works when roles or nick or joined at is present and the guild is cached.
+        Args:
+            data: json representation of user
 
-        :return: The ID of the guild this member belongs to.
-        :rtype: Optional[Union[Snowflake, LibraryException]]
+        Returns:
+            The processed User data
         """
+        user_id = to_snowflake(data["id"])
 
-        if hasattr(self, "_guild_id"):
-            return self._guild_id
+        user = self.user_cache.get(user_id)
 
-        elif _id := self._extras.get("guild_id"):
-            return Snowflake(_id)
+        if user is None:
+            user = User.from_dict(data, self._client)
+            self.user_cache[user_id] = user
+        else:
+            user.update_from_dict(data)
+        return user
 
-        if not self._client:
-            raise LibraryException(code=13)
+    def delete_user(self, user_id: "Snowflake_Type") -> None:
+        """
+        Delete a user from the cache.
 
-        from .guild import Guild
+        Args:
+            user_id: The user's ID
+        """
+        self.user_cache.pop(to_snowflake(user_id), None)
 
-        if self.roles:
-            for guild in self._client.cache[Guild].values.values():
-                for role in guild.roles:
-                    if role.id in self.roles:
-                        self._extras["guild_id"] = int(guild.id)
-                        return guild.id
+    # endregion User cache
 
-        possible_guilds: List[Guild] = []
+    # region Member cache
 
-        if self.nick:
+    async def fetch_member(self, guild_id: "Snowflake_Type", user_id: "Snowflake_Type") -> Member:
+        """
+        Fetch a member by their guild and user IDs.
 
-            def check(_member: Member):
-                return _member.nick == self.nick and _member.id == self.id
+        Args:
+            guild_id: The ID of the guild this user belongs to
+            user_id: The ID of the user
 
-            for guild in self._client.cache[Guild].values.values():
-                if len(search_iterable(guild.members, check=check)) > 0:
-                    possible_guilds.append(guild)
+        Returns:
+            Member object if found
 
-        if len(possible_guilds) == 1:
-            self._extras["guild_id"] = int(possible_guilds[0].id)
-            return possible_guilds[0].id
+        """
+        guild_id = to_snowflake(guild_id)
+        user_id = to_snowflake(user_id)
+        member = self.member_cache.get((guild_id, user_id))
+        if member is None:
+            data = await self._client.http.get_member(guild_id, user_id)
+            member = self.place_member_data(guild_id, data)
+        return member
 
-        elif not possible_guilds:
-            possible_guilds = list(self._client.cache[Guild].values.values())
+    def get_member(self, guild_id: Optional["Snowflake_Type"], user_id: Optional["Snowflake_Type"]) -> Optional[Member]:
+        """
+        Get a member by their guild and user IDs.
 
-        for guild in possible_guilds:
-            for member in guild.members:
-                if member.joined_at == self.joined_at:
-                    self._extras["guild_id"] = int(guild.id)
-                    return guild.id
+        Args:
+            guild_id: The ID of the guild this user belongs to
+            user_id: The ID of the user
 
-        else:
-            return LibraryException(
-                code=12, message="the guild_id could not be retrieved, please insert one!"
-            )
+        Returns:
+            Member object if found
+        """
+        return self.member_cache.get((to_optional_snowflake(guild_id), to_optional_snowflake(user_id)))
+
+    def place_member_data(
+        self, guild_id: "Snowflake_Type", data: discord_typings.resources.guild.GuildMemberData
+    ) -> Member:
+        """
+        Take json data representing a User, process it, and cache it.
 
-    @property
-    def avatar(self) -> Optional[str]:
-        """Returns the user's avatar hash, if any."""
-        return self._avatar or getattr(self.user, "avatar", None)
+        Args:
+            guild_id: The ID of the guild this member belongs to
+            data: json representation of the member
 
-    @property
-    def id(self) -> Snowflake:
+        Returns:
+            The processed member
         """
-        .. versionadded:: 4.1.0
+        guild_id = to_snowflake(guild_id)
+        is_user = "member" in data
+        user_id = to_snowflake(data["user"]["id"] if "user" in data else data["id"])
+
+        member = self.member_cache.get((guild_id, user_id))
+        if member is None:
+            member_extra = {"guild_id": guild_id}
+            member = data["member"] if is_user else data
+            member.update(member_extra)
+
+            member = Member.from_dict(data, self._client)
+            self.member_cache[(guild_id, user_id)] = member
+        else:
+            member.update_from_dict(data)
 
-        Returns the ID of the user.
+        self.place_user_guild(user_id, guild_id)
+        if guild := self.guild_cache.get(guild_id):
+            # todo: this is slow, find a faster way
+            guild._member_ids.add(user_id)
+        return member
 
-        :return: The ID of the user
-        :rtype: Snowflake
+    def delete_member(self, guild_id: "Snowflake_Type", user_id: "Snowflake_Type") -> None:
         """
-        return self.user.id if self.user else None
+        Delete a member from the cache.
 
-    @property
-    def mention(self) -> str:
+        Args:
+            guild_id: The ID of the guild this user belongs to
+            user_id: The ID of the user
         """
-        .. versionadded:: 4.1.0
+        user_id = to_snowflake(user_id)
+        guild_id = to_snowflake(guild_id)
 
-        Returns a string that allows you to mention the given member.
+        if member := self.member_cache.pop((guild_id, user_id), None):
+            if member.guild:
+                member.guild._member_ids.discard(user_id)
 
-        :return: The string of the mentioned member.
-        :rtype: str
+        self.delete_user_guild(user_id, guild_id)
+
+    def place_user_guild(self, user_id: "Snowflake_Type", guild_id: "Snowflake_Type") -> None:
         """
-        return f"<@{'!' if self.nick else ''}{self.id}>"
+        Add a guild to the list of guilds a user has joined.
 
-    @property
-    def name(self) -> str:
+        Args:
+            user_id: The ID of the user
+            guild_id: The ID of the guild to add
         """
-        .. versionadded:: 4.2.0
+        user_id = to_snowflake(user_id)
+        guild_id = to_snowflake(guild_id)
+        if user_id == self._client.user.id:
+            # noinspection PyProtectedMember
+            self._client.user._add_guilds({guild_id})
+        else:
+            guilds = self.user_guilds.get(user_id)
+            if guilds:
+                guilds.add(guild_id)
+            else:
+                guilds = {guild_id}
+            self.user_guilds[user_id] = guilds
 
-        Returns the string of either the user's nickname or username.
+    def delete_user_guild(self, user_id: "Snowflake_Type", guild_id: "Snowflake_Type") -> None:
+        """
+        Remove a guild from the list of a guilds a user has joined.
 
-        :return: The name of the member
-        :rtype: str
+        Args:
+            user_id: The ID of the user
+            guild_id: The ID of the guild to add
         """
-        return self.nick or (self.user.username if self.user else None)
+        user_id = to_snowflake(user_id)
+        guild_id = to_snowflake(guild_id)
+
+        if user_id == self._client.user.id:
+            # noinspection PyProtectedMember
+            self._client.user._guild_ids.discard(guild_id)
+        else:
+            guilds = self.user_guilds.get(user_id)
+            if guilds:
+                guilds.discard(guild_id)
+            else:
+                guilds = {}
+            self.user_guilds[user_id] = guilds
 
-    async def ban(
+    async def is_user_in_guild(
         self,
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        seconds: Optional[int] = 0,
-        minutes: Optional[int] = MISSING,
-        hours: Optional[int] = MISSING,
-        days: Optional[int] = MISSING,
-        reason: Optional[str] = None,
-    ) -> None:
-        """
-        .. versionadded:: 4.0.2
-
-        .. versionchanged:: 4.3.2
-            Method has been aligned to changes in the Discord API. You can now input days, hours, minutes and seconds,
-            as long as it doesn't exceed 604800 seconds in total for deleting messages, instead of only days.
-
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required
-
-        Bans the member from a guild.
-
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to ban the member from
-        :param Optional[int] seconds: Number of seconds to delete messages, from 0 to 604800. Defaults to 0
-        :param Optional[int] minutes: Number of minutes to delete messages, from 0 to 10080
-        :param Optional[int] hours: Number of hours to delete messages, from 0 to 168
-        :param Optional[int] days: Number of days to delete messages, from 0 to 7
-        :param Optional[str] reason: The reason of the ban
-        """
-
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        user_id: "Snowflake_Type",
+        guild_id: "Snowflake_Type",
+    ) -> bool:
+        """
+        Determine if a user is in a specified guild.
+
+        Args:
+            user_id: The ID of the user to check
+            guild_id: The ID of the guild
+
+        """
+        user_id = to_snowflake(user_id)
+        guild_id = to_snowflake(guild_id)
 
+        # Try to get guild members list from the cache, without sending requests
+        guild = self.get_guild(guild_id)
+        if guild and (user_id in guild._member_ids):
+            return True
+
+        # If no such guild in cache or member not in guild cache, try to get member directly. May send requests
+        try:
+            member = await self.fetch_member(guild_id, user_id)
+        except (NotFound, Forbidden):  # there is no such member in the guild (as per request)
+            pass
         else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (Snowflake, int)) else int(guild_id.id)
-            )
+            if member:
+                return True
 
-        if days is not MISSING:
-            seconds += days * 24 * 3600
-        if hours is not MISSING:
-            seconds += hours * 3600
-        if minutes is not MISSING:
-            seconds += minutes * 60
-
-        if seconds > 604800:
-            raise LibraryException(
-                code=12,
-                message="The amount of total seconds to delete messages exceeds the limit Discord provides (604800)",
-            )
+        return False
+
+    async def fetch_user_guild_ids(
+        self,
+        user_id: "Snowflake_Type",
+    ) -> List["Snowflake_Type"]:
+        """
+        Fetch a list of IDs for the guilds a user has joined.
+
+        Args:
+            user_id: The ID of the user
+        Returns:
+            A list of snowflakes for the guilds the client can see the user is within
+        """
+        user_id = to_snowflake(user_id)
+        guild_ids = self.user_guilds.get(user_id)
+        if not guild_ids:
+            guild_ids = [
+                guild_id for guild_id in self._client.user._guild_ids if await self.is_user_in_guild(user_id, guild_id)
+            ]
+            self.user_guilds[user_id] = set(guild_ids)
+        return guild_ids
+
+    def get_user_guild_ids(self, user_id: "Snowflake_Type") -> List["Snowflake_Type"]:
+        """
+        Get a list of IDs for the guilds the user has joined.
 
-        await self._client.create_guild_ban(
-            guild_id=_guild_id,
-            user_id=int(self.user.id),
-            reason=reason,
-            delete_message_seconds=seconds,
-        )
+        Args:
+            user_id: The ID of the user
 
-    async def kick(
+        Returns:
+            A list of snowflakes for the guilds the client can see the user is within
+        """
+        return list(self.user_guilds.get(to_snowflake(user_id)))
+
+    # endregion Member cache
+
+    # region Message cache
+
+    async def fetch_message(
         self,
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        reason: Optional[str] = None,
-    ) -> None:
+        channel_id: "Snowflake_Type",
+        message_id: "Snowflake_Type",
+    ) -> Message:
+        """
+        Fetch a message from a channel based on their IDs.
+
+        Args:
+            channel_id: The ID of the channel the message is in
+            message_id: The ID of the message
+
+        Returns:
+            The message if found
         """
-        .. versionadded:: 4.0.2
+        channel_id = to_snowflake(channel_id)
+        message_id = to_snowflake(message_id)
+        message = self.message_cache.get((channel_id, message_id))
+
+        if message is None:
+            data = await self._client.http.get_message(channel_id, message_id)
+            message = self.place_message_data(data)
+            if message.channel is None:
+                await self.fetch_channel(channel_id)
 
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required.
+            if not message.guild and isinstance(message.channel, GuildChannel):
+                message._guild_id = message.channel._guild_id
+        return message
 
-        Kicks the member from a guild.
+    def get_message(
+        self, channel_id: Optional["Snowflake_Type"], message_id: Optional["Snowflake_Type"]
+    ) -> Optional[Message]:
+        """
+        Get a message from a channel based on their IDs.
+
+        Args:
+            channel_id: The ID of the channel the message is in
+            message_id: The ID of the message
 
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to kick the member from
-        :param Optional[str] reason: The reason for the kick
+        Returns:
+            The message if found
         """
-        if not self._client:
-            raise LibraryException(code=13)
+        return self.message_cache.get((to_optional_snowflake(channel_id), to_optional_snowflake(message_id)))
 
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
+    def place_message_data(self, data: discord_typings.MessageData) -> Message:
+        """
+        Take json data representing a message, process it, and cache it.
 
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        Args:
+            data: json representation of the message
 
+        Returns:
+            The processed message
+        """
+        channel_id = to_snowflake(data["channel_id"])
+        message_id = to_snowflake(data["id"])
+        message = self.message_cache.get((channel_id, message_id))
+        if message is None:
+            message = Message.from_dict(data, self._client)
+            self.message_cache[(channel_id, message_id)] = message
         else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (Snowflake, int)) else int(guild_id.id)
-            )
+            message.update_from_dict(data)
+        return message
 
-        await self._client.create_guild_kick(
-            guild_id=_guild_id,
-            user_id=int(self.user.id),
-            reason=reason,
-        )
+    def delete_message(self, channel_id: "Snowflake_Type", message_id: "Snowflake_Type") -> None:
+        """
+        Deletes a message from the cache.
+
+        Args:
+            channel_id: The ID of the channel the message is in
+            message_id: The ID of the message
+        """
+        self.message_cache.pop((to_snowflake(channel_id), to_snowflake(message_id)), None)
 
-    async def add_role(
+    # endregion Message cache
+
+    # region Channel cache
+    async def fetch_channel(
         self,
-        role: Union[Role, int, Snowflake],
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        reason: Optional[str] = None,
-    ) -> None:
-        """
-        .. versionadded:: 4.0.2
-
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required.
-
-        This method adds a role to a member.
-
-        :param Union[Role, int, Snowflake] role: The role to add. Either ``Role`` object or role_id
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to add the roles to the member
-        :param Optional[str] reason: The reason why the roles are added
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-
-        _role = int(role.id) if isinstance(role, Role) else int(role)
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        channel_id: "Snowflake_Type",
+    ) -> "TYPE_ALL_CHANNEL":
+        """
+        Get a channel based on its ID.
 
-        else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (Snowflake, int)) else int(guild_id.id)
-            )
+        Args:
+            channel_id: The ID of the channel
 
-        await self._client.add_member_role(
-            guild_id=_guild_id,
-            user_id=int(self.user.id),
-            role_id=_role,
-            reason=reason,
-        )
+        Returns:
+            The channel if found
+        """
+        channel_id = to_snowflake(channel_id)
+        channel = self.channel_cache.get(channel_id)
+        if channel is None:
+            try:
+                data = await self._client.http.get_channel(channel_id)
+                channel = self.place_channel_data(data)
+            except Forbidden:
+                self.logger.warning(f"Forbidden access to channel {channel_id}. Generating fallback channel object")
+                channel = BaseChannel.from_dict({"id": channel_id, "type": MISSING}, self._client)
+        return channel
 
-    async def remove_role(
-        self,
-        role: Union[Role, int],
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        reason: Optional[str] = None,
-    ) -> None:
+    def get_channel(self, channel_id: Optional["Snowflake_Type"]) -> Optional["TYPE_ALL_CHANNEL"]:
         """
-        .. versionadded:: 4.0.2
+        Get a channel based on its ID.
 
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required.
+        Args:
+            channel_id: The ID of the channel
 
-        This method removes a role from a member.
+        Returns:
+            The channel if found
+        """
+        return self.channel_cache.get(to_optional_snowflake(channel_id))
 
-        :param Union[Role, int] role: The role to remove. Either ``Role`` object or role_id
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to remove the roles of the member
-        :param Optional[str] reason: The reason why the roles are removed
+    def place_channel_data(self, data: discord_typings.ChannelData) -> "TYPE_ALL_CHANNEL":
         """
-        if not self._client:
-            raise LibraryException(code=13)
+        Take json data representing a channel, process it, and cache it.
 
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        Args:
+            data: json representation of the channel
 
+        Returns:
+            The processed channel
+        """
+        channel_id = to_snowflake(data["id"])
+        channel = self.channel_cache.get(channel_id)
+        if channel is None:
+            channel = BaseChannel.from_dict_factory(data, self._client)
+            self.channel_cache[channel_id] = channel
+            if guild := getattr(channel, "guild", None):
+                if isinstance(channel, ThreadChannel):
+                    guild._thread_ids.add(channel.id)
+                elif isinstance(channel, GuildChannel):
+                    guild._channel_ids.add(channel.id)
+                guild._channel_gui_positions = {}
         else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (Snowflake, int)) else int(guild_id.id)
-            )
-        _role = int(role.id) if isinstance(role, Role) else int(role)
+            # Create entire new channel object if the type changes
+            channel_type = data.get("type", None)
+            if channel_type and channel_type != channel.type:
+                self.channel_cache.pop(channel_id)
+                channel = BaseChannel.from_dict_factory(data, self._client)
+            else:
+                channel.update_from_dict(data)
+                if guild := getattr(channel, "guild", None):
+                    guild._channel_gui_positions = {}
 
-        await self._client.remove_member_role(
-            guild_id=_guild_id,
-            user_id=int(self.user.id),
-            role_id=_role,
-            reason=reason,
-        )
+        return channel
 
-    async def send(
-        self,
-        content: Optional[str] = MISSING,
-        *,
-        components: Optional[
-            Union[
-                "ActionRow",
-                "Button",
-                "SelectMenu",
-                List["ActionRow"],
-                List["Button"],
-                List["SelectMenu"],
-            ]
-        ] = MISSING,
-        tts: Optional[bool] = MISSING,
-        attachments: Optional[List["Attachment"]] = MISSING,
-        files: Optional[Union[File, List[File]]] = MISSING,
-        embeds: Optional[Union["Embed", List["Embed"]]] = MISSING,
-        allowed_mentions: Optional[Union[AllowedMentions, dict]] = MISSING,
-    ) -> "Message":
-        """
-        .. versionadded:: 4.0.2
-
-        Sends a DM to the member.
-
-        :param Optional[str] content: The contents of the message as a string or string-converted value.
-        :param Optional[Union[ActionRow, Button, SelectMenu, List[ActionRow], List[Button], List[SelectMenu]]] components: A component, or list of components for the message.
-        :param Optional[bool] tts: Whether the message utilizes the text-to-speech Discord programme or not.
-        :param Optional[List[Attachment]] attachments:
-            .. versionadded:: 4.3.0
-
-            The attachments to attach to the message. Needs to be uploaded to the CDN first
-        :param Optional[Union[File, List[File]]] files:
-            .. versionadded:: 4.2.0
-
-            A file or list of files to be attached to the message.
-        :param Optional[Union[Embed, List[Embed]]] embeds: An embed, or list of embeds for the message.
-        :param Optional[Union[AllowedMentions, dict]] allowed_mentions: The allowed mentions for the message.
-        :return: The sent message as an object.
-        :rtype: Message
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-        from ...client.models.component import _build_components
-        from .message import Message
-
-        _content: str = "" if content is MISSING else content
-        _tts: bool = False if tts is MISSING else tts
-        _attachments = [] if attachments is MISSING else [a._json for a in attachments]
-        _embeds: list = (
-            []
-            if not embeds or embeds is MISSING
-            else ([embed._json for embed in embeds] if isinstance(embeds, list) else [embeds._json])
-        )
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
-        if not components or components is MISSING:
-            _components = []
-        else:
-            _components = _build_components(components=components)
+    def place_dm_channel_id(self, user_id: "Snowflake_Type", channel_id: "Snowflake_Type") -> None:
+        """
+        Cache that the bot is active within a DM channel.
+
+        Args:
+            user_id: The id of the user this DM channel belongs to
+            channel_id: The id of the DM channel
+
+        """
+        self.dm_channels[to_snowflake(user_id)] = to_snowflake(channel_id)
 
-        if not files or files is MISSING:
-            _files = []
-        elif isinstance(files, list):
-            _files = [file._json_payload(id) for id, file in enumerate(files)]
+    async def fetch_dm_channel_id(self, user_id: "Snowflake_Type") -> "Snowflake_Type":
+        """
+        Get the DM channel ID for a user.
+
+        Args:
+            user_id: The ID of the user
+        """
+        user_id = to_snowflake(user_id)
+        channel_id = self.dm_channels.get(user_id)
+        if channel_id is None:
+            data = await self._client.http.create_dm(user_id)
+            channel = self.place_channel_data(data)
+            channel_id = channel.id
+        return channel_id
+
+    async def fetch_dm_channel(self, user_id: "Snowflake_Type") -> "DM":
+        """
+        Fetch the DM channel for a user.
+
+        Args:
+            user_id: The ID of the user
+        """
+        user_id = to_snowflake(user_id)
+        channel_id = await self.fetch_dm_channel_id(user_id)
+        return await self.fetch_channel(channel_id)
+
+    def get_dm_channel(self, user_id: Optional["Snowflake_Type"]) -> Optional["DM"]:
+        """
+        Get the DM channel for a user.
+
+        Args:
+            user_id: The ID of the user
+        """
+        user_id = to_optional_snowflake(user_id)
+        channel_id = self.dm_channels.get(user_id)
+        return None if channel_id is None else self.get_channel(channel_id)
+
+    def delete_channel(self, channel_id: "Snowflake_Type") -> None:
+        """
+        Delete a channel from the cache.
+
+        Args:
+            channel_id: The channel to be deleted
+        """
+        channel_id = to_snowflake(channel_id)
+        channel = self.channel_cache.pop(channel_id, None)
+        if guild := getattr(channel, "guild", None):
+            if isinstance(channel, ThreadChannel):
+                guild._thread_ids.discard(channel.id)
+            elif isinstance(channel, GuildChannel):
+                guild._channel_ids.discard(channel.id)
+            guild._channel_gui_positions = {}
+
+    # endregion Channel cache
+
+    # region Guild cache
+
+    async def fetch_guild(self, guild_id: "Snowflake_Type") -> Guild:
+        """
+        Fetch a guild based on its ID.
+
+        Args:
+            guild_id: The ID of the guild
+
+        Returns:
+            The guild if found
+        """
+        guild_id = to_snowflake(guild_id)
+        guild = self.guild_cache.get(guild_id)
+        if guild is None:
+            data = await self._client.http.get_guild(guild_id)
+            guild = self.place_guild_data(data)
+        return guild
+
+    def get_guild(self, guild_id: Optional["Snowflake_Type"]) -> Optional[Guild]:
+        """
+        Get a guild based on its ID.
+
+        Args:
+            guild_id: The ID of the guild.
+
+        Returns:
+            The guild if found
+        """
+        return self.guild_cache.get(to_optional_snowflake(guild_id))
+
+    def place_guild_data(self, data: discord_typings.GuildData) -> Guild:
+        """
+        Take json data representing a guild, process it, and cache it.
+
+        Args:
+            data: json representation of the guild
+
+        Returns:
+            The processed guild
+        """
+        guild_id = to_snowflake(data["id"])
+        guild: Guild = self.guild_cache.get(guild_id)
+        if guild is None:
+            guild = Guild.from_dict(data, self._client)
+            self.guild_cache[guild_id] = guild
         else:
-            _files = [files._json_payload(0)]
-            files = [files]
+            guild.update_from_dict(data)
+        return guild
 
-        _files.extend(_attachments)
+    def delete_guild(self, guild_id: "Snowflake_Type") -> None:
+        """
+        Delete a guild from the cache.
 
-        payload = dict(
-            content=_content,
-            tts=_tts,
-            attachments=_files,
-            embeds=_embeds,
-            components=_components,
-            allowed_mentions=_allowed_mentions,
-        )
-        channel = Channel(**await self._client.create_dm(recipient_id=int(self.user.id)))
-        res = await self._client.create_message(
-            channel_id=int(channel.id), payload=payload, files=files
-        )
+        Args:
+            guild_id: The ID of the guild
+        """
+        if guild := self.guild_cache.pop(to_snowflake(guild_id), None):
+            # delete associated objects
+            [self.delete_channel(c) for c in guild.channels]
+            [self.delete_member(m.id, guild_id) for m in guild.members]
+            [self.delete_role(r) for r in guild.roles]
+            if self.enable_emoji_cache:  # todo: this is ungodly slow, find a better way to do this
+                for emoji in self.emoji_cache.values():
+                    if emoji._guild_id == guild_id:
+                        self.delete_emoji(emoji)
+
+    # endregion Guild cache
 
-        return Message(**res, _client=self._client)
+    # region Roles cache
 
-    async def modify(
+    async def fetch_role(
         self,
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        nick: Optional[str] = MISSING,
-        roles: Optional[List[int]] = MISSING,
-        mute: Optional[bool] = MISSING,
-        deaf: Optional[bool] = MISSING,
-        channel_id: Optional[Union[Channel, int, Snowflake]] = MISSING,
-        communication_disabled_until: Optional[datetime.isoformat] = MISSING,
-        reason: Optional[str] = None,
-    ) -> "Member":
-        """
-        .. versionadded:: 4.0.2
-
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required.
-
-        Modifies the member of a guild.
-
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to modify the member on
-        :param Optional[str] nick: The nickname of the member
-        :param Optional[List[int]] roles: A list of all role ids the member has
-        :param Optional[bool] mute: whether the user is muted in voice channels
-        :param Optional[bool] deaf: whether the user is deafened in voice channels
-        :param Optional[Union[Channel, int, Snowflake]] channel_id: id of channel to move user to (if they are connected to voice)
-        :param Optional[datetime.isoformat] communication_disabled_until: when the user's timeout will expire and the user will be able to communicate in the guild again (up to 28 days in the future)
-        :param Optional[str] reason: The reason of the modifying
-        :return: The modified member object
-        :rtype: Member
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        guild_id: "Snowflake_Type",
+        role_id: "Snowflake_Type",
+    ) -> Role:
+        """
+        Fetch a role based on the guild and its own ID.
 
-        else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
-            )
+        Args:
+            guild_id: The ID of the guild this role belongs to
+            role_id: The ID of the role
 
-        payload = {}
-        if nick is not MISSING:
-            payload["nick"] = nick
-
-        if roles is not MISSING:
-            payload["roles"] = roles
-
-        if channel_id is not MISSING:
-            payload["channel_id"] = (
-                int(channel_id.id)
-                if isinstance(channel_id, Channel)
-                else (int(channel_id) if channel_id is not None else None)
-            )
+        Returns:
+            The role if found
+        """
+        guild_id = to_snowflake(guild_id)
+        role_id = to_snowflake(role_id)
+        role = self.role_cache.get(role_id)
+        if role is None:
+            data = await self._client.http.get_roles(guild_id)
+            role = self.place_role_data(guild_id, data).get(role_id)
+        return role
 
-        if mute is not MISSING:
-            payload["mute"] = mute
+    def get_role(self, role_id: Optional["Snowflake_Type"]) -> Optional[Role]:
+        """
+        Get a role based on the role ID.
 
-        if deaf is not MISSING:
-            payload["deaf"] = deaf
+        Args:
+            role_id: The ID of the role
+
+        Returns:
+            The role if found
+        """
+        return self.role_cache.get(to_optional_snowflake(role_id))
 
-        if communication_disabled_until is not MISSING:
-            payload["communication_disabled_until"] = communication_disabled_until
+    def place_role_data(
+        self, guild_id: "Snowflake_Type", data: List[Dict["Snowflake_Type", Any]]
+    ) -> Dict["Snowflake_Type", Role]:
+        """
+        Take json data representing a role, process it, and cache it.
 
-        res = await self._client.modify_member(
-            user_id=int(self.user.id),
-            guild_id=_guild_id,
-            payload=payload,
-            reason=reason,
-        )
+        Can handle multiple roles at once
 
-        self.update(res)
-        return self
+        Args:
+            guild_id: The ID of the guild this role belongs to
+            data: json representation of the role
 
-    async def add_to_thread(
-        self,
-        thread_id: Union[int, Snowflake, Channel],
-    ) -> None:
+        Returns:
+            The processed role
         """
-        .. versionadded:: 4.0.2
+        guild_id = to_snowflake(guild_id)
+
+        roles: Dict["Snowflake_Type", Role] = {}
+        for role_data in data:  # todo not update cache expiration order for roles
+            role_data.update({"guild_id": guild_id})
+            role_id = to_snowflake(role_data["id"])
+
+            role = self.role_cache.get(role_id)
+            if role is None:
+                role = Role.from_dict(role_data, self._client)
+                self.role_cache[role_id] = role
+            else:
+                role.update_from_dict(role_data)
+
+            roles[role_id] = role
 
-        Adds the member to a thread.
+        return roles
 
-        :param Union[int, Snowflake, Channel] thread_id: The id of the thread to add the member to
+    def delete_role(self, role_id: "Snowflake_Type") -> None:
         """
-        if not self._client:
-            raise LibraryException(code=13)
+        Delete a role from the cache.
 
-        _thread_id = int(thread_id.id) if isinstance(thread_id, Channel) else int(thread_id)
+        Args:
+            role_id: The ID of the role
+        """
+        if role := self.role_cache.pop(to_snowflake(role_id), None):
+            if guild := self.get_guild(role._guild_id):
+                # noinspection PyProtectedMember
+                guild._role_ids.discard(role_id)
+
+    # endregion Role cache
 
-        await self._client.add_member_to_thread(
-            user_id=int(self.user.id),
-            thread_id=_thread_id,
-        )
+    # region Voice cache
 
-    def get_avatar_url(
-        self, guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING
-    ) -> Optional[str]:
+    def get_voice_state(self, user_id: Optional["Snowflake_Type"]) -> Optional[VoiceState]:
         """
-        .. versionadded:: 4.2.0
+        Get a voice state by their guild and user IDs.
+
+        Args:
+            user_id: The ID of the user
 
-        .. versionchanged:: 4.3.0
-            Has been renamed to `get_avatar_url` instead of `get_member_avatar_url`
+        Returns:
+            VoiceState object if found
 
-        .. versionchanged:: 4.3.2
-            ``guild_id`` is no longer required.
+        """
+        return self.voice_state_cache.get(to_optional_snowflake(user_id))
+
+    async def place_voice_state_data(self, data: discord_typings.VoiceStateData) -> Optional[VoiceState]:
+        """
+        Take json data representing a VoiceState, process it, and cache it.
 
-        Returns the URL of the member's avatar for the specified guild.
+        Args:
+            data: json representation of the VoiceState
 
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild to get the member's avatar from
-        :return: URL of the members's avatar (None will be returned if no avatar is set)
-        :rtype: str
+        Returns:
+            The processed VoiceState object
         """
-        if not self.avatar or self.avatar == self.user.avatar:
-            return None
+        user_id = to_snowflake(data["user_id"])
 
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        if old_state := self.get_voice_state(user_id):
+            # noinspection PyProtectedMember
+            if user_id in old_state.channel._voice_member_ids:
+                # noinspection PyProtectedMember
+                old_state.channel._voice_member_ids.remove(user_id)
 
+        # check if the channel_id is None
+        # if that is the case, the user disconnected, and we can delete them from the cache
+        if not data["channel_id"]:
+            if user_id in self.voice_state_cache:
+                self.voice_state_cache.pop(user_id)
+            voice_state = None
+
+        # this means the user swapped / joined a channel
         else:
-            _guild_id = (
-                int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
-            )
+            # update the _voice_member_ids of the new channel
+            new_channel = await self.fetch_channel(data["channel_id"])
+            # noinspection PyProtectedMember
+            new_channel._voice_member_ids.append(user_id)
+
+            voice_state = VoiceState.from_dict(data, self._client)
+            self.voice_state_cache[user_id] = voice_state
 
-        url = f"https://cdn.discordapp.com/guilds/{_guild_id}/users/{int(self.user.id)}/avatars/{self.avatar}"
-        url += ".gif" if self.avatar.startswith("a_") else ".png"
-        return url
+        return voice_state
+
+    def delete_voice_state(self, user_id: "Snowflake_Type") -> None:
+        """
+        Delete a voice state from the cache.
 
-    async def get_guild_permissions(
-        self, guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING
-    ) -> Permissions:
+        Args:
+            user_id: The ID of the user
         """
-        .. versionadded:: 4.3.2
+        self.voice_state_cache.pop(to_snowflake(user_id), None)
 
-        Returns the permissions of the member for the specified guild.
+    # endregion Voice cache
 
-        .. note::
-            The permissions returned by this function will not take into account role and
-            user overwrites that can be assigned to channels or categories. If you need
-            these overwrites, look into :meth:`.Channel.get_permissions_for`.
+    # region Bot Voice cache
 
-        :param Guild guild: The guild of the member
-        :return: Base permissions of the member in the specified guild
-        :rtype: Permissions
+    def get_bot_voice_state(self, guild_id: Optional["Snowflake_Type"]) -> Optional[ActiveVoiceState]:
         """
-        from .guild import Guild
+        Get a voice state for the bot, by the guild id.
 
-        if guild_id is MISSING:
-            _guild_id = self.guild_id
-            if isinstance(_guild_id, LibraryException):
-                raise _guild_id
+        Args:
+            guild_id: The id of the guild
 
-        else:
-            _guild_id = int(guild_id.id) if isinstance(guild_id, Guild) else int(guild_id)
+        Returns:
+            ActiveVoiceState if found
+        """
+        return self.bot_voice_state_cache.get(to_optional_snowflake(guild_id))
 
-        guild = Guild(**await self._client.get_guild(int(_guild_id)), _client=self._client)
+    def place_bot_voice_state(self, state: ActiveVoiceState) -> None:
+        """
+        Place an ActiveVoiceState into the cache.
+
+        Args:
+            state: The voice state to cache
+        """
+        if state._guild_id is None:
+            return
 
-        if int(guild.owner_id) == int(self.id):
-            return Permissions.ALL
+        # noinspection PyProtectedMember
+        self.bot_voice_state_cache[to_snowflake(state._guild_id)] = state
 
-        role_everyone = await guild.get_role(int(guild.id))
-        permissions = int(role_everyone.permissions)
+    def delete_bot_voice_state(self, guild_id: "Snowflake_Type") -> None:
+        """
+        Delete an ActiveVoiceState from the cache.
 
-        for role_id in self.roles:
-            role = await guild.get_role(role_id)
-            permissions |= int(role.permissions)
+        Args:
+            guild_id: The id of the guild
+        """
+        self.bot_voice_state_cache.pop(to_snowflake(guild_id), None)
 
-        if Permissions.ADMINISTRATOR in Permissions(permissions):
-            return Permissions.ALL
+    # endregion Bot Voice cache
 
-        return Permissions(permissions)
+    # region Emoji cache
 
-    async def has_permissions(
+    async def fetch_emoji(
         self,
-        *permissions: Union[int, Permissions],
-        channel: Optional[Channel] = MISSING,
-        guild_id: Optional[Union[int, Snowflake, "Guild"]] = MISSING,
-        operator: str = "and",
-    ) -> bool:
-        r"""
-        .. versionadded:: 4.3.2
+        guild_id: "Snowflake_Type",
+        emoji_id: "Snowflake_Type",
+    ) -> "CustomEmoji":
+        """
+        Fetch an emoji based on the guild and its own ID.
 
-        Returns whether the member has the permissions passed.
+        This cache is disabled by default, start your bot with `Client(enable_emoji_cache=True)` to enable it.
 
-        .. note::
-            If the channel argument is present, the function will look if the member has the permissions in the specified channel.
-            If the argument is missing, then it will only consider the member's guild permissions.
-
-        :param Union[int, Permissions] \*permissions: The list of permissions
-        :param Channel channel: The channel where to check for permissions
-        :param Optional[Union[int, Snowflake, Guild]] guild_id: The id of the guild
-        :param Optional[str] operator: The operator to use to calculate permissions. Possible values: `and`, `or`. Defaults to `and`.
-        :return: Whether the member has the permissions
-        :rtype: bool
-        """
-        perms = (
-            await self.get_guild_permissions(guild_id)
-            if channel is MISSING
-            else await channel.get_permissions_for(self)
-        )
+        Args:
+            guild_id: The ID of the guild this emoji belongs to
+            emoji_id: The ID of the emoji
 
-        if operator == "and":
-            return all(perm in perms for perm in permissions)
-        else:
-            return any(perm in perms for perm in permissions)
+        Returns:
+            The Emoji if found
+        """
+        guild_id = to_snowflake(guild_id)
+        emoji_id = to_snowflake(emoji_id)
+        emoji = self.emoji_cache.get(emoji_id) if self.emoji_cache is not None else None
+        if emoji is None:
+            data = await self._client.http.get_guild_emoji(guild_id, emoji_id)
+            emoji = self.place_emoji_data(guild_id, data)
+
+        return emoji
+
+    def get_emoji(self, emoji_id: Optional["Snowflake_Type"]) -> Optional["CustomEmoji"]:
+        """
+        Get an emoji based on the emoji ID.
+
+        This cache is disabled by default, start your bot with `Client(enable_emoji_cache=True)` to enable it.
+
+        Args:
+            emoji_id: The ID of the emoji
+
+        Returns:
+            The Emoji if found
+        """
+        return self.emoji_cache.get(to_optional_snowflake(emoji_id)) if self.emoji_cache is not None else None
+
+    def place_emoji_data(self, guild_id: "Snowflake_Type", data: discord_typings.EmojiData) -> "CustomEmoji":
+        """
+        Take json data representing an emoji, process it, and cache it. This cache is disabled by default, start your bot with `Client(enable_emoji_cache=True)` to enable it.
+
+        Args:
+            guild_id: The ID of the guild this emoji belongs to
+            data: json representation of the emoji
+
+        Returns:
+            The processed emoji
+        """
+        with suppress(KeyError):
+            del data["guild_id"]  # discord sometimes packages a guild_id - this will cause an exception
+
+        emoji = CustomEmoji.from_dict(data, self._client, to_snowflake(guild_id))
+        if self.emoji_cache is not None:
+            self.emoji_cache[emoji.id] = emoji
+
+        return emoji
+
+    def delete_emoji(self, emoji_id: "Snowflake_Type") -> None:
+        """
+        Delete an emoji from the cache.
+
+        Args:
+            emoji_id: The ID of the emoji
+        """
+        if self.emoji_cache is not None:
+            self.emoji_cache.pop(to_snowflake(emoji_id), None)
+
+    # endregion Emoji cache
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/misc.py` & `discord-py-interactions-5.0.0/interactions/models/discord/webhooks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,444 +1,315 @@
-# TODO: This is post-v4.
-#   Reorganise these models based on which big obj uses little obj
-#   Potentially rename some model references to enums, if applicable
-#   Reorganise mixins to its own thing, currently placed here because circular import sucks.
-# also, it should be serialiser* but idk, fl0w'd say something if I left it like that. /shrug
-# pycharm says serializer for me /shrug
-
-import datetime
-from base64 import b64encode
-from io import FileIO, IOBase
-from logging import Logger
-from math import floor
-from os.path import basename
-from typing import List, Optional, Union
-
-from ...base import get_logger
-from ...client.enums import IntEnum, StrEnum
-from ...utils.attrs_utils import DictSerializerMixin, convert_int, convert_list, define, field
-from ...utils.missing import MISSING
-from ..error import LibraryException
-from .flags import Permissions
-
-__all__ = (
-    "AutoModKeywordPresetTypes",
-    "AutoModTriggerType",
-    "AutoModMetaData",
-    "AutoModActionTypes",
-    "AutoModAction",
-    "AutoModTriggerMetadata",
-    "AllowedMentionType",
-    "AllowedMentions",
-    "Snowflake",
-    "Color",
-    "ClientStatus",
-    "IDMixin",
-    "Image",
-    "File",
-    "Overwrite",
-)
-
-log: Logger = get_logger("mixin")
-
-
-@define()
-class Overwrite(DictSerializerMixin):
-    """
-    This is used for the PermissionOverride object.
-
-    :ivar str id: Role or User ID
-    :ivar int type: Type that corresponds ot the ID; 0 for role and 1 for member.
-    :ivar Permissions allow: Permission bit set.
-    :ivar Permissions deny: Permission bit set.
-    """
-
-    id: int = field()
-    type: int = field()
-    allow: Permissions = field(converter=convert_int(Permissions))
-    deny: Permissions = field(converter=convert_int(Permissions))
-
-
-@define()
-class ClientStatus(DictSerializerMixin):
-    """
-    An object that symbolizes the status per client device per session.
-
-    :ivar Optional[str] desktop: User's status set for an active desktop application session
-    :ivar Optional[str] mobile: User's status set for an active mobile application session
-    :ivar Optional[str] web: User's status set for an active web application session
-    """
-
-    desktop: Optional[str] = field(default=None)
-    mobile: Optional[str] = field(default=None)
-    web: Optional[str] = field(default=None)
-
-
-class Snowflake:
-    """
-    .. versionadded:: 4.0.0
-
-    .. important::
-        By default every ID in this library is of this class. This makes some information of them easier accessible.
-        If you need the ID as :class:`int` or :class:`str` object, for example to store it in a database,
-        just call ``str(id)`` or ``int(id)``.
-
-    .. versionchanged:: 4.2.0
-        Added ``__eq__``. You no longer have to convert this object to compare it to a string or integer
-
-    The Snowflake object.
-
-    This snowflake object will have features closely related to the
-    API schema. In turn, compared to regular d.py's treated snowflakes,
-    these will be treated as strings.
-
-
-    (Basically, snowflakes will be treated as if they were from d.py 0.16.12)
-
-    .. note::
-        You can still provide integers to them, to ensure ease of use of transition and/or
-        if discord API for some odd reason will switch to integer.
-    """
-
-    __slots__ = "_snowflake"
-
-    # Slotting properties are pointless, they are not in-memory
-    # and are instead computed in-model.
-
-    def __init__(self, snowflake: Union[int, str, "Snowflake"]) -> None:
-        self._snowflake = str(snowflake)
-
-    def __str__(self) -> str:
-        # This is overridden for model comparison between IDs.
-        return self._snowflake
-
-    def __int__(self) -> int:
-        # Easier to use for HTTP calling instead of int(str(obj)).
-        return int(self._snowflake)
-
-    @property
-    def increment(self) -> int:
-        """
-        This is the 'Increment' portion of the snowflake.
-        This is incremented for every ID generated on that process.
-
-        :return: An integer denoting the increment.
-        """
-        return int(self._snowflake) & 0xFFF
-
-    @property
-    def worker_id(self) -> int:
-        """
-        This is the Internal Worker ID of the snowflake.
-
-        :return: An integer denoting the internal worker ID.
-        """
-        return (int(self._snowflake) & 0x3E0000) >> 17
-
-    @property
-    def process_id(self) -> int:
-        """
-        This is the Internal Process ID of the snowflake.
-
-        :return: An integer denoting the internal process ID.
-        """
-        return (int(self._snowflake) & 0x1F000) >> 12
-
-    @property
-    def epoch(self) -> float:
-        """
-        This is the Timestamp field of the snowflake.
-
-        :return: A float containing the seconds since Discord Epoch.
-        """
-        return floor(((int(self._snowflake) >> 22) + 1420070400000) / 1000)
-
-    @property
-    def timestamp(self) -> datetime.datetime:
-        """
-        The Datetime object variation of the Timestamp field of the snowflake.
-
-        :return: The converted Datetime object from the Epoch. This respects UTC.
-        """
-        return datetime.datetime.utcfromtimestamp(self.epoch)
-
-    # ---- Extra stuff that might be helpful.
-
-    def __hash__(self) -> int:
-        return hash(self._snowflake)
-
-    def __eq__(self, other) -> bool:
-        if isinstance(other, Snowflake):
-            return str(self) == str(other)
-        elif isinstance(other, int):
-            return int(self) == other
-        elif isinstance(other, str):
-            return str(self) == other
-
-        return NotImplemented
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self._snowflake})"
-
-
-class IDMixin:
-    """
-    .. versionadded:: 4.3.0
-
-    A mixin to implement equality and hashing for models that have an id.
-    """
-
-    id: Snowflake
-
-    def __eq__(self, other) -> bool:
-        return (
-            self.id is not None
-            and isinstance(
-                other, IDMixin
-            )  # different classes can't share ids, covers cases like Member/User
-            and self.id == other.id
-        )
-
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-
-@define()
-class AutoModMetaData(DictSerializerMixin):
-    """
-    .. versionadded:: 4.3.0
-
-    A class object used to represent the AutoMod Action Metadata.
-
-    .. note::
-        This is not meant to be instantiated outside the Gateway.
-
-    .. note::
-        The maximum duration for duration_seconds is 2419200 seconds, aka 4 weeks.
-
-    :ivar Optional[Snowflake] channel_id: Channel to which user content should be logged, if set.
-    :ivar Optional[int] duration_seconds: Timeout duration in seconds, if timed out.
-    """
-
-    channel_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    duration_seconds: Optional[int] = field(default=None)
-
-
-class AutoModTriggerType(IntEnum):
-    """
-    .. versionadded:: 4.3.0
-
-    An enumeration for the different AutoMod trigger types.
-    """
-
-    KEYWORD = 1
-    HARMFUL_LINK = 2
-    SPAM = 3
-    KEYWORD_PRESET = 4
-    MENTION_SPAM = 5
-
-
-class AutoModKeywordPresetTypes(IntEnum):
-    """
-    .. versionadded:: 4.3.0
-
-    An enumeration for the different AutoMod keyword preset types.
-    """
-
-    PROFANITY = 1
-    SEXUAL_CONTENT = 2
-    SLURS = 3
-
-
-class AutoModActionTypes(IntEnum):
-    """
-    .. versionadded:: 4.3.0
-
-    An enumeration for the different AutoMod action types.
-    """
-
-    BLOCK_MESSAGE = 1
-    SEND_ALERT_MESSAGE = 2
-    TIMEOUT = 3
-
-
-@define()
-class AutoModAction(DictSerializerMixin):
-    """
-    .. versionadded:: 4.3.0
-
-    A class object used for the ``AUTO_MODERATION_ACTION_EXECUTION`` event.
-
-    .. note::
-        This is not to be confused with the GW event ``AUTO_MODERATION_ACTION_EXECUTION``.
-        This object is not the same as that dispatched object. Moreover, that dispatched object name will be
-        ``AutoModerationAction``
-
-    .. note::
-        The metadata can be omitted depending on the action type.
-
-    :ivar AutoModActionTypes type: Action type.
-    :ivar AutoModMetaData metadata: Additional metadata needed during execution for this specific action type.
-    """
-
-    type: AutoModActionTypes = field(converter=AutoModActionTypes)
-    metadata: Optional[AutoModMetaData] = field(converter=AutoModMetaData, default=None)
-
-
-@define()
-class AutoModTriggerMetadata(DictSerializerMixin):
-    """
-    .. versionadded:: 4.3.0
-
-    A class object used to represent the trigger metadata from the AutoMod rule object.
-
-    :ivar Optional[List[str]] keyword_filter: Words to match against content.
-    :ivar Optional[List[str]] regex_patterns: Regular expression patterns to match against content.
-    :ivar Optional[List[AutoModKeywordPresetTypes]] presets: The internally pre-defined wordsets which will be searched for in content.
-    :ivar Optional[List[str]] allow_list: Substrings which will be exempt from triggering the preset trigger type.
-    :ivar Optional[int] mention_total_limit: Total number of unique role and user mentions allowed per message (Maximum of 50)
-    """
-
-    keyword_filter: Optional[List[str]] = field(default=None)
-    regex_patterns: Optional[List[str]] = field(default=None)
-    presets: Optional[List[AutoModKeywordPresetTypes]] = field(
-        converter=convert_list(AutoModKeywordPresetTypes), default=None
+import re
+from enum import IntEnum
+from typing import Optional, TYPE_CHECKING, Union, Dict, Any, List
+
+import attrs
+
+from interactions.client.const import MISSING, Absent
+from interactions.client.errors import ForeignWebhookException, EmptyMessageException
+from interactions.client.mixins.send import SendMixin
+from interactions.client.utils.serializer import to_image_data
+from interactions.models.discord.message import process_message_payload
+from interactions.models.discord.snowflake import to_snowflake, to_optional_snowflake
+from .base import DiscordObject
+
+if TYPE_CHECKING:
+    from interactions.models.discord.file import UPLOADABLE_TYPE
+    from interactions.client import Client
+    from interactions.models.discord.enums import MessageFlags
+    from interactions.models.discord.snowflake import Snowflake_Type
+    from interactions.models.discord.channel import TYPE_MESSAGEABLE_CHANNEL
+    from interactions.models.discord.components import BaseComponent
+    from interactions.models.discord.embed import Embed
+
+    from interactions.models.discord.message import (
+        AllowedMentions,
+        Message,
+        MessageReference,
     )
-    allow_list: Optional[List[str]] = field(default=None)
-    mention_total_limit: Optional[int] = field(default=None)
-
-
-class Color(IntEnum):
-    """
-    .. versionadded:: 4.2.0
+    from interactions.models.discord.sticker import Sticker
 
-    .. versionchanged:: 4.4.0
-        Color class is now an Enum
+__all__ = ("WebhookTypes", "Webhook")
 
-    An object representing Discord branding colors.
 
-    .. note::
-        This object only intends to cover the branding colors
-        and no others. The main reason behind this is due to
-        the current accepted standard of using hex codes or other
-        custom-defined colors.
-    """
+class WebhookTypes(IntEnum):
+    INCOMING = 1
+    """Incoming Webhooks can post messages to channels with a generated token"""
+    CHANNEL_FOLLOWER = 2
+    """Channel Follower Webhooks are internal webhooks used with Channel Following to post new messages into channels"""
+    APPLICATION = 3
+    """Application webhooks are webhooks used with Interactions"""
 
-    BLURPLE = 0x5865F2
-    GREEN = 0x57F287
-    YELLOW = 0xFEE75C
-    FUCHSIA = 0xEB459E
-    RED = 0xED4245
-    WHITE = 0xFFFFFF
-    BLACK = 0x000000
 
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class Webhook(DiscordObject, SendMixin):
+    type: WebhookTypes = attrs.field(
+        repr=False,
+    )
+    """The type of webhook"""
 
-class File:
-    """
-    .. versionadded:: 4.2.0
+    application_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the bot/OAuth2 application that created this webhook"""
 
-    A File object to be sent as an attachment along with a message.
+    guild_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the guild id this webhook is for, if any"""
+    channel_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the channel id this webhook is for, if any"""
+    user_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the user this webhook was created by"""
 
-    If a fp is not given, this will try to open & send a local file at the location
-    specified in the 'filename' parameter.
+    name: Optional[str] = attrs.field(repr=False, default=None)
+    """the default name of the webhook"""
+    avatar: Optional[str] = attrs.field(repr=False, default=None)
+    """the default user avatar hash of the webhook"""
+    token: str = attrs.field(repr=False, default=MISSING)
+    """the secure token of the webhook (returned for Incoming Webhooks)"""
+    url: Optional[str] = attrs.field(repr=False, default=None)
+    """the url used for executing the webhook (returned by the webhooks OAuth2 flow)"""
 
-    .. note::
-        If a description is not given the file's basename is used instead.
-    """
+    source_guild_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the guild of the channel that this webhook is following (returned for Channel Follower Webhooks)"""
+    source_channel_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None)
+    """the channel that this webhook is following (returned for Channel Follower Webhooks)"""
 
-    def __init__(
-        self, filename: str, fp: Optional[IOBase] = MISSING, description: Optional[str] = MISSING
-    ):
-        if not isinstance(filename, str):
-            raise LibraryException(
-                message=f"File's first parameter 'filename' must be a string, not {str(type(filename))}",
-                code=12,
-            )
+    @classmethod
+    def from_url(cls, url: str, client: "Client") -> "Webhook":
+        """
+        Webhook object from a URL.
 
-        self._fp = open(filename, "rb") if not fp or fp is MISSING else fp
-        self._filename = basename(filename)
+        Args:
+            client: The client to use to make the request.
+            url: Webhook URL
 
-        if not description or description is MISSING:
-            self._description = self._filename
-        else:
-            self._description = description
+        Returns:
+            A Webhook object.
 
-    def _json_payload(self, id: int) -> dict:
-        return {"id": id, "description": self._description, "filename": self._filename}
+        """
+        match = re.search(r"discord(?:app)?\.com/api/webhooks/(?P<id>[0-9]{17,})/(?P<token>[\w\-.]{60,68})", url)
+        if match is None:
+            raise ValueError("Invalid webhook URL given.")
 
+        data: Dict[str, Any] = match.groupdict()
+        data["type"] = WebhookTypes.INCOMING
+        return cls.from_dict(data, client)
 
-class Image:
-    """
-    .. versionadded:: 4.2.0
+    @classmethod
+    async def create(
+        cls,
+        client: "Client",
+        channel: Union["Snowflake_Type", "TYPE_MESSAGEABLE_CHANNEL"],
+        name: str,
+        avatar: Absent["UPLOADABLE_TYPE"] = MISSING,
+    ) -> "Webhook":
+        """
+        Create a webhook.
 
-    This class object allows you to upload Images to the Discord API.
+        Args:
+            client: The bot's client
+            channel: The channel to create the webhook in
+            name: The name of the webhook
+            avatar: An optional default avatar to use
 
-    If a fp is not given, this will try to open & send a local file at the location
-    specified in the 'file' parameter.
-    """
+        Returns:
+            New webhook object
 
-    def __init__(self, file: Union[str, FileIO], fp: Optional[IOBase] = MISSING):
-        self._URI = "data:image/"
+        Raises:
+            ValueError: If you try to name the webhook "Clyde"
 
-        if fp is MISSING or isinstance(file, FileIO):
-            file: FileIO = file if isinstance(file, FileIO) else FileIO(file)  # noqa
+        """
+        if name.lower() == "clyde":
+            raise ValueError('Webhook names cannot be "Clyde"')
 
-            self._name = file.name
-            _file = file.read()
+        if not isinstance(channel, (str, int)):
+            channel = to_snowflake(channel)
 
-        else:
-            self._name = file
-            _file = fp
+        if avatar:
+            avatar = to_image_data(avatar)
 
-        if (
-            not self._name.endswith(".jpeg")
-            and not self._name.endswith(".png")
-            and not self._name.endswith(".gif")
-        ):
-            raise LibraryException(message="File type must be jpeg, png or gif!", code=12)
+        data = await client.http.create_webhook(channel, name, avatar)
 
-        self._URI += f"{'jpeg' if self._name.endswith('jpeg') else self._name[-3:]};"
-        self._URI += f"base64,{b64encode(_file).decode('utf-8')}"
+        return cls.from_dict(data, client)
 
-    @property
-    def data(self) -> str:
-        return self._URI
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if data.get("user"):
+            user = client.cache.place_user_data(data.pop("user"))
+            data["user_id"] = user.id
+        return data
 
-    @property
-    def filename(self) -> str:
+    async def edit(
+        self,
+        *,
+        name: Absent[str] = MISSING,
+        avatar: Absent["UPLOADABLE_TYPE"] = MISSING,
+        channel_id: Absent["Snowflake_Type"] = MISSING,
+    ) -> None:
         """
-        Returns the name of the file.
-        """
-        return self._name.split("/")[-1].split(".")[0]
-
-
-class AllowedMentionType(StrEnum):
-    """
-    .. versionadded:: 4.3.2
+        Edit this webhook.
 
-    An enumerable object representing the allowed mention types
-    """
+        Args:
+            name: The default name of the webhook.
+            avatar: The image for the default webhook avatar.
+            channel_id: The new channel id this webhook should be moved to.
 
-    EVERYONE = "everyone"
-    USERS = "users"
-    ROLES = "roles"
+        Raises:
+            ValueError: If you try to name the webhook "Clyde"
 
+        """
+        if name.lower() == "clyde":
+            raise ValueError('Webhook names cannot be "Clyde"')
 
-@define()
-class AllowedMentions(DictSerializerMixin):
-    """
-    .. versionadded:: 4.3.2
+        data = await self._client.http.modify_webhook(
+            self.id, name, to_image_data(avatar), to_optional_snowflake(channel_id), self.token
+        )
+        self.update_from_dict(data)
 
-    A class object representing the allowed mentions object
+    async def delete(self) -> None:
+        """Delete this webhook."""
+        await self._client.http.delete_webhook(self.id, self.token)
+
+    async def send(
+        self,
+        content: Optional[str] = None,
+        *,
+        embed: Optional[Union["Embed", dict]] = None,
+        embeds: Optional[Union[List[Union["Embed", dict]], Union["Embed", dict]]] = None,
+        components: Optional[
+            Union[
+                List[List[Union["BaseComponent", dict]]],
+                List[Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        stickers: Optional[Union[List[Union["Sticker", "Snowflake_Type"]], "Sticker", "Snowflake_Type"]] = None,
+        allowed_mentions: Optional[Union["AllowedMentions", dict]] = None,
+        reply_to: Optional[Union["MessageReference", "Message", dict, "Snowflake_Type"]] = None,
+        files: Optional[Union["UPLOADABLE_TYPE", List["UPLOADABLE_TYPE"]]] = None,
+        file: Optional["UPLOADABLE_TYPE"] = None,
+        tts: bool = False,
+        suppress_embeds: bool = False,
+        flags: Optional[Union[int, "MessageFlags"]] = None,
+        username: str = None,
+        avatar_url: str = None,
+        wait: bool = False,
+        thread: "Snowflake_Type" = None,
+        **kwargs,
+    ) -> Optional["Message"]:
+        """
+        Send a message as this webhook.
+
+        Args:
+            content: Message text content.
+            embeds: Embedded rich content (up to 6000 characters).
+            embed: Embedded rich content (up to 6000 characters).
+            components: The components to include with the message.
+            stickers: IDs of up to 3 stickers in the server to send in the message.
+            allowed_mentions: Allowed mentions for the message.
+            reply_to: Message to reference, must be from the same channel.
+            files: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            file: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            tts: Should this message use Text To Speech.
+            suppress_embeds: Should embeds be suppressed on this send
+            flags: Message flags to apply.
+            username: The username to use
+            avatar_url: The url of an image to use as the avatar
+            wait: Waits for confirmation of delivery. Set this to True if you intend to edit the message
+            thread: Send this webhook to a thread channel
+
+        Returns:
+            New message object that was sent if `wait` is set to True
+
+        """
+        if not self.token:
+            raise ForeignWebhookException("You cannot send messages with a webhook without a token!")
+
+        if not content and not embeds and not embed and not files and not file and not stickers:
+            raise EmptyMessageException("You cannot send a message without any content, embeds, files, or stickers")
+
+        if suppress_embeds:
+            if isinstance(flags, int):
+                flags = MessageFlags(flags)
+            flags = flags | MessageFlags.SUPPRESS_EMBEDS
+
+        message_payload = process_message_payload(
+            content=content,
+            embeds=embeds or embed,
+            components=components,
+            stickers=stickers,
+            allowed_mentions=allowed_mentions,
+            reply_to=reply_to,
+            tts=tts,
+            flags=flags,
+            username=username,
+            avatar_url=avatar_url,
+            **kwargs,
+        )
 
-    :ivar Optional[List[AllowedMentionType]] parse: An array of allowed mention types to parse from the content.
-    :ivar Optional[List[int]] users: An array of user ids to mention.
-    :ivar Optional[List[int]] roles: An array of role ids to mention.
-    :ivar Optional[bool] replied_user: For replies, whether to mention the author of the message being replied to.
-    """
+        message_data = await self._client.http.execute_webhook(
+            self.id,
+            self.token,
+            message_payload,
+            wait,
+            to_optional_snowflake(thread),
+            files=files or file,
+        )
+        if message_data:
+            return self._client.cache.place_message_data(message_data)
 
-    parse: Optional[List[AllowedMentionType]] = field(
-        converter=convert_list(AllowedMentionType), default=None
-    )
-    users: Optional[List[int]] = field(default=None)
-    roles: Optional[List[int]] = field(default=None)
-    replied_user: Optional[bool] = field(default=None)
+    async def edit_message(
+        self,
+        message: Union["Message", "Snowflake_Type"],
+        *,
+        content: Optional[str] = None,
+        embeds: Optional[Union[List[Union["Embed", dict]], Union["Embed", dict]]] = None,
+        components: Optional[
+            Union[
+                List[List[Union["BaseComponent", dict]]],
+                List[Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        stickers: Optional[Union[List[Union["Sticker", "Snowflake_Type"]], "Sticker", "Snowflake_Type"]] = None,
+        allowed_mentions: Optional[Union["AllowedMentions", dict]] = None,
+        reply_to: Optional[Union["MessageReference", "Message", dict, "Snowflake_Type"]] = None,
+        files: Optional[Union["UPLOADABLE_TYPE", List["UPLOADABLE_TYPE"]]] = None,
+        file: Optional["UPLOADABLE_TYPE"] = None,
+        tts: bool = False,
+        flags: Optional[Union[int, "MessageFlags"]] = None,
+    ) -> Optional["Message"]:
+        """
+        Edit a message as this webhook.
+
+        Args:
+            message: Message to edit
+            content: Message text content.
+            embeds: Embedded rich content (up to 6000 characters).
+            components: The components to include with the message.
+            stickers: IDs of up to 3 stickers in the server to send in the message.
+            allowed_mentions: Allowed mentions for the message.
+            reply_to: Message to reference, must be from the same channel.
+            files: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            file: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            tts: Should this message use Text To Speech.
+            flags: Message flags to apply.
+
+        Returns:
+            Updated message object that was sent if `wait` is set to True
+
+        """
+        message_payload = process_message_payload(
+            content=content,
+            embeds=embeds,
+            components=components,
+            stickers=stickers,
+            allowed_mentions=allowed_mentions,
+            reply_to=reply_to,
+            tts=tts,
+            flags=flags,
+        )
+        msg_data = await self._client.http.edit_webhook_message(
+            self.id, self.token, to_snowflake(message), message_payload, files=files or file
+        )
+        if msg_data:
+            return self._client.cache.place_message_data(msg_data)
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/role.py` & `discord-py-interactions-5.0.0/interactions/models/discord/role.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,234 @@
-from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union
+from functools import partial, total_ordering
+from typing import Any, TYPE_CHECKING
 
-from ...utils.attrs_utils import (
-    ClientSerializerMixin,
-    DictSerializerMixin,
-    convert_int,
-    define,
-    field,
-)
-from ...utils.missing import MISSING
-from ..error import LibraryException
-from .flags import Permissions
-from .misc import IDMixin, Image, Snowflake
+import attrs
+
+from interactions.client.const import MISSING, T, Missing
+from interactions.client.utils import nulled_boolean_get
+from interactions.client.utils.attr_converters import optional as optional_c
+from interactions.client.utils.serializer import dict_filter
+from interactions.models.discord.asset import Asset
+from interactions.models.discord.color import COLOR_TYPES, Color, process_color
+from interactions.models.discord.emoji import PartialEmoji
+from interactions.models.discord.enums import Permissions
+from .base import DiscordObject
 
 if TYPE_CHECKING:
-    from .guild import Guild
+    from interactions.client import Client
+    from interactions.models.discord.guild import Guild
+    from interactions.models.discord.user import Member
+    from interactions.models.discord.snowflake import Snowflake_Type
 
-__all__ = (
-    "Role",
-    "RoleTags",
-)
-
-
-@define()
-class RoleTags(DictSerializerMixin):
-    """
-    A class object representing the tags of a role.
-
-    .. note ::
-        With the premium_subscriber and available_for_purchase attributes currently,
-        if the attribute is present and "null" it's true, and if the attribute is not present it's false.
-
-
-    :ivar Optional[Snowflake] bot_id: The id of the bot this role belongs to
-    :ivar Optional[Snowflake] integration_id: The id of the integration this role belongs to
-    :ivar Optional[bool] premium_subscriber: Whether if this is the guild's booster role.
-    :ivar Optional[Snowflake] subscription_listing_id: The id of this role's subscription sku and listing, if any.
-    :ivar Optional[bool] available_for_purchase: Whether this role is available for purchase.
-    """
-
-    bot_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    integration_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    premium_subscriber: Optional[bool] = field(default=None)
-
-    subscription_listing_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    purchasable_or_has_subscribers: Optional[bool] = field(default=None)
-
-
-@define()
-class Role(ClientSerializerMixin, IDMixin):
-    """
-    A class object representing a role.
-
-    :ivar Snowflake id: Role ID
-    :ivar str name: Role name
-    :ivar int color: Role color in integer representation
-    :ivar bool hoist: A status denoting if this role is hoisted
-    :ivar Optional[str] icon: Role icon hash, if any.
-    :ivar Optional[str] unicode_emoji: Role unicode emoji
-    :ivar int position: Role position
-    :ivar Permissions permissions: Role permissions as a bit set
-    :ivar bool managed: A status denoting if this role is managed by an integration
-    :ivar bool mentionable: A status denoting if this role is mentionable
-    :ivar Optional[RoleTags] tags: The tags this role has
-    """
-
-    id: Snowflake = field(converter=Snowflake)
-    name: str = field()
-    color: int = field()
-    hoist: bool = field()
-    icon: Optional[str] = field(default=None, repr=False)
-    unicode_emoji: Optional[str] = field(default=None)
-    position: int = field()
-    permissions: Permissions = field(converter=convert_int(Permissions))
-    managed: bool = field()
-    mentionable: bool = field()
-    tags: Optional[RoleTags] = field(converter=RoleTags, default=None)
+__all__ = ("Role",)
 
-    @property
-    def mention(self) -> str:
+
+def sentinel_converter(value: bool | T | None, sentinel: T = attrs.NOTHING) -> bool | T:
+    if value is sentinel:
+        return False
+    return True if value is None else value
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+@total_ordering
+class Role(DiscordObject):
+    _sentinel = object()
+
+    name: str = attrs.field(repr=True)
+    color: "Color" = attrs.field(repr=False, converter=Color)
+    hoist: bool = attrs.field(repr=False, default=False)
+    position: int = attrs.field(repr=True)
+    permissions: "Permissions" = attrs.field(repr=False, converter=Permissions)
+    managed: bool = attrs.field(repr=False, default=False)
+    mentionable: bool = attrs.field(repr=False, default=True)
+    premium_subscriber: bool = attrs.field(
+        repr=False, default=_sentinel, converter=partial(sentinel_converter, sentinel=_sentinel)
+    )
+    subscription_listing_id: "Snowflake_Type | None" = attrs.field(default=None, repr=False)
+    purchasable_or_has_subscribers: bool = attrs.field(default=False)
+    _icon: Asset | None = attrs.field(repr=False, default=None)
+    _unicode_emoji: PartialEmoji | None = attrs.field(
+        repr=False, default=None, converter=optional_c(PartialEmoji.from_str)
+    )
+    _guild_id: "Snowflake_Type" = attrs.field(
+        repr=False,
+    )
+    _bot_id: "Snowflake_Type | None" = attrs.field(repr=False, default=None)
+    _integration_id: "Snowflake_Type | None" = attrs.field(repr=False, default=None)  # todo integration object?
+    _guild_connections: bool = attrs.field(repr=False, default=False)
+
+    def __lt__(self: "Role", other: "Role") -> bool:
+        if not isinstance(self, Role) or not isinstance(other, Role):
+            return NotImplemented
+
+        if self._guild_id != other._guild_id:
+            raise RuntimeError("Unable to compare Roles from different guilds.")
+
+        if self.id == self._guild_id:  # everyone role
+            # everyone role is on the bottom, so check if the other role is, well, not it
+            # because then it must be higher than it
+            return other.id != self.id
+
+        if self.position < other.position:
+            return True
+
+        return self.id < other.id if self.position == other.position else False
+
+    @classmethod
+    def _process_dict(cls, data: dict[str, Any], client: "Client") -> dict[str, Any]:
+        data |= data.pop("tags", {})
+
+        if icon_hash := data.get("icon"):
+            data["icon"] = Asset.from_path_hash(client, f"role-icons/{data['id']}/{{}}", icon_hash)
+
+        data["premium_subscriber"] = nulled_boolean_get(data, "premium_subscriber")
+        data["guild_connections"] = nulled_boolean_get(data, "guild_connections")
+        data["available_for_purchase"] = nulled_boolean_get(data, "available_for_purchase")
+
+        return data
+
+    async def fetch_bot(self) -> "Member | None":
         """
-        .. versionadded:: 4.1.0
+        Fetch the bot associated with this role if any.
 
-        Returns a string that allows you to mention the given role.
+        Returns:
+            Member object if any
 
-        :return: The string of the mentioned role.
-        :rtype: str
         """
-        return f"<@&{self.id}>"
+        if self._bot_id is None:
+            return None
+        return await self._client.cache.fetch_member(self._guild_id, self._bot_id)
+
+    def get_bot(self) -> "Member | None":
+        """
+        Get the bot associated with this role if any.
+
+        Returns:
+            Member object if any
+
+        """
+        if self._bot_id is None:
+            return None
+        return self._client.cache.get_member(self._guild_id, self._bot_id)
+
+    @property
+    def guild(self) -> "Guild":
+        """The guild object this role is from."""
+        return self._client.cache.get_guild(self._guild_id)  # pyright: ignore [reportGeneralTypeIssues]
+
+    @property
+    def default(self) -> bool:
+        """Is this the `@everyone` role."""
+        return self.id == self._guild_id
 
     @property
-    def created_at(self) -> datetime:
+    def bot_managed(self) -> bool:
+        """Is this role owned/managed by a bot."""
+        return self._bot_id is not None
+
+    @property
+    def is_linked_role(self) -> bool:
+        """Is this role a linked role."""
+        return self._guild_connections
+
+    @property
+    def mention(self) -> str:
+        """Returns a string that would mention the role."""
+        return f"<@&{self.id}>" if self.id != self._guild_id else "@everyone"
+
+    @property
+    def integration(self) -> bool:
+        """Is this role owned/managed by an integration."""
+        return self._integration_id is not None
+
+    @property
+    def members(self) -> list["Member"]:
+        """List of members with this role"""
+        return [member for member in self.guild.members if member.has_role(self)]
+
+    @property
+    def icon(self) -> Asset | PartialEmoji | None:
         """
-        .. versionadded:: 4.4.0
+        The icon of this role
 
-        Returns when the role was created.
+        !!! note
+            You have to use this method instead of the `_icon` attribute, because the first does account for unicode emojis
         """
-        return self.id.timestamp
+        return self._icon or self._unicode_emoji
 
-    async def delete(
-        self,
-        guild_id: Union[int, Snowflake, "Guild"],
-        reason: Optional[str] = None,
-    ) -> None:
+    @property
+    def is_assignable(self) -> bool:
         """
-        .. versionadded:: 4.0.2
+        Can this role be assigned or removed by this bot?
 
-        Deletes the role from the guild.
+        !!! note
+            This does not account for permissions, only the role hierarchy
 
-        :param int guild_id: The id of the guild to delete the role from
-        :param Optional[str] reason: The reason for the deletion
         """
-        if not self._client:
-            raise LibraryException(code=13)
+        return (self.default or self.guild.me.top_role > self) and not self.managed
 
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
+    async def delete(self, reason: str | Missing = MISSING) -> None:
+        """
+        Delete this role.
 
-        await self._client.delete_guild_role(
-            guild_id=_guild_id, role_id=int(self.id), reason=reason
-        )
+        Args:
+            reason: An optional reason for this deletion
+
+        """
+        await self._client.http.delete_guild_role(self._guild_id, self.id, reason)
 
-    async def modify(
+    async def edit(
         self,
-        guild_id: Union[int, Snowflake, "Guild"],
-        name: Optional[str] = MISSING,
-        permissions: Optional[Union[Permissions, int]] = MISSING,
-        color: Optional[int] = MISSING,
-        hoist: Optional[bool] = MISSING,
-        icon: Optional[Image] = MISSING,
-        unicode_emoji: Optional[str] = MISSING,
-        mentionable: Optional[bool] = MISSING,
-        reason: Optional[str] = None,
+        *,
+        name: str | None = None,
+        permissions: str | None = None,
+        color: Color | COLOR_TYPES | None = None,
+        hoist: bool | None = None,
+        mentionable: bool | None = None,
     ) -> "Role":
         """
-        .. versionadded:: 4.0.2
-
-        Edits the role in a guild.
+        Edit this role, all arguments are optional.
 
-        :param int guild_id: The id of the guild to edit the role on
-        :param Optional[str] name: The name of the role, defaults to the current value of the role
-        :param Optional[int] color: RGB color value as integer, defaults to the current value of the role
-        :param Optional[Union[Permissions, int]] permissions: Bitwise value of the enabled/disabled permissions, defaults to the current value of the role
-        :param Optional[bool] hoist: Whether the role should be displayed separately in the sidebar, defaults to the current value of the role
-        :param Optional[Image] icon: The role's icon image (if the guild has the ROLE_ICONS feature), defaults to the current value of the role
-        :param Optional[str] unicode_emoji: The role's unicode emoji as a standard emoji (if the guild has the ROLE_ICONS feature), defaults to the current value of the role
-        :param Optional[bool] mentionable: Whether the role should be mentionable, defaults to the current value of the role
-        :param Optional[str] reason: The reason why the role is edited, default ``None``
-        :return: The modified role object
-        :rtype: Role
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-        _name = self.name if name is MISSING else name
-        _color = self.color if color is MISSING else color
-        _hoist = self.hoist if hoist is MISSING else hoist
-        _mentionable = self.mentionable if mentionable is MISSING else mentionable
-        _permissions = int(self.permissions if permissions is MISSING else permissions)
-        _icon = self.icon if icon is MISSING else icon
-        _unicode_emoji = self.unicode_emoji if unicode_emoji is MISSING else unicode_emoji
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
-
-        payload = dict(
-            name=_name,
-            color=_color,
-            hoist=_hoist,
-            mentionable=_mentionable,
-            permissions=_permissions,
-            icon=_icon,
-            unicode_emoji=_unicode_emoji,
+        Args:
+            name: name of the role
+            permissions: New permissions to use
+            color: The color of the role
+            hoist: whether the role should be displayed separately in the sidebar
+            mentionable: whether the role should be mentionable
+
+        Returns:
+            Role with updated information
+
+        """
+        color = process_color(color)
+
+        payload = dict_filter(
+            {
+                "name": name,
+                "permissions": permissions,
+                "color": color,
+                "hoist": hoist,
+                "mentionable": mentionable,
+            }
         )
 
-        res = await self._client.modify_guild_role(
-            guild_id=_guild_id,
-            role_id=int(self.id),
-            payload=payload,
-            reason=reason,
-        )
+        r_data = await self._client.http.modify_guild_role(self._guild_id, self.id, payload)
+        r_data = dict(r_data)  # to convert typed dict to regular dict
+        r_data["guild_id"] = self._guild_id
+        return self.from_dict(r_data, self._client)
 
-        self.update(res)
+    async def move(self, position: int, reason: str | Missing = MISSING) -> "Role":
+        """
+        Move this role to a new position.
 
-        return self
+        Args:
+            position: The new position of the role
+            reason: An optional reason for this move
 
-    async def modify_position(
-        self,
-        guild_id: Union[int, Snowflake, "Guild"],
-        position: int,
-        reason: Optional[str] = None,
-    ) -> List["Role"]:
-        """
-        .. versionadded:: 4.0.2
-
-        Modifies the position of a role in the guild.
-
-        :param int guild_id: The id of the guild to modify the role position on
-        :param int position: The new position of the role
-        :param Optional[str] reason: The reason for the modifying
-        :return: List of guild roles with updated hierarchy
-        :rtype: List[Role]
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-
-        _guild_id = int(guild_id) if isinstance(guild_id, (int, Snowflake)) else int(guild_id.id)
-
-        res = await self._client.modify_guild_role_positions(
-            guild_id=_guild_id,
-            payload=[{"position": position, "id": int(self.id)}],
-            reason=reason,
+        Returns:
+            The role object
+
+        """
+        await self._client.http.modify_guild_role_positions(
+            self._guild_id, [{"id": self.id, "position": position}], reason
         )
-        return [Role(**role, _client=self._client) for role in res]
+        return self
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/user.py` & `discord-py-interactions-5.0.0/interactions/models/discord/emoji.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,239 +1,259 @@
-from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union
-
-from ...utils.attrs_utils import ClientSerializerMixin, define, field
-from ...utils.missing import MISSING
-from ..error import LibraryException
-from .flags import UserFlags
-from .misc import AllowedMentions, File, IDMixin, Snowflake
+import re
+import string
+import unicodedata
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+
+import attrs
+import emoji
+
+from interactions.client.mixins.serialization import DictSerializationMixin
+from interactions.client.utils.attr_converters import list_converter
+from interactions.client.utils.attr_converters import optional
+from interactions.client.utils.serializer import dict_filter_none, no_export_meta
+from interactions.models.discord.base import ClientObject
+from interactions.models.discord.snowflake import SnowflakeObject, to_snowflake
 
 if TYPE_CHECKING:
-    from ...client.models.component import ActionRow, Button, SelectMenu
-    from .channel import Channel
-    from .gw import Presence
-    from .message import Attachment, Embed, Message
+    from interactions.client import Client
+    from interactions.models.discord.guild import Guild
+    from interactions.models.discord.user import User, Member
+    from interactions.models.discord.role import Role
+    from interactions.models.discord.snowflake import Snowflake_Type
+
+__all__ = ("PartialEmoji", "CustomEmoji", "process_emoji_req_format", "process_emoji")
+
+emoji_regex = re.compile(r"<?(a)?:(\w*):(\d*)>?")
+unicode_emoji_reg = re.compile(r"[^\w\s,’‘“”…–—•◦‣⁃⁎⁏⁒⁓⁺⁻⁼⁽⁾ⁿ₊₋₌₍₎]")  # noqa: RUF001
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class PartialEmoji(SnowflakeObject, DictSerializationMixin):
+    """Represent a basic ("partial") emoji used in discord."""
+
+    id: Optional["Snowflake_Type"] = attrs.field(
+        repr=True, default=None, converter=optional(to_snowflake)
+    )  # can be None for Standard Emoji
+    """The custom emoji id. Leave empty if you are using standard unicode emoji."""
+    name: Optional[str] = attrs.field(repr=True, default=None)
+    """The custom emoji name, or standard unicode emoji in string"""
+    animated: bool = attrs.field(repr=True, default=False)
+    """Whether this emoji is animated"""
+
+    @classmethod
+    def from_str(cls, emoji_str: str, *, language: str = "alias") -> Optional["PartialEmoji"]:
+        """
+        Generate a PartialEmoji from a discord Emoji string representation, or unicode emoji.
+
+        Handles:
+            <:emoji_name:emoji_id>
+            :emoji_name:emoji_id
+            <a:emoji_name:emoji_id>
+            a:emoji_name:emoji_id
+            👋
+            :wave:
+
+        Args:
+            emoji_str: The string representation an emoji
+            language: The language to use for the unicode emoji parsing
+
+        Returns:
+            A PartialEmoji object
+
+        Raises:
+            ValueError: if the string cannot be parsed
+
+        """
+        if parsed := emoji_regex.findall(emoji_str):
+            parsed = tuple(filter(None, parsed[0]))
+            if len(parsed) == 3:
+                return cls(name=parsed[1], id=parsed[2], animated=True)
+            if len(parsed) == 2:
+                return cls(name=parsed[0], id=parsed[1])
+            _name = emoji.emojize(emoji_str, language=language)
+            if _emoji_list := emoji.distinct_emoji_list(_name):
+                return cls(name=_emoji_list[0])
+        else:
+            if _emoji_list := emoji.distinct_emoji_list(emoji_str):
+                return cls(name=_emoji_list[0])
 
-__all__ = ("User",)
+            # the emoji lib handles *most* emoji, however there are certain ones that it misses
+            # this acts as a fallback check
+            if matches := unicode_emoji_reg.search(emoji_str):
+                match = matches.group()
+
+                # the regex will match certain special characters, so this acts as a final failsafe
+                if match not in string.printable and unicodedata.category(match) == "So":
+                    return cls(name=match)
+        return None
+
+    def __str__(self) -> str:
+        s = self.req_format
+        if self.id:
+            s = f"<{'a:' if self.animated else ':'}{s}>"
+        return s
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, PartialEmoji):
+            return False
+        return self.id == other.id if self.id else self.name == other.name
 
-@define()
-class User(ClientSerializerMixin, IDMixin):
-    """
-    A class object representing a user.
+    @property
+    def req_format(self) -> str:
+        """Format used for web request."""
+        return f"{self.name}:{self.id}" if self.id else self.name
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class CustomEmoji(PartialEmoji, ClientObject):
+    """Represent a custom emoji in a guild with all its properties."""
+
+    _client: "Client" = attrs.field(repr=False, metadata=no_export_meta)
+
+    require_colons: bool = attrs.field(repr=False, default=False)
+    """Whether this emoji must be wrapped in colons"""
+    managed: bool = attrs.field(repr=False, default=False)
+    """Whether this emoji is managed"""
+    available: bool = attrs.field(repr=False, default=False)
+    """Whether this emoji can be used, may be false due to loss of Server Boosts."""
+
+    _creator_id: Optional["Snowflake_Type"] = attrs.field(repr=False, default=None, converter=optional(to_snowflake))
+    _role_ids: List["Snowflake_Type"] = attrs.field(
+        repr=False, factory=list, converter=optional(list_converter(to_snowflake))
+    )
+    _guild_id: "Snowflake_Type" = attrs.field(repr=False, default=None, converter=to_snowflake)
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        creator_dict = data.pop("user", None)
+        data["creator_id"] = client.cache.place_user_data(creator_dict).id if creator_dict else None
+
+        if "roles" in data:
+            data["role_ids"] = data.pop("roles")
+
+        return data
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any], client: "Client", guild_id: int) -> "CustomEmoji":
+        data = cls._process_dict(data, client)
+        return cls(client=client, guild_id=guild_id, **cls._filter_kwargs(data, cls._get_init_keys()))
 
-    :ivar Snowflake id: The User ID
-    :ivar str username: The Username associated (not necessarily unique across the platform)
-    :ivar str discriminator: The User's 4-digit discord-tag (i.e.: XXXX)
-    :ivar Optional[str] avatar: The user's avatar hash, if any
-    :ivar Optional[bool] bot: A status denoting if the user is a bot
-    :ivar Optional[bool] system: A status denoting if the user is an Official Discord System user
-    :ivar Optional[bool] mfa_enabled: A status denoting if the user has 2fa on their account
-    :ivar Optional[str] banner: The user's banner hash, if any
-    :ivar Optional[str] banner_color: The user's banner color as a hex, if any
-    :ivar Optional[int] accent_color: The user's banner color as an integer represented of hex color codes
-    :ivar Optional[str] locale: The user's chosen language option
-    :ivar Optional[bool] verified: Whether the email associated with this account has been verified
-    :ivar Optional[str] email: The user's email, if any
-    :ivar Optional[UserFlags] flags: The user's flags
-    :ivar Optional[int] premium_type: The type of Nitro subscription the user has
-    :ivar Optional[UserFlags] public_flags: The user's public flags
-    """
+    @property
+    def guild(self) -> "Guild":
+        """The guild this emoji belongs to."""
+        return self._client.cache.get_guild(self._guild_id)
 
-    id: Snowflake = field(converter=Snowflake)
-    username: str = field(repr=True)
-    discriminator: str = field(repr=True)
-    avatar: Optional[str] = field(default=None, repr=False)
-    bot: Optional[bool] = field(default=None)
-    system: Optional[bool] = field(default=None, repr=False)
-    mfa_enabled: Optional[bool] = field(default=None)
-    banner: Optional[str] = field(default=None, repr=False)
-    accent_color: Optional[int] = field(default=None, repr=False)
-    banner_color: Optional[str] = field(default=None, repr=False)
-    locale: Optional[str] = field(default=None)
-    verified: Optional[bool] = field(default=None)
-    email: Optional[str] = field(default=None)
-    flags: Optional[UserFlags] = field(converter=UserFlags, default=None, repr=False)
-    premium_type: Optional[int] = field(default=None, repr=False)
-    public_flags: Optional[UserFlags] = field(converter=UserFlags, default=None, repr=False)
-    bio: Optional[str] = field(default=None)
+    @property
+    def creator(self) -> Optional[Union["Member", "User"]]:
+        """The member that created this emoji."""
+        return self._client.cache.get_member(self._creator_id, self._guild_id) or self._client.cache.get_user(
+            self._creator_id
+        )
 
-    def has_public_flag(self, flag: Union[UserFlags, int]) -> bool:
-        """
-        .. versionadded:: 4.3.0
+    @property
+    def roles(self) -> List["Role"]:
+        """The roles allowed to use this emoji."""
+        return [self._client.cache.get_role(role_id) for role_id in self._role_ids]
 
-        Returns whether the user has public flag.
-        """
-        if self.public_flags == 0 or self.public_flags is None:
+    @property
+    def is_usable(self) -> bool:
+        """Determines if this emoji is usable by the current user."""
+        if not self.available:
             return False
-        return bool(int(self.public_flags) & flag)
 
-    @property
-    def mention(self) -> str:
-        """
-        .. versionadded:: 4.1.0
+        guild = self.guild
+        return any(e_role_id in guild.me._role_ids for e_role_id in self._role_ids)
 
-        Returns a string that allows you to mention the given user.
+    async def edit(
+        self,
+        *,
+        name: Optional[str] = None,
+        roles: Optional[List[Union["Snowflake_Type", "Role"]]] = None,
+        reason: Optional[str] = None,
+    ) -> "CustomEmoji":
+        """
+        Modify the custom emoji information.
+
+        Args:
+            name: The name of the emoji.
+            roles: The roles allowed to use this emoji.
+            reason: Attach a reason to this action, used for audit logs.
+
+        Returns:
+            The newly modified custom emoji.
+
+        """
+        data_payload = dict_filter_none(
+            {
+                "name": name,
+                "roles": roles,
+            }
+        )
 
-        :return: The string of the mentioned user.
-        :rtype: str
-        """
-        return f"<@{self.id}>"
+        updated_data = await self._client.http.modify_guild_emoji(data_payload, self._guild_id, self.id, reason=reason)
+        self.update_from_dict(updated_data)
+        return self
 
-    @property
-    def avatar_url(self) -> str:
+    async def delete(self, reason: Optional[str] = None) -> None:
         """
-        .. versionadded:: 4.2.0
+        Deletes the custom emoji from the guild.
 
-        Returns the URL of the user's avatar
+        Args:
+            reason: Attach a reason to this action, used for audit logs.
 
-        :return: URL of the user's avatar.
-        :rtype: str
         """
-        url = "https://cdn.discordapp.com/"
-        if self.avatar:
-            url += f"avatars/{int(self.id)}/{self.avatar}"
-            url += ".gif" if self.avatar.startswith("a_") else ".png"
-        else:
-            url += f"embed/avatars/{int(self.discriminator) % 5}.png"
-        return url
+        if not self._guild_id:
+            raise ValueError("Cannot delete emoji, no guild id set.")
 
-    @property
-    def banner_url(self) -> Optional[str]:
-        """
-        .. versionadded:: 4.2.0
+        await self._client.http.delete_guild_emoji(self._guild_id, self.id, reason=reason)
 
-        Returns the URL of the user's banner.
 
-        :return: URL of the user's banner (None will be returned if no banner is set)
-        :rtype: str
-        """
-        if not self.banner:
-            return None
-
-        url = f"https://cdn.discordapp.com/banners/{int(self.id)}/{self.banner}"
-        url += ".gif" if self.banner.startswith("a_") else ".png"
-        return url
+def process_emoji_req_format(emoji: Optional[Union[PartialEmoji, dict, str]]) -> Optional[str]:
+    """
+    Processes the emoji parameter into the str format required by the API.
 
-    @property
-    def presence(self) -> Optional["Presence"]:
-        """
-        .. versionadded:: 4.3.2
+    Args:
+        emoji: The emoji to process.
 
-        Returns the presence of the user.
+    Returns:
+        formatted string for discord
 
-        :return: Presence of the user (None will be returned if not cached)
-        :rtype: Optional[Presence]
-        """
-        from .gw import Presence
+    """
+    if not emoji:
+        return emoji
 
-        return self._client.cache[Presence].get(self.id)
+    if isinstance(emoji, str):
+        emoji = PartialEmoji.from_str(emoji)
 
-    @property
-    def created_at(self) -> datetime:
-        """
-        .. versionadded:: 4.4.0
+    if isinstance(emoji, dict):
+        emoji = PartialEmoji.from_dict(emoji)
 
-        Returns when the user was created.
-        """
-        return self.id.timestamp
+    if isinstance(emoji, PartialEmoji):
+        return emoji.req_format
 
-    async def send(
-        self,
-        content: Optional[str] = MISSING,
-        *,
-        components: Optional[
-            Union[
-                "ActionRow",
-                "Button",
-                "SelectMenu",
-                List["ActionRow"],
-                List["Button"],
-                List["SelectMenu"],
-            ]
-        ] = MISSING,
-        tts: Optional[bool] = MISSING,
-        attachments: Optional[List["Attachment"]] = MISSING,
-        files: Optional[Union[File, List[File]]] = MISSING,
-        embeds: Optional[Union["Embed", List["Embed"]]] = MISSING,
-        allowed_mentions: Optional[Union[AllowedMentions, dict]] = MISSING,
-    ) -> "Message":
-        """
-        .. versionadded:: 4.3.2
-
-        Sends a DM to the user.
-
-        :param Optional[str] content: The contents of the message as a string or string-converted value.
-        :param Optional[Union[ActionRow, Button, SelectMenu, List[ActionRow], List[Button], List[SelectMenu]]] components: A component, or list of components for the message.
-        :param Optional[bool] tts: Whether the message utilizes the text-to-speech Discord programme or not.
-        :param Optional[List[Attachment]] attachments: The attachments to attach to the message. Needs to be uploaded to the CDN first
-        :param Optional[Union[File, List[File]]] files: A file or list of files to be attached to the message.
-        :param Optional[Union[Embed, List[Embed]]] embeds: An embed, or list of embeds for the message.
-        :param Optional[Union[AllowedMentions, dict]] allowed_mentions: The allowed mentions for the message.
-        :return: The sent message as an object.
-        :rtype: Message
-        """
-        if not self._client:
-            raise LibraryException(code=13)
-        from ...client.models.component import _build_components
-        from .message import Message
-
-        _content: str = "" if content is MISSING else content
-        _tts: bool = False if tts is MISSING else tts
-        _attachments = [] if attachments is MISSING else [a._json for a in attachments]
-        _embeds: list = (
-            []
-            if not embeds or embeds is MISSING
-            else ([embed._json for embed in embeds] if isinstance(embeds, list) else [embeds._json])
-        )
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
-        if not components or components is MISSING:
-            _components = []
-        else:
-            _components = _build_components(components=components)
+    raise ValueError(f"Invalid emoji: {emoji}")
 
-        if not files or files is MISSING:
-            _files = []
-        elif isinstance(files, list):
-            _files = [file._json_payload(id) for id, file in enumerate(files)]
-        else:
-            _files = [files._json_payload(0)]
-            files = [files]
 
-        _files.extend(_attachments)
+def process_emoji(emoji: Optional[Union[PartialEmoji, dict, str]]) -> Optional[dict]:
+    """
+    Processes the emoji parameter into the dictionary format required by the API.
 
-        payload = dict(
-            content=_content,
-            tts=_tts,
-            attachments=_files,
-            embeds=_embeds,
-            components=_components,
-            allowed_mentions=_allowed_mentions,
-        )
-        channel = await self._client.create_dm(recipient_id=int(self.id))
-        res = await self._client.create_message(
-            channel_id=int(channel["id"]), payload=payload, files=files
-        )
+    Args:
+        emoji: The emoji to process.
 
-        return Message(**res, _client=self._client)
+    Returns:
+        formatted dictionary for discord
 
-    async def get_dm_channel(self) -> "Channel":
-        """
-        .. versionadded:: 4.4.0
+    """
+    if not emoji:
+        return emoji
 
-        Gets the DM channel with the user
+    if isinstance(emoji, dict):
+        return emoji
 
-        :return: The DM channel with the user
-        :rtype: Channel
-        """
-        if not self._client:
-            raise LibraryException(code=13)
+    if isinstance(emoji, str):
+        emoji = PartialEmoji.from_str(emoji)
 
-        from .channel import Channel
+    if isinstance(emoji, PartialEmoji):
+        return emoji.to_dict()
 
-        return Channel(**await self._client.create_dm(int(self.id)), _client=self._client)
+    raise ValueError(f"Invalid emoji: {emoji}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `discord-py-interactions-4.4.1/interactions/api/models/webhook.py` & `discord-py-interactions-5.0.0/interactions/models/internal/extension.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,304 +1,278 @@
-# versionadded is specified in docs gen file
+import asyncio
+import inspect
+import typing
+from typing import Awaitable, Dict, List, TYPE_CHECKING, Callable, Coroutine, Optional
+
+import interactions.models.internal as models
+import interactions.api.events as events
+from interactions.models.internal.callback import CallbackObject
+from interactions.client.const import MISSING
+from interactions.client.utils.misc_utils import wrap_partial
+from interactions.models.internal.tasks import Task
 
-from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union
+if TYPE_CHECKING:
+    from interactions.client import Client
+    from interactions.models.discord import Snowflake_Type
+    from interactions.models.internal import AutoDefer, BaseCommand, InteractionCommand, Listener
+    from interactions.models.internal import BaseContext
 
-from ...client.enums import IntEnum
-from ...utils.attrs_utils import ClientSerializerMixin, define, field
-from ...utils.missing import MISSING
-from ..error import LibraryException
-from .misc import AllowedMentions, File, IDMixin, Image, Snowflake
-from .user import User
 
-if TYPE_CHECKING:
-    from ...client.models.component import ActionRow, Button, SelectMenu
-    from ..http import HTTPClient
-    from .channel import Channel
-    from .guild import Guild
-    from .message import Attachment, Embed, Message
-
-__all__ = (
-    "Webhook",
-    "WebhookType",
-)
-
-
-class WebhookType(IntEnum):
-    Incoming = 1
-    Channel_Follower = 2
-    Application = 3
+__all__ = ("Extension",)
 
 
-@define()
-class Webhook(ClientSerializerMixin, IDMixin):
+class Extension:
     """
-    A class object representing a Webhook.
+    A class that allows you to separate your commands and listeners into separate files. Skins require an entrypoint in the same file called `setup`, this function allows client to load the Extension.
+
+    ??? Hint "Example Usage:"
+        ```python
+        class ExampleExt(Extension):
+            def __init__(self, bot):
+                print("Extension Created")
+
+            @prefixed_command()
+            async def some_command(self, context):
+                await ctx.send(f"I was sent from a extension called {self.name}")
+        ```
+
+    Attributes:
+        bot Client: A reference to the client
+        name str: The name of this Extension (`read-only`)
+        description str: A description of this Extension
+        extension_checks str: A list of checks to be ran on any command in this extension
+        extension_prerun List: A list of coroutines to be run before any command in this extension
+        extension_postrun List: A list of coroutines to be run after any command in this extension
+        interaction_tree Dict: A dictionary of registered application commands in a tree
 
-    :ivar Snowflake id: the id of the webhook
-    :ivar WebhookType type: the type of the webhook
-    :ivar Snowflake guild_id: the guild id this webhook is for, if any
-    :ivar Snowflake channel_id: the channel id this webhook is for, if any
-    :ivar User user: the user this webhook was created by (not returned when getting a webhook with its token)
-    :ivar str name: the default name of the webhook
-    :ivar str avatar: the default user avatar hash of the webhook
-    :ivar str token: the secure token of the webhook (returned for Incoming Webhooks)
-    :ivar Snowflake application_id: the bot/OAuth2 application that created this webhook
-    :ivar Guild source_guild: the guild of the channel that this webhook is following (returned for Channel Follower Webhooks)
-    :ivar Channel source_channel: the channel that this webhook is following (returned for Channel Follower Webhooks)
-    :ivar str url: the url used for executing the webhook (returned by the webhooks OAuth2 flow)
     """
 
-    id: Snowflake = field(converter=Snowflake)
-    type: Union[WebhookType, int] = field(converter=WebhookType)
-    guild_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    channel_id: Optional[Snowflake] = field(converter=Snowflake, default=None)
-    user: Optional[User] = field(converter=User, default=None, add_client=True)
-    name: str = field()
-    avatar: str = field(repr=False)
-    token: Optional[str] = field(default=None)
-    application_id: Snowflake = field(converter=Snowflake)
-    source_guild: Optional["Guild"] = field(default=None)
-    source_channel: Optional["Channel"] = field(default=None)
-    url: Optional[str] = field(default=None)
-
-    def __attrs_post_init__(self):
-        # circular imports suck
-        from .channel import Channel
-        from .guild import Guild
+    bot: "Client"
+    name: str
+    extension_name: str
+    description: str
+    extension_checks: List
+    extension_prerun: List
+    extension_postrun: List
+    extension_error: Optional[Callable[..., Coroutine]]
+    interaction_tree: Dict["Snowflake_Type", Dict[str, "InteractionCommand" | Dict[str, "InteractionCommand"]]]
+    _commands: List
+    _listeners: List
+    auto_defer: "AutoDefer"
+
+    class Metadata:
+        """Info about the Extension"""
+
+        name: str
+        """The name of this Extension"""
+        version: str
+        """The version of this Extension"""
+        url: str
+        """The repository url of this Extension"""
+        description: str
+        """A description of this Extension"""
+        requirements: List[str]
+        """A list of requirements for this Extension"""
+
+    def __new__(cls, bot: "Client", *args, **kwargs) -> "Extension":
+        instance = super().__new__(cls)
+        instance.bot = bot
+        instance.client = bot
+
+        instance.name = cls.__name__
+        instance.extension_checks = []
+        instance.extension_prerun = []
+        instance.extension_postrun = []
+        instance.extension_error = None
+        instance.interaction_tree = {}
+        instance.auto_defer = MISSING
+
+        instance.description = kwargs.get("Description")
+        if not instance.description:
+            instance.description = inspect.cleandoc(cls.__doc__) if cls.__doc__ else None
+
+        # load commands from class
+        instance._commands = []
+        instance._listeners = []
 
-        self.source_guild = (
-            Guild(**self.source_guild, _client=self._client) if self.source_guild else None
-        )
-        self.source_channel = (
-            Channel(**self.source_channel, _client=self._client) if self.source_channel else None
+        callables: list[tuple[str, typing.Callable]] = inspect.getmembers(
+            instance, predicate=lambda x: isinstance(x, (CallbackObject, Task))
         )
 
-    @property
-    def created_at(self) -> datetime:
-        """
-        .. versionadded:: 4.4.0
+        for _name, val in callables:
+            if isinstance(val, models.BaseCommand):
+                val.extension = instance
+                val = wrap_partial(val, instance)
+                bot.add_command(val)
+                instance._commands.append(val)
+
+            elif isinstance(val, Task):
+                wrap_partial(val, instance)
+
+            elif isinstance(val, models.Listener):
+                val.extension = instance
+                val = wrap_partial(val, instance)
+                bot.add_listener(val)  # type: ignore
+                instance._listeners.append(val)
+            elif isinstance(val, models.GlobalAutoComplete):
+                val.extension = instance
+                val = wrap_partial(val, instance)
+                bot.add_global_autocomplete(val)
+        bot.dispatch(events.ExtensionCommandParse(extension=instance, callables=callables))
+
+        instance.extension_name = inspect.getmodule(instance).__name__
+        instance.bot.ext[instance.name] = instance
+
+        if hasattr(instance, "async_start"):
+            if inspect.iscoroutinefunction(instance.async_start):
+                bot.async_startup_tasks.append((instance.async_start, (), {}))
+            else:
+                raise TypeError("async_start is a reserved method and must be a coroutine")
 
-        Returns when the webhook was created.
-        """
-        return self.id.timestamp
+        bot.dispatch(events.ExtensionLoad(extension=instance))
+        return instance
 
-    @classmethod
-    async def create(
-        cls,
-        client: "HTTPClient",
-        channel_id: int,
-        name: str,
-        avatar: Optional[Image] = MISSING,
-    ) -> "Webhook":
-        """
-        Creates a webhook in a channel.
-
-        :param HTTPClient client: The HTTPClient of the bot, has to be set to ``bot._http``.
-        :param int channel_id: The ID of the channel to create the webhook in.
-        :param str name: The name of the webhook.
-        :param Optional[Image] avatar: The avatar of the Webhook, if any.
-        :return: The created webhook as object
-        :rtype: Webhook
-        """
+    @property
+    def __name__(self) -> str:
+        return self.name
 
-        _avatar = avatar.data if avatar is not MISSING else None
+    @property
+    def commands(self) -> List["BaseCommand"]:
+        """Get the commands from this Extension."""
+        return self._commands
 
-        res = await client.create_webhook(channel_id=channel_id, name=name, avatar=_avatar)
+    @property
+    def listeners(self) -> List["Listener"]:
+        """Get the listeners from this Extension."""
+        return self._listeners
 
-        return cls(**res, _client=client)
+    def drop(self) -> None:
+        """Called when this Extension is being removed."""
+        for func in self._commands:
+            if isinstance(func, models.ModalCommand):
+                for listener in func.listeners:
+                    # noinspection PyProtectedMember
+                    self.bot._modal_callbacks.pop(listener)
+            elif isinstance(func, models.ComponentCommand):
+                for listener in func.listeners:
+                    # noinspection PyProtectedMember
+                    self.bot._component_callbacks.pop(listener)
+            elif isinstance(func, models.InteractionCommand):
+                for scope in func.scopes:
+                    if self.bot.interactions_by_scope.get(scope):
+                        self.bot.interactions_by_scope[scope].pop(func.resolved_name, [])
+        for func in self.listeners:
+            self.bot.listeners[func.event].remove(func)
 
-    @classmethod
-    async def get(
-        cls,
-        client: "HTTPClient",
-        webhook_id: int,
-        webhook_token: Optional[str] = MISSING,
-    ) -> "Webhook":
-        """
-        Gets an existing webhook.
+        self.bot.ext.pop(self.name, None)
+        self.bot.dispatch(events.ExtensionUnload(extension=self))
+        self.bot.logger.debug(f"{self.name} has been drop")
 
-        :param HTTPClient client: The HTTPClient of the bot, has to be set to ``bot._http``.
-        :param int webhook_id: The ID of the webhook.
-        :param Optional[str] webhook_token: The token of the webhook, optional
-        :return: The Webhook object
-        :rtype: Webhook
+    def add_ext_auto_defer(self, enabled: bool = True, ephemeral: bool = False, time_until_defer: float = 0.0) -> None:
         """
+        Add a auto defer for all commands in this extension.
 
-        _token = webhook_token if webhook_token is not MISSING else None
-
-        res = await client.get_webhook(webhook_id=webhook_id, webhook_token=_token)
+        Args:
+            enabled: Should the command be deferred automatically
+            ephemeral: Should the command be deferred as ephemeral
+            time_until_defer: How long to wait before deferring automatically
 
-        return cls(**res, _client=client)
-
-    async def modify(
-        self,
-        name: Optional[str] = MISSING,
-        channel_id: int = MISSING,
-        avatar: Optional[Image] = MISSING,
-    ) -> "Webhook":  # sourcery skip: compare-via-equals
         """
-        Modifies the current webhook.
+        self.auto_defer = models.AutoDefer(enabled=enabled, ephemeral=ephemeral, time_until_defer=time_until_defer)
 
-        :param Optional[str] name: The new name of the webhook
-        :param int channel_id: The channel id of the webhook. If not provided, the webhook token will be used for authentication
-        :param Optional[Image] avatar: The new avatar of the webhook
-        :return: The modified webhook object
-        :rtype: Webhook
+    def add_ext_check(self, coroutine: Callable[["BaseContext"], Awaitable[bool]]) -> None:
         """
+        Add a coroutine as a check for all commands in this extension to run. This coroutine must take **only** the parameter `context`.
 
-        if not self._client:
-            raise LibraryException(code=13)
+        ??? Hint "Example Usage:"
+            ```python
+            def __init__(self, bot):
+                self.add_ext_check(self.example)
 
-        if channel_id in (None, MISSING) and not self.token:
-            raise LibraryException(
-                message="no token was found, please specify a channel id!", code=12
-            )
+            @staticmethod
+            async def example(context: BaseContext):
+                if context.author.id == 123456789:
+                    return True
+                return False
+            ```
+        Args:
+            coroutine: The coroutine to use as a check
 
-        payload = {}
+        """
+        if not asyncio.iscoroutinefunction(coroutine):
+            raise TypeError("Check must be a coroutine")
 
-        if name is not MISSING:
-            payload["name"] = name
+        if not self.extension_checks:
+            self.extension_checks = []
 
-        if avatar is not MISSING:
-            payload["avatar"] = avatar.data
+        self.extension_checks.append(coroutine)
 
-        if channel_id is not MISSING:
-            payload["channel_id"] = channel_id
+    def add_extension_prerun(self, coroutine: Callable[..., Coroutine]) -> None:
+        """
+        Add a coroutine to be run **before** all commands in this Extension.
 
-        res = await self._client.modify_webhook(
-            webhook_id=int(self.id),
-            payload=payload,
-            webhook_token=None if channel_id else self.token,
-        )
+        !!! note
+            Pre-runs will **only** be run if the commands checks pass
 
-        self.update(res)
-        return self
+        ??? Hint "Example Usage:"
+            ```python
+            def __init__(self, bot):
+                self.add_extension_prerun(self.example)
 
-    async def execute(
-        self,
-        content: Optional[str] = MISSING,
-        username: Optional[str] = MISSING,
-        avatar_url: Optional[str] = MISSING,
-        tts: Optional[bool] = MISSING,
-        embeds: Optional[Union["Embed", List["Embed"]]] = MISSING,
-        allowed_mentions: Optional[Union[AllowedMentions, dict]] = MISSING,
-        attachments: Optional[List["Attachment"]] = MISSING,
-        components: Optional[
-            Union[
-                "ActionRow",
-                "Button",
-                "SelectMenu",
-                List["ActionRow"],
-                List["Button"],
-                List["SelectMenu"],
-            ]
-        ] = MISSING,
-        files: Optional[Union[File, List[File]]] = MISSING,
-        thread_id: Optional[int] = MISSING,
-    ) -> Optional["Message"]:  # sourcery skip: low-code-quality
-        """
-        Executes the webhook. All parameters to this function are optional.
+            async def example(self, context: BaseContext):
+                await ctx.send("I ran first")
+            ```
 
-        .. important::
-            The ``components`` argument requires an application-owned webhook.
+        Args:
+            coroutine: The coroutine to run
 
-        :param str content: the message contents (up to 2000 characters)
-        :param str username: override the default username of the webhook
-        :param str avatar_url: override the default avatar of the webhook
-        :param bool tts: true if this is a TTS message
-        :param Optional[List[Attachment]] attachments: The attachments to attach to the message. Needs to be uploaded to the CDN first
-        :param Union[Embed, List[Embed]] embeds: embedded ``rich`` content
-        :param Optional[Union[AllowedMentions, dict]] allowed_mentions: The allowed mentions for the message.
-        :param Union[ActionRow, Button, SelectMenu, List[ActionRow], List[Button], List[SelectMenu]] components: the components to include with the message
-        :param Union[File, List[File]] files: The files to attach to the message
-        :param int thread_id: Send a message to a specified thread within a webhook's channel. The thread will automatically be unarchived
-        :return: The sent message, if present
-        :rtype: Optional[Message]
         """
+        if not asyncio.iscoroutinefunction(coroutine):
+            raise TypeError("Callback must be a coroutine")
 
-        if not self._client:
-            raise LibraryException(code=13)
-
-        from ...client.models.component import _build_components
-        from .message import Message
+        if not self.extension_prerun:
+            self.extension_prerun = []
+        self.extension_prerun.append(coroutine)
 
-        _content: str = "" if content is MISSING else content
-        _tts: bool = False if tts is MISSING else tts
-        _attachments = [] if attachments is MISSING else [a._json for a in attachments]
-
-        _embeds: list = (
-            []
-            if not embeds or embeds is MISSING
-            else ([embed._json for embed in embeds] if isinstance(embeds, list) else [embeds._json])
-        )
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
+    def add_extension_postrun(self, coroutine: Callable[..., Coroutine]) -> None:
+        """
+        Add a coroutine to be run **after** all commands in this Extension.
 
-        if not components or components is MISSING:
-            _components = []
-        else:
-            _components = _build_components(components=components)
-
-        if not files or files is MISSING:
-            _files = []
-        elif isinstance(files, list):
-            _files = [file._json_payload(id) for id, file in enumerate(files)]
-        else:
-            _files = [files._json_payload(0)]
-            files = [files]
-
-        _files.extend(_attachments)
-
-        payload: dict = dict(
-            content=_content,
-            tts=_tts,
-            attachments=_files,
-            embeds=_embeds,
-            components=_components,
-            allowed_mentions=_allowed_mentions,
-        )
+        ??? Hint "Example Usage:"
+            ```python
+            def __init__(self, bot):
+                self.add_extension_postrun(self.example)
 
-        if username is not MISSING:
-            payload["username"] = username
+            async def example(self, context: BaseContext):
+                await ctx.send("I ran first")
+            ```
 
-        if avatar_url is not MISSING:
-            payload["avatar_url"] = avatar_url
+        Args:
+            coroutine: The coroutine to run
 
-        res = await self._client.execute_webhook(
-            webhook_id=int(self.id),
-            webhook_token=self.token,
-            files=files,
-            payload=payload,
-            thread_id=thread_id if thread_id is not MISSING else None,
-        )
+        """
+        if not asyncio.iscoroutinefunction(coroutine):
+            raise TypeError("Callback must be a coroutine")
 
-        return Message(**res, _client=self._client) if isinstance(res, dict) else res
+        if not self.extension_postrun:
+            self.extension_postrun = []
+        self.extension_postrun.append(coroutine)
 
-    async def delete(self) -> None:
+    def set_extension_error(self, coroutine: Callable[..., Coroutine]) -> None:
         """
-        Deletes the webhook.
-        """
-        if not self._client:
-            raise LibraryException(code=13)
+        Add a coroutine to handle any exceptions raised in this extension.
 
-        await self._client.delete_webhook(webhook_id=int(self.id), webhook_token=self.token)
+        ??? Hint "Example Usage:"
+            ```python
+            def __init__(self, bot):
+                self.set_extension_error(self.example)
 
-    @property
-    def avatar_url(self) -> Optional[str]:
-        """
-        Returns the URL of the webhook's avatar.
+        Args:
+            coroutine: The coroutine to run
 
-        :return: URL of the webhook's avatar
-        :rtype: str
         """
-        if not self.avatar:
-            return None
+        if not asyncio.iscoroutinefunction(coroutine):
+            raise TypeError("Callback must be a coroutine")
 
-        url = f"https://cdn.discordapp.com/avatars/{int(self.id)}/{self.avatar}"
-        url += ".gif" if self.avatar.startswith("a_") else ".png"
-        return url
+        if self.extension_error:
+            self.bot.logger.warning("Extension error callback has been overridden!")
+        self.extension_error = coroutine
```

### Comparing `discord-py-interactions-4.4.1/interactions/client/bot.py` & `discord-py-interactions-5.0.0/interactions/models/discord/guild.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,2147 +1,2338 @@
-import contextlib
-import logging
-import re
-import sys
-from asyncio import AbstractEventLoop, CancelledError, get_event_loop, iscoroutinefunction, wait_for
-from functools import wraps
-from importlib import import_module
-from importlib.util import resolve_name
-from inspect import getmembers, isawaitable
-from types import ModuleType
-from typing import Any, Awaitable, Callable, Coroutine, Dict, List, Optional, Tuple, Union
-
-from ..api import WebSocketClient as WSClient
-from ..api.cache import Cache
-from ..api.error import LibraryException
-from ..api.http.client import HTTPClient
-from ..api.models.channel import Channel
-from ..api.models.flags import Intents, Permissions
-from ..api.models.guild import Guild
-from ..api.models.member import Member
-from ..api.models.message import Message
-from ..api.models.misc import Image, Snowflake
-from ..api.models.presence import ClientPresence
-from ..api.models.role import Role
-from ..api.models.team import Application, ApplicationRoleConnectionMetadata
-from ..api.models.user import User
-from ..base import get_logger
-from ..utils.attrs_utils import convert_list
-from ..utils.missing import MISSING
-from .context import CommandContext, ComponentContext
-from .decor import component as _component
-from .enums import ApplicationCommandType, Locale, OptionType
-from .models.command import ApplicationCommand, Choice, Command, Option
-from .models.component import ActionRow, Button, Modal, SelectMenu
+import asyncio
+import time
+from asyncio import QueueEmpty
+from collections import namedtuple
+from functools import cmp_to_key
+from typing import List, Optional, Union, Set, Dict, Any, TYPE_CHECKING
+from warnings import warn
+
+import attrs
+
+import interactions.models as models
+from interactions.client.const import Absent, MISSING, PREMIUM_GUILD_LIMITS
+from interactions.client.errors import EventLocationNotProvided, NotFound
+from interactions.client.mixins.serialization import DictSerializationMixin
+from interactions.client.utils.attr_converters import optional
+from interactions.client.utils.attr_converters import timestamp_converter
+from interactions.client.utils.attr_utils import docs
+from interactions.client.utils.deserialise_app_cmds import deserialize_app_cmds
+from interactions.client.utils.serializer import to_image_data, no_export_meta
+from interactions.models.discord.app_perms import CommandPermissions, ApplicationCommandPermission
+from interactions.models.discord.auto_mod import AutoModRule, BaseAction, BaseTrigger
+from interactions.models.discord.file import UPLOADABLE_TYPE
+from interactions.models.misc.iterator import AsyncIterator
+from .base import DiscordObject, ClientObject
+from .enums import (
+    NSFWLevel,
+    Permissions,
+    SystemChannelFlags,
+    VerificationLevel,
+    DefaultNotificationLevel,
+    ExplicitContentFilterLevel,
+    MFALevel,
+    ChannelType,
+    IntegrationExpireBehaviour,
+    ScheduledEventPrivacyLevel,
+    ScheduledEventType,
+    AuditLogEventType,
+    AutoModEvent,
+    AutoModTriggerType,
+    ForumLayoutType,
+)
+from .snowflake import to_snowflake, Snowflake_Type, to_optional_snowflake, to_snowflake_list
 
-log: logging.Logger = get_logger("client")
+if TYPE_CHECKING:
+    from interactions.client.client import Client
+    from interactions import InteractionCommand
 
 __all__ = (
-    "Client",
-    "Extension",
-    "extension_listener",
-    "extension_command",
-    "extension_component",
-    "extension_modal",
-    "extension_autocomplete",
-    "extension_user_command",
-    "extension_message_command",
+    "GuildBan",
+    "BaseGuild",
+    "GuildWelcome",
+    "GuildPreview",
+    "Guild",
+    "GuildTemplate",
+    "GuildWelcomeChannel",
+    "GuildIntegration",
+    "GuildWidgetSettings",
+    "GuildWidget",
+    "AuditLogChange",
+    "AuditLogEntry",
+    "AuditLog",
+    "AuditLogHistory",
 )
 
 
-class Client:
-    """
-    A class representing the client connection to Discord's gateway and API via. WebSocket and HTTP.
-
-    :param str token: The token of the application for authentication and connection.
-    :param Optional[Intents] intents: Allows specific control of permissions the application has when connected. In order to use multiple intents, the ``|`` operator is recommended. Defaults to :attr:`.Intents.DEFAULT`.
-    :param Optional[List[Tuple[int]]] shards: Dictates and controls the shards that the application connects under.
-    :param Optional[ClientPresence] presence: Sets an RPC-like presence on the application when connected to the Gateway.
-    :param Optional[Union[int, Guild, List[int], List[Guild]]] default_scope:
-        .. versionadded:: 4.3.0
-
-        Sets the default scope of all commands.
-    :param Optional[bool] disable_sync: Controls whether synchronization in the user-facing API should be automatic or not.
-    :param Optional[Union[bool, logging.DEBUG, logging.INFO, logging.NOTSET, logging.WARNING, logging.ERROR, logging.CRITICAL]] logging:
-        .. versionadded:: 4.3.2
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildBan:
+    reason: Optional[str]
+    """The reason for the ban"""
+    user: "models.User"
+    """The banned user"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class BaseGuild(DiscordObject):
+    name: str = attrs.field(repr=True)
+    """Name of guild. (2-100 characters, excluding trailing and leading whitespace)"""
+    description: Optional[str] = attrs.field(repr=True, default=None)
+    """The description for the guild, if the guild is discoverable"""
+
+    icon: Optional["models.Asset"] = attrs.field(repr=False, default=None)
+    """Icon image asset"""
+    splash: Optional["models.Asset"] = attrs.field(repr=False, default=None)
+    """Splash image asset"""
+    discovery_splash: Optional["models.Asset"] = attrs.field(repr=False, default=None)
+    """Discovery splash image. Only present for guilds with the "DISCOVERABLE" feature."""
+    features: List[str] = attrs.field(repr=False, factory=list)
+    """The features of this guild"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if icon_hash := data.pop("icon", None):
+            data["icon"] = models.Asset.from_path_hash(client, f"icons/{data['id']}/{{}}", icon_hash)
+        if splash_hash := data.pop("splash", None):
+            data["splash"] = models.Asset.from_path_hash(client, f"splashes/{data['id']}/{{}}", splash_hash)
+        if disco_splash := data.pop("discovery_splash", None):
+            data["discovery_splash"] = models.Asset.from_path_hash(
+                client, f"discovery-splashes/{data['id']}/{{}}", disco_splash
+            )
+        return data
 
-        Set to ``True`` to enable debug logging or set to a log level to use a specific level
 
-    :ivar Application me: The application representation of the client.
-    """
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildWelcome(ClientObject):
+    description: Optional[str] = attrs.field(
+        repr=False, default=None, metadata=docs("Welcome Screen server description")
+    )
+    welcome_channels: List["models.GuildWelcomeChannel"] = attrs.field(
+        repr=False, metadata=docs("List of Welcome Channel objects, up to 5")
+    )
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildPreview(BaseGuild):
+    """A partial guild object."""
+
+    emoji: list["models.PartialEmoji"] = attrs.field(repr=False, factory=list)
+    """A list of custom emoji from this guild"""
+    approximate_member_count: int = attrs.field(repr=False, default=0)
+    """Approximate number of members in this guild"""
+    approximate_presence_count: int = attrs.field(repr=False, default=0)
+    """Approximate number of online members in this guild"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        return super()._process_dict(data, client)
+
+
+class MemberIterator(AsyncIterator):
+    def __init__(self, guild: "Guild", limit: int = 0) -> None:
+        super().__init__(limit)
+        self.guild = guild
+        self._more = True
+
+    async def fetch(self) -> list:
+        if self._more:
+            expected = self.get_limit
 
-    def __init__(
-        self,
-        token: Optional[str] = None,
-        cache_limits: Optional[Dict[type, int]] = None,
-        intents: Intents = Intents.DEFAULT,
-        shards: Optional[List[Tuple[int]]] = None,
-        default_scope: Optional[Union[int, Snowflake, List[Union[int, Snowflake]]]] = None,
-        presence: Optional[ClientPresence] = None,
-        _logging: Union[bool, int] = None,
-        disable_sync: bool = False,
-        **kwargs,
-    ) -> None:
-        self._loop: AbstractEventLoop = get_event_loop()
-        self._http: Union[str, HTTPClient] = token
-        self._intents: Intents = intents
-        self._shards: List[Tuple[int]] = shards or []
-        self._commands: List[Command] = []
-        self._default_scope = default_scope
-        self._presence = presence
-        self._token = token
-        self._extensions = {}
-        self._scopes = set()
-        self.__command_coroutines = []
-        self.__global_commands = {}
-        self.__guild_commands = {}
-
-        self.me: Optional[Application] = None
-        self.__id_autocomplete = {}
-        if self._default_scope:
-            if not isinstance(self._default_scope, list):
-                self._default_scope = [self._default_scope]
-            if any(isinstance(scope, Guild) for scope in self._default_scope):
-                self._default_scope = [
-                    (scope.id if isinstance(scope, Guild) else scope)
-                    for scope in self._default_scope
-                ]
-        self._default_scope = convert_list(int)(self._default_scope)
-
-        if cache_limits is None:
-            # Messages have the most explosive growth, but more limits can be added as needed
-            cache_limits = {
-                Message: 1000,  # Most users won't need to cache many messages
-            }
-
-        self._cache: Cache = Cache(cache_limits)
-        self._websocket: WSClient = WSClient(
-            token=token,
-            cache=self._cache,
-            intents=self._intents,
-            shards=self._shards,
-            presence=self._presence,
+            rcv = await self.guild._client.http.list_members(
+                self.guild.id, limit=expected, after=self.last["id"] if self.last else MISSING
+            )
+            if not rcv:
+                raise QueueEmpty
+            self._more = len(rcv) == expected
+            return rcv
+        raise QueueEmpty
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class Guild(BaseGuild):
+    """Guilds in Discord represent an isolated collection of users and channels, and are often referred to as "servers" in the UI."""
+
+    unavailable: bool = attrs.field(repr=False, default=False)
+    """True if this guild is unavailable due to an outage."""
+    # owner: bool = attrs.field(repr=False, default=False)  # we get this from api but it's kinda useless to store
+    afk_channel_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
+    """The channel id for afk."""
+    afk_timeout: Optional[int] = attrs.field(repr=False, default=None)
+    """afk timeout in seconds."""
+    widget_enabled: bool = attrs.field(repr=False, default=False)
+    """True if the server widget is enabled."""
+    widget_channel_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
+    """The channel id that the widget will generate an invite to, or None if set to no invite."""
+    verification_level: Union[VerificationLevel, int] = attrs.field(repr=False, default=VerificationLevel.NONE)
+    """The verification level required for the guild."""
+    default_message_notifications: Union[DefaultNotificationLevel, int] = attrs.field(
+        repr=False, default=DefaultNotificationLevel.ALL_MESSAGES
+    )
+    """The default message notifications level."""
+    explicit_content_filter: Union[ExplicitContentFilterLevel, int] = attrs.field(
+        repr=False, default=ExplicitContentFilterLevel.DISABLED
+    )
+    """The explicit content filter level."""
+    mfa_level: Union[MFALevel, int] = attrs.field(repr=False, default=MFALevel.NONE)
+    """The required MFA (Multi Factor Authentication) level for the guild."""
+    system_channel_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
+    """The id of the channel where guild notices such as welcome messages and boost events are posted."""
+    system_channel_flags: SystemChannelFlags = attrs.field(
+        repr=False, default=SystemChannelFlags.NONE, converter=SystemChannelFlags
+    )
+    """The system channel flags."""
+    rules_channel_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
+    """The id of the channel where Community guilds can display rules and/or guidelines."""
+    joined_at: str = attrs.field(repr=False, default=None, converter=optional(timestamp_converter))
+    """When this guild was joined at."""
+    large: bool = attrs.field(repr=False, default=False)
+    """True if this is considered a large guild."""
+    member_count: int = attrs.field(repr=False, default=0)
+    """The total number of members in this guild."""
+    presences: List[dict] = attrs.field(repr=False, factory=list)
+    """The presences of the members in the guild, will only include non-offline members if the size is greater than large threshold."""
+    max_presences: Optional[int] = attrs.field(repr=False, default=None)
+    """The maximum number of presences for the guild. (None is always returned, apart from the largest of guilds)"""
+    max_members: Optional[int] = attrs.field(repr=False, default=None)
+    """The maximum number of members for the guild."""
+    vanity_url_code: Optional[str] = attrs.field(repr=False, default=None)
+    """The vanity url code for the guild."""
+    banner: Optional[str] = attrs.field(repr=False, default=None)
+    """Hash for banner image."""
+    premium_tier: Optional[str] = attrs.field(repr=False, default=None)
+    """The premium tier level. (Server Boost level)"""
+    premium_subscription_count: int = attrs.field(repr=False, default=0)
+    """The number of boosts this guild currently has."""
+    preferred_locale: str = attrs.field(
+        repr=False,
+    )
+    """The preferred locale of a Community guild. Used in server discovery and notices from Discord. Defaults to \"en-US\""""
+    public_updates_channel_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
+    """The id of the channel where admins and moderators of Community guilds receive notices from Discord."""
+    max_video_channel_users: int = attrs.field(repr=False, default=0)
+    """The maximum amount of users in a video channel."""
+    welcome_screen: Optional["GuildWelcome"] = attrs.field(repr=False, default=None)
+    """The welcome screen of a Community guild, shown to new members, returned in an Invite's guild object."""
+    nsfw_level: Union[NSFWLevel, int] = attrs.field(repr=False, default=NSFWLevel.DEFAULT)
+    """The guild NSFW level."""
+    stage_instances: List[dict] = attrs.field(repr=False, factory=list)  # TODO stage instance objects
+    """Stage instances in the guild."""
+    chunked = attrs.field(repr=False, factory=asyncio.Event, metadata=no_export_meta)
+    """An event that is fired when this guild has been chunked"""
+    command_permissions: dict[Snowflake_Type, CommandPermissions] = attrs.field(
+        repr=False, factory=dict, metadata=no_export_meta
+    )
+    """A cache of all command permissions for this guild"""
+    premium_progress_bar_enabled: bool = attrs.field(repr=False, default=False)
+    """True if the guild has the boost progress bar enabled"""
+
+    _owner_id: Snowflake_Type = attrs.field(repr=False, converter=to_snowflake)
+    _channel_ids: Set[Snowflake_Type] = attrs.field(repr=False, factory=set)
+    _thread_ids: Set[Snowflake_Type] = attrs.field(repr=False, factory=set)
+    _member_ids: Set[Snowflake_Type] = attrs.field(repr=False, factory=set)
+    _role_ids: Set[Snowflake_Type] = attrs.field(repr=False, factory=set)
+    _chunk_cache: list = attrs.field(repr=False, factory=list)
+    _channel_gui_positions: Dict[Snowflake_Type, int] = attrs.field(repr=False, factory=dict)
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        data = super()._process_dict(data, client)
+        guild_id = data["id"]
+
+        channels_data = data.pop("channels", [])
+        for c in channels_data:
+            c["guild_id"] = guild_id
+        data["channel_ids"] = {client.cache.place_channel_data(channel_data).id for channel_data in channels_data}
+
+        threads_data = data.pop("threads", [])
+        data["thread_ids"] = {client.cache.place_channel_data(thread_data).id for thread_data in threads_data}
+
+        members_data = data.pop("members", [])
+        data["member_ids"] = {client.cache.place_member_data(guild_id, member_data).id for member_data in members_data}
+
+        roles_data = data.pop("roles", [])
+        data["role_ids"] = set(client.cache.place_role_data(guild_id, roles_data).keys())
+
+        if welcome_screen := data.get("welcome_screen"):
+            data["welcome_screen"] = GuildWelcome.from_dict(welcome_screen, client)
+
+        if voice_states := data.get("voice_states"):
+            [
+                asyncio.create_task(client.cache.place_voice_state_data(state | {"guild_id": guild_id}))
+                for state in voice_states
+            ]
+        return data
+
+    @classmethod
+    async def create(
+        cls,
+        name: str,
+        client: "Client",
+        *,
+        icon: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        verification_level: Absent["VerificationLevel"] = MISSING,
+        default_message_notifications: Absent["DefaultNotificationLevel"] = MISSING,
+        explicit_content_filter: Absent["ExplicitContentFilterLevel"] = MISSING,
+        roles: Absent[list[dict]] = MISSING,
+        channels: Absent[list[dict]] = MISSING,
+        afk_channel_id: Absent["Snowflake_Type"] = MISSING,
+        afk_timeout: Absent[int] = MISSING,
+        system_channel_id: Absent["Snowflake_Type"] = MISSING,
+        system_channel_flags: Absent["SystemChannelFlags"] = MISSING,
+    ) -> "Guild":
+        """
+        Create a guild.
+
+        !!! note
+            This method will only work for bots in less than 10 guilds.
+
+        ??? note "Param notes"
+            Roles:
+                - When using the `roles` parameter, the first member of the array is used to change properties of the guild's `@everyone` role. If you are trying to bootstrap a guild with additional roles, keep this in mind.
+                - When using the `roles` parameter, the required id field within each role object is an integer placeholder, and will be replaced by the API upon consumption. Its purpose is to allow you to overwrite a role's permissions in a channel when also passing in channels with the channels array.
+
+            Channels:
+                - When using the `channels` parameter, the position field is ignored, and none of the default channels are created.
+                - When using the `channels` parameter, the id field within each channel object may be set to an integer placeholder, and will be replaced by the API upon consumption. Its purpose is to allow you to create `GUILD_CATEGORY` channels by setting the `parent_id` field on any children to the category's id field. Category channels must be listed before any children.
+
+        Args:
+            name: name of the guild (2-100 characters)
+            client: The client
+            icon: An icon for the guild
+            verification_level: The guild's verification level
+            default_message_notifications: The default message notification level
+            explicit_content_filter: The guild's explicit content filter level
+            roles: An array of partial role dictionaries
+            channels: An array of partial channel dictionaries
+            afk_channel_id: id for afk channel
+            afk_timeout: afk timeout in seconds
+            system_channel_id: the id of the channel where guild notices should go
+            system_channel_flags: flags for the system channel
+
+        Returns:
+            The created guild object
+
+        """
+        data = await client.http.create_guild(
+            name=name,
+            icon=to_image_data(icon) if icon else MISSING,
+            verification_level=verification_level,
+            default_message_notifications=default_message_notifications,
+            explicit_content_filter=explicit_content_filter,
+            roles=roles,
+            channels=channels,
+            afk_channel_id=afk_channel_id,
+            afk_timeout=afk_timeout,
+            system_channel_id=system_channel_id,
+            system_channel_flags=int(system_channel_flags) if system_channel_flags else MISSING,
         )
+        return client.cache.place_guild_data(data)
 
-        if _logging := kwargs.get("logging", _logging):
-            # thx i0 for posting this on the retux Discord
+    @property
+    def channels(self) -> List["models.TYPE_GUILD_CHANNEL"]:
+        """Returns a list of channels associated with this guild."""
+        channels = [self._client.cache.get_channel(c_id) for c_id in self._channel_ids]
+        return [c for c in channels if c]
 
-            if _logging is True:
-                _logging = logging.DEBUG
+    @property
+    def threads(self) -> List["models.TYPE_THREAD_CHANNEL"]:
+        """Returns a list of threads associated with this guild."""
+        return [self._client.cache.get_channel(t_id) for t_id in self._thread_ids]
 
-            _format = (
-                "%(asctime)s [%(levelname)s] - .%(funcName)s(): %(message)s"
-                if _logging == logging.DEBUG
-                else "%(asctime)s [%(levelname)s] - %(message)s"
-            )
+    @property
+    def members(self) -> List["models.Member"]:
+        """Returns a list of all members within this guild."""
+        return [self._client.cache.get_member(self.id, m_id) for m_id in self._member_ids]
 
-            logging.basicConfig(format=_format, level=_logging)
+    @property
+    def premium_subscribers(self) -> List["models.Member"]:
+        """Returns a list of all premium subscribers"""
+        return [member for member in self.members if member.premium]
 
-        if disable_sync:
-            self._automate_sync = False
-            log.warning(
-                "Automatic synchronization has been disabled. Interactions may need to be manually synchronized."
-            )
-        else:
-            self._automate_sync = True
+    @property
+    def bots(self) -> List["models.Member"]:
+        """Returns a list of all bots within this guild"""
+        return [member for member in self.members if member.bot]
 
-    async def modify_nick_in_guild(
-        self, guild_id: Union[int, str, Snowflake, Guild], new_nick: Optional[str] = MISSING
-    ) -> Member:
-        """
-        .. versionadded:: 4.4.0
+    @property
+    def humans(self) -> List["models.Member"]:
+        """Returns a list of all humans within this guild"""
+        return [member for member in self.members if not member.bot]
 
-        Sets a new nick in the specified guild.
+    @property
+    def roles(self) -> List["models.Role"]:
+        """Returns a list of roles associated with this guild."""
+        return [self._client.cache.get_role(r_id) for r_id in self._role_ids]
 
-        :param Union[int, str, Snowflake, Guild] guild_id: The ID of the guild to modify the nick in
-        :param Optional[str] new_nick: The new nick to assign
-        """
-        if not self._http or isinstance(self._http, str):
-            raise LibraryException(
-                code=13, message="You cannot use this method until the bot has started!"
-            )
+    @property
+    def me(self) -> "models.Member":
+        """Returns this bots member object within this guild."""
+        return self._client.cache.get_member(self.id, self._client.user.id)
 
-        if new_nick is MISSING:
-            raise LibraryException(code=12, message="new nick name must either a string or `None`")
+    @property
+    def system_channel(self) -> Optional["models.GuildText"]:
+        """Returns the channel this guild uses for system messages."""
+        return self._client.cache.get_channel(self.system_channel_id)
 
-        _id = int(guild_id.id) if isinstance(guild_id, Guild) else int(guild_id)
+    @property
+    def rules_channel(self) -> Optional["models.GuildText"]:
+        """Returns the channel declared as a rules channel."""
+        return self._client.cache.get_channel(self.rules_channel_id)
 
-        return Member(
-            **await self._http.modify_self_nick_in_guild(_id, new_nick), _client=self._http
-        )
+    @property
+    def public_updates_channel(self) -> Optional["models.GuildText"]:
+        """Returns the channel where server staff receive notices from Discord."""
+        return self._client.cache.get_channel(self.public_updates_channel_id)
 
     @property
-    def guilds(self) -> List[Guild]:
-        """
-        .. versionadded:: 4.2.0
+    def emoji_limit(self) -> int:
+        """The maximum number of emoji this guild can have."""
+        base = 200 if "MORE_EMOJI" in self.features else 50
+        return max(base, PREMIUM_GUILD_LIMITS[self.premium_tier]["emoji"])
 
-        Returns a list of guilds the bot is in.
-        """
+    @property
+    def sticker_limit(self) -> int:
+        """The maximum number of stickers this guild can have."""
+        base = 60 if "MORE_STICKERS" in self.features else 0
+        return max(base, PREMIUM_GUILD_LIMITS[self.premium_tier]["stickers"])
 
-        if not self._http or isinstance(self._http, str):
-            raise LibraryException(
-                code=13, message="You cannot use this method until the bot has started!"
-            )
+    @property
+    def bitrate_limit(self) -> int:
+        """The maximum bitrate for this guild."""
+        base = 128000 if "VIP_REGIONS" in self.features else 96000
+        return max(base, PREMIUM_GUILD_LIMITS[self.premium_tier]["bitrate"])
 
-        return list(self._http.cache[Guild].values.values())
+    @property
+    def filesize_limit(self) -> int:
+        """The maximum filesize that may be uploaded within this guild."""
+        return PREMIUM_GUILD_LIMITS[self.premium_tier]["filesize"]
 
     @property
-    def latency(self) -> float:
-        """
-        .. versionadded:: 4.2.0
+    def default_role(self) -> "models.Role":
+        """The `@everyone` role in this guild."""
+        return self._client.cache.get_role(self.id)  # type: ignore
 
-        Returns the connection latency in milliseconds.
-        """
+    @property
+    def premium_subscriber_role(self) -> Optional["models.Role"]:
+        """The role given to boosters of this server, if set."""
+        return next((role for role in self.roles if role.premium_subscriber), None)
 
-        return self._websocket.latency * 1000
+    @property
+    def my_role(self) -> Optional["models.Role"]:
+        """The role associated with this client, if set."""
+        m_r_id = self._client.user.id
+        return next((role for role in self.roles if role._bot_id == m_r_id), None)
 
-    def start(self, token: Optional[str] = None) -> None:
-        """
-        Starts the client session.
+    @property
+    def permissions(self) -> Permissions:
+        """Alias for me.guild_permissions"""
+        return self.me.guild_permissions
+
+    @property
+    def voice_state(self) -> Optional["models.VoiceState"]:
+        """Get the bot's voice state for the guild."""
+        return self._client.cache.get_bot_voice_state(self.id)
 
-        :param Optional[str] token: The token of bot.
+    @property
+    def voice_states(self) -> List["models.VoiceState"]:
+        """Get a list of the active voice states in this guild."""
+        # this is *very* ick, but we cache by user_id, so we have to do it this way,
+        # alternative would be maintaining a lookup table in this guild object, which is inherently unreliable
+        # noinspection PyProtectedMember
+        return [v_state for v_state in self._client.cache.voice_state_cache.values() if v_state._guild_id == self.id]
+
+    async def fetch_member(self, member_id: Snowflake_Type) -> Optional["models.Member"]:
         """
+        Return the Member with the given discord ID, fetching from the API if necessary.
+
+        Args:
+            member_id: The ID of the member.
+
+        Returns:
+            The member object fetched. If the member is not in this guild, returns None.
 
+        """
         try:
-            self._loop.run_until_complete(self._ready(token=token))
-        except (CancelledError, Exception) as e:
-            self._loop.run_until_complete(self._logout())
-            raise e from e
-        except KeyboardInterrupt:
-            log.error("KeyboardInterrupt detected, shutting down the bot.")
-        finally:
-            self._loop.run_until_complete(self._logout())
-
-    async def __register_id_autocomplete(self) -> None:  # TODO: make this use ID and not name
-        for key in self.__id_autocomplete.keys():
-            if isinstance(key, str):  # compatibility with the decorator from the Command obj
-                for _ in self.__id_autocomplete[key]:
-                    # _ contains {"coro" : coro, "name": <name_as_string>}
-                    self.event(
-                        _["coro"],
-                        name=f"autocomplete_{key}_{_['name']}",
-                    )
-            else:
-                _command_obj = self._find_command(key)
-                _command: str = _command_obj.name
-                for _ in self.__id_autocomplete[key]:
-                    # _ contains {"coro" : coro, "name": <name_as_string>}
-                    self.event(
-                        _["coro"],
-                        name=f"autocomplete_{_command}_{_['name']}",
-                    )
-
-    @staticmethod
-    async def __compare_sync(
-        data: dict, pool: List[dict]
-    ) -> Tuple[bool, dict]:  # sourcery no-metrics
-        """
-        Compares an application command during the synchronization process.
-
-        :param dict data: The application command to compare.
-        :param List[dict] pool: The "pool" or list of commands to compare from.
-        :return: Whether the command has changed or not.
-        :rtype: bool
-        """
-
-        # sourcery skip: none-compare
-
-        attrs: List[str] = [
-            name
-            for name in ApplicationCommand.__slots__
-            if not name.startswith("_")
-            and not name.endswith("id")
-            and name not in {"version", "default_permission"}
-        ]
+            return await self._client.cache.fetch_member(self.id, member_id)
+        except NotFound:
+            return None
 
-        option_attrs: List[str] = [name for name in Option.__slots__ if not name.startswith("_")]
-        choice_attrs: List[str] = [name for name in Choice.__slots__ if not name.startswith("_")]
-        log.debug(f"Current attributes to compare: {', '.join(attrs)}.")
-        clean: bool = True
-
-        _command: dict = {}
-
-        def __check_options(command, data):
-            # sourcery skip: low-code-quality, none-compare
-            # sourcery no-metrics
-            _command_option_names = [option["name"] for option in command.get("options")]
-            _data_option_names = [option["name"] for option in data.get("options")]
-
-            if any(option not in _command_option_names for option in _data_option_names) or len(
-                _data_option_names
-            ) != len(_command_option_names):
-                return False
-
-            for option in command.get("options"):
-                for _option in data.get("options"):
-                    if _option["name"] == option["name"]:
-                        for option_attr in option_attrs:
-                            if (
-                                option.get(option_attr)
-                                and not _option.get(option_attr)
-                                or not option.get(option_attr)
-                                and _option.get(option_attr)
-                            ):
-                                return False
-                            elif option_attr == "choices":
-                                if not option.get("choices") or not _option.get("choices"):
-                                    continue
-
-                                _option_choice_names = [
-                                    choice["name"] for choice in option.get("choices")
-                                ]
-                                _data_choice_names = [
-                                    choice["name"] for choice in _option.get("choices")
-                                ]
-
-                                if any(
-                                    _ not in _option_choice_names for _ in _data_choice_names
-                                ) or len(_data_choice_names) != len(_option_choice_names):
-                                    return False
-
-                                for choice in option.get("choices"):
-                                    for _choice in _option.get("choices"):
-                                        if choice["name"] == _choice["name"]:
-                                            for choice_attr in choice_attrs:
-                                                if (
-                                                    choice.get(choice_attr)
-                                                    and not _choice.get(choice_attr)
-                                                    or not choice.get(choice_attr)
-                                                    and _choice.get(choice_attr)
-                                                ):
-                                                    return False
-                                                elif choice.get(choice_attr) != _choice.get(
-                                                    choice_attr
-                                                ):
-                                                    return False
-                                                else:
-                                                    continue
-
-                                for i, __name in enumerate(_option_choice_names):
-                                    if _data_choice_names[i] != __name:
-                                        return False
-
-                            elif option_attr == "required":
-                                if (
-                                    option.get(option_attr) == None  # noqa: E711
-                                    and _option.get(option_attr) == False  # noqa: E712
-                                ):
-                                    # API not including if False
-                                    continue
-
-                            elif option_attr == "options":
-                                if not option.get(option_attr) and not _option.get("options"):
-                                    continue
-                                _clean = __check_options(option, _option)
-                                if not _clean:
-                                    return _clean
-
-                            elif option.get(option_attr) != _option.get(option_attr):
-                                return False
-                            else:
-                                continue
-            return next(
-                (
-                    False
-                    for i, __name in enumerate(_command_option_names)
-                    if _data_option_names[i] != __name
-                ),
-                True,
-            )
+    def get_member(self, member_id: Snowflake_Type) -> Optional["models.Member"]:
+        """
+        Return the Member with the given discord ID.
 
-        for command in pool:
-            if command["name"] == data["name"]:
-                _command = command
-                # in case it continues looping
-                if not command.get("options"):
-                    command["options"] = []
-                    # this will ensure that the option will be an emtpy list, since discord returns `None`
-                    # when no options are present, but they're in the data as `[]`
-                if command.get("guild_id") and not isinstance(command.get("guild_id"), int):
-                    if isinstance(command.get("guild_id"), list):
-                        command["guild_id"] = [int(_) for _ in command["guild_id"]]
-                    else:
-                        command["guild_id"] = int(command["guild_id"])
-                    # ensure that IDs are present as integers since discord returns strings.
-                for attr in attrs:
-                    if attr == "options":
-                        if (
-                            not command.get("options")
-                            and data.get("options")
-                            or command.get("options")
-                            and not data.get("options")
-                        ):
-                            clean = False
-                            return clean, _command
-
-                        elif command.get("options") and data.get("options"):
-                            clean = __check_options(command, data)
-
-                        if not clean:
-                            return clean, _command
-
-                        else:
-                            continue
-
-                    elif attr.endswith("localizations"):
-                        if command.get(attr, None) is None and data.get(attr) == {}:
-                            # This is an API/Version difference.
-                            continue
-
-                    elif (
-                        attr == "dm_permission"
-                        and data.get(attr) == True  # noqa: E712
-                        and command.get(attr) == None  # noqa: E711
-                    ):
-                        # idk, it encountered me and synced unintentionally
-                        continue
-
-                    # elif data.get(attr, None) and command.get(attr) == data.get(attr):
-                    elif command.get(attr, None) == data.get(attr, None):
-                        # hasattr checks `dict.attr` not `dict[attr]`
-                        continue
-                    clean = False
-                    break
-
-        return clean, _command
-
-    async def _ready(self, token: Optional[str] = None) -> None:
-        """
-        Prepares the client with an internal "ready" check to ensure
-        that all conditions have been met in a chronological order:
-
-        .. code-block::
-
-            CLIENT START
-            |___ GATEWAY
-            |   |___ READY
-            |   |___ DISPATCH
-            |___ SYNCHRONIZE
-            |   |___ CACHE
-            |___ DETECT DECORATOR
-            |   |___ BUILD MODEL
-            |   |___ SYNCHRONIZE
-            |   |___ CALLBACK
-            LOOP
-
-        :param Optional[str] token: The token of bot.
-        """
-        if self._http and token and self._http is not token:
-            raise RuntimeError("You cannot pass a token to the bot twice!")
-        elif not (self._http or token):
-            raise RuntimeError("No token was passed to the bot!")
-
-        if token:
-            self._token = token
-            self._http = token
-            self._websocket._http = token  # Update the websockets token if it wasn't set before
+        Args:
+            member_id: The ID of the member
 
-        if isinstance(self._http, str):
-            self._http = HTTPClient(self._http, self._cache)
+        Returns:
+            Member object or None
 
-        data = await self._http.get_current_bot_information()
-        self.me = Application(**data, _client=self._http)
+        """
+        return self._client.cache.get_member(self.id, member_id)
 
-        ready: bool = False
-        try:
-            if self.me.flags is not None:
-                # This can be None.
-                if (
-                    self._intents.GUILD_PRESENCES in self._intents
-                    and self.me.flags.GATEWAY_PRESENCE not in self.me.flags
-                    and self.me.flags.GATEWAY_PRESENCE_LIMITED not in self.me.flags
-                ):
-                    raise RuntimeError("Client not authorised for the GUILD_PRESENCES intent.")
-                if (
-                    self._intents.GUILD_MEMBERS in self._intents
-                    and self.me.flags.GATEWAY_GUILD_MEMBERS not in self.me.flags
-                    and self.me.flags.GATEWAY_GUILD_MEMBERS_LIMITED not in self.me.flags
-                ):
-                    raise RuntimeError("Client not authorised for the GUILD_MEMBERS intent.")
-                if (
-                    self._intents.GUILD_MESSAGE_CONTENT in self._intents
-                    and self.me.flags.GATEWAY_MESSAGE_CONTENT not in self.me.flags
-                    and self.me.flags.GATEWAY_MESSAGE_CONTENT_LIMITED not in self.me.flags
-                ):
-                    log.critical("Client not authorised for the MESSAGE_CONTENT intent.")
-            elif self._intents.value != Intents.DEFAULT.value:
-                raise RuntimeError("Client not authorised for any privileged intents.")
+    async def fetch_owner(self) -> "models.Member":
+        """
+        Return the Guild owner, fetching from the API if necessary.
 
-            self.__resolve_commands()
+        Returns:
+            Member object or None
 
-            if self._automate_sync:
-                await self.__sync()
-            else:
-                await self.__get_all_commands()
-            await self.__register_id_autocomplete()
+        """
+        return await self._client.cache.fetch_member(self.id, self._owner_id)
 
-            ready = True
-        except Exception:
-            log.exception("Could not prepare the client:")
-        finally:
-            if ready:
-                log.debug("Client is now ready.")
-                await self._login()
-
-    async def _stop(self) -> None:
-        """Stops the websocket connection gracefully."""
-
-        log.debug("Shutting down the client....")
-        self._websocket.ready.clear()  # Clears ready state.
-        self._websocket._closing_lock.set()  # Toggles the "ready-to-shutdown" state for the bot.
-        # And subsequently, the processes will close itself.
+    def get_owner(self) -> "models.Member":
+        """
+        Return the Guild owner
 
-        if isinstance(self._http, HTTPClient):
-            await self._http._req._session.close()  # Closes the HTTP session associated with the client.
+        Returns:
+            Member object or None
 
-    async def _login(self) -> None:
-        """Makes a login with the Discord API."""
+        """
+        return self._client.cache.get_member(self.id, self._owner_id)
 
-        try:
-            await self._websocket.run()
-        except Exception:
-            log.exception("Websocket have raised an exception, closing.")
+    async def fetch_channels(self) -> List["models.TYPE_VOICE_CHANNEL"]:
+        """
+        Fetch this guild's channels.
 
-            if self._websocket._closing_lock.is_set():
-                # signal for closing.
+        Returns:
+            A list of channels in this guild
 
-                try:
-                    if self._websocket._task is not None:
-                        self._websocket.__heartbeat_event.set()
-                        try:
-                            # Wait for the keep-alive handler to finish so we can discard it gracefully
-                            await self._websocket._task
-                        finally:
-                            self._websocket._task = None
-                finally:  # then the overall WS client
-                    if self._websocket._client is not None:
-                        # This needs to be properly closed
-                        try:
-                            await self._websocket._client.close(code=1000)
-                        finally:
-                            self._websocket._client = None
+        """
+        data = await self._client.http.get_guild_channels(self.id)
+        return [self._client.cache.place_channel_data(channel_data) for channel_data in data]
 
-    async def wait_until_ready(self) -> None:
+    async def fetch_app_cmd_perms(self) -> dict[Snowflake_Type, "CommandPermissions"]:
         """
-        .. versionadded:: 4.2.0
+        Fetch the application command permissions for this guild.
+
+        Returns:
+            The application command permissions for this guild.
 
-        Helper method that waits until the websocket is ready.
         """
-        await self._websocket.wait_until_ready()
+        data = await self._client.http.batch_get_application_command_permissions(self._client.app.id, self.id)
+
+        for command in data:
+            command_permissions = CommandPermissions(client=self._client, command_id=command["id"], guild=self)
+            perms = [ApplicationCommandPermission.from_dict(perm, self._client) for perm in command["permissions"]]
+
+            command_permissions.update_permissions(*perms)
+
+            self.command_permissions[int(command["id"])] = command_permissions
+
+        return self.command_permissions
 
-    async def _get_all_guilds(self) -> List[dict]:
+    def is_owner(self, user: Snowflake_Type) -> bool:
         """
-        Gets all guilds that the bot is present in.
+        Whether the user is owner of the guild.
+
+        Args:
+            user: The user to check
+
+        Returns:
+            True if the user is the owner of the guild, False otherwise.
+
+        !!! note
+            the `user` argument can be any type that meets `Snowflake_Type`
 
-        :return: List of guilds
-        :rtype: List[dict]
         """
+        return self._owner_id == to_snowflake(user)
 
-        _after = None
-        _all: list = []
+    async def edit_nickname(self, new_nickname: Absent[str] = MISSING, reason: Absent[str] = MISSING) -> None:
+        """
+        Alias for me.edit_nickname
 
-        res = await self._http.get_self_guilds(limit=200)
+        Args:
+            new_nickname: The new nickname to apply
+            reason: The reason for this change
 
-        while len(res) >= 200:
-            _all.extend(res)
-            _after = int(res[-1]["id"])
+        !!! note
+            Leave `new_nickname` empty to clean user's nickname
 
-            res = await self._http.get_self_guilds(
-                after=_after,
-            )
+        """
+        await self.me.edit_nickname(new_nickname, reason=reason)
 
-        _all.extend(res)
+    async def http_chunk(self) -> None:
+        """Populates all members of this guild using the REST API."""
+        start_time = time.perf_counter()
 
-        return _all
+        iterator = MemberIterator(self)
+        async for member in iterator:
+            self._client.cache.place_member_data(self.id, member)
 
-    async def __get_all_commands(self) -> None:
-        # this method is just copied from the sync method
-        # I expect this to be changed in the sync rework
-        # until then this will deliver a cache if sync is off to make autocomplete work bug-free
-        # but even with sync off, we should cache all commands here always
-
-        _guilds = await self._get_all_guilds()
-        _guild_ids = [int(_["id"]) for _ in _guilds]
-        self._scopes.update(_guild_ids)
-        _cmds = await self._http.get_application_commands(
-            application_id=self.me.id, with_localizations=True
+        self.chunked.set()
+        self.logger.info(
+            f"Cached {iterator.total_retrieved} members for {self.id} in {time.perf_counter() - start_time:.2f} seconds"
         )
 
-        for command in _cmds:
-            if command.get("code"):
-                # Error exists.
-                raise LibraryException(command["code"], message=f'{command["message"]} |')
+    async def gateway_chunk(self, wait=True, presences=True) -> None:
+        """
+        Trigger a gateway `get_members` event, populating this object with members.
 
-        self.__global_commands = {"commands": _cmds, "clean": True}
-        # TODO: add to cache (later)
+        Args:
+            wait: Wait for chunking to be completed before continuing
+            presences: Do you need presence data for members?
+        """
+        ws = self._client.get_guild_websocket(self.id)
+        await ws.request_member_chunks(self.id, limit=0, presences=presences)
+        if wait:
+            await self.chunked.wait()
 
-        # responsible for checking if a command is in the cache but not a coro -> allowing removal
+    async def chunk(self) -> None:
+        """Populates all members of this guild using the REST API."""
+        await self.http_chunk()
 
-        for _id in _guild_ids:
-            try:
-                _cmds = await self._http.get_application_commands(
-                    application_id=self.me.id, guild_id=_id, with_localizations=True
-                )
-            except LibraryException as e:
-                if int(e.code) != 50001:
-                    raise LibraryException(code=e.code, message=e.message) from e
-
-                log.warning(
-                    f"Your bot is missing access to guild with corresponding id {_id}! "
-                    "Syncing commands will not be possible until it is invited with "
-                    "`application.commands` scope!"
-                )
-                continue
+    async def chunk_guild(self, wait=True, presences=True) -> None:
+        """
+        Trigger a gateway `get_members` event, populating this object with members.
 
-            for command in _cmds:
-                if command.get("code"):
-                    # Error exists.
-                    raise LibraryException(command["code"], message=f'{command["message"]} |')
+        !!! warning "Depreciation Warning"
+            Gateway chunking is deprecated and replaced by http chunking. Use `guild.gateway_chunk` if you need gateway chunking.
 
-            self.__guild_commands[_id] = {"commands": _cmds, "clean": True}
+        Args:
+            wait: Wait for chunking to be completed before continuing
+            presences: Do you need presence data for members?
 
-    def __resolve_commands(self) -> None:  # sourcery skip: low-code-quality
         """
-        Resolves all commands to the command coroutines.
+        warn(
+            "Gateway chunking is deprecated and replaced by http chunking. Use `guild.gateway_chunk` if you need gateway chunking.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        await self.gateway_chunk(wait=wait, presences=presences)
 
-        .. warning::
-            This is an internal method. Do not call it unless you know what you are doing!
+    async def process_member_chunk(self, chunk: dict) -> None:
         """
-        for cmd in self._commands:
-            if cmd.coro.__qualname__ in [_cmd.__qualname__ for _cmd in self.__command_coroutines]:
-                continue
+        Receive and either cache or process the chunks of members from gateway.
 
-            cmd.listener = self._websocket._dispatch
+        Args:
+            chunk: A member chunk from discord
 
-            if cmd.default_scope and self._default_scope:
-                if isinstance(cmd.scope, list):
-                    cmd.scope.extend(self._default_scope)
-                else:
-                    cmd.scope = self._default_scope
+        """
+        if self.chunked.is_set():
+            self.chunked.clear()
 
-            data: Union[dict, List[dict]] = cmd.full_data
-            coro = cmd.dispatcher
+        if presences := chunk.get("presences"):
+            # combine the presence dict into the members dict
+            for presence in presences:
+                u_id = presence["user"]["id"]
+                # find the user this presence is for
+                member_index = next(
+                    (index for (index, d) in enumerate(chunk.get("members")) if d["user"]["id"] == u_id),
+                    None,
+                )
+                del presence["user"]
+                chunk["members"][member_index]["user"] = chunk["members"][member_index]["user"] | presence
 
-            self.__check_command(
-                command=ApplicationCommand(**(data[0] if isinstance(data, list) else data)),
-                coro=coro,
-            )
+        self._chunk_cache = self._chunk_cache + chunk.get("members") if self._chunk_cache else chunk.get("members")
+        if chunk.get("chunk_index") != chunk.get("chunk_count") - 1:
+            return self.logger.debug(f"Cached chunk of {len(chunk.get('members'))} members for {self.id}")
+        members = self._chunk_cache
+        self.logger.info(f"Processing {len(members)} members for {self.id}")
+
+        s = time.monotonic()
+        start_time = time.perf_counter()
+
+        for member in members:
+            self._client.cache.place_member_data(self.id, member)
+            if (time.monotonic() - s) > 0.05:
+                # look, i get this *could* be a thread, but because it needs to modify data in the main thread,
+                # it is still blocking. So by periodically yielding to the event loop, we can avoid blocking, and still
+                # process this data properly
+                await asyncio.sleep(0)
+                s = time.monotonic()
+
+        total_time = time.perf_counter() - start_time
+        self.chunk_cache = []
+        self.logger.info(f"Cached members for {self.id} in {total_time:.2f} seconds")
+        self.chunked.set()
 
-            if cmd.autocompletions:
-                self.__id_autocomplete.update(cmd.autocompletions)
+    async def fetch_audit_log(
+        self,
+        user_id: Optional["Snowflake_Type"] = MISSING,
+        action_type: Optional["AuditLogEventType"] = MISSING,
+        before: Optional["Snowflake_Type"] = MISSING,
+        after: Optional["Snowflake_Type"] = MISSING,
+        limit: int = 100,
+    ) -> "AuditLog":
+        """
+        Fetch section of the audit log for this guild.
+
+        Args:
+            user_id: The ID of the user to filter by
+            action_type: The type of action to filter by
+            before: The ID of the entry to start at
+            after: The ID of the entry to end at
+            limit: The number of entries to return
 
-            coro = coro.__func__ if hasattr(coro, "__func__") else coro
+        Returns:
+            An AuditLog object
 
-            coro._command_data = data
-            coro._name = cmd.name
-            coro._converters = cmd.converters
-
-            if (data["name"] if isinstance(data, dict) else data[0]["name"]) not in (
-                (
-                    c._command_data["name"]
-                    if isinstance(c._command_data, dict)
-                    else c._command_data[0]["name"]
-                )
-                for c in self.__command_coroutines
-            ):
-                self.__command_coroutines.append(coro)
+        """
+        data = await self._client.http.get_audit_log(self.id, user_id, action_type, before, after, limit)
+        return AuditLog.from_dict(data, self._client)
 
-            if cmd.scope not in (MISSING, None):
-                if isinstance(cmd.scope, List):
-                    [self._scopes.add(_ if isinstance(_, int) else _.id) for _ in cmd.scope]
-                else:
-                    self._scopes.add(cmd.scope if isinstance(cmd.scope, int) else cmd.scope.id)
+    def audit_log_history(
+        self,
+        user_id: Optional["Snowflake_Type"] = MISSING,
+        action_type: Optional["AuditLogEventType"] = MISSING,
+        before: Optional["Snowflake_Type"] = MISSING,
+        after: Optional["Snowflake_Type"] = MISSING,
+        limit: int = 100,
+    ) -> "AuditLogHistory":
+        """
+        Get an async iterator for the history of the audit log.
+
+        Args:
+            user_id (:class:`Snowflake_Type`): The user ID to search for.
+            action_type (:class:`AuditLogEventType`): The action type to search for.
+            before: get entries before this message ID
+            after: get entries after this message ID
+            limit: The maximum number of entries to return (set to 0 for no limit)
+
+        ??? Hint "Example Usage:"
+            ```python
+            async for entry in guild.audit_log_history(limit=0):
+                entry: "AuditLogEntry"
+                if entry.changes:
+                    # ...
+            ```
+            or
+            ```python
+            history = guild.audit_log_history(limit=250)
+            # Flatten the async iterator into a list
+            entries = await history.flatten()
+            ```
 
-            self.event(coro, name=f"command_{cmd.name}")
+        Returns:
+            AuditLogHistory (AsyncIterator)
 
-    async def __sync(self) -> None:  # sourcery no-metrics
         """
-        Synchronizes all commands to the API.
+        return AuditLogHistory(self, user_id, action_type, before, after, limit)
 
-        .. warning::
-            This is an internal method. Do not call it unless you know what you are doing!
+    async def edit(
+        self,
+        *,
+        name: Absent[Optional[str]] = MISSING,
+        description: Absent[Optional[str]] = MISSING,
+        verification_level: Absent[Optional["VerificationLevel"]] = MISSING,
+        default_message_notifications: Absent[Optional["DefaultNotificationLevel"]] = MISSING,
+        explicit_content_filter: Absent[Optional["ExplicitContentFilterLevel"]] = MISSING,
+        afk_channel: Absent[Optional[Union["models.GuildVoice", Snowflake_Type]]] = MISSING,
+        afk_timeout: Absent[Optional[int]] = MISSING,
+        system_channel: Absent[Optional[Union["models.GuildText", Snowflake_Type]]] = MISSING,
+        system_channel_flags: Absent[Union[SystemChannelFlags, int]] = MISSING,
+        owner: Absent[Optional[Union["models.Member", Snowflake_Type]]] = MISSING,
+        icon: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        splash: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        discovery_splash: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        banner: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        rules_channel: Absent[Optional[Union["models.GuildText", Snowflake_Type]]] = MISSING,
+        public_updates_channel: Absent[Optional[Union["models.GuildText", Snowflake_Type]]] = MISSING,
+        preferred_locale: Absent[Optional[str]] = MISSING,
+        premium_progress_bar_enabled: Absent[Optional[bool]] = False,
+        # ToDo: Fill in guild features. No idea how this works - https://discord.com/developers/docs/resources/guild#guild-object-guild-features
+        features: Absent[Optional[list[str]]] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> None:
         """
-        # sourcery skip: low-code-quality
+        Edit the guild.
 
-        log.debug("starting command sync")
-        _guilds = await self._get_all_guilds()
-        _guild_ids = [int(_["id"]) for _ in _guilds]
-        self._scopes.update(_guild_ids)
-        _cmds = await self._http.get_application_commands(
-            application_id=self.me.id, with_localizations=True
+        Args:
+            name: The new name of the guild.
+            description: The new description of the guild.
+            verification_level: The new verification level for the guild.
+            default_message_notifications: The new notification level for the guild.
+            explicit_content_filter: The new explicit content filter level for the guild.
+            afk_channel: The voice channel that should be the new AFK channel.
+            afk_timeout: How many seconds does a member need to be afk before they get moved to the AFK channel. Must be either `60`, `300`, `900`, `1800` or `3600`, otherwise HTTPException will be raised.
+            icon: The new icon. Requires a bytes like object or a path to an image.
+            owner: The new owner of the guild. You, the bot, need to be owner for this to work.
+            splash: The new invite splash image. Requires a bytes like object or a path to an image.
+            discovery_splash: The new discovery image. Requires a bytes like object or a path to an image.
+            banner: The new banner image. Requires a bytes like object or a path to an image.
+            system_channel: The text channel where new system messages should appear. This includes boosts and welcome messages.
+            system_channel_flags: The new settings for the system channel.
+            rules_channel: The text channel where your rules and community guidelines are displayed.
+            public_updates_channel: The text channel where updates from discord should appear.
+            preferred_locale: The new preferred locale of the guild. Must be an ISO 639 code.
+            premium_progress_bar_enabled: The status of the Nitro boost bar.
+            features: The enabled guild features
+            reason: An optional reason for the audit log.
+
+        """
+        await self._client.http.modify_guild(
+            guild_id=self.id,
+            name=name,
+            description=description,
+            verification_level=int(verification_level) if verification_level else MISSING,
+            default_message_notifications=int(default_message_notifications)
+            if default_message_notifications
+            else MISSING,
+            explicit_content_filter=int(explicit_content_filter) if explicit_content_filter else MISSING,
+            afk_channel_id=to_snowflake(afk_channel) if afk_channel else MISSING,
+            afk_timeout=afk_timeout,
+            icon=to_image_data(icon) if icon else MISSING,
+            owner_id=to_snowflake(owner) if owner else MISSING,
+            splash=to_image_data(splash) if splash else MISSING,
+            discovery_splash=to_image_data(discovery_splash) if discovery_splash else MISSING,
+            banner=to_image_data(banner) if banner else MISSING,
+            system_channel_id=to_snowflake(system_channel) if system_channel else MISSING,
+            system_channel_flags=int(system_channel_flags) if system_channel_flags else MISSING,
+            rules_channel_id=to_snowflake(rules_channel) if rules_channel else MISSING,
+            public_updates_channel_id=to_snowflake(public_updates_channel) if public_updates_channel else MISSING,
+            preferred_locale=preferred_locale,
+            premium_progress_bar_enabled=premium_progress_bar_enabled if premium_progress_bar_enabled else False,
+            features=features,
+            reason=reason,
         )
 
-        for command in _cmds:
-            if command.get("code"):
-                # Error exists.
-                raise LibraryException(command["code"], message=f'{command["message"]} |')
-
-        self.__global_commands = {"commands": _cmds, "clean": True}
-        # TODO: add to cache (later)
+    async def create_custom_emoji(
+        self,
+        name: str,
+        imagefile: UPLOADABLE_TYPE,
+        roles: Absent[List[Union[Snowflake_Type, "models.Role"]]] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.CustomEmoji":
+        """
+        Create a new custom emoji for the guild.
 
-        __check_global_commands: List[str] = [cmd["name"] for cmd in _cmds]
-        __check_guild_commands: Dict[int, List[str]] = {}
-        __blocked_guilds: set = set()
+        Args:
+            name: Name of the emoji
+            imagefile: The emoji image. (Supports PNG, JPEG, WebP, GIF)
+            roles: Roles allowed to use this emoji.
+            reason: An optional reason for the audit log.
 
-        # responsible for checking if a command is in the cache but not a coro -> allowing removal
+        Returns:
+            The new custom emoji created.
 
-        for _id in _guild_ids.copy():
-            try:
-                _cmds = await self._http.get_application_commands(
-                    application_id=self.me.id, guild_id=_id, with_localizations=True
-                )
-            except LibraryException as e:
-                if int(e.code) != 50001:
-                    raise LibraryException(code=e.code, message=e.message) from e
-
-                log.warning(
-                    f"Your bot is missing access to guild with corresponding id {_id}! "
-                    "Adding commands will not be possible until it is invited with "
-                    "`application.commands` scope!"
-                )
-                __blocked_guilds.add(_id)
-                _guild_ids.remove(_id)
-                continue
-
-            self.__guild_commands[_id] = {"commands": _cmds, "clean": True}
-            __check_guild_commands[_id] = [cmd["name"] for cmd in _cmds] if _cmds else []
-
-        for coro in self.__command_coroutines:
-            if hasattr(coro, "_command_data"):  # just so IDE knows it exists
-                if isinstance(coro._command_data, list):
-                    _guild_command: dict
-                    for _guild_command in coro._command_data:
-                        _guild_id = int(_guild_command.get("guild_id"))
-                        if _guild_id in __blocked_guilds:
-                            log.fatal(f"Cannot sync commands on guild with id {_guild_id}!")
-                            raise LibraryException(50001, message="Missing Access |")
-                        if _guild_id not in _guild_ids:
-                            log.warning(f"The bot is not in guild with id {_guild_id}")
-                            continue
-                        if _guild_command["name"] not in __check_guild_commands[_guild_id]:
-                            self.__guild_commands[_guild_id]["clean"] = False
-                            self.__guild_commands[_guild_id]["commands"].append(_guild_command)
-
-                        else:
-                            clean, _command = await self.__compare_sync(
-                                _guild_command, self.__guild_commands[_guild_id]["commands"]
-                            )
-                            if not clean:
-                                self.__guild_commands[_guild_id]["clean"] = False
-                                # _pos = self.__guild_commands[_guild_id]["commands"].index(_command)
-                                # self.__guild_commands[_guild_id]["commands"][_pos] = _guild_command
-
-                                for _pos, _dict in enumerate(
-                                    self.__guild_commands[_guild_id]["commands"]
-                                ):
-                                    if _dict["name"] == _command["name"]:
-                                        self.__guild_commands[_guild_id]["commands"][
-                                            _pos
-                                        ] = _guild_command
-                                        break
-
-                            if __check_guild_commands[_guild_id]:
-                                del __check_guild_commands[_guild_id][
-                                    __check_guild_commands[_guild_id].index(_guild_command["name"])
-                                ]
-
-                elif coro._command_data["name"] in __check_global_commands:  # noqa
-                    clean, _command = await self.__compare_sync(
-                        coro._command_data, self.__global_commands["commands"]
-                    )
-
-                    if not clean:
-                        self.__global_commands["clean"] = False
-                        # _pos = self.__global_commands["commands"].index(_command)
-                        # self.__global_commands["commands"][_pos] = coro._command_data
-
-                        for _pos, _dict in enumerate(self.__global_commands["commands"]):
-                            if _dict["name"] == _command["name"]:
-                                self.__global_commands["commands"][_pos] = coro._command_data
-                                break
-
-                    if __check_global_commands:
-                        del __check_global_commands[
-                            __check_global_commands.index(coro._command_data["name"])  # noqa
-                        ]
-
-                else:
-                    self.__global_commands["clean"] = False
-                    self.__global_commands["commands"].append(coro._command_data)
-
-        if not self.__command_coroutines:
-            if self.__global_commands["commands"]:
-                self.__global_commands["clean"] = False
-                self.__global_commands["commands"] = []
-                __check_global_commands = []
-            for _id in _guild_ids:
-                if self.__guild_commands[_id]["commands"]:
-                    __check_guild_commands[_id] = []
-                    self.__guild_commands[_id]["clean"] = False
-                    self.__guild_commands[_id]["commands"] = []
-
-        if __check_global_commands:
-            # names are present but not found in registered global command coroutines. Deleting.
-            self.__global_commands["clean"] = False
-            for name in __check_global_commands:
-                _pos = self.__global_commands["commands"].index(
-                    [_ for _ in self.__global_commands["commands"] if _["name"] == name][0]
-                )
-                del self.__global_commands["commands"][_pos]
+        """
+        data_payload = {
+            "name": name,
+            "image": to_image_data(imagefile),
+            "roles": to_snowflake_list(roles) if roles else MISSING,
+        }
 
-        for _id in _guild_ids:
-            if __check_guild_commands[_id]:
-                self.__guild_commands[_id]["clean"] = False
-                for name in __check_guild_commands[_id]:
-                    _pos = self.__guild_commands[_id]["commands"].index(
-                        [_ for _ in self.__guild_commands[_id]["commands"] if _["name"] == name][0]
-                    )
-                    del self.__guild_commands[_id]["commands"][_pos]
-
-        if not self.__global_commands["clean"] or any(
-            not self.__guild_commands[_id]["clean"] for _id in _guild_ids
-        ):
-            if not self.__global_commands["clean"]:
-                res = await self._http.overwrite_application_command(
-                    application_id=int(self.me.id), data=self.__global_commands["commands"]
-                )
-                self.__global_commands["clean"] = True
-                self.__global_commands["commands"] = res
+        emoji_data = await self._client.http.create_guild_emoji(data_payload, self.id, reason=reason)
+        return self._client.cache.place_emoji_data(self.id, emoji_data)
 
-            for _id in _guild_ids:
-                if not self.__guild_commands[_id]["clean"]:
-                    res = await self._http.overwrite_application_command(
-                        application_id=int(self.me.id),
-                        data=self.__guild_commands[_id]["commands"],
-                        guild_id=_id,
-                    )
-                    self.__guild_commands[_id]["clean"] = True
-                    self.__guild_commands[_id]["commands"] = res
-
-    def event(
-        self, coro: Optional[Callable[..., Coroutine]] = MISSING, *, name: Optional[str] = MISSING
-    ) -> Callable[..., Any]:
-        """
-        A decorator for listening to events dispatched from the
-        Gateway.
-
-        Documentation on how to listen to specific events can be found :ref:`here<events:Event Documentation>`.
-
-        :param Optional[Callable[..., Coroutine]] coro: The coroutine of the event.
-        :param Optional[str] name: The name of the event. If not given, this defaults to the coroutine's name.
-        :return: A callable response.
-        :rtype: Callable[..., Any]
-        """
-
-        def decorator(coro: Optional[Callable[..., Coroutine]]):
-            self._websocket._dispatch.register(
-                coro, name=name if name is not MISSING else coro.__name__
-            )
-            return coro
+    async def create_guild_template(self, name: str, description: Absent[str] = MISSING) -> "models.GuildTemplate":
+        """
+        Create a new guild template based on this guild.
 
-        if coro is not MISSING:
-            self._websocket._dispatch.register(
-                coro, name=name if name is not MISSING else coro.__name__
-            )
-            return coro
+        Args:
+            name: The name of the template (1-100 characters)
+            description: The description for the template (0-120 characters)
 
-        return decorator
+        Returns:
+            The new guild template created.
 
-    async def change_presence(self, presence: ClientPresence) -> None:
         """
-        .. versionadded:: 4.2.0
+        template = await self._client.http.create_guild_template(self.id, name, description)
+        return GuildTemplate.from_dict(template, self._client)
 
-        A method that changes the current client's presence on runtime.
+    async def fetch_guild_templates(self) -> List["models.GuildTemplate"]:
+        """
+        Fetch all guild templates for this guild.
 
-        .. note::
-            There is a ratelimit to using this method (5 per minute).
-            As there's no gateway ratelimiter yet, breaking this ratelimit
-            will force your bot to disconnect.
+        Returns:
+            A list of guild template objects.
 
-        :param ClientPresence presence: The presence to change the bot to on identify.
         """
-        await self._websocket._update_presence(presence)
+        templates = await self._client.http.get_guild_templates(self.id)
+        return GuildTemplate.from_list(templates, self._client)
 
-    def __check_command(
-        self,
-        command: ApplicationCommand,
-        coro: Callable[..., Coroutine],
-        regex: str = r"^[a-z0-9_-]{1,32}$",
-    ) -> None:  # sourcery no-metrics
-        """
-        Checks if a command is valid.
+    async def fetch_all_custom_emojis(self) -> List["models.CustomEmoji"]:
         """
-        reg = re.compile(regex)
-        _options_names: List[str] = []
-        _sub_groups_present: bool = False
-        _sub_cmds_present: bool = False
+        Gets all the custom emoji present for this guild.
 
-        def __check_sub_group(_sub_group: Option):
-            nonlocal _sub_groups_present
-            _sub_groups_present = True
-            if _sub_group.name is MISSING:
-                raise LibraryException(11, message="Sub command groups must have a name.")
-            __indent = 4
-            log.debug(
-                f"{' ' * __indent}checking sub command group '{_sub_group.name}' of command '{command.name}'"
-            )
-            if not re.fullmatch(reg, _sub_group.name):
-                raise LibraryException(
-                    11,
-                    message=f"The sub command group name does not match the regex for valid names ('{regex}')",
-                )
-            elif _sub_group.description is MISSING and not _sub_group.description:
-                raise LibraryException(11, message="A description is required.")
-            elif len(_sub_group.description) > 100:
-                raise LibraryException(11, message="Descriptions must be less than 100 characters.")
-
-            if not _sub_group.options:
-                raise LibraryException(11, message="sub command groups must have subcommands!")
-            if len(_sub_group.options) > 25:
-                raise LibraryException(
-                    11, message="A sub command group cannot contain more than 25 sub commands!"
-                )
-            for _sub_command in _sub_group.options:
-                __check_sub_command(_sub_command, _sub_group)
+        Returns:
+            A list of custom emoji objects.
 
-        def __check_sub_command(_sub_command: Option, _sub_group: Option = MISSING):
-            nonlocal _sub_cmds_present
-            _sub_cmds_present = True
-            if _sub_command.name is MISSING:
-                raise LibraryException(11, message="sub commands must have a name!")
-            if _sub_group is not MISSING:
-                __indent = 8
-                log.debug(
-                    f"{' ' * __indent}checking sub command '{_sub_command.name}' of group '{_sub_group.name}'"
-                )
-            else:
-                __indent = 4
-                log.debug(
-                    f"{' ' * __indent}checking sub command '{_sub_command.name}' of command '{command.name}'"
-                )
-            if not re.fullmatch(reg, _sub_command.name):
-                raise LibraryException(
-                    11,
-                    message=f"The sub command name does not match the regex for valid names ('{reg}')",
-                )
-            elif _sub_command.description is MISSING or not _sub_command.description:
-                raise LibraryException(11, message="A description is required.")
-            elif len(_sub_command.description) > 100:
-                raise LibraryException(11, message="Descriptions must be less than 100 characters.")
-
-            if _sub_command.options is not MISSING and _sub_command.options:
-                if len(_sub_command.options) > 25:
-                    raise LibraryException(
-                        11, message="Your sub command must have less than 25 options."
-                    )
-                _sub_opt_names = []
-                for _opt in _sub_command.options:
-                    __check_options(_opt, _sub_opt_names, _sub_command)
-                del _sub_opt_names
-
-        def __check_options(_option: Option, _names: list, _sub_command: Option = MISSING):
-            nonlocal _options_names
-            if getattr(_option, "autocomplete", False) and getattr(_option, "choices", False):
-                log.warning("Autocomplete may not be set to true if choices are present.")
-            if _option.name is MISSING:
-                raise LibraryException(11, message="Options must have a name.")
-            if _sub_command is not MISSING:
-                __indent = 12 if _sub_groups_present else 8
-                log.debug(
-                    f"{' ' * __indent}checking option '{_option.name}' of sub command '{_sub_command.name}'"
-                )
-            else:
-                __indent = 4
-                log.debug(
-                    f"{' ' * __indent}checking option '{_option.name}' of command '{command.name}'"
-                )
-            _options_names.append(_option.name)
-            if not re.fullmatch(reg, _option.name):
-                raise LibraryException(
-                    11,
-                    message=f"The option name ('{_option.name}') does not match the regex for valid names ('{regex}').",
-                )
-            if _option.description is MISSING or not _option.description:
-                raise LibraryException(
-                    11,
-                    message="A description is required.",
-                )
-            elif len(_option.description) > 100:
-                raise LibraryException(
-                    11,
-                    message="Descriptions must be less than 100 characters.",
-                )
-            if _option.name in _names:
-                raise LibraryException(
-                    11, message="You must not have two options with the same name in a command!"
-                )
-            _names.append(_option.name)
+        """
+        emojis_data = await self._client.http.get_all_guild_emoji(self.id)
+        return [self._client.cache.place_emoji_data(self.id, emoji_data) for emoji_data in emojis_data]
 
-        def __check_coro():
-            __indent = 4
-            log.debug(f"{' ' * __indent}Checking coroutine: '{coro.__name__}'")
-            _ismethod = hasattr(coro, "__func__")
-            if not len(coro.__code__.co_varnames) ^ (
-                _ismethod and len(coro.__code__.co_varnames) == 1
-            ):
-                raise LibraryException(
-                    11, message="Your command needs at least one argument to return context."
-                )
-            elif "kwargs" in coro.__code__.co_varnames:
-                return
-            elif _sub_cmds_present and len(coro.__code__.co_varnames) < (3 if _ismethod else 2):
-                raise LibraryException(
-                    11, message="Your command needs one argument for the sub_command."
-                )
-            elif _sub_groups_present and len(coro.__code__.co_varnames) < (4 if _ismethod else 3):
-                raise LibraryException(
-                    11,
-                    message="Your command needs one argument for the sub_command and one for the sub_command_group.",
-                )
-            add: int = (
-                1 + abs(_sub_cmds_present) + abs(_sub_groups_present) + 1 if _ismethod else +0
-            )
+    async def fetch_custom_emoji(self, emoji_id: Snowflake_Type) -> Optional["models.CustomEmoji"]:
+        """
+        Fetches the custom emoji present for this guild, based on the emoji id.
 
-            if len(coro.__code__.co_varnames) - add < len(set(_options_names)):
-                log.debug(
-                    "Coroutine is missing arguments for options:"
-                    f" {[_arg for _arg in _options_names if _arg not in coro.__code__.co_varnames]}"
-                )
-                raise LibraryException(
-                    11, message="You need one argument for every option name in your command!"
-                )
+        Args:
+            emoji_id: The target emoji to get data of.
 
-        if command.name is MISSING:
-            raise LibraryException(11, message="Your command must have a name.")
+        Returns:
+            The custom emoji object. If the emoji is not found, returns None.
 
-        else:
-            log.debug(f"checking command '{command.name}':")
-        if (
-            not re.fullmatch(reg, command.name)
-            and command.type == ApplicationCommandType.CHAT_INPUT
-        ):
-            raise LibraryException(
-                11,
-                message=f"Your command name ('{command.name}') does not match the regex for valid names ('{regex}').",
-            )
-        elif command.type == ApplicationCommandType.CHAT_INPUT and (
-            command.description is MISSING or not command.description
-        ):
-            raise LibraryException(11, message="A description is required.")
-        elif command.type != ApplicationCommandType.CHAT_INPUT and (
-            command.description is not MISSING and command.description
-        ):
-            raise LibraryException(11, message="Only chat-input commands can have a description.")
-
-        elif command.description is not MISSING and len(command.description) > 100:
-            raise LibraryException(11, message="Descriptions must be less than 100 characters.")
-
-        if command.options and command.options is not MISSING:
-            if len(command.options) > 25:
-                raise LibraryException(11, message="Your command must have less than 25 options.")
-
-            if command.type != ApplicationCommandType.CHAT_INPUT:
-                raise LibraryException(
-                    11, message="Only CHAT_INPUT commands can have options/sub-commands!"
-                )
+        """
+        try:
+            return await self._client.cache.fetch_emoji(self.id, emoji_id)
+        except NotFound:
+            return None
 
-            _opt_names = []
-            for _option in command.options:
-                if _option.type == OptionType.SUB_COMMAND_GROUP:
-                    __check_sub_group(_option)
+    def get_custom_emoji(self, emoji_id: Snowflake_Type) -> Optional["models.CustomEmoji"]:
+        """
+        Gets the custom emoji present for this guild, based on the emoji id.
 
-                elif _option.type == OptionType.SUB_COMMAND:
-                    __check_sub_command(_option)
+        Args:
+            emoji_id: The target emoji to get data of.
 
-                else:
-                    __check_options(_option, _opt_names)
-            del _opt_names
+        Returns:
+            The custom emoji object.
 
-        __check_coro()
+        """
+        emoji_id = to_snowflake(emoji_id)
+        emoji = self._client.cache.get_emoji(emoji_id)
+        return emoji if emoji and emoji._guild_id == self.id else None
 
-    def command(
+    async def create_channel(
         self,
-        *,
-        type: Optional[Union[int, ApplicationCommandType]] = ApplicationCommandType.CHAT_INPUT,
-        name: Optional[str] = MISSING,
-        description: Optional[str] = MISSING,
-        scope: Optional[Union[int, Guild, List[int], List[Guild]]] = MISSING,
-        options: Optional[
-            Union[Dict[str, Any], List[Dict[str, Any]], Option, List[Option]]
+        channel_type: Union[ChannelType, int],
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
         ] = MISSING,
-        name_localizations: Optional[Dict[Union[str, Locale], str]] = MISSING,
-        description_localizations: Optional[Dict[Union[str, Locale], str]] = MISSING,
-        default_member_permissions: Optional[Union[int, Permissions]] = MISSING,
-        dm_permission: Optional[bool] = MISSING,
-        nsfw: Optional[bool] = MISSING,
-        default_scope: bool = True,
-    ) -> Callable[[Callable[..., Coroutine]], Command]:
-        """
-        A decorator for registering an application command to the Discord API,
-        as well as being able to listen for ``INTERACTION_CREATE`` dispatched
-        gateway events.
-
-        The structure of a chat-input command:
-
-        .. code-block:: python
-
-            @bot.command(name="command-name", description="this is a command.")
-            async def command_name(ctx):
-                ...
-
-        The ``scope`` kwarg field may also be used to designate the command in question
-        applicable to a guild or set of guilds.
-
-        To properly utilise the ``default_member_permissions`` kwarg, it requires OR'ing the permission values, similar to instantiating the client with Intents.
-        For example:
-
-        .. code-block:: python
-
-            @bot.command(name="kick", description="Kick a user.", default_member_permissions=interactions.Permissions.BAN_MEMBERS | interactions.Permissions.KICK_MEMBERS)
-            async def kick(ctx, user: interactions.Member):
-                ...
-
-        Another example below for instance is an admin-only command:
-
-        .. code-block:: python
-
-            @bot.command(name="sudo", description="this is an admin-only command.", default_member_permissions=interactions.Permissions.ADMINISTRATOR)
-            async def sudo(ctx):
-                ...
-
-        .. note::
-            If ``default_member_permissions`` is not given, this will default to anyone that is able to use the command.
-
-        :param Optional[Union[str, int, ApplicationCommandType]] type: The type of application command. Defaults to :attr:`.ApplicationCommandType.CHAT_INPUT`.
-        :param Optional[str] name: The name of the application command. This *is* required but kept optional to follow kwarg rules.
-        :param Optional[str] description: The description of the application command. This should be left blank if you are not using ``CHAT_INPUT``.
-        :param Optional[Union[int, Guild, List[int], List[Guild]]] scope: The "scope"/applicable guilds the application command applies to.
-        :param Optional[Union[Dict[str, Any], List[Dict[str, Any]], Option, List[Option]]] options: The "arguments"/options of an application command. This should be left blank if you are not using ``CHAT_INPUT``.
-        :param Optional[Dict[Union[str, Locale], str]] name_localizations:
-            .. versionadded:: 4.2.0
-
-            The dictionary of localization for the ``name`` field. This enforces the same restrictions as the ``name`` field.
-        :param Optional[Dict[Union[str, Locale], str]] description_localizations:
-            .. versionadded:: 4.2.0
-
-            The dictionary of localization for the ``description`` field. This enforces the same restrictions as the ``description`` field.
-        :param Optional[Union[int, Permissions]] default_member_permissions: The permissions bit value of :class:`.Permissions`. If not given, defaults to :attr:`.Permissions.USE_APPLICATION_COMMANDS`
-        :param Optional[bool] dm_permission: The application permissions if executed in a Direct Message. Defaults to ``True``.
-        :param Optional[bool] nsfw:
-            .. versionadded:: 4.4.0
-
-            Indicates whether the command is age-restricted. Defaults to ``False``
-        :param Optional[bool] default_scope:
-            .. versionadded:: 4.3.0
-
-            Whether the scope of the command is the default scope set in the client. Defaults to ``True``.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Command]
-        """
-
-        def decorator(coro: Callable[..., Coroutine]) -> Command:
-            cmd = Command(
-                coro=coro,
-                type=type,
-                name=name,
-                description=description,
-                options=options,
-                scope=scope,
-                default_member_permissions=default_member_permissions,
-                dm_permission=dm_permission,
-                nsfw=nsfw,
-                name_localizations=name_localizations,
-                description_localizations=description_localizations,
-                default_scope=default_scope,
-            )
-            cmd.client = self
-            self._commands.append(cmd)
-            return cmd
+        category: Union[Snowflake_Type, "models.GuildCategory"] = None,
+        nsfw: bool = False,
+        bitrate: int = 64000,
+        user_limit: int = 0,
+        rate_limit_per_user: int = 0,
+        reason: Absent[Optional[str]] = MISSING,
+        **kwargs: dict,
+    ) -> "models.TYPE_GUILD_CHANNEL":
+        """
+        Create a guild channel, allows for explicit channel type setting.
+
+        Args:
+            channel_type: The type of channel to create
+            name: The name of the channel
+            topic: The topic of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            category: The category this channel should be within
+            nsfw: Should this channel be marked nsfw
+            bitrate: The bitrate of this channel, only for voice
+            user_limit: The max users that can be in this channel, only for voice
+            rate_limit_per_user: The time users must wait between sending messages
+            reason: The reason for creating this channel
+            kwargs: Additional keyword arguments to pass to the channel creation
+
+        Returns:
+            The newly created channel.
+
+        """
+        channel_data = await self._client.http.create_guild_channel(
+            self.id,
+            name,
+            channel_type,
+            topic,
+            position,
+            models.process_permission_overwrites(permission_overwrites),
+            to_optional_snowflake(category),
+            nsfw,
+            bitrate,
+            user_limit,
+            rate_limit_per_user,
+            reason,
+            **kwargs,
+        )
+        return self._client.cache.place_channel_data(channel_data)
 
-        return decorator
+    async def create_text_channel(
+        self,
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        category: Union[Snowflake_Type, "models.GuildCategory"] = None,
+        nsfw: bool = False,
+        rate_limit_per_user: int = 0,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildText":
+        """
+        Create a text channel in this guild.
+
+        Args:
+            name: The name of the channel
+            topic: The topic of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            category: The category this channel should be within
+            nsfw: Should this channel be marked nsfw
+            rate_limit_per_user: The time users must wait between sending messages
+            reason: The reason for creating this channel
+
+        Returns:
+           The newly created text channel.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_TEXT,
+            name=name,
+            topic=topic,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            category=category,
+            nsfw=nsfw,
+            rate_limit_per_user=rate_limit_per_user,
+            reason=reason,
+        )
 
-    def message_command(
+    async def create_forum_channel(
         self,
-        *,
-        name: Optional[str] = MISSING,
-        scope: Optional[Union[int, Guild, List[int], List[Guild]]] = MISSING,
-        name_localizations: Optional[Dict[Union[str, Locale], Any]] = MISSING,
-        default_member_permissions: Optional[Union[int, Permissions]] = MISSING,
-        dm_permission: Optional[bool] = MISSING,
-        nsfw: Optional[bool] = MISSING,
-        default_scope: bool = True,
-    ) -> Callable[[Callable[..., Coroutine]], Command]:
-        """
-        A decorator for registering a message context menu to the Discord API,
-        as well as being able to listen for ``INTERACTION_CREATE`` dispatched
-        gateway events.
-
-        The structure of a message context menu:
-
-        .. code-block:: python
-
-            @bot.message_command(name="Context menu name")
-            async def context_menu_name(ctx):
-                ...
-
-        The ``scope`` kwarg field may also be used to designate the command in question
-        applicable to a guild or set of guilds.
-
-        :param Optional[str] name: The name of the application command.
-        :param Optional[Union[int, Guild, List[int], List[Guild]]] scope: The "scope"/applicable guilds the application command applies to. Defaults to ``None``.
-        :param Optional[Dict[Union[str, Locale], str]] name_localizations:
-            .. versionadded:: 4.2.0
-
-            The dictionary of localization for the ``name`` field. This enforces the same restrictions as the ``name`` field.
-        :param Optional[Union[int, Permissions]] default_member_permissions: The permissions bit value of :class:`.Permissions`. If not given, defaults to :attr:`.Permissions.USE_APPLICATION_COMMANDS`
-        :param Optional[bool] dm_permission: The application permissions if executed in a Direct Message. Defaults to ``True``.
-        :param Optional[bool] nsfw:
-            .. versionadded:: 4.4.0
-
-            Indicates whether the command is age-restricted. Defaults to ``False``
-        :param Optional[bool] default_scope:
-            .. versionadded:: 4.3.0
-
-            Whether the scope of the command is the default scope set in the client. Defaults to ``True``.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Command]
-        """
-
-        def decorator(coro: Callable[..., Coroutine]) -> Command:
-            return self.command(
-                type=ApplicationCommandType.MESSAGE,
-                name=name,
-                scope=scope,
-                default_member_permissions=default_member_permissions,
-                dm_permission=dm_permission,
-                nsfw=nsfw,
-                name_localizations=name_localizations,
-                default_scope=default_scope,
-            )(coro)
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        category: Union[Snowflake_Type, "models.GuildCategory"] = None,
+        nsfw: bool = False,
+        rate_limit_per_user: int = 0,
+        layout: ForumLayoutType = ForumLayoutType.NOT_SET,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildForum":
+        """
+        Create a forum channel in this guild.
+
+        Args:
+            name: The name of the forum channel
+            topic: The topic of the forum channel
+            position: The position of the forum channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the forum channel
+            category: The category this forum channel should be within
+            nsfw: Should this forum be marked nsfw
+            rate_limit_per_user: The time users must wait between sending messages
+            layout: The layout of the forum channel
+            reason: The reason for creating this channel
+
+        Returns:
+           The newly created forum channel.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_FORUM,
+            name=name,
+            topic=topic,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            category=category,
+            nsfw=nsfw,
+            rate_limit_per_user=rate_limit_per_user,
+            default_forum_layout=layout,
+            reason=reason,
+        )
 
-        return decorator
+    async def create_news_channel(
+        self,
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        category: Union[Snowflake_Type, "models.GuildCategory"] = None,
+        nsfw: bool = False,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildNews":
+        """
+        Create a news channel in this guild.
+
+        Args:
+            name: The name of the channel
+            topic: The topic of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            category: The category this channel should be within
+            nsfw: Should this channel be marked nsfw
+            reason: The reason for creating this channel
+
+        Returns:
+           The newly created news channel.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_NEWS,
+            name=name,
+            topic=topic,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            category=category,
+            nsfw=nsfw,
+            reason=reason,
+        )
 
-    def user_command(
+    async def create_voice_channel(
         self,
-        *,
-        name: Optional[str] = MISSING,
-        scope: Optional[Union[int, Guild, List[int], List[Guild]]] = MISSING,
-        name_localizations: Optional[Dict[Union[str, Locale], Any]] = MISSING,
-        default_member_permissions: Optional[Union[int, Permissions]] = MISSING,
-        dm_permission: Optional[bool] = MISSING,
-        nsfw: Optional[bool] = MISSING,
-        default_scope: bool = True,
-    ) -> Callable[[Callable[..., Coroutine]], Command]:
-        """
-        A decorator for registering a user context menu to the Discord API,
-        as well as being able to listen for ``INTERACTION_CREATE`` dispatched
-        gateway events.
-
-        The structure of a user context menu:
-
-        .. code-block:: python
-
-            @bot.user_command(name="Context menu name")
-            async def context_menu_name(ctx):
-                ...
-
-        The ``scope`` kwarg field may also be used to designate the command in question
-        applicable to a guild or set of guilds.
-
-        :param Optional[str] name: The name of the application command.
-        :param Optional[Union[int, Guild, List[int], List[Guild]]] scope: The "scope"/applicable guilds the application command applies to. Defaults to ``None``.
-        :param Optional[Dict[Union[str, Locale], str]] name_localizations:
-            .. versionadded:: 4.2.0
-
-            The dictionary of localization for the ``name`` field. This enforces the same restrictions as the ``name`` field.
-        :param Optional[Union[int, Permissions]] default_member_permissions:
-        The permissions bit value of :class:`.Permissions`. If not given, defaults to :attr:`.Permissions.USE_APPLICATION_COMMANDS`
-        :param Optional[bool] dm_permission: The application permissions if executed in a Direct Message. Defaults to ``True``.
-        :param Optional[bool] nsfw:
-            .. versionadded:: 4.4.0
-
-            Indicates whether the command is age-restricted. Defaults to ``False``
-        :param Optional[bool] default_scope:
-            .. versionadded:: 4.3.0
-
-            Whether the scope of the command is the default scope set in the client. Defaults to ``True``.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Command]
-        """
-
-        def decorator(coro: Callable[..., Coroutine]) -> Command:
-            return self.command(
-                type=ApplicationCommandType.USER,
-                name=name,
-                scope=scope,
-                default_member_permissions=default_member_permissions,
-                dm_permission=dm_permission,
-                nsfw=nsfw,
-                name_localizations=name_localizations,
-                default_scope=default_scope,
-            )(coro)
-
-        return decorator
-
-    def component(
-        self, component: Union[str, Button, SelectMenu]
-    ) -> Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]:
-        """
-        A decorator for listening to ``INTERACTION_CREATE`` dispatched gateway
-        events involving components.
-
-        The structure for a component callback:
-
-        .. code-block:: python
-
-            # Method 1
-            @bot.component(interactions.Button(
-                style=interactions.ButtonStyle.PRIMARY,
-                label="click me!",
-                custom_id="click_me_button",
-            ))
-            async def button_response(ctx):
-                ...
-
-            # Method 2
-            @bot.component("custom_id")
-            async def button_response(ctx):
-                ...
-
-        The context of the component callback decorator inherits the same
-        as of the command decorator.
-
-        :param Union[str, Button, SelectMenu] component: The component you wish to callback for.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]
-        """
-
-        def decorator(coro: Callable[..., Coroutine]) -> Callable[..., Coroutine]:
-            payload: str = (
-                _component(component).custom_id
-                if isinstance(component, (Button, SelectMenu))
-                else component
-            )
-            return self.event(coro, name=f"component_{payload}")
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        category: Union[Snowflake_Type, "models.GuildCategory"] = None,
+        nsfw: bool = False,
+        bitrate: int = 64000,
+        user_limit: int = 0,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildVoice":
+        """
+        Create a guild voice channel.
+
+        Args:
+            name: The name of the channel
+            topic: The topic of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            category: The category this channel should be within
+            nsfw: Should this channel be marked nsfw
+            bitrate: The bitrate of this channel, only for voice
+            user_limit: The max users that can be in this channel, only for voice
+            reason: The reason for creating this channel
+
+        Returns:
+           The newly created voice channel.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_VOICE,
+            name=name,
+            topic=topic,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            category=category,
+            nsfw=nsfw,
+            bitrate=bitrate,
+            user_limit=user_limit,
+            reason=reason,
+        )
 
-        return decorator
+    async def create_stage_channel(
+        self,
+        name: str,
+        topic: Absent[Optional[str]] = MISSING,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        category: Absent[Union[Snowflake_Type, "models.GuildCategory"]] = MISSING,
+        bitrate: int = 64000,
+        user_limit: int = 0,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildStageVoice":
+        """
+        Create a guild stage channel.
+
+        Args:
+            name: The name of the channel
+            topic: The topic of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            category: The category this channel should be within
+            bitrate: The bitrate of this channel, only for voice
+            user_limit: The max users that can be in this channel, only for voice
+            reason: The reason for creating this channel
+
+        Returns:
+            The newly created stage channel.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_STAGE_VOICE,
+            name=name,
+            topic=topic,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            category=category,
+            bitrate=bitrate,
+            user_limit=user_limit,
+            reason=reason,
+        )
 
-    def _find_command(self, command: Union[str, int]) -> ApplicationCommand:
+    async def create_category(
+        self,
+        name: str,
+        position: Absent[Optional[int]] = MISSING,
+        permission_overwrites: Absent[
+            Union[dict, "models.PermissionOverwrite", List[Union[dict, "models.PermissionOverwrite"]]]
+        ] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.GuildCategory":
         """
-        Iterates over `commands` and returns an :class:`ApplicationCommand` if it matches the name from `command`
+        Create a category within this guild.
 
-        :param Union[str, int] command: The name or ID of the command to match
-        :return: An ApplicationCommand model
-        :rtype: ApplicationCommand
-        """
-        key = "name" if isinstance(command, str) else "id"
-        _command_obj = next(
-            (
-                ApplicationCommand(**_command)
-                for _command in self.__global_commands["commands"]
-                if str(_command[key]) == str(command)
-            ),
-            None,
+        Args:
+            name: The name of the channel
+            position: The position of the channel in the channel list
+            permission_overwrites: Permission overwrites to apply to the channel
+            reason: The reason for creating this channel
+
+        Returns:
+            The newly created category.
+
+        """
+        return await self.create_channel(
+            channel_type=ChannelType.GUILD_CATEGORY,
+            name=name,
+            position=position,
+            permission_overwrites=permission_overwrites,
+            reason=reason,
         )
 
-        if not _command_obj:
-            for scope in self._scopes:
-                _command_obj = next(
-                    (
-                        ApplicationCommand(**_command)
-                        for _command in self.__guild_commands[scope]["commands"]
-                        if str(_command[key]) == str(command)
-                    ),
-                    None,
-                )
-                if _command_obj:
-                    break
+    async def delete_channel(
+        self, channel: Union["models.TYPE_GUILD_CHANNEL", Snowflake_Type], reason: str = None
+    ) -> None:
+        """
+        Delete the given channel, can handle either a snowflake or channel object.
 
-        if not _command_obj or (hasattr(_command_obj, "id") and not _command_obj.id):
-            raise LibraryException(
-                6,
-                message="The command does not exist. Make sure to define"
-                + " your autocomplete callback after your commands",
-            )
-        else:
-            return _command_obj
+        This is effectively just an alias for `channel.delete()`
 
-    def autocomplete(
-        self, command: Union[ApplicationCommand, int, str, Snowflake], name: str
-    ) -> Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]:
-        """
-        .. versionadded:: 4.0.2
+        Args:
+            channel: The channel to be deleted
+            reason: The reason for this deletion
 
-        A decorator for listening to ``INTERACTION_CREATE`` dispatched gateway
-        events involving autocompletion fields.
+        """
+        if isinstance(channel, (str, int)):
+            channel = await self._client.fetch_channel(channel)
 
-        The structure for an autocomplete callback:
+        if not channel:
+            raise ValueError("Unable to find requested channel")
 
-        .. code-block:: python
+        if channel.id not in self._channel_ids:
+            raise ValueError("This guild does not hold the requested channel")
 
-            @bot.autocomplete(command="command_name", name="option_name")
-            async def autocomplete_choice_list(ctx, user_input: str = ""):
-                await ctx.populate([
-                    interactions.Choice(...),
-                    interactions.Choice(...),
-                    ...
-                ])
+        await channel.delete(reason)
 
-        :param Union[ApplicationCommand, int, str, Snowflake] command: The command, command ID, or command name with the option.
-        :param str name: The name of the option to autocomplete.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]
+    async def list_scheduled_events(self, with_user_count: bool = False) -> List["models.ScheduledEvent"]:
         """
+        List all scheduled events in this guild.
 
-        if isinstance(command, ApplicationCommand):
-            _command: str = command.name
-        elif isinstance(command, str):
-            _command: str = command
-        elif isinstance(command, (int, Snowflake)):
-            _command: Union[Snowflake, int] = int(command)
-        else:
-            raise LibraryException(
-                message="You can only insert strings, integers and ApplicationCommands here!",
-                code=12,
-            )
-
-        def decorator(coro: Callable[..., Coroutine]) -> Callable[..., Coroutine]:
-            if isinstance(_command, (int, Snowflake)):
-                curr_autocomplete = self.__id_autocomplete.get(_command, [])
-                curr_autocomplete.append({"coro": coro, "name": name})
-                self.__id_autocomplete[_command] = curr_autocomplete
-                return coro
-            return self.event(coro, name=f"autocomplete_{_command}_{name}")
-
-        return decorator
-
-    def modal(
-        self, modal: Union[Modal, str]
-    ) -> Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]:
-        """
-        A decorator for listening to ``INTERACTION_CREATE`` dispatched gateway
-        events involving modals.
-
-        The structure for a modal callback:
-
-        .. code-block:: python
-
-            @bot.modal(interactions.Modal(
-                interactions.TextInput(
-                    style=interactions.TextStyleType.PARAGRAPH,
-                    custom_id="how_was_your_day_field",
-                    label="How has your day been?",
-                    placeholder="Well, so far...",
-                ),
-            ))
-            async def modal_response(ctx, how_was_your_day_field: str):
-                ...
-
-        The context of the modal callback decorator inherits the same
-        as of the component decorator.
-
-        :param Union[Modal, str] modal: The modal or custom_id of modal you wish to callback for.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]
-        """
-
-        def decorator(coro: Callable[..., Coroutine]) -> Callable[..., Coroutine]:
-            payload: str = modal.custom_id if isinstance(modal, Modal) else modal
-            return self.event(coro, name=f"modal_{payload}")
-
-        return decorator
-
-    def load(
-        self, name: str, package: Optional[str] = None, *args, **kwargs
-    ) -> Optional["Extension"]:
-        r"""
-        .. versionadded:: 4.1.0
-
-        "Loads" an extension off of the current client by adding a new class
-        which is imported from the library.
-
-        :param str name: The name of the extension.
-        :param Optional[str] package: The package of the extension.
-        :param tuple \*args: Optional arguments to pass to the extension
-        :param dict \**kwargs: Optional keyword-only arguments to pass to the extension.
-        :return: The loaded extension.
-        :rtype: Optional[Extension]
-        """
-        _name: str = resolve_name(name, package)
-
-        if _name in self._extensions:
-            log.error(f"Extension {name} has already been loaded. Skipping.")
-            return
-
-        module = import_module(
-            name, package
-        )  # should be a module, because Extensions just need to be __init__-ed
+        Returns:
+            A list of scheduled events.
 
-        try:
-            setup = getattr(module, "setup")
-            extension = setup(self, *args, **kwargs)
-        except Exception as error:
-            del sys.modules[name]
-            log.error(f"Could not load {name}: {error}. Skipping.")
-            raise error from error
-        else:
-            log.debug(f"Loaded extension {name}.")
-            self._extensions[_name] = module
-            del sys.modules[name]
-            return extension
+        """
+        scheduled_events_data = await self._client.http.list_schedules_events(self.id, with_user_count)
+        return models.ScheduledEvent.from_list(scheduled_events_data, self._client)
 
-    def remove(
-        self, name: str, remove_commands: bool = True, package: Optional[str] = None
-    ) -> None:
+    async def fetch_scheduled_event(
+        self, scheduled_event_id: Snowflake_Type, with_user_count: bool = False
+    ) -> Optional["models.ScheduledEvent"]:
         """
-        .. versionadded:: 4.1.0
+        Get a scheduled event by id.
+
+        Args:
+            scheduled_event_id: The id of the scheduled event.
+            with_user_count: Whether to include the user count in the response.
 
-        Removes an extension out of the current client from an import resolve.
+        Returns:
+            The scheduled event. If the event does not exist, returns None.
 
-        :param str name: The name of the extension.
-        :param Optional[bool] remove_commands: Whether to remove commands before reloading. Defaults to ``True``.
-        :param Optional[str] package: The package of the extension.
         """
         try:
-            _name: str = resolve_name(name, package)
-        except AttributeError:
-            _name = name
-
-        extension = self._extensions.get(_name)
-
-        if _name not in self._extensions:
-            log.error(f"Extension {name} has not been loaded before. Skipping.")
-            return
-
-        if isinstance(extension, ModuleType):  # loaded as a module
-            for ext_name, ext in getmembers(
-                extension, lambda x: isinstance(x, type) and issubclass(x, Extension)
-            ):
-                if ext_name != "Extension":
-                    _extension = self._extensions.get(ext_name)
-                    with contextlib.suppress(AttributeError):
-                        self._loop.create_task(
-                            _extension.teardown(remove_commands=remove_commands)
-                        )  # made for Extension, usable by others
+            scheduled_event_data = await self._client.http.get_scheduled_event(
+                self.id, scheduled_event_id, with_user_count
+            )
+        except NotFound:
+            return None
+        return models.ScheduledEvent.from_dict(scheduled_event_data, self._client)
 
-        else:
-            with contextlib.suppress(AttributeError):
-                self._loop.create_task(
-                    extension.teardown(remove_commands=remove_commands)
-                )  # made for Extension, usable by others
-        del self._extensions[_name]
+    async def create_scheduled_event(
+        self,
+        name: str,
+        event_type: ScheduledEventType,
+        start_time: "models.Timestamp",
+        end_time: Absent[Optional["models.Timestamp"]] = MISSING,
+        description: Absent[Optional[str]] = MISSING,
+        channel_id: Absent[Optional[Snowflake_Type]] = MISSING,
+        external_location: Absent[Optional[str]] = MISSING,
+        entity_metadata: Optional[dict] = None,
+        privacy_level: ScheduledEventPrivacyLevel = ScheduledEventPrivacyLevel.GUILD_ONLY,
+        cover_image: Absent[UPLOADABLE_TYPE] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.ScheduledEvent":
+        """
+        Create a scheduled guild event.
+
+        Args:
+            name: event name
+            event_type: event type
+            start_time: `Timestamp` object
+            end_time: `Timestamp` object
+            description: event description
+            channel_id: channel id
+            external_location: event external location (For external events)
+            entity_metadata: event metadata (additional data for the event)
+            privacy_level: event privacy level
+            cover_image: the cover image of the scheduled event
+            reason: reason for creating this scheduled event
+
+        Returns:
+            The newly created ScheduledEvent object
+
+        !!! note
+            For external events, external_location is required
+            For voice/stage events, channel_id is required
+
+        ??? note
+            entity_metadata is the backend dictionary for fluff fields. Where possible, we plan to expose these fields directly.
+            The full list of supported fields is https://discord.com/developers/docs/resources/guild-scheduled-event#guild-scheduled-event-object-guild-scheduled-event-entity-metadata
+            Example: `entity_metadata=dict(location="cool place")`
+
+        """
+        if external_location is not MISSING:
+            entity_metadata = {"location": external_location}
+
+        if event_type == ScheduledEventType.EXTERNAL and external_location == MISSING:
+            raise EventLocationNotProvided("Location is required for external events")
+
+        payload = {
+            "name": name,
+            "entity_type": event_type,
+            "scheduled_start_time": start_time.isoformat(),
+            "scheduled_end_time": end_time.isoformat() if end_time is not MISSING else end_time,
+            "description": description,
+            "channel_id": channel_id,
+            "entity_metadata": entity_metadata,
+            "privacy_level": privacy_level,
+            "image": to_image_data(cover_image) if cover_image else MISSING,
+        }
 
-        log.debug(f"Removed extension {name}.")
+        scheduled_event_data = await self._client.http.create_scheduled_event(self.id, payload, reason)
+        return models.ScheduledEvent.from_dict(scheduled_event_data, self._client)
 
-    def reload(
+    async def create_custom_sticker(
         self,
         name: str,
-        package: Optional[str] = None,
-        remove_commands: bool = True,
-        *args,
-        **kwargs,
-    ) -> Optional["Extension"]:
-        r"""
-        .. versionadded:: 4.1.0
+        file: UPLOADABLE_TYPE,
+        tags: list[str],
+        description: Absent[Optional[str]] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.Sticker":
+        """
+        Creates a custom sticker for a guild.
 
-        "Reloads" an extension off of current client from an import resolve.
+        Args:
+            name: The name of the sticker (2-30 characters)
+            file: The sticker file to upload, must be a PNG, APNG, or Lottie JSON file (max 500 KB)
+            tags: Autocomplete/suggestion tags for the sticker (max 200 characters)
+            description: The description of the sticker (empty or 2-100 characters)
+            reason: Reason for creating the sticker
 
-        .. warning::
-            This will remove and re-add application commands, counting towards your daily application
-            command creation limit, as long as you have the ``remove_commands`` argument set to ``True``, which it is by
-            default.
+        Returns:
+            New Sticker instance
 
-        :param str name: The name of the extension
-        :param Optional[str] package: The package of the extension
-        :param Optional[bool] remove_commands: Whether to remove commands before reloading. Defaults to True
-        :param tuple \*args: Optional arguments to pass to the extension
-        :param dict \**kwargs: Optional keyword-only arguments to pass to the extension.
-        :return: The reloaded extension.
-        :rtype: Optional[Extension]
         """
-        _name: str = resolve_name(name, package)
-        extension = self._extensions.get(_name)
+        payload = {"name": name, "tags": " ".join(tags)}
 
-        if extension is None:
-            log.warning(f"Extension {name} could not be reloaded because it was never loaded.")
-            return self.load(name, package)
+        if description:
+            payload["description"] = description
 
-        self.remove(name, package=package, remove_commands=remove_commands)
-        return self.load(name, package, *args, **kwargs)
+        sticker_data = await self._client.http.create_guild_sticker(payload, self.id, file=file, reason=reason)
+        return models.Sticker.from_dict(sticker_data, self._client)
 
-    def get_extension(self, name: str) -> Optional[Union[ModuleType, "Extension"]]:
+    async def fetch_all_custom_stickers(self) -> List["models.Sticker"]:
         """
-        .. versionadded:: 4.2.0
+        Fetches all custom stickers for a guild.
 
-        Get an extension based on its name.
+        Returns:
+            List of Sticker objects
 
-        :param str name: Name of the extension.
-        :return: The found extension.
-        :rtype: Optional[Union[ModuleType, Extension]]
         """
-        return self._extensions.get(name)
+        stickers_data = await self._client.http.list_guild_stickers(self.id)
+        return models.Sticker.from_list(stickers_data, self._client)
 
-    async def modify(
-        self,
-        username: Optional[str] = MISSING,
-        avatar: Optional[Image] = MISSING,
-    ) -> User:
+    async def fetch_custom_sticker(self, sticker_id: Snowflake_Type) -> Optional["models.Sticker"]:
         """
-        .. versionadded:: 4.2.0
+        Fetches a specific custom sticker for a guild.
+
+        Args:
+            sticker_id: ID of sticker to get
 
-        Modify the bot user account settings.
+        Returns:
+            The custom sticker object. If the sticker does not exist, returns None.
 
-        :param Optional[str] username: The new username of the bot
-        :param Optional[Image] avatar: The new avatar of the bot
-        :return: The modified User object
-        :rtype: User
         """
-        if not self._http or isinstance(self._http, str):
-            raise LibraryException(
-                code=13, message="You cannot use this method until the bot has started!"
-            )
+        try:
+            sticker_data = await self._client.http.get_guild_sticker(self.id, to_snowflake(sticker_id))
+        except NotFound:
+            return None
+        return models.Sticker.from_dict(sticker_data, self._client)
 
-        payload: dict = {}
-        if avatar is not MISSING:
-            payload["avatar"] = avatar.data
-        if username is not MISSING:
-            payload["username"] = username
-        data: dict = await self._http.modify_self(payload=payload)
-
-        return User(**data)
-
-    async def request_guild_members(
-        self,
-        guild_id: Union[Guild, Snowflake, int, str],
-        limit: Optional[int] = MISSING,
-        query: Optional[str] = MISSING,
-        presences: Optional[bool] = MISSING,
-        user_ids: Optional[Union[Snowflake, List[Snowflake]]] = MISSING,
-        nonce: Optional[str] = MISSING,
-    ) -> None:
+    async def fetch_active_threads(self) -> "models.ThreadList":
         """
-        .. versionadded:: 4.3.2
+        Fetches all active threads in the guild, including public and private threads. Threads are ordered by their id, in descending order.
 
-        Requests guild members via websocket.
+        Returns:
+            List of active threads and thread member object for each returned thread the bot user has joined.
 
-        :param Union[Guild, Snowflake, int, str] guild_id: ID of the guild to get members for.
-        :param Optional[int] limit: Maximum number of members to send matching the 'query' parameter. Required when specifying 'query'.
-        :param Optional[str] query: String that username starts with.
-        :param Optional[bool] presences: Used to specify if we want the presences of the matched members.
-        :param Optional[Union[Snowflake, List[Snowflake]]] user_ids: Used to specify which users you wish to fetch.
-        :param Optional[str] nonce: Nonce to identify the Guild Members Chunk response.
-        """
-        await self._websocket.request_guild_members(
-            guild_id=int(guild_id.id) if isinstance(guild_id, Guild) else int(guild_id),
-            limit=limit if limit is not MISSING else 0,
-            query=query if query is not MISSING else None,
-            presences=presences if presences is not MISSING else None,
-            user_ids=user_ids if user_ids is not MISSING else None,
-            nonce=nonce if nonce is not MISSING else None,
-        )
+        """
+        threads_data = await self._client.http.list_active_threads(self.id)
+        return models.ThreadList.from_dict(threads_data, self._client)
+
+    async def fetch_role(self, role_id: Snowflake_Type) -> Optional["models.Role"]:
+        """
+        Fetch the specified role by ID.
 
-    async def _logout(self) -> None:
-        await self._websocket.close()
-        if isinstance(self._http, HTTPClient):
-            await self._http._req.close()
+        Args:
+            role_id: The ID of the role to get
 
-    async def wait_for(
+        Returns:
+            The role object. If the role does not exist, returns None.
+
+        """
+        try:
+            return await self._client.cache.fetch_role(self.id, role_id)
+        except NotFound:
+            return None
+
+    def get_role(self, role_id: Snowflake_Type) -> Optional["models.Role"]:
+        """
+        Get the specified role by ID.
+
+        Args:
+            role_id: The ID of the role to get
+
+        Returns:
+            A role object or None if the role is not found.
+
+        """
+        role_id = to_snowflake(role_id)
+        if role_id in self._role_ids:
+            return self._client.cache.get_role(role_id)
+        return None
+
+    async def create_role(
         self,
-        name: str,
-        check: Optional[Callable[..., Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> Any:
+        name: Absent[Optional[str]] = MISSING,
+        permissions: Absent[Optional[Permissions]] = MISSING,
+        colour: Absent[Optional[Union["models.Color", int]]] = MISSING,
+        color: Absent[Optional[Union["models.Color", int]]] = MISSING,
+        hoist: Optional[bool] = False,
+        mentionable: Optional[bool] = False,
+        icon: Absent[Optional[UPLOADABLE_TYPE]] = MISSING,
+        reason: Absent[Optional[str]] = MISSING,
+    ) -> "models.Role":
+        """
+        Create a new role for the guild. You must have the `manage roles` permission.
+
+        Args:
+            name: The name the role should have. `Default: new role`
+            permissions: The permissions the role should have. `Default: @everyone permissions`
+            colour: The colour of the role. Can be either `Color` or an RGB integer. `Default: BrandColors.BLACK`
+            color: Alias for `colour`
+            icon: Can be either a bytes like object or a path to an image, or a unicode emoji which is supported by discord.
+            hoist: Whether the role is shown separately in the members list. `Default: False`
+            mentionable: Whether the role can be mentioned. `Default: False`
+            reason: An optional reason for the audit log.
+
+        Returns:
+            A role object or None if the role is not found.
+
+        """
+        payload = {}
+
+        if name:
+            payload["name"] = name
+
+        if permissions:
+            payload["permissions"] = str(int(permissions))
+
+        if colour := colour or color:
+            payload["color"] = colour.value
+
+        if hoist:
+            payload["hoist"] = True
+
+        if mentionable:
+            payload["mentionable"] = True
+
+        if icon:
+            # test if the icon is probably a unicode emoji (str and len() == 1) or a path / bytes obj
+            if isinstance(icon, str) and len(icon) == 1:
+                payload["unicode_emoji"] = icon
+
+            else:
+                payload["icon"] = to_image_data(icon)
+
+        result = await self._client.http.create_guild_role(guild_id=self.id, payload=payload, reason=reason)
+        return self._client.cache.place_role_data(guild_id=self.id, data=[result])[to_snowflake(result["id"])]
+
+    def get_channel(self, channel_id: Snowflake_Type) -> Optional["models.TYPE_GUILD_CHANNEL"]:
         """
-        .. versionadded:: 4.4.0
+        Returns a channel with the given `channel_id`.
+
+        Args:
+            channel_id: The ID of the channel to get
 
-        Waits for an event once, and returns the result.
+        Returns:
+            Channel object if found, otherwise None
 
-        Unlike event decorators, this is not persistent, and can be used to only proceed in a command once an event happens.
+        """
+        channel_id = to_snowflake(channel_id)
+        if channel_id in self._channel_ids:
+            # theoretically, this could get any channel the client can see,
+            # but to make it less confusing to new programmers,
+            # i intentionally check that the guild contains the channel first
+            return self._client.cache.get_channel(channel_id)
+        return None
 
-        :param str name: The event to wait for
-        :param Optional[Callable[..., Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param float timeout: How long to wait for the event before raising an error
-        :return: The value of the dispatched event
-        :rtype: Any
+    async def fetch_channel(self, channel_id: Snowflake_Type) -> Optional["models.TYPE_GUILD_CHANNEL"]:
         """
-        while True:
-            fut = self._websocket._dispatch.add(name=name)
+        Returns a channel with the given `channel_id` from the API.
+
+        Args:
+            channel_id: The ID of the channel to get
+
+        Returns:
+            The channel object. If the channel does not exist, returns None.
+
+        """
+        channel_id = to_snowflake(channel_id)
+        if channel_id in self._channel_ids or not self._client.gateway_started:
+            # The latter check here is to see if the bot is running with the gateway.
+            # If not, then we need to check the API since only the gateway
+            # populates the channel IDs
+
+            # theoretically, this could get any channel the client can see,
+            # but to make it less confusing to new programmers,
+            # i intentionally check that the guild contains the channel first
             try:
-                # asyncio's wait_for
-                res: tuple = await wait_for(fut, timeout=timeout)
-            except TimeoutError:
-                with contextlib.suppress(ValueError):
-                    self._websocket._dispatch.extra_events[name].remove(fut)
-                raise
-
-            if not check:
-                break
-            checked = check(*res)
-            if isawaitable(checked):
-                checked = await checked
-            if checked:
-                break
-            else:
-                # The check failed, so try again next time
-                log.info(f"A check failed waiting for the {name} event")
+                channel = await self._client.fetch_channel(channel_id)
+                if channel._guild_id == self.id:
+                    return channel
+            except (NotFound, AttributeError):
+                return None
 
-        if res:
-            return res[0] if len(res) == 1 else res
+        return None
 
-    async def wait_for_component(
-        self,
-        components: Union[
-            Union[str, Button, SelectMenu],
-            List[Union[str, Button, SelectMenu]],
-        ] = None,
-        messages: Union[Message, int, List[Union[Message, int]]] = None,
-        check: Optional[Callable[[ComponentContext], Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> ComponentContext:
-        """
-        .. versionadded:: 4.4.0
-
-        Waits for a component to be interacted with, and returns the resulting context.
-
-        .. note::
-            If you are waiting for a select menu, you can find the selected values in ``ctx.data.values``.
-            Another possibility is using the :meth:`.Client.wait_for_select` method.
-
-        :param Union[str, Button, SelectMenu, List[Union[str, Button, SelectMenu]]] components: The component(s) to wait for
-        :param Union[Message, int, List[Union[Message, int]]] messages: The message(s) to check for
-        :param Optional[Callable[[ComponentContext], Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param float timeout: How long to wait for the event before raising an error
-        :return: The ComponentContext of the dispatched event
-        :rtype: ComponentContext
-        """
-        custom_ids: List[str] = []
-        messages_ids: List[int] = []
-
-        if components:
-            if isinstance(components, list):
-                for component in components:
-                    if isinstance(component, (Button, SelectMenu)):
-                        custom_ids.append(component.custom_id)
-                    elif isinstance(component, ActionRow):
-                        custom_ids.extend([c.custom_id for c in component.components])
-                    elif isinstance(component, list):
-                        for c in component:
-                            if isinstance(c, (Button, SelectMenu)):
-                                custom_ids.append(c.custom_id)
-                            elif isinstance(c, ActionRow):
-                                custom_ids.extend([b.custom_id for b in c.components])
-                            elif isinstance(c, str):
-                                custom_ids.append(c)
-                    elif isinstance(component, str):
-                        custom_ids.append(component)
-            elif isinstance(components, (Button, SelectMenu)):
-                custom_ids.append(components.custom_id)
-            elif isinstance(components, ActionRow):
-                custom_ids.extend([c.custom_id for c in components.components])  # noqa
-            elif isinstance(components, str):
-                custom_ids.append(components)
-
-        if messages:
-            if isinstance(messages, Message):
-                messages_ids.append(int(messages.id))
-            elif isinstance(messages, list):
-                for message in messages:
-                    if isinstance(message, Message):
-                        messages_ids.append(int(message.id))
-                    else:
-                        messages_ids.append(int(message))
-            else:  # account for plain ints, string, or Snowflakes
-                messages_ids.append(int(messages))
-
-        def _check(ctx: ComponentContext) -> bool:
-            if custom_ids and ctx.data.custom_id not in custom_ids:
-                return False
-            if messages_ids and int(ctx.message.id) not in messages_ids:
-                return False
-            return check(ctx) if check else True
-
-        return await self.wait_for("on_component", check=_check, timeout=timeout)
-
-    async def wait_for_select(
-        self,
-        components: Union[
-            Union[str, SelectMenu],
-            List[Union[str, SelectMenu]],
-        ] = None,
-        messages: Union[Message, int, List[Union[Message, int]]] = None,
-        check: Optional[Callable[[ComponentContext], Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> Tuple[ComponentContext, List[Union[str, Member, User, Role, Channel]]]:
-        """
-        .. versionadded:: 4.4.0
-
-        Waits for a select menu to be interacted with, and returns the resulting context and a list of the selected values.
-
-        The method can be used like this:
-
-        .. code-block:: python
-
-            ctx, values = await bot.wait_for_select(custom_id)
-
-        In this case ``ctx`` will be your normal context and ``values`` will be a list of :class:`str`, :class:`.Member`, :class:`.User`, :class:`.Channel` or :class:`.Role` objects,
-        depending on which select type you received.
-
-
-        :param Union[str, SelectMenu, List[Union[str, SelectMenu]]] components: The component(s) to wait for
-        :param Union[Message, int, List[Union[Message, int]]] messages: The message(s) to check for
-        :param Optional[Callable[[ComponentContext], Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param float timeout: How long to wait for the event before raising an error
-        :return: The ComponentContext and list of selections of the dispatched event
-        :rtype: Tuple[ComponentContext, Union[List[str], List[Member], List[User], List[Channel], List[Role]]]
-        """
-
-        def _check(_ctx: ComponentContext) -> bool:
-            if _ctx.data.component_type.value not in {3, 5, 6, 7, 8}:
-                return False
-            return check(_ctx) if check else True
+    def get_thread(self, thread_id: Snowflake_Type) -> Optional["models.TYPE_THREAD_CHANNEL"]:
+        """
+        Returns a Thread with the given `thread_id`.
 
-        ctx: ComponentContext = await self.wait_for_component(
-            components, messages, check=_check, timeout=timeout
-        )
+        Args:
+            thread_id: The ID of the thread to get
 
-        if ctx.data.component_type == 3:
-            return ctx, ctx.data.values
+        Returns:
+            Thread object if found, otherwise None
 
-        _list = []  # temp storage for items
-        _data = self._websocket._WebSocketClient__select_option_type_context(
-            ctx, ctx.data.component_type.value
-        )  # resolved.
-        for value in ctx.data.values:
-            _list.append(_data[value])
-        return ctx, _list
+        """
+        thread_id = to_snowflake(thread_id)
+        if thread_id in self._thread_ids:
+            return self._client.cache.get_channel(thread_id)
+        return None
 
-    async def wait_for_modal(
-        self,
-        modals: Union[Modal, str, List[Union[Modal, str]]],
-        check: Optional[Callable[[CommandContext], Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> Tuple[CommandContext, List[str]]:
+    async def fetch_thread(self, thread_id: Snowflake_Type) -> Optional["models.TYPE_THREAD_CHANNEL"]:
         """
-        .. versionadded:: 4.4.0
+        Returns a Thread with the given `thread_id` from the API.
 
-        Waits for a modal to be interacted with, and returns the resulting context and submitted data.
+        Args:
+            thread_id: The ID of the thread to get
 
-        .. note::
-            This function returns both the context of the modal and the data the user input.
-            The recommended way to use it is to do:
-            ``modal_ctx, fields = await bot.wait_for_modal(...)``
+        Returns:
+            Thread object if found, otherwise None
 
-            Alternatively, to get the fields immediately, you can do:
-            ``modal_ctx, (field1, field2, ...) = await bot.wait_for_modal(...)``
+        """
+        thread_id = to_snowflake(thread_id)
+        if thread_id in self._thread_ids:
+            try:
+                return await self._client.fetch_channel(thread_id)
+            except NotFound:
+                return None
+        return None
 
-        :param Union[Modal, str, List[Modal, str]] modals: The modal(s) to wait for
-        :param Optional[Callable[[CommandContext], Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param Optional[float] timeout: How long to wait for the event before raising an error
-        :return: The context of the modal, followed by the data the user inputted
-        :rtype: tuple[CommandContext, list[str]]
+    async def prune_members(
+        self,
+        days: int = 7,
+        roles: Optional[List[Snowflake_Type]] = None,
+        compute_prune_count: bool = True,
+        reason: Absent[str] = MISSING,
+    ) -> Optional[int]:
+        """
+        Begin a guild prune. Removes members from the guild who who have not interacted for the last `days` days. By default, members with roles are excluded from pruning, to include them, pass their role (or role id) in `roles` Requires `kick members` permission.
+
+        Args:
+            days: number of days to prune (1-30)
+            roles: list of roles to include in the prune
+            compute_prune_count: Whether the number of members pruned should be calculated (disable this for large guilds)
+            reason: The reason for this prune
+
+        Returns:
+            The total number of members pruned, if `compute_prune_count` is set to True, otherwise None
+
+        """
+        if roles:
+            roles = [str(to_snowflake(r)) for r in roles]
+
+        resp = await self._client.http.begin_guild_prune(
+            self.id,
+            days,
+            include_roles=roles,
+            compute_prune_count=compute_prune_count,
+            reason=reason,
+        )
+        return resp["pruned"]
+
+    async def estimate_prune_members(
+        self, days: int = 7, roles: List[Union[Snowflake_Type, "models.Role"]] = MISSING
+    ) -> int:
         """
-        ids: List[str] = []
+        Calculate how many members would be pruned, should `guild.prune_members` be used. By default, members with roles are excluded from pruning, to include them, pass their role (or role id) in `roles`.
 
-        if isinstance(modals, Modal):
-            ids = [str(modals.custom_id)]
-        elif isinstance(modals, str):
-            ids = [modals]
-        elif isinstance(modals, list):
-            for modal in modals:
-                if isinstance(modal, Modal):
-                    ids.append(str(modal.custom_id))
-                elif isinstance(modal, str):
-                    modals.append(modal)
+        Args:
+            days: number of days to prune (1-30)
+            roles: list of roles to include in the prune
 
-        if not all(isinstance(id, str) for id in ids):
-            raise TypeError("No modals were passed!")
+        Returns:
+            Total number of members that would be pruned
 
-        def _check(ctx: CommandContext):
-            if ids and ctx.data.custom_id not in ids:
-                return False
-            return check(ctx) if check else True
+        """
+        if roles is not MISSING:
+            roles = [r.id if isinstance(r, models.Role) else r for r in roles]
+        else:
+            roles = []
 
-        ctx: CommandContext = await self.wait_for("on_modal", check=_check, timeout=timeout)
+        resp = await self._client.http.get_guild_prune_count(self.id, days=days, include_roles=roles)
+        return resp["pruned"]
 
-        # Ed requested that it returns a result similar to the decorator
-        fields: List[str] = []
-        for actionrow in ctx.data.components:  # discord is weird with this
-            if actionrow.components:
-                data = actionrow.components[0].value
-                fields.append(data)
+    async def leave(self) -> None:
+        """Leave this guild."""
+        await self._client.http.leave_guild(self.id)
+
+    async def delete(self) -> None:
+        """
+        Delete the guild.
 
-        return ctx, fields
+        !!! note
+            You must own this guild to do this.
 
-    async def get_self_user(self) -> User:
         """
-        .. versionadded:: 4.4.0
+        await self._client.http.delete_guild(self.id)
 
-        Gets the bot's user information.
+    async def kick(
+        self,
+        user: Union["models.User", "models.Member", Snowflake_Type],
+        reason: Absent[str] = MISSING,
+    ) -> None:
         """
-        return User(**await self._http.get_self(), _client=self._http)
+        Kick a user from the guild.
+
+        !!! note
+            You must have the `kick members` permission
+
+        Args:
+            user: The user to kick
+            reason: The reason for the kick
 
-    async def get_role_connection_metadata(self) -> List[ApplicationRoleConnectionMetadata]:
         """
-        .. versionadded:: 4.4.0
+        await self._client.http.remove_guild_member(self.id, to_snowflake(user), reason=reason)
 
-        Gets the bot's role connection metadata.
+    async def ban(
+        self,
+        user: Union["models.User", "models.Member", Snowflake_Type],
+        delete_message_days: Absent[int] = MISSING,
+        delete_message_seconds: int = 0,
+        reason: Absent[str] = MISSING,
+    ) -> None:
+        """
+        Ban a user from the guild.
+
+        !!! note
+            You must have the `ban members` permission
+
+        Args:
+            user: The user to ban
+            delete_message_days: (deprecated) How many days worth of messages to remove
+            delete_message_seconds: How many seconds worth of messages to remove
+            reason: The reason for the ban
+
+        """
+        if delete_message_days is not MISSING:
+            warn(
+                "delete_message_days is deprecated and will be removed in a future update",
+                DeprecationWarning,
+            )
+            delete_message_seconds = delete_message_days * 3600
+        await self._client.http.create_guild_ban(self.id, to_snowflake(user), delete_message_seconds, reason=reason)
 
-        :return: The list of bot's role connection metadata.
+    async def fetch_ban(self, user: Union["models.User", "models.Member", Snowflake_Type]) -> Optional[GuildBan]:
         """
+        Fetches the ban information for the specified user in the guild. You must have the `ban members` permission.
 
-        res: List[dict] = await self._http.get_application_role_connection_metadata(
-            application_id=int(self.me.id)
-        )
-        return [ApplicationRoleConnectionMetadata(**metadata) for metadata in res]
+        Args:
+            user: The user to look up.
+
+        Returns:
+            The ban information. If the user is not banned, returns None.
 
-    async def update_role_connection_metadata(
+        """
+        try:
+            ban_info = await self._client.http.get_guild_ban(self.id, to_snowflake(user))
+        except NotFound:
+            return None
+        return GuildBan(reason=ban_info["reason"], user=self._client.cache.place_user_data(ban_info["user"]))
+
+    async def fetch_bans(
         self,
-        metadata: Union[List[ApplicationRoleConnectionMetadata], ApplicationRoleConnectionMetadata],
-    ) -> List[ApplicationRoleConnectionMetadata]:
+        before: Optional["Snowflake_Type"] = MISSING,
+        after: Optional["Snowflake_Type"] = MISSING,
+        limit: int = 1000,
+    ) -> list[GuildBan]:
+        """
+        Fetches bans for the guild. You must have the `ban members` permission.
+
+        Args:
+            before: consider only users before given user id
+            after: consider only users after given user id
+            limit: number of users to return (up to maximum 1000)
+
+        Returns:
+            A list containing bans and information about them.
+
+        """
+        ban_infos = await self._client.http.get_guild_bans(self.id, before=before, after=after, limit=limit)
+        return [
+            GuildBan(reason=ban_info["reason"], user=self._client.cache.place_user_data(ban_info["user"]))
+            for ban_info in ban_infos
+        ]
+
+    async def create_auto_moderation_rule(
+        self,
+        name: str,
+        *,
+        trigger: BaseTrigger,
+        actions: list[BaseAction],
+        exempt_roles: list["Snowflake_Type"] = MISSING,
+        exempt_channels: list["Snowflake_Type"] = MISSING,
+        enabled: bool = True,
+        event_type: AutoModEvent = AutoModEvent.MESSAGE_SEND,
+    ) -> AutoModRule:
+        """
+        Create an auto-moderation rule in this guild.
+
+        Args:
+            name: The name of the rule
+            trigger: The trigger for this rule
+            actions: A list of actions to take upon triggering
+            exempt_roles: Roles that ignore this rule
+            exempt_channels: Channels that ignore this role
+            enabled: Is this rule enabled?
+            event_type: The type of event that triggers this rule
+
+        Returns:
+            The created rule
+        """
+        rule = AutoModRule(
+            name=name,
+            enabled=enabled,
+            actions=actions,
+            event_type=event_type,
+            trigger=trigger,
+            exempt_channels=exempt_channels if exempt_roles is not MISSING else [],
+            exempt_roles=exempt_roles if exempt_roles is not MISSING else [],
+            client=self._client,
+        )
+        data = await self._client.http.create_auto_moderation_rule(self.id, rule.to_dict())
+        return AutoModRule.from_dict(data, self._client)
+
+    async def fetch_auto_moderation_rules(self) -> List[AutoModRule]:
         """
-        .. versionadded:: 4.4.0
+        Get this guild's auto moderation rules.
 
-        Updates the bot's role connection metadata.
+        Returns:
+            A list of auto moderation rules
+        """
+        data = await self._client.http.get_auto_moderation_rules(self.id)
+        return [AutoModRule.from_dict(d, self._client) for d in data]
 
-        .. note::
-            This method overwrites all current bot's role connection metadata.
+    async def delete_auto_moderation_rule(self, rule: "Snowflake_Type", reason: Absent[str] = MISSING) -> None:
+        """
+        Delete a given auto moderation rule.
 
-        :param List[ApplicationRoleConnectionMetadata] metadata: The list of role connection metadata. The maximum is five.
-        :return: The updated list of bot's role connection metadata.
+        Args:
+            rule: The rule to delete
+            reason: The reason for deleting this rule
         """
-        if not isinstance(metadata, list):
-            metadata = [metadata]
+        await self._client.http.delete_auto_moderation_rule(self.id, to_snowflake(rule), reason=reason)
 
-        res: List[dict] = await self._http.update_application_role_connection_metadata(
-            application_id=int(self.me.id), payload=[_._json for _ in metadata]
+    async def modify_auto_moderation_rule(
+        self,
+        rule: "Snowflake_Type",
+        *,
+        name: Absent[str] = MISSING,
+        trigger: Absent[BaseTrigger] = MISSING,
+        trigger_type: Absent[AutoModTriggerType] = MISSING,
+        trigger_metadata: Absent[dict] = MISSING,
+        actions: Absent[list[BaseAction]] = MISSING,
+        exempt_channels: Absent[list["Snowflake_Type"]] = MISSING,
+        exempt_roles: Absent[list["Snowflake_Type"]] = MISSING,
+        event_type: Absent[AutoModEvent] = MISSING,
+        enabled: Absent[bool] = MISSING,
+        reason: Absent[str] = MISSING,
+    ) -> AutoModRule:
+        """
+        Modify an existing automod rule.
+
+        Args:
+            rule: The rule to modify
+            name: The name of the rule
+            trigger: A trigger for this rule
+            trigger_type: The type trigger for this rule (ignored if trigger specified)
+            trigger_metadata: Metadata for the trigger (ignored if trigger specified)
+            actions: A list of actions to take upon triggering
+            exempt_roles: Roles that ignore this rule
+            exempt_channels: Channels that ignore this role
+            enabled: Is this rule enabled?
+            event_type: The type of event that triggers this rule
+            reason: The reason for this change
+
+        Returns:
+            The updated rule
+        """
+        if trigger:
+            _data = trigger.to_dict()
+            trigger_type = _data["trigger_type"]
+            trigger_metadata = _data.get("trigger_metadata", {})
+
+        out = await self._client.http.modify_auto_moderation_rule(
+            self.id,
+            to_snowflake(rule),
+            name=name,
+            trigger_type=trigger_type,
+            trigger_metadata=trigger_metadata,
+            actions=actions,
+            exempt_roles=to_snowflake_list(exempt_roles) if exempt_roles is not MISSING else MISSING,
+            exempt_channels=to_snowflake_list(exempt_channels) if exempt_channels is not MISSING else MISSING,
+            event_type=event_type,
+            enabled=enabled,
+            reason=reason,
         )
-        return [ApplicationRoleConnectionMetadata(**_) for _ in res]
+        return AutoModRule.from_dict(out, self._client)
 
+    async def unban(
+        self,
+        user: Union["models.User", "models.Member", Snowflake_Type],
+        reason: Absent[str] = MISSING,
+    ) -> None:
+        """
+        Unban a user from the guild.
 
-class Extension:
-    """
-    .. versionadded:: 4.1.0
+        !!! note
+            You must have the `ban members` permission
+
+        Args:
+            user: The user to unban
+            reason: The reason for the ban
+
+        """
+        await self._client.http.remove_guild_ban(self.id, to_snowflake(user), reason=reason)
 
-    A class that allows you to represent "extensions" of your code, or
-    essentially cogs that can be ran independent of the root file in
-    an object-oriented structure.
+    async def fetch_widget_image(self, style: str = None) -> str:
+        """
+        Fetch a guilds widget image.
 
-    The structure of an extension:
+        For a list of styles, look here: https://discord.com/developers/docs/resources/guild#get-guild-widget-image-widget-style-options
 
-    .. code-block:: python
+        Args:
+            style: The style to use for the widget image
 
-        class CoolCode(interactions.Extension):
-            def __init__(self, client):
-                self.client = client
+        Returns:
+            The URL of the widget image.
 
-            @extension_user_command(
-                name="User command in cog",
-            )
-            async def cog_user_cmd(self, ctx):
-                ...
+        """
+        return await self._client.http.get_guild_widget_image(self.id, style)
 
-        def setup(client):
-            CoolCode(client)
-    """
+    async def fetch_widget_settings(self) -> "GuildWidgetSettings":
+        """
+        Fetches the guilds widget settings.
 
-    client: Client
+        Returns:
+            The guilds widget settings object.
 
-    def __new__(cls, client: Client, *args, **kwargs) -> "Extension":
-        # sourcery skip: low-code-quality
+        """
+        return await GuildWidgetSettings.from_dict(await self._client.http.get_guild_widget_settings(self.id))
 
-        self = super().__new__(cls)
+    async def fetch_widget(self) -> "GuildWidget":
+        """
+        Fetches the guilds widget.
 
-        self.client = client
-        self._commands = {}
-        self._listeners = {}
-
-        # This gets every coroutine in a way that we can easily change them
-        # cls
-        for name, func in getmembers(self, predicate=iscoroutinefunction):
-            # TODO we can make these all share the same list, might make it easier to load/unload
-            if hasattr(func, "__listener_name__"):  # set by extension_listener
-                all_listener_names: List[str] = func.__listener_name__
-                for listener_name in all_listener_names:
-                    func = client.event(
-                        func, name=listener_name
-                    )  # capture the return value for friendlier ext-ing
-
-                    listeners = self._listeners.get(listener_name, [])
-                    listeners.append(func)
-                    self._listeners[listener_name] = listeners
-
-            if hasattr(func, "__component_data__"):
-                all_component_data: List[Tuple[tuple, dict]] = func.__component_data__
-                for args, kwargs in all_component_data:
-                    func = client.component(*args, **kwargs)(func)
-
-                    component = kwargs.get("component") or args[0]
-                    comp_name = (
-                        _component(component).custom_id
-                        if isinstance(component, (Button, SelectMenu))
-                        else component
-                    )
-                    comp_name = f"component_{comp_name}"
-
-                    listeners = self._listeners.get(comp_name, [])
-                    listeners.append(func)
-                    self._listeners[comp_name] = listeners
-
-            if hasattr(func, "__autocomplete_data__"):
-                all_args_kwargs = func.__autocomplete_data__
-                for args, kwargs in all_args_kwargs:
-                    func = client.autocomplete(*args, **kwargs)(func)
-
-                    _command = kwargs.get("command") or args[0]
-                    name = kwargs.get("name") or args[1]
-
-                    _command: Union[Snowflake, int] = (
-                        _command.id if isinstance(_command, ApplicationCommand) else _command
-                    )
-
-                    auto_name = f"autocomplete_{_command}_{name}"
-
-                    listeners = self._listeners.get(auto_name, [])
-                    listeners.append(func)
-                    self._listeners[auto_name] = listeners
-
-            if hasattr(func, "__modal_data__"):
-                all_modal_data: List[Tuple[tuple, dict]] = func.__modal_data__
-                for args, kwargs in all_modal_data:
-                    func = client.modal(*args, **kwargs)(func)
-
-                    modal = kwargs.get("modal") or args[0]
-                    _modal_id: str = modal.custom_id if isinstance(modal, Modal) else modal
-                    modal_name = f"modal_{_modal_id}"
-
-                    listeners = self._listeners.get(modal_name, [])
-                    listeners.append(func)
-                    self._listeners[modal_name] = listeners
-
-        for _, cmd in getmembers(self, predicate=lambda command: isinstance(command, Command)):
-            cmd: Command
-
-            if cmd.name in {_cmd.name for _cmd in self.client._commands}:
-                continue
-
-            cmd.extension = self
-            cmd.client = self.client
-            self.client._commands.append(cmd)
-
-            commands = self._commands.get(cmd.name, [])
-            coro = cmd.dispatcher
-            coro = coro.__func__ if hasattr(coro, "__func__") else coro
-            commands.append(coro)
-            self._commands[f"command_{cmd.name}"] = commands
+        Returns:
+            The guilds widget object.
 
-        client._extensions[cls.__name__] = self
+        """
+        return GuildWidget.from_dict(await self._client.http.get_guild_widget(self.id), self._client)
 
-        self.client._Client__resolve_commands()  # noqa
+    async def modify_widget(
+        self,
+        enabled: Absent[bool] = MISSING,
+        channel: Absent[Union["models.TYPE_GUILD_CHANNEL", Snowflake_Type]] = MISSING,
+        settings: Absent["GuildWidgetSettings"] = MISSING,
+    ) -> "GuildWidget":
+        """
+        Modify the guild's widget.
 
-        if client._websocket.ready.is_set() and client._automate_sync:
-            client._loop.create_task(client._Client__sync())  # noqa
+        Args:
+            enabled: Should the widget be enabled?
+            channel: The channel to use in the widget
+            settings: The settings to use for the widget
 
-        return self
+        Returns:
+            The updated guilds widget object.
 
-    async def teardown(self, remove_commands: bool = True):
-        for event, funcs in self._listeners.items():
-            for func in funcs:
-                self.client._websocket._dispatch.events[event].remove(func)
+        """
+        if isinstance(settings, GuildWidgetSettings):
+            enabled = settings.enabled
+            channel = settings.channel_id
 
-        for cmd, funcs in self._commands.items():
-            _cmd: str = cmd.split("_", 1)[1]
+        channel = to_optional_snowflake(channel)
+        return GuildWidget.from_dict(
+            await self._client.http.modify_guild_widget(self.id, enabled, channel), self._client
+        )
 
-            for _coro in self.client._Client__command_coroutines:
-                if _coro._name == _cmd:
-                    self.client._Client__command_coroutines.remove(_coro)  # noqa
-                    break
+    async def fetch_invites(self) -> List["models.Invite"]:
+        """
+        Fetches all invites for the guild.
 
-            for _command in self.client._commands:
-                if _command.name == _cmd:
-                    self.client._commands.remove(_command)
-                    break
+        Returns:
+            A list of invites for the guild.
 
-            for i in range(len(funcs)):
-                self.client._websocket._dispatch.events[cmd].pop(i)  # noqa
+        """
+        invites_data = await self._client.http.get_guild_invites(self.id)
+        return models.Invite.from_list(invites_data, self._client)
 
-        if self.client._automate_sync and remove_commands:
-            await self.client._Client__sync()  # noqa
+    async def fetch_guild_integrations(self) -> List["models.GuildIntegration"]:
+        """
+        Fetches all integrations for the guild.
 
+        Returns:
+            A list of integrations for the guild.
 
-@wraps(Client.command)
-def extension_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(coro) -> Command:
-        cmd = Command(coro=coro, **kwargs)
-        coro.__command_data__ = cmd
-        return cmd
+        """
+        data = await self._client.http.get_guild_integrations(self.id)
+        return [GuildIntegration.from_dict(d | {"guild_id": self.id}, self._client) for d in data]
 
-    return decorator
+    async def search_members(self, query: str, limit: int = 1) -> List["models.Member"]:
+        """
+        Search for members in the guild whose username or nickname starts with a provided string.
 
+        Args:
+            query: Query string to match username(s) and nickname(s) against.
+            limit: Max number of members to return (1-1000)
 
-@wraps(Client.event)
-def extension_listener(func: Optional[Coroutine] = None, name: Optional[str] = None):
-    def decorator(func: Coroutine):
-        if not hasattr(func, "__listener_name__"):
-            func.__listener_name__ = []
-        func.__listener_name__.append(name or func.__name__)
+        Returns:
+            A list of members matching the query.
 
-        return func
+        """
+        data = await self._client.http.search_guild_members(guild_id=self.id, query=query, limit=limit)
+        return [self._client.cache.place_member_data(self.id, _d) for _d in data]
 
-    if func:
-        # allows omitting `()` on `@listener`
-        return decorator(func)
+    async def fetch_voice_regions(self) -> List["models.VoiceRegion"]:
+        """
+        Fetches the voice regions for the guild.
 
-    return decorator
+        Unlike the `Client.fetch_voice_regions` method, this will returns VIP servers when the guild is VIP-enabled.
 
+        Returns:
+            A list of voice regions.
 
-@wraps(Client.component)
-def extension_component(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__component_data__"):
-            func.__component_data__ = []
-        func.__component_data__.append((args, kwargs))
+        """
+        regions_data = await self._client.http.get_guild_voice_regions(self.id)
+        return models.VoiceRegion.from_list(regions_data)
 
-        return func
+    @property
+    def gui_sorted_channels(self) -> list["models.TYPE_GUILD_CHANNEL"]:
+        """Return this guilds channels sorted by their gui positions"""
+        # create a sorted list of objects by their gui position
+        if not self._channel_gui_positions:
+            self._calculate_gui_channel_positions()
+        return [
+            self._client.get_channel(k)
+            for k, v in sorted(self._channel_gui_positions.items(), key=lambda item: item[1])
+        ]
 
-    return decorator
+    def get_channel_gui_position(self, channel_id: "Snowflake_Type") -> int:
+        """
+        Get a given channels gui position.
+
+        Args:
+            channel_id: The ID of the channel to get the gui position for.
 
+        Returns:
+            The gui position of the channel.
+        """
+        if not self._channel_gui_positions:
+            self._calculate_gui_channel_positions()
+        return self._channel_gui_positions.get(to_snowflake(channel_id), 0)
+
+    def _calculate_gui_channel_positions(self) -> list["models.TYPE_GUILD_CHANNEL"]:
+        """
+        Calculates the GUI position for all known channels within this guild.
+
+        Note this is an expensive operation and should only be run when actually required.
+
+        Returns:
+            The list of channels in this guild, sorted by their GUI position.
+        """
+        # sorting is based on this https://github.com/discord/discord-api-docs/issues/4613#issuecomment-1059997612
+        sort_map = {
+            ChannelType.GUILD_NEWS_THREAD: 1,
+            ChannelType.GUILD_PUBLIC_THREAD: 1,
+            ChannelType.GUILD_PRIVATE_THREAD: 1,
+            ChannelType.GUILD_TEXT: 2,
+            ChannelType.GUILD_CATEGORY: 2,
+            ChannelType.GUILD_NEWS: 2,
+            ChannelType.GUILD_FORUM: 2,  # assumed value
+            ChannelType.GUILD_VOICE: 3,
+            ChannelType.GUILD_STAGE_VOICE: 3,
+        }
+
+        def channel_sort_func(a, b) -> int:
+            a_sorting = sort_map.get(a.type, 0)
+            b_sorting = sort_map.get(b.type, 0)
+
+            if a_sorting != b_sorting:
+                return a_sorting - b_sorting
+            return a.position - b.position or a.id - b.id
+
+        sorted_channels = sorted(self.channels, key=cmp_to_key(channel_sort_func))
+
+        for channel in sorted_channels[::-1]:
+            if channel.parent_id:
+                # sort channels under their respective categories
+                sorted_channels.remove(channel)
+                parent_index = sorted_channels.index(channel.category)
+                sorted_channels.insert(parent_index + 1, channel)
+            elif channel.type != ChannelType.GUILD_CATEGORY:
+                # move non-category channels to the top
+                sorted_channels.remove(channel)
+                sorted_channels.insert(0, channel)
+
+        self._channel_gui_positions = {channel.id: i for i, channel in enumerate(sorted_channels)}
+
+        return sorted_channels
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildTemplate(ClientObject):
+    code: str = attrs.field(repr=True, metadata=docs("the template code (unique ID)"))
+    name: str = attrs.field(repr=True, metadata=docs("the name"))
+    description: Optional[str] = attrs.field(repr=False, default=None, metadata=docs("the description"))
+
+    usage_count: int = attrs.field(repr=False, default=0, metadata=docs("number of times this template has been used"))
+
+    creator_id: Snowflake_Type = attrs.field(repr=False, metadata=docs("The ID of the user who created this template"))
+    creator: Optional["models.User"] = attrs.field(
+        repr=False, default=None, metadata=docs("the user who created this template")
+    )
+
+    created_at: "models.Timestamp" = attrs.field(repr=False, metadata=docs("When this template was created"))
+    updated_at: "models.Timestamp" = attrs.field(
+        repr=False, metadata=docs("When this template was last synced to the source guild")
+    )
+
+    source_guild_id: Snowflake_Type = attrs.field(
+        repr=False, metadata=docs("The ID of the guild this template is based on")
+    )
+    guild_snapshot: "models.Guild" = attrs.field(
+        repr=False, metadata=docs("A snapshot of the guild this template contains")
+    )
+
+    is_dirty: bool = attrs.field(
+        repr=False, default=False, metadata=docs("Whether this template has un-synced changes")
+    )
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        data["creator"] = client.cache.place_user_data(data["creator"])
+
+        # todo: partial guild obj that **isn't** cached
+        data["guild_snapshot"] = data.pop("serialized_source_guild")
+        return data
+
+    async def synchronise(self) -> "models.GuildTemplate":
+        """Synchronise the template to the source guild's current state."""
+        data = await self._client.http.sync_guild_template(self.source_guild_id, self.code)
+        self.update_from_dict(data)
+        return self
 
-@wraps(Client.autocomplete)
-def extension_autocomplete(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__autocomplete_data__"):
-            func.__autocomplete_data__ = []
-        func.__autocomplete_data__.append((args, kwargs))
+    async def modify(self, name: Absent[str] = MISSING, description: Absent[str] = MISSING) -> "models.GuildTemplate":
+        """
+        Modify the template's metadata.
 
-        return func
+        Args:
+            name: The name for the template
+            description: The description for the template
 
-    return decorator
+        Returns:
+            The modified template object.
 
+        """
+        data = await self._client.http.modify_guild_template(
+            self.source_guild_id, self.code, name=name, description=description
+        )
+        self.update_from_dict(data)
+        return self
 
-@wraps(Client.modal)
-def extension_modal(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__modal_data__"):
-            func.__modal_data__ = []
-        func.__modal_data__.append((args, kwargs))
+    async def delete(self) -> None:
+        """Delete the guild template."""
+        await self._client.http.delete_guild_template(self.source_guild_id, self.code)
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class GuildWelcomeChannel(ClientObject):
+    channel_id: Snowflake_Type = attrs.field(repr=True, metadata=docs("Welcome Channel ID"))
+    description: str = attrs.field(repr=False, metadata=docs("Welcome Channel description"))
+    emoji_id: Optional[Snowflake_Type] = attrs.field(
+        repr=False, default=None, metadata=docs("Welcome Channel emoji ID if the emoji is custom")
+    )
+    emoji_name: Optional[str] = attrs.field(
+        repr=False,
+        default=None,
+        metadata=docs("Emoji name if custom, unicode character if standard"),
+    )
+
+
+class GuildIntegration(DiscordObject):
+    name: str = attrs.field(repr=True)
+    """The name of the integration"""
+    type: str = attrs.field(repr=True)
+    """integration type (twitch, youtube, or discord)"""
+    enabled: bool = attrs.field(repr=True)
+    """is this integration enabled"""
+    account: dict = attrs.field(
+        repr=False,
+    )
+    """integration account information"""
+    application: Optional["models.Application"] = attrs.field(repr=False, default=None)
+    """The bot/OAuth2 application for discord integrations"""
+    _guild_id: Snowflake_Type = attrs.field(
+        repr=False,
+    )
+
+    syncing: Optional[bool] = attrs.field(repr=False, default=MISSING)
+    """is this integration syncing"""
+    role_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=MISSING)
+    """id that this integration uses for "subscribers\""""
+    enable_emoticons: bool = attrs.field(repr=False, default=MISSING)
+    """whether emoticons should be synced for this integration (twitch only currently)"""
+    expire_behavior: IntegrationExpireBehaviour = attrs.field(
+        repr=False, default=MISSING, converter=optional(IntegrationExpireBehaviour)
+    )
+    """the behavior of expiring subscribers"""
+    expire_grace_period: int = attrs.field(repr=False, default=MISSING)
+    """the grace period (in days) before expiring subscribers"""
+    user: "models.BaseUser" = attrs.field(repr=False, default=MISSING)
+    """user for this integration"""
+    synced_at: "models.Timestamp" = attrs.field(repr=False, default=MISSING, converter=optional(timestamp_converter))
+    """when this integration was last synced"""
+    subscriber_count: int = attrs.field(repr=False, default=MISSING)
+    """how many subscribers this integration has"""
+    revoked: bool = attrs.field(repr=False, default=MISSING)
+    """has this integration been revoked"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if app := data.get("application", None):
+            data["application"] = models.Application.from_dict(app, client)
+        if user := data.get("user", None):
+            data["user"] = client.cache.place_user_data(user)
+
+        return data
+
+    async def delete(self, reason: Absent[str] = MISSING) -> None:
+        """Delete this guild integration."""
+        await self._client.http.delete_guild_integration(self._guild_id, self.id, reason)
+
+
+class GuildWidgetSettings(DictSerializationMixin):
+    enabled: bool = attrs.field(repr=True, default=False)
+    """Whether the widget is enabled."""
+    channel_id: Optional["Snowflake_Type"] = attrs.field(repr=True, default=None, converter=to_optional_snowflake)
+    """The widget channel id. None if widget is not enabled."""
+
+
+class GuildWidget(DiscordObject):
+    name: str = attrs.field(repr=True)
+    """Guild name (2-100 characters)"""
+    instant_invite: str = attrs.field(repr=True, default=None)
+    """Instant invite for the guilds specified widget invite channel"""
+    presence_count: int = attrs.field(repr=True, default=0)
+    """Number of online members in this guild"""
+
+    _channel_ids: List["Snowflake_Type"] = attrs.field(repr=False, default=[])
+    """Voice and stage channels which are accessible by @everyone"""
+    _member_ids: List["Snowflake_Type"] = attrs.field(repr=False, default=[])
+    """Special widget user objects that includes users presence (Limit 100)"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if channels := data.get("channels"):
+            data["channel_ids"] = [channel["id"] for channel in channels]
+        if members := data.get("members"):
+            data["member_ids"] = [member["id"] for member in members]
+        return data
+
+    def get_channels(self) -> List["models.TYPE_VOICE_CHANNEL"]:
+        """
+        Gets voice and stage channels which are accessible by @everyone
+
+        Returns:
+            List of channels
+
+        """
+        return [self._client.get_channel(channel_id) for channel_id in self._channel_ids]
+
+    async def fetch_channels(self) -> List["models.TYPE_VOICE_CHANNEL"]:
+        """
+        Gets voice and stage channels which are accessible by @everyone. Fetches the channels from API if they are not cached.
+
+        Returns:
+            List of channels
+
+        """
+        return [await self._client.fetch_channel(channel_id) for channel_id in self._channel_ids]
+
+    def get_members(self) -> List["models.User"]:
+        """
+        Gets special widget user objects that includes users presence (Limit 100)
+
+        Returns:
+            List of users
+
+        """
+        return [self._client.get_user(member_id) for member_id in self._member_ids]
+
+    async def fetch_members(self) -> List["models.User"]:
+        """
+        Gets special widget user objects that includes users presence (Limit 100). Fetches the users from API if they are not cached.
+
+        Returns:
+            List of users
+
+        """
+        return [await self._client.fetch_user(member_id) for member_id in self._member_ids]
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class AuditLogChange(ClientObject):
+    key: str = attrs.field(repr=True)
+    """name of audit log change key"""
+    new_value: Optional[Union[list, str, int, bool, "Snowflake_Type"]] = attrs.field(repr=False, default=MISSING)
+    """new value of the key"""
+    old_value: Optional[Union[list, str, int, bool, "Snowflake_Type"]] = attrs.field(repr=False, default=MISSING)
+    """old value of the key"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class AuditLogEntry(DiscordObject):
+    target_id: Optional["Snowflake_Type"] = attrs.field(repr=False, converter=optional(to_snowflake))
+    """id of the affected entity (webhook, user, role, etc.)"""
+    user_id: "Snowflake_Type" = attrs.field(repr=False, converter=optional(to_snowflake))
+    """the user who made the changes"""
+    action_type: "AuditLogEventType" = attrs.field(repr=False, converter=AuditLogEventType)
+    """type of action that occurred"""
+    changes: Optional[List[AuditLogChange]] = attrs.field(repr=False, default=MISSING)
+    """changes made to the target_id"""
+    options: Optional[Union["Snowflake_Type", str]] = attrs.field(repr=False, default=MISSING)
+    """additional info for certain action types"""
+    reason: Optional[str] = attrs.field(repr=False, default=MISSING)
+    """the reason for the change (0-512 characters)"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if changes := data.get("changes", None):
+            data["changes"] = AuditLogChange.from_list(changes, client)
+
+        return data
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class AuditLog(ClientObject):
+    """Contains entries and other data given from selected"""
+
+    application_commands: list["InteractionCommand"] = attrs.field(
+        repr=False, factory=list, converter=optional(deserialize_app_cmds)
+    )
+    """list of application commands that have had their permissions updated"""
+    entries: Optional[List["AuditLogEntry"]] = attrs.field(repr=False, default=MISSING)
+    """list of audit log entries"""
+    scheduled_events: Optional[List["models.ScheduledEvent"]] = attrs.field(repr=False, default=MISSING)
+    """list of guild scheduled events found in the audit log"""
+    integrations: Optional[List["GuildIntegration"]] = attrs.field(repr=False, default=MISSING)
+    """list of partial integration objects"""
+    threads: Optional[List["models.ThreadChannel"]] = attrs.field(repr=False, default=MISSING)
+    """list of threads found in the audit log"""
+    users: Optional[List["models.User"]] = attrs.field(repr=False, default=MISSING)
+    """list of users found in the audit log"""
+    webhooks: Optional[List["models.Webhook"]] = attrs.field(repr=False, default=MISSING)
+    """list of webhooks found in the audit log"""
+
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
+        if entries := data.get("audit_log_entries", None):
+            data["entries"] = AuditLogEntry.from_list(entries, client)
+        if scheduled_events := data.get("guild_scheduled_events", None):
+            data["scheduled_events"] = models.ScheduledEvent.from_list(scheduled_events, client)
+        if integrations := data.get("integrations", None):
+            data["integrations"] = GuildIntegration.from_list(integrations, client)
+        if threads := data.get("threads", None):
+            data["threads"] = models.ThreadChannel.from_list(threads, client)
+        if users := data.get("users", None):
+            data["users"] = models.User.from_list(users, client)
+        if webhooks := data.get("webhooks", None):
+            data["webhooks"] = models.Webhook.from_list(webhooks, client)
 
-        return func
+        return data
 
-    return decorator
 
+class AuditLogHistory(AsyncIterator):
+    """
+    An async iterator for searching through a audit log's entry history.
 
-@wraps(Client.message_command)
-def extension_message_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(func) -> Command:
-        kwargs["type"] = ApplicationCommandType.MESSAGE
-        return extension_command(**kwargs)(func)
+    Attributes:
+        guild (:class:`Guild`): The guild to search through.
+        user_id (:class:`Snowflake_Type`): The user ID to search for.
+        action_type (:class:`AuditLogEventType`): The action type to search for.
+        before: get messages before this message ID
+        after: get messages after this message ID
+        limit: The maximum number of entries to return (set to 0 for no limit)
 
-    return decorator
+    """
 
+    def __init__(
+        self,
+        guild: "Guild",
+        user_id: Snowflake_Type = None,
+        action_type: "AuditLogEventType" = None,
+        before: Snowflake_Type = None,
+        after: Snowflake_Type = None,
+        limit: int = 50,
+    ) -> None:
+        self.guild: "Guild" = guild
+        self.user_id: Snowflake_Type = user_id
+        self.action_type: "AuditLogEventType" = action_type
+        self.before: Snowflake_Type = before
+        self.after: Snowflake_Type = after
+        super().__init__(limit)
+
+    async def fetch(self) -> List["AuditLog"]:
+        """
+        Retrieves the audit log entries from discord API.
+
+        Returns:
+            The list of audit log entries.
+
+        """
+        if self.after:
+            if not self.last:
+                self.last = namedtuple("temp", "id")
+                self.last.id = self.after
+            log = await self.guild.fetch_audit_log(limit=self.get_limit, after=self.last.id)
+        else:
+            if self.before and not self.last:
+                self.last = namedtuple("temp", "id")
+                self.last.id = self.before
 
-@wraps(Client.user_command)
-def extension_user_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(func) -> Command:
-        kwargs["type"] = ApplicationCommandType.USER
-        return extension_command(**kwargs)(func)
+            log = await self.guild.fetch_audit_log(limit=self.get_limit, before=self.last.id)
+        entries = log.entries or []
 
-    return decorator
+        return entries
```

### Comparing `discord-py-interactions-4.4.1/interactions/client/context.py` & `discord-py-interactions-5.0.0/interactions/models/internal/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,833 +1,892 @@
-import asyncio
-from contextlib import suppress
-from datetime import datetime
-from logging import Logger
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
-
-from ..api.error import LibraryException
-from ..api.models.channel import Channel, Thread
-from ..api.models.flags import MessageFlags, Permissions
-from ..api.models.guild import Guild
-from ..api.models.member import Member
-from ..api.models.message import Attachment, Embed, File, Message, MessageReference
-from ..api.models.misc import AllowedMentions, Snowflake
-from ..api.models.user import User
-from ..base import get_logger
-from ..utils.attrs_utils import ClientSerializerMixin, convert_int, define, field
-from ..utils.missing import MISSING
-from .enums import ComponentType, InteractionCallbackType, InteractionType, Locale
-from .models.command import Choice
-from .models.component import ActionRow, Button, Modal, SelectMenu, _build_components
-from .models.misc import InteractionData
-
-if TYPE_CHECKING:
-    from .bot import Client, Extension
-    from .models.command import Command
-
-log: Logger = get_logger("context")
+import abc
+import datetime
+import re
+import typing
+from typing_extensions import Self
+
+import discord_typings
+from aiohttp import FormData
+from interactions.client.const import get_logger, MISSING
+from interactions.models.discord.components import BaseComponent
+from interactions.models.discord.file import UPLOADABLE_TYPE
+from interactions.models.discord.sticker import Sticker
+from interactions.models.discord.user import Member, User
+
+from interactions.models.internal.command import BaseCommand
+from interactions.client.mixins.modal import ModalMixin
+
+from interactions.client.errors import HTTPException, AlreadyDeferred, AlreadyResponded
+from interactions.client.mixins.send import SendMixin
+from interactions.models.discord.enums import (
+    Permissions,
+    MessageFlags,
+    InteractionType,
+    ComponentType,
+    CommandType,
+)
+from interactions.models.discord.message import (
+    AllowedMentions,
+    Attachment,
+    Message,
+    MessageReference,
+    process_message_payload,
+)
+from interactions.models.discord.snowflake import Snowflake, Snowflake_Type, to_snowflake, to_optional_snowflake
+from interactions.models.discord.embed import Embed
+from interactions.models.internal.application_commands import (
+    OptionType,
+    CallbackType,
+    SlashCommandOption,
+    InteractionCommand,
+)
 
 __all__ = (
-    "_Context",
-    "CommandContext",
+    "AutocompleteContext",
+    "BaseContext",
+    "BaseInteractionContext",
     "ComponentContext",
+    "ContextMenuContext",
+    "InteractionContext",
+    "ModalContext",
+    "Resolved",
+    "SlashContext",
 )
 
 
-@define()
-class _Context(ClientSerializerMixin):
-    """
-    The base class of "context" for dispatched event data
-    from the gateway. The premise of having this class is so
-    that the user-facing API is able to allow developers to
-    easily access information presented from any event in
-    a "contextualized" sense.
-    """
+if typing.TYPE_CHECKING:
+    import interactions
 
-    message: Optional[Message] = field(converter=Message, default=None, add_client=True)
-    member: Optional[Member] = field(default=None, converter=Member, add_client=True)
-    user: User = field(converter=User, default=None, add_client=True)
-    id: Snowflake = field(converter=Snowflake)
-    application_id: Snowflake = field(converter=Snowflake)
-    type: InteractionType = field(converter=InteractionType)
-    callback: Optional[InteractionCallbackType] = field(
-        converter=InteractionCallbackType, default=None
-    )
-    data: InteractionData = field(converter=InteractionData)
-    version: int = field()
-    token: str = field()
-    guild_id: Snowflake = field(converter=Snowflake)
-    channel_id: Snowflake = field(converter=Snowflake)
-    responded: bool = field(default=False)
-    deferred: bool = field(default=False)
-    app_permissions: Permissions = field(converter=convert_int(Permissions), default=None)
-    locale: Optional[Locale] = field(converter=Locale, default=None)
-    guild_locale: Optional[Locale] = field(converter=Locale, default=None)
-
-    def __attrs_post_init__(self) -> None:
-        if self.member and self.guild_id:
-            self.member._extras["guild_id"] = self.guild_id
 
-        if self.user is None:
-            self.user = self.member.user if self.member else None
+class Resolved:
+    """
+    A class representing the resolved data from an interaction.
 
-        if self.member and not self.member.user and self.user:
-            self.member.user = self.user
+    Attributes:
+        channels: A dictionary of channels resolved from the interaction.
+        members: A dictionary of members resolved from the interaction.
+        users: A dictionary of users resolved from the interaction.
+        roles: A dictionary of roles resolved from the interaction.
+        messages: A dictionary of messages resolved from the interaction.
+        attachments: A dictionary of attachments resolved from the interaction.
+    """
 
-    @property
-    def deferred_ephemeral(self) -> bool:
-        """
-        .. versionadded:: 4.4.0
+    def __init__(self) -> None:
+        self.channels: dict[Snowflake, "interactions.TYPE_MESSAGEABLE_CHANNEL"] = {}
+        self.members: dict[Snowflake, "interactions.Member"] = {}
+        self.users: dict[Snowflake, "interactions.User"] = {}
+        self.roles: dict[Snowflake, "interactions.Role"] = {}
+        self.messages: dict[Snowflake, "interactions.Message"] = {}
+        self.attachments: dict[Snowflake, "interactions.Attachment"] = {}
 
-        Returns whether the current interaction was deferred ephemerally.
-        """
-        return bool(
-            self.message.flags & MessageFlags.EPHEMERAL
-            and self.message.flags & MessageFlags.LOADING
+    def __bool__(self) -> bool:
+        """Returns whether any resolved data is present."""
+        return (
+            bool(self.channels)
+            or bool(self.members)
+            or bool(self.users)
+            or bool(self.roles)
+            or bool(self.messages)
+            or bool(self.attachments)
         )
 
-    @property
-    def created_at(self) -> datetime:
-        """
-        .. versionadded:: 4.4.0
-
-        Returns when the interaction was created.
-        """
-        return self.id.timestamp
-
-    @property
-    def author(self) -> Optional[Member]:
-        """
-        Returns the author/member that invoked the interaction.
-        """
-        return self.member
-
-    @property
-    def channel(self) -> Optional[Channel]:
-        """
-        .. versionadded:: 4.1.0
-
-        .. versionchanged:: 4.4.0
-            Channel now returns ``None`` instead of ``MISSING`` if it is not found to avoid confusion
-
-        Returns the current channel, if cached.
-        """
-        return self._client.cache[Channel].get(self.channel_id, None) or self._client.cache[
-            Thread
-        ].get(self.channel_id, None)
-
-    @property
-    def guild(self) -> Optional[Guild]:
-        """
-         .. versionadded:: 4.1.0
-
-         .. versionchanged:: 4.4.0
-            Guild now returns ``None`` instead of ``MISSING`` if it is not found to avoid confusion
-
-        Returns the current guild, if cached.
-        """
-
-        return self._client.cache[Guild].get(self.guild_id, None)
-
-    async def get_channel(self) -> Channel:
-        """
-        .. versionadded:: 4.1.0
-
-        This gets the channel the context was invoked in. If the channel is not cached, an HTTP request is made.
-
-        :return: The channel as object
-        :rtype: Channel
-        """
-        if channel := self.channel:
-            await asyncio.sleep(0)
+    def get(self, snowflake: Snowflake | str, default: typing.Any = None) -> typing.Any:
+        snowflake = Snowflake(snowflake)
+        """Returns the value of the given snowflake."""
+        if channel := self.channels.get(snowflake):
             return channel
-
-        res = await self._client.get_channel(int(self.channel_id))
-        return Channel(**res, _client=self._client)
-
-    async def get_guild(self) -> Guild:
-        """
-        .. versionadded:: 4.1.0
-
-        This gets the guild the context was invoked in. If the guild is not cached, an HTTP request is made.
-
-        :return: The guild as object
-        :rtype: Guild
-        """
-
-        if guild := self.guild:
-            await asyncio.sleep(0)
-            return guild
-
-        res = await self._client.get_guild(int(self.guild_id))
-        return Guild(**res, _client=self._client)
-
-    async def defer(
-        self, ephemeral: Optional[bool] = False, edit_origin: Optional[bool] = False
-    ) -> Message:
-        """
-        .. versionchanged:: 4.4.0
-            Now returns the created message object
-
-        This "defers" an interaction response, allowing up
-        to a 15-minute delay between invocation and responding.
-
-        :param Optional[bool] ephemeral: Whether the deferred state is hidden or not.
-        :param Optional[bool] edit_origin: Whether you want to edit the original message or send a followup message
-        :return: The deferred message
-        :rtype: Message
-        """
-        if edit_origin and self.type in {
-            InteractionType.APPLICATION_COMMAND,
-            InteractionType.APPLICATION_COMMAND_AUTOCOMPLETE,
-        }:
-            raise LibraryException(
-                message="You cannot defer with edit_origin parameter in this type of interaction"
-            )
-
-        if not self.responded:
-            self.deferred = True
-            is_ephemeral: int = MessageFlags.EPHEMERAL.value if bool(ephemeral) else 0
-            # ephemeral doesn't change callback typings. just data json
-            self.callback = (
-                InteractionCallbackType.DEFERRED_UPDATE_MESSAGE
-                if edit_origin
-                else InteractionCallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE
-            )
-
-            await self._client.create_interaction_response(
-                token=self.token,
-                application_id=int(self.id),
-                data={"type": self.callback.value, "data": {"flags": is_ephemeral}},
-            )
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
+        if member := self.members.get(snowflake):
+            return member
+        if user := self.users.get(snowflake):
+            return user
+        if role := self.roles.get(snowflake):
+            return role
+        if message := self.messages.get(snowflake):
+            return message
+        if attachment := self.attachments.get(snowflake):
+            return attachment
+        return default
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", data: dict, guild_id: None | Snowflake = None) -> Self:
+        instance = cls()
+
+        if channels := data.get("channels"):
+            for key, _channel in channels.items():
+                instance.channels[Snowflake(key)] = client.cache.place_channel_data(_channel)
+
+        if members := data.get("members"):
+            for key, _member in members.items():
+                instance.members[Snowflake(key)] = client.cache.place_member_data(
+                    guild_id, {**_member, "user": {**data["users"][key]}}
                 )
-                _message = Message(**res, _client=self._client)
 
-            self.responded = True
+        if users := data.get("users"):
+            for key, _user in users.items():
+                instance.users[Snowflake(key)] = client.cache.place_user_data(_user)
 
-            return _message
+        if roles := data.get("roles"):
+            for key, _role in roles.items():
+                instance.roles[Snowflake(key)] = client.cache.get_role(Snowflake(key))
 
-    async def send(
-        self,
-        content: Optional[str] = MISSING,
-        *,
-        tts: Optional[bool] = MISSING,
-        attachments: Optional[List[Attachment]] = MISSING,
-        files: Optional[Union[File, List[File]]] = MISSING,
-        embeds: Optional[Union[Embed, List[Embed]]] = MISSING,
-        allowed_mentions: Optional[Union[AllowedMentions, dict]] = MISSING,
-        components: Optional[
-            Union[ActionRow, Button, SelectMenu, List[ActionRow], List[Button], List[SelectMenu]]
-        ] = MISSING,
-        ephemeral: Optional[bool] = False,
-        suppress_embeds: bool = False,
-    ) -> Tuple[dict, List[File]]:
-        """
-        This allows the invocation state described in the "context"
-        to send an interaction response.
+        if messages := data.get("messages"):
+            for key, _msg in messages.items():
+                instance.messages[Snowflake(key)] = client.cache.place_message_data(_msg)
 
-        :param Optional[str] content: The contents of the message as a string or string-converted value.
-        :param Optional[bool] tts: Whether the message utilizes the text-to-speech Discord programme or not.
-        :param Optional[List[Attachment]] attachments: The attachments to attach to the message. Needs to be uploaded to the CDN first
-        :param Optional[Union[File, List[File]]] files:
-            .. versionadded:: 4.4.0
-
-            The files to attach to the message.
-        :param Optional[Union[Embed, List[Embed]]] embeds: An embed, or list of embeds for the message.
-        :param Optional[Union[AllowedMentions, dict]] allowed_mentions: The allowed mentions for the message.
-        :param Optional[Union[ActionRow, Button, SelectMenu, List[Union[ActionRow, Button, SelectMenu]]]] components: A component, or list of components for the message.
-        :param Optional[bool] ephemeral: Whether the response is hidden or not.
-        :param Optional[bool] suppress_embeds: Whether embeds are not shown in the message.
-        :return: The sent message.
-        """
-        if (
-            content is MISSING
-            and self.message
-            and self.callback == InteractionCallbackType.DEFERRED_UPDATE_MESSAGE
-        ):
-            _content = self.message.content
-        else:
-            _content: str = "" if content is MISSING else content
-        _tts: bool = False if tts is MISSING else tts
-
-        if (
-            embeds is MISSING
-            and self.message
-            and self.callback == InteractionCallbackType.DEFERRED_UPDATE_MESSAGE
-        ):
-            embeds = self.message.embeds
-        _embeds: list = (
-            []
-            if not embeds or embeds is MISSING
-            else ([embed._json for embed in embeds] if isinstance(embeds, list) else [embeds._json])
-        )
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
-
-        if components is not MISSING and components:
-            # components could be not missing but an empty list
+        if attachments := data.get("attachments"):
+            for key, _attach in attachments.items():
+                instance.attachments[Snowflake(key)] = Attachment.from_dict(_attach, client)
 
-            _components = _build_components(components=components)
-        elif (
-            components is MISSING
-            and self.message
-            and self.callback == InteractionCallbackType.DEFERRED_UPDATE_MESSAGE
-        ):
-            if isinstance(self.message.components, list):
-                _components = self.message.components
-            else:
-                _components = [self.message.components]
+        return instance
 
-        else:
-            _components = []
 
-        _flags = MessageFlags.EPHEMERAL if ephemeral else MessageFlags(0)
-        if suppress_embeds:
-            _flags |= MessageFlags.SUPPRESS_EMBEDS
+class BaseContext(metaclass=abc.ABCMeta):
+    """
+    Base context class for all contexts.
 
-        _attachments = [] if attachments is MISSING else [a._json for a in attachments]
+    Define your own context class by inheriting from this class. For compatibility with the library, you must define a `from_dict` classmethod that takes a dict and returns an instance of your context class.
 
-        if not files or files is MISSING:
-            _files = []
-        elif isinstance(files, list):
-            _files = [file._json_payload(id) for id, file in enumerate(files)]
-        else:
-            _files = [files._json_payload(0)]
-            files = [files]
+    """
 
-        _files.extend(_attachments)
+    client: "interactions.Client"
+    """The client that created this context."""
 
-        return (
-            dict(
-                content=_content,
-                tts=_tts,
-                embeds=_embeds,
-                allowed_mentions=_allowed_mentions,
-                components=_components,
-                attachments=_files,
-                flags=_flags.value,
-            ),
-            files,
-        )
+    command: BaseCommand
+    """The command this context invokes."""
 
-    async def edit(
-        self,
-        content: Optional[str] = MISSING,
-        *,
-        tts: Optional[bool] = MISSING,
-        attachments: Optional[List[Attachment]] = MISSING,
-        files: Optional[Union[File, List[File]]] = MISSING,
-        embeds: Optional[Union[Embed, List[Embed]]] = MISSING,
-        allowed_mentions: Optional[Union[AllowedMentions, dict]] = MISSING,
-        message_reference: Optional[MessageReference] = MISSING,
-        components: Optional[
-            Union[ActionRow, Button, SelectMenu, List[ActionRow], List[Button], List[SelectMenu]]
-        ] = MISSING,
-    ) -> Tuple[dict, List[File]]:  # sourcery skip: low-code-quality
-        """
-        This allows the invocation state described in the "context"
-        to send an interaction response.
-
-        :param Optional[str] content: The contents of the message as a string or string-converted value.
-        :param Optional[bool] tts: Whether the message utilizes the text-to-speech Discord programme or not.
-        :param Optional[List[Attachment]] attachments: The attachments to attach to the message. Needs to be uploaded to the CDN first
-        :param Optional[Union[File, List[File]]] files:
-            .. versionadded:: 4.4.0
-
-            The files to attach to the message.
-        :param Optional[Union[Embed, List[Embed]]] embeds: An embed, or list of embeds for the message.
-        :param Optional[Union[AllowedMentions, dict]] allowed_mentions: The allowed mentions for the message.
-        :param Optional[MessageReference] message_reference: Include to make your message a reply.
-        :param Optional[Union[ActionRow, Button, SelectMenu, List[Union[ActionRow, Button, SelectMenu]]]] components: A component, or list of components for the message.
-        :return: The edited message.
-        """
-
-        if self.message is None:
-            raise LibraryException(message="There is no message to edit.")
-
-        payload = {}
-
-        if self.message.content is not None or content is not MISSING:
-            _content: str = self.message.content if content is MISSING else content
-            payload["content"] = _content
-
-        _tts: bool = False if tts is MISSING else tts
-        payload["tts"] = _tts
-
-        if self.message.embeds is not None or embeds is not MISSING:
-            if embeds is MISSING:
-                embeds = self.message.embeds
-            _embeds: list = (
-                ([embed._json for embed in embeds] if isinstance(embeds, list) else [embeds._json])
-                if embeds
-                else []
-            )
+    author_id: Snowflake
+    """The id of the user that invoked this context."""
+    channel_id: Snowflake
+    """The id of the channel this context was invoked in."""
+    message_id: Snowflake
+    """The id of the message that invoked this context."""
+
+    guild_id: typing.Optional[Snowflake]
+    """The id of the guild this context was invoked in, if any."""
+
+    def __init__(self, client: "interactions.Client") -> None:
+        self.client = client
+        self.author_id = MISSING
+        self.channel_id = MISSING
+        self.message_id = MISSING
+        self.guild_id = MISSING
 
-            payload["embeds"] = _embeds
+    @property
+    def guild(self) -> typing.Optional["interactions.Guild"]:
+        """The guild this context was invoked in."""
+        return self.client.cache.get_guild(self.guild_id)
 
-        if self.message.attachments is not None or attachments is not MISSING:
-            if attachments is MISSING:
-                attachments = self.message.attachments
-            _attachments: list = (
-                (
-                    [attachment._json for attachment in attachments]
-                    if isinstance(attachments, list)
-                    else [attachments._json]
-                )
-                if attachments
-                else []
-            )
+    @property
+    def user(self) -> "interactions.User":
+        """The user that invoked this context."""
+        return self.client.cache.get_user(self.author_id)
 
-        if not files or files is MISSING:
-            _files = []
-        elif isinstance(files, list):
-            _files = [file._json_payload(id) for id, file in enumerate(files)]
-        else:
-            _files = [files._json_payload(0)]
-            files = [files]
+    @property
+    def member(self) -> typing.Optional["interactions.Member"]:
+        """The member object that invoked this context."""
+        return self.client.cache.get_member(self.guild_id, self.author_id)
 
-        _files.extend(_attachments)
+    @property
+    def author(self) -> "interactions.Member | interactions.User":
+        """The member or user that invoked this context."""
+        return self.member or self.user
 
-        payload["attachments"] = _files
+    @property
+    def channel(self) -> "interactions.TYPE_MESSAGEABLE_CHANNEL":
+        """The channel this context was invoked in."""
+        if self.guild_id:
+            return self.client.cache.get_channel(self.channel_id)
+        return self.client.cache.get_dm_channel(self.author_id)
 
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
-        _message_reference: dict = {} if message_reference is MISSING else message_reference._json
+    @property
+    def message(self) -> typing.Optional["interactions.Message"]:
+        """The message that invoked this context, if any."""
+        return self.client.cache.get_message(self.channel_id, self.message_id)
 
-        payload["allowed_mentions"] = _allowed_mentions
-        payload["message_reference"] = _message_reference
+    @property
+    def voice_state(self) -> typing.Optional["interactions.VoiceState"]:
+        """The current voice state of the bot in the guild this context was invoked in, if any."""
+        return self.client.cache.get_bot_voice_state(self.guild_id)
 
-        if self.message.components is not None or components is not MISSING:
-            if components is MISSING:
-                _components = _build_components(components=self.message.components)
-            elif not components:
-                _components = []
-            else:
-                _components = _build_components(components=components)
+    @property
+    def bot(self) -> "interactions.Client":
+        return self.client
 
-            payload["components"] = _components
+    @classmethod
+    @abc.abstractmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        """
+        Create a context instance from a dict.
+
+        Args:
+            client: The client creating this context.
+            payload: The dict to create the context from.
+
+        Returns:
+            The context instance.
+
+        """
+        raise NotImplementedError
+
+
+class BaseInteractionContext(BaseContext):
+    token: str
+    """The interaction token."""
+    id: Snowflake
+    """The interaction ID."""
+
+    app_permissions: Permissions
+    """The permissions available to this interaction"""
+    locale: str
+    """The selected locale of the invoking user (https://discord.com/developers/docs/reference#locales)"""
+    guild_locale: str
+    """The selected locale of the invoking user's guild (https://discord.com/developers/docs/reference#locales)"""
+    resolved: Resolved
+    """The resolved data for this interaction."""
+
+    # state info
+    deferred: bool
+    """Whether the interaction has been deferred."""
+    responded: bool
+    """Whether the interaction has been responded to."""
+    ephemeral: bool
+    """Whether the interaction response is ephemeral."""
+
+    _context_type: int
+    """The context type of the interaction."""
+    command_id: Snowflake
+    """The command ID of the interaction."""
+    _command_name: str
+    """The command name of the interaction."""
+
+    args: list[typing.Any]
+    """The arguments passed to the interaction."""
+    kwargs: dict[str, typing.Any]
+    """The keyword arguments passed to the interaction."""
+
+    def __init__(self, client: "interactions.Client") -> None:
+        super().__init__(client)
+        self.deferred = False
+        self.responded = False
+        self.ephemeral = False
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        instance = cls(client=client)
+        instance.token = payload["token"]
+        instance.id = Snowflake(payload["id"])
+        instance.app_permissions = Permissions(payload.get("app_permissions", 0))
+        instance.locale = payload["locale"]
+        instance.guild_locale = payload.get("guild_locale", instance.locale)
+        instance._context_type = payload.get("type", 0)
+        instance.resolved = Resolved.from_dict(client, payload["data"].get("resolved", {}), payload.get("guild_id"))
+
+        instance.channel_id = Snowflake(payload["channel_id"])
+        if member := payload.get("member"):
+            instance.author_id = Snowflake(member["user"]["id"])
+            instance.guild_id = Snowflake(payload["guild_id"])
+            client.cache.place_member_data(instance.guild_id, member)
+        else:
+            instance.author_id = Snowflake(payload["user"]["id"])
+            client.cache.place_user_data(payload["user"])
+
+        if message_data := payload.get("message"):
+            message = client.cache.place_message_data(message_data)
+            instance.message_id = message.id
+
+        instance.guild_id = to_optional_snowflake(payload.get("guild_id"))
+
+        if payload["type"] in (InteractionType.APPLICATION_COMMAND, InteractionType.AUTOCOMPLETE):
+            instance.command_id = Snowflake(payload["data"]["id"])
+            instance._command_name = payload["data"]["name"]
 
-        return payload, files
+        instance.process_options(payload)
 
-    async def popup(self, modal: Modal) -> dict:
-        """
-        This "pops up" a modal to present information back to the
-        user.
+        return instance
 
-        :param Modal modal: The components you wish to show.
-        """
+    @property
+    def command(self) -> InteractionCommand:
+        return self.client._interaction_lookup[self._command_name]
 
-        payload: dict = {
-            "type": InteractionCallbackType.MODAL.value,
-            "data": {
-                "title": modal.title,
-                "components": modal._json.get("components"),
-                "custom_id": modal.custom_id,
-            },
-        }
+    @property
+    def expires_at(self) -> typing.Optional[datetime.datetime]:
+        """The time at which the interaction expires."""
+        if self.responded:
+            return self.id.created_at + datetime.timedelta(minutes=15)
+        return self.id.created_at + datetime.timedelta(seconds=3)
 
-        await self._client.create_interaction_response(
-            token=self.token,
-            application_id=int(self.id),
-            data=payload,
-        )
-        self.responded = True
+    @property
+    def expired(self) -> bool:
+        """Whether the interaction has expired."""
+        return datetime.datetime.utcnow() > self.expires_at
 
-        return payload
+    @property
+    def invoke_target(self) -> str:
+        """The invoke target of the interaction."""
+        return self._command_name
 
-    async def has_permissions(
-        self, *permissions: Union[int, Permissions], operator: str = "and"
-    ) -> bool:
-        r"""
-        .. versionadded:: 4.3.2
-
-        Returns whether the author of the interaction has the permissions in the given context.
-
-        :param Union[int, Permissions] \*permissions: The list of permissions
-        :param Optional[str] operator: The operator to use to calculate permissions. Possible values: ``and``, ``or``. Defaults to ``and``.
-        :return: Whether the author has the permissions
-        :rtype: bool
-        """
-        if operator == "and":
-            return all(perm in self.author.permissions for perm in permissions)
-        else:
-            return any(perm in self.author.permissions for perm in permissions)
+    @property
+    def deferred_ephemeral(self) -> bool:
+        """Whether the interaction has been deferred ephemerally."""
+        return self.deferred and self.ephemeral
 
-    async def delete(self) -> None:
+    def option_processing_hook(self, option: dict) -> typing.Any:
         """
-        This deletes the interaction response of a message sent by
-        the contextually derived information from this class.
+        Hook for extending options processing.
 
-        .. note::
-            Doing this will proceed in the context message no longer
-            being present.
-        """
-        if self.responded and self.message is not None:
-            await self._client.delete_interaction_response(
-                application_id=str(self.application_id),
-                token=self.token,
-                message_id=int(self.message.id),
-            )
-        else:
-            await self._client.delete_interaction_response(
-                application_id=str(self.application_id), token=self.token
-            )
+        This is called for each option, before the library processes it. If this returns a value, the library will not process the option further.
 
-        self.message = None
+        Args:
+            option: The option to process.
 
+        Returns:
+            The processed option.
 
-@define()
-class CommandContext(_Context):
-    """
-    A derivation of context
-    designed specifically for application command data.
+        """
+        return option
 
-    :ivar Snowflake id: The ID of the interaction.
-    :ivar Snowflake application_id: The application ID of the interaction.
-    :ivar InteractionType type: The type of interaction.
-    :ivar InteractionData data: The application command data.
-    :ivar Optional[Union[Message, Member, User]] target: The target selected if this interaction is invoked as a context menu.
-    :ivar str token: The token of the interaction response.
-    :ivar Snowflake guild_id: The ID of the current guild.
-    :ivar Snowflake channel_id: The ID of the current channel.
-    :ivar User user: The user data model.
-    :ivar bool responded: Whether an original response was made or not.
-    :ivar bool deferred: Whether the response was deferred or not.
-    :ivar Optional[Locale] locale: The selected language of the user invoking the interaction.
-    :ivar Optional[Locale] guild_locale: The guild's preferred language, if invoked in a guild.
-    :ivar Permissions app_permissions: Bitwise set of permissions the bot has within the channel the interaction was sent from.
-    :ivar Client client:
-        .. versionadded:: 4.3.0
-
-        The client instance that the command belongs to.
-    :ivar Command command:
-        .. versionadded:: 4.3.0
-
-        The command object that is being invoked.
-    :ivar Extension extension:
-        .. versionadded:: 4.3.0
+    def process_options(self, data: discord_typings.InteractionCallbackData) -> None:
+        if data["type"] not in (InteractionType.APPLICATION_COMMAND, InteractionType.AUTOCOMPLETE):
+            self.args = []
+            self.kwargs = {}
+            return
 
-        The extension the command belongs to.
-    """
+        def gather_options(_options: list[dict[str, typing.Any]]) -> dict[str, typing.Any]:
+            """Recursively gather options from an option list."""
+            kwargs = {}
+            for option in _options:
+                if hook_result := self.option_processing_hook(option):
+                    kwargs[option["name"]] = hook_result
 
-    target: Optional[Union[Message, Member, User]] = field(default=None)
+                if option["type"] in (OptionType.SUB_COMMAND, OptionType.SUB_COMMAND_GROUP):
+                    self._command_name = f"{self._command_name} {option['name']}"
+                    return gather_options(option["options"])
 
-    client: "Client" = field(default=None, init=False)
-    command: "Command" = field(default=None, init=False)
-    extension: "Extension" = field(default=None, init=False)
-
-    def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
-
-        if self.data.target_id:
-            target = self.data.target_id
-
-            if self.data.type == 2:
-                self.target = (
-                    self.data.resolved.members[target]
-                    if self.guild_id and str(self.data.target_id) in self.data.resolved.members
-                    else self.data.resolved.users[target]
-                )
-                # member id would have potential to exist, and therefore have target def priority.
+                value = option.get("value")
 
-            elif self.data.type == 3:
-                self.target = self.data.resolved.messages[target]
+                if option["type"] in OptionType.resolvable_types():
+                    value = self.resolved.get(value, value)
 
-            self.target._client = self._client
+                kwargs[option["name"]] = value
+            return kwargs
 
-    async def edit(
-        self, content: Optional[str] = MISSING, **kwargs
-    ) -> Message:  # sourcery skip: low-code-quality
-        payload, files = await super().edit(content, **kwargs)
-        msg = None
-
-        if self.deferred or self.responded:
-            res = await self._client.edit_interaction_response(
-                data=payload,
-                files=files,
-                token=self.token,
-                application_id=str(self.application_id),
-            )
-            self.message = msg = Message(**res, _client=self._client)
+        if options := data["data"].get("options"):
+            self.kwargs = gather_options(options)  # type: ignore
         else:
-            self.callback = InteractionCallbackType.UPDATE_MESSAGE
-            await self._client.create_interaction_response(
-                data={"type": self.callback.value, "data": payload},
-                files=files,
-                token=self.token,
-                application_id=int(self.id),
-            )
-
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
-                )
-                self.message = msg = Message(**res, _client=self._client)
-
-            self.responded = True
+            self.kwargs = {}
+        self.args = list(self.kwargs.values())
 
-        return msg or Message(**payload, _client=self._client)
 
-    async def send(self, content: Optional[str] = MISSING, **kwargs) -> Message:
-        payload, files = await super().send(content, **kwargs)
-
-        if not self.deferred:
-            self.callback = InteractionCallbackType.CHANNEL_MESSAGE_WITH_SOURCE
+class InteractionContext(BaseInteractionContext, SendMixin):
+    async def defer(self, *, ephemeral: bool = False) -> None:
+        """
+        Defer the interaction.
 
-        _payload: dict = {"type": self.callback.value, "data": payload}
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
 
-        msg = None
+        payload = {"type": CallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE}
+        if ephemeral:
+            payload["data"] = {"flags": MessageFlags.EPHEMERAL}
+
+        await self.client.http.post_initial_response(payload, self.id, self.token)
+        self.deferred = True
+        self.ephemeral = ephemeral
+
+    async def _send_http_request(
+        self, message_payload: dict, files: typing.Iterable["UPLOADABLE_TYPE"] | None = None
+    ) -> dict:
         if self.responded:
-            res = await self._client._post_followup(
-                data=payload,
-                files=files,
-                token=self.token,
-                application_id=str(self.application_id),
+            message_data = await self.client.http.post_followup(
+                message_payload, self.client.app.id, self.token, files=files
             )
-            self.message = msg = Message(**res, _client=self._client)
         else:
-            await self._client.create_interaction_response(
-                token=self.token,
-                application_id=int(self.id),
-                data=_payload,
-                files=files,
-            )
-
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
+            if isinstance(message_payload, FormData) and not self.deferred:
+                await self.defer(ephemeral=self.ephemeral)
+            if self.deferred:
+                message_data = await self.client.http.edit_interaction_message(
+                    message_payload, self.client.app.id, self.token, files=files
                 )
-                self.message = msg = Message(**res, _client=self._client)
+            else:
+                payload = {
+                    "type": CallbackType.CHANNEL_MESSAGE_WITH_SOURCE,
+                    "data": message_payload,
+                }
+                message_data = await self.client.http.post_initial_response(payload, self.id, self.token, files=files)
+
+        if not message_data:
+            try:
+                message_data = await self.client.http.get_interaction_message(self.client.app.id, self.token)
+            except HTTPException:
+                pass
 
-            self.responded = True
+        self.responded = True
+        return message_data
 
-        return msg or Message(
-            **payload,
-            _client=self._client,
-            author={"_client": self._client, "id": None, "username": None, "discriminator": None},
+    async def send(
+        self,
+        content: typing.Optional[str] = None,
+        *,
+        embeds: typing.Optional[
+            typing.Union[typing.Iterable[typing.Union["Embed", dict]], typing.Union["Embed", dict]]
+        ] = None,
+        embed: typing.Optional[typing.Union["Embed", dict]] = None,
+        components: typing.Optional[
+            typing.Union[
+                typing.Iterable[typing.Iterable[typing.Union["BaseComponent", dict]]],
+                typing.Iterable[typing.Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        stickers: typing.Optional[
+            typing.Union[
+                typing.Iterable[typing.Union["Sticker", "Snowflake_Type"]],
+                "Sticker",
+                "Snowflake_Type",
+            ]
+        ] = None,
+        allowed_mentions: typing.Optional[typing.Union["AllowedMentions", dict]] = None,
+        reply_to: typing.Optional[typing.Union["MessageReference", "Message", dict, "Snowflake_Type"]] = None,
+        files: typing.Optional[typing.Union["UPLOADABLE_TYPE", typing.Iterable["UPLOADABLE_TYPE"]]] = None,
+        file: typing.Optional["UPLOADABLE_TYPE"] = None,
+        tts: bool = False,
+        suppress_embeds: bool = False,
+        silent: bool = False,
+        flags: typing.Optional[typing.Union[int, "MessageFlags"]] = None,
+        delete_after: typing.Optional[float] = None,
+        ephemeral: bool = False,
+        **kwargs: typing.Any,
+    ) -> "interactions.Message":
+        """
+        Send a message.
+
+        Args:
+            content: Message text content.
+            embeds: Embedded rich content (up to 6000 characters).
+            embed: Embedded rich content (up to 6000 characters).
+            components: The components to include with the message.
+            stickers: IDs of up to 3 stickers in the server to send in the message.
+            allowed_mentions: Allowed mentions for the message.
+            reply_to: Message to reference, must be from the same channel.
+            files: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            file: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            tts: Should this message use Text To Speech.
+            suppress_embeds: Should embeds be suppressed on this send
+            silent: Should this message be sent without triggering a notification.
+            flags: Message flags to apply.
+            delete_after: Delete message after this many seconds.
+            ephemeral: Whether the response should be ephemeral
+
+        Returns:
+            New message object that was sent.
+        """
+        flags = MessageFlags(flags or 0)
+        if ephemeral:
+            flags |= MessageFlags.EPHEMERAL
+            self.ephemeral = True
+        if suppress_embeds:
+            flags |= MessageFlags.SUPPRESS_EMBEDS
+        if silent:
+            flags |= MessageFlags.SILENT
+
+        return await super().send(
+            content=content,
+            embeds=embeds,
+            embed=embed,
+            components=components,
+            stickers=stickers,
+            allowed_mentions=allowed_mentions,
+            reply_to=reply_to,
+            files=files,
+            file=file,
+            tts=tts,
+            flags=flags,
+            delete_after=delete_after,
+            **kwargs,
         )
 
-    async def populate(self, choices: Union[Choice, List[Choice]]) -> List[Choice]:
+    respond = send
+
+    async def delete(self, message: "Snowflake_Type") -> None:
         """
-        This "populates" the list of choices that the client-end
-        user will be able to select from in the autocomplete field.
+        Delete a message sent in response to this interaction.
 
-        .. warning::
-            Only a maximum of ``25`` choices may be presented
-            within an autocomplete option.
-
-        :param Union[Choice, List[Choice]] choices: The choices you wish to present.
-        :return: The list of choices you've given.
-        :rtype: List[Choice]
-        """
-
-        _choices: Union[list, None] = []
-
-        if not choices or (isinstance(choices, list) and len(choices) == 0):
-            _choices = None
-        elif isinstance(choices, Choice):
-            _choices.append(choices._json)
-        elif isinstance(choices, list) and all(isinstance(choice, Choice) for choice in choices):
-            _choices = [choice._json for choice in choices]
-        elif all(
-            isinstance(choice, dict) and all(isinstance(x, str) for x in choice)
-            for choice in choices
-        ):
-            _choices = list(choices)
-        else:
-            raise LibraryException(6, message="Autocomplete choice items must be of type Choice")
+        Args:
+            message: The message to delete
+        """
+        await self.client.http.delete_interaction_message(self.client.app.id, self.token, to_snowflake(message))
 
-        await self._client.create_interaction_response(
-            token=self.token,
-            application_id=int(self.id),
-            data={
-                "type": InteractionCallbackType.APPLICATION_COMMAND_AUTOCOMPLETE_RESULT.value,
-                "data": {"choices": _choices},
-            },
+    async def edit(
+        self,
+        message: "Snowflake_Type",
+        *,
+        content: typing.Optional[str] = None,
+        embeds: typing.Optional[
+            typing.Union[typing.Iterable[typing.Union["Embed", dict]], typing.Union["Embed", dict]]
+        ] = None,
+        embed: typing.Optional[typing.Union["Embed", dict]] = None,
+        components: typing.Optional[
+            typing.Union[
+                typing.Iterable[typing.Iterable[typing.Union["BaseComponent", dict]]],
+                typing.Iterable[typing.Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        attachments: typing.Optional[typing.Sequence[Attachment | dict]] = None,
+        allowed_mentions: typing.Optional[typing.Union["AllowedMentions", dict]] = None,
+        files: typing.Optional[typing.Union["UPLOADABLE_TYPE", typing.Iterable["UPLOADABLE_TYPE"]]] = None,
+        file: typing.Optional["UPLOADABLE_TYPE"] = None,
+        tts: bool = False,
+    ) -> "interactions.Message":
+        message_payload = process_message_payload(
+            content=content,
+            embeds=embeds or embed,
+            components=components,
+            allowed_mentions=allowed_mentions,
+            attachments=attachments,
+            tts=tts,
         )
 
-        return _choices
-
-
-@define()
-class ComponentContext(_Context):
-    """
-    A derivation of context
-    designed specifically for component data.
-
-    :ivar Snowflake id: The ID of the interaction.
-    :ivar Snowflake application_id: The application ID of the interaction.
-    :ivar InteractionType type: The type of interaction.
-    :ivar InteractionData data: The application command data.
-    :ivar str token: The token of the interaction response.
-    :ivar Snowflake guild_id: The ID of the current guild.
-    :ivar Snowflake channel_id: The ID of the current channel.
-    :ivar Optional[Message] message: The message data model.
-    :ivar User user: The user data model.
-    :ivar bool responded: Whether an original response was made or not.
-    :ivar bool deferred: Whether the response was deferred or not.
-    :ivar Optional[Locale] locale: The selected language of the user invoking the interaction.
-    :ivar Optional[Locale] guild_locale: The guild's preferred language, if invoked in a guild.
-    :ivar Permissions app_permissions: Bitwise set of permissions the bot has within the channel the interaction was sent from.
-    """
+        if file:
+            files = [file, *files] if files else [file]
+        message_data = await self.client.http.edit_interaction_message(
+            payload=message_payload,
+            application_id=self.client.app.id,
+            token=self.token,
+            message_id=to_snowflake(message),
+            files=files,
+        )
+        if message_data:
+            return self.client.cache.place_message_data(message_data)
 
-    async def edit(self, content: Optional[str] = MISSING, **kwargs) -> Message:
-        payload, files = await super().edit(content, **kwargs)
-        msg = None
-
-        if not self.deferred:
-            self.callback = InteractionCallbackType.UPDATE_MESSAGE
-            await self._client.create_interaction_response(
-                data={"type": self.callback.value, "data": payload},
-                files=files,
-                token=self.token,
-                application_id=int(self.id),
-            )
 
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
-                )
+class SlashContext(InteractionContext, ModalMixin):
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        return super().from_dict(client, payload)
 
-                self.message = msg = Message(**res, _client=self._client)
 
-            self.responded = True
-        elif self.callback != InteractionCallbackType.DEFERRED_UPDATE_MESSAGE:
-            await self._client._post_followup(
-                data=payload,
-                files=files,
-                token=self.token,
-                application_id=str(self.application_id),
-            )
-        else:
-            res = await self._client.edit_interaction_response(
-                data=payload,
-                files=files,
-                token=self.token,
-                application_id=str(self.application_id),
-            )
-            self.responded = True
-            self.message = msg = Message(**res, _client=self._client)
-
-        return msg or Message(**payload, _client=self._client)
+class ContextMenuContext(InteractionContext, ModalMixin):
+    target_id: Snowflake
+    """The id of the target of the context menu."""
+    editing_origin: bool
+    """Whether you have deferred the interaction and are editing the original response."""
+    target_type: None | CommandType
+    """The type of the target of the context menu."""
 
-    async def send(self, content: Optional[str] = MISSING, **kwargs) -> Message:
-        payload, files = await super().send(content, **kwargs)
+    def __init__(self, client: "interactions.Client") -> None:
+        super().__init__(client)
+        self.editing_origin = False
 
-        if not self.deferred:
-            self.callback = InteractionCallbackType.CHANNEL_MESSAGE_WITH_SOURCE
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        instance = super().from_dict(client, payload)
+        instance.target_id = Snowflake(payload["data"]["target_id"])
+        instance.target_type = CommandType(payload["data"]["type"])
+        return instance
 
-        _payload: dict = {"type": self.callback.value, "data": payload}
+    async def defer(self, *, ephemeral: bool = False, edit_origin: bool = False) -> None:
+        """
+        Defer the interaction.
 
-        msg = None
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+            edit_origin: Whether to edit the original message instead of sending a new one.
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
         if self.responded:
-            res = await self._client._post_followup(
-                data=payload,
-                files=files,
-                token=self.token,
-                application_id=str(self.application_id),
-            )
-            self.message = msg = Message(**res, _client=self._client)
-        else:
-            await self._client.create_interaction_response(
-                token=self.token,
-                application_id=int(self.id),
-                data=_payload,
-                files=files,
-            )
-
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
-                )
-                self.message = msg = Message(**res, _client=self._client)
+            raise AlreadyResponded("Interaction has already been responded to.")
 
-            self.responded = True
+        payload = {
+            "type": CallbackType.DEFERRED_UPDATE_MESSAGE
+            if edit_origin
+            else CallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE
+        }
+        if ephemeral:
+            if edit_origin:
+                raise ValueError("Cannot use ephemeral and edit_origin together.")
+            payload["data"] = {"flags": MessageFlags.EPHEMERAL}
+
+        await self.client.http.post_initial_response(payload, self.id, self.token)
+        self.deferred = True
+        self.ephemeral = ephemeral
+        self.editing_origin = edit_origin
 
-        return msg if msg is not None else Message(**payload, _client=self._client)
+    @property
+    def target(self) -> None | Message | User | Member:
+        """
+        The target of the context menu.
 
-    async def disable_all_components(
-        self, respond_to_interaction: Optional[bool] = True, **other_kwargs: Optional[dict]
-    ) -> Message:
-        r"""
-        .. versionadded:: 4.3.2
+        Returns:
+            The target of the context menu.
+        """
+        return self.resolved.get(self.target_id)
 
-        Disables all components of the message.
 
-        :param Optional[bool] respond_to_interaction: Whether the components should be disabled in an interaction response, default True
-        :param Optional[dict] \**other_kwargs: Additional keyword-arguments to pass to the edit method. This only works when this method is used as interaction response and takes the same arguments as :func:`ComponentContext.edit()`
+class ComponentContext(InteractionContext, ModalMixin):
+    values: list[str]
+    """The values of the SelectMenu component, if any."""
+    custom_id: str
+    """The custom_id of the component."""
+    component_type: int
+    """The type of the component."""
+    defer_edit_origin: bool
+    """Whether you have deferred the interaction and are editing the original response."""
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        instance = super().from_dict(client, payload)
+        instance.values = payload["data"].get("values", [])
+        instance.custom_id = payload["data"]["custom_id"]
+        instance._command_id = instance.custom_id
+        instance._command_name = instance.custom_id
+        instance.component_type = payload["data"]["component_type"]
+        instance.defer_edit_origin = False
+
+        searches = {
+            "users": instance.component_type in (ComponentType.USER_SELECT, ComponentType.MENTIONABLE_SELECT),
+            "members": instance.guild_id
+            and instance.component_type in (ComponentType.USER_SELECT, ComponentType.MENTIONABLE_SELECT),
+            "channels": instance.component_type in (ComponentType.CHANNEL_SELECT, ComponentType.MENTIONABLE_SELECT),
+            "roles": instance.guild_id
+            and instance.component_type in (ComponentType.ROLE_SELECT, ComponentType.MENTIONABLE_SELECT),
+        }
 
-        :return: The modified Message
-        :rtype: Message
+        if instance.component_type in (
+            ComponentType.USER_SELECT,
+            ComponentType.CHANNEL_SELECT,
+            ComponentType.ROLE_SELECT,
+            ComponentType.MENTIONABLE_SELECT,
+        ):
+            for i, value in enumerate(instance.values):
+                if re.match(r"\d{17,}", value):
+                    key = Snowflake(value)
+
+                    if resolved := instance.resolved.get(key):
+                        instance.values[i] = resolved
+                    elif searches["members"] and (member := instance.client.cache.get_member(instance.guild_id, key)):
+                        instance.values[i] = member
+                    elif searches["users"] and (user := instance.client.cache.get_user(key)):
+                        instance.values[i] = user
+                    elif searches["roles"] and (role := instance.client.cache.get_role(key)):
+                        instance.values[i] = role
+                    elif searches["channels"] and (channel := instance.client.cache.get_channel(key)):
+                        instance.values[i] = channel
+        return instance
+
+    async def defer(self, *, ephemeral: bool = False, edit_origin: bool = False) -> None:
+        """
+        Defer the interaction.
+
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+            edit_origin: Whether to edit the original message instead of sending a new one.
         """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
 
-        if not respond_to_interaction:
-            return await self.message.disable_all_components()
+        payload = {
+            "type": CallbackType.DEFERRED_UPDATE_MESSAGE
+            if edit_origin
+            else CallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE
+        }
+        if ephemeral:
+            if edit_origin:
+                raise ValueError("Cannot use ephemeral and edit_origin together.")
+            payload["data"] = {"flags": MessageFlags.EPHEMERAL}
+
+        await self.client.http.post_initial_response(payload, self.id, self.token)
+        self.deferred = True
+        self.ephemeral = ephemeral
+        self.editing_origin = edit_origin
 
-        for components in self.message.components:
-            for component in components.components:
-                component.disabled = True
+    async def edit_origin(
+        self,
+        *,
+        content: typing.Optional[str] = None,
+        embeds: typing.Optional[
+            typing.Union[typing.Iterable[typing.Union["Embed", dict]], typing.Union["Embed", dict]]
+        ] = None,
+        embed: typing.Optional[typing.Union["Embed", dict]] = None,
+        components: typing.Optional[
+            typing.Union[
+                typing.Iterable[typing.Iterable[typing.Union["BaseComponent", dict]]],
+                typing.Iterable[typing.Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        allowed_mentions: typing.Optional[typing.Union["AllowedMentions", dict]] = None,
+        files: typing.Optional[typing.Union["UPLOADABLE_TYPE", typing.Iterable["UPLOADABLE_TYPE"]]] = None,
+        file: typing.Optional["UPLOADABLE_TYPE"] = None,
+        tts: bool = False,
+    ) -> "Message":
+        """
+        Edits the original message of the component.
+
+        Args:
+            content: Message text content.
+            embeds: Embedded rich content (up to 6000 characters).
+            embed: Embedded rich content (up to 6000 characters).
+            components: The components to include with the message.
+            allowed_mentions: Allowed mentions for the message.
+            files: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            file: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
+            tts: Should this message use Text To Speech.
+
+        Returns:
+            The message after it was edited.
+        """
+        if not self.responded and not self.deferred and (files or file):
+            # Discord doesn't allow files at initial response, so we defer then edit.
+            await self.defer(edit_origin=True)
+
+        message_payload = process_message_payload(
+            content=content,
+            embeds=embeds or embed,
+            components=components,
+            allowed_mentions=allowed_mentions,
+            tts=tts,
+        )
+
+        message_data = None
+        if self.deferred:
+            if not self.editing_origin:
+                get_logger().warning(
+                    "If you want to edit the original message, and need to defer, you must set the `edit_origin` kwarg to True!"
+                )
 
-        if other_kwargs.get("components"):
-            raise LibraryException(
-                12, "You must not specify the `components` argument in this method."
+            message_data = await self.client.http.edit_interaction_message(
+                message_payload, self.client.app.id, self.token, files=files or file
             )
+            self.deferred = False
+            self.editing_origin = False
+        else:
+            payload = {"type": CallbackType.UPDATE_MESSAGE, "data": message_payload}
+            await self.client.http.post_initial_response(payload, str(self.id), self.token, files=files or file)
+            message_data = await self.client.http.get_interaction_message(self.client.app.id, self.token)
+
+        if message_data:
+            message = self.client.cache.place_message_data(message_data)
+            self.message_id = message.id
+            return message
+
+
+class ModalContext(InteractionContext):
+    responses: dict[str, str]
+    """The responses of the modal. The key is the `custom_id` of the component."""
+    custom_id: str
+    """The developer defined custom ID of this modal"""
+    edit_origin: bool
+    """Whether to edit the original message instead of sending a new one."""
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        instance = super().from_dict(client, payload)
+        instance.responses = {
+            comp["components"][0]["custom_id"]: comp["components"][0]["value"] for comp in payload["data"]["components"]
+        }
+        instance.kwargs = instance.responses
+        instance.custom_id = payload["data"]["custom_id"]
+        instance.edit_origin = False
+        return instance
+
+    async def edit(self, message: "Snowflake_Type", **kwargs) -> "interactions.Message":
+        if not self.deferred and not self.responded:
+            await self.defer(edit_origin=True)
+        return await super().edit(message, **kwargs)
+
+    async def defer(self, *, ephemeral: bool = False, edit_origin: bool = False) -> None:
+        """
+        Defer the interaction.
+
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+            edit_origin: Whether to edit the original message instead of sending a followup.
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
 
-        other_kwargs["components"] = self.message.components
-        return await self.edit(**other_kwargs)
+        payload = {
+            "type": CallbackType.DEFERRED_UPDATE_MESSAGE
+            if edit_origin
+            else CallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE
+        }
+        if ephemeral:
+            payload["data"] = {"flags": MessageFlags.EPHEMERAL}
 
-    @property
-    def custom_id(self) -> Optional[str]:
-        """
-        The custom ID of the interacted component.
+        if edit_origin:
+            self.edit_origin = True
 
-        :rtype: Optional[str]
-        """
-        return self.data.custom_id
+        await self.client.http.post_initial_response(payload, self.id, self.token)
+        self.deferred = True
+        self.ephemeral = ephemeral
 
-    @property
-    def label(self) -> Optional[str]:
-        """
-        The label of the interacted button.
 
-        :rtype: Optional[str]
-        """
-        if self.data.component_type != ComponentType.BUTTON:
-            return
-        if self.message is None:
-            return
-        if self.message.components is None:
-            return
-        for action_row in self.message.components:
-            for component in action_row.components:
-                if component.custom_id == self.custom_id:
-                    return component.label
+class AutocompleteContext(BaseInteractionContext):
+    focussed_option: SlashCommandOption  # todo: option parsing
+    """The option the user is currently filling in."""
 
-    @property
-    def component(self) -> Optional[Union[Button, SelectMenu]]:
-        """
-        .. versionadded:: 4.4.0
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        return super().from_dict(client, payload)
 
-        The component that you interacted.
+    @property
+    def input_text(self) -> str:
+        """The text the user has already filled in."""
+        return self.kwargs.get(str(self.focussed_option.name), "")
+
+    def option_processing_hook(self, option: dict) -> None:
+        if option.get("focused", False):
+            self.focussed_option = SlashCommandOption.from_dict(option)
+        return
+
+    async def send(self, choices: typing.Iterable[str | int | float | dict[str, int | float | str]]) -> None:
+        """
+        Send your autocomplete choices to discord. Choices must be either a list of strings, or a dictionary following the following format:
+
+        ```json
+            {
+              "name": str,
+              "value": str
+            }
+        ```
+        Where name is the text visible in Discord, and value is the data sent back to your client when that choice is
+        chosen.
+
+        Args:
+            choices: 25 choices the user can pick
+        """
+        if self.focussed_option.type == OptionType.STRING:
+            type_cast = str
+        elif self.focussed_option.type == OptionType.INTEGER:
+            type_cast = int
+        elif self.focussed_option.type == OptionType.NUMBER:
+            type_cast = float
+        else:
+            type_cast = None
+
+        processed_choices = []
+        for choice in choices:
+            if isinstance(choice, dict):
+                name = choice["name"]
+                value = choice["value"]
+            else:
+                name = str(choice)
+                value = choice
 
-        :rtype: Optional[Union[Button, SelectMenu]]
-        """
-        if self.message is None or self.message.components is None:
-            return
+            processed_choices.append({"name": name, "value": type_cast(value) if type_cast else value})
 
-        for action_row in self.message.components:
-            for component in action_row.components:
-                if component.custom_id == self.custom_id:
-                    return component
+        payload = {"type": CallbackType.AUTOCOMPLETE_RESULT, "data": {"choices": processed_choices}}
+        await self.client.http.post_initial_response(payload, self.id, self.token)
```

