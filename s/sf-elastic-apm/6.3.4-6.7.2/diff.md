# Comparing `tmp/sf-elastic-apm-6.3.4.tar.gz` & `tmp/sf-elastic-apm-6.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sf-elastic-apm-6.3.4.tar", last modified: Wed Sep  1 11:32:00 2021, max compression
+gzip compressed data, was "sf-elastic-apm-6.7.2.tar", last modified: Tue Jan 11 07:38:26 2022, max compression
```

## Comparing `sf-elastic-apm-6.3.4.tar` & `sf-elastic-apm-6.7.2.tar`

### file list

```diff
@@ -1,174 +1,190 @@
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.792242 sf-elastic-apm-6.3.4/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1587 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/LICENSE
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)      110 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/MANIFEST.in
--rw-rw-r--   0 pradeep   (1000) pradeep   (1000)     3003 2021-09-01 11:32:00.792242 sf-elastic-apm-6.3.4/PKG-INFO
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1643 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/README.rst
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.764242 sf-elastic-apm-6.3.4/elasticapm/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2692 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    25785 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/base.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.764242 sf-elastic-apm-6.3.4/elasticapm/conf/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    31719 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/conf/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3565 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/conf/constants.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.764242 sf-elastic-apm-6.3.4/elasticapm/context/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2631 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/context/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1901 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/context/base.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2529 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/context/contextvars.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2434 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/context/threadlocal.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.764242 sf-elastic-apm-6.3.4/elasticapm/contrib/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2338 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4968 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/middleware.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2711 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/utils.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/asyncio/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/asyncio/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4164 2021-09-01 11:29:44.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/asyncio/traces.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/celery/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4024 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/celery/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/django/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1801 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     7943 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/apps.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/django/celery/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1588 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/celery/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1862 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/celery/models.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    12519 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/client.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2244 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/context_processors.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3410 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/handlers.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/commands/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1519 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/commands/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    13196 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/commands/elasticapm.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/django/middleware/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     9007 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/middleware/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2302 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/middleware/wsgi.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3925 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/django/utils.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/flask/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     8570 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/flask/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3683 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/flask/utils.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.768242 sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1673 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5900 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/span.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6263 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/tracer.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1838 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/paste.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/pylons/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2208 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/pylons/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/rq/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2402 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/rq/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/starlette/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    10279 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/starlette/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4912 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/starlette/utils.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/tornado/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3097 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/tornado/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3473 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/tornado/utils.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/twisted/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2462 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/twisted/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/contrib/zerorpc/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3902 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/contrib/zerorpc/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     8323 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/events.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/handlers/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1588 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/handlers/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4340 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/handlers/logbook.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    10842 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/handlers/logging.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2658 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/handlers/structlog.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.772242 sf-elastic-apm-6.3.4/elasticapm/instrumentation/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2123 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/control.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.780242 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/__init__.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.780242 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4615 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3054 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiomysql.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3201 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiopg.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4228 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aioredis.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3340 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/asyncpg.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1852 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/base.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3532 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/elasticsearch.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6708 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/httpcore.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2927 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/httpx.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2132 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/sleep.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    11103 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/base.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     8939 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/botocore.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3899 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/cassandra.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     9948 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/dbapi2.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.780242 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/django/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/django/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2926 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/django/template.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5303 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/elasticsearch.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4455 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/graphql.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6062 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httpcore.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5528 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httplib2.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2853 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httpx.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2123 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/jinja2.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2597 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/mysql.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2569 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/mysql_connector.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5917 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/psycopg2.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3572 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pylibmc.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4195 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymemcache.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6008 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymongo.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2967 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymssql.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2239 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymysql.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2224 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pyodbc.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3082 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/python_memcached.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4371 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/redis.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2969 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/requests.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3450 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/sqlite.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5909 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/tornado.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5436 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/urllib.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6359 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/urllib3.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2105 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/zlib.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6147 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/instrumentation/register.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.780242 sf-elastic-apm-6.3.4/elasticapm/metrics/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    18604 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/base_metrics.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.784242 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1591 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1752 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/breakdown.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1870 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    11817 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu_linux.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2902 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu_psutil.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5449 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/prometheus.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1755 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/metrics/sets/transactions.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2944 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/middleware.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    11237 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/processors.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    31535 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/traces.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.784242 sf-elastic-apm-6.3.4/elasticapm/transport/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1615 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    15481 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/base.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1840 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/exceptions.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     9764 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/http.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4009 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/http_base.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1916 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/transport/http_urllib3.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.788242 sf-elastic-apm-6.3.4/elasticapm/utils/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     6518 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4432 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/cgroup.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     7562 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/cloud.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5667 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/compat.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2641 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/deprecation.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     9931 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/disttracing.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     9554 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/encoding.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2520 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/json_encoder.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2038 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/logging.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     2348 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/module_import.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    13373 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/stacks.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4480 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/threading.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.788242 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)      699 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/__init__.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    81870 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/_wrappers.c
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     4059 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/arguments.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    20127 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/decorators.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     7726 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/importer.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)    32389 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/wrappers.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5031 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/utils/wsgi.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     1658 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/elasticapm/version.py
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)      243 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/pyproject.toml
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3543 2021-09-01 11:32:00.792242 sf-elastic-apm-6.3.4/setup.cfg
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5666 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/setup.py
-drwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        0 2021-09-01 11:32:00.792242 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     3003 2021-09-01 11:32:00.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/PKG-INFO
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)     5405 2021-09-01 11:32:00.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/SOURCES.txt
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        1 2021-09-01 11:32:00.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/dependency_links.txt
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)        1 2021-09-01 11:29:45.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/not-zip-safe
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)      128 2021-09-01 11:32:00.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/requires.txt
--rwxrwxr-x   0 pradeep   (1000) pradeep   (1000)       11 2021-09-01 11:32:00.000000 sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.706834 sf-elastic-apm-6.7.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1587 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      110 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     3076 2022-01-11 07:38:26.706834 sf-elastic-apm-6.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1643 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/
+-rw-r--r--   0 runner    (1001) docker     (116)     2767 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27194 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/conf/
+-rw-r--r--   0 runner    (1001) docker     (116)    32131 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3564 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/conf/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/context/
+-rw-r--r--   0 runner    (1001) docker     (116)     2631 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1901 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2529 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/context/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2434 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/context/threadlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (116)     2346 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5955 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2682 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4164 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/asyncio/traces.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/celery/
+-rw-r--r--   0 runner    (1001) docker     (116)     4024 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/celery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7943 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/django/celery/
+-rw-r--r--   0 runner    (1001) docker     (116)     1588 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1862 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/celery/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11920 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2244 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3410 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.682834 sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)     1519 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13196 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/commands/elasticapm.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/django/middleware/
+-rw-r--r--   0 runner    (1001) docker     (116)     9007 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2302 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/middleware/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4454 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/flask/
+-rw-r--r--   0 runner    (1001) docker     (116)     8570 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3651 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/flask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/
+-rw-r--r--   0 runner    (1001) docker     (116)     1673 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5900 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/span.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6263 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1838 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/paste.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/pylons/
+-rw-r--r--   0 runner    (1001) docker     (116)     2208 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/pylons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/rq/
+-rw-r--r--   0 runner    (1001) docker     (116)     2402 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/rq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/sanic/
+-rw-r--r--   0 runner    (1001) docker     (116)    15806 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4282 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/sanic/patch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2745 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/sanic/sanic_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5829 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/sanic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/serverless/
+-rw-r--r--   0 runner    (1001) docker     (116)     1983 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17663 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/serverless/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/starlette/
+-rw-r--r--   0 runner    (1001) docker     (116)    10279 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4876 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/starlette/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/tornado/
+-rw-r--r--   0 runner    (1001) docker     (116)     3097 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3431 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/tornado/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/twisted/
+-rw-r--r--   0 runner    (1001) docker     (116)     2462 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/twisted/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.686834 sf-elastic-apm-6.7.2/elasticapm/contrib/zerorpc/
+-rw-r--r--   0 runner    (1001) docker     (116)     3902 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/contrib/zerorpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8323 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/events.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.690834 sf-elastic-apm-6.7.2/elasticapm/handlers/
+-rw-r--r--   0 runner    (1001) docker     (116)     1588 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4340 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/handlers/logbook.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10572 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/handlers/logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2584 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/handlers/structlog.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.690834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2123 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/control.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.694834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.694834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4521 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3047 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3201 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiopg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4218 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aioredis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3775 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1852 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3532 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2132 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18252 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/azure.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11103 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8939 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3814 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9977 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/dbapi2.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.694834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/django/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2926 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/django/template.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5210 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4455 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5517 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httplib2.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.694834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.698834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5052 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/httpcore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2835 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.698834 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/sync/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4606 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/sync/httpcore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2761 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/sync/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3701 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2123 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2520 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2492 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5950 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3484 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4107 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymemcache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5926 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2890 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2239 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymysql.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2224 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3171 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/python_memcached.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4393 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/redis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2875 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/requests.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3450 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5909 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5425 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6348 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2105 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/zlib.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6247 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/instrumentation/register.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.698834 sf-elastic-apm-6.7.2/elasticapm/metrics/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18604 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/base_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.698834 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/
+-rw-r--r--   0 runner    (1001) docker     (116)     1591 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1752 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1870 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11817 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu_linux.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2902 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu_psutil.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5454 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/metrics/sets/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2944 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11237 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/processors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41122 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/traces.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.698834 sf-elastic-apm-6.7.2/elasticapm/transport/
+-rw-r--r--   0 runner    (1001) docker     (116)     1615 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16562 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1840 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10186 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/http.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4009 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/http_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1916 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/transport/http_urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.702834 sf-elastic-apm-6.7.2/elasticapm/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)     7132 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4432 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7562 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5667 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2641 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9931 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/disttracing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9554 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2520 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2038 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2348 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/module_import.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13373 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/stacks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4480 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3760 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.702834 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (116)      699 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    81870 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (116)     4059 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20127 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7726 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32389 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5031 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/utils/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1658 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/elasticapm/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     3639 2022-01-11 07:38:26.706834 sf-elastic-apm-6.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     5666 2022-01-11 07:38:18.000000 sf-elastic-apm-6.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-01-11 07:38:26.706834 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3076 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5913 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      143 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2022-01-11 07:38:26.000000 sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/top_level.txt
```

### Comparing `sf-elastic-apm-6.3.4/LICENSE` & `sf-elastic-apm-6.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/PKG-INFO` & `sf-elastic-apm-6.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-elastic-apm
-Version: 6.3.4
+Version: 6.7.2
 Summary: The official Python module for Elastic APM
 Home-page: https://github.com/snappyflow/sftrace-python-agent
 Author: Elastic, Inc
 License: BSD
 Project-URL: Documentation, https://www.elastic.co/guide/en/apm/agent/python/current/index.html
 Project-URL: Release notes, https://www.elastic.co/guide/en/apm/agent/python/current/release-notes.html
 Project-URL: Source, https://github.com/elastic/apm-agent-python
@@ -15,23 +15,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: <4,>=3.6
 Provides-Extra: flask
 Provides-Extra: aiohttp
 Provides-Extra: tornado
 Provides-Extra: starlette
 Provides-Extra: opentracing
+Provides-Extra: sanic
 License-File: LICENSE
 
 elastic-apm -- Elastic APM agent for Python
 ===========================================
 
 .. image:: https://apm-ci.elastic.co/buildStatus/icon?job=apm-agent-python%2Fapm-agent-python-mbp%2Fmaster
     :target: https://apm-ci.elastic.co/job/apm-agent-python/job/apm-agent-python-mbp/
```

### Comparing `sf-elastic-apm-6.3.4/README.rst` & `sf-elastic-apm-6.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 import sys
 
 from elasticapm.base import Client, get_client  # noqa: F401
 from elasticapm.conf import setup_logging  # noqa: F401
+from elasticapm.contrib.serverless import capture_serverless  # noqa: F401
 from elasticapm.instrumentation.control import instrument, uninstrument  # noqa: F401
 from elasticapm.traces import (  # noqa: F401
     capture_span,
     get_span_id,
     get_trace_id,
     get_trace_parent_header,
     get_transaction_id,
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/base.py` & `sf-elastic-apm-6.7.2/elasticapm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,21 @@
 from __future__ import absolute_import
 
 import inspect
 import itertools
 import logging
 import os
 import platform
+import re
 import sys
 import threading
 import time
 import warnings
 from copy import deepcopy
+from typing import Optional, Tuple
 
 import elasticapm
 from elasticapm.conf import Config, VersionedConfig, constants
 from elasticapm.conf.constants import ERROR
 from elasticapm.metrics.base_metrics import MetricsRegistry
 from elasticapm.traces import Tracer, execution_context
 from elasticapm.utils import cgroup, cloud, compat, is_master_process, stacks, varmap
@@ -130,30 +132,30 @@
 
                 new_factory = elastic_logging.log_record_factory(record_factory)
                 logging.setLogRecordFactory(new_factory)
 
         headers = {
             "Content-Type": "application/x-ndjson",
             "Content-Encoding": "gzip",
-            "User-Agent": "elasticapm-python/%s" % elasticapm.VERSION,
+            "User-Agent": self.get_user_agent(),
         }
 
         transport_kwargs = {
             "headers": headers,
             "verify_server_cert": self.config.verify_server_cert,
             "server_cert": self.config.server_cert,
             "timeout": self.config.server_timeout,
             "processors": self.load_processors(),
         }
         self._api_endpoint_url = compat.urlparse.urljoin(
             self.config.server_url if self.config.server_url.endswith("/") else self.config.server_url + "/",
             constants.EVENTS_API_PATH,
         )
         transport_class = import_string(self.config.transport_class)
-        self._transport = transport_class(self._api_endpoint_url, self, **transport_kwargs)
+        self._transport = transport_class(url=self._api_endpoint_url, client=self, **transport_kwargs)
         self.config.transport = self._transport
         self._thread_managers["transport"] = self._transport
 
         for exc_to_filter in self.config.filter_exception_types or []:
             exc_to_filter_type = exc_to_filter.split(".")[-1]
             exc_to_filter_module = ".".join(exc_to_filter.split(".")[:-1])
             self.filter_exception_types_dict[exc_to_filter_type] = exc_to_filter_module
@@ -195,15 +197,16 @@
         self._metrics = MetricsRegistry(self)
         for path in self.config.metrics_sets:
             self._metrics.register(path)
         if self.config.breakdown_metrics:
             self._metrics.register("elasticapm.metrics.sets.breakdown.BreakdownMetricSet")
         if self.config.prometheus_metrics:
             self._metrics.register("elasticapm.metrics.sets.prometheus.PrometheusMetrics")
-        self._thread_managers["metrics"] = self._metrics
+        if self.config.metrics_interval:
+            self._thread_managers["metrics"] = self._metrics
         compat.atexit_register(self.close)
         if self.config.central_config:
             self._thread_managers["config"] = self.config
         else:
             self._config_updater = None
         if self.config.use_elastic_excepthook:
             self.original_excepthook = sys.excepthook
@@ -413,14 +416,25 @@
                 return data
             data = cloud.azure_metadata()
             return data
         else:
             self.logger.warning("Unknown value for CLOUD_PROVIDER, skipping cloud metadata: {}".format(provider))
             return {}
 
+    def get_user_agent(self) -> str:
+        """
+        Compiles the user agent, which will be added as a header to all requests
+        to the APM Server
+        """
+        if self.config.service_version:
+            service_version = re.sub(r"[^\t _\x21-\x27\x2a-\x5b\x5d-\x7e\x80-\xff]", "_", self.config.service_version)
+            return "apm-agent-python/{} ({} {})".format(elasticapm.VERSION, self.config.service_name, service_version)
+        else:
+            return "apm-agent-python/{} ({})".format(elasticapm.VERSION, self.config.service_name)
+
     def build_metadata(self):
         data = {
             "service": self.get_service_info(),
             "process": self.get_process_info(),
             "system": self.get_system_info(),
             "cloud": self.get_cloud_info(),
         }
@@ -613,25 +627,39 @@
                     "Please upgrade to Python 3.5+ to continue to use the latest features."
                 ),
                 PendingDeprecationWarning,
             )
         elif v < (3, 5):
             warnings.warn("The Elastic APM agent only supports Python 3.5+", DeprecationWarning)
 
+    def check_server_version(self, gte: Optional[Tuple[int]] = None, lte: Optional[Tuple[int]] = None) -> bool:
+        """
+        Check APM Server version against greater-or-equal and/or lower-or-equal limits, provided as tuples of integers.
+        If server_version is not set, always returns True.
+        :param gte: a tuple of ints describing the greater-or-equal limit, e.g. (7, 16)
+        :param lte: a tuple of ints describing the lower-or-equal limit, e.g. (7, 99)
+        :return: bool
+        """
+        if not self.server_version:
+            return True
+        gte = gte or (0,)
+        lte = lte or (2 ** 32,)  # let's assume APM Server version will never be greater than 2^32
+        return bool(gte <= self.server_version <= lte)
+
 
 class DummyClient(Client):
     """Sends messages into an empty void"""
 
     def send(self, url, **kwargs):
         return None
 
 
-def get_client():
+def get_client() -> Client:
     return CLIENT_SINGLETON
 
 
-def set_client(client):
+def set_client(client: Client):
     global CLIENT_SINGLETON
     if CLIENT_SINGLETON:
         logger = get_logger("elasticapm")
         logger.warning("Client object is being set more than once", stack_info=True)
     CLIENT_SINGLETON = client
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/conf/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,15 +546,14 @@
     sanitize_field_names = _ListConfigValue(
         "SANITIZE_FIELD_NAMES", type=starmatch_to_regex, default=BASE_SANITIZE_FIELD_NAMES
     )
     metrics_sets = _ListConfigValue(
         "METRICS_SETS",
         default=[
             "elasticapm.metrics.sets.cpu.CPUMetricSet",
-            "elasticapm.metrics.sets.transactions.TransactionsMetricSet",
         ],
     )
     metrics_interval = _ConfigValue(
         "METRICS_INTERVAL",
         type=int,
         validators=[duration_validator, ExcludeRangeValidator(1, 999, "{range_start} - {range_end} ms")],
         default=30000,
@@ -575,14 +574,27 @@
         "SPAN_FRAMES_MIN_DURATION",
         default=5,
         validators=[
             UnitValidator(r"^((?:-)?\d+)(ms|s|m)?$", r"\d+(ms|s|m)", {"ms": 1, "s": 1000, "m": 60000, None: 1})
         ],
         type=int,
     )
+    span_compression_enabled = _BoolConfigValue("SPAN_COMPRESSION_ENABLED", default=False)
+    span_compression_exact_match_max_duration = _ConfigValue(
+        "SPAN_COMPRESSION_EXACT_MATCH_MAX_DURATION",
+        default=50,
+        validators=[duration_validator],
+        type=int,
+    )
+    span_compression_same_kind_max_duration = _ConfigValue(
+        "SPAN_COMPRESSION_SAME_KIND_MAX_DURATION",
+        default=5,
+        validators=[duration_validator],
+        type=int,
+    )
     collect_local_variables = _ConfigValue("COLLECT_LOCAL_VARIABLES", default="errors")
     source_lines_error_app_frames = _ConfigValue("SOURCE_LINES_ERROR_APP_FRAMES", type=int, default=5)
     source_lines_error_library_frames = _ConfigValue("SOURCE_LINES_ERROR_LIBRARY_FRAMES", type=int, default=5)
     source_lines_span_app_frames = _ConfigValue("SOURCE_LINES_SPAN_APP_FRAMES", type=int, default=0)
     source_lines_span_library_frames = _ConfigValue("SOURCE_LINES_SPAN_LIBRARY_FRAMES", type=int, default=0)
     local_var_max_length = _ConfigValue("LOCAL_VAR_MAX_LENGTH", type=int, default=200)
     local_var_list_max_length = _ConfigValue("LOCAL_VAR_LIST_MAX_LENGTH", type=int, default=10)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/conf/constants.py` & `sf-elastic-apm-6.7.2/elasticapm/conf/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         else:
             res.append(re.escape(c))
     return re.compile(r"(?:%s)\Z" % "".join(res), options)
 
 
 EVENTS_API_PATH = "intake/v2/events"
 AGENT_CONFIG_PATH = "config/v1/agents"
-SERVER_INFO_PATH = "/"
+SERVER_INFO_PATH = ""
 
 TRACE_CONTEXT_VERSION = 0
 TRACEPARENT_HEADER_NAME = "traceparent"
 TRACEPARENT_LEGACY_HEADER_NAME = "elastic-apm-traceparent"
 TRACESTATE_HEADER_NAME = "tracestate"
 
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/context/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/context/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/context/base.py` & `sf-elastic-apm-6.7.2/elasticapm/context/base.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/context/contextvars.py` & `sf-elastic-apm-6.7.2/elasticapm/context/contextvars.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/context/threadlocal.py` & `sf-elastic-apm-6.7.2/elasticapm/context/threadlocal.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,10 +44,10 @@
         self.app = app
         self.client = client
         self.install_tracing(app, client)
 
     def install_tracing(self, app, client):
         from elasticapm.contrib.aiohttp.middleware import tracing_middleware
 
-        app.middlewares.insert(0, tracing_middleware(app))
+        app.middlewares.insert(0, tracing_middleware(app, client))
         if client.config.instrument and client.config.enabled:
             elasticapm.instrument()
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/middleware.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import aiohttp
-from aiohttp.web import HTTPException, Response, middleware
+from aiohttp.web import HTTPException, middleware
 
 import elasticapm
 from elasticapm import get_client
 from elasticapm.conf import constants
 from elasticapm.contrib.aiohttp.utils import get_data_from_request, get_data_from_response
 from elasticapm.utils.disttracing import TraceParent
 
 
 class AioHttpTraceParent(TraceParent):
     @classmethod
     def merge_duplicate_headers(cls, headers, key):
         return ",".join(headers.getall(key, [])) or None
 
 
-def tracing_middleware(app):
+def tracing_middleware(app, client=None):
     async def handle_request(request, handler):
-        elasticapm_client = get_client()
+        elasticapm_client = get_client() if client is None else client
         should_trace = elasticapm_client and not elasticapm_client.should_ignore_url(request.path)
         if should_trace:
             trace_parent = AioHttpTraceParent.from_headers(request.headers)
             elasticapm_client.begin_transaction("request", trace_parent=trace_parent)
             resource = request.match_info.route.resource
             name = request.method
             if resource:
@@ -74,29 +74,45 @@
                 elasticapm.set_transaction_result("HTTP {}xx".format(response.status // 100), override=False)
                 elasticapm.set_transaction_outcome(http_status_code=response.status, override=False)
                 elasticapm.set_context(
                     lambda: get_data_from_response(response, elasticapm_client.config, constants.TRANSACTION),
                     "response",
                 )
             return response
-        except Exception as exc:
+        except HTTPException as exc:
+            # HTTPExceptions are response-like, e.g. have headers and status code. They can represent an HTTP
+            # response below a 500 status code and therefore not something to capture as exception. Like
+            # HTTPOk can be raised but will most likely be wrongly tagged as an APM error. Let's try and
+            # capture this according to the status.
+            if exc.status_code < 500 and not should_trace:
+                raise
             if elasticapm_client:
-                elasticapm_client.capture_exception(
-                    context={"request": get_data_from_request(request, elasticapm_client.config, constants.ERROR)}
+                elasticapm.set_transaction_result("HTTP {}xx".format(exc.status_code // 100), override=False)
+                elasticapm.set_transaction_outcome(http_status_code=exc.status_code, override=False)
+                elasticapm.set_context(
+                    lambda: get_data_from_response(
+                        exc,  # noqa: F821
+                        elasticapm_client.config,
+                        constants.ERROR if exc.status_code >= 500 else constants.TRANSACTION,  # noqa: F821
+                    ),
+                    "response",
                 )
+                if exc.status_code >= 500:
+                    elasticapm_client.capture_exception(
+                        context={"request": get_data_from_request(request, elasticapm_client.config, constants.ERROR)}
+                    )
+            raise
+        except Exception:
+            if elasticapm_client:
                 elasticapm.set_transaction_result("HTTP 5xx", override=False)
                 elasticapm.set_transaction_outcome(http_status_code=500, override=False)
                 elasticapm.set_context({"status_code": 500}, "response")
-                # some exceptions are response-like, e.g. have headers and status code. Let's try and capture them
-                if isinstance(exc, (Response, HTTPException)):
-                    elasticapm.set_context(
-                        lambda: get_data_from_response(exc, elasticapm_client.config, constants.ERROR),  # noqa: F821
-                        "response",
-                    )
-
+                elasticapm_client.capture_exception(
+                    context={"request": get_data_from_request(request, elasticapm_client.config, constants.ERROR)}
+                )
             raise
         finally:
             elasticapm_client.end_transaction()
 
     # decorating with @middleware is only required in aiohttp < 4.0, and we only support 3+
     if aiohttp.__version__.startswith("3"):
         return middleware(handle_request)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/aiohttp/utils.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/aiohttp/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from elasticapm.conf import Config
 from elasticapm.utils import compat, get_url_dict
 
 
 def get_data_from_request(request: Request, config: Config, event_type: str):
     result = {
         "method": request.method,
-        "socket": {"remote_address": request.remote, "encrypted": request.secure},
+        "socket": {"remote_address": request.remote},
         "cookies": dict(request.cookies),
     }
     if config.capture_headers:
         result["headers"] = dict(request.headers)
 
     # TODO: capture body
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/asyncio/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/asyncio/traces.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/asyncio/traces.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/celery/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/apps.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/celery/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/celery/models.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/celery/models.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/client.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,26 @@
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 
 
 from __future__ import absolute_import
 
 import django
 from django.conf import settings as django_settings
-from django.core.exceptions import DisallowedHost
 from django.db import DatabaseError
 from django.http import HttpRequest
 
 try:
     from rest_framework.request import Request as DrfRequest
 except ImportError:
     DrfRequest = HttpRequest
 
 from elasticapm import get_client as _get_client
 from elasticapm.base import Client
 from elasticapm.conf import constants
-from elasticapm.contrib.django.utils import iterate_with_template_sources
+from elasticapm.contrib.django.utils import get_raw_uri, iterate_with_template_sources
 from elasticapm.utils import compat, encoding, get_url_dict
 from elasticapm.utils.logging import get_logger
 from elasticapm.utils.module_import import import_string
 from elasticapm.utils.wsgi import get_environ, get_headers
 
 __all__ = ("DjangoClient",)
 
@@ -115,15 +114,15 @@
 
         return user_info
 
     def get_data_from_request(self, request, event_type):
         result = {
             "env": dict(get_environ(request.META)),
             "method": request.method,
-            "socket": {"remote_address": request.META.get("REMOTE_ADDR"), "encrypted": request.is_secure()},
+            "socket": {"remote_address": request.META.get("REMOTE_ADDR")},
             "cookies": dict(request.COOKIES),
         }
         if self.config.capture_headers:
             request_headers = dict(get_headers(request.META))
 
             for key, value in request_headers.items():
                 if isinstance(value, (int, float)):
@@ -148,29 +147,16 @@
                         data = request.body
                     except Exception as e:
                         self.logger.debug("Can't capture request body: %s", compat.text_type(e))
                         data = "<unavailable>"
                 if data is not None:
                     result["body"] = data
 
-        if hasattr(request, "get_raw_uri"):
-            # added in Django 1.9
-            url = request.get_raw_uri()
-        else:
-            try:
-                # Requires host to be in ALLOWED_HOSTS, might throw a
-                # DisallowedHost exception
-                url = request.build_absolute_uri()
-            except DisallowedHost:
-                # We can't figure out the real URL, so we have to set it to
-                # DisallowedHost
-                result["url"] = {"full": "DisallowedHost"}
-                url = None
-        if url:
-            result["url"] = get_url_dict(url)
+        url = get_raw_uri(request)
+        result["url"] = get_url_dict(url)
         return result
 
     def get_data_from_response(self, response, event_type):
         result = {"status_code": response.status_code}
 
         if self.config.capture_headers and hasattr(response, "items"):
             response_headers = dict(response.items())
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/context_processors.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/handlers.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/handlers.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/commands/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/management/commands/elasticapm.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/management/commands/elasticapm.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/middleware/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/middleware/wsgi.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/django/utils.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/django/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 import logging
 
+from django.http import HttpRequest
 from django.template.base import Node
 
 from elasticapm.utils.stacks import get_frame_info
 
 try:
     from django.template.base import Template
 except ImportError:
@@ -87,7 +88,24 @@
             library_frame_context_lines=library_frame_context_lines,
             in_app_frame_context_lines=in_app_frame_context_lines,
             with_locals=with_locals,
             include_paths_re=include_paths_re,
             exclude_paths_re=exclude_paths_re,
             locals_processor_func=locals_processor_func,
         )
+
+
+def get_raw_uri(request: HttpRequest) -> str:
+    """
+    Return an absolute URI from variables available in this request. Skip
+    allowed hosts protection, so may return insecure URI.
+
+    Re-implementation of Request.get_raw_uri that was removed with Django 4.0.
+
+    :param request: a Request object
+    :return: the URL
+    """
+    return "{scheme}://{host}{path}".format(
+        scheme=request.scheme,
+        host=request._get_raw_host(),
+        path=request.get_full_path(),
+    )
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/flask/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/flask/utils.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/flask/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from elasticapm.utils.wsgi import get_environ, get_headers
 
 
 def get_data_from_request(request, config, event_type):
     result = {
         "env": dict(get_environ(request.environ)),
         "method": request.method,
-        "socket": {"remote_address": request.environ.get("REMOTE_ADDR"), "encrypted": request.is_secure},
+        "socket": {"remote_address": request.environ.get("REMOTE_ADDR")},
         "cookies": request.cookies,
     }
     if config.capture_headers:
         result["headers"] = dict(get_headers(request.environ))
     if request.method in constants.HTTP_WITH_BODY:
         if config.capture_body not in ("all", event_type):
             result["body"] = "[REDACTED]"
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/span.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/opentracing/tracer.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/paste.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/paste.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/pylons/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/rq/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/starlette/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/starlette/utils.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/starlette/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         event_type (str)
 
     Returns:
         dict
     """
     result = {
         "method": request.method,
-        "socket": {"remote_address": _get_client_ip(request), "encrypted": request.url.is_secure},
+        "socket": {"remote_address": _get_client_ip(request)},
         "cookies": request.cookies,
     }
     if config.capture_headers:
         result["headers"] = dict(request.headers)
 
     if request.method in constants.HTTP_WITH_BODY:
         if config.capture_body not in ("all", event_type):
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/tornado/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/tornado/utils.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/tornado/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def get_data_from_request(request_handler, request, config, event_type):
     """
     Capture relevant data from a tornado.httputil.HTTPServerRequest
     """
     result = {
         "method": request.method,
-        "socket": {"remote_address": request.remote_ip, "encrypted": request.protocol == "https"},
+        "socket": {"remote_address": request.remote_ip},
         "cookies": request.cookies,
         "http_version": request.version,
     }
     if config.capture_headers:
         result["headers"] = dict(request.headers)
     if request.method in constants.HTTP_WITH_BODY:
         if tornado.web._has_stream_request_body(request_handler.__class__):
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/twisted/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/contrib/zerorpc/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/zerorpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/events.py` & `sf-elastic-apm-6.7.2/elasticapm/events.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/handlers/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/handlers/logbook.py` & `sf-elastic-apm-6.7.2/elasticapm/handlers/logbook.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/handlers/logging.py` & `sf-elastic-apm-6.7.2/elasticapm/handlers/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -227,23 +227,20 @@
     span = execution_context.get_span()
     span_id = span.id if span else None
     record.elasticapm_span_id = span_id
 
     client = get_client()
     service_name = client.config.service_name if client else None
     record.elasticapm_service_name = service_name
-    event_dataset = f"{client.config.service_name}.log" if client else None
-    record.elasticapm_event_dataset = event_dataset
 
     record.elasticapm_labels = {
         "transaction.id": transaction_id,
         "trace.id": trace_id,
         "span.id": span_id,
         "service.name": service_name,
-        "event.dataset": event_dataset,
     }
 
     return record
 
 
 class Formatter(logging.Formatter):
     """
@@ -275,18 +272,16 @@
 
     def format(self, record):
         if not hasattr(record, "elasticapm_transaction_id"):
             record.elasticapm_transaction_id = None
             record.elasticapm_trace_id = None
             record.elasticapm_span_id = None
             record.elasticapm_service_name = None
-            record.elasticapm_event_dataset = None
         return super(Formatter, self).format(record=record)
 
     def formatTime(self, record, datefmt=None):
         if not hasattr(record, "elasticapm_transaction_id"):
             record.elasticapm_transaction_id = None
             record.elasticapm_trace_id = None
             record.elasticapm_span_id = None
             record.elasticapm_service_name = None
-            record.elasticapm_event_dataset = None
         return super(Formatter, self).formatTime(record=record, datefmt=datefmt)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/handlers/structlog.py` & `sf-elastic-apm-6.7.2/elasticapm/handlers/structlog.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,13 @@
     """
     transaction = execution_context.get_transaction()
     if transaction:
         event_dict["transaction.id"] = transaction.id
     client = get_client()
     if client:
         event_dict["service.name"] = client.config.service_name
-        event_dict["event.dataset"] = f"{client.config.service_name}.log"
     if transaction and transaction.trace_parent:
         event_dict["trace.id"] = transaction.trace_parent.trace_id
     span = execution_context.get_span()
     if span and span.id:
         event_dict["span.id"] = span.id
     return event_dict
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/control.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/control.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,38 +28,37 @@
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm import async_capture_span
 from elasticapm.conf import constants
 from elasticapm.instrumentation.packages.asyncio.base import AsyncAbstractInstrumentedModule
 from elasticapm.traces import DroppedSpan, execution_context
-from elasticapm.utils import get_host_from_url, sanitize_url, url_to_destination
+from elasticapm.utils import get_host_from_url, sanitize_url
 from elasticapm.utils.disttracing import TracingOptions
 
 
 class AioHttpClientInstrumentation(AsyncAbstractInstrumentedModule):
     name = "aiohttp_client"
 
     instrument_list = [("aiohttp.client", "ClientSession._request")]
 
     async def call(self, module, method, wrapped, instance, args, kwargs):
         method = kwargs["method"] if "method" in kwargs else args[0]
         url = kwargs["url"] if "url" in kwargs else args[1]
         url = str(url)
-        destination = url_to_destination(url)
 
         signature = " ".join([method.upper(), get_host_from_url(url)])
         url = sanitize_url(url)
         transaction = execution_context.get_transaction()
 
         async with async_capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
             leaf_span = span
             while isinstance(leaf_span, DroppedSpan):
                 leaf_span = leaf_span.parent
 
             parent_id = leaf_span.id if leaf_span else transaction.id
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiomysql.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiomysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             query = shorten(query, string_length=10000)
 
             context = {
                 "db": {"type": "sql", "statement": query},
                 "destination": {
                     "address": instance.connection.host,
                     "port": instance.connection.port,
-                    "service": {"name": "mysql", "resource": "mysql", "type": "db"},
+                    "service": {"name": "", "resource": "mysql", "type": ""},
                 },
             }
             action = "query"
         else:
             raise AssertionError("call from uninstrumented method")
 
         async with async_capture_span(
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aiopg.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aiopg.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/aioredis.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/aioredis.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         span = execution_context.get_span()
         if span and span.subtype == "aioredis":
             span.context["destination"] = _get_destination_info(instance)
         return wrapped(*args, **kwargs)
 
 
 def _get_destination_info(connection):
-    destination_info = {"service": {"name": "aioredis", "resource": "redis", "type": "db"}}
+    destination_info = {"service": {"name": "", "resource": "redis", "type": ""}}
 
     if hasattr(connection, "_pool_or_conn"):
         destination_info["port"] = connection._pool_or_conn.address[1]
         destination_info["address"] = connection._pool_or_conn.address[0]
     else:
         destination_info["port"] = connection.address[1]
         destination_info["address"] = connection.address[0]
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/asyncpg.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/asyncpg.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,42 +28,52 @@
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm.contrib.asyncio.traces import async_capture_span
 from elasticapm.instrumentation.packages.asyncio.base import AsyncAbstractInstrumentedModule
 from elasticapm.instrumentation.packages.dbapi2 import extract_signature
 from elasticapm.utils import default_ports
+from elasticapm.utils.encoding import shorten
 
 
 class AsyncPGInstrumentation(AsyncAbstractInstrumentedModule):
     """
     Implement asyncpg instrumentation with two methods Connection.execute
     and Connection.executemany since Connection._do_execute is not called
     given a prepared query is passed to a connection. As in:
     https://github.com/MagicStack/asyncpg/blob/master/asyncpg/connection.py#L294-L297
     """
 
     name = "asyncpg"
 
     instrument_list = [
-        ("asyncpg.connection", "Connection.execute"),
-        ("asyncpg.connection", "Connection.executemany"),
-        ("asyncpg.connection", "Connection.fetch"),
-        ("asyncpg.connection", "Connection.fetchval"),
-        ("asyncpg.connection", "Connection.fetchrow"),
+        ("asyncpg.protocol.protocol", "Protocol.bind_execute"),
+        ("asyncpg.protocol.protocol", "Protocol.bind_execute_many"),
+        ("asyncpg.protocol.protocol", "Protocol.bind"),
+        ("asyncpg.protocol.protocol", "Protocol.execute"),
+        ("asyncpg.protocol.protocol", "Protocol.query"),
+        ("asyncpg.protocol.protocol", "Protocol.copy_in"),
+        ("asyncpg.protocol.protocol", "Protocol.copy_out"),
     ]
 
+    def get_query(self, method, args):
+        if method in ["Protocol.query", "Protocol.copy_in", "Protocol.copy_out"]:
+            return args[0]
+        else:
+            return args[0].query
+
     async def call(self, module, method, wrapped, instance, args, kwargs):
-        query = args[0] if len(args) else kwargs["query"]
+        query = self.get_query(method, args)
         name = extract_signature(query)
-        context = {"db": {"type": "sql", "statement": query}}
+        sql_string = shorten(query, string_length=10000)
+        context = {"db": {"type": "sql", "statement": sql_string}}
         action = "query"
         destination_info = {
             "address": kwargs.get("host", "localhost"),
             "port": int(kwargs.get("port", default_ports.get("postgresql"))),
-            "service": {"name": "postgres", "resource": "postgres", "type": "db"},
+            "service": {"name": "", "resource": "postgresql", "type": ""},
         }
         context["destination"] = destination_info
         async with async_capture_span(
-            name, leaf=True, span_type="db", span_subtype="postgres", span_action=action, extra=context
+            name, leaf=True, span_type="db", span_subtype="postgresql", span_action=action, extra=context
         ):
             return await wrapped(*args, **kwargs)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/base.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/elasticsearch.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/httpcore.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/urllib3.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,120 +24,120 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import itertools
+
 from elasticapm.conf import constants
-from elasticapm.contrib.asyncio.traces import async_capture_span
-from elasticapm.instrumentation.packages.asyncio.base import AsyncAbstractInstrumentedModule
-from elasticapm.traces import DroppedSpan, execution_context
-from elasticapm.utils import default_ports, url_to_destination
+from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
+from elasticapm.traces import DroppedSpan, capture_span, execution_context
+from elasticapm.utils import default_ports
 from elasticapm.utils.disttracing import TracingOptions
 
 
-class HTTPCoreAsyncInstrumentation(AsyncAbstractInstrumentedModule):
+def _set_disttracing_headers(headers, trace_parent, transaction):
+    trace_parent_str = trace_parent.to_string()
+    headers[constants.TRACEPARENT_HEADER_NAME] = trace_parent_str
+    if transaction.tracer.config.use_elastic_traceparent_header:
+        headers[constants.TRACEPARENT_LEGACY_HEADER_NAME] = trace_parent_str
+    if trace_parent.tracestate:
+        headers[constants.TRACESTATE_HEADER_NAME] = trace_parent.tracestate
+
+
+def update_headers(args, kwargs, instance, transaction, trace_parent):
     """
-    This instrumentation only exists to make sure we add distributed tracing
-    headers on our requests from `httpx`. `httpx` is the only place this library
-    is used, so no spans will actually be created (due to already being in
-    a leaf span). However, the rest of the logic was left in (much of this
-    mirrors the urllib3 instrumentation) in case that situation ever changes.
+    The headers might be in 3 different places: as 4th positional argument, as "headers" keyword argument,
+    or, if none of the former two are provided, as instance variable on the HTTPConnection object.
+
+    If the headers are in the positional arguments tuple, a new tuple with updated headers will be returned.
+    If they are in the keyword arguments or on the instance, an updated kwargs dict will be returned
+
+    :param args: list of positional arguments
+    :param kwargs: dict of keyword arguments
+    :param instance: the HTTPConnection instance
+    :param transaction: the Transaction object
+    :param trace_parent: the TraceParent object
+    :return: an (args, kwargs) tuple
     """
+    if len(args) >= 4 and args[3]:
+        headers = args[3].copy()
+        args = tuple(itertools.chain((args[:3]), (headers,), args[4:]))
+    elif "headers" in kwargs and kwargs["headers"]:
+        headers = kwargs["headers"].copy()
+        kwargs["headers"] = headers
+    else:
+        headers = instance.headers.copy() if instance.headers else {}
+        # we don't want to change the instance headers, so we'll cheat and
+        # set the headers as keywords. This slightly changes how the wrapped
+        # method is called compared to uninstrumented code.
+        kwargs["headers"] = headers
+    _set_disttracing_headers(headers, trace_parent, transaction)
+    return args, kwargs
 
-    name = "httpcore"
+
+class Urllib3Instrumentation(AbstractInstrumentedModule):
+    name = "urllib3"
 
     instrument_list = [
-        ("httpcore._async.connection", "AsyncHTTPConnection.request"),  # < httpcore 0.11
-        ("httpcore._async.connection", "AsyncHTTPConnection.arequest"),  # httpcore 0.11 - 0.12
-        ("httpcore._async.connection", "AsyncHTTPConnection.handle_async_request"),  # >= httpcore 0.13
+        ("urllib3.connectionpool", "HTTPConnectionPool.urlopen"),
+        # packages that vendor or vendored urllib3 in the past
+        ("requests.packages.urllib3.connectionpool", "HTTPConnectionPool.urlopen"),
+        ("botocore.vendored.requests.packages.urllib3.connectionpool", "HTTPConnectionPool.urlopen"),
     ]
 
-    async def call(self, module, method, wrapped, instance, args, kwargs):
+    def call(self, module, method, wrapped, instance, args, kwargs):
         if "method" in kwargs:
-            method = kwargs["method"].decode("utf-8")
+            method = kwargs["method"]
         else:
-            method = args[0].decode("utf-8")
+            method = args[0]
 
-        # URL is a tuple of (scheme, host, port, path), we want path
-        if "url" in kwargs:
-            url = kwargs["url"][3].decode("utf-8")
-        else:
-            url = args[1][3].decode("utf-8")
+        host = instance.host
 
-        headers = None
-        if "headers" in kwargs:
-            headers = kwargs["headers"]
-            if headers is None:
-                headers = []
-                kwargs["headers"] = headers
-
-        scheme, host, port = instance.origin
-        scheme = scheme.decode("utf-8")
-        host = host.decode("utf-8")
+        if instance.port != default_ports.get(instance.scheme):
+            host += ":" + str(instance.port)
 
-        if port != default_ports.get(scheme):
-            host += ":" + str(port)
+        if "url" in kwargs:
+            url = kwargs["url"]
+        else:
+            url = args[1]
 
-        signature = "%s %s" % (method.upper(), host)
+        signature = method.upper() + " " + host
 
-        url = "%s://%s%s" % (scheme, host, url)
-        destination = url_to_destination(url)
+        url = "%s://%s%s" % (instance.scheme, host, url)
 
         transaction = execution_context.get_transaction()
 
-        async with async_capture_span(
+        with capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
-            # if httpcore has been called in a leaf span, this span might be a DroppedSpan.
+            # if urllib3 has been called in a leaf span, this span might be a DroppedSpan.
             leaf_span = span
             while isinstance(leaf_span, DroppedSpan):
                 leaf_span = leaf_span.parent
 
-            if headers is not None:
-                # It's possible that there are only dropped spans, e.g. if we started dropping spans due to the
-                # transaction_max_spans limit. In this case, the transaction.id is used
-                parent_id = leaf_span.id if leaf_span else transaction.id
-                trace_parent = transaction.trace_parent.copy_from(
-                    span_id=parent_id, trace_options=TracingOptions(recorded=True)
-                )
-                self._set_disttracing_headers(headers, trace_parent, transaction)
-            response = await wrapped(*args, **kwargs)
-            if len(response) > 4:
-                # httpcore < 0.11.0
-                # response = (http_version, status_code, reason_phrase, headers, stream)
-                status_code = response[1]
-            else:
-                # httpcore >= 0.11.0
-                # response = (status_code, headers, stream, ext)
-                status_code = response[0]
-            if status_code:
+            parent_id = leaf_span.id if leaf_span else transaction.id
+            trace_parent = transaction.trace_parent.copy_from(
+                span_id=parent_id, trace_options=TracingOptions(recorded=True)
+            )
+            args, kwargs = update_headers(args, kwargs, instance, transaction, trace_parent)
+            if leaf_span:
+                leaf_span.dist_tracing_propagated = True
+            response = wrapped(*args, **kwargs)
+            if response:
                 if span.context:
-                    span.context["http"]["status_code"] = status_code
-                span.set_success() if status_code < 400 else span.set_failure()
+                    span.context["http"]["status_code"] = response.status
+                span.set_success() if response.status < 400 else span.set_failure()
             return response
 
     def mutate_unsampled_call_args(self, module, method, wrapped, instance, args, kwargs, transaction):
         # since we don't have a span, we set the span id to the transaction id
         trace_parent = transaction.trace_parent.copy_from(
             span_id=transaction.id, trace_options=TracingOptions(recorded=False)
         )
-        if "headers" in kwargs:
-            headers = kwargs["headers"]
-            if headers is None:
-                headers = []
-                kwargs["headers"] = headers
-            self._set_disttracing_headers(headers, trace_parent, transaction)
-        return args, kwargs
-
-    def _set_disttracing_headers(self, headers, trace_parent, transaction):
-        trace_parent_str = trace_parent.to_string()
-        headers.append((bytes(constants.TRACEPARENT_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
-        if transaction.tracer.config.use_elastic_traceparent_header:
-            headers.append((bytes(constants.TRACEPARENT_LEGACY_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
-        if trace_parent.tracestate:
-            headers.append((bytes(constants.TRACESTATE_HEADER_NAME, "utf-8"), bytes(trace_parent.tracestate, "utf-8")))
+        return update_headers(args, kwargs, instance, transaction, trace_parent)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/httpx.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/httpx.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,36 +26,35 @@
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm.contrib.asyncio.traces import async_capture_span
 from elasticapm.instrumentation.packages.asyncio.base import AsyncAbstractInstrumentedModule
-from elasticapm.utils import get_host_from_url, sanitize_url, url_to_destination
+from elasticapm.utils import get_host_from_url, sanitize_url
 
 
 class HttpxAsyncClientInstrumentation(AsyncAbstractInstrumentedModule):
     name = "httpx"
 
     instrument_list = [("httpx", "AsyncClient.send")]
 
     async def call(self, module, method, wrapped, instance, args, kwargs):
-        request = kwargs.get("request", args[0])
+        request = kwargs.get("request") or args[0]
 
         request_method = request.method.upper()
         url = str(request.url)
         name = "{request_method} {host}".format(request_method=request_method, host=get_host_from_url(url))
         url = sanitize_url(url)
-        destination = url_to_destination(url)
 
         async with async_capture_span(
             name,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
             response = await wrapped(*args, **kwargs)
             if response is not None:
                 if span.context:
                     span.context["http"]["status_code"] = response.status_code
                 span.set_success() if response.status_code < 400 else span.set_failure()
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/asyncio/sleep.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/asyncio/sleep.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/base.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/base.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/botocore.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/botocore.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/cassandra.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/cassandra.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,12 +71,11 @@
                 query_str = None
             if query_str:
                 name = extract_signature(query_str)
                 context["db"] = {"type": "sql", "statement": query_str}
         context["destination"] = {
             "address": host,
             "port": port,
-            "service": {"name": "cassandra", "resource": "cassandra", "type": "db"},
         }
 
         with capture_span(name, span_type="db", span_subtype="cassandra", span_action=span_action, extra=context):
             return wrapped(*args, **kwargs)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/dbapi2.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/dbapi2.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 class CursorProxy(wrapt.ObjectProxy):
     provider_name = None
     DML_QUERIES = ("INSERT", "DELETE", "UPDATE")
 
     def __init__(self, wrapped, destination_info=None):
         super(CursorProxy, self).__init__(wrapped)
-        self._self_destination_info = destination_info
+        self._self_destination_info = destination_info or {}
 
     def callproc(self, procname, params=None):
         return self._trace_sql(self.__wrapped__.callproc, procname, params, action=EXEC_ACTION)
 
     def execute(self, sql, params=None):
         return self._trace_sql(self.__wrapped__.execute, sql, params)
 
@@ -233,14 +233,15 @@
         with capture_span(
             signature,
             span_type="db",
             span_subtype=self.provider_name,
             span_action=action,
             extra={"db": {"type": "sql", "statement": sql_string}, "destination": self._self_destination_info},
             skip_frames=1,
+            leaf=True,
         ) as span:
             if params is None:
                 result = method(sql)
             else:
                 result = method(sql, params)
             # store "rows affected", but only for DML queries like insert/update/delete
             if span and self.rowcount not in (-1, None) and signature.startswith(self.DML_QUERIES):
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/django/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/django/template.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/django/template.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/elasticsearch.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/elasticsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,14 @@
                 else:
                     query.append(body_serialized)
             if query:
                 context["db"]["statement"] = "\n\n".join(query)
 
         context["destination"] = {
             "address": instance.host,
-            "service": {"name": "elasticsearch", "resource": "elasticsearch", "type": "db"},
         }
 
 
 class ElasticsearchTransportInstrumentation(AbstractInstrumentedModule):
     name = "elasticsearch_connection"
 
     instrument_list = [
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/graphql.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/graphql.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httpcore.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/urllib.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,110 +24,101 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+
 from elasticapm.conf import constants
 from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
 from elasticapm.traces import DroppedSpan, capture_span, execution_context
-from elasticapm.utils import default_ports, url_to_destination
+from elasticapm.utils import compat, default_ports, sanitize_url
 from elasticapm.utils.disttracing import TracingOptions
 
 
-class HTTPCoreInstrumentation(AbstractInstrumentedModule):
-    name = "httpcore"
-
-    instrument_list = [
-        ("httpcore._sync.connection", "SyncHTTPConnection.request"),  # < httpcore 0.13
-        ("httpcore._sync.connection", "SyncHTTPConnection.handle_request"),  # >= httpcore 0.13
-    ]
+# copied and adapted from urllib.request
+def request_host(request):
+    """Return request-host, as defined by RFC 2965.
+
+    Variation from RFC: returned value is lowercased, for convenient
+    comparison.
+
+    """
+    url = request.get_full_url()
+    parse_result = compat.urlparse.urlparse(url)
+    scheme, host, port = parse_result.scheme, parse_result.hostname, parse_result.port
+    try:
+        port = int(port)
+    except (ValueError, TypeError):
+        pass
+    if host == "":
+        host = request.get_header("Host", "")
+
+    if port and port != default_ports.get(scheme):
+        host = "%s:%s" % (host, port)
+    return host
+
+
+class UrllibInstrumentation(AbstractInstrumentedModule):
+    name = "urllib"
+
+    if compat.PY2:
+        instrument_list = [("urllib2", "AbstractHTTPHandler.do_open")]
+    else:
+        instrument_list = [("urllib.request", "AbstractHTTPHandler.do_open")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
-        if "method" in kwargs:
-            method = kwargs["method"].decode("utf-8")
-        else:
-            method = args[0].decode("utf-8")
-
-        # URL is a tuple of (scheme, host, port, path), we want path
-        if "url" in kwargs:
-            url = kwargs["url"][3].decode("utf-8")
-        else:
-            url = args[1][3].decode("utf-8")
-
-        headers = None
-        if "headers" in kwargs:
-            headers = kwargs["headers"]
-            if headers is None:
-                headers = []
-                kwargs["headers"] = headers
-
-        scheme, host, port = instance.origin
-        scheme = scheme.decode("utf-8")
-        host = host.decode("utf-8")
+        request_object = args[1] if len(args) > 1 else kwargs["req"]
 
-        if port != default_ports.get(scheme):
-            host += ":" + str(port)
+        method = request_object.get_method()
+        host = request_host(request_object)
 
-        signature = "%s %s" % (method.upper(), host)
-
-        url = "%s://%s%s" % (scheme, host, url)
-        destination = url_to_destination(url)
+        url = sanitize_url(request_object.get_full_url())
+        signature = method.upper() + " " + host
 
         transaction = execution_context.get_transaction()
 
         with capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
-            # if httpcore has been called in a leaf span, this span might be a DroppedSpan.
+            # if urllib has been called in a leaf span, this span might be a DroppedSpan.
             leaf_span = span
             while isinstance(leaf_span, DroppedSpan):
                 leaf_span = leaf_span.parent
 
-            if headers is not None:
-                # It's possible that there are only dropped spans, e.g. if we started dropping spans.
-                # In this case, the transaction.id is used
-                parent_id = leaf_span.id if leaf_span else transaction.id
-                trace_parent = transaction.trace_parent.copy_from(
-                    span_id=parent_id, trace_options=TracingOptions(recorded=True)
-                )
-                self._set_disttracing_headers(headers, trace_parent, transaction)
+            parent_id = leaf_span.id if leaf_span else transaction.id
+            trace_parent = transaction.trace_parent.copy_from(
+                span_id=parent_id, trace_options=TracingOptions(recorded=True)
+            )
+            self._set_disttracing_headers(request_object, trace_parent, transaction)
+            if leaf_span:
+                leaf_span.dist_tracing_propagated = True
             response = wrapped(*args, **kwargs)
-            if len(response) > 4:
-                # httpcore < 0.11.0
-                # response = (http_version, status_code, reason_phrase, headers, stream)
-                status_code = response[1]
-            else:
-                # httpcore >= 0.11.0
-                # response = (status_code, headers, stream, ext)
-                status_code = response[0]
-            if status_code:
+            if response:
+                status = getattr(response, "status", None) or response.getcode()  # Python 2 compat
                 if span.context:
-                    span.context["http"]["status_code"] = status_code
-                span.set_success() if status_code < 400 else span.set_failure()
+                    span.context["http"]["status_code"] = status
+                span.set_success() if status < 400 else span.set_failure()
             return response
 
     def mutate_unsampled_call_args(self, module, method, wrapped, instance, args, kwargs, transaction):
+        request_object = args[1] if len(args) > 1 else kwargs["req"]
         # since we don't have a span, we set the span id to the transaction id
         trace_parent = transaction.trace_parent.copy_from(
             span_id=transaction.id, trace_options=TracingOptions(recorded=False)
         )
-        if "headers" in kwargs:
-            headers = kwargs["headers"]
-            if headers is None:
-                headers = []
-                kwargs["headers"] = headers
-            self._set_disttracing_headers(headers, trace_parent, transaction)
+
+        self._set_disttracing_headers(request_object, trace_parent, transaction)
         return args, kwargs
 
-    def _set_disttracing_headers(self, headers, trace_parent, transaction):
+    def _set_disttracing_headers(self, request_object, trace_parent, transaction):
         trace_parent_str = trace_parent.to_string()
-        headers.append((bytes(constants.TRACEPARENT_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
+        request_object.add_header(constants.TRACEPARENT_HEADER_NAME, trace_parent_str)
         if transaction.tracer.config.use_elastic_traceparent_header:
-            headers.append((bytes(constants.TRACEPARENT_LEGACY_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
+            request_object.add_header(constants.TRACEPARENT_LEGACY_HEADER_NAME, trace_parent_str)
         if trace_parent.tracestate:
-            headers.append((bytes(constants.TRACESTATE_HEADER_NAME, "utf-8"), bytes(trace_parent.tracestate, "utf-8")))
+            request_object.add_header(constants.TRACESTATE_HEADER_NAME, trace_parent.tracestate)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httplib2.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httplib2.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm.conf import constants
 from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
 from elasticapm.traces import DroppedSpan, capture_span, execution_context
-from elasticapm.utils import get_host_from_url, sanitize_url, url_to_destination
+from elasticapm.utils import get_host_from_url, sanitize_url
 from elasticapm.utils.disttracing import TracingOptions
 
 
 class Httplib2Instrumentation(AbstractInstrumentedModule):
     name = "httplib2"
 
     instrument_list = [("httplib2", "Http.request")]
@@ -68,35 +68,36 @@
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         args, kwargs, params = self._ensure_headers_in_kwargs(args, kwargs)
 
         signature = params.get("method", "GET").upper()
         signature += " " + get_host_from_url(params["url"])
         url = sanitize_url(params["url"])
-        destination = url_to_destination(url)
         transaction = execution_context.get_transaction()
         with capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
             # if httplib2 has been called in a leaf span, this span might be a DroppedSpan.
             leaf_span = span
             while isinstance(leaf_span, DroppedSpan):
                 leaf_span = leaf_span.parent
 
             # It's possible that there are only dropped spans, e.g. if we started dropping spans.
             # In this case, the transaction.id is used
             parent_id = leaf_span.id if leaf_span else transaction.id
             trace_parent = transaction.trace_parent.copy_from(
                 span_id=parent_id, trace_options=TracingOptions(recorded=True)
             )
             self._set_disttracing_headers(params["headers"], trace_parent, transaction)
+            if leaf_span:
+                leaf_span.dist_tracing_propagated = True
 
             response, content = wrapped(*args, **kwargs)
             if span.context:
                 span.context["http"]["status_code"] = response.status
             span.set_success() if response.status < 400 else span.set_failure()
             return response, content
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/httpx.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/sync/httpx.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,36 +26,35 @@
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
 from elasticapm.traces import capture_span
-from elasticapm.utils import get_host_from_url, sanitize_url, url_to_destination
+from elasticapm.utils import get_host_from_url, sanitize_url
 
 
 class HttpxClientInstrumentation(AbstractInstrumentedModule):
     name = "httpx"
 
     instrument_list = [("httpx", "Client.send")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
-        request = kwargs.get("request", args[0])
+        request = kwargs.get("request") or args[0]
 
         request_method = request.method.upper()
         url = str(request.url)
         name = "{request_method} {host}".format(request_method=request_method, host=get_host_from_url(url))
         url = sanitize_url(url)
-        destination = url_to_destination(url)
 
         with capture_span(
             name,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
             response = wrapped(*args, **kwargs)
             if response is not None:
                 if span.context:
                     span.context["http"]["status_code"] = response.status_code
                 span.set_success() if response.status_code < 400 else span.set_failure()
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/jinja2.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/jinja2.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/mysql.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,10 +53,9 @@
 
     instrument_list = [("MySQLdb", "connect")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         destination_info = {
             "address": args[0] if len(args) else kwargs.get("host", "localhost"),
             "port": args[4] if len(args) > 4 else int(kwargs.get("port", default_ports.get("mysql"))),
-            "service": {"name": "mysql", "resource": "mysql", "type": "db"},
         }
         return MySQLConnectionProxy(wrapped(*args, **kwargs), destination_info=destination_info)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/mysql_connector.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/mysql_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,10 +54,9 @@
 
     instrument_list = [("mysql.connector", "connect")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         destination_info = {
             "address": kwargs.get("host", "localhost"),
             "port": int(kwargs.get("port", default_ports.get("mysql"))),
-            "service": {"name": "mysql", "resource": "mysql", "type": "db"},
         }
         return MySQLConnectionProxy(wrapped(*args, **kwargs), destination_info=destination_info)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/psycopg2.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/psycopg2.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from __future__ import absolute_import
 
+from typing import Optional, Union
+
 from elasticapm.instrumentation.packages.dbapi2 import (
     ConnectionProxy,
     CursorProxy,
     DbApi2Instrumentation,
     extract_signature,
 )
 from elasticapm.traces import capture_span
@@ -72,31 +74,19 @@
     name = "psycopg2"
 
     instrument_list = [("psycopg2", "connect")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         signature = "psycopg2.connect"
 
-        host = kwargs.get("host")
-        if host:
-            signature += " " + compat.text_type(host)
-
-            port = kwargs.get("port")
-            if port:
-                port = str(port)
-                if int(port) != default_ports.get("postgresql"):
-                    host += ":" + port
-            signature += " " + compat.text_type(host)
-        else:
-            # Parse connection string and extract host/port
-            pass
+        host, port = get_destination_info(kwargs.get("host"), kwargs.get("port"))
+        signature = f"{signature} {host}:{port}"
         destination_info = {
-            "address": kwargs.get("host", "localhost"),
-            "port": int(kwargs.get("port", default_ports.get("postgresql"))),
-            "service": {"name": "postgresql", "resource": "postgresql", "type": "db"},
+            "address": host,
+            "port": port,
         }
         with capture_span(
             signature,
             span_type="db",
             span_subtype="postgresql",
             span_action="connect",
             extra={"destination": destination_info},
@@ -137,7 +127,23 @@
             # connection/cursor is either 3rd argument, or "scope" keyword argument
             if len(args) >= 3 and hasattr(args[2], "__wrapped__"):
                 args = args[:2] + (args[2].__wrapped__,) + args[3:]
             elif "scope" in kwargs and hasattr(kwargs["scope"], "__wrapped__"):
                 kwargs["scope"] = kwargs["scope"].__wrapped__
 
         return wrapped(*args, **kwargs)
+
+
+def get_destination_info(host: Optional[str], port: Union[None, str, int]) -> tuple:
+    if host:
+        if "," in host:  # multiple hosts defined, take first
+            host = host.split(",")[0]
+    else:
+        host = "localhost"
+    if port:
+        port = str(port)
+        if "," in port:  # multiple ports defined, take first
+            port = port.split(",")[0]
+        port = int(port)
+    else:
+        port = default_ports.get("postgresql")
+    return host, port
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pylibmc.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pylibmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         wrapped_name = self.get_wrapped_name(wrapped, instance, method)
         address, port = get_address_port_from_instance(instance)
         destination = {
             "address": address,
             "port": port,
-            "service": {"name": "memcached", "resource": "memcached", "type": "cache"},
         }
         with capture_span(
             wrapped_name,
             span_type="cache",
             span_subtype="memcached",
             span_action="query",
             extra={"destination": destination},
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymemcache.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymemcache.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,14 @@
                 address, port = instance.server
             else:
                 # Server is a UNIX domain socket
                 address = instance.server
         destination = {
             "address": address,
             "port": port,
-            "service": {"name": "memcached", "resource": "memcached", "type": "cache"},
         }
 
         if "PooledClient" in name:
             # PooledClient calls out to Client for the "work", but only once,
             # so we don't care about the "duplicate" spans from Client in that
             # case
             with capture_span(
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymongo.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymongo.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 class PyMongoInstrumentation(AbstractInstrumentedModule):
     name = "pymongo"
 
     instrument_list = [
         ("pymongo.collection", "Collection.aggregate"),
         ("pymongo.collection", "Collection.bulk_write"),
         ("pymongo.collection", "Collection.count"),
+        ("pymongo.collection", "Collection.count_documents"),
+        ("pymongo.collection", "Collection.estimated_document_count"),
         ("pymongo.collection", "Collection.create_index"),
         ("pymongo.collection", "Collection.create_indexes"),
         ("pymongo.collection", "Collection.delete_many"),
         ("pymongo.collection", "Collection.delete_one"),
         ("pymongo.collection", "Collection.distinct"),
         ("pymongo.collection", "Collection.drop"),
         ("pymongo.collection", "Collection.drop_index"),
@@ -76,15 +78,14 @@
         if nodes:
             host, port = list(nodes)[0]
         else:
             host, port = None, None
         destination_info = {
             "address": host,
             "port": port,
-            "service": {"name": "mongodb", "resource": "mongodb", "type": "db"},
         }
         with capture_span(
             signature,
             span_type="db",
             span_subtype="mongodb",
             span_action="query",
             leaf=True,
@@ -102,15 +103,15 @@
         collection = instance._BulkOperationBuilder__bulk.collection
         signature = ".".join([collection.full_name, "bulk.execute"])
         with capture_span(
             signature,
             span_type="db",
             span_subtype="mongodb",
             span_action="query",
-            extra={"destination": {"service": {"name": "mongodb", "resource": "mongodb", "type": "db"}}},
+            extra={"destination": {}},
         ):
             return wrapped(*args, **kwargs)
 
 
 class PyMongoCursorInstrumentation(AbstractInstrumentedModule):
     name = "pymongo"
 
@@ -120,15 +121,15 @@
         collection = instance.collection
         signature = ".".join([collection.full_name, "cursor.refresh"])
         with capture_span(
             signature,
             span_type="db",
             span_subtype="mongodb",
             span_action="query",
-            extra={"destination": {"service": {"name": "mongodb", "resource": "mongodb", "type": "db"}}},
+            extra={"destination": {}},
         ) as span:
             response = wrapped(*args, **kwargs)
             if span.context and instance.address:
                 host, port = instance.address
                 span.context["destination"]["address"] = host
                 span.context["destination"]["port"] = port
             else:
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymssql.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymssql.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     instrument_list = [("pymssql", "connect")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         host, port = get_host_port(args, kwargs)
         destination_info = {
             "address": host,
             "port": port,
-            "service": {"name": "mssql", "resource": "mssql", "type": "db"},
         }
         return PyMSSQLConnectionProxy(wrapped(*args, **kwargs), destination_info=destination_info)
 
 
 def get_host_port(args, kwargs):
     host = args[0] if args else kwargs.get("server")
     port = None
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pymysql.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pymysql.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/pyodbc.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/pyodbc.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/python_memcached.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/python_memcached.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import socket
 
 from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
 from elasticapm.traces import capture_span
 
 
 class PythonMemcachedInstrumentation(AbstractInstrumentedModule):
     name = "python_memcached"
@@ -62,17 +63,20 @@
     def get_instrument_list(self):
         return [("memcache", "Client." + method) for method in self.method_list]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         name = self.get_wrapped_name(wrapped, instance, method)
         address, port = None, None
         if instance.servers:
-            address, port = instance.servers[0].address
+            first_server = instance.servers[0]
+            if first_server.family == socket.AF_UNIX:
+                address = first_server.address
+            else:
+                address, port = first_server.address
         destination = {
             "address": address,
             "port": port,
-            "service": {"name": "memcached", "resource": "memcached", "type": "cache"},
         }
         with capture_span(
             name, span_type="cache", span_subtype="memcached", span_action="query", extra={"destination": destination}
         ):
             return wrapped(*args, **kwargs)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/redis.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,17 +55,18 @@
     # no need to instrument StrictRedis in redis-py >= 3.0
     instrument_list_3 = [("redis.client", "Redis.execute_command"), ("redis.client", "PubSub.execute_command")]
     instrument_list = [("redis.client", "Redis.execute_command"), ("redis.client", "StrictRedis.execute_command")]
 
     def call(self, module, method, wrapped, instance, args, kwargs):
         if len(args) > 0:
             wrapped_name = str(args[0])
+            if len(args) >= 2:
+                wrapped_name += ': {}'.format(args[1])
         else:
             wrapped_name = self.get_wrapped_name(wrapped, instance, method)
-
         with capture_span(wrapped_name, span_type="db", span_subtype="redis", span_action="query", leaf=True):
             return wrapped(*args, **kwargs)
 
 
 class RedisPipelineInstrumentation(Redis3CheckMixin, AbstractInstrumentedModule):
     name = "redis"
 
@@ -88,15 +89,15 @@
         span = execution_context.get_span()
         if span and span.subtype == "redis":
             span.context["destination"] = get_destination_info(instance)
         return wrapped(*args, **kwargs)
 
 
 def get_destination_info(connection):
-    destination_info = {"service": {"name": "redis", "resource": "redis", "type": "db"}}
+    destination_info = {}
     if hasattr(connection, "port"):
         destination_info["port"] = connection.port
         destination_info["address"] = connection.host
     elif hasattr(connection, "path"):
         destination_info["port"] = None
         destination_info["address"] = "unix://" + connection.path
     return destination_info
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/requests.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
 from elasticapm.traces import capture_span
-from elasticapm.utils import get_host_from_url, sanitize_url, url_to_destination
+from elasticapm.utils import get_host_from_url, sanitize_url
 
 
 class RequestsInstrumentation(AbstractInstrumentedModule):
     name = "requests"
 
     instrument_list = [("requests.sessions", "Session.send")]
 
@@ -43,21 +43,20 @@
             request = kwargs["request"]
         else:
             request = args[0]
 
         signature = request.method.upper()
         signature += " " + get_host_from_url(request.url)
         url = sanitize_url(request.url)
-        destination = url_to_destination(url)
 
         with capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
             response = wrapped(*args, **kwargs)
             # requests.Response objects are falsy if status code > 400, so we have to check for None instead
             if response is not None:
                 if span.context:
                     span.context["http"]["status_code"] = response.status_code
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/sqlite.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/sqlite.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/tornado.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/tornado.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/urllib.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/httpx/async/httpcore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  BSD 3-Clause License
 #
-#  Copyright (c) 2019, Elasticsearch BV
+#  Copyright (c) 2021, Elasticsearch BV
 #  All rights reserved.
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are met:
 #
 #  * Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -24,100 +24,81 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-
-from elasticapm.conf import constants
-from elasticapm.instrumentation.packages.base import AbstractInstrumentedModule
-from elasticapm.traces import DroppedSpan, capture_span, execution_context
-from elasticapm.utils import compat, default_ports, sanitize_url, url_to_destination
+from elasticapm.contrib.asyncio.traces import async_capture_span
+from elasticapm.instrumentation.packages.asyncio.base import AsyncAbstractInstrumentedModule
+from elasticapm.instrumentation.packages.httpx import utils
+from elasticapm.traces import DroppedSpan, execution_context
+from elasticapm.utils import default_ports
 from elasticapm.utils.disttracing import TracingOptions
 
 
-# copied and adapted from urllib.request
-def request_host(request):
-    """Return request-host, as defined by RFC 2965.
+class HTTPCoreAsyncInstrumentation(AsyncAbstractInstrumentedModule):
+    """
+    This instrumentation only exists to make sure we add distributed tracing
+    headers on our requests from `httpx`. `httpx` is the only place this library
+    is used, so no spans will actually be created (due to already being in
+    a leaf span). However, the rest of the logic was left in (much of this
+    mirrors the urllib3 instrumentation) in case that situation ever changes.
+    """
 
-    Variation from RFC: returned value is lowercased, for convenient
-    comparison.
+    name = "httpcore"
 
-    """
-    url = request.get_full_url()
-    parse_result = compat.urlparse.urlparse(url)
-    scheme, host, port = parse_result.scheme, parse_result.hostname, parse_result.port
-    try:
-        port = int(port)
-    except (ValueError, TypeError):
-        pass
-    if host == "":
-        host = request.get_header("Host", "")
-
-    if port and port != default_ports.get(scheme):
-        host = "%s:%s" % (host, port)
-    return host
-
-
-class UrllibInstrumentation(AbstractInstrumentedModule):
-    name = "urllib"
-
-    if compat.PY2:
-        instrument_list = [("urllib2", "AbstractHTTPHandler.do_open")]
-    else:
-        instrument_list = [("urllib.request", "AbstractHTTPHandler.do_open")]
-
-    def call(self, module, method, wrapped, instance, args, kwargs):
-        request_object = args[1] if len(args) > 1 else kwargs["req"]
-
-        method = request_object.get_method()
-        host = request_host(request_object)
-
-        url = sanitize_url(request_object.get_full_url())
-        destination = url_to_destination(url)
-        signature = method.upper() + " " + host
+    instrument_list = [
+        ("httpcore._async.connection", "AsyncHTTPConnection.request"),  # < httpcore 0.11
+        ("httpcore._async.connection", "AsyncHTTPConnection.arequest"),  # httpcore 0.11 - 0.12
+        ("httpcore._async.connection", "AsyncHTTPConnection.handle_async_request"),  # >= httpcore 0.13
+    ]
+
+    async def call(self, module, method, wrapped, instance, args, kwargs):
+        url, method, headers = utils.get_request_data(args, kwargs)
+        scheme, host, port, target = url
+
+        if port != default_ports.get(scheme):
+            host += ":" + str(port)
+
+        signature = "%s %s" % (method.upper(), host)
+
+        url = "%s://%s%s" % (scheme, host, url)
 
         transaction = execution_context.get_transaction()
 
-        with capture_span(
+        async with async_capture_span(
             signature,
             span_type="external",
             span_subtype="http",
-            extra={"http": {"url": url}, "destination": destination},
+            extra={"http": {"url": url}},
             leaf=True,
         ) as span:
-            # if urllib has been called in a leaf span, this span might be a DroppedSpan.
+            # if httpcore has been called in a leaf span, this span might be a DroppedSpan.
             leaf_span = span
             while isinstance(leaf_span, DroppedSpan):
                 leaf_span = leaf_span.parent
 
-            parent_id = leaf_span.id if leaf_span else transaction.id
-            trace_parent = transaction.trace_parent.copy_from(
-                span_id=parent_id, trace_options=TracingOptions(recorded=True)
-            )
-            self._set_disttracing_headers(request_object, trace_parent, transaction)
-            response = wrapped(*args, **kwargs)
-            if response:
-                status = getattr(response, "status", None) or response.getcode()  # Python 2 compat
+            if headers is not None:
+                # It's possible that there are only dropped spans, e.g. if we started dropping spans due to the
+                # transaction_max_spans limit. In this case, the transaction.id is used
+                parent_id = leaf_span.id if leaf_span else transaction.id
+                trace_parent = transaction.trace_parent.copy_from(
+                    span_id=parent_id, trace_options=TracingOptions(recorded=True)
+                )
+                utils.set_disttracing_headers(headers, trace_parent, transaction)
+            response = await wrapped(*args, **kwargs)
+            status_code = utils.get_status(response)
+            if status_code:
                 if span.context:
-                    span.context["http"]["status_code"] = status
-                span.set_success() if status < 400 else span.set_failure()
+                    span.context["http"]["status_code"] = status_code
+                span.set_success() if status_code < 400 else span.set_failure()
             return response
 
     def mutate_unsampled_call_args(self, module, method, wrapped, instance, args, kwargs, transaction):
-        request_object = args[1] if len(args) > 1 else kwargs["req"]
         # since we don't have a span, we set the span id to the transaction id
         trace_parent = transaction.trace_parent.copy_from(
             span_id=transaction.id, trace_options=TracingOptions(recorded=False)
         )
-
-        self._set_disttracing_headers(request_object, trace_parent, transaction)
+        headers = utils.get_request_data(args, kwargs)[2]
+        utils.set_disttracing_headers(headers, trace_parent, transaction)
         return args, kwargs
-
-    def _set_disttracing_headers(self, request_object, trace_parent, transaction):
-        trace_parent_str = trace_parent.to_string()
-        request_object.add_header(constants.TRACEPARENT_HEADER_NAME, trace_parent_str)
-        if transaction.tracer.config.use_elastic_traceparent_header:
-            request_object.add_header(constants.TRACEPARENT_LEGACY_HEADER_NAME, trace_parent_str)
-        if trace_parent.tracestate:
-            request_object.add_header(constants.TRACESTATE_HEADER_NAME, trace_parent.tracestate)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/packages/zlib.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/packages/zlib.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/instrumentation/register.py` & `sf-elastic-apm-6.7.2/elasticapm/instrumentation/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import sys
 
 from elasticapm.utils.module_import import import_string
 
 _cls_register = {
     "elasticapm.instrumentation.packages.botocore.BotocoreInstrumentation",
-    "elasticapm.instrumentation.packages.httpx.HttpxClientInstrumentation",
+    "elasticapm.instrumentation.packages.httpx.sync.httpx.HttpxClientInstrumentation",
     "elasticapm.instrumentation.packages.jinja2.Jinja2Instrumentation",
     "elasticapm.instrumentation.packages.psycopg2.Psycopg2Instrumentation",
     "elasticapm.instrumentation.packages.psycopg2.Psycopg2ExtensionsInstrumentation",
     "elasticapm.instrumentation.packages.mysql.MySQLInstrumentation",
     "elasticapm.instrumentation.packages.mysql_connector.MySQLConnectorInstrumentation",
     "elasticapm.instrumentation.packages.pymysql.PyMySQLConnectorInstrumentation",
     "elasticapm.instrumentation.packages.pylibmc.PyLibMcInstrumentation",
@@ -59,32 +59,33 @@
     "elasticapm.instrumentation.packages.pymssql.PyMSSQLInstrumentation",
     "elasticapm.instrumentation.packages.pyodbc.PyODBCInstrumentation",
     "elasticapm.instrumentation.packages.django.template.DjangoTemplateInstrumentation",
     "elasticapm.instrumentation.packages.django.template.DjangoTemplateSourceInstrumentation",
     "elasticapm.instrumentation.packages.urllib.UrllibInstrumentation",
     "elasticapm.instrumentation.packages.graphql.GraphQLExecutorInstrumentation",
     "elasticapm.instrumentation.packages.graphql.GraphQLBackendInstrumentation",
-    "elasticapm.instrumentation.packages.httpcore.HTTPCoreInstrumentation",
+    "elasticapm.instrumentation.packages.httpx.sync.httpcore.HTTPCoreInstrumentation",
     "elasticapm.instrumentation.packages.httplib2.Httplib2Instrumentation",
+    "elasticapm.instrumentation.packages.azure.AzureInstrumentation",
 }
 
 if sys.version_info >= (3, 7):
     _cls_register.update(
         [
             "elasticapm.instrumentation.packages.asyncio.sleep.AsyncIOSleepInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aiohttp_client.AioHttpClientInstrumentation",
-            "elasticapm.instrumentation.packages.asyncio.httpx.HttpxAsyncClientInstrumentation",
+            "elasticapm.instrumentation.packages.httpx.async.httpx.HttpxAsyncClientInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.elasticsearch.ElasticSearchAsyncConnection",
             "elasticapm.instrumentation.packages.asyncio.elasticsearch.ElasticsearchAsyncTransportInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aiopg.AioPGInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.asyncpg.AsyncPGInstrumentation",
             "elasticapm.instrumentation.packages.tornado.TornadoRequestExecuteInstrumentation",
             "elasticapm.instrumentation.packages.tornado.TornadoHandleRequestExceptionInstrumentation",
             "elasticapm.instrumentation.packages.tornado.TornadoRenderInstrumentation",
-            "elasticapm.instrumentation.packages.asyncio.httpcore.HTTPCoreAsyncInstrumentation",
+            "elasticapm.instrumentation.packages.httpx.async.httpcore.HTTPCoreAsyncInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aioredis.RedisConnectionPoolInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aioredis.RedisPipelineInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aioredis.RedisConnectionInstrumentation",
             "elasticapm.instrumentation.packages.asyncio.aiomysql.AioMySQLInstrumentation",
         ]
     )
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/base_metrics.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/breakdown.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/breakdown.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu_linux.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu_linux.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/cpu_psutil.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/cpu_psutil.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/prometheus.py` & `sf-elastic-apm-6.7.2/elasticapm/metrics/sets/prometheus.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         counts = []
         values = []
         name = self._registry.client.config.prometheus_metrics_prefix + name
         while sample_pos < len(samples):
             sample = samples[sample_pos]
             if "le" in sample.labels:
                 values.append(float(sample.labels["le"]))
-                counts.append(sample.value - prev_val)
+                counts.append(int(sample.value - prev_val))
                 prev_val = sample.value
                 sample_pos += 1
 
             else:
                 # we reached the end of one set of buckets/values, this is the "count" sample
                 self.histogram(name, unit=unit, buckets=values, **sample.labels).val = counts
                 prev_val = 0
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/metrics/sets/transactions.py` & `sf-elastic-apm-6.7.2/elasticapm/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,9 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from __future__ import absolute_import
-
-from elasticapm.metrics.base_metrics import SpanBoundMetricSet
-
-
-class TransactionsMetricSet(SpanBoundMetricSet):
-    pass
+__version__ = (6, 7, 2)
+VERSION = ".".join(map(str, __version__))
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/middleware.py` & `sf-elastic-apm-6.7.2/elasticapm/middleware.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/processors.py` & `sf-elastic-apm-6.7.2/elasticapm/processors.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/traces.py` & `sf-elastic-apm-6.7.2/elasticapm/traces.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,82 +31,104 @@
 import functools
 import random
 import re
 import threading
 import time
 import timeit
 from collections import defaultdict
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 from elasticapm.conf import constants
 from elasticapm.conf.constants import LABEL_RE, SPAN, TRANSACTION
 from elasticapm.context import init_execution_context
 from elasticapm.metrics.base_metrics import Timer
-from elasticapm.utils import compat, encoding, get_name_from_func
+from elasticapm.utils import compat, encoding, get_name_from_func, nested_key, url_to_destination_resource
 from elasticapm.utils.disttracing import TraceParent, TracingOptions
 from elasticapm.utils.logging import get_logger
-import sys
-if sys.version_info[0] < 3:
-   import base
-else:
-   from elasticapm import base
+from elasticapm import base
 
+from elasticapm.utils.time import time_to_perf_counter
 
 __all__ = ("capture_span", "label", "set_transaction_name", "set_custom_context", "set_user_context")
 
 error_logger = get_logger("elasticapm.errors")
 logger = get_logger("elasticapm.traces")
 
 _time_func = timeit.default_timer
 
 
 execution_context = init_execution_context()
 
+SpanType = Union["Span", "DroppedSpan"]
+
 
 class ChildDuration(object):
     __slots__ = ("obj", "_nesting_level", "_start", "_duration", "_lock")
 
-    def __init__(self, obj):
+    def __init__(self, obj: "BaseSpan"):
         self.obj = obj
-        self._nesting_level = 0
-        self._start = None
-        self._duration = 0
+        self._nesting_level: int = 0
+        self._start: float = 0
+        self._duration: float = 0
         self._lock = threading.Lock()
 
-    def start(self, timestamp):
+    def start(self, timestamp: float):
         with self._lock:
             self._nesting_level += 1
             if self._nesting_level == 1:
                 self._start = timestamp
 
-    def stop(self, timestamp):
+    def stop(self, timestamp: float):
         with self._lock:
             self._nesting_level -= 1
             if self._nesting_level == 0:
                 self._duration += timestamp - self._start
 
     @property
-    def duration(self):
+    def duration(self) -> float:
         return self._duration
 
 
 class BaseSpan(object):
-    def __init__(self, labels=None):
+    def __init__(self, labels=None, start=None):
         self._child_durations = ChildDuration(self)
         self.labels = {}
-        self.outcome = None
+        self.outcome: Optional[str] = None
+        self.compression_buffer: Optional[Union[Span, DroppedSpan]] = None
+        self.compression_buffer_lock = threading.Lock()
+        self.start_time: float = time_to_perf_counter(start) if start is not None else _time_func()
+        self.ended_time: Optional[float] = None
+        self.duration: Optional[float] = None
         if labels:
             self.label(**labels)
 
     def child_started(self, timestamp):
         self._child_durations.start(timestamp)
 
-    def child_ended(self, timestamp):
-        self._child_durations.stop(timestamp)
+    def child_ended(self, child: SpanType):
+        with self.compression_buffer_lock:
+            if not child.is_compression_eligible():
+                if self.compression_buffer:
+                    self.compression_buffer.report()
+                    self.compression_buffer = None
+                child.report()
+            elif self.compression_buffer is None:
+                self.compression_buffer = child
+            elif not self.compression_buffer.try_to_compress(child):
+                self.compression_buffer.report()
+                self.compression_buffer = child
+
+    def end(self, skip_frames: int = 0, duration: Optional[float] = None):
+        self.ended_time = _time_func()
+        self.duration = duration if duration is not None else (self.ended_time - self.start_time)
+        if self.compression_buffer:
+            self.compression_buffer.report()
+            self.compression_buffer = None
 
-    def end(self, skip_frames=0, duration=None):
+    def to_dict(self) -> dict:
         raise NotImplementedError()
 
     def label(self, **labels):
         """
         Label this span with one or multiple key/value labels. Keys should be strings, values can be strings, booleans,
         or numerical values (int, float, Decimal)
 
@@ -117,71 +139,91 @@
         :param labels: key/value pairs of labels
         :return: None
         """
         labels = encoding.enforce_label_format(labels)
         self.labels.update(labels)
 
     def set_success(self):
-        self.outcome = "success"
+        self.outcome = constants.OUTCOME.SUCCESS
 
     def set_failure(self):
-        self.outcome = "failure"
+        self.outcome = constants.OUTCOME.FAILURE
 
     @staticmethod
-    def get_dist_tracing_id():
+    def get_dist_tracing_id() -> str:
         return "%016x" % random.getrandbits(64)
 
+    @property
+    def tracer(self) -> "Tracer":
+        raise NotImplementedError()
+
 
 class Transaction(BaseSpan):
     def __init__(
-        self, tracer, transaction_type="custom", trace_parent=None, is_sampled=True, start=None, sample_rate=None
+        self,
+        tracer: "Tracer",
+        transaction_type: str = "custom",
+        trace_parent: Optional[TraceParent] = None,
+        is_sampled: bool = True,
+        start: Optional[float] = None,
+        sample_rate: Optional[float] = None,
     ):
+        """
+        tracer
+            Tracer object
+        transaction_type
+            Transaction type
+        trace_parent
+            TraceParent object representing the parent trace and trace state
+        is_sampled
+            Whether or not this transaction is sampled
+        start
+            Optional start timestamp. This is expected to be an epoch timestamp
+            in seconds (such as from `time.time()`). If it is not, it's recommended
+            that a `duration` is passed into the `end()` method.
+        sample_rate
+            Sample rate which was used to decide whether to sample this transaction.
+            This is reported to the APM server so that unsampled transactions can
+            be extrapolated.
+        """
         self.id = self.get_dist_tracing_id()
-        self.trace_parent = trace_parent
-        if start:
-            self.timestamp = self.start_time = start
-        else:
-            self.timestamp, self.start_time = time.time(), _time_func()
-        self.name = None
-        self.duration = None
-        self.result = None
+        if not trace_parent:
+            trace_parent = TraceParent(
+                constants.TRACE_CONTEXT_VERSION,
+                "%032x" % random.getrandbits(128),
+                self.id,
+                TracingOptions(recorded=is_sampled),
+            )
+
+        self.trace_parent: TraceParent = trace_parent
+        self.timestamp = start if start is not None else time.time()
+        self.name: Optional[str] = None
+        self.result: Optional[str] = None
         self.transaction_type = transaction_type
-        self.tracer = tracer
+        self._tracer = tracer
 
-        self.dropped_spans = 0
-        self.context = {}
+        self.dropped_spans: int = 0
+        self.context: Dict[str, Any] = {}
 
         self._is_sampled = is_sampled
         self.sample_rate = sample_rate
-        self._span_counter = 0
-        self._span_timers = defaultdict(Timer)
+        self._span_counter: int = 0
+        self._span_timers: Dict[Tuple[str, str], Timer] = defaultdict(Timer)
         self._span_timers_lock = threading.Lock()
+        self._dropped_span_statistics = defaultdict(lambda: {"count": 0, "duration.sum.us": 0})
         try:
             self._breakdown = self.tracer._agent._metrics.get_metricset(
                 "elasticapm.metrics.sets.breakdown.BreakdownMetricSet"
             )
         except (LookupError, AttributeError):
             self._breakdown = None
-        try:
-            self._transaction_metrics = self.tracer._agent._metrics.get_metricset(
-                "elasticapm.metrics.sets.transactions.TransactionsMetricSet"
-            )
-        except (LookupError, AttributeError):
-            self._transaction_metrics = None
-        super(Transaction, self).__init__()
+        super(Transaction, self).__init__(start=start)
 
-    def end(self, skip_frames=0, duration=None):
-        self.duration = duration if duration is not None else (_time_func() - self.start_time)
-        if self._transaction_metrics:
-            self._transaction_metrics.timer(
-                "transaction.duration",
-                reset_on_collect=True,
-                unit="us",
-                **{"transaction.name": self.name, "transaction.type": self.transaction_type}
-            ).update(int(self.duration * 1000000))
+    def end(self, skip_frames: int = 0, duration: Optional[float] = None):
+        super().end(skip_frames, duration)
         if self._breakdown:
             for (span_type, span_subtype), timer in compat.iteritems(self._span_timers):
                 labels = {
                     "span.type": span_type,
                     "transaction.name": self.name,
                     "transaction.type": self.transaction_type,
                 }
@@ -189,20 +231,19 @@
                     labels["span.subtype"] = span_subtype
                 val = timer.val
                 self._breakdown.timer("span.self_time", reset_on_collect=True, unit="us", **labels).update(
                     int(val[0] * 1000000), val[1]
                 )
             labels = {"transaction.name": self.name, "transaction.type": self.transaction_type}
             if self.is_sampled:
-                self._breakdown.counter("transaction.breakdown.count", reset_on_collect=True, **labels).inc()
                 self._breakdown.timer(
                     "span.self_time",
                     reset_on_collect=True,
                     unit="us",
-                    **{"span.type": "app", "transaction.name": self.name, "transaction.type": self.transaction_type}
+                    **{"span.type": "app", "transaction.name": self.name, "transaction.type": self.transaction_type},
                 ).update(int((self.duration - self._child_durations.duration) * 1000000))
 
     def _begin_span(
         self,
         name,
         span_type,
         context=None,
@@ -216,16 +257,15 @@
     ):
         parent_span = execution_context.get_span()
         tracer = self.tracer
         if parent_span and parent_span.leaf:
             span = DroppedSpan(parent_span, leaf=True)
         elif tracer.config.transaction_max_spans and self._span_counter > tracer.config.transaction_max_spans - 1:
             self.dropped_spans += 1
-            span = DroppedSpan(parent_span)
-            self._span_counter += 1
+            span = DroppedSpan(parent_span, context=context)
         else:
             span = Span(
                 transaction=self,
                 name=name,
                 span_type=span_type or "code.custom",
                 context=context,
                 leaf=leaf,
@@ -276,15 +316,15 @@
             parent_span_id=None,
             span_subtype=span_subtype,
             span_action=span_action,
             sync=sync,
             start=start,
         )
 
-    def end_span(self, skip_frames=0, duration=None, outcome="unknown"):
+    def end_span(self, skip_frames: int = 0, duration: Optional[float] = None, outcome: str = "unknown"):
         """
         End the currently active span
         :param skip_frames: numbers of frames to skip in the stack trace
         :param duration: override duration, mostly useful for testing
         :param outcome: outcome of the span, either success, failure or unknown
         :return: the ended span
         """
@@ -295,58 +335,70 @@
         # only overwrite span outcome if it is still unknown
         if not span.outcome or span.outcome == "unknown":
             span.outcome = outcome
 
         span.end(skip_frames=skip_frames, duration=duration)
         return span
 
-    def ensure_parent_id(self):
+    def ensure_parent_id(self) -> str:
         """If current trace_parent has no span_id, generate one, then return it
 
         This is used to generate a span ID which the RUM agent will use to correlate
         the RUM transaction with the backend transaction.
         """
         if self.trace_parent.span_id == self.id:
             self.trace_parent.span_id = "%016x" % random.getrandbits(64)
             logger.debug("Set parent id to generated %s", self.trace_parent.span_id)
         return self.trace_parent.span_id
 
-    def to_dict(self):
+    def to_dict(self) -> dict:
         self.context["tags"] = self.labels
         result = {
             "id": self.id,
             "trace_id": self.trace_parent.trace_id,
             "name": encoding.keyword_field(self.name or ""),
             "type": encoding.keyword_field(self.transaction_type),
             "duration": self.duration * 1000,  # milliseconds
             "result": encoding.keyword_field(str(self.result)),
             "timestamp": int(self.timestamp * 1000000),  # microseconds
             "outcome": self.outcome,
             "sampled": self.is_sampled,
-            "span_count": {"started": self._span_counter - self.dropped_spans, "dropped": self.dropped_spans},
+            "span_count": {"started": self._span_counter, "dropped": self.dropped_spans},
         }
+        if self._dropped_span_statistics:
+            result["dropped_spans_stats"] = [
+                {
+                    "destination_service_resource": resource,
+                    "outcome": outcome,
+                    "duration": {"count": v["count"], "sum": {"us": int(v["duration.sum.us"] * 1000000)}},
+                }
+                for (resource, outcome), v in self._dropped_span_statistics.items()
+            ]
         if self.sample_rate is not None:
             result["sample_rate"] = float(self.sample_rate)
         if self.trace_parent:
             result["trace_id"] = self.trace_parent.trace_id
             # only set parent_id if this transaction isn't the root
             if self.trace_parent.span_id and self.trace_parent.span_id != self.id:
                 result["parent_id"] = self.trace_parent.span_id
+        # faas context belongs top-level on the transaction
+        if "faas" in self.context:
+            result["faas"] = self.context.pop("faas")
         if self.is_sampled:
             result["context"] = self.context
         return result
 
     def track_span_duration(self, span_type, span_subtype, self_duration):
         # TODO: once asynchronous spans are supported, we should check if the transaction is already finished
         # TODO: and, if it has, exit without tracking.
         with self._span_timers_lock:
             self._span_timers[(span_type, span_subtype)].update(self_duration)
 
     @property
-    def is_sampled(self):
+    def is_sampled(self) -> bool:
         return self._is_sampled
 
     @is_sampled.setter
     def is_sampled(self, is_sampled):
         """
         This should never be called in normal operation, but often is used
         for testing. We just want to make sure our sample_rate comes out correctly
@@ -354,51 +406,57 @@
         """
         self._is_sampled = is_sampled
         if not is_sampled:
             if self.sample_rate:
                 self.sample_rate = "0"
                 self.trace_parent.add_tracestate(constants.TRACESTATE.SAMPLE_RATE, self.sample_rate)
 
+    @property
+    def tracer(self) -> "Tracer":
+        return self._tracer
+
 
 class Span(BaseSpan):
     __slots__ = (
         "id",
         "transaction",
         "name",
         "type",
         "subtype",
         "action",
         "context",
         "leaf",
+        "dist_tracing_propagated",
         "timestamp",
         "start_time",
+        "ended_time",
         "duration",
         "parent",
         "parent_span_id",
         "frames",
         "labels",
         "sync",
         "outcome",
         "_child_durations",
     )
 
     def __init__(
         self,
-        transaction,
-        name,
-        span_type,
-        context=None,
-        leaf=False,
-        labels=None,
-        parent=None,
-        parent_span_id=None,
-        span_subtype=None,
-        span_action=None,
-        sync=None,
-        start=None,
+        transaction: Transaction,
+        name: str,
+        span_type: str,
+        context: Optional[dict] = None,
+        leaf: bool = False,
+        labels: Optional[dict] = None,
+        parent: Optional["Span"] = None,
+        parent_span_id: Optional[str] = None,
+        span_subtype: Optional[str] = None,
+        span_action: Optional[str] = None,
+        sync: Optional[bool] = None,
+        start: Optional[int] = None,
     ):
         """
         Create a new Span
 
         :param transaction: transaction object that this span relates to
         :param name: Generic name of the span
         :param span_type: type of the span, e.g. db
@@ -407,53 +465,54 @@
         :param labels: a dict of labels
         :param parent_span_id: override of the span ID
         :param span_subtype: sub type of the span, e.g. mysql
         :param span_action: sub type of the span, e.g. query
         :param sync: indicate if the span was executed synchronously or asynchronously
         :param start: timestamp, mostly useful for testing
         """
-        self.start_time = start or _time_func()
         self.id = self.get_dist_tracing_id()
         self.transaction = transaction
         self.name = name
         self.context = context if context is not None else {}
         self.leaf = leaf
         # timestamp is bit of a mix of monotonic and non-monotonic time sources.
         # we take the (non-monotonic) transaction timestamp, and add the (monotonic) difference of span
         # start time and transaction start time. In this respect, the span timestamp is guaranteed to grow
         # monotonically with respect to the transaction timestamp
-        self.timestamp = transaction.timestamp + (self.start_time - transaction.start_time)
-        self.duration = None
         self.parent = parent
         self.parent_span_id = parent_span_id
         self.frames = None
         self.sync = sync
-        if span_subtype is None and "." in span_type:
-            # old style dottet type, let's split it up
-            type_bits = span_type.split(".")
-            if len(type_bits) == 2:
-                span_type, span_subtype = type_bits[:2]
-            else:
-                span_type, span_subtype, span_action = type_bits[:3]
         self.type = span_type
         self.subtype = span_subtype
         self.action = span_action
+        self.dist_tracing_propagated = False
+        self.composite: Dict[str, Any] = {}
+        super(Span, self).__init__(labels=labels, start=start)
+        self.timestamp = transaction.timestamp + (self.start_time - transaction.start_time)
         if self.transaction._breakdown:
             p = self.parent if self.parent else self.transaction
             p.child_started(self.start_time)
-        super(Span, self).__init__(labels=labels)
 
-    def to_dict(self):
+    def to_dict(self) -> dict:
+        if (
+            self.composite
+            and self.composite["compression_strategy"] == "same_kind"
+            and nested_key(self.context, "destination", "service", "resource")
+        ):
+            name = "Calls to " + self.context["destination"]["service"]["resource"]
+        else:
+            name = self.name
         result = {
             "id": self.id,
             "transaction_id": self.transaction.id,
             "trace_id": self.transaction.trace_parent.trace_id,
             # use either the explicitly set parent_span_id, or the id of the parent, or finally the transaction id
             "parent_id": self.parent_span_id or (self.parent.id if self.parent else self.transaction.id),
-            "name": encoding.keyword_field(self.name),
+            "name": encoding.keyword_field(name),
             "type": encoding.keyword_field(self.type),
             "subtype": encoding.keyword_field(self.subtype),
             "action": encoding.keyword_field(self.action),
             "timestamp": int(self.timestamp * 1000000),  # microseconds
             "duration": self.duration * 1000,  # milliseconds
             "outcome": self.outcome,
         }
@@ -462,103 +521,226 @@
         if self.sync is not None:
             result["sync"] = self.sync
         if self.labels:
             if self.context is None:
                 self.context = {}
             self.context["tags"] = self.labels
         if self.context:
+            resource = nested_key(self.context, "destination", "service", "resource")
+            if not resource and (self.leaf or any(k in self.context for k in ("destination", "db", "message", "http"))):
+                type_info = self.subtype or self.type
+                instance = nested_key(self.context, "db", "instance")
+                queue_name = nested_key(self.context, "message", "queue", "name")
+                http_url = nested_key(self.context, "http", "url")
+                if instance:
+                    resource = f"{type_info}/{instance}"
+                elif queue_name:
+                    resource = f"{type_info}/{queue_name}"
+                elif http_url:
+                    resource = url_to_destination_resource(http_url)
+                else:
+                    resource = type_info
+                if "destination" not in self.context:
+                    self.context["destination"] = {}
+                if "service" not in self.context["destination"]:
+                    self.context["destination"]["service"] = {}
+                self.context["destination"]["service"]["resource"] = resource
+                # set fields that are deprecated, but still required by APM Server API
+                if "name" not in self.context["destination"]["service"]:
+                    self.context["destination"]["service"]["name"] = ""
+                if "type" not in self.context["destination"]["service"]:
+                    self.context["destination"]["service"]["type"] = ""
             result["context"] = self.context
         if self.frames:
             result["stacktrace"] = self.frames
+        if self.composite:
+            result["composite"] = {
+                "compression_strategy": self.composite["compression_strategy"],
+                "sum": self.composite["sum"] * 1000,
+                "count": self.composite["count"],
+            }
         return result
 
-    def end(self, skip_frames=0, duration=None):
+    def is_same_kind(self, other_span: SpanType) -> bool:
+        """
+        For compression purposes, two spans are considered to be of the same kind if they have the same
+        values for type, subtype, and destination.service.resource
+        :param other_span: another span object
+        :return: bool
+        """
+        resource = nested_key(self.context, "destination", "service", "resource")
+        return bool(
+            self.type == other_span.type
+            and self.subtype == other_span.subtype
+            and (resource and resource == nested_key(other_span.context, "destination", "service", "resource"))
+        )
+
+    def is_exact_match(self, other_span: SpanType) -> bool:
+        """
+        For compression purposes, two spans are considered to be an exact match if the have the same
+        name and are of the same kind.
+
+        :param other_span: another span object
+        :return: bool
+        """
+        return bool(self.name == other_span.name and self.is_same_kind(other_span))
+
+    def is_compression_eligible(self) -> bool:
+        """
+        Determine if this span is eligible for compression.
+        """
+        if self.tracer.config.span_compression_enabled:
+            return self.leaf and not self.dist_tracing_propagated and self.outcome in (None, constants.OUTCOME.SUCCESS)
+        return False
+
+    def end(self, skip_frames: int = 0, duration: Optional[float] = None):
         """
         End this span and queue it for sending.
 
         :param skip_frames: amount of frames to skip from the beginning of the stack trace
         :param duration: override duration, mostly useful for testing
         :return: None
         """
+        super().end(skip_frames, duration)
         tracer = self.transaction.tracer
-        timestamp = _time_func()
-        self.duration = duration if duration is not None else (timestamp - self.start_time)
         if not tracer.span_frames_min_duration or self.duration >= tracer.span_frames_min_duration and self.frames:
             self.frames = tracer.frames_processing_func(self.frames)[skip_frames:]
         else:
             self.frames = None
         execution_context.set_span(self.parent)
-        tracer.queue_func(SPAN, self.to_dict())
+
+        p = self.parent if self.parent else self.transaction
         if self.transaction._breakdown:
-            p = self.parent if self.parent else self.transaction
-            p.child_ended(self.start_time + self.duration)
+            p._child_durations.stop(self.start_time + self.duration)
             self.transaction.track_span_duration(
                 self.type, self.subtype, self.duration - self._child_durations.duration
             )
+        p.child_ended(self)
+
+    def report(self) -> None:
+        self.tracer.queue_func(SPAN, self.to_dict())
+
+    def try_to_compress(self, sibling: SpanType) -> bool:
+        compression_strategy = (
+            self._try_to_compress_composite(sibling) if self.composite else self._try_to_compress_regular(sibling)
+        )
+        if not compression_strategy:
+            return False
+
+        if not self.composite:
+            self.composite = {"compression_strategy": compression_strategy, "count": 1, "sum": self.duration}
+        self.composite["count"] += 1
+        self.composite["sum"] += sibling.duration
+        self.duration = sibling.ended_time - self.start_time
+        self.transaction._span_counter -= 1
+        return True
+
+    def _try_to_compress_composite(self, sibling: SpanType) -> Optional[str]:
+        if self.composite["compression_strategy"] == "exact_match":
+            return (
+                "exact_match"
+                if (
+                    self.is_exact_match(sibling)
+                    and sibling.duration <= self.transaction.tracer.config.span_compression_exact_match_max_duration
+                )
+                else None
+            )
+        elif self.composite["compression_strategy"] == "same_kind":
+            return (
+                "same_kind"
+                if (
+                    self.is_same_kind(sibling)
+                    and sibling.duration <= self.transaction.tracer.config.span_compression_same_kind_max_duration
+                )
+                else None
+            )
+        return None
+
+    def _try_to_compress_regular(self, sibling: SpanType) -> Optional[str]:
+        if not self.is_same_kind(sibling):
+            return None
+        if self.name == sibling.name:
+            max_duration = self.transaction.tracer.config.span_compression_exact_match_max_duration
+            if self.duration <= max_duration and sibling.duration <= max_duration:
+                return "exact_match"
+            return None
+        max_duration = self.transaction.tracer.config.span_compression_same_kind_max_duration
+        if self.duration <= max_duration and sibling.duration <= max_duration:
+            return "same_kind"
+        return None
 
     def update_context(self, key, data):
         """
         Update the context data for given key
         :param key: the key, e.g. "db"
         :param data: a dictionary
         :return: None
         """
         current = self.context.get(key, {})
         current.update(data)
         self.context[key] = current
 
     def __str__(self):
-        return u"{}/{}/{}".format(self.name, self.type, self.subtype)
+        return "{}/{}/{}".format(self.name, self.type, self.subtype)
+
+    @property
+    def tracer(self) -> "Tracer":
+        return self.transaction.tracer
 
 
 class DroppedSpan(BaseSpan):
-    __slots__ = ("leaf", "parent", "id")
+    __slots__ = ("leaf", "parent", "id", "context", "outcome", "dist_tracing_propagated")
 
-    def __init__(self, parent, leaf=False):
+    def __init__(self, parent, leaf=False, start=None, context=None):
         self.parent = parent
         self.leaf = leaf
         self.id = None
-        super(DroppedSpan, self).__init__()
+        self.dist_tracing_propagated = False
+        self.context = context
+        self.outcome = constants.OUTCOME.UNKNOWN
+        super(DroppedSpan, self).__init__(start=start)
 
-    def end(self, skip_frames=0, duration=None):
+    def end(self, skip_frames: int = 0, duration: Optional[float] = None):
+        super().end(skip_frames, duration)
         execution_context.set_span(self.parent)
 
     def child_started(self, timestamp):
         pass
 
-    def child_ended(self, timestamp):
+    def child_ended(self, child: SpanType):
         pass
 
     def update_context(self, key, data):
         pass
 
+    def report(self):
+        pass
+
+    def try_to_compress(self, sibling: SpanType) -> bool:
+        return False
+
+    def is_compression_eligible(self) -> bool:
+        return False
+
+    @property
+    def name(self):
+        return "DroppedSpan"
+
     @property
     def type(self):
         return None
 
     @property
     def subtype(self):
         return None
 
     @property
     def action(self):
         return None
 
-    @property
-    def context(self):
-        return None
-
-    @property
-    def outcome(self):
-        return "unknown"
-
-    @outcome.setter
-    def outcome(self, value):
-        return
-
 
 class Tracer(object):
     def __init__(self, frames_collector_func, frames_processing_func, queue_func, config, agent):
         self.config = config
         self.queue_func = queue_func
         self.frames_processing_func = frames_processing_func
         self.frames_collector_func = frames_collector_func
@@ -599,20 +781,14 @@
             transaction_type,
             trace_parent=trace_parent,
             is_sampled=is_sampled,
             start=start,
             sample_rate=sample_rate,
         )
         if trace_parent is None:
-            transaction.trace_parent = TraceParent(
-                constants.TRACE_CONTEXT_VERSION,
-                "%032x" % random.getrandbits(128),
-                transaction.id,
-                TracingOptions(recorded=is_sampled),
-            )
             transaction.trace_parent.add_tracestate(constants.TRACESTATE.SAMPLE_RATE, sample_rate)
         execution_context.set_transaction(transaction)
         return transaction
 
     def end_transaction(self, result=None, transaction_name=None, duration=None):
         """
         End the current transaction and queue it for sending
@@ -620,15 +796,15 @@
         :param transaction_name: name of the transaction
         :param duration: override duration, mostly useful for testing
         :return:
         """
         transaction = execution_context.get_transaction(clear=True)
         if transaction:
             if transaction.name is None:
-                transaction.name = transaction_name if transaction_name is not None else ""
+                transaction.name = str(transaction_name) if transaction_name is not None else ""
             transaction.end(duration=duration)
             if self._should_ignore(transaction.name):
                 return
             if transaction.result is None:
                 transaction.result = result
             self.queue_func(TRANSACTION, transaction.to_dict())
         return transaction
@@ -653,70 +829,89 @@
         "duration",
         "start",
         "sync",
     )
 
     def __init__(
         self,
-        name=None,
-        span_type="code.custom",
-        extra=None,
-        skip_frames=0,
-        leaf=False,
-        labels=None,
-        span_subtype=None,
-        span_action=None,
-        start=None,
-        duration=None,
-        sync=None,
+        name: Optional[str] = None,
+        span_type: str = "code.custom",
+        extra: Optional[dict] = None,
+        skip_frames: int = 0,
+        leaf: bool = False,
+        labels: Optional[dict] = None,
+        span_subtype: Optional[str] = None,
+        span_action: Optional[str] = None,
+        start: Optional[int] = None,
+        duration: Optional[int] = None,
+        sync: Optional[bool] = None,
     ):
         self.name = name
+        if span_subtype is None and "." in span_type:
+            # old style dotted type, let's split it up
+            type_bits = span_type.split(".")
+            if len(type_bits) == 2:
+                span_type, span_subtype = type_bits[:2]
+            else:
+                span_type, span_subtype, span_action = type_bits[:3]
         self.type = span_type
         self.subtype = span_subtype
         self.action = span_action
         self.extra = extra
         self.skip_frames = skip_frames
         self.leaf = leaf
         self.labels = labels
         self.start = start
         self.duration = duration
         self.sync = sync
 
-    def __call__(self, func):
+    def __call__(self, func: Callable) -> Callable:
         self.name = self.name or get_name_from_func(func)
 
         @functools.wraps(func)
         def decorated(*args, **kwds):
             with self:
                 return func(*args, **kwds)
 
         return decorated
 
-    def __enter__(self):
+    def __enter__(self) -> Union[Span, DroppedSpan, None]:
         transaction = execution_context.get_transaction()
         if transaction and transaction.is_sampled:
             return transaction.begin_span(
                 self.name,
                 self.type,
                 context=self.extra,
                 leaf=self.leaf,
                 labels=self.labels,
                 span_subtype=self.subtype,
                 span_action=self.action,
                 start=self.start,
                 sync=self.sync,
             )
+        return None
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         transaction = execution_context.get_transaction()
 
         if transaction and transaction.is_sampled:
             try:
                 outcome = "failure" if exc_val else "success"
                 span = transaction.end_span(self.skip_frames, duration=self.duration, outcome=outcome)
+                should_send = (
+                    transaction.tracer._agent.check_server_version(gte=(7, 16)) if transaction.tracer._agent else True
+                )
+                if should_send and isinstance(span, DroppedSpan) and span.context:
+                    try:
+                        resource = span.context["destination"]["service"]["resource"]
+                        stats = transaction._dropped_span_statistics[(resource, span.outcome)]
+                        stats["count"] += 1
+                        stats["duration.sum.us"] += span.duration
+                    except KeyError:
+                        pass
                 if exc_val and not isinstance(span, DroppedSpan):
                     try:
                         exc_val._elastic_apm_span_id = span.id
                         try:
                             # from django.conf import settings
                             # client = base.Client(settings.ELASTIC_APM)
                             client = base.get_client()
@@ -740,35 +935,35 @@
     transaction = execution_context.get_transaction()
     if not transaction:
         error_logger.warning("Ignored labels %s. No transaction currently active.", ", ".join(labels.keys()))
     else:
         transaction.label(**labels)
 
 
-def set_transaction_name(name, override=True):
+def set_transaction_name(name: str, override: bool = True) -> None:
     """
     Sets the name of the transaction
 
     :param name: the name of the transaction
     :param override: if set to False, the name is only set if no name has been set before
     :return: None
     """
     transaction = execution_context.get_transaction()
     if not transaction:
         return
     if transaction.name is None or override:
-        transaction.name = name
+        transaction.name = str(name)
 
 
 def set_transaction_result(result, override=True):
     """
     Sets the result of the transaction. The result could be e.g. the HTTP status class (e.g "HTTP 5xx") for
-    HTTP requests, or "success"/"fail" for background tasks.
+    HTTP requests, or "success"/"failure" for background tasks.
 
-    :param name: the name of the transaction
+    :param result: Details of the transaction result that should be set
     :param override: if set to False, the name is only set if no name has been set before
     :return: None
     """
 
     transaction = execution_context.get_transaction()
     if not transaction:
         return
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/base.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,17 @@
                         )
                 self._flushed.set()
                 return  # time to go home!
 
             if data is not None:
                 data = self._process_event(event_type, data)
                 if data is not None:
+                    if not buffer_written:
+                        # Write metadata just in time to allow for late metadata changes (such as in lambda)
+                        self._write_metadata(buffer)
                     buffer.write((self._json_serializer({event_type: data}) + "\n").encode("utf-8"))
                     buffer_written = True
                     self._counts[event_type] += 1
 
             queue_size = 0 if buffer.fileobj is None else buffer.fileobj.tell()
 
             if flush:
@@ -197,17 +200,38 @@
                         exc_info=True,
                     )
                     return None
         return data
 
     def _init_buffer(self):
         buffer = gzip.GzipFile(fileobj=compat.BytesIO(), mode="w", compresslevel=self._compress_level)
+        return buffer
+
+    def _write_metadata(self, buffer):
         data = (self._json_serializer({"metadata": self._metadata}) + "\n").encode("utf-8")
         buffer.write(data)
-        return buffer
+
+    def add_metadata(self, data):
+        """
+        Add additional metadata do the dictionary
+
+        Only used in specific instances where metadata relies on data we only
+        have at request time, such as for lambda metadata
+
+        Metadata is only merged one key deep.
+        """
+        if self._metadata is not None:
+            # Merge one key deep
+            for key, val in data.items():
+                if isinstance(val, dict) and key in self._metadata and isinstance(self._metadata[key], dict):
+                    self._metadata[key].update(val)
+                else:
+                    self._metadata[key] = val
+        else:
+            self._metadata = data
 
     def _init_event_queue(self, chill_until, max_chill_time):
         # some libraries like eventlet monkeypatch queue.Queue and switch out the implementation.
         # In those cases we can't rely on internals of queue.Queue to be there, so we simply use
         # their queue and forgo the optimizations of ChilledQueue. In the case of eventlet, this
         # isn't really a loss, because the main reason for ChilledQueue (avoiding context switches
         # due to the event processor thread being woken up all the time) is not an issue.
@@ -240,14 +264,15 @@
                 self.handle_transport_success()
             except Exception as e:
                 self.handle_transport_fail(e)
 
     def start_thread(self, pid=None):
         super(Transport, self).start_thread(pid=pid)
         if (not self._thread or self.pid != self._thread.pid) and not self._closed:
+            self.handle_fork()
             try:
                 self._thread = threading.Thread(target=self._process_queue, name="eapm event processor thread")
                 self._thread.daemon = True
                 self._thread.pid = self.pid
                 self._thread.start()
             except RuntimeError:
                 pass
@@ -293,14 +318,18 @@
         """
         Failure handler called by the transport on send failure
         """
         message = str(exception)
         logger.error("Failed to submit message: %r", message, exc_info=getattr(exception, "print_trace", True))
         self.state.set_fail()
 
+    def handle_fork(self) -> None:
+        """Helper method to run code after a fork has been detected"""
+        pass
+
 
 # left for backwards compatibility
 AsyncTransport = Transport
 
 
 class TransportState(object):
     ONLINE = 1
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/exceptions.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/http.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,32 +48,29 @@
 except ImportError:
     certifi = None
 
 logger = get_logger("elasticapm.transport.http")
 
 
 class Transport(HTTPTransportBase):
-    def __init__(self, url, *args, **kwargs):
+    def __init__(self, url: str, *args, **kwargs) -> None:
         super(Transport, self).__init__(url, *args, **kwargs)
-        url_parts = compat.urlparse.urlparse(url)
         pool_kwargs = {"cert_reqs": "CERT_REQUIRED", "ca_certs": self.ca_certs, "block": True}
-        if self._server_cert and url_parts.scheme != "http":
-            pool_kwargs.update(
-                {"assert_fingerprint": self.cert_fingerprint, "assert_hostname": False, "cert_reqs": ssl.CERT_NONE}
-            )
-            del pool_kwargs["ca_certs"]
-        elif not self._verify_server_cert and url_parts.scheme != "http":
-            pool_kwargs["cert_reqs"] = ssl.CERT_NONE
-            pool_kwargs["assert_hostname"] = False
-        proxies = compat.getproxies_environment()
-        proxy_url = proxies.get("https", proxies.get("http", None))
-        if proxy_url and not compat.proxy_bypass_environment(url_parts.netloc):
-            self.http = urllib3.ProxyManager(proxy_url, **pool_kwargs)
-        else:
-            self.http = urllib3.PoolManager(**pool_kwargs)
+        if url.startswith("https"):
+            if self._server_cert:
+                pool_kwargs.update(
+                    {"assert_fingerprint": self.cert_fingerprint, "assert_hostname": False, "cert_reqs": ssl.CERT_NONE}
+                )
+                del pool_kwargs["ca_certs"]
+            elif not self._verify_server_cert:
+                pool_kwargs["cert_reqs"] = ssl.CERT_NONE
+                pool_kwargs["assert_hostname"] = False
+        self._pool_kwargs = pool_kwargs
+        self._http = None
+        self._url = url
 
     def send(self, data):
         response = None
 
         headers = self._headers.copy() if self._headers else {}
         headers.update(self.auth_headers)
 
@@ -109,14 +106,30 @@
                 message += body.decode("utf8", errors="replace")[:10000]
                 raise TransportException(message, data, print_trace=print_trace)
             return response.getheader("Location")
         finally:
             if response:
                 response.close()
 
+    @property
+    def http(self) -> urllib3.PoolManager:
+        if not self._http:
+            url_parts = compat.urlparse.urlparse(self._url)
+            proxies = compat.getproxies_environment()
+            proxy_url = proxies.get("https", proxies.get("http", None))
+            if proxy_url and not compat.proxy_bypass_environment(url_parts.netloc):
+                self._http = urllib3.ProxyManager(proxy_url, **self._pool_kwargs)
+            else:
+                self._http = urllib3.PoolManager(**self._pool_kwargs)
+        return self._http
+
+    def handle_fork(self) -> None:
+        # reset http pool to avoid sharing connections with the parent process
+        self._http = None
+
     def get_config(self, current_version=None, keys=None):
         """
         Gets configuration from a remote APM Server
 
         :param current_version: version of the current configuration
         :param keys: a JSON-serializable dict to identify this instance, e.g.
                 {
@@ -184,15 +197,15 @@
             version = data["version"]
             logger.info("Fetched APM Server version %s", version)
             self.client.server_version = version_string_to_tuple(version)
         except (urllib3.exceptions.RequestError, urllib3.exceptions.HTTPError) as e:
             logger.warning("HTTP error while fetching server information: %s", str(e))
         except json.JSONDecodeError as e:
             logger.warning("JSON decoding error while fetching server information: %s", str(e))
-        except KeyError:
+        except (KeyError, TypeError):
             logger.warning("No version key found in server response: %s", response.data)
 
     @property
     def cert_fingerprint(self):
         if self._server_cert:
             with open(self._server_cert, "rb") as f:
                 cert_data = read_pem_file(f)
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/http_base.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/http_base.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/transport/http_urllib3.py` & `sf-elastic-apm-6.7.2/elasticapm/transport/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 
 import base64
 import os
 import re
 from functools import partial
+from types import FunctionType
+from typing import Pattern
 
 from elasticapm.conf import constants
 from elasticapm.utils import compat, encoding
 
 try:
     from functools import partialmethod
 
@@ -69,15 +71,15 @@
         ret = func(name, [varmap(func, f, context, name, **kwargs) for f in var], **kwargs)
     else:
         ret = func(name, var, **kwargs)
     context.remove(objid)
     return ret
 
 
-def get_name_from_func(func):
+def get_name_from_func(func: FunctionType) -> str:
     # partials don't have `__module__` or `__name__`, so we use the values from the "inner" function
     if isinstance(func, partial_types):
         return "partial({})".format(get_name_from_func(func.func))
     elif hasattr(func, "_partialmethod") and hasattr(func._partialmethod, "func"):
         return "partial({})".format(get_name_from_func(func._partialmethod.func))
 
     module = func.__module__
@@ -90,25 +92,25 @@
     return "{0}.{1}".format(module, view_name)
 
 
 def build_name_with_http_method_prefix(name, request):
     return " ".join((request.method, name)) if name else name
 
 
-def is_master_process():
+def is_master_process() -> bool:
     # currently only recognizes uwsgi master process
     try:
         import uwsgi
 
         return os.getpid() == uwsgi.masterpid()
     except ImportError:
         return False
 
 
-def get_url_dict(url):
+def get_url_dict(url: str) -> dict:
     parse_result = compat.urlparse.urlparse(url)
 
     url_dict = {
         "full": encoding.keyword_field(url),
         "protocol": parse_result.scheme + ":",
         "hostname": encoding.keyword_field(parse_result.hostname),
         "pathname": encoding.keyword_field(parse_result.path),
@@ -119,32 +121,32 @@
     if port:
         url_dict["port"] = port
     if parse_result.query:
         url_dict["search"] = encoding.keyword_field("?" + parse_result.query)
     return url_dict
 
 
-def sanitize_url(url):
+def sanitize_url(url: str) -> str:
     if "@" not in url:
         return url
     parts = compat.urlparse.urlparse(url)
     return url.replace("%s:%s" % (parts.username, parts.password), "%s:%s" % (parts.username, constants.MASK))
 
 
-def get_host_from_url(url):
+def get_host_from_url(url: str) -> str:
     parsed_url = compat.urlparse.urlparse(url)
     host = parsed_url.hostname or " "
 
     if parsed_url.port and default_ports.get(parsed_url.scheme) != parsed_url.port:
         host += ":" + str(parsed_url.port)
 
     return host
 
 
-def url_to_destination(url, service_type="external"):
+def url_to_destination_resource(url: str) -> dict:
     parts = compat.urlparse.urlsplit(url)
     hostname = parts.hostname if parts.hostname else ""
     # preserve brackets for IPv6 URLs
     if "://[" in url:
         hostname = "[%s]" % hostname
     try:
         port = parts.port
@@ -156,31 +158,31 @@
     resource = hostname
     if not port and parts.scheme in default_ports:
         port = default_ports[parts.scheme]
     if port:
         if port != default_port:
             name += ":%d" % port
         resource += ":%d" % port
-    return {"service": {"name": name, "resource": resource, "type": service_type}}
+    return resource
 
 
-def read_pem_file(file_obj):
+def read_pem_file(file_obj) -> bytes:
     cert = b""
     for line in file_obj:
         if line.startswith(b"-----BEGIN CERTIFICATE-----"):
             break
     # scan until we find the first END CERTIFICATE marker
     for line in file_obj:
         if line.startswith(b"-----END CERTIFICATE-----"):
             break
         cert += line.strip()
     return base64.b64decode(cert)
 
 
-def starmatch_to_regex(pattern):
+def starmatch_to_regex(pattern: str) -> Pattern:
     options = re.DOTALL
     # check if we are case sensitive
     if pattern.startswith("(?-i)"):
         pattern = pattern[5:]
     else:
         options |= re.IGNORECASE
     i, n = 0, len(pattern)
@@ -189,7 +191,30 @@
         c = pattern[i]
         i = i + 1
         if c == "*":
             res.append(".*")
         else:
             res.append(re.escape(c))
     return re.compile(r"(?:%s)\Z" % "".join(res), options)
+
+
+def nested_key(d: dict, *args):
+    """
+    Traverses a dictionary for nested keys. Returns `None` if the at any point
+    in the traversal a key cannot be found.
+
+    Example:
+
+        >>> from elasticapm.utils import nested_key
+        >>> d = {"a": {"b": {"c": 0}}}
+        >>> nested_key(d, "a", "b", "c")
+        0
+        >>> nested_key(d, "a", "b", "d")
+        None
+    """
+    for arg in args:
+        try:
+            d = d[arg]
+        except (TypeError, KeyError):
+            d = None
+            break
+    return d
```

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/cgroup.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/cgroup.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/cloud.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/compat.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/compat.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/deprecation.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/disttracing.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/disttracing.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/encoding.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/json_encoder.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/logging.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/module_import.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/module_import.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/stacks.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/stacks.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/threading.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/threading.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/__init__.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/_wrappers.c` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/arguments.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/decorators.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/importer.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wrapt/wrappers.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/utils/wsgi.py` & `sf-elastic-apm-6.7.2/elasticapm/utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/elasticapm/version.py` & `sf-elastic-apm-6.7.2/elasticapm/contrib/serverless/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,9 +24,18 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = (6, 3, 4)
-VERSION = ".".join(map(str, __version__))
+import os
+
+# Future providers such as GCP and Azure will be added to this if/elif block
+# This way you can use the same syntax for each of the providers from a user
+# perspective
+if os.environ.get("AWS_REGION"):
+    from elasticapm.contrib.serverless.aws import capture_serverless
+else:
+    from elasticapm.contrib.serverless.aws import capture_serverless
+
+__all__ = ("capture_serverless",)
```

### Comparing `sf-elastic-apm-6.3.4/setup.cfg` & `sf-elastic-apm-6.7.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Operating System :: OS Independent
 	Topic :: Software Development
 	Programming Language :: Python
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	License :: OSI Approved :: BSD License
 project_urls = 
 	Documentation = https://www.elastic.co/guide/en/apm/agent/python/current/index.html
 	Release notes = https://www.elastic.co/guide/en/apm/agent/python/current/release-notes.html
 	Source = https://github.com/elastic/apm-agent-python
@@ -92,26 +93,29 @@
 	asynctest==0.12.2 ; python_version >= '3.7'
 	aiohttp ; python_version >= '3.7'
 	tornado ; python_version >= '3.7'
 	starlette ; python_version >= '3.7'
 	pytest-asyncio ; python_version >= '3.7'
 	pytest-mock ; python_version >= '3.7'
 	httpx ; python_version >= '3.6'
+	sanic ; python_version >= '3.7'
 
 [options.extras_require]
 flask = 
 	blinker
 aiohttp = 
 	aiohttp
 tornado = 
 	tornado
 starlette = 
 	starlette
 opentracing = 
 	opentracing>=2.0.0
+sanic = 
+	sanic
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [tool:pytest]
@@ -147,14 +151,15 @@
 	aiomysql
 	asyncpg
 	tornado
 	starlette
 	graphene
 	httpx
 	prometheus_client
+	sanic
 
 [isort]
 line_length = 120
 skip = wrapt,setup.py,build,src,elasticapm/__init__.py
 multi_line_output = 3
 include_trailing_comma = true
```

### Comparing `sf-elastic-apm-6.3.4/setup.py` & `sf-elastic-apm-6.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/PKG-INFO` & `sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-elastic-apm
-Version: 6.3.4
+Version: 6.7.2
 Summary: The official Python module for Elastic APM
 Home-page: https://github.com/snappyflow/sftrace-python-agent
 Author: Elastic, Inc
 License: BSD
 Project-URL: Documentation, https://www.elastic.co/guide/en/apm/agent/python/current/index.html
 Project-URL: Release notes, https://www.elastic.co/guide/en/apm/agent/python/current/release-notes.html
 Project-URL: Source, https://github.com/elastic/apm-agent-python
@@ -15,23 +15,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: <4,>=3.6
 Provides-Extra: flask
 Provides-Extra: aiohttp
 Provides-Extra: tornado
 Provides-Extra: starlette
 Provides-Extra: opentracing
+Provides-Extra: sanic
 License-File: LICENSE
 
 elastic-apm -- Elastic APM agent for Python
 ===========================================
 
 .. image:: https://apm-ci.elastic.co/buildStatus/icon?job=apm-agent-python%2Fapm-agent-python-mbp%2Fmaster
     :target: https://apm-ci.elastic.co/job/apm-agent-python/job/apm-agent-python-mbp/
```

### Comparing `sf-elastic-apm-6.3.4/sf_elastic_apm.egg-info/SOURCES.txt` & `sf-elastic-apm-6.7.2/sf_elastic_apm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,37 +41,42 @@
 elasticapm/contrib/flask/__init__.py
 elasticapm/contrib/flask/utils.py
 elasticapm/contrib/opentracing/__init__.py
 elasticapm/contrib/opentracing/span.py
 elasticapm/contrib/opentracing/tracer.py
 elasticapm/contrib/pylons/__init__.py
 elasticapm/contrib/rq/__init__.py
+elasticapm/contrib/sanic/__init__.py
+elasticapm/contrib/sanic/patch.py
+elasticapm/contrib/sanic/sanic_types.py
+elasticapm/contrib/sanic/utils.py
+elasticapm/contrib/serverless/__init__.py
+elasticapm/contrib/serverless/aws.py
 elasticapm/contrib/starlette/__init__.py
 elasticapm/contrib/starlette/utils.py
 elasticapm/contrib/tornado/__init__.py
 elasticapm/contrib/tornado/utils.py
 elasticapm/contrib/twisted/__init__.py
 elasticapm/contrib/zerorpc/__init__.py
 elasticapm/handlers/__init__.py
 elasticapm/handlers/logbook.py
 elasticapm/handlers/logging.py
 elasticapm/handlers/structlog.py
 elasticapm/instrumentation/__init__.py
 elasticapm/instrumentation/control.py
 elasticapm/instrumentation/register.py
 elasticapm/instrumentation/packages/__init__.py
+elasticapm/instrumentation/packages/azure.py
 elasticapm/instrumentation/packages/base.py
 elasticapm/instrumentation/packages/botocore.py
 elasticapm/instrumentation/packages/cassandra.py
 elasticapm/instrumentation/packages/dbapi2.py
 elasticapm/instrumentation/packages/elasticsearch.py
 elasticapm/instrumentation/packages/graphql.py
-elasticapm/instrumentation/packages/httpcore.py
 elasticapm/instrumentation/packages/httplib2.py
-elasticapm/instrumentation/packages/httpx.py
 elasticapm/instrumentation/packages/jinja2.py
 elasticapm/instrumentation/packages/mysql.py
 elasticapm/instrumentation/packages/mysql_connector.py
 elasticapm/instrumentation/packages/psycopg2.py
 elasticapm/instrumentation/packages/pylibmc.py
 elasticapm/instrumentation/packages/pymemcache.py
 elasticapm/instrumentation/packages/pymongo.py
@@ -90,28 +95,33 @@
 elasticapm/instrumentation/packages/asyncio/aiohttp_client.py
 elasticapm/instrumentation/packages/asyncio/aiomysql.py
 elasticapm/instrumentation/packages/asyncio/aiopg.py
 elasticapm/instrumentation/packages/asyncio/aioredis.py
 elasticapm/instrumentation/packages/asyncio/asyncpg.py
 elasticapm/instrumentation/packages/asyncio/base.py
 elasticapm/instrumentation/packages/asyncio/elasticsearch.py
-elasticapm/instrumentation/packages/asyncio/httpcore.py
-elasticapm/instrumentation/packages/asyncio/httpx.py
 elasticapm/instrumentation/packages/asyncio/sleep.py
 elasticapm/instrumentation/packages/django/__init__.py
 elasticapm/instrumentation/packages/django/template.py
+elasticapm/instrumentation/packages/httpx/__init__.py
+elasticapm/instrumentation/packages/httpx/utils.py
+elasticapm/instrumentation/packages/httpx/async/__init__.py
+elasticapm/instrumentation/packages/httpx/async/httpcore.py
+elasticapm/instrumentation/packages/httpx/async/httpx.py
+elasticapm/instrumentation/packages/httpx/sync/__init__.py
+elasticapm/instrumentation/packages/httpx/sync/httpcore.py
+elasticapm/instrumentation/packages/httpx/sync/httpx.py
 elasticapm/metrics/__init__.py
 elasticapm/metrics/base_metrics.py
 elasticapm/metrics/sets/__init__.py
 elasticapm/metrics/sets/breakdown.py
 elasticapm/metrics/sets/cpu.py
 elasticapm/metrics/sets/cpu_linux.py
 elasticapm/metrics/sets/cpu_psutil.py
 elasticapm/metrics/sets/prometheus.py
-elasticapm/metrics/sets/transactions.py
 elasticapm/transport/__init__.py
 elasticapm/transport/base.py
 elasticapm/transport/exceptions.py
 elasticapm/transport/http.py
 elasticapm/transport/http_base.py
 elasticapm/transport/http_urllib3.py
 elasticapm/utils/__init__.py
@@ -122,14 +132,15 @@
 elasticapm/utils/disttracing.py
 elasticapm/utils/encoding.py
 elasticapm/utils/json_encoder.py
 elasticapm/utils/logging.py
 elasticapm/utils/module_import.py
 elasticapm/utils/stacks.py
 elasticapm/utils/threading.py
+elasticapm/utils/time.py
 elasticapm/utils/wsgi.py
 elasticapm/utils/wrapt/__init__.py
 elasticapm/utils/wrapt/_wrappers.c
 elasticapm/utils/wrapt/arguments.py
 elasticapm/utils/wrapt/decorators.py
 elasticapm/utils/wrapt/importer.py
 elasticapm/utils/wrapt/wrappers.py
```

