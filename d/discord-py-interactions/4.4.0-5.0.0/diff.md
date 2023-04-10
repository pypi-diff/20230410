# Comparing `tmp/discord-py-interactions-4.4.0.tar.gz` & `tmp/discord-py-interactions-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-4.4.0.tar", last modified: Sat Feb 11 17:43:55 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.0.0.tar", last modified: Mon Apr 10 11:44:03 2023, max compression
```

## Comparing `discord-py-interactions-4.4.0.tar` & `discord-py-interactions-5.0.0.tar`

### file list

```diff
@@ -1,96 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.776263 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-02-11 17:43:55.000000 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-02-11 17:43:55.000000 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 17:43:55.000000 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-11 17:43:55.000000 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-11 17:43:55.000000 discord-py-interactions-4.4.0/discord_py_interactions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.776263 discord-py-interactions-4.4.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.776263 discord-py-interactions-4.4.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.776263 discord-py-interactions-4.4.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45756 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/gateway/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/gateway/ratelimit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.780263 discord-py-interactions-4.4.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    29975 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/scheduledEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/http/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.780263 discord-py-interactions-4.4.0/interactions/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    78002 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)   125222 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/gw.py
--rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    48144 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/api/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.780263 discord-py-interactions-4.4.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    32748 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/decor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.780263 discord-py-interactions-4.4.0/interactions/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38947 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/client/models/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/ext/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/ext/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/ext/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/ext/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/interactions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/interactions/utils/abc/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/abc/base_context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/abc/base_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/attrs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/dict_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/get.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/interactions/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-11 17:43:55.784263 discord-py-interactions-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-11 17:43:45.000000 discord-py-interactions-4.4.0/setup.py
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

### Comparing `discord-py-interactions-4.4.0/LICENSE` & `discord-py-interactions-5.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `discord-py-interactions-4.4.0/interactions/client/bot.py` & `discord-py-interactions-5.0.0/interactions/client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,2142 +1,2235 @@
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
-
-log: logging.Logger = get_logger("client")
-
-__all__ = (
-    "Client",
-    "Extension",
-    "extension_listener",
-    "extension_command",
-    "extension_component",
-    "extension_modal",
-    "extension_autocomplete",
-    "extension_user_command",
-    "extension_message_command",
-)
-
-
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
-
-        Set to ``True`` to enable debug logging or set to a log level to use a specific level
-
-    :ivar Application me: The application representation of the client.
-    """
-
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
-        )
-
-        if _logging := kwargs.get("logging", _logging):
-            # thx i0 for posting this on the retux Discord
-
-            if _logging is True:
-                _logging = logging.DEBUG
-
-            _format = (
-                "%(asctime)s [%(levelname)s] - .%(funcName)s(): %(message)s"
-                if _logging == logging.DEBUG
-                else "%(asctime)s [%(levelname)s] - %(message)s"
-            )
-
-            logging.basicConfig(format=_format, level=_logging)
-
-        if disable_sync:
-            self._automate_sync = False
-            log.warning(
-                "Automatic synchronization has been disabled. Interactions may need to be manually synchronized."
-            )
-        else:
-            self._automate_sync = True
-
-    async def modify_nick_in_guild(
-        self, guild_id: Union[int, str, Snowflake, Guild], new_nick: Optional[str] = MISSING
-    ) -> Member:
-        """
-        .. versionadded:: 4.4.0
-
-        Sets a new nick in the specified guild.
-
-        :param Union[int, str, Snowflake, Guild] guild_id: The ID of the guild to modify the nick in
-        :param Optional[str] new_nick: The new nick to assign
-        """
-        if not self._http or isinstance(self._http, str):
-            raise LibraryException(
-                code=13, message="You cannot use this method until the bot has started!"
-            )
-
-        if new_nick is MISSING:
-            raise LibraryException(code=12, message="new nick name must either a string or `None`")
-
-        _id = int(guild_id.id) if isinstance(guild_id, Guild) else int(guild_id)
-
-        return Member(
-            **await self._http.modify_self_nick_in_guild(_id, new_nick), _client=self._http
-        )
-
-    @property
-    def guilds(self) -> List[Guild]:
-        """
-        .. versionadded:: 4.2.0
-
-        Returns a list of guilds the bot is in.
-        """
-
-        return list(self._http.cache[Guild].values.values())
-
-    @property
-    def latency(self) -> float:
-        """
-        .. versionadded:: 4.2.0
-
-        Returns the connection latency in milliseconds.
-        """
-
-        return self._websocket.latency * 1000
-
-    def start(self, token: Optional[str] = None) -> None:
-        """
-        Starts the client session.
-
-        :param Optional[str] token: The token of bot.
-        """
-
-        try:
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
-
-        option_attrs: List[str] = [name for name in Option.__slots__ if not name.startswith("_")]
-        choice_attrs: List[str] = [name for name in Choice.__slots__ if not name.startswith("_")]
-        log.info(f"Current attributes to compare: {', '.join(attrs)}.")
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
-
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
-
-        if isinstance(self._http, str):
-            self._http = HTTPClient(self._http, self._cache)
-
-        data = await self._http.get_current_bot_information()
-        self.me = Application(**data, _client=self._http)
-
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
-                    self._intents.GUILD_MESSAGES in self._intents
-                    and self.me.flags.GATEWAY_MESSAGE_CONTENT not in self.me.flags
-                    and self.me.flags.GATEWAY_MESSAGE_CONTENT_LIMITED not in self.me.flags
-                ):
-                    log.critical("Client not authorised for the MESSAGE_CONTENT intent.")
-            elif self._intents.value != Intents.DEFAULT.value:
-                raise RuntimeError("Client not authorised for any privileged intents.")
-
-            self.__resolve_commands()
-
-            if self._automate_sync:
-                await self.__sync()
-            else:
-                await self.__get_all_commands()
-            await self.__register_id_autocomplete()
-
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
-
-        if isinstance(self._http, HTTPClient):
-            await self._http._req._session.close()  # Closes the HTTP session associated with the client.
-
-    async def _login(self) -> None:
-        """Makes a login with the Discord API."""
-
-        try:
-            await self._websocket.run()
-        except Exception:
-            log.exception("Websocket have raised an exception, closing.")
-
-            if self._websocket._closing_lock.is_set():
-                # signal for closing.
-
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
-
-    async def wait_until_ready(self) -> None:
-        """
-        .. versionadded:: 4.2.0
-
-        Helper method that waits until the websocket is ready.
-        """
-        await self._websocket.wait_until_ready()
-
-    async def _get_all_guilds(self) -> List[dict]:
-        """
-        Gets all guilds that the bot is present in.
-
-        :return: List of guilds
-        :rtype: List[dict]
-        """
-
-        _after = None
-        _all: list = []
-
-        res = await self._http.get_self_guilds(limit=200)
-
-        while len(res) >= 200:
-            _all.extend(res)
-            _after = int(res[-1]["id"])
-
-            res = await self._http.get_self_guilds(
-                after=_after,
-            )
-
-        _all.extend(res)
-
-        return _all
-
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
-        )
-
-        for command in _cmds:
-            if command.get("code"):
-                # Error exists.
-                raise LibraryException(command["code"], message=f'{command["message"]} |')
-
-        self.__global_commands = {"commands": _cmds, "clean": True}
-        # TODO: add to cache (later)
-
-        # responsible for checking if a command is in the cache but not a coro -> allowing removal
-
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
-
-            for command in _cmds:
-                if command.get("code"):
-                    # Error exists.
-                    raise LibraryException(command["code"], message=f'{command["message"]} |')
-
-            self.__guild_commands[_id] = {"commands": _cmds, "clean": True}
-
-    def __resolve_commands(self) -> None:  # sourcery skip: low-code-quality
-        """
-        Resolves all commands to the command coroutines.
-
-        .. warning::
-            This is an internal method. Do not call it unless you know what you are doing!
-        """
-        for cmd in self._commands:
-            if cmd.coro.__qualname__ in [_cmd.__qualname__ for _cmd in self.__command_coroutines]:
-                continue
-
-            cmd.listener = self._websocket._dispatch
-
-            if cmd.default_scope and self._default_scope:
-                if isinstance(cmd.scope, list):
-                    cmd.scope.extend(self._default_scope)
-                else:
-                    cmd.scope = self._default_scope
-
-            data: Union[dict, List[dict]] = cmd.full_data
-            coro = cmd.dispatcher
-
-            self.__check_command(
-                command=ApplicationCommand(**(data[0] if isinstance(data, list) else data)),
-                coro=coro,
-            )
-
-            if cmd.autocompletions:
-                self.__id_autocomplete.update(cmd.autocompletions)
-
-            coro = coro.__func__ if hasattr(coro, "__func__") else coro
-
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
-
-            if cmd.scope not in (MISSING, None):
-                if isinstance(cmd.scope, List):
-                    [self._scopes.add(_ if isinstance(_, int) else _.id) for _ in cmd.scope]
-                else:
-                    self._scopes.add(cmd.scope if isinstance(cmd.scope, int) else cmd.scope.id)
-
-            self.event(coro, name=f"command_{cmd.name}")
-
-    async def __sync(self) -> None:  # sourcery no-metrics
-        """
-        Synchronizes all commands to the API.
-
-        .. warning::
-            This is an internal method. Do not call it unless you know what you are doing!
-        """
-        # sourcery skip: low-code-quality
-
-        log.debug("starting command sync")
-        _guilds = await self._get_all_guilds()
-        _guild_ids = [int(_["id"]) for _ in _guilds]
-        self._scopes.update(_guild_ids)
-        _cmds = await self._http.get_application_commands(
-            application_id=self.me.id, with_localizations=True
-        )
-
-        for command in _cmds:
-            if command.get("code"):
-                # Error exists.
-                raise LibraryException(command["code"], message=f'{command["message"]} |')
-
-        self.__global_commands = {"commands": _cmds, "clean": True}
-        # TODO: add to cache (later)
-
-        __check_global_commands: List[str] = [cmd["name"] for cmd in _cmds]
-        __check_guild_commands: Dict[int, List[str]] = {}
-        __blocked_guilds: set = set()
-
-        # responsible for checking if a command is in the cache but not a coro -> allowing removal
-
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
-
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
-
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
-
-        if coro is not MISSING:
-            self._websocket._dispatch.register(
-                coro, name=name if name is not MISSING else coro.__name__
-            )
-            return coro
-
-        return decorator
-
-    async def change_presence(self, presence: ClientPresence) -> None:
-        """
-        .. versionadded:: 4.2.0
-
-        A method that changes the current client's presence on runtime.
-
-        .. note::
-            There is a ratelimit to using this method (5 per minute).
-            As there's no gateway ratelimiter yet, breaking this ratelimit
-            will force your bot to disconnect.
-
-        :param ClientPresence presence: The presence to change the bot to on identify.
-        """
-        await self._websocket._update_presence(presence)
-
-    def __check_command(
-        self,
-        command: ApplicationCommand,
-        coro: Callable[..., Coroutine],
-        regex: str = r"^[a-z0-9_-]{1,32}$",
-    ) -> None:  # sourcery no-metrics
-        """
-        Checks if a command is valid.
-        """
-        reg = re.compile(regex)
-        _options_names: List[str] = []
-        _sub_groups_present: bool = False
-        _sub_cmds_present: bool = False
-
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
-
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
-
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
-
-            if len(coro.__code__.co_varnames) - add < len(set(_options_names)):
-                log.debug(
-                    "Coroutine is missing arguments for options:"
-                    f" {[_arg for _arg in _options_names if _arg not in coro.__code__.co_varnames]}"
-                )
-                raise LibraryException(
-                    11, message="You need one argument for every option name in your command!"
-                )
-
-        if command.name is MISSING:
-            raise LibraryException(11, message="Your command must have a name.")
-
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
-
-            _opt_names = []
-            for _option in command.options:
-                if _option.type == OptionType.SUB_COMMAND_GROUP:
-                    __check_sub_group(_option)
-
-                elif _option.type == OptionType.SUB_COMMAND:
-                    __check_sub_command(_option)
-
-                else:
-                    __check_options(_option, _opt_names)
-            del _opt_names
-
-        __check_coro()
-
-    def command(
-        self,
-        *,
-        type: Optional[Union[int, ApplicationCommandType]] = ApplicationCommandType.CHAT_INPUT,
-        name: Optional[str] = MISSING,
-        description: Optional[str] = MISSING,
-        scope: Optional[Union[int, Guild, List[int], List[Guild]]] = MISSING,
-        options: Optional[
-            Union[Dict[str, Any], List[Dict[str, Any]], Option, List[Option]]
-        ] = MISSING,
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
-
-        return decorator
-
-    def message_command(
-        self,
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
-
-        return decorator
-
-    def user_command(
-        self,
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
-
-        return decorator
-
-    def _find_command(self, command: Union[str, int]) -> ApplicationCommand:
-        """
-        Iterates over `commands` and returns an :class:`ApplicationCommand` if it matches the name from `command`
-
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
-        )
-
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
-
-        if not _command_obj or (hasattr(_command_obj, "id") and not _command_obj.id):
-            raise LibraryException(
-                6,
-                message="The command does not exist. Make sure to define"
-                + " your autocomplete callback after your commands",
-            )
-        else:
-            return _command_obj
-
-    def autocomplete(
-        self, command: Union[ApplicationCommand, int, str, Snowflake], name: str
-    ) -> Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]:
-        """
-        .. versionadded:: 4.0.2
-
-        A decorator for listening to ``INTERACTION_CREATE`` dispatched gateway
-        events involving autocompletion fields.
-
-        The structure for an autocomplete callback:
-
-        .. code-block:: python
-
-            @bot.autocomplete(command="command_name", name="option_name")
-            async def autocomplete_choice_list(ctx, user_input: str = ""):
-                await ctx.populate([
-                    interactions.Choice(...),
-                    interactions.Choice(...),
-                    ...
-                ])
-
-        :param Union[ApplicationCommand, int, str, Snowflake] command: The command, command ID, or command name with the option.
-        :param str name: The name of the option to autocomplete.
-        :return: A callable response.
-        :rtype: Callable[[Callable[..., Coroutine]], Callable[..., Coroutine]]
-        """
-
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
-
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
-
-    def remove(
-        self, name: str, remove_commands: bool = True, package: Optional[str] = None
-    ) -> None:
-        """
-        .. versionadded:: 4.1.0
-
-        Removes an extension out of the current client from an import resolve.
-
-        :param str name: The name of the extension.
-        :param Optional[bool] remove_commands: Whether to remove commands before reloading. Defaults to ``True``.
-        :param Optional[str] package: The package of the extension.
-        """
-        try:
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
-
-        else:
-            with contextlib.suppress(AttributeError):
-                self._loop.create_task(
-                    extension.teardown(remove_commands=remove_commands)
-                )  # made for Extension, usable by others
-        del self._extensions[_name]
-
-        log.debug(f"Removed extension {name}.")
-
-    def reload(
-        self,
-        name: str,
-        package: Optional[str] = None,
-        remove_commands: bool = True,
-        *args,
-        **kwargs,
-    ) -> Optional["Extension"]:
-        r"""
-        .. versionadded:: 4.1.0
-
-        "Reloads" an extension off of current client from an import resolve.
-
-        .. warning::
-            This will remove and re-add application commands, counting towards your daily application
-            command creation limit, as long as you have the ``remove_commands`` argument set to ``True``, which it is by
-            default.
-
-        :param str name: The name of the extension
-        :param Optional[str] package: The package of the extension
-        :param Optional[bool] remove_commands: Whether to remove commands before reloading. Defaults to True
-        :param tuple \*args: Optional arguments to pass to the extension
-        :param dict \**kwargs: Optional keyword-only arguments to pass to the extension.
-        :return: The reloaded extension.
-        :rtype: Optional[Extension]
-        """
-        _name: str = resolve_name(name, package)
-        extension = self._extensions.get(_name)
-
-        if extension is None:
-            log.warning(f"Extension {name} could not be reloaded because it was never loaded.")
-            return self.load(name, package)
-
-        self.remove(name, package=package, remove_commands=remove_commands)
-        return self.load(name, package, *args, **kwargs)
-
-    def get_extension(self, name: str) -> Optional[Union[ModuleType, "Extension"]]:
-        """
-        .. versionadded:: 4.2.0
-
-        Get an extension based on its name.
-
-        :param str name: Name of the extension.
-        :return: The found extension.
-        :rtype: Optional[Union[ModuleType, Extension]]
-        """
-        return self._extensions.get(name)
-
-    async def modify(
-        self,
-        username: Optional[str] = MISSING,
-        avatar: Optional[Image] = MISSING,
-    ) -> User:
-        """
-        .. versionadded:: 4.2.0
-
-        Modify the bot user account settings.
-
-        :param Optional[str] username: The new username of the bot
-        :param Optional[Image] avatar: The new avatar of the bot
-        :return: The modified User object
-        :rtype: User
-        """
-        if not self._http or isinstance(self._http, str):
-            raise LibraryException(
-                code=13, message="You cannot use this method until the bot has started!"
-            )
-
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
-        """
-        .. versionadded:: 4.3.2
-
-        Requests guild members via websocket.
-
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
-
-    async def _logout(self) -> None:
-        await self._websocket.close()
-        if isinstance(self._http, HTTPClient):
-            await self._http._req.close()
-
-    async def wait_for(
-        self,
-        name: str,
-        check: Optional[Callable[..., Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> Any:
-        """
-        .. versionadded:: 4.4.0
-
-        Waits for an event once, and returns the result.
-
-        Unlike event decorators, this is not persistent, and can be used to only proceed in a command once an event happens.
-
-        :param str name: The event to wait for
-        :param Optional[Callable[..., Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param float timeout: How long to wait for the event before raising an error
-        :return: The value of the dispatched event
-        :rtype: Any
-        """
-        while True:
-            fut = self._websocket._dispatch.add(name=name)
-            try:
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
-
-        if res:
-            return res[0] if len(res) == 1 else res
-
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
-            if _ctx.data.component_type.value not in {4, 5, 6, 7, 8}:
-                return False
-            return check(_ctx) if check else True
-
-        ctx: ComponentContext = await self.wait_for_component(
-            components, messages, check=_check, timeout=timeout
-        )
-
-        if ctx.data.component_type == 4:
-            return ctx, ctx.data.values
-
-        _list = []  # temp storage for items
-        _data = self._websocket._WebSocketClient__select_option_type_context(
-            ctx, ctx.data.component_type.value
-        )  # resolved.
-        for value in ctx.data.values:
-            _list.append(_data[value])
-        return ctx, _list
-
-    async def wait_for_modal(
-        self,
-        modals: Union[Modal, str, List[Union[Modal, str]]],
-        check: Optional[Callable[[CommandContext], Union[bool, Awaitable[bool]]]] = None,
-        timeout: Optional[float] = None,
-    ) -> Tuple[CommandContext, List[str]]:
-        """
-        .. versionadded:: 4.4.0
-
-        Waits for a modal to be interacted with, and returns the resulting context and submitted data.
-
-        .. note::
-            This function returns both the context of the modal and the data the user input.
-            The recommended way to use it is to do:
-            ``modal_ctx, fields = await bot.wait_for_modal(...)``
-
-            Alternatively, to get the fields immediately, you can do:
-            ``modal_ctx, (field1, field2, ...) = await bot.wait_for_modal(...)``
-
-        :param Union[Modal, str, List[Modal, str]] modals: The modal(s) to wait for
-        :param Optional[Callable[[CommandContext], Union[bool, Awaitable[bool]]]] check: A function or coroutine to call, which should return a truthy value if the data should be returned
-        :param Optional[float] timeout: How long to wait for the event before raising an error
-        :return: The context of the modal, followed by the data the user inputted
-        :rtype: tuple[CommandContext, list[str]]
-        """
-        ids: List[str] = []
-
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
-
-        if not all(isinstance(id, str) for id in ids):
-            raise TypeError("No modals were passed!")
-
-        def _check(ctx: CommandContext):
-            if ids and ctx.data.custom_id not in ids:
-                return False
-            return check(ctx) if check else True
-
-        ctx: CommandContext = await self.wait_for("on_modal", check=_check, timeout=timeout)
-
-        # Ed requested that it returns a result similar to the decorator
-        fields: List[str] = []
-        for actionrow in ctx.data.components:  # discord is weird with this
-            if actionrow.components:
-                data = actionrow.components[0].value
-                fields.append(data)
-
-        return ctx, fields
-
-    async def get_self_user(self) -> User:
-        """
-        .. versionadded:: 4.4.0
-
-        Gets the bot's user information.
-        """
-        return User(**await self._http.get_self(), _client=self._http)
-
-    async def get_role_connection_metadata(self) -> List[ApplicationRoleConnectionMetadata]:
-        """
-        .. versionadded:: 4.4.0
-
-        Gets the bot's role connection metadata.
-
-        :return: The list of bot's role connection metadata.
-        """
-
-        res: List[dict] = await self._http.get_application_role_connection_metadata(
-            application_id=int(self.me.id)
-        )
-        return [ApplicationRoleConnectionMetadata(**metadata) for metadata in res]
-
-    async def update_role_connection_metadata(
-        self,
-        metadata: Union[List[ApplicationRoleConnectionMetadata], ApplicationRoleConnectionMetadata],
-    ) -> List[ApplicationRoleConnectionMetadata]:
-        """
-        .. versionadded:: 4.4.0
-
-        Updates the bot's role connection metadata.
-
-        .. note::
-            This method overwrites all current bot's role connection metadata.
-
-        :param List[ApplicationRoleConnectionMetadata] metadata: The list of role connection metadata. The maximum is five.
-        :return: The updated list of bot's role connection metadata.
-        """
-        if not isinstance(metadata, list):
-            metadata = [metadata]
-
-        res: List[dict] = await self._http.update_application_role_connection_metadata(
-            application_id=int(self.me.id), payload=[_._json for _ in metadata]
-        )
-        return [ApplicationRoleConnectionMetadata(**_) for _ in res]
-
-
-class Extension:
-    """
-    .. versionadded:: 4.1.0
-
-    A class that allows you to represent "extensions" of your code, or
-    essentially cogs that can be ran independent of the root file in
-    an object-oriented structure.
-
-    The structure of an extension:
-
-    .. code-block:: python
-
-        class CoolCode(interactions.Extension):
-            def __init__(self, client):
-                self.client = client
-
-            @extension_user_command(
-                name="User command in cog",
-            )
-            async def cog_user_cmd(self, ctx):
-                ...
-
-        def setup(client):
-            CoolCode(client)
-    """
-
-    client: Client
-
-    def __new__(cls, client: Client, *args, **kwargs) -> "Extension":
-        # sourcery skip: low-code-quality
-
-        self = super().__new__(cls)
-
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
-
-        client._extensions[cls.__name__] = self
-
-        self.client._Client__resolve_commands()  # noqa
-
-        if client._websocket.ready.is_set() and client._automate_sync:
-            client._loop.create_task(client._Client__sync())  # noqa
-
-        return self
-
-    async def teardown(self, remove_commands: bool = True):
-        for event, funcs in self._listeners.items():
-            for func in funcs:
-                self.client._websocket._dispatch.events[event].remove(func)
-
-        for cmd, funcs in self._commands.items():
-            _cmd: str = cmd.split("_", 1)[1]
-
-            for _coro in self.client._Client__command_coroutines:
-                if _coro._name == _cmd:
-                    self.client._Client__command_coroutines.remove(_coro)  # noqa
-                    break
-
-            for _command in self.client._commands:
-                if _command.name == _cmd:
-                    self.client._commands.remove(_command)
-                    break
-
-            for i in range(len(funcs)):
-                self.client._websocket._dispatch.events[cmd].pop(i)  # noqa
-
-        if self.client._automate_sync and remove_commands:
-            await self.client._Client__sync()  # noqa
-
-
-@wraps(Client.command)
-def extension_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(coro) -> Command:
-        cmd = Command(coro=coro, **kwargs)
-        coro.__command_data__ = cmd
-        return cmd
-
-    return decorator
-
-
-@wraps(Client.event)
-def extension_listener(func: Optional[Coroutine] = None, name: Optional[str] = None):
-    def decorator(func: Coroutine):
-        if not hasattr(func, "__listener_name__"):
-            func.__listener_name__ = []
-        func.__listener_name__.append(name or func.__name__)
-
-        return func
-
-    if func:
-        # allows omitting `()` on `@listener`
-        return decorator(func)
-
-    return decorator
-
-
-@wraps(Client.component)
-def extension_component(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__component_data__"):
-            func.__component_data__ = []
-        func.__component_data__.append((args, kwargs))
-
-        return func
-
-    return decorator
-
-
-@wraps(Client.autocomplete)
-def extension_autocomplete(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__autocomplete_data__"):
-            func.__autocomplete_data__ = []
-        func.__autocomplete_data__.append((args, kwargs))
-
-        return func
-
-    return decorator
-
-
-@wraps(Client.modal)
-def extension_modal(*args, **kwargs):
-    def decorator(func):
-        if not hasattr(func, "__modal_data__"):
-            func.__modal_data__ = []
-        func.__modal_data__.append((args, kwargs))
-
-        return func
-
-    return decorator
-
-
-@wraps(Client.message_command)
-def extension_message_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(func) -> Command:
-        kwargs["type"] = ApplicationCommandType.MESSAGE
-        return extension_command(**kwargs)(func)
-
-    return decorator
-
-
-@wraps(Client.user_command)
-def extension_user_command(**kwargs) -> Callable[[Callable[..., Coroutine]], Command]:
-    def decorator(func) -> Command:
-        kwargs["type"] = ApplicationCommandType.USER
-        return extension_command(**kwargs)(func)
-
-    return decorator
+import asyncio
+import contextlib
+import functools
+import importlib.util
+import inspect
+import logging
+import re
+import sys
+import time
+import traceback
+from collections.abc import Iterable
+from datetime import datetime
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    Dict,
+    List,
+    NoReturn,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+    Awaitable,
+)
+
+import interactions.api.events as events
+import interactions.client.const as constants
+from interactions.models.internal.callback import CallbackObject
+from interactions.api.events import BaseEvent, RawGatewayEvent, processors
+from interactions.api.events.internal import CallbackAdded
+from interactions.api.gateway.gateway import GatewayClient
+from interactions.api.gateway.state import ConnectionState
+from interactions.api.http.http_client import HTTPClient
+from interactions.client import errors
+from interactions.client.const import (
+    GLOBAL_SCOPE,
+    MISSING,
+    Absent,
+    EMBED_MAX_DESC_LENGTH,
+    get_logger,
+    AsyncCallable,
+)
+from interactions.client.errors import (
+    BotException,
+    ExtensionLoadException,
+    ExtensionNotFound,
+    Forbidden,
+    InteractionMissingAccess,
+    HTTPException,
+    NotFound,
+)
+from interactions.client.smart_cache import GlobalCache
+from interactions.client.utils import NullCache, FastJson
+from interactions.client.utils.misc_utils import get_event_name, wrap_partial
+from interactions.client.utils.serializer import to_image_data
+from interactions.models import (
+    Activity,
+    Application,
+    CustomEmoji,
+    Guild,
+    GuildTemplate,
+    Message,
+    Extension,
+    ClientUser,
+    User,
+    Member,
+    Modal,
+    StickerPack,
+    Sticker,
+    ScheduledEvent,
+    InteractionCommand,
+    SlashCommand,
+    OptionType,
+    to_snowflake,
+    ComponentCommand,
+    application_commands_to_dict,
+    sync_needed,
+    VoiceRegion,
+)
+from interactions.models import Wait
+from interactions.models.discord.color import BrandColors
+from interactions.models.discord.components import get_components_ids, BaseComponent
+from interactions.models.discord.embed import Embed
+from interactions.models.discord.enums import (
+    ComponentType,
+    Intents,
+    InteractionType,
+    Status,
+)
+from interactions.models.discord.file import UPLOADABLE_TYPE
+from interactions.models.discord.snowflake import Snowflake, to_snowflake_list
+from interactions.models.internal.active_voice_state import ActiveVoiceState
+from interactions.models.internal.application_commands import ContextMenu, ModalCommand, GlobalAutoComplete
+from interactions.models.internal.auto_defer import AutoDefer
+from interactions.models.internal.command import BaseCommand
+from interactions.models.internal.context import (
+    BaseContext,
+    InteractionContext,
+    SlashContext,
+    ModalContext,
+    ComponentContext,
+    AutocompleteContext,
+    ContextMenuContext,
+)
+from interactions.models.internal.listener import Listener
+from interactions.models.internal.tasks import Task
+
+if TYPE_CHECKING:
+    from interactions.models import Snowflake_Type, TYPE_ALL_CHANNEL
+
+
+__all__ = ("Client",)
+
+
+# see https://discord.com/developers/docs/topics/gateway#list-of-intents
+_INTENT_EVENTS: dict[BaseEvent, list[Intents]] = {
+    # Intents.GUILDS
+    events.GuildJoin: [Intents.GUILDS],
+    events.GuildLeft: [Intents.GUILDS],
+    events.GuildUpdate: [Intents.GUILDS],
+    events.RoleCreate: [Intents.GUILDS],
+    events.RoleDelete: [Intents.GUILDS],
+    events.RoleUpdate: [Intents.GUILDS],
+    events.ChannelCreate: [Intents.GUILDS],
+    events.ChannelDelete: [Intents.GUILDS],
+    events.ChannelUpdate: [Intents.GUILDS],
+    events.ThreadCreate: [Intents.GUILDS],
+    events.ThreadDelete: [Intents.GUILDS],
+    events.ThreadListSync: [Intents.GUILDS],
+    events.ThreadMemberUpdate: [Intents.GUILDS],
+    events.ThreadUpdate: [Intents.GUILDS],
+    events.StageInstanceCreate: [Intents.GUILDS],
+    events.StageInstanceDelete: [Intents.GUILDS],
+    events.StageInstanceUpdate: [Intents.GUILDS],
+    # Intents.GUILD_MEMBERS
+    events.MemberAdd: [Intents.GUILD_MEMBERS],
+    events.MemberRemove: [Intents.GUILD_MEMBERS],
+    events.MemberUpdate: [Intents.GUILD_MEMBERS],
+    # Intents.GUILD_MODERATION
+    events.BanCreate: [Intents.GUILD_MODERATION],
+    events.BanRemove: [Intents.GUILD_MODERATION],
+    events.GuildAuditLogEntryCreate: [Intents.GUILD_MODERATION],
+    # Intents.GUILD_EMOJIS_AND_STICKERS
+    events.GuildEmojisUpdate: [Intents.GUILD_EMOJIS_AND_STICKERS],
+    events.GuildStickersUpdate: [Intents.GUILD_EMOJIS_AND_STICKERS],
+    # Intents.GUILD_INTEGRATIONS
+    events.IntegrationCreate: [Intents.GUILD_INTEGRATIONS],
+    events.IntegrationDelete: [Intents.GUILD_INTEGRATIONS],
+    events.IntegrationUpdate: [Intents.GUILD_INTEGRATIONS],
+    # Intents.GUILD_WEBHOOKS
+    events.WebhooksUpdate: [Intents.GUILD_WEBHOOKS],
+    # Intents.GUILD_INVITES
+    events.InviteCreate: [Intents.GUILD_INVITES],
+    events.InviteDelete: [Intents.GUILD_INVITES],
+    # Intents.GUILD_VOICE_STATES
+    events.VoiceStateUpdate: [Intents.GUILD_VOICE_STATES],
+    # Intents.GUILD_PRESENCES
+    events.PresenceUpdate: [Intents.GUILD_PRESENCES],
+    # Intents.GUILD_MESSAGES
+    events.MessageDeleteBulk: [Intents.GUILD_MESSAGES],
+    # Intents.AUTO_MODERATION_CONFIGURATION
+    events.AutoModExec: [Intents.AUTO_MODERATION_EXECUTION, Intents.AUTO_MOD],
+    # Intents.AUTO_MODERATION_CONFIGURATION
+    events.AutoModCreated: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
+    events.AutoModUpdated: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
+    events.AutoModDeleted: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
+    # multiple intents
+    events.ThreadMembersUpdate: [Intents.GUILDS, Intents.GUILD_MEMBERS],
+    events.TypingStart: [
+        Intents.GUILD_MESSAGE_TYPING,
+        Intents.DIRECT_MESSAGE_TYPING,
+        Intents.TYPING,
+    ],
+    events.MessageUpdate: [Intents.GUILD_MESSAGES, Intents.DIRECT_MESSAGES, Intents.MESSAGES],
+    events.MessageCreate: [Intents.GUILD_MESSAGES, Intents.DIRECT_MESSAGES, Intents.MESSAGES],
+    events.MessageDelete: [Intents.GUILD_MESSAGES, Intents.DIRECT_MESSAGES, Intents.MESSAGES],
+    events.ChannelPinsUpdate: [Intents.GUILDS, Intents.DIRECT_MESSAGES],
+    events.MessageReactionAdd: [
+        Intents.GUILD_MESSAGE_REACTIONS,
+        Intents.DIRECT_MESSAGE_REACTIONS,
+        Intents.REACTIONS,
+    ],
+    events.MessageReactionRemove: [
+        Intents.GUILD_MESSAGE_REACTIONS,
+        Intents.DIRECT_MESSAGE_REACTIONS,
+        Intents.REACTIONS,
+    ],
+    events.MessageReactionRemoveAll: [
+        Intents.GUILD_MESSAGE_REACTIONS,
+        Intents.DIRECT_MESSAGE_REACTIONS,
+        Intents.REACTIONS,
+    ],
+}
+
+
+class Client(
+    processors.AutoModEvents,
+    processors.ChannelEvents,
+    processors.GuildEvents,
+    processors.IntegrationEvents,
+    processors.MemberEvents,
+    processors.MessageEvents,
+    processors.ReactionEvents,
+    processors.RoleEvents,
+    processors.StageEvents,
+    processors.ThreadEvents,
+    processors.UserEvents,
+    processors.VoiceEvents,
+):
+    """
+
+    The bot client.
+
+    Args:
+        intents: The intents to use
+
+        status: The status the bot should log in with (IE ONLINE, DND, IDLE)
+        activity: The activity the bot should log in "playing"
+
+        sync_interactions: Should application commands be synced with discord?
+        delete_unused_application_cmds: Delete any commands from discord that aren't implemented in this client
+        enforce_interaction_perms: Enforce discord application command permissions, locally
+        fetch_members: Should the client fetch members from guilds upon startup (this will delay the client being ready)
+        send_command_tracebacks: Automatically send uncaught tracebacks if a command throws an exception
+
+        auto_defer: AutoDefer: A system to automatically defer commands after a set duration
+        interaction_context: Type[InteractionContext]: InteractionContext: The object to instantiate for Interaction Context
+        component_context: Type[ComponentContext]: The object to instantiate for Component Context
+        autocomplete_context: Type[AutocompleteContext]: The object to instantiate for Autocomplete Context
+        modal_context: Type[ModalContext]: The object to instantiate for Modal Context
+
+        total_shards: The total number of shards in use
+        shard_id: The zero based int ID of this shard
+
+        debug_scope: Force all application commands to be registered within this scope
+        disable_dm_commands: Should interaction commands be disabled in DMs?
+        basic_logging: Utilise basic logging to output library data to console. Do not use in combination with `Client.logger`
+        logging_level: The level of logging to use for basic_logging. Do not use in combination with `Client.logger`
+        logger: The logger interactions.py should use. Do not use in combination with `Client.basic_logging` and `Client.logging_level`. Note: Different loggers with multiple clients are not supported
+
+    Optionally, you can configure the caches here, by specifying the name of the cache, followed by a dict-style object to use.
+    It is recommended to use `smart_cache.create_cache` to configure the cache here.
+    as an example, this is a recommended attribute `message_cache=create_cache(250, 50)`,
+
+    ???+ note "Intents Note"
+        By default, all non-privileged intents will be enabled
+
+    ???+ note "Caching Note"
+        Setting a message cache hard limit to None is not recommended, as it could result in extremely high memory usage, we suggest a sane limit.
+
+
+    """
+
+    def __init__(
+        self,
+        *,
+        activity: Union[Activity, str] = None,
+        auto_defer: Absent[Union[AutoDefer, bool]] = MISSING,
+        autocomplete_context: Type[BaseContext] = AutocompleteContext,
+        basic_logging: bool = False,
+        component_context: Type[BaseContext] = ComponentContext,
+        context_menu_context: Type[BaseContext] = ContextMenuContext,
+        debug_scope: Absent["Snowflake_Type"] = MISSING,
+        delete_unused_application_cmds: bool = False,
+        disable_dm_commands: bool = False,
+        enforce_interaction_perms: bool = True,
+        fetch_members: bool = False,
+        global_post_run_callback: Absent[Callable[..., Coroutine]] = MISSING,
+        global_pre_run_callback: Absent[Callable[..., Coroutine]] = MISSING,
+        intents: Union[int, Intents] = Intents.DEFAULT,
+        interaction_context: Type[InteractionContext] = InteractionContext,
+        logger: logging.Logger = MISSING,
+        logging_level: int = logging.INFO,
+        modal_context: Type[BaseContext] = ModalContext,
+        owner_ids: Iterable["Snowflake_Type"] = (),
+        send_command_tracebacks: bool = True,
+        shard_id: int = 0,
+        show_ratelimit_tracebacks: bool = False,
+        slash_context: Type[BaseContext] = SlashContext,
+        status: Status = Status.ONLINE,
+        sync_ext: bool = True,
+        sync_interactions: bool = True,
+        token: str | None = None,
+        total_shards: int = 1,
+        **kwargs,
+    ) -> None:
+        if logger is MISSING:
+            logger = constants.get_logger()
+
+        if basic_logging:
+            logging.basicConfig()
+            logger.setLevel(logging_level)
+
+        # Set Up logger and overwrite the constant
+        self.logger = logger
+        """The logger interactions.py should use. Do not use in combination with `Client.basic_logging` and `Client.logging_level`.
+        !!! note
+            Different loggers with multiple clients are not supported"""
+        constants._logger = logger
+
+        # Configuration
+        self.sync_interactions: bool = sync_interactions
+        """Should application commands be synced"""
+        self.del_unused_app_cmd: bool = delete_unused_application_cmds
+        """Should unused application commands be deleted?"""
+        self.sync_ext: bool = sync_ext
+        """Should we sync whenever a extension is (un)loaded"""
+        self.debug_scope = to_snowflake(debug_scope) if debug_scope is not MISSING else MISSING
+        """Sync global commands as guild for quicker command updates during debug"""
+        self.send_command_tracebacks: bool = send_command_tracebacks
+        """Should the traceback of command errors be sent in reply to the command invocation"""
+        if auto_defer is True:
+            auto_defer = AutoDefer(enabled=True)
+        else:
+            auto_defer = auto_defer or AutoDefer()
+        self.auto_defer = auto_defer
+        """A system to automatically defer commands after a set duration"""
+        self.intents = intents if isinstance(intents, Intents) else Intents(intents)
+
+        # resources
+
+        self.http: HTTPClient = HTTPClient(logger=self.logger, show_ratelimit_tracebacks=show_ratelimit_tracebacks)
+        """The HTTP client to use when interacting with discord endpoints"""
+
+        # context factories
+        self.interaction_context: Type[BaseContext] = interaction_context
+        """The object to instantiate for Interaction Context"""
+        self.component_context: Type[BaseContext] = component_context
+        """The object to instantiate for Component Context"""
+        self.autocomplete_context: Type[BaseContext] = autocomplete_context
+        """The object to instantiate for Autocomplete Context"""
+        self.modal_context: Type[BaseContext] = modal_context
+        """The object to instantiate for Modal Context"""
+        self.slash_context: Type[BaseContext] = slash_context
+        """The object to instantiate for Slash Context"""
+        self.context_menu_context: Type[BaseContext] = context_menu_context
+        """The object to instantiate for Context Menu Context"""
+
+        self.token: str | None = token
+
+        # flags
+        self._ready = asyncio.Event()
+        self._closed = False
+        self._startup = False
+        self.disable_dm_commands = disable_dm_commands
+
+        self._guild_event = asyncio.Event()
+        self.guild_event_timeout = 3
+        """How long to wait for guilds to be cached"""
+
+        # Sharding
+        self.total_shards = total_shards
+        self._connection_state: ConnectionState = ConnectionState(self, intents, shard_id=shard_id)
+
+        self.enforce_interaction_perms = enforce_interaction_perms
+
+        self.fetch_members = fetch_members
+        """Fetch the full members list of all guilds on startup"""
+
+        self._mention_reg = MISSING
+
+        # caches
+        self.cache: GlobalCache = GlobalCache(self, **{k: v for k, v in kwargs.items() if hasattr(GlobalCache, k)})
+        # these store the last sent presence data for change_presence
+        self._status: Status = status
+        if isinstance(activity, str):
+            self._activity = Activity.create(name=str(activity))
+        else:
+            self._activity: Activity = activity
+
+        self._user: Absent[ClientUser] = MISSING
+        self._app: Absent[Application] = MISSING
+
+        # collections
+        self.interactions_by_scope: Dict["Snowflake_Type", Dict[str, InteractionCommand]] = {}
+        """A dictionary of registered application commands: `{scope: [commands]}`"""
+        self._interaction_lookup: dict[str, InteractionCommand] = {}
+        """A dictionary of registered application commands: `{name: command}`"""
+        self.interaction_tree: Dict[
+            "Snowflake_Type", Dict[str, InteractionCommand | Dict[str, InteractionCommand]]
+        ] = {}
+        """A dictionary of registered application commands in a tree"""
+        self._component_callbacks: Dict[str, Callable[..., Coroutine]] = {}
+        self._modal_callbacks: Dict[str, Callable[..., Coroutine]] = {}
+        self._global_autocompletes: Dict[str, GlobalAutoComplete] = {}
+        self.processors: Dict[str, Callable[..., Coroutine]] = {}
+        self.__modules = {}
+        self.ext: Dict[str, Extension] = {}
+        """A dictionary of mounted ext"""
+        self.listeners: Dict[str, list[Listener]] = {}
+        self.waits: Dict[str, List] = {}
+        self.owner_ids: set[Snowflake_Type] = set(owner_ids)
+
+        self.async_startup_tasks: list[tuple[Callable[..., Coroutine], Iterable[Any], dict[str, Any]]] = []
+        """A list of coroutines to run during startup"""
+
+        # callbacks
+        if global_pre_run_callback:
+            if asyncio.iscoroutinefunction(global_pre_run_callback):
+                self.pre_run_callback: Callable[..., Coroutine] = global_pre_run_callback
+            else:
+                raise TypeError("Callback must be a coroutine")
+        else:
+            self.pre_run_callback = MISSING
+
+        if global_post_run_callback:
+            if asyncio.iscoroutinefunction(global_post_run_callback):
+                self.post_run_callback: Callable[..., Coroutine] = global_post_run_callback
+            else:
+                raise TypeError("Callback must be a coroutine")
+        else:
+            self.post_run_callback = MISSING
+
+        super().__init__()
+        self._sanity_check()
+
+    async def __aenter__(self) -> "Client":
+        if not self.token:
+            raise ValueError(
+                "Token not found - to use the bot in a context manager, you must pass the token in the Client constructor."
+            )
+        await self.login(self.token)
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+        if not self.is_closed:
+            await self.stop()
+
+    @property
+    def is_closed(self) -> bool:
+        """Returns True if the bot has closed."""
+        return self._closed
+
+    @property
+    def is_ready(self) -> bool:
+        """Returns True if the bot is ready."""
+        return self._ready.is_set()
+
+    @property
+    def latency(self) -> float:
+        """Returns the latency of the websocket connection (seconds)."""
+        return self._connection_state.latency
+
+    @property
+    def average_latency(self) -> float:
+        """Returns the average latency of the websocket connection (seconds)."""
+        return self._connection_state.average_latency
+
+    @property
+    def start_time(self) -> datetime:
+        """The start time of the bot."""
+        return self._connection_state.start_time
+
+    @property
+    def gateway_started(self) -> bool:
+        """Returns if the gateway has been started."""
+        return self._connection_state.gateway_started.is_set()
+
+    @property
+    def user(self) -> ClientUser:
+        """Returns the bot's user."""
+        return self._user
+
+    @property
+    def app(self) -> Application:
+        """Returns the bots application."""
+        return self._app
+
+    @property
+    def owner(self) -> Optional["User"]:
+        """Returns the bot's owner'."""
+        try:
+            return self.app.owner
+        except TypeError:
+            return MISSING
+
+    @property
+    def owners(self) -> List["User"]:
+        """Returns the bot's owners as declared via `client.owner_ids`."""
+        return [self.get_user(u_id) for u_id in self.owner_ids]
+
+    @property
+    def guilds(self) -> List["Guild"]:
+        """Returns a list of all guilds the bot is in."""
+        return self.user.guilds
+
+    @property
+    def status(self) -> Status:
+        """
+        Get the status of the bot.
+
+        IE online, afk, dnd
+
+        """
+        return self._status
+
+    @property
+    def activity(self) -> Activity:
+        """Get the activity of the bot."""
+        return self._activity
+
+    @property
+    def application_commands(self) -> List[InteractionCommand]:
+        """A list of all application commands registered within the bot."""
+        commands = []
+        for scope in self.interactions_by_scope.keys():
+            commands += [cmd for cmd in self.interactions_by_scope[scope].values() if cmd not in commands]
+
+        return commands
+
+    @property
+    def ws(self) -> GatewayClient:
+        """Returns the websocket client."""
+        return self._connection_state.gateway
+
+    def get_guild_websocket(self, id: "Snowflake_Type") -> GatewayClient:
+        return self.ws
+
+    def _sanity_check(self) -> None:
+        """Checks for possible and common errors in the bot's configuration."""
+        self.logger.debug("Running client sanity checks...")
+        contexts = {
+            self.interaction_context: InteractionContext,
+            self.component_context: ComponentContext,
+            self.autocomplete_context: AutocompleteContext,
+            self.modal_context: ModalContext,
+        }
+        for obj, expected in contexts.items():
+            if not issubclass(obj, expected):
+                raise TypeError(f"{obj.__name__} must inherit from {expected.__name__}")
+
+        if self.del_unused_app_cmd:
+            self.logger.warning(
+                "As `delete_unused_application_cmds` is enabled, the client must cache all guilds app-commands, this could take a while."
+            )
+
+        if Intents.GUILDS not in self._connection_state.intents:
+            self.logger.warning("GUILD intent has not been enabled; this is very likely to cause errors")
+
+        if self.fetch_members and Intents.GUILD_MEMBERS not in self._connection_state.intents:
+            raise BotException("Members Intent must be enabled in order to use fetch members")
+        if self.fetch_members:
+            self.logger.warning("fetch_members enabled; startup will be delayed")
+
+        if len(self.processors) == 0:
+            self.logger.warning("No Processors are loaded! This means no events will be processed!")
+
+        caches = [
+            c[0]
+            for c in inspect.getmembers(self.cache, predicate=lambda x: isinstance(x, dict))
+            if not c[0].startswith("__")
+        ]
+        for cache in caches:
+            _cache_obj = getattr(self.cache, cache)
+            if isinstance(_cache_obj, NullCache):
+                self.logger.warning(f"{cache} has been disabled")
+
+    def _queue_task(self, coro: Listener, event: BaseEvent, *args, **kwargs) -> asyncio.Task:
+        async def _async_wrap(_coro: Listener, _event: BaseEvent, *_args, **_kwargs) -> None:
+            try:
+                if (
+                    not isinstance(_event, (events.Error, events.RawGatewayEvent))
+                    and coro.delay_until_ready
+                    and not self.is_ready
+                ):
+                    await self.wait_until_ready()
+
+                if len(_event.__attrs_attrs__) == 2 and coro.event != "event":
+                    # override_name & bot & logging
+                    await _coro()
+                else:
+                    await _coro(_event, *_args, **_kwargs)
+            except asyncio.CancelledError:
+                pass
+            except Exception as e:
+                if isinstance(event, events.Error):
+                    # No infinite loops please
+                    self.default_error_handler(repr(event), e)
+                else:
+                    self.dispatch(events.Error(source=repr(event), error=e))
+
+        try:
+            asyncio.get_running_loop()
+            return asyncio.create_task(
+                _async_wrap(coro, event, *args, **kwargs), name=f"interactions:: {event.resolved_name}"
+            )
+        except RuntimeError:
+            self.logger.debug("Event loop is closed; queuing task for execution on startup")
+            self.async_startup_tasks.append((_async_wrap, (coro, event, *args), kwargs))
+
+    @staticmethod
+    def default_error_handler(source: str, error: BaseException) -> None:
+        """
+        The default error logging behaviour.
+
+        Args:
+            source: The source of this error
+            error: The exception itself
+
+        """
+        out = traceback.format_exception(error)
+
+        if isinstance(error, HTTPException):
+            # HTTPException's are of 3 known formats, we can parse them for human readable errors
+            with contextlib.suppress(Exception):
+                out = [str(error)]
+        get_logger().error(
+            "Ignoring exception in {}:{}{}".format(source, "\n" if len(out) > 1 else " ", "".join(out)),
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_error(self, event: events.Error) -> None:
+        """
+        Catches all errors dispatched by the library.
+
+        By default it will format and print them to console.
+
+        Listen to the `Error` event to overwrite this behaviour.
+
+        """
+        self.default_error_handler(event.source, event.error)
+
+    @Listener.create(is_default_listener=True)
+    async def on_command_error(self, event: events.CommandError) -> None:
+        """
+        Catches all errors dispatched by commands.
+
+        By default it will dispatch the `Error` event.
+
+        Listen to the `CommandError` event to overwrite this behaviour.
+
+        """
+        self.dispatch(
+            events.Error(
+                source=f"cmd `/{event.ctx.invoke_target}`",
+                error=event.error,
+                args=event.args,
+                kwargs=event.kwargs,
+                ctx=event.ctx,
+            )
+        )
+        with contextlib.suppress(errors.LibraryException):
+            if isinstance(event.error, errors.CommandOnCooldown):
+                await event.ctx.send(
+                    embeds=Embed(
+                        description=f"This command is on cooldown!\n"
+                        f"Please try again in {int(event.error.cooldown.get_cooldown_time())} seconds",
+                        color=BrandColors.FUCHSIA,
+                    )
+                )
+            elif isinstance(event.error, errors.MaxConcurrencyReached):
+                await event.ctx.send(
+                    embeds=Embed(
+                        description="This command has reached its maximum concurrent usage!\n"
+                        "Please try again shortly.",
+                        color=BrandColors.FUCHSIA,
+                    )
+                )
+            elif isinstance(event.error, errors.CommandCheckFailure):
+                await event.ctx.send(
+                    embeds=Embed(
+                        description="You do not have permission to run this command!",
+                        color=BrandColors.YELLOW,
+                    )
+                )
+            elif self.send_command_tracebacks:
+                out = "".join(traceback.format_exception(event.error))
+                if self.http.token is not None:
+                    out = out.replace(self.http.token, "[REDACTED TOKEN]")
+                await event.ctx.send(
+                    embeds=Embed(
+                        title=f"Error: {type(event.error).__name__}",
+                        color=BrandColors.RED,
+                        description=f"```\n{out[:EMBED_MAX_DESC_LENGTH-8]}```",
+                    )
+                )
+
+    @Listener.create(is_default_listener=True)
+    async def on_command_completion(self, event: events.CommandCompletion) -> None:
+        """
+        Called *after* any command is ran.
+
+        By default, it will simply log the command.
+
+        Listen to the `CommandCompletion` event to overwrite this behaviour.
+
+        """
+        self.logger.info(f"Command Called: {event.ctx.invoke_target} with {event.ctx.args = } | {event.ctx.kwargs = }")
+
+    @Listener.create(is_default_listener=True)
+    async def on_component_error(self, event: events.ComponentError) -> None:
+        """
+        Catches all errors dispatched by components.
+
+        By default it will dispatch the `Error` event.
+
+        Listen to the `ComponentError` event to overwrite this behaviour.
+
+        """
+        self.dispatch(
+            events.Error(
+                source=f"Component Callback for {event.ctx.custom_id}",
+                error=event.error,
+                args=event.args,
+                kwargs=event.kwargs,
+                ctx=event.ctx,
+            )
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_component_completion(self, event: events.ComponentCompletion) -> None:
+        """
+        Called *after* any component callback is ran.
+
+        By default, it will simply log the component use.
+
+        Listen to the `ComponentCompletion` event to overwrite this behaviour.
+
+        """
+        symbol = "¢"
+        self.logger.info(
+            f"Component Called: {symbol}{event.ctx.invoke_target} with {event.ctx.args = } | {event.ctx.kwargs = }"
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_autocomplete_error(self, event: events.AutocompleteError) -> None:
+        """
+        Catches all errors dispatched by autocompletion options.
+
+        By default it will dispatch the `Error` event.
+
+        Listen to the `AutocompleteError` event to overwrite this behaviour.
+
+        """
+        self.dispatch(
+            events.Error(
+                source=f"Autocomplete Callback for /{event.ctx.invoke_target} - Option: {event.ctx.focussed_option}",
+                error=event.error,
+                args=event.args,
+                kwargs=event.kwargs,
+                ctx=event.ctx,
+            )
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_autocomplete_completion(self, event: events.AutocompleteCompletion) -> None:
+        """
+        Called *after* any autocomplete callback is ran.
+
+        By default, it will simply log the autocomplete callback.
+
+        Listen to the `AutocompleteCompletion` event to overwrite this behaviour.
+
+        """
+        symbol = "$"
+        self.logger.info(
+            f"Autocomplete Called: {symbol}{event.ctx.invoke_target} with {event.ctx.focussed_option = } | {event.ctx.kwargs = }"
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_modal_error(self, event: events.ModalError) -> None:
+        """
+        Catches all errors dispatched by modals.
+
+        By default it will dispatch the `Error` event.
+
+        Listen to the `ModalError` event to overwrite this behaviour.
+
+        """
+        self.dispatch(
+            events.Error(
+                source=f"Modal Callback for custom_id {event.ctx.custom_id}",
+                error=event.error,
+                args=event.args,
+                kwargs=event.kwargs,
+                ctx=event.ctx,
+            )
+        )
+
+    @Listener.create(is_default_listener=True)
+    async def on_modal_completion(self, event: events.ModalCompletion) -> None:
+        """
+        Called *after* any modal callback is ran.
+
+        By default, it will simply log the modal callback.
+
+        Listen to the `ModalCompletion` event to overwrite this behaviour.
+
+        """
+        self.logger.info(f"Modal Called: {event.ctx.custom_id = } with {event.ctx.responses = }")
+
+    @Listener.create()
+    async def on_resume(self) -> None:
+        self._ready.set()
+
+    @Listener.create(is_default_listener=True)
+    async def _on_websocket_ready(self, event: events.RawGatewayEvent) -> None:
+        """
+        Catches websocket ready and determines when to dispatch the client `READY` signal.
+
+        Args:
+            event: The websocket ready packet
+
+        """
+        data = event.data
+        expected_guilds = {to_snowflake(guild["id"]) for guild in data["guilds"]}
+        self._user._add_guilds(expected_guilds)
+
+        if not self._startup:
+            while len(self.guilds) != len(expected_guilds):
+                try:  # wait to let guilds cache
+                    await asyncio.wait_for(self._guild_event.wait(), self.guild_event_timeout)
+                except asyncio.TimeoutError:
+                    # this will *mostly* occur when a guild has been shadow deleted by discord T&S.
+                    # there is no way to check for this, so we just need to wait for this to time out.
+                    # We still log it though, just in case.
+                    self.logger.debug("Timeout waiting for guilds cache")
+                    break
+                self._guild_event.clear()
+
+            if self.fetch_members:
+                # ensure all guilds have completed chunking
+                for guild in self.guilds:
+                    if guild and not guild.chunked.is_set():
+                        self.logger.debug(f"Waiting for {guild.id} to chunk")
+                        await guild.chunked.wait()
+
+            # cache slash commands
+            if not self._startup:
+                await self._init_interactions()
+
+            self._startup = True
+            self.dispatch(events.Startup())
+
+        else:
+            # reconnect ready
+            ready_guilds = set()
+
+            async def _temp_listener(_event: events.RawGatewayEvent) -> None:
+                ready_guilds.add(_event.data["id"])
+
+            listener = Listener.create("_on_raw_guild_create")(_temp_listener)
+            self.add_listener(listener)
+
+            while True:
+                try:
+                    await asyncio.wait_for(self._guild_event.wait(), self.guild_event_timeout)
+                    if len(ready_guilds) == len(expected_guilds):
+                        break
+                except asyncio.TimeoutError:
+                    break
+
+            self.listeners["raw_guild_create"].remove(listener)
+
+        self._ready.set()
+        self.dispatch(events.Ready())
+
+    async def login(self, token: str | None = None) -> None:
+        """
+        Login to discord via http.
+
+        !!! note
+            You will need to run Client.start_gateway() before you start receiving gateway events.
+
+        Args:
+            token str: Your bot's token
+
+        """
+        if not self.token and not token:
+            raise RuntimeError(
+                "No token provided - please provide a token in the client constructor or via the login method."
+            )
+        self.token = (token or self.token).strip()
+
+        # i needed somewhere to put this call,
+        # login will always run after initialisation
+        # so im gathering commands here
+        self._gather_callbacks()
+
+        self.logger.debug("Attempting to login")
+        me = await self.http.login(self.token)
+        self._user = ClientUser.from_dict(me, self)
+        self.cache.place_user_data(me)
+        self._app = Application.from_dict(await self.http.get_current_bot_information(), self)
+        self._mention_reg = re.compile(rf"^(<@!?{self.user.id}*>\s)")
+
+        if self.app.owner:
+            self.owner_ids.add(self.app.owner.id)
+
+        self.dispatch(events.Login())
+
+    async def astart(self, token: str | None = None) -> None:
+        """
+        Asynchronous method to start the bot.
+
+        Args:
+            token: Your bot's token
+        """
+        await self.login(token)
+
+        # run any pending startup tasks
+        if self.async_startup_tasks:
+            try:
+                await asyncio.gather(
+                    *[
+                        task[0](*task[1] if len(task) > 1 else [], **task[2] if len(task) == 3 else {})
+                        for task in self.async_startup_tasks
+                    ]
+                )
+            except Exception as e:
+                self.dispatch(events.Error(source="async-extension-loader", error=e))
+        try:
+            await self._connection_state.start()
+        finally:
+            await self.stop()
+
+    def start(self, token: str | None = None) -> None:
+        """
+        Start the bot.
+
+        If `uvloop` is installed, it will be used.
+
+        info:
+            This is the recommended method to start the bot
+        """
+        try:
+            import uvloop
+
+            has_uvloop = True
+        except ImportError:
+            has_uvloop = False
+
+        with contextlib.suppress(KeyboardInterrupt):
+            if has_uvloop:
+                self.logger.info("uvloop is installed, using it")
+                if sys.version_info >= (3, 11):
+                    with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
+                        runner.run(self.astart(token))
+                else:
+                    uvloop.install()
+                    asyncio.run(self.astart(token))
+            else:
+                asyncio.run(self.astart(token))
+
+    async def start_gateway(self) -> None:
+        """Starts the gateway connection."""
+        try:
+            await self._connection_state.start()
+        finally:
+            await self.stop()
+
+    async def stop(self) -> None:
+        """Shutdown the bot."""
+        self.logger.debug("Stopping the bot.")
+        self._ready.clear()
+        await self.http.close()
+        await self._connection_state.stop()
+
+    async def _process_waits(self, event: events.BaseEvent) -> None:
+        if _waits := self.waits.get(event.resolved_name, []):
+            index_to_remove = []
+            for i, _wait in enumerate(_waits):
+                result = await _wait(event)
+                if result:
+                    index_to_remove.append(i)
+
+            for idx in sorted(index_to_remove, reverse=True):
+                _waits.pop(idx)
+
+    def dispatch(self, event: events.BaseEvent, *args, **kwargs) -> None:
+        """
+        Dispatch an event.
+
+        Args:
+            event: The event to be dispatched.
+
+        """
+        if listeners := self.listeners.get(event.resolved_name, []):
+            self.logger.debug(f"Dispatching Event: {event.resolved_name}")
+            event.bot = self
+            for _listen in listeners:
+                try:
+                    self._queue_task(_listen, event, *args, **kwargs)
+                except Exception as e:
+                    raise BotException(
+                        f"An error occurred attempting during {event.resolved_name} event processing"
+                    ) from e
+
+        try:
+            asyncio.get_running_loop()
+            _ = asyncio.create_task(self._process_waits(event))
+        except RuntimeError:
+            # dispatch attempt before event loop is running
+            self.async_startup_tasks.append((self._process_waits, (event,), {}))
+
+        if "event" in self.listeners:
+            # special meta event listener
+            for _listen in self.listeners["event"]:
+                self._queue_task(_listen, event, *args, **kwargs)
+
+    async def wait_until_ready(self) -> None:
+        """Waits for the client to become ready."""
+        await self._ready.wait()
+
+    def wait_for(
+        self,
+        event: Union[str, "BaseEvent"],
+        checks: Absent[Optional[Union[Callable[..., bool], Callable[..., Awaitable[bool]]]]] = MISSING,
+        timeout: Optional[float] = None,
+    ) -> Any:
+        """
+        Waits for a WebSocket event to be dispatched.
+
+        Args:
+            event: The name of event to wait.
+            checks: A predicate to check what to wait for.
+            timeout: The number of seconds to wait before timing out.
+
+        Returns:
+            The event object.
+        """
+        event = get_event_name(event)
+
+        if event not in self.waits:
+            self.waits[event] = []
+
+        future = asyncio.Future()
+        self.waits[event].append(Wait(event, checks, future))
+
+        return asyncio.wait_for(future, timeout)
+
+    async def wait_for_modal(
+        self,
+        modal: "Modal",
+        author: Optional["Snowflake_Type"] = None,
+        timeout: Optional[float] = None,
+    ) -> "ModalContext":
+        """
+        Wait for a modal response.
+
+        Args:
+            modal: The modal we're waiting for.
+            author: The user we're waiting for to reply
+            timeout: A timeout in seconds to stop waiting
+
+        Returns:
+            The context of the modal response
+
+        Raises:
+            asyncio.TimeoutError: if no response is received that satisfies the predicate before timeout seconds have passed
+
+        """
+        author = to_snowflake(author) if author else None
+
+        def predicate(event) -> bool:
+            if modal.custom_id != event.ctx.custom_id:
+                return False
+            return author == to_snowflake(event.ctx.author) if author else True
+
+        resp = await self.wait_for("modal_completion", predicate, timeout)
+        return resp.ctx
+
+    async def wait_for_component(
+        self,
+        messages: Union[Message, int, list] = None,
+        components: Optional[
+            Union[
+                List[List[Union["BaseComponent", dict]]],
+                List[Union["BaseComponent", dict]],
+                "BaseComponent",
+                dict,
+            ]
+        ] = None,
+        check: Optional[Callable] = None,
+        timeout: Optional[float] = None,
+    ) -> "events.Component":
+        """
+        Waits for a component to be sent to the bot.
+
+        Args:
+            messages: The message object to check for.
+            components: The components to wait for.
+            check: A predicate to check what to wait for.
+            timeout: The number of seconds to wait before timing out.
+
+        Returns:
+            `Component` that was invoked. Use `.ctx` to get the `ComponentContext`.
+
+        Raises:
+            asyncio.TimeoutError: if timed out
+
+        """
+        if not messages and not components:
+            raise ValueError("You must specify messages or components (or both)")
+
+        message_ids = (
+            to_snowflake_list(messages) if isinstance(messages, list) else to_snowflake(messages) if messages else None
+        )
+        custom_ids = list(get_components_ids(components)) if components else None
+
+        # automatically convert improper custom_ids
+        if custom_ids and not all(isinstance(x, str) for x in custom_ids):
+            custom_ids = [str(i) for i in custom_ids]
+
+        def _check(event: events.Component) -> bool:
+            ctx: ComponentContext = event.ctx
+            # if custom_ids is empty or there is a match
+            wanted_message = not message_ids or ctx.message.id in (
+                [message_ids] if isinstance(message_ids, int) else message_ids
+            )
+            wanted_component = not custom_ids or ctx.custom_id in custom_ids
+            if wanted_message and wanted_component:
+                return bool(check is None or check(event))
+            return False
+
+        return await self.wait_for("component", checks=_check, timeout=timeout)
+
+    def command(self, *args, **kwargs) -> Callable:
+        """A decorator that registers a command. Aliases `interactions.slash_command`"""
+        raise NotImplementedError  # TODO: implement
+
+    def listen(self, event_name: Absent[str] = MISSING) -> Callable[[AsyncCallable], Listener]:
+        """
+        A decorator to be used in situations that the library can't automatically hook your listeners. Ideally, the standard listen decorator should be used, not this.
+
+        Args:
+            event_name: The event name to use, if not the coroutine name
+
+        Returns:
+            A listener that can be used to hook into the event.
+
+        """
+
+        def wrapper(coro: AsyncCallable) -> Listener:
+            listener = Listener.create(event_name)(coro)
+            self.add_listener(listener)
+            return listener
+
+        return wrapper
+
+    event = listen  # alias for easier migration
+
+    def add_event_processor(self, event_name: Absent[str] = MISSING) -> Callable[[AsyncCallable], AsyncCallable]:
+        """
+        A decorator to be used to add event processors.
+
+        Args:
+            event_name: The event name to use, if not the coroutine name
+
+        Returns:
+            A function that can be used to hook into the event.
+
+        """
+
+        def wrapper(coro: AsyncCallable) -> AsyncCallable:
+            name = event_name
+            if name is MISSING:
+                name = coro.__name__
+            name = name.lstrip("_")
+            name = name.removeprefix("on_")
+            self.processors[name] = coro
+            return coro
+
+        return wrapper
+
+    def add_listener(self, listener: Listener) -> None:
+        """
+        Add a listener for an event, if no event is passed, one is determined.
+
+        Args:
+            listener Listener: The listener to add to the client
+
+        """
+        if listener.event == "event":
+            self.logger.critical(
+                f"Subscribing to `{listener.event}` - Meta Events are very expensive; remember to remove it before releasing your bot"
+            )
+
+        if not listener.is_default_listener:
+            # check that the required intents are enabled
+
+            event_class_name = "".join([name.capitalize() for name in listener.event.split("_")])
+            if event_class := globals().get(event_class_name):
+                if required_intents := _INTENT_EVENTS.get(event_class):
+                    if all(required_intent not in self.intents for required_intent in required_intents):
+                        self.logger.warning(
+                            f"Event `{listener.event}` will not work since the required intent is not set -> Requires any of: `{required_intents}`"
+                        )
+
+        # prevent the same callback being added twice
+        if listener in self.listeners.get(listener.event, []):
+            self.logger.debug(f"Listener {listener} has already been hooked, not re-hooking it again")
+            return
+
+        if listener.event not in self.listeners:
+            self.listeners[listener.event] = []
+        self.listeners[listener.event].append(listener)
+
+        # check if other listeners are to be deleted
+        default_listeners = [c_listener.is_default_listener for c_listener in self.listeners[listener.event]]
+        removes_defaults = [c_listener.disable_default_listeners for c_listener in self.listeners[listener.event]]
+
+        if any(default_listeners) and any(removes_defaults):
+            self.listeners[listener.event] = [
+                c_listener for c_listener in self.listeners[listener.event] if not c_listener.is_default_listener
+            ]
+
+    def add_interaction(self, command: InteractionCommand) -> bool:
+        """
+        Add a slash command to the client.
+
+        Args:
+            command InteractionCommand: The command to add
+
+        """
+        if self.debug_scope:
+            command.scopes = [self.debug_scope]
+
+        if self.disable_dm_commands:
+            command.dm_permission = False
+
+        # for SlashCommand objs without callback (like objects made to hold group info etc)
+        if command.callback is None:
+            return False
+
+        if isinstance(command, SlashCommand):
+            command._parse_parameters()
+
+        base, group, sub, *_ = [*command.resolved_name.split(" "), None, None]
+
+        for scope in command.scopes:
+            if scope not in self.interactions_by_scope:
+                self.interactions_by_scope[scope] = {}
+            elif command.resolved_name in self.interactions_by_scope[scope]:
+                old_cmd = self.interactions_by_scope[scope][command.resolved_name]
+                raise ValueError(f"Duplicate Command! {scope}::{old_cmd.resolved_name}")
+
+            # if self.enforce_interaction_perms:
+            #     command.checks.append(command._permission_enforcer)
+
+            self.interactions_by_scope[scope][command.resolved_name] = command
+
+            if scope not in self.interaction_tree:
+                self.interaction_tree[scope] = {}
+
+            if group is None or isinstance(command, ContextMenu):
+                self.interaction_tree[scope][command.resolved_name] = command
+            else:
+                if not (current := self.interaction_tree[scope].get(base)) or isinstance(current, SlashCommand):
+                    self.interaction_tree[scope][base] = {}
+                if sub is None:
+                    self.interaction_tree[scope][base][group] = command
+                else:
+                    if not (current := self.interaction_tree[scope][base].get(group)) or isinstance(
+                        current, SlashCommand
+                    ):
+                        self.interaction_tree[scope][base][group] = {}
+                    self.interaction_tree[scope][base][group][sub] = command
+
+        return True
+
+    def add_component_callback(self, command: ComponentCommand) -> None:
+        """
+        Add a component callback to the client.
+
+        Args:
+            command: The command to add
+
+        """
+        for listener in command.listeners:
+            # I know this isn't an ideal solution, but it means we can lookup callbacks with O(1)
+            if listener in self._component_callbacks.keys():
+                raise ValueError(f"Duplicate Component! Multiple component callbacks for `{listener}`")
+            self._component_callbacks[listener] = command
+            continue
+
+    def add_modal_callback(self, command: ModalCommand) -> None:
+        """
+        Add a modal callback to the client.
+
+        Args:
+            command: The command to add
+        """
+        for listener in command.listeners:
+            if listener in self._modal_callbacks.keys():
+                raise ValueError(f"Duplicate Component! Multiple modal callbacks for `{listener}`")
+            self._modal_callbacks[listener] = command
+            continue
+
+    def add_global_autocomplete(self, callback: GlobalAutoComplete) -> None:
+        """
+        Add a global autocomplete to the client.
+
+        Args:
+            callback: The autocomplete to add
+        """
+        self._global_autocompletes[callback.option_name] = callback
+
+    def add_command(self, func: Callable) -> None:
+        """
+        Add a command to the client.
+
+        Args:
+            func: The command to add
+        """
+        if isinstance(func, ModalCommand):
+            self.add_modal_callback(func)
+        elif isinstance(func, ComponentCommand):
+            self.add_component_callback(func)
+        elif isinstance(func, InteractionCommand):
+            self.add_interaction(func)
+        elif isinstance(func, Listener):
+            self.add_listener(func)
+        elif isinstance(func, GlobalAutoComplete):
+            self.add_global_autocomplete(func)
+        elif not isinstance(func, BaseCommand):
+            raise TypeError("Invalid command type")
+
+        if not func.callback:
+            # for group = SlashCommand(...) usage
+            return
+
+        if isinstance(func.callback, functools.partial):
+            ext = getattr(func, "extension", None)
+            self.logger.debug(f"Added callback: {f'{ext.name}.' if ext else ''}{func.callback.func.__name__}")
+        else:
+            self.logger.debug(f"Added callback: {func.callback.__name__}")
+
+        self.dispatch(CallbackAdded(callback=func, extension=func.extension if hasattr(func, "extension") else None))
+
+    def _gather_callbacks(self) -> None:
+        """Gathers callbacks from __main__ and self."""
+
+        def process(callables, location: str) -> None:
+            added = 0
+            for func in callables:
+                try:
+                    self.add_command(func)
+                    added += 1
+                except TypeError:
+                    self.logger.debug(f"Failed to add callback {func} from {location}")
+                    continue
+
+            self.logger.debug(f"{added} callbacks have been loaded from {location}.")
+
+        main_commands = [
+            obj for _, obj in inspect.getmembers(sys.modules["__main__"]) if isinstance(obj, CallbackObject)
+        ]
+        client_commands = [
+            obj.copy_with_binding(self) for _, obj in inspect.getmembers(self) if isinstance(obj, CallbackObject)
+        ]
+        process(main_commands, "__main__")
+        process(client_commands, self.__class__.__name__)
+
+        [wrap_partial(obj, self) for _, obj in inspect.getmembers(self) if isinstance(obj, Task)]
+
+    async def _init_interactions(self) -> None:
+        """
+        Initialise slash commands.
+
+        If `sync_interactions` this will submit all registered slash
+        commands to discord. Otherwise, it will get the list of
+        interactions and cache their scopes.
+
+        """
+        # allow for ext and main to share the same decorator
+        try:
+            if self.sync_interactions:
+                await self.synchronise_interactions()
+            else:
+                await self._cache_interactions(warn_missing=False)
+        except Exception as e:
+            self.dispatch(events.Error(source="Interaction Syncing", error=e))
+
+    async def _cache_interactions(self, warn_missing: bool = False) -> None:
+        """Get all interactions used by this bot and cache them."""
+        if warn_missing or self.del_unused_app_cmd:
+            bot_scopes = {g.id for g in self.cache.guild_cache.values()}
+            bot_scopes.add(GLOBAL_SCOPE)
+        else:
+            bot_scopes = set(self.interactions_by_scope)
+
+        sem = asyncio.Semaphore(5)
+
+        async def wrap(*args, **kwargs) -> Absent[List[Dict]]:
+            async with sem:
+                try:
+                    return await self.http.get_application_commands(*args, **kwargs)
+                except Forbidden:
+                    return MISSING
+
+        results = await asyncio.gather(*[wrap(self.app.id, scope) for scope in bot_scopes])
+        results = dict(zip(bot_scopes, results, strict=False))
+
+        for scope, remote_cmds in results.items():
+            if remote_cmds == MISSING:
+                self.logger.debug(f"Bot was not invited to guild {scope} with `application.commands` scope")
+                continue
+
+            remote_cmds = {cmd_data["name"]: cmd_data for cmd_data in remote_cmds}
+
+            found = set()
+            if scope in self.interactions_by_scope:
+                for cmd in self.interactions_by_scope[scope].values():
+                    cmd_name = str(cmd.name)
+                    cmd_data = remote_cmds.get(cmd_name, MISSING)
+                    if cmd_data is MISSING:
+                        if cmd_name not in found and warn_missing:
+                            self.logger.error(
+                                f'Detected yet to sync slash command "/{cmd_name}" for scope '
+                                f"{'global' if scope == GLOBAL_SCOPE else scope}"
+                            )
+                        continue
+                    found.add(cmd_name)
+                    self._interaction_lookup[cmd.resolved_name] = cmd
+                    cmd.cmd_id[scope] = int(cmd_data["id"])
+
+            if warn_missing:
+                for cmd_data in remote_cmds.values():
+                    self.logger.error(
+                        f"Detected unimplemented slash command \"/{cmd_data['name']}\" for scope "
+                        f"{'global' if scope == GLOBAL_SCOPE else scope}"
+                    )
+
+    async def synchronise_interactions(
+        self,
+        *,
+        scopes: Sequence["Snowflake_Type"] = MISSING,
+        delete_commands: Absent[bool] = MISSING,
+    ) -> None:
+        """
+        Synchronise registered interactions with discord.
+
+        Args:
+            scopes: Optionally specify which scopes are to be synced
+            delete_commands: Override the client setting and delete commands
+        """
+        s = time.perf_counter()
+        _delete_cmds = self.del_unused_app_cmd if delete_commands is MISSING else delete_commands
+        await self._cache_interactions()
+
+        if scopes is not MISSING:
+            cmd_scopes = scopes
+        elif self.del_unused_app_cmd:
+            # if we're deleting unused commands, we check all scopes
+            cmd_scopes = [to_snowflake(g_id) for g_id in self._user._guild_ids] + [GLOBAL_SCOPE]
+        else:
+            # if we're not deleting, just check the scopes we have cmds registered in
+            cmd_scopes = list(set(self.interactions_by_scope) | {GLOBAL_SCOPE})
+
+        local_cmds_json = application_commands_to_dict(self.interactions_by_scope, self)
+
+        async def sync_scope(cmd_scope) -> None:
+            sync_needed_flag = False  # a flag to force this scope to synchronise
+            sync_payload = []  # the payload to be pushed to discord
+
+            try:
+                try:
+                    remote_commands = await self.http.get_application_commands(self.app.id, cmd_scope)
+                except Forbidden:
+                    self.logger.warning(f"Bot is lacking `application.commands` scope in {cmd_scope}!")
+                    return
+
+                for local_cmd in self.interactions_by_scope.get(cmd_scope, {}).values():
+                    # get remote equivalent of this command
+                    remote_cmd_json = next(
+                        (v for v in remote_commands if int(v["id"]) == local_cmd.cmd_id.get(cmd_scope)),
+                        None,
+                    )
+                    # get json representation of this command
+                    local_cmd_json = next((c for c in local_cmds_json[cmd_scope] if c["name"] == str(local_cmd.name)))
+
+                    # this works by adding any command we *want* on Discord, to a payload, and synchronising that
+                    # this allows us to delete unused commands, add new commands, or do nothing in 1 or less API calls
+
+                    if sync_needed(local_cmd_json, remote_cmd_json):
+                        # determine if the local and remote commands are out-of-sync
+                        sync_needed_flag = True
+                        sync_payload.append(local_cmd_json)
+                    elif not _delete_cmds and remote_cmd_json:
+                        _remote_payload = {
+                            k: v for k, v in remote_cmd_json.items() if k not in ("id", "application_id", "version")
+                        }
+                        sync_payload.append(_remote_payload)
+                    elif _delete_cmds:
+                        sync_payload.append(local_cmd_json)
+
+                sync_payload = [FastJson.loads(_dump) for _dump in {FastJson.dumps(_cmd) for _cmd in sync_payload}]
+
+                if sync_needed_flag or (_delete_cmds and len(sync_payload) < len(remote_commands)):
+                    # synchronise commands if flag is set, or commands are to be deleted
+                    self.logger.info(f"Overwriting {cmd_scope} with {len(sync_payload)} application commands")
+                    sync_response: list[dict] = await self.http.overwrite_application_commands(
+                        self.app.id, sync_payload, cmd_scope
+                    )
+                    self._cache_sync_response(sync_response, cmd_scope)
+                else:
+                    self.logger.debug(f"{cmd_scope} is already up-to-date with {len(remote_commands)} commands.")
+
+            except Forbidden as e:
+                raise InteractionMissingAccess(cmd_scope) from e
+            except HTTPException as e:
+                self._raise_sync_exception(e, local_cmds_json, cmd_scope)
+
+        await asyncio.gather(*[sync_scope(scope) for scope in cmd_scopes])
+
+        t = time.perf_counter() - s
+        self.logger.debug(f"Sync of {len(cmd_scopes)} scopes took {t} seconds")
+
+    def get_application_cmd_by_id(
+        self, cmd_id: "Snowflake_Type", *, scope: "Snowflake_Type" = None
+    ) -> Optional[InteractionCommand]:
+        """
+        Get a application command from the internal cache by its ID.
+
+        Args:
+            cmd_id: The ID of the command
+            scope: Optionally specify a scope to search in
+
+        Returns:
+            The command, if one with the given ID exists internally, otherwise None
+
+        """
+        if scope is not None:
+            return self.interactions_by_scope.get(scope, {}).get(cmd_id)
+        return next(
+            (scope[cmd_id] for scope in self.interactions_by_scope.values() if cmd_id in scope),
+            None,
+        )
+
+    def _raise_sync_exception(self, e: HTTPException, cmds_json: dict, cmd_scope: "Snowflake_Type") -> NoReturn:
+        try:
+            if isinstance(e.errors, dict):
+                for cmd_num in e.errors.keys():
+                    cmd = cmds_json[cmd_scope][int(cmd_num)]
+                    output = e.search_for_message(e.errors[cmd_num], cmd)
+                    if len(output) > 1:
+                        output = "\n".join(output)
+                        self.logger.error(f"Multiple Errors found in command `{cmd['name']}`:\n{output}")
+                    else:
+                        self.logger.error(f"Error in command `{cmd['name']}`: {output[0]}")
+            else:
+                raise e from None
+        except Exception:
+            # the above shouldn't fail, but if it does, just raise the exception normally
+            raise e from None
+
+    def _cache_sync_response(self, sync_response: list[dict], scope: "Snowflake_Type") -> None:
+        for cmd_data in sync_response:
+            command_id = Snowflake(cmd_data["id"])
+            command_name = cmd_data["name"]
+
+            if any(
+                option["type"] in (OptionType.SUB_COMMAND, OptionType.SUB_COMMAND_GROUP)
+                for option in cmd_data.get("options", [])
+            ):
+                for option in cmd_data.get("options", []):
+                    if option["type"] in (OptionType.SUB_COMMAND, OptionType.SUB_COMMAND_GROUP):
+                        command_name = f"{command_name} {option['name']}"
+                        if option["type"] == OptionType.SUB_COMMAND_GROUP:
+                            for _sc in option.get("options", []):
+                                command_name = f"{command_name} {_sc['name']}"
+                                if command := self.interactions_by_scope[scope].get(command_name):
+                                    command.cmd_id[scope] = command_id
+                                    self._interaction_lookup[command.resolved_name] = command
+                        elif command := self.interactions_by_scope[scope].get(command_name):
+                            command.cmd_id[scope] = command_id
+                            self._interaction_lookup[command.resolved_name] = command
+                            continue
+            elif command := self.interactions_by_scope[scope].get(command_name):
+                command.cmd_id[scope] = command_id
+                self._interaction_lookup[command.resolved_name] = command
+                continue
+
+    async def get_context(self, data: dict) -> InteractionContext:
+        match data["type"]:
+            case InteractionType.MESSAGE_COMPONENT:
+                cls = self.component_context.from_dict(self, data)
+            case InteractionType.AUTOCOMPLETE:
+                cls = self.autocomplete_context.from_dict(self, data)
+            case InteractionType.MODAL_RESPONSE:
+                cls = self.modal_context.from_dict(self, data)
+            case InteractionType.APPLICATION_COMMAND:
+                if data["data"].get("target_id"):
+                    cls = self.context_menu_context.from_dict(self, data)
+                else:
+                    cls = self.slash_context.from_dict(self, data)
+            case _:
+                self.logger.warning(f"Unknown interaction type [{data['type']}] - please update or report this.")
+                cls = self.interaction_context.from_dict(self, data)
+        if not cls.channel:
+            # fallback channel if not provided
+            try:
+                if cls.guild_id:
+                    channel = await self.cache.fetch_channel(data["channel_id"])
+                else:
+                    channel = await self.cache.fetch_dm_channel(cls.author_id)
+                cls.channel_id = channel.id
+            except Forbidden:
+                self.logger.debug(f"Failed to fetch channel data for {data['channel_id']}")
+        return cls
+
+    async def _run_slash_command(self, command: SlashCommand, ctx: "InteractionContext") -> Any:
+        """Overrideable method that executes slash commands, can be used to wrap callback execution"""
+        return await command(ctx, **ctx.kwargs)
+
+    @processors.Processor.define("raw_interaction_create")
+    async def _dispatch_interaction(self, event: RawGatewayEvent) -> None:
+        """
+        Identify and dispatch interaction of slash commands or components.
+
+        Args:
+            raw interaction event
+
+        """
+        interaction_data = event.data
+
+        if interaction_data["type"] in (
+            InteractionType.APPLICATION_COMMAND,
+            InteractionType.AUTOCOMPLETE,
+        ):
+            interaction_id = interaction_data["data"]["id"]
+            name = interaction_data["data"]["name"]
+
+            ctx = await self.get_context(interaction_data)
+            if ctx.command:
+                self.logger.debug(f"{ctx.command_id}::{ctx.command.name} should be called")
+
+                if ctx.command.auto_defer:
+                    auto_defer = ctx.command.auto_defer
+                elif ctx.command.extension and ctx.command.extension.auto_defer:
+                    auto_defer = ctx.command.extension.auto_defer
+                else:
+                    auto_defer = self.auto_defer
+
+                if auto_opt := getattr(ctx, "focussed_option", None):
+                    if autocomplete := ctx.command.autocomplete_callbacks.get(str(auto_opt.name)):
+                        callback = autocomplete
+                    elif autocomplete := self._global_autocompletes.get(str(auto_opt.name)):
+                        callback = autocomplete
+                    else:
+                        raise ValueError(f"Autocomplete callback for {str(auto_opt.name)} not found")
+
+                    await self.__dispatch_interaction(
+                        ctx=ctx,
+                        callback=callback(ctx),
+                        callback_kwargs=ctx.kwargs,
+                        error_callback=events.AutocompleteError,
+                        completion_callback=events.AutocompleteCompletion,
+                    )
+                else:
+                    await auto_defer(ctx)
+                    await self.__dispatch_interaction(
+                        ctx=ctx,
+                        callback=self._run_slash_command(ctx.command, ctx),
+                        callback_kwargs=ctx.kwargs,
+                        error_callback=events.CommandError,
+                        completion_callback=events.CommandCompletion,
+                    )
+            else:
+                self.logger.error(f"Unknown cmd_id received:: {interaction_id} ({name})")
+
+        elif interaction_data["type"] == InteractionType.MESSAGE_COMPONENT:
+            # Buttons, Selects, ContextMenu::Message
+            ctx = await self.get_context(interaction_data)
+            component_type = interaction_data["data"]["component_type"]
+
+            self.dispatch(events.Component(ctx=ctx))
+            if callback := self._component_callbacks.get(ctx.custom_id):
+                await self.__dispatch_interaction(
+                    ctx=ctx,
+                    callback=callback(ctx),
+                    error_callback=events.ComponentError,
+                    completion_callback=events.ComponentCompletion,
+                )
+
+            if component_type == ComponentType.BUTTON:
+                self.dispatch(events.ButtonPressed(ctx))
+
+            if component_type == ComponentType.STRING_SELECT:
+                self.dispatch(events.Select(ctx))
+
+        elif interaction_data["type"] == InteractionType.MODAL_RESPONSE:
+            ctx = await self.get_context(interaction_data)
+            self.dispatch(events.ModalCompletion(ctx=ctx))
+
+            if callback := self._modal_callbacks.get(ctx.custom_id):
+                await self.__dispatch_interaction(ctx=ctx, callback=callback(ctx), error_callback=events.ModalError)
+
+        else:
+            raise NotImplementedError(f"Unknown Interaction Received: {interaction_data['type']}")
+
+    # todo add typing once context is re-implemented
+    async def __dispatch_interaction(
+        self,
+        ctx,
+        callback: Coroutine,
+        error_callback: Type[BaseEvent],
+        completion_callback: Type[BaseEvent] | None = None,
+        callback_kwargs: dict | None = None,
+    ) -> None:
+        if callback_kwargs is None:
+            callback_kwargs = {}
+
+        try:
+            if self.pre_run_callback:
+                await self.pre_run_callback(ctx, **callback_kwargs)
+
+            # allow interactions to be responded by returning a string or an embed
+            response = await callback
+            if not getattr(ctx, "responded", True) and response:
+                if isinstance(response, Embed) or (
+                    isinstance(response, list) and all(isinstance(item, Embed) for item in response)
+                ):
+                    await ctx.send(embeds=response)
+                else:
+                    if not isinstance(response, str):
+                        self.logger.warning(
+                            "Command callback returned non-string value - casting to string and sending"
+                        )
+                    await ctx.send(str(response))
+
+            if self.post_run_callback:
+                _ = asyncio.create_task(self.post_run_callback(ctx, **callback_kwargs))
+        except Exception as e:
+            self.dispatch(error_callback(ctx=ctx, error=e))
+        finally:
+            if completion_callback:
+                self.dispatch(completion_callback(ctx=ctx))
+
+    @Listener.create("disconnect", is_default_listener=True)
+    async def _disconnect(self) -> None:
+        self._ready.clear()
+
+    def get_extensions(self, name: str) -> list[Extension]:
+        """
+        Get all ext with a name or extension name.
+
+        Args:
+            name: The name of the extension, or the name of it's extension
+
+        Returns:
+            List of Extensions
+        """
+        if name not in self.ext.keys():
+            return [ext for ext in self.ext.values() if ext.extension_name == name]
+
+        return [self.ext.get(name, None)]
+
+    def get_ext(self, name: str) -> Extension | None:
+        """
+        Get a extension with a name or extension name.
+
+        Args:
+            name: The name of the extension, or the name of it's extension
+
+        Returns:
+            A extension, if found
+        """
+        return ext[0] if (ext := self.get_extensions(name)) else None
+
+    def __load_module(self, module, module_name, **load_kwargs) -> None:
+        """Internal method that handles loading a module."""
+        try:
+            if setup := getattr(module, "setup", None):
+                setup(self, **load_kwargs)
+            else:
+                self.logger.debug("No setup function found in %s", module_name)
+
+                found = False
+                objects = {name: obj for name, obj in inspect.getmembers(module) if isinstance(obj, type)}
+                for obj_name, obj in objects.items():
+                    if Extension in obj.__bases__:
+                        self.logger.debug(f"Found extension class {obj_name} in {module_name}: Attempting to load")
+                        obj(self, **load_kwargs)
+                        found = True
+                if not found:
+                    raise ValueError(f"{module_name} contains no Extensions")
+
+        except ExtensionLoadException:
+            raise
+        except Exception as e:
+            sys.modules.pop(module_name, None)
+            raise ExtensionLoadException(f"Unexpected Error loading {module_name}") from e
+
+        else:
+            self.logger.debug(f"Loaded Extension: {module_name}")
+            self.__modules[module_name] = module
+
+            if self.sync_ext and self._ready.is_set():
+                try:
+                    asyncio.get_running_loop()
+                except RuntimeError:
+                    return
+                _ = asyncio.create_task(self.synchronise_interactions())
+
+    def load_extension(
+        self,
+        name: str,
+        package: str | None = None,
+        **load_kwargs: Any,
+    ) -> None:
+        """
+        Load an extension with given arguments.
+
+        Args:
+            name: The name of the extension.
+            package: The package the extension is in
+            **load_kwargs: The auto-filled mapping of the load keyword arguments
+        """
+        module_name = importlib.util.resolve_name(name, package)
+        if module_name in self.__modules:
+            raise Exception(f"{module_name} already loaded")
+
+        module = importlib.import_module(module_name, package)
+        self.__load_module(module, module_name, **load_kwargs)
+
+    def unload_extension(
+        self, name: str, package: str | None = None, force: bool = False, **unload_kwargs: Any
+    ) -> None:
+        """
+        Unload an extension with given arguments.
+
+        Args:
+            name: The name of the extension.
+            package: The package the extension is in
+            force: Whether to force unload the extension - for use in reversions
+            **unload_kwargs: The auto-filled mapping of the unload keyword arguments
+
+        """
+        name = importlib.util.resolve_name(name, package)
+        module = self.__modules.get(name)
+
+        if module is None and not force:
+            raise ExtensionNotFound(f"No extension called {name} is loaded")
+
+        with contextlib.suppress(AttributeError):
+            teardown = module.teardown
+            teardown(**unload_kwargs)
+
+        for ext in self.get_extensions(name):
+            ext.drop(**unload_kwargs)
+
+        sys.modules.pop(name, None)
+        self.__modules.pop(name, None)
+
+        if self.sync_ext and self._ready.is_set():
+            try:
+                asyncio.get_running_loop()
+            except RuntimeError:
+                return
+            _ = asyncio.create_task(self.synchronise_interactions())
+
+    def reload_extension(
+        self,
+        name: str,
+        package: str | None = None,
+        *,
+        load_kwargs: Any = None,
+        unload_kwargs: Any = None,
+    ) -> None:
+        """
+        Helper method to reload an extension. Simply unloads, then loads the extension with given arguments.
+
+        Args:
+            name: The name of the extension.
+            package: The package the extension is in
+            load_kwargs: The manually-filled mapping of the load keyword arguments
+            unload_kwargs: The manually-filled mapping of the unload keyword arguments
+
+        """
+        name = importlib.util.resolve_name(name, package)
+        module = self.__modules.get(name)
+
+        if module is None:
+            self.logger.warning("Attempted to reload extension thats not loaded. Loading extension instead")
+            return self.load_extension(name, package)
+
+        backup = module
+
+        try:
+            if not load_kwargs:
+                load_kwargs = {}
+            if not unload_kwargs:
+                unload_kwargs = {}
+
+            self.unload_extension(name, package, **unload_kwargs)
+            self.load_extension(name, package, **load_kwargs)
+        except Exception as e:
+            try:
+                self.logger.error(f"Error reloading extension {name}: {e} - attempting to revert to previous state")
+                try:
+                    self.unload_extension(name, package, force=True, **unload_kwargs)  # make sure no remnants are left
+                except Exception as t:
+                    self.logger.debug(f"Suppressing error unloading extension {name} during reload revert: {t}")
+
+                sys.modules[name] = backup
+                self.__load_module(backup, name, **load_kwargs)
+                self.logger.info(f"Reverted extension {name} to previous state ", exc_info=e)
+            except Exception as ex:
+                sys.modules.pop(name, None)
+                raise ex from e
+
+    async def fetch_guild(self, guild_id: "Snowflake_Type") -> Optional[Guild]:
+        """
+        Fetch a guild.
+
+        !!! note
+            This method is an alias for the cache which will either return a cached object, or query discord for the object
+            if its not already cached.
+
+        Args:
+            guild_id: The ID of the guild to get
+
+        Returns:
+            Guild Object if found, otherwise None
+
+        """
+        try:
+            return await self.cache.fetch_guild(guild_id)
+        except NotFound:
+            return None
+
+    def get_guild(self, guild_id: "Snowflake_Type") -> Optional[Guild]:
+        """
+        Get a guild.
+
+        !!! note
+            This method is an alias for the cache which will return a cached object.
+
+        Args:
+            guild_id: The ID of the guild to get
+
+        Returns:
+            Guild Object if found, otherwise None
+
+        """
+        return self.cache.get_guild(guild_id)
+
+    async def create_guild_from_template(
+        self,
+        template_code: Union["GuildTemplate", str],
+        name: str,
+        icon: Absent[UPLOADABLE_TYPE] = MISSING,
+    ) -> Optional[Guild]:
+        """
+        Creates a new guild based on a template.
+
+        !!! note
+            This endpoint can only be used by bots in less than 10 guilds.
+
+        Args:
+            template_code: The code of the template to use.
+            name: The name of the guild (2-100 characters)
+            icon: Location or File of icon to set
+
+        Returns:
+            The newly created guild object
+
+        """
+        if isinstance(template_code, GuildTemplate):
+            template_code = template_code.code
+
+        if icon:
+            icon = to_image_data(icon)
+        guild_data = await self.http.create_guild_from_guild_template(template_code, name, icon)
+        return Guild.from_dict(guild_data, self)
+
+    async def fetch_channel(self, channel_id: "Snowflake_Type") -> Optional["TYPE_ALL_CHANNEL"]:
+        """
+        Fetch a channel.
+
+        !!! note
+            This method is an alias for the cache which will either return a cached object, or query discord for the object
+            if its not already cached.
+
+        Args:
+            channel_id: The ID of the channel to get
+
+        Returns:
+            Channel Object if found, otherwise None
+
+        """
+        try:
+            return await self.cache.fetch_channel(channel_id)
+        except NotFound:
+            return None
+
+    def get_channel(self, channel_id: "Snowflake_Type") -> Optional["TYPE_ALL_CHANNEL"]:
+        """
+        Get a channel.
+
+        !!! note
+            This method is an alias for the cache which will return a cached object.
+
+        Args:
+            channel_id: The ID of the channel to get
+
+        Returns:
+            Channel Object if found, otherwise None
+
+        """
+        return self.cache.get_channel(channel_id)
+
+    async def fetch_user(self, user_id: "Snowflake_Type") -> Optional[User]:
+        """
+        Fetch a user.
+
+        !!! note
+            This method is an alias for the cache which will either return a cached object, or query discord for the object
+            if its not already cached.
+
+        Args:
+            user_id: The ID of the user to get
+
+        Returns:
+            User Object if found, otherwise None
+
+        """
+        try:
+            return await self.cache.fetch_user(user_id)
+        except NotFound:
+            return None
+
+    def get_user(self, user_id: "Snowflake_Type") -> Optional[User]:
+        """
+        Get a user.
+
+        !!! note
+            This method is an alias for the cache which will return a cached object.
+
+        Args:
+            user_id: The ID of the user to get
+
+        Returns:
+            User Object if found, otherwise None
+
+        """
+        return self.cache.get_user(user_id)
+
+    async def fetch_member(self, user_id: "Snowflake_Type", guild_id: "Snowflake_Type") -> Optional[Member]:
+        """
+        Fetch a member from a guild.
+
+        !!! note
+            This method is an alias for the cache which will either return a cached object, or query discord for the object
+            if its not already cached.
+
+        Args:
+            user_id: The ID of the member
+            guild_id: The ID of the guild to get the member from
+
+        Returns:
+            Member object if found, otherwise None
+
+        """
+        try:
+            return await self.cache.fetch_member(guild_id, user_id)
+        except NotFound:
+            return None
+
+    def get_member(self, user_id: "Snowflake_Type", guild_id: "Snowflake_Type") -> Optional[Member]:
+        """
+        Get a member from a guild.
+
+        !!! note
+            This method is an alias for the cache which will return a cached object.
+
+        Args:
+            user_id: The ID of the member
+            guild_id: The ID of the guild to get the member from
+
+        Returns:
+            Member object if found, otherwise None
+
+        """
+        return self.cache.get_member(guild_id, user_id)
+
+    async def fetch_scheduled_event(
+        self,
+        guild_id: "Snowflake_Type",
+        scheduled_event_id: "Snowflake_Type",
+        with_user_count: bool = False,
+    ) -> Optional["ScheduledEvent"]:
+        """
+        Fetch a scheduled event by id.
+
+        Args:
+            guild_id: The ID of the guild to get the scheduled event from
+            scheduled_event_id: The ID of the scheduled event to get
+            with_user_count: Whether to include the user count in the response
+
+        Returns:
+            The scheduled event if found, otherwise None
+
+        """
+        try:
+            scheduled_event_data = await self.http.get_scheduled_event(guild_id, scheduled_event_id, with_user_count)
+            return ScheduledEvent.from_dict(scheduled_event_data, self)
+        except NotFound:
+            return None
+
+    async def fetch_custom_emoji(self, emoji_id: "Snowflake_Type", guild_id: "Snowflake_Type") -> Optional[CustomEmoji]:
+        """
+        Fetch a custom emoji by id.
+
+        Args:
+            emoji_id: The id of the custom emoji.
+            guild_id: The id of the guild the emoji belongs to.
+
+        Returns:
+            The custom emoji if found, otherwise None.
+
+        """
+        try:
+            return await self.cache.fetch_emoji(guild_id, emoji_id)
+        except NotFound:
+            return None
+
+    def get_custom_emoji(
+        self, emoji_id: "Snowflake_Type", guild_id: Optional["Snowflake_Type"] = None
+    ) -> Optional[CustomEmoji]:
+        """
+        Get a custom emoji by id.
+
+        Args:
+            emoji_id: The id of the custom emoji.
+            guild_id: The id of the guild the emoji belongs to.
+
+        Returns:
+            The custom emoji if found, otherwise None.
+
+        """
+        emoji = self.cache.get_emoji(emoji_id)
+        if emoji and (not guild_id or emoji._guild_id == to_snowflake(guild_id)):
+            return emoji
+        return None
+
+    async def fetch_sticker(self, sticker_id: "Snowflake_Type") -> Optional[Sticker]:
+        """
+        Fetch a sticker by ID.
+
+        Args:
+            sticker_id: The ID of the sticker.
+
+        Returns:
+            A sticker object if found, otherwise None
+
+        """
+        try:
+            sticker_data = await self.http.get_sticker(sticker_id)
+            return Sticker.from_dict(sticker_data, self)
+        except NotFound:
+            return None
+
+    async def fetch_nitro_packs(self) -> Optional[List["StickerPack"]]:
+        """
+        List the sticker packs available to Nitro subscribers.
+
+        Returns:
+            A list of StickerPack objects if found, otherwise returns None
+
+        """
+        try:
+            packs_data = await self.http.list_nitro_sticker_packs()
+            return [StickerPack.from_dict(data, self) for data in packs_data]
+
+        except NotFound:
+            return None
+
+    async def fetch_voice_regions(self) -> List["VoiceRegion"]:
+        """
+        List the voice regions available on Discord.
+
+        Returns:
+            A list of voice regions.
+
+        """
+        regions_data = await self.http.list_voice_regions()
+        return VoiceRegion.from_list(regions_data)
+
+    async def connect_to_vc(
+        self,
+        guild_id: "Snowflake_Type",
+        channel_id: "Snowflake_Type",
+        muted: bool = False,
+        deafened: bool = False,
+    ) -> ActiveVoiceState:
+        """
+        Connect the bot to a voice channel.
+
+        Args:
+            guild_id: id of the guild the voice channel is in.
+            channel_id: id of the voice channel client wants to join.
+            muted: Whether the bot should be muted when connected.
+            deafened: Whether the bot should be deafened when connected.
+
+        Returns:
+            The new active voice state on successfully connection.
+
+        """
+        return await self._connection_state.voice_connect(guild_id, channel_id, muted, deafened)
+
+    def get_bot_voice_state(self, guild_id: "Snowflake_Type") -> Optional[ActiveVoiceState]:
+        """
+        Get the bot's voice state for a guild.
+
+        Args:
+            guild_id: The target guild's id.
+
+        Returns:
+            The bot's voice state for the guild if connected, otherwise None.
+
+        """
+        return self._connection_state.get_voice_state(guild_id)
+
+    async def change_presence(
+        self,
+        status: Optional[Union[str, Status]] = Status.ONLINE,
+        activity: Optional[Union[Activity, str]] = None,
+    ) -> None:
+        """
+        Change the bots presence.
+
+        Args:
+            status: The status for the bot to be. i.e. online, afk, etc.
+            activity: The activity for the bot to be displayed as doing.
+
+        !!! note
+            Bots may only be `playing` `streaming` `listening` `watching` or `competing`, other activity types are likely to fail.
+
+        """
+        await self._connection_state.change_presence(status, activity)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `discord-py-interactions-4.4.0/interactions/client/context.py` & `discord-py-interactions-5.0.0/interactions/models/internal/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,863 +1,892 @@
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
-
-__all__ = (
-    "_Context",
-    "CommandContext",
-    "ComponentContext",
-)
-
-
-@define()
-class _Context(ClientSerializerMixin):
-    """
-    The base class of "context" for dispatched event data
-    from the gateway. The premise of having this class is so
-    that the user-facing API is able to allow developers to
-    easily access information presented from any event in
-    a "contextualized" sense.
-    """
-
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
-
-        if self.user is None:
-            self.user = self.member.user if self.member else None
-
-        if self.member and not self.member.user and self.user:
-            self.member.user = self.user
-
-    @property
-    def deferred_ephemeral(self) -> bool:
-        """
-        .. versionadded:: 4.4.0
-
-        Returns whether the current interaction was deferred ephemerally.
-        """
-        return bool(
-            self.message.flags & MessageFlags.EPHEMERAL
-            and self.message.flags & MessageFlags.LOADING
-        )
-
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
-            return channel
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
-
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
-                )
-                self.message = Message(**res, _client=self._client)
-
-            self.responded = True
-
-            return self.message
-
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
-
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
-
-        else:
-            _components = []
-
-        _flags = MessageFlags.EPHEMERAL if ephemeral else MessageFlags(0)
-        if suppress_embeds:
-            _flags |= MessageFlags.SUPPRESS_EMBEDS
-
-        _attachments = [] if attachments is MISSING else [a._json for a in attachments]
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
-
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
-
-            payload["embeds"] = _embeds
-
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
-        payload["attachments"] = _files
-
-        _allowed_mentions: dict = (
-            {}
-            if allowed_mentions is MISSING
-            else allowed_mentions._json
-            if isinstance(allowed_mentions, AllowedMentions)
-            else allowed_mentions
-        )
-        _message_reference: dict = {} if message_reference is MISSING else message_reference._json
-
-        payload["allowed_mentions"] = _allowed_mentions
-        payload["message_reference"] = _message_reference
-
-        if self.message.components is not None or components is not MISSING:
-            if components is MISSING:
-                _components = _build_components(components=self.message.components)
-            elif not components:
-                _components = []
-            else:
-                _components = _build_components(components=components)
-
-            payload["components"] = _components
-
-        return payload, files
-
-    async def popup(self, modal: Modal) -> dict:
-        """
-        This "pops up" a modal to present information back to the
-        user.
-
-        :param Modal modal: The components you wish to show.
-        """
-
-        payload: dict = {
-            "type": InteractionCallbackType.MODAL.value,
-            "data": {
-                "title": modal.title,
-                "components": modal._json.get("components"),
-                "custom_id": modal.custom_id,
-            },
-        }
-
-        await self._client.create_interaction_response(
-            token=self.token,
-            application_id=int(self.id),
-            data=payload,
-        )
-        self.responded = True
-
-        return payload
-
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
-
-    async def delete(self) -> None:
-        """
-        This deletes the interaction response of a message sent by
-        the contextually derived information from this class.
-
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
-
-        self.message = None
-
-
-@define()
-class CommandContext(_Context):
-    """
-    A derivation of context
-    designed specifically for application command data.
-
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
-
-        The extension the command belongs to.
-    """
-
-    target: Optional[Union[Message, Member, User]] = field(default=None)
-
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
-
-            elif self.data.type == 3:
-                self.target = self.data.resolved.messages[target]
-
-            self.target._client = self._client
-
-    async def edit(
-        self, content: Optional[str] = MISSING, **kwargs
-    ) -> Message:  # sourcery skip: low-code-quality
-        payload, files = await super().edit(content, **kwargs)
-        msg = None
-
-        if self.deferred:
-            if (
-                hasattr(self.message, "id")
-                and self.message.id is not None
-                and self.message.flags != 64
-            ):
-                try:
-                    res = await self._client.edit_message(
-                        int(self.channel_id), int(self.message.id), payload=payload, files=files
-                    )
-                except LibraryException as e:
-                    if e.code in {10015, 10018}:
-                        log.warning(f"You can't edit hidden messages." f"({e.message}).")
-                    else:
-                        # if its not ephemeral or some other thing.
-                        raise e from e
-                else:
-                    self.message = msg = Message(**res, _client=self._client)
-            else:
-                try:
-                    res = await self._client.edit_interaction_response(
-                        token=self.token,
-                        application_id=str(self.application_id),
-                        data=payload,
-                        files=files,
-                        message_id=self.message.id
-                        if self.message and self.message.flags != 64
-                        else "@original",
-                    )
-                except LibraryException as e:
-                    if e.code in {10015, 10018}:
-                        log.warning(f"You can't edit hidden messages." f"({e.message}).")
-                    else:
-                        # if its not ephemeral or some other thing.
-                        raise e from e
-                else:
-                    self.message = msg = Message(**res, _client=self._client)
-        else:
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
-
-        return msg or Message(**payload, _client=self._client)
-
-    async def send(self, content: Optional[str] = MISSING, **kwargs) -> Message:
-        payload, files = await super().send(content, **kwargs)
-
-        if not self.deferred:
-            self.callback = InteractionCallbackType.CHANNEL_MESSAGE_WITH_SOURCE
-
-        _payload: dict = {"type": self.callback.value, "data": payload}
-
-        msg = None
-        if self.responded:
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
-
-            self.responded = True
-
-        return msg or Message(
-            **payload,
-            _client=self._client,
-            author={"_client": self._client, "id": None, "username": None, "discriminator": None},
-        )
-
-    async def populate(self, choices: Union[Choice, List[Choice]]) -> List[Choice]:
-        """
-        This "populates" the list of choices that the client-end
-        user will be able to select from in the autocomplete field.
-
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
-
-        await self._client.create_interaction_response(
-            token=self.token,
-            application_id=int(self.id),
-            data={
-                "type": InteractionCallbackType.APPLICATION_COMMAND_AUTOCOMPLETE_RESULT.value,
-                "data": {"choices": _choices},
-            },
-        )
-
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
-
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
-
-            with suppress(LibraryException):
-                res = await self._client.get_original_interaction_response(
-                    self.token, str(self.application_id)
-                )
-
-                self.message = msg = Message(**res, _client=self._client)
-
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
-
-    async def send(self, content: Optional[str] = MISSING, **kwargs) -> Message:
-        payload, files = await super().send(content, **kwargs)
-
-        if not self.deferred:
-            self.callback = InteractionCallbackType.CHANNEL_MESSAGE_WITH_SOURCE
-
-        _payload: dict = {"type": self.callback.value, "data": payload}
-
-        msg = None
-        if self.responded:
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
-
-            self.responded = True
-
-        return msg if msg is not None else Message(**payload, _client=self._client)
-
-    async def disable_all_components(
-        self, respond_to_interaction: Optional[bool] = True, **other_kwargs: Optional[dict]
-    ) -> Message:
-        r"""
-        .. versionadded:: 4.3.2
-
-        Disables all components of the message.
-
-        :param Optional[bool] respond_to_interaction: Whether the components should be disabled in an interaction response, default True
-        :param Optional[dict] \**other_kwargs: Additional keyword-arguments to pass to the edit method. This only works when this method is used as interaction response and takes the same arguments as :func:`ComponentContext.edit()`
-
-        :return: The modified Message
-        :rtype: Message
-        """
-
-        if not respond_to_interaction:
-            return await self.message.disable_all_components()
-
-        for components in self.message.components:
-            for component in components.components:
-                component.disabled = True
-
-        if other_kwargs.get("components"):
-            raise LibraryException(
-                12, "You must not specify the `components` argument in this method."
-            )
-
-        other_kwargs["components"] = self.message.components
-        return await self.edit(**other_kwargs)
-
-    @property
-    def custom_id(self) -> Optional[str]:
-        """
-        The custom ID of the interacted component.
-
-        :rtype: Optional[str]
-        """
-        return self.data.custom_id
-
-    @property
-    def label(self) -> Optional[str]:
-        """
-        The label of the interacted button.
-
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
-
-    @property
-    def component(self) -> Optional[Union[Button, SelectMenu]]:
-        """
-        .. versionadded:: 4.4.0
-
-        The component that you interacted.
-
-        :rtype: Optional[Union[Button, SelectMenu]]
-        """
-        if self.message is None or self.message.components is None:
-            return
-
-        for action_row in self.message.components:
-            for component in action_row.components:
-                if component.custom_id == self.custom_id:
-                    return component
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
+
+__all__ = (
+    "AutocompleteContext",
+    "BaseContext",
+    "BaseInteractionContext",
+    "ComponentContext",
+    "ContextMenuContext",
+    "InteractionContext",
+    "ModalContext",
+    "Resolved",
+    "SlashContext",
+)
+
+
+if typing.TYPE_CHECKING:
+    import interactions
+
+
+class Resolved:
+    """
+    A class representing the resolved data from an interaction.
+
+    Attributes:
+        channels: A dictionary of channels resolved from the interaction.
+        members: A dictionary of members resolved from the interaction.
+        users: A dictionary of users resolved from the interaction.
+        roles: A dictionary of roles resolved from the interaction.
+        messages: A dictionary of messages resolved from the interaction.
+        attachments: A dictionary of attachments resolved from the interaction.
+    """
+
+    def __init__(self) -> None:
+        self.channels: dict[Snowflake, "interactions.TYPE_MESSAGEABLE_CHANNEL"] = {}
+        self.members: dict[Snowflake, "interactions.Member"] = {}
+        self.users: dict[Snowflake, "interactions.User"] = {}
+        self.roles: dict[Snowflake, "interactions.Role"] = {}
+        self.messages: dict[Snowflake, "interactions.Message"] = {}
+        self.attachments: dict[Snowflake, "interactions.Attachment"] = {}
+
+    def __bool__(self) -> bool:
+        """Returns whether any resolved data is present."""
+        return (
+            bool(self.channels)
+            or bool(self.members)
+            or bool(self.users)
+            or bool(self.roles)
+            or bool(self.messages)
+            or bool(self.attachments)
+        )
+
+    def get(self, snowflake: Snowflake | str, default: typing.Any = None) -> typing.Any:
+        snowflake = Snowflake(snowflake)
+        """Returns the value of the given snowflake."""
+        if channel := self.channels.get(snowflake):
+            return channel
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
+                )
+
+        if users := data.get("users"):
+            for key, _user in users.items():
+                instance.users[Snowflake(key)] = client.cache.place_user_data(_user)
+
+        if roles := data.get("roles"):
+            for key, _role in roles.items():
+                instance.roles[Snowflake(key)] = client.cache.get_role(Snowflake(key))
+
+        if messages := data.get("messages"):
+            for key, _msg in messages.items():
+                instance.messages[Snowflake(key)] = client.cache.place_message_data(_msg)
+
+        if attachments := data.get("attachments"):
+            for key, _attach in attachments.items():
+                instance.attachments[Snowflake(key)] = Attachment.from_dict(_attach, client)
+
+        return instance
+
+
+class BaseContext(metaclass=abc.ABCMeta):
+    """
+    Base context class for all contexts.
+
+    Define your own context class by inheriting from this class. For compatibility with the library, you must define a `from_dict` classmethod that takes a dict and returns an instance of your context class.
+
+    """
+
+    client: "interactions.Client"
+    """The client that created this context."""
+
+    command: BaseCommand
+    """The command this context invokes."""
+
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
+
+    @property
+    def guild(self) -> typing.Optional["interactions.Guild"]:
+        """The guild this context was invoked in."""
+        return self.client.cache.get_guild(self.guild_id)
+
+    @property
+    def user(self) -> "interactions.User":
+        """The user that invoked this context."""
+        return self.client.cache.get_user(self.author_id)
+
+    @property
+    def member(self) -> typing.Optional["interactions.Member"]:
+        """The member object that invoked this context."""
+        return self.client.cache.get_member(self.guild_id, self.author_id)
+
+    @property
+    def author(self) -> "interactions.Member | interactions.User":
+        """The member or user that invoked this context."""
+        return self.member or self.user
+
+    @property
+    def channel(self) -> "interactions.TYPE_MESSAGEABLE_CHANNEL":
+        """The channel this context was invoked in."""
+        if self.guild_id:
+            return self.client.cache.get_channel(self.channel_id)
+        return self.client.cache.get_dm_channel(self.author_id)
+
+    @property
+    def message(self) -> typing.Optional["interactions.Message"]:
+        """The message that invoked this context, if any."""
+        return self.client.cache.get_message(self.channel_id, self.message_id)
+
+    @property
+    def voice_state(self) -> typing.Optional["interactions.VoiceState"]:
+        """The current voice state of the bot in the guild this context was invoked in, if any."""
+        return self.client.cache.get_bot_voice_state(self.guild_id)
+
+    @property
+    def bot(self) -> "interactions.Client":
+        return self.client
+
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
+
+        instance.process_options(payload)
+
+        return instance
+
+    @property
+    def command(self) -> InteractionCommand:
+        return self.client._interaction_lookup[self._command_name]
+
+    @property
+    def expires_at(self) -> typing.Optional[datetime.datetime]:
+        """The time at which the interaction expires."""
+        if self.responded:
+            return self.id.created_at + datetime.timedelta(minutes=15)
+        return self.id.created_at + datetime.timedelta(seconds=3)
+
+    @property
+    def expired(self) -> bool:
+        """Whether the interaction has expired."""
+        return datetime.datetime.utcnow() > self.expires_at
+
+    @property
+    def invoke_target(self) -> str:
+        """The invoke target of the interaction."""
+        return self._command_name
+
+    @property
+    def deferred_ephemeral(self) -> bool:
+        """Whether the interaction has been deferred ephemerally."""
+        return self.deferred and self.ephemeral
+
+    def option_processing_hook(self, option: dict) -> typing.Any:
+        """
+        Hook for extending options processing.
+
+        This is called for each option, before the library processes it. If this returns a value, the library will not process the option further.
+
+        Args:
+            option: The option to process.
+
+        Returns:
+            The processed option.
+
+        """
+        return option
+
+    def process_options(self, data: discord_typings.InteractionCallbackData) -> None:
+        if data["type"] not in (InteractionType.APPLICATION_COMMAND, InteractionType.AUTOCOMPLETE):
+            self.args = []
+            self.kwargs = {}
+            return
+
+        def gather_options(_options: list[dict[str, typing.Any]]) -> dict[str, typing.Any]:
+            """Recursively gather options from an option list."""
+            kwargs = {}
+            for option in _options:
+                if hook_result := self.option_processing_hook(option):
+                    kwargs[option["name"]] = hook_result
+
+                if option["type"] in (OptionType.SUB_COMMAND, OptionType.SUB_COMMAND_GROUP):
+                    self._command_name = f"{self._command_name} {option['name']}"
+                    return gather_options(option["options"])
+
+                value = option.get("value")
+
+                if option["type"] in OptionType.resolvable_types():
+                    value = self.resolved.get(value, value)
+
+                kwargs[option["name"]] = value
+            return kwargs
+
+        if options := data["data"].get("options"):
+            self.kwargs = gather_options(options)  # type: ignore
+        else:
+            self.kwargs = {}
+        self.args = list(self.kwargs.values())
+
+
+class InteractionContext(BaseInteractionContext, SendMixin):
+    async def defer(self, *, ephemeral: bool = False) -> None:
+        """
+        Defer the interaction.
+
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
+
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
+        if self.responded:
+            message_data = await self.client.http.post_followup(
+                message_payload, self.client.app.id, self.token, files=files
+            )
+        else:
+            if isinstance(message_payload, FormData) and not self.deferred:
+                await self.defer(ephemeral=self.ephemeral)
+            if self.deferred:
+                message_data = await self.client.http.edit_interaction_message(
+                    message_payload, self.client.app.id, self.token, files=files
+                )
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
+
+        self.responded = True
+        return message_data
+
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
+        )
+
+    respond = send
+
+    async def delete(self, message: "Snowflake_Type") -> None:
+        """
+        Delete a message sent in response to this interaction.
+
+        Args:
+            message: The message to delete
+        """
+        await self.client.http.delete_interaction_message(self.client.app.id, self.token, to_snowflake(message))
+
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
+        )
+
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
+
+
+class SlashContext(InteractionContext, ModalMixin):
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        return super().from_dict(client, payload)
+
+
+class ContextMenuContext(InteractionContext, ModalMixin):
+    target_id: Snowflake
+    """The id of the target of the context menu."""
+    editing_origin: bool
+    """Whether you have deferred the interaction and are editing the original response."""
+    target_type: None | CommandType
+    """The type of the target of the context menu."""
+
+    def __init__(self, client: "interactions.Client") -> None:
+        super().__init__(client)
+        self.editing_origin = False
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        instance = super().from_dict(client, payload)
+        instance.target_id = Snowflake(payload["data"]["target_id"])
+        instance.target_type = CommandType(payload["data"]["type"])
+        return instance
+
+    async def defer(self, *, ephemeral: bool = False, edit_origin: bool = False) -> None:
+        """
+        Defer the interaction.
+
+        Args:
+            ephemeral: Whether the interaction response should be ephemeral.
+            edit_origin: Whether to edit the original message instead of sending a new one.
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
+
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
+
+    @property
+    def target(self) -> None | Message | User | Member:
+        """
+        The target of the context menu.
+
+        Returns:
+            The target of the context menu.
+        """
+        return self.resolved.get(self.target_id)
+
+
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
+
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
+        """
+        if self.deferred:
+            raise AlreadyDeferred("Interaction has already been responded to.")
+        if self.responded:
+            raise AlreadyResponded("Interaction has already been responded to.")
+
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
+
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
+
+            message_data = await self.client.http.edit_interaction_message(
+                message_payload, self.client.app.id, self.token, files=files or file
+            )
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
+
+        payload = {
+            "type": CallbackType.DEFERRED_UPDATE_MESSAGE
+            if edit_origin
+            else CallbackType.DEFERRED_CHANNEL_MESSAGE_WITH_SOURCE
+        }
+        if ephemeral:
+            payload["data"] = {"flags": MessageFlags.EPHEMERAL}
+
+        if edit_origin:
+            self.edit_origin = True
+
+        await self.client.http.post_initial_response(payload, self.id, self.token)
+        self.deferred = True
+        self.ephemeral = ephemeral
+
+
+class AutocompleteContext(BaseInteractionContext):
+    focussed_option: SlashCommandOption  # todo: option parsing
+    """The option the user is currently filling in."""
+
+    @classmethod
+    def from_dict(cls, client: "interactions.Client", payload: dict) -> Self:
+        return super().from_dict(client, payload)
+
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
+
+            processed_choices.append({"name": name, "value": type_cast(value) if type_cast else value})
+
+        payload = {"type": CallbackType.AUTOCOMPLETE_RESULT, "data": {"choices": processed_choices}}
+        await self.client.http.post_initial_response(payload, self.id, self.token)
```

### Comparing `discord-py-interactions-4.4.0/interactions/utils/abc/base_iterators.py` & `discord-py-interactions-5.0.0/interactions/models/misc/iterator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,97 @@
-from abc import ABC, ABCMeta, abstractmethod
-from math import inf
-from typing import TYPE_CHECKING, Awaitable, Callable, List, Optional, TypeVar, Union
-
-from ..missing import MISSING
-
-_T = TypeVar("_T")
-_O = TypeVar("_O")
-
-__all__ = ("BaseAsyncIterator", "BaseIterator", "DiscordPaginationIterator")
-
-if TYPE_CHECKING:
-    from ...api.http.client import HTTPClient
-    from ...api.models.misc import Snowflake
-
-
-class BaseAsyncIterator(ABC):
-    """
-    .. versionadded:: 4.3.2
-
-    A base class for async iterators.
-    """
-
-    @abstractmethod
-    def __init__(self):
-        """Initialise the iterator"""
-        raise NotImplementedError
-
-    def __aiter__(self):
-        return self
-
-    async def flatten(self):
-        """
-        Returns all items of the iterator as list
-        """
-        return [item async for item in self]
-
-    @abstractmethod
-    async def __anext__(self) -> _O:
-        """Return the next object"""
-        raise NotImplementedError
-
-
-class DiscordPaginationIterator(BaseAsyncIterator, metaclass=ABCMeta):
-    """
-    .. versionadded:: 4.3.2
-
-    A base class for Discord Pagination Iterators.
-    """
-
-    def __init__(
-        self,
-        obj: Union[int, str, "Snowflake", _T] = None,
-        _client: Optional["HTTPClient"] = None,
-        maximum: Optional[int] = inf,
-        start_at: Optional[Union[int, str, "Snowflake", _O]] = MISSING,
-        check: Optional[Callable[[_O], Union[bool, Awaitable[bool]]]] = None,
-    ):
-        """
-        Create a Discord Pagination iterator. All attributes are optional but may be useful for getting Discord objects.
-        Check usages in the :class:`.AsyncMembersIterator` and :class:`.AsyncHistoryIterator` or
-        :meth:`.Guild.get_members` and :meth:`.Channel.history`
-        for more information about the arguments.
-
-        :param Union[int, str, "Snowflake", _T] obj:
-        :param Optional["HTTPClient"] _client:
-        :param Optional[int] maximum:
-        :param Optional[Union[int, str, "Snowflake", _O]] start_at:
-        :param Optional[Callable[[_O], Union[bool, Awaitable[bool]]]] check:
-        """
-
-        self.object_id = (int(obj.id) if hasattr(obj, "id") else int(obj)) if obj else None
-
-        self.maximum = maximum
-        self.check = check
-        self._client = _client
-        self.object_count: int = 0
-        self.start_at = (
-            None
-            if start_at is MISSING
-            else int(start_at.id)
-            if hasattr(start_at, "id")
-            else int(start_at)
-        )
-
-        self.objects: Optional[List[_O]] = None
-
-
-class BaseIterator(ABC):
-    """
-    .. versionadded:: 4.3.2
-
-    A base class for iterators.
-    """
-
-    @abstractmethod
-    def __init__(self):
-        """Initialise the iterator"""
-        raise NotImplementedError
-
-    def __iter__(self):
-        return self
-
-    def flatten(self):
-        """
-        Returns all items of the iterator as list
-        """
-        return [item for item in self]
-
-    @abstractmethod
-    def __next__(self) -> _O:
-        """Return the next object"""
-        raise NotImplementedError
+import asyncio
+from abc import ABC, abstractmethod
+from asyncio import QueueEmpty
+from collections.abc import AsyncIterator as _AsyncIterator
+from typing import List, Any
+
+from interactions.client.const import MISSING, Absent
+from interactions.models.discord import snowflake
+
+__all__ = ("AsyncIterator",)
+
+
+class AsyncIterator(_AsyncIterator, ABC):
+    def __init__(self, limit: int = 50) -> None:
+        self._queue: asyncio.Queue = asyncio.Queue()
+        """The queue of items in the iterator"""
+
+        self._limit: int = limit or MISSING
+        """the limit of items to retrieve"""
+
+        self.last: Absent[Any] = MISSING
+        """The last item retrieved"""
+
+        self._retrieved_objects: List = []
+        """All items this iterator has retrieved"""
+
+    @property
+    def _continue(self) -> bool:
+        """Whether iteration should continue. Returns False if the limit has been reached."""
+        return len(self._retrieved_objects) < self._limit if self._limit else True
+
+    @property
+    def get_limit(self) -> int:
+        """Get how the maximum number of items that should be retrieved."""
+        return min(self._limit - len(self._retrieved_objects), 100) if self._limit else 100
+
+    @property
+    def total_retrieved(self) -> int:
+        """Get the total number of objects this iterator has retrieved."""
+        return len(self._retrieved_objects)
+
+    async def add_object(self, obj) -> None:
+        """Add an object to iterator's queue."""
+        return await self._queue.put(obj)
+
+    @abstractmethod
+    async def fetch(self) -> list:
+        """
+        Fetch additional objects.
+
+        Your implementation of this method *must* return a list of objects.
+        If no more objects are available, raise QueueEmpty
+
+        Returns:
+            List of objects
+
+        Raises:
+            QueueEmpty:  when no more objects are available.
+
+        """
+        ...
+
+    async def _get_items(self) -> None:
+        if self._continue:
+            data = await self.fetch()
+            [await self.add_object(obj) for obj in data]
+        else:
+            raise QueueEmpty
+
+    async def __anext__(self) -> Any:
+        try:
+            if self._queue.empty():
+                await self._get_items()
+            self.last = self._queue.get_nowait()
+
+            # add the message to the already retrieved objects, so that the search function works when calling it multiple times
+            self._retrieved_objects.append(self.last)
+
+            return self.last
+        except QueueEmpty as e:
+            raise StopAsyncIteration from e
+
+    async def flatten(self) -> List:
+        """Flatten this iterator into a list of objects."""
+        return [elem async for elem in self]
+
+    async def search(self, target_id: "snowflake.Snowflake_Type") -> bool:
+        """Search the iterator for an object with the given ID."""
+        target_id = snowflake.to_snowflake(target_id)
+
+        if target_id in [o.id for o in self._retrieved_objects]:
+            return True
+
+        async for o in self:
+            if o.id == target_id:
+                return True
+        return False
```

