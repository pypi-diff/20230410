# Comparing `tmp/ellar-0.3.4.tar.gz` & `tmp/ellar-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.3.4.tar", last modified: Sun Mar 26 09:04:14 2023, max compression
+gzip compressed data, was "ellar-0.3.6.tar", last modified: Mon Apr 10 20:01:35 2023, max compression
```

## Comparing `ellar-0.3.4.tar` & `ellar-0.3.6.tar`

### file list

```diff
@@ -1,448 +1,455 @@
--rw-r--r--   0        0        0      270 2023-03-26 09:03:42.548547 ellar-0.3.4/.coveragerc
--rw-r--r--   0        0        0       65 2023-03-26 09:03:42.548547 ellar-0.3.4/.dockerignore
--rw-r--r--   0        0        0      146 2023-03-26 09:03:42.548547 ellar-0.3.4/.flake8
--rw-r--r--   0        0        0      205 2023-03-26 09:03:42.548547 ellar-0.3.4/.github/dependabot.yml
--rw-r--r--   0        0        0      635 2023-03-26 09:03:42.548547 ellar-0.3.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-03-26 09:03:42.548547 ellar-0.3.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1122 2023-03-26 09:03:42.548547 ellar-0.3.4/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-03-26 09:03:42.548547 ellar-0.3.4/.gitignore
--rw-r--r--   0        0        0       53 2023-03-26 09:03:42.548547 ellar-0.3.4/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-03-26 09:03:42.548547 ellar-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-03-26 09:03:42.548547 ellar-0.3.4/LICENSE
--rw-r--r--   0        0        0     1166 2023-03-26 09:03:42.548547 ellar-0.3.4/Makefile
--rw-r--r--   0        0        0     9896 2023-03-26 09:03:42.552547 ellar-0.3.4/README.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/background-task.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/api-docs.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/custom-providers.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/events.md
--rw-r--r--   0        0        0    11223 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/execution-context.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/file-streaming.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/injection-scope.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/model-view-controller.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/testing.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/basics/versioning.md
--rw-r--r--   0        0        0    20977 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/caching.md
--rw-r--r--   0        0        0     1177 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/command-grouping.md
--rw-r--r--   0        0        0     6586 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/create-module-command.md
--rw-r--r--   0        0        0      388 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/create-project-command.md
--rw-r--r--   0        0        0     2755 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/custom-commands.md
--rw-r--r--   0        0        0     1343 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/index.md
--rw-r--r--   0        0        0     1206 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/new-command.md
--rw-r--r--   0        0        0      803 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/commands/runserver-command.md
--rw-r--r--   0        0        0     9064 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/configurations.md
--rw-r--r--   0        0        0     1765 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/custom-setup.md
--rw-r--r--   0        0        0     6728 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/handling-response/response-model.md
--rw-r--r--   0        0        0     6849 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/handling-response/response.md
--rwxr-xr-x   0        0        0    25915 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0    26456 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/EllarLogoW.png
--rwxr-xr-x   0        0        0     3888 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/Icon.svg
--rwxr-xr-x   0        0        0     4781 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/Logo.svg
--rw-r--r--   0        0        0    92094 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/ModuleDescription.png
--rw-r--r--   0        0        0    71483 2023-03-26 09:03:42.552547 ellar-0.3.4/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0   233058 2023-03-26 09:03:42.556547 ellar-0.3.4/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0   196608 2023-03-26 09:03:42.556547 ellar-0.3.4/docs/img/body-schema-doc3.png
--rwxr-xr-x   0        0        0    54689 2023-03-26 09:03:42.556547 ellar-0.3.4/docs/img/car_api.png
--rw-r--r--   0        0        0  1632661 2023-03-26 09:03:42.568547 ellar-0.3.4/docs/img/car_controller.gif
--rw-r--r--   0        0        0    50364 2023-03-26 09:03:42.568547 ellar-0.3.4/docs/img/controller_description.png
--rw-r--r--   0        0        0    45273 2023-03-26 09:03:42.568547 ellar-0.3.4/docs/img/create-car-schema.png
--rw-r--r--   0        0        0    19519 2023-03-26 09:03:42.568547 ellar-0.3.4/docs/img/create-dog-schema.png
--rwxr-xr-x   0        0        0  1326350 2023-03-26 09:03:42.576547 ellar-0.3.4/docs/img/ellar_demo.gif
--rwxr-xr-x   0        0        0    69977 2023-03-26 09:03:42.576547 ellar-0.3.4/docs/img/ellar_framework.png
--rw-r--r--   0        0        0   244178 2023-03-26 09:03:42.576547 ellar-0.3.4/docs/img/enum_docs_swagger.png
--rw-r--r--   0        0        0   168505 2023-03-26 09:03:42.580547 ellar-0.3.4/docs/img/event_docs_swagger.png
--rw-r--r--   0        0        0   253271 2023-03-26 09:03:42.580547 ellar-0.3.4/docs/img/form-schema-doc.png
--rw-r--r--   0        0        0   170683 2023-03-26 09:03:42.580547 ellar-0.3.4/docs/img/json_api_response_model.png
--rw-r--r--   0        0        0   216500 2023-03-26 09:03:42.584547 ellar-0.3.4/docs/img/math_router.png
--rw-r--r--   0        0        0   280669 2023-03-26 09:03:42.584547 ellar-0.3.4/docs/img/math_router_with_request_object.png
--rw-r--r--   0        0        0    52280 2023-03-26 09:03:42.584547 ellar-0.3.4/docs/img/middleware.png
--rw-r--r--   0        0        0   267982 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/img/query_filter_swagger.png
--rw-r--r--   0        0        0   208787 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/img/response_description.png
--rw-r--r--   0        0        0     3082 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/index.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/mount.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/openapi/index.md
--rw-r--r--   0        0        0    12584 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/controllers.md
--rw-r--r--   0        0        0    22248 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/custom_decorators.md
--rw-r--r--   0        0        0     8099 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/exception_handling.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/guards.md
--rw-r--r--   0        0        0     7667 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/index.md
--rw-r--r--   0        0        0     9240 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/middleware.md
--rw-r--r--   0        0        0     4493 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/module-router.md
--rw-r--r--   0        0        0    16316 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/modules.md
--rw-r--r--   0        0        0     9376 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/overview/providers.md
--rw-r--r--   0        0        0     9184 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/body.md
--rw-r--r--   0        0        0     1443 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/cookie-params.md
--rw-r--r--   0        0        0     6826 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/file-params.md
--rw-r--r--   0        0        0     4268 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/form-params.md
--rw-r--r--   0        0        0     3911 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/header-params.md
--rw-r--r--   0        0        0     1621 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/index.md
--rw-r--r--   0        0        0     6931 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/path-params.md
--rw-r--r--   0        0        0     5080 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/parsing-inputs/query-params.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/release-notes.md
--rw-r--r--   0        0        0       57 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     4115 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/templating/staticfiles.md
--rw-r--r--   0        0        0    13770 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/templating/templating.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/throttling.md
--rw-r--r--   0        0        0       15 2023-03-26 09:03:42.588547 ellar-0.3.4/docs/websockets.md
--rw-r--r--   0        0        0      143 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/__init__.py
--rw-r--r--   0        0        0      396 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/asgi_args.py
--rw-r--r--   0        0        0      257 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4361 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5138 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      944 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2215 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6541 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1397 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     5144 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/decorator.py
--rw-r--r--   0        0        0    10943 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/interface.py
--rw-r--r--   0        0        0     2020 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2501 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/model.py
--rw-r--r--   0        0        0     1859 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/module.py
--rw-r--r--   0        0        0      852 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/schema.py
--rw-r--r--   0        0        0     4505 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/cache/service.py
--rw-r--r--   0        0        0       62 2023-03-26 09:03:42.588547 ellar-0.3.4/ellar/commands/__init__.py
--rw-r--r--   0        0        0     2234 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/commands/base.py
--rw-r--r--   0        0        0     1566 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/__init__.py
--rw-r--r--   0        0        0      921 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      494 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     1510 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/command.py
--rw-r--r--   0        0        0     7627 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1029 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      554 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2503 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/file.py
--rw-r--r--   0        0        0      516 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4712 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/html.py
--rw-r--r--   0        0        0      800 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3421 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0      918 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/openapi.py
--rw-r--r--   0        0        0     1230 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/request.py
--rw-r--r--   0        0        0     1285 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      380 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0     1238 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/routing/__init__.py
--rw-r--r--   0        0        0    10415 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/common/routing/params.py
--rw-r--r--   0        0        0      345 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/compatible/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/compatible/cache_properties.py
--rw-r--r--   0        0        0      238 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/compatible/contextmanager.py
--rw-r--r--   0        0        0     1515 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/compatible/dict.py
--rw-r--r--   0        0        0      641 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/compatible/emails.py
--rw-r--r--   0        0        0     5482 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/constants.py
--rw-r--r--   0        0        0     1520 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/__init__.py
--rw-r--r--   0        0        0      120 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     4995 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2149 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/conf/config.py
--rw-r--r--   0        0        0     5418 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      129 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      681 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0      786 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/__init__.py
--rw-r--r--   0        0        0      103 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/exceptions.py
--rw-r--r--   0        0        0     1468 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/execution.py
--rw-r--r--   0        0        0     2474 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/factory.py
--rw-r--r--   0        0        0     2038 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/host.py
--rw-r--r--   0        0        0     2077 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/http.py
--rw-r--r--   0        0        0     3767 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/interface.py
--rw-r--r--   0        0        0      791 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/context/websocket.py
--rw-r--r--   0        0        0       98 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/controller/__init__.py
--rw-r--r--   0        0        0      927 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/controller/model.py
--rw-r--r--   0        0        0     1670 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/converters.py
--rw-r--r--   0        0        0      809 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/datastructures.py
--rw-r--r--   0        0        0     2045 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/events.py
--rw-r--r--   0        0        0     1862 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     1447 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/base.py
--rw-r--r--   0        0        0     2501 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0     2522 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/handlers.py
--rw-r--r--   0        0        0     1366 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/interfaces.py
--rw-r--r--   0        0        0     2239 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0      598 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/exceptions/validation.py
--rw-r--r--   0        0        0     7826 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/factory.py
--rw-r--r--   0        0        0      422 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/guard/__init__.py
--rw-r--r--   0        0        0      731 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/guard/apikey.py
--rw-r--r--   0        0        0     4274 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/guard/base.py
--rw-r--r--   0        0        0     3249 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/guard/http.py
--rw-r--r--   0        0        0    10288 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/main.py
--rw-r--r--   0        0        0     1159 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2663 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2685 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2244 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      447 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/schema.py
--rw-r--r--   0        0        0      121 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/sessions.py
--rw-r--r--   0        0        0     1081 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      317 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1250 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/base.py
--rw-r--r--   0        0        0     3857 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     7259 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/helper.py
--rw-r--r--   0        0        0    11087 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/modules/ref.py
--rw-r--r--   0        0        0      681 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/__init__.py
--rw-r--r--   0        0        0      315 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/__init__.py
--rw-r--r--   0        0        0    14136 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/base.py
--rw-r--r--   0        0        0     1608 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/extra_args.py
--rw-r--r--   0        0        0     2002 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/factory.py
--rw-r--r--   0        0        0     4158 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/request_model.py
--rw-r--r--   0        0        0     5830 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2425 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/args/websocket_model.py
--rw-r--r--   0        0        0     1203 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/helpers.py
--rw-r--r--   0        0        0     9194 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/params.py
--rw-r--r--   0        0        0     1083 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1651 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/base.py
--rw-r--r--   0        0        0     4455 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0      687 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/__init__.py
--rw-r--r--   0        0        0     2942 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/base.py
--rw-r--r--   0        0        0      386 2023-03-26 09:03:42.592547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/connection.py
--rw-r--r--   0        0        0      323 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/context.py
--rw-r--r--   0        0        0     1648 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/inject.py
--rw-r--r--   0        0        0      382 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/request.py
--rw-r--r--   0        0        0      389 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/response.py
--rw-r--r--   0        0        0      519 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/session.py
--rw-r--r--   0        0        0      381 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/non_parameter/websocket.py
--rw-r--r--   0        0        0     9511 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/params/resolvers/parameter.py
--rw-r--r--   0        0        0      623 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/__init__.py
--rw-r--r--   0        0        0      961 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/__init__.py
--rw-r--r--   0        0        0     8397 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/base.py
--rw-r--r--   0        0        0      715 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/factory.py
--rw-r--r--   0        0        0     3117 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/file.py
--rw-r--r--   0        0        0     2036 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/html.py
--rw-r--r--   0        0        0      802 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/interface.py
--rw-r--r--   0        0        0     2310 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/json.py
--rw-r--r--   0        0        0     4244 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/model/route.py
--rw-r--r--   0        0        0      995 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/response/response_types.py
--rw-r--r--   0        0        0      465 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     4609 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/base.py
--rw-r--r--   0        0        0      272 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/__init__.py
--rw-r--r--   0        0        0     1180 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/base.py
--rw-r--r--   0        0        0     1233 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/route.py
--rw-r--r--   0        0        0      190 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1421 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     2004 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/controller/websocket/route.py
--rw-r--r--   0        0        0     9572 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/operation_definitions.py
--rw-r--r--   0        0        0     4616 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/route.py
--rw-r--r--   0        0        0      230 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/router/__init__.py
--rw-r--r--   0        0        0     3838 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/router/app.py
--rw-r--r--   0        0        0     7891 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/router/module.py
--rw-r--r--   0        0        0     3567 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/router/route_collections.py
--rw-r--r--   0        0        0      217 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/websocket/__init__.py
--rw-r--r--   0        0        0     5643 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/websocket/handler.py
--rw-r--r--   0        0        0     5016 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/routing/websocket/route.py
--rw-r--r--   0        0        0     3402 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/schema.py
--rw-r--r--   0        0        0     1445 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/services.py
--rw-r--r--   0        0        0     1718 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/staticfiles.py
--rw-r--r--   0        0        0      600 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/templating/__init__.py
--rw-r--r--   0        0        0      472 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/templating/environment.py
--rw-r--r--   0        0        0     7362 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/templating/interface.py
--rw-r--r--   0        0        0     1634 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/templating/loader.py
--rw-r--r--   0        0        0     2421 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/templating/renderer.py
--rw-r--r--   0        0        0     2958 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/testclient.py
--rw-r--r--   0        0        0      556 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2519 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6182 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0      620 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/__init__.py
--rw-r--r--   0        0        0      400 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     7411 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5270 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      845 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/providers.py
--rw-r--r--   0        0        0     2253 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/scopes.py
--rw-r--r--   0        0        0     4545 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/di/service_config.py
--rw-r--r--   0        0        0     1485 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/__init__.py
--rw-r--r--   0        0        0      658 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/enums.py
--rw-r--r--   0        0        0      389 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/event_loop.py
--rw-r--r--   0        0        0     2137 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/importer.py
--rw-r--r--   0        0        0     1272 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/modelfield.py
--rw-r--r--   0        0        0      703 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/helper/module_loading.py
--rw-r--r--   0        0        0       52 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/logger.py
--rw-r--r--   0        0        0      573 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/__init__.py
--rw-r--r--   0        0        0     8077 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/builder.py
--rw-r--r--   0        0        0      239 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/docs_generators/__init__.py
--rw-r--r--   0        0        0      530 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/docs_generators/base.py
--rw-r--r--   0        0        0      959 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/docs_generators/redocs.py
--rw-r--r--   0        0        0     1025 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/docs_generators/swagger.py
--rw-r--r--   0        0        0     2934 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/module.py
--rw-r--r--   0        0        0    10597 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    15790 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      702 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      758 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/py.typed
--rw-r--r--   0        0        0     5274 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/reflect.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      403 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2023-03-26 09:03:42.596547 ellar-0.3.4/ellar/samples/modules.py
--rw-r--r--   0        0        0   155845 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/samples/static/css/bootstrap.min.css
--rwxr-xr-x   0        0        0    25915 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     1312 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0     4959 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/serializer.py
--rw-r--r--   0        0        0       58 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/services/__init__.py
--rw-r--r--   0        0        0     1903 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/services/reflector.py
--rw-r--r--   0        0        0      458 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/shortcuts.py
--rw-r--r--   0        0        0      585 2023-03-26 09:03:42.600547 ellar-0.3.4/ellar/types.py
--rw-r--r--   0        0        0      492 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/README.md
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/__init__.py
--rw-r--r--   0        0        0      837 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/controllers.py
--rw-r--r--   0        0        0      426 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/module.py
--rw-r--r--   0        0        0      908 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/routers.py
--rw-r--r--   0        0        0      756 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/services.py
--rw-r--r--   0        0        0     1708 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/statics/blog/blog.css
--rw-r--r--   0        0        0     1586 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/statics/blog/blog.rtl.css
--rw-r--r--   0        0        0     1008 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/statics/brand/bootstrap-logo-white.svg
--rw-r--r--   0        0        0     2047 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/statics/brand/bootstrap-logo.svg
--rw-r--r--   0        0        0      202 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/views/cat/list.html
--rw-r--r--   0        0        0    15257 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/cats/views/index.html
--rw-r--r--   0        0        0      150 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/application/module.py
--rw-r--r--   0        0        0      187 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/config.py
--rw-r--r--   0        0        0      786 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/server.py
--rw-r--r--   0        0        0      799 2023-03-26 09:03:42.600547 ellar-0.3.4/examples/catapp/tests/test_application.py
--rw-r--r--   0        0        0     3790 2023-03-26 09:03:42.600547 ellar-0.3.4/mkdocs.yml
--rw-r--r--   0        0        0      639 2023-03-26 09:03:42.600547 ellar-0.3.4/mypy.ini
--rw-r--r--   0        0        0     2920 2023-03-26 09:03:42.600547 ellar-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      207 2023-03-26 09:03:42.600547 ellar-0.3.4/pytest.ini
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/injector_module.py
--rw-r--r--   0        0        0     5270 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/main.py
--rw-r--r--   0        0        0       23 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/private/test.css
--rw-r--r--   0        0        0      741 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/schema.py
--rw-r--r--   0        0        0        4 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/statics/example.txt
--rw-r--r--   0        0        0      160 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/templates/ellar/index.html
--rw-r--r--   0        0        0      102 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/templates/ellar/list.html
--rw-r--r--   0        0        0      129 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/templates/index.html
--rw-r--r--   0        0        0      128 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/templates/list.html
--rw-r--r--   0        0        0       65 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/templates/render_string.html
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/__init__.py
--rw-r--r--   0        0        0       84 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/config.py
--rw-r--r--   0        0        0     2869 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/sample.py
--rw-r--r--   0        0        0     3360 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_application_factory.py
--rw-r--r--   0        0        0    16258 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_application_functions.py
--rw-r--r--   0        0        0    18162 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_cors.py
--rw-r--r--   0        0        0     4298 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_replacing_app_services.py
--rw-r--r--   0        0        0     2540 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_testclient_factory.py
--rw-r--r--   0        0        0     2308 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_application/test_trusted_host.py
--rw-r--r--   0        0        0      860 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_attribute_dict.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/__init__.py
--rw-r--r--   0        0        0     3625 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/_test_aio_memcache.py.ellar
--rw-r--r--   0        0        0     1893 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/pylib_mock.py
--rw-r--r--   0        0        0     2592 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/redis_mock.py
--rw-r--r--   0        0        0     1819 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_cache_many_config.py
--rw-r--r--   0        0        0     4758 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_cache_service.py
--rw-r--r--   0        0        0     4981 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_local_cache.py
--rw-r--r--   0        0        0      632 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_module_setup.py
--rw-r--r--   0        0        0     9959 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_pylibmc_cache.py
--rw-r--r--   0        0        0     6079 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_redis_cache.py
--rw-r--r--   0        0        0      577 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_cache/test_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/__init__.py
--rw-r--r--   0        0        0     2837 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_cache.py
--rw-r--r--   0        0        0     3345 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_controller.py
--rw-r--r--   0        0        0      782 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_exception.py
--rw-r--r--   0        0        0     3495 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_file.py
--rw-r--r--   0        0        0     1104 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_guards.py
--rw-r--r--   0        0        0     4078 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_html.py
--rw-r--r--   0        0        0      646 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_middleware.py
--rw-r--r--   0        0        0     2064 2023-03-26 09:03:42.600547 ellar-0.3.4/tests/test_common/test_decorators/test_modules.py
--rw-r--r--   0        0        0      901 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_common/test_decorators/test_openapi.py
--rw-r--r--   0        0        0     1447 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_common/test_decorators/test_request.py
--rw-r--r--   0        0        0     1297 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_common/test_decorators/test_serializer.py
--rw-r--r--   0        0        0      468 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_common/test_decorators/test_versioning.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_conf/__init__.py
--rw-r--r--   0        0        0     5216 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_conf/test_default_conf.py
--rw-r--r--   0        0        0     1369 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_conf/test_mixins.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/__init__.py
--rw-r--r--   0        0        0      439 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/sample.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/test_application_router.py
--rw-r--r--   0        0        0     4442 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/test_controller_decorator.py
--rw-r--r--   0        0        0     2445 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/test_controller_inheritance.py
--rw-r--r--   0        0        0     2626 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/test_module_router.py
--rw-r--r--   0        0        0     7148 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_controller/test_route_collection.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/__init__.py
--rw-r--r--   0        0        0     1332 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/examples.py
--rw-r--r--   0        0        0     2078 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/test_injectable_resolving.py
--rw-r--r--   0        0        0     5824 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/test_injector.py
--rw-r--r--   0        0        0     3508 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/test_provider_scopes.py
--rw-r--r--   0        0        0     3993 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_di/test_providers.py
--rw-r--r--   0        0        0     1815 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_events.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/__init__.py
--rw-r--r--   0        0        0      206 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/exception_runner.py
--rw-r--r--   0        0        0     2561 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/test_api_exception.py
--rw-r--r--   0        0        0     8507 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/test_custom_exceptions.py
--rw-r--r--   0        0        0     1195 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/test_error_details.py
--rw-r--r--   0        0        0     3715 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_exceptions/test_validation_exception.py
--rw-r--r--   0        0        0     7232 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_guard.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_helper/__init__.py
--rw-r--r--   0        0        0      564 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_helper/test_enum.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_helper/test_importer.py
--rw-r--r--   0        0        0      784 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_helper/test_model_field.py
--rw-r--r--   0        0        0      291 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_helper/test_module_loading.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_middleware/__init__.py
--rw-r--r--   0        0        0     2326 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_middleware/test_functional_middleware.py
--rw-r--r--   0        0        0     4190 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_middleware/test_service_provider_middleware.py
--rw-r--r--   0        0        0     2136 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_middleware/test_versioning_middleware.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_modules/__init__.py
--rw-r--r--   0        0        0     1847 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_modules/sample.py
--rw-r--r--   0        0        0     6080 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_modules/test_module_config.py
--rw-r--r--   0        0        0    11824 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_modules/test_module_ref.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_openapi/__init__.py
--rw-r--r--   0        0        0     8369 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_openapi/test_builder.py
--rw-r--r--   0        0        0     6656 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_openapi/test_module.py
--rw-r--r--   0        0        0    16438 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_openapi/test_open_api_route_documentation.py
--rw-r--r--   0        0        0     5598 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_reflect.py
--rw-r--r--   0        0        0     2159 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_reflector.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/__init__.py
--rw-r--r--   0        0        0     2483 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_defined_response_model.py
--rw-r--r--   0        0        0     4592 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_pydantic_response_model.py
--rw-r--r--   0        0        0     3433 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_response_file.py
--rw-r--r--   0        0        0     5069 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_response_html.py
--rw-r--r--   0        0        0     3268 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_response_streaming.py
--rw-r--r--   0        0        0     3882 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_response_type_definition_converter.py
--rw-r--r--   0        0        0     3509 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_response/test_route_response_model.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/__init__.py
--rw-r--r--   0        0        0     1088 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/sample.py
--rw-r--r--   0        0        0     3598 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_body_schema.py
--rw-r--r--   0        0        0     3653 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_body_schema_extra_properties.py
--rw-r--r--   0        0        0     4128 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_body_union_schema.py
--rw-r--r--   0        0        0     3944 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_cookie_schema.py
--rw-r--r--   0        0        0     6869 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_extra_args.py
--rw-r--r--   0        0        0     2407 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_form_schema.py
--rw-r--r--   0        0        0    10048 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_formparsers.py
--rw-r--r--   0        0        0     1330 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_forms.py
--rw-r--r--   0        0        0     1301 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0     3564 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_header_schema.py
--rw-r--r--   0        0        0     1569 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_invalid_path_param.py
--rw-r--r--   0        0        0     1788 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     5227 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_multi_body_errors.py
--rw-r--r--   0        0        0     3805 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_multi_query_errors.py
--rw-r--r--   0        0        0     9431 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_path.py
--rw-r--r--   0        0        0     2830 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_path_with_schema.py
--rw-r--r--   0        0        0     3355 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_put_with_no_body_schema.py
--rw-r--r--   0        0        0     2250 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_query.py
--rw-r--r--   0        0        0     3630 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_query_schema.py
--rw-r--r--   0        0        0     2035 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_request.py
--rw-r--r--   0        0        0     3426 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_routing/test_route_endpoint_params.py
--rw-r--r--   0        0        0      471 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_sample_project.py
--rw-r--r--   0        0        0     2689 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_schema.py
--rw-r--r--   0        0        0     6372 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_serializer.py
--rw-r--r--   0        0        0      768 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_shortcuts.py
--rw-r--r--   0        0        0    14079 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_staticfiles.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/module_statics/watever.txt
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/static/watever.txt
--rw-r--r--   0        0        0      167 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/templates/watever.html
--rw-r--r--   0        0        0     2889 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/test_module_templating.py
--rw-r--r--   0        0        0     2756 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/test_renderer.py
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_templating/views/watever.html
--rw-r--r--   0        0        0        0 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_versioning/__init__.py
--rw-r--r--   0        0        0     1968 2023-03-26 09:03:42.604547 ellar-0.3.4/tests/test_versioning/operations.py
--rw-r--r--   0        0        0     2098 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_default_versioning.py
--rw-r--r--   0        0        0     4410 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_default_versioning_for_controllers.py
--rw-r--r--   0        0        0     4431 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_header_versioning.py
--rw-r--r--   0        0        0     7755 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_header_versioning_controller.py
--rw-r--r--   0        0        0     3781 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_host_versioning.py
--rw-r--r--   0        0        0     3185 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_query_versioning.py
--rw-r--r--   0        0        0     2828 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_versioning/test_url_versioning.py
--rw-r--r--   0        0        0    17496 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_websocket.py
--rw-r--r--   0        0        0     9924 2023-03-26 09:03:42.608547 ellar-0.3.4/tests/test_websocket_handler.py
--rw-r--r--   0        0        0    13776 1970-01-01 00:00:00.000000 ellar-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      270 2023-04-10 20:01:01.562943 ellar-0.3.6/.coveragerc
+-rw-r--r--   0        0        0       65 2023-04-10 20:01:01.562943 ellar-0.3.6/.dockerignore
+-rw-r--r--   0        0        0      146 2023-04-10 20:01:01.562943 ellar-0.3.6/.flake8
+-rw-r--r--   0        0        0      205 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      635 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1122 2023-04-10 20:01:01.562943 ellar-0.3.6/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-04-10 20:01:01.562943 ellar-0.3.6/.gitignore
+-rw-r--r--   0        0        0       53 2023-04-10 20:01:01.562943 ellar-0.3.6/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-04-10 20:01:01.562943 ellar-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-04-10 20:01:01.562943 ellar-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1166 2023-04-10 20:01:01.562943 ellar-0.3.6/Makefile
+-rw-r--r--   0        0        0    10995 2023-04-10 20:01:01.562943 ellar-0.3.6/README.md
+-rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/background-task.md
+-rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/api-docs.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/custom-providers.md
+-rw-r--r--   0        0        0       15 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/events.md
+-rw-r--r--   0        0        0    10761 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/execution-context.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/file-streaming.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/injection-scope.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/model-view-controller.md
+-rw-r--r--   0        0        0    14945 2023-04-10 20:01:01.562943 ellar-0.3.6/docs/basics/testing.md
+-rw-r--r--   0        0        0     7829 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/basics/versioning.md
+-rw-r--r--   0        0        0    20977 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/caching.md
+-rw-r--r--   0        0        0     1177 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/command-grouping.md
+-rw-r--r--   0        0        0     6586 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/create-module-command.md
+-rw-r--r--   0        0        0      388 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/create-project-command.md
+-rw-r--r--   0        0        0     2755 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/custom-commands.md
+-rw-r--r--   0        0        0     1340 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/index.md
+-rw-r--r--   0        0        0     1206 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/new-command.md
+-rw-r--r--   0        0        0      803 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/commands/runserver-command.md
+-rw-r--r--   0        0        0     9064 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/configurations.md
+-rw-r--r--   0        0        0     1765 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/custom-setup.md
+-rw-r--r--   0        0        0     6728 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/handling-response/response-model.md
+-rw-r--r--   0        0        0     6813 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/handling-response/response.md
+-rwxr-xr-x   0        0        0    25915 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0    26456 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/EllarLogoW.png
+-rwxr-xr-x   0        0        0     3888 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/Icon.svg
+-rwxr-xr-x   0        0        0     4781 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/Logo.svg
+-rw-r--r--   0        0        0    92094 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/ModuleDescription.png
+-rw-r--r--   0        0        0    71483 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0   233058 2023-04-10 20:01:01.566943 ellar-0.3.6/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0   196608 2023-04-10 20:01:01.570943 ellar-0.3.6/docs/img/body-schema-doc3.png
+-rwxr-xr-x   0        0        0    54689 2023-04-10 20:01:01.570943 ellar-0.3.6/docs/img/car_api.png
+-rw-r--r--   0        0        0  1632661 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/car_controller.gif
+-rw-r--r--   0        0        0    50364 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/controller_description.png
+-rw-r--r--   0        0        0    45273 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/create-car-schema.png
+-rw-r--r--   0        0        0    19519 2023-04-10 20:01:01.582943 ellar-0.3.6/docs/img/create-dog-schema.png
+-rwxr-xr-x   0        0        0  1326350 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/ellar_demo.gif
+-rwxr-xr-x   0        0        0    69977 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/ellar_framework.png
+-rw-r--r--   0        0        0   244178 2023-04-10 20:01:01.594943 ellar-0.3.6/docs/img/enum_docs_swagger.png
+-rw-r--r--   0        0        0   168505 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/event_docs_swagger.png
+-rw-r--r--   0        0        0   253271 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/form-schema-doc.png
+-rw-r--r--   0        0        0   170683 2023-04-10 20:01:01.598943 ellar-0.3.6/docs/img/json_api_response_model.png
+-rw-r--r--   0        0        0   216500 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/math_router.png
+-rw-r--r--   0        0        0   280669 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/math_router_with_request_object.png
+-rw-r--r--   0        0        0    52280 2023-04-10 20:01:01.602943 ellar-0.3.6/docs/img/middleware.png
+-rw-r--r--   0        0        0   267982 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/img/query_filter_swagger.png
+-rw-r--r--   0        0        0   208787 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/img/response_description.png
+-rw-r--r--   0        0        0     4427 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/index.md
+-rw-r--r--   0        0        0       15 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/mount.md
+-rw-r--r--   0        0        0    12584 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/controllers.md
+-rw-r--r--   0        0        0    22543 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/custom_decorators.md
+-rw-r--r--   0        0        0     8099 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/exception_handling.md
+-rw-r--r--   0        0        0     8830 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/guards.md
+-rw-r--r--   0        0        0     7667 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/index.md
+-rw-r--r--   0        0        0     9240 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/middleware.md
+-rw-r--r--   0        0        0     4493 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/module-router.md
+-rw-r--r--   0        0        0    16329 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/modules.md
+-rw-r--r--   0        0        0     9435 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/overview/providers.md
+-rw-r--r--   0        0        0     9184 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/body.md
+-rw-r--r--   0        0        0     1443 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/cookie-params.md
+-rw-r--r--   0        0        0     6826 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/file-params.md
+-rw-r--r--   0        0        0     4268 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/form-params.md
+-rw-r--r--   0        0        0     3911 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/header-params.md
+-rw-r--r--   0        0        0     1621 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/index.md
+-rw-r--r--   0        0        0     6931 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/path-params.md
+-rw-r--r--   0        0        0     5080 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/parsing-inputs/query-params.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/release-notes.md
+-rw-r--r--   0        0        0       57 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     4115 2023-04-10 20:01:01.606943 ellar-0.3.6/docs/templating/staticfiles.md
+-rw-r--r--   0        0        0    13624 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/templating/templating.md
+-rw-r--r--   0        0        0     7321 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/throttling.md
+-rw-r--r--   0        0        0       15 2023-04-10 20:01:01.610942 ellar-0.3.6/docs/websockets.md
+-rw-r--r--   0        0        0      143 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/asgi_args.py
+-rw-r--r--   0        0        0      257 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4361 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5138 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      944 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2215 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6541 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1397 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     5144 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    10943 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2020 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2501 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/model.py
+-rw-r--r--   0        0        0     1859 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/module.py
+-rw-r--r--   0        0        0      852 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/schema.py
+-rw-r--r--   0        0        0     4505 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/cache/service.py
+-rw-r--r--   0        0        0       62 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/commands/__init__.py
+-rw-r--r--   0        0        0     2234 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/commands/base.py
+-rw-r--r--   0        0        0     1496 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     1510 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/command.py
+-rw-r--r--   0        0        0     6821 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1029 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      554 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2503 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0      531 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4712 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0      800 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3421 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0      918 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/openapi.py
+-rw-r--r--   0        0        0     1285 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      395 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0     1238 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/routing/__init__.py
+-rw-r--r--   0        0        0    10415 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/common/routing/params.py
+-rw-r--r--   0        0        0      345 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/cache_properties.py
+-rw-r--r--   0        0        0      238 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/contextmanager.py
+-rw-r--r--   0        0        0     1515 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/dict.py
+-rw-r--r--   0        0        0      641 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/compatible/emails.py
+-rw-r--r--   0        0        0     5387 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/constants.py
+-rw-r--r--   0        0        0     1423 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     4877 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2149 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     5129 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      129 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      681 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0      786 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/execution.py
+-rw-r--r--   0        0        0     2474 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/factory.py
+-rw-r--r--   0        0        0     2038 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/host.py
+-rw-r--r--   0        0        0     2077 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/http.py
+-rw-r--r--   0        0        0     3767 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/interface.py
+-rw-r--r--   0        0        0      791 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/context/websocket.py
+-rw-r--r--   0        0        0       98 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/controller/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/controller/model.py
+-rw-r--r--   0        0        0     1670 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/converters.py
+-rw-r--r--   0        0        0     1511 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/core_service_registration.py
+-rw-r--r--   0        0        0      809 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/datastructures.py
+-rw-r--r--   0        0        0      867 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     1447 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/base.py
+-rw-r--r--   0        0        0     2510 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0     1239 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/exceptions_types.py
+-rw-r--r--   0        0        0     2529 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/handlers.py
+-rw-r--r--   0        0        0     1366 2023-04-10 20:01:01.610942 ellar-0.3.6/ellar/core/exceptions/interfaces.py
+-rw-r--r--   0        0        0     2239 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0      598 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/exceptions/validation.py
+-rw-r--r--   0        0        0     7619 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/factory.py
+-rw-r--r--   0        0        0      422 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/__init__.py
+-rw-r--r--   0        0        0      731 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/apikey.py
+-rw-r--r--   0        0        0     4266 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/base.py
+-rw-r--r--   0        0        0     3249 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/guard/http.py
+-rw-r--r--   0        0        0     9179 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/main.py
+-rw-r--r--   0        0        0     1159 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2680 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2244 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      447 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/schema.py
+-rw-r--r--   0        0        0      121 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/sessions.py
+-rw-r--r--   0        0        0     1076 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      317 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1292 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     2935 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     7450 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0    10173 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0      681 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/__init__.py
+-rw-r--r--   0        0        0    14136 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/base.py
+-rw-r--r--   0        0        0     1608 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/extra_args.py
+-rw-r--r--   0        0        0     2002 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/factory.py
+-rw-r--r--   0        0        0     4158 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/request_model.py
+-rw-r--r--   0        0        0     5830 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2425 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/args/websocket_model.py
+-rw-r--r--   0        0        0     1203 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/helpers.py
+-rw-r--r--   0        0        0     9194 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/params.py
+-rw-r--r--   0        0        0     1083 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/base.py
+-rw-r--r--   0        0        0     4455 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0      687 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/__init__.py
+-rw-r--r--   0        0        0     2942 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/base.py
+-rw-r--r--   0        0        0      386 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/connection.py
+-rw-r--r--   0        0        0      323 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/context.py
+-rw-r--r--   0        0        0     1648 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/inject.py
+-rw-r--r--   0        0        0      382 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/request.py
+-rw-r--r--   0        0        0      389 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/response.py
+-rw-r--r--   0        0        0      519 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/session.py
+-rw-r--r--   0        0        0      381 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/non_parameter/websocket.py
+-rw-r--r--   0        0        0     9511 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      623 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/__init__.py
+-rw-r--r--   0        0        0     8397 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/base.py
+-rw-r--r--   0        0        0      715 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/factory.py
+-rw-r--r--   0        0        0     3117 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/file.py
+-rw-r--r--   0        0        0     2036 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/html.py
+-rw-r--r--   0        0        0      802 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/interface.py
+-rw-r--r--   0        0        0     2310 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/json.py
+-rw-r--r--   0        0        0     4244 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/model/route.py
+-rw-r--r--   0        0        0      995 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/response/response_types.py
+-rw-r--r--   0        0        0      465 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     4609 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/base.py
+-rw-r--r--   0        0        0      272 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/__init__.py
+-rw-r--r--   0        0        0     1180 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/base.py
+-rw-r--r--   0        0        0     1233 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1421 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     2004 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0    10981 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/operation_definitions.py
+-rw-r--r--   0        0        0     4616 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/route.py
+-rw-r--r--   0        0        0      230 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/__init__.py
+-rw-r--r--   0        0        0     3838 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/app.py
+-rw-r--r--   0        0        0     7819 2023-04-10 20:01:01.614942 ellar-0.3.6/ellar/core/routing/router/module.py
+-rw-r--r--   0        0        0     3567 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/router/route_collections.py
+-rw-r--r--   0        0        0      161 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     5643 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/handler.py
+-rw-r--r--   0        0        0     4917 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/routing/websocket/route.py
+-rw-r--r--   0        0        0     3402 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/schema.py
+-rw-r--r--   0        0        0     1718 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0      600 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/__init__.py
+-rw-r--r--   0        0        0      472 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/environment.py
+-rw-r--r--   0        0        0     7419 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/interface.py
+-rw-r--r--   0        0        0     1634 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/loader.py
+-rw-r--r--   0        0        0     2421 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/templating/renderer.py
+-rw-r--r--   0        0        0      563 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2519 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6182 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0      620 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/__init__.py
+-rw-r--r--   0        0        0      400 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     7411 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5270 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      845 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/providers.py
+-rw-r--r--   0        0        0     2253 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/scopes.py
+-rw-r--r--   0        0        0     4545 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/di/service_config.py
+-rw-r--r--   0        0        0     2045 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/events.py
+-rw-r--r--   0        0        0     1485 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/__init__.py
+-rw-r--r--   0        0        0      658 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/enums.py
+-rw-r--r--   0        0        0      389 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/event_loop.py
+-rw-r--r--   0        0        0     2137 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/importer.py
+-rw-r--r--   0        0        0     1272 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/modelfield.py
+-rw-r--r--   0        0        0      703 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/helper/module_loading.py
+-rw-r--r--   0        0        0       52 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/logger.py
+-rw-r--r--   0        0        0      573 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0     8077 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      239 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/__init__.py
+-rw-r--r--   0        0        0      530 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/base.py
+-rw-r--r--   0        0        0      959 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/redocs.py
+-rw-r--r--   0        0        0     1025 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/docs_generators/swagger.py
+-rw-r--r--   0        0        0     2934 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/module.py
+-rw-r--r--   0        0        0    10597 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    15790 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      702 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      758 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/py.typed
+-rw-r--r--   0        0        0     5274 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/reflect.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      403 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/modules.py
+-rw-r--r--   0        0        0   155845 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/static/css/bootstrap.min.css
+-rwxr-xr-x   0        0        0    25915 2023-04-10 20:01:01.618942 ellar-0.3.6/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     1312 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0     4959 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/serializer.py
+-rw-r--r--   0        0        0       58 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/services/__init__.py
+-rw-r--r--   0        0        0     1949 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/services/reflector.py
+-rw-r--r--   0        0        0      458 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/shortcuts.py
+-rw-r--r--   0        0        0      129 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4034 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/testing/module.py
+-rw-r--r--   0        0        0      585 2023-04-10 20:01:01.622942 ellar-0.3.6/ellar/types.py
+-rw-r--r--   0        0        0      509 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/__init__.py
+-rw-r--r--   0        0        0     1681 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/controllers.py
+-rw-r--r--   0        0        0     1077 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/module.py
+-rw-r--r--   0        0        0     1237 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/routers.py
+-rw-r--r--   0        0        0      622 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/schemas.py
+-rw-r--r--   0        0        0      666 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/services.py
+-rw-r--r--   0        0        0     1708 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
+-rw-r--r--   0        0        0     1586 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
+-rw-r--r--   0        0        0     1008 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
+-rw-r--r--   0        0        0     2047 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/__init__.py
+-rw-r--r--   0        0        0     2900 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
+-rw-r--r--   0        0        0     1604 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/tests/test_services.py
+-rw-r--r--   0        0        0      202 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/car/list.html
+-rw-r--r--   0        0        0      202 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/cat/list.html
+-rw-r--r--   0        0        0    15257 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/index.html
+-rw-r--r--   0        0        0      242 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/commands.py
+-rw-r--r--   0        0        0      187 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/config.py
+-rw-r--r--   0        0        0      635 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/root_module.py
+-rw-r--r--   0        0        0      947 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/server.py
+-rw-r--r--   0        0        0      134 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/carapp/tests/conftest.py
+-rw-r--r--   0        0        0      241 2023-04-10 20:01:01.622942 ellar-0.3.6/examples/01-carapp/pyproject.toml
+-rw-r--r--   0        0        0     3755 2023-04-10 20:01:01.622942 ellar-0.3.6/mkdocs.yml
+-rw-r--r--   0        0        0      639 2023-04-10 20:01:01.622942 ellar-0.3.6/mypy.ini
+-rw-r--r--   0        0        0     2920 2023-04-10 20:01:01.622942 ellar-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-04-10 20:01:01.622942 ellar-0.3.6/pytest.ini
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/injector_module.py
+-rw-r--r--   0        0        0     5270 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/main.py
+-rw-r--r--   0        0        0       23 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/private/test.css
+-rw-r--r--   0        0        0      741 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/schema.py
+-rw-r--r--   0        0        0        4 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/statics/example.txt
+-rw-r--r--   0        0        0      160 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/ellar/index.html
+-rw-r--r--   0        0        0      102 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/ellar/list.html
+-rw-r--r--   0        0        0      129 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/index.html
+-rw-r--r--   0        0        0      128 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/list.html
+-rw-r--r--   0        0        0       65 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/templates/render_string.html
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/config.py
+-rw-r--r--   0        0        0     2869 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/sample.py
+-rw-r--r--   0        0        0     3385 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_application_factory.py
+-rw-r--r--   0        0        0    15889 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_application_functions.py
+-rw-r--r--   0        0        0    18052 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_cors.py
+-rw-r--r--   0        0        0     4254 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_replacing_app_services.py
+-rw-r--r--   0        0        0     2329 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_application/test_trusted_host.py
+-rw-r--r--   0        0        0      860 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_attribute_dict.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/__init__.py
+-rw-r--r--   0        0        0     3625 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/_test_aio_memcache.py.ellar
+-rw-r--r--   0        0        0     1893 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/pylib_mock.py
+-rw-r--r--   0        0        0     2592 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/redis_mock.py
+-rw-r--r--   0        0        0     2795 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_decorator.py
+-rw-r--r--   0        0        0     1775 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_many_config.py
+-rw-r--r--   0        0        0     4772 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_cache_service.py
+-rw-r--r--   0        0        0     4995 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_local_cache.py
+-rw-r--r--   0        0        0      596 2023-04-10 20:01:01.622942 ellar-0.3.6/tests/test_cache/test_module_setup.py
+-rw-r--r--   0        0        0     9973 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_pylibmc_cache.py
+-rw-r--r--   0        0        0     6093 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_redis_cache.py
+-rw-r--r--   0        0        0      577 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_cache/test_schema.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_controller.py
+-rw-r--r--   0        0        0      782 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_exception.py
+-rw-r--r--   0        0        0     3495 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_file.py
+-rw-r--r--   0        0        0     1104 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_guards.py
+-rw-r--r--   0        0        0     4078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_html.py
+-rw-r--r--   0        0        0      646 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_middleware.py
+-rw-r--r--   0        0        0     2064 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_modules.py
+-rw-r--r--   0        0        0      901 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_openapi.py
+-rw-r--r--   0        0        0     1297 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_serializer.py
+-rw-r--r--   0        0        0      468 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_common/test_decorators/test_versioning.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/__init__.py
+-rw-r--r--   0        0        0     5216 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/test_default_conf.py
+-rw-r--r--   0        0        0     1151 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_conf/test_mixins.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/__init__.py
+-rw-r--r--   0        0        0      439 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/sample.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_application_router.py
+-rw-r--r--   0        0        0     4442 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_controller_decorator.py
+-rw-r--r--   0        0        0     2445 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_controller_inheritance.py
+-rw-r--r--   0        0        0     2626 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_module_router.py
+-rw-r--r--   0        0        0     7156 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_controller/test_route_collection.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/examples.py
+-rw-r--r--   0        0        0     2078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_injectable_resolving.py
+-rw-r--r--   0        0        0     5831 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_injector.py
+-rw-r--r--   0        0        0     3508 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_provider_scopes.py
+-rw-r--r--   0        0        0     3993 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_di/test_providers.py
+-rw-r--r--   0        0        0     1810 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_events.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/exception_runner.py
+-rw-r--r--   0        0        0     2560 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_api_exception.py
+-rw-r--r--   0        0        0     8679 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_custom_exceptions.py
+-rw-r--r--   0        0        0     1195 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_error_details.py
+-rw-r--r--   0        0        0     3720 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_exceptions/test_validation_exception.py
+-rw-r--r--   0        0        0     7249 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_guard.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/__init__.py
+-rw-r--r--   0        0        0      564 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_enum.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_importer.py
+-rw-r--r--   0        0        0      784 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_model_field.py
+-rw-r--r--   0        0        0      291 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_helper/test_module_loading.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/__init__.py
+-rw-r--r--   0        0        0     2286 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_functional_middleware.py
+-rw-r--r--   0        0        0     4207 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_service_provider_middleware.py
+-rw-r--r--   0        0        0     2161 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_middleware/test_versioning_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/__init__.py
+-rw-r--r--   0        0        0     1847 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/sample.py
+-rw-r--r--   0        0        0     6752 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/test_module_config.py
+-rw-r--r--   0        0        0     9889 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_modules/test_module_ref.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/__init__.py
+-rw-r--r--   0        0        0     8369 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_builder.py
+-rw-r--r--   0        0        0     6656 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_module.py
+-rw-r--r--   0        0        0    16438 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_openapi/test_open_api_route_documentation.py
+-rw-r--r--   0        0        0     5598 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_reflect.py
+-rw-r--r--   0        0        0     2159 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_reflector.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/__init__.py
+-rw-r--r--   0        0        0     2483 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_defined_response_model.py
+-rw-r--r--   0        0        0     4592 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_pydantic_response_model.py
+-rw-r--r--   0        0        0     3447 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_file.py
+-rw-r--r--   0        0        0     5078 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_html.py
+-rw-r--r--   0        0        0     3282 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_streaming.py
+-rw-r--r--   0        0        0     3882 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_response_type_definition_converter.py
+-rw-r--r--   0        0        0     3509 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_response/test_route_response_model.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/sample.py
+-rw-r--r--   0        0        0     3598 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_schema.py
+-rw-r--r--   0        0        0     3659 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_schema_extra_properties.py
+-rw-r--r--   0        0        0     4135 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_body_union_schema.py
+-rw-r--r--   0        0        0     3958 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_cookie_schema.py
+-rw-r--r--   0        0        0     6875 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_extra_args.py
+-rw-r--r--   0        0        0     2402 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_form_schema.py
+-rw-r--r--   0        0        0    10085 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_formparsers.py
+-rw-r--r--   0        0        0     1312 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_forms.py
+-rw-r--r--   0        0        0     1326 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0     3578 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_header_schema.py
+-rw-r--r--   0        0        0     1569 2023-04-10 20:01:01.626942 ellar-0.3.6/tests/test_routing/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1788 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     5233 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3811 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_multi_query_errors.py
+-rw-r--r--   0        0        0     9423 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_path.py
+-rw-r--r--   0        0        0     2825 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_path_with_schema.py
+-rw-r--r--   0        0        0     3361 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_put_with_no_body_schema.py
+-rw-r--r--   0        0        0     2242 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_query.py
+-rw-r--r--   0        0        0     3644 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_query_schema.py
+-rw-r--r--   0        0        0     2017 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_request.py
+-rw-r--r--   0        0        0     3430 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_routing/test_route_endpoint_params.py
+-rw-r--r--   0        0        0      451 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_sample_project.py
+-rw-r--r--   0        0        0     2689 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_schema.py
+-rw-r--r--   0        0        0     6372 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_serializer.py
+-rw-r--r--   0        0        0      768 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_shortcuts.py
+-rw-r--r--   0        0        0    14104 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_staticfiles.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/module_statics/watever.txt
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/static/watever.txt
+-rw-r--r--   0        0        0      167 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/templates/watever.html
+-rw-r--r--   0        0        0     2892 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/test_module_templating.py
+-rw-r--r--   0        0        0     2757 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/test_renderer.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_templating/views/watever.html
+-rw-r--r--   0        0        0     2418 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_testing.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/operations.py
+-rw-r--r--   0        0        0     2138 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_default_versioning.py
+-rw-r--r--   0        0        0     4449 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_default_versioning_for_controllers.py
+-rw-r--r--   0        0        0     4468 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_header_versioning.py
+-rw-r--r--   0        0        0     7813 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_header_versioning_controller.py
+-rw-r--r--   0        0        0     3816 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_host_versioning.py
+-rw-r--r--   0        0        0     3220 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_query_versioning.py
+-rw-r--r--   0        0        0     2858 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_versioning/test_url_versioning.py
+-rw-r--r--   0        0        0    17496 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_websocket.py
+-rw-r--r--   0        0        0    11066 2023-04-10 20:01:01.630942 ellar-0.3.6/tests/test_websocket_handler.py
+-rw-r--r--   0        0        0    14875 1970-01-01 00:00:00.000000 ellar-0.3.6/PKG-INFO
```

### Comparing `ellar-0.3.4/.github/workflows/publish.yml` & `ellar-0.3.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/.github/workflows/test.yml` & `ellar-0.3.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/.github/workflows/test_full.yml` & `ellar-0.3.6/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/.gitignore` & `ellar-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/.pre-commit-config.yaml` & `ellar-0.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/LICENSE` & `ellar-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/Makefile` & `ellar-0.3.6/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/README.md` & `ellar-0.3.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 [![PyPI version](https://img.shields.io/pypi/pyversions/ellar.svg)](https://pypi.python.org/pypi/ellar)
 
 ## Introduction
 
 Ellar is a lightweight ASGI framework for building efficient and scalable server-side python applications.
 It supports both OOP (Object-Oriented Programming) and FP (Functional Programming)
 
-Ellar is based on [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services in Python. 
+Ellar is based on [Starlette (ASGI toolkit)](https://www.starlette.io/), a lightweight ASGI framework/toolkit well-suited for developing asynchronous web services with Python. 
 While Ellar provides a high level of abstraction on top of Starlette, it still incorporates some of its features, as well as those of FastAPI. 
 If you are familiar with these frameworks, you will find it easy to understand and use Ellar.
 
+## Features Summary
+
+- **Easy to Use**: Ellar has a simple and intuitive API that makes it easy to get started with building a fast and scalable web applications or web APIs in Python.
+- **Dependency Injection (DI)**: It comes with DI system makes it easy to manage dependencies and reduce coupling between components.
+- **Pydantic Integration**: It is properly integrated with Pydantic, a popular Python library for data validation, to ensure that input data is valid.
+- **Templating with Jinja2**: Ellar provides built-in support for Jinja2 templates, making it easy to create dynamic web pages.
+- **OpenAPI Documentation**: It comes with built-in support for OpenAPI documentation, making it easy to generate `Swagger` or `ReDoc` documentation for your API. And more can be added with ease if necessary.
+- **Controller (MVC) Architecture**: Ellar's controller architecture follows the Model-View-Controller (MVC) pattern, making it easy to organize your code.
+- **Guards for Authentication and Authorization**: It provides built-in support for guards, allowing you to easily implement authentication and authorization in your application.
+- **Modularity**: Ellar follows a modular architecture inspired by NestJS, making it easy to organize your code into reusable modules.
+- **Asynchronous programming**: It allows you to takes advantage of Python's `async/await` feature to write efficient and fast code that can handle large numbers of concurrent requests
+
 ## Dependencies
 - Python >= 3.7
 - Starlette
 - Injector
 - Pydantic
 
-## Features Summary
-- `Pydantic integration`
-- `Dependency Injection (DI)`
-- `Templating with Jinja2`
-- `OpenAPI Documentation (Swagger and ReDoc)`
-- `Controller (MVC)`
-- `Guards (authentications, roles and permissions)`
-- `Modularization (eg: flask blueprint)`
-- `Websocket support`
-- `Session and Cookie support`
-- `CORS, GZip, Static Files, Streaming responses`
-
 ## Installation
 ### Poetry Installation
 For [Poetry](https://python-poetry.org/) usages
 
 ```shell
 poetry add ellar-cli
 ```
```

### Comparing `ellar-0.3.4/docs/basics/execution-context.md` & `ellar-0.3.6/docs/basics/execution-context.md`

 * *Files 8% similar despite different names*

```diff
@@ -190,122 +190,103 @@
 Once you have access to the `ExecutionContext` object, you can use its methods and properties to access information about the current request.
 
 ## **Reflector and Metadata**
 Ellar provides the ability to attach **custom metadata** to route handlers through the `@set_metadata()` decorator. 
 We can then access this metadata from within our class to make certain decisions.
 
 ```python
-# project_name/apps/dogs/controllers.py
+# project_name/apps/cars/controllers.py
 
 from ellar.common import Body, Controller, post, set_metadata
 from ellar.core import ControllerBase
-from .schemas import CreateDogSerializer, DogListFilter
+from .schemas import CreateCarSerializer
 
 
-@Controller('/dogs')
-class DogsController(ControllerBase):
+@Controller('/car')
+class CarController(ControllerBase):
     @post()
     @set_metadata('role', ['admin'])
-    async def create(self, payload: CreateDogSerializer = Body()):
+    async def create(self, payload: CreateCarSerializer = Body()):
         result = payload.dict()
-        result.update(message='This action adds a new dog')
+        result.update(message='This action adds a new car')
         return result
 ```
 
 With the construction above, we attached the `roles` metadata (roles is a metadata key and ['admin'] is the associated value) 
 to the `create()` method. While this works, it's not good practice to use `@set_metadata()` directly in your routes. 
 Instead, create your own decorators, as shown below:
 
 ```python
-# project_name/apps/dogs/controllers.py
+# project_name/apps/cars/controllers.py
 import typing
 from ellar.common import Body, Controller, post, set_metadata
 from ellar.core import ControllerBase
-from .schemas import CreateDogSerializer, DogListFilter
+from .schemas import CreateCarSerializer
 
 
 def roles(*_roles: str) -> typing.Callable:
     return set_metadata('roles', list(_roles))
 
 
-@Controller('/dogs')
-class DogsController(ControllerBase):
+@Controller('/car')
+class CarController(ControllerBase):
     @post()
     @roles('admin', 'is_staff')
-    async def create(self, payload: CreateDogSerializer = Body()):
+    async def create(self, payload: CreateCarSerializer = Body()):
         result = payload.dict()
-        result.update(message='This action adds a new dog')
+        result.update(message='This action adds a new car')
         return result
 ```
 
 !!! info
     It's important to note that `ExecutionContext` becomes available when there is route handler found to handle the current request.
 
 To access the route's role(s) (custom metadata), we'll use the `Reflector` helper class, which is provided out of the box by the framework. 
 `Reflector` can be injected into a class in the normal way:
 
 ```python
-# project_name/apps/dogs/guards.py
+# project_name/apps/cars/guards.py
 from ellar.di import injectable
 from ellar.core import GuardCanActivate, IExecutionContext
 from ellar.services import Reflector
 
 
 @injectable()
 class RoleGuard(GuardCanActivate):
     def __init__(self, reflector: Reflector):
         self.reflector = reflector
 
     async def can_activate(self, context: IExecutionContext) -> bool:
         roles = self.reflector.get('roles', context.get_handler())
         # request = context.switch_to_http_connection().get_request()
         # check if user in request object has role
+        if not roles:
+            return True
         return 'user' in roles
 ```
 
-Next, we apply the `RoleGuard` to `DogsController`
+Next, we apply the `RoleGuard` to `CarController`
 
 ```python
-# project_name/apps/dogs/controllers.py
+# project_name/apps/cars/controllers.py
 import typing
-from ellar.common import Body, Controller, post, set_metadata
+from ellar.common import Body, Controller, post, set_metadata, Guards
 from ellar.core import ControllerBase
-from .schemas import CreateDogSerializer, DogListFilter
+from .schemas import CreateCarSerializer
 from .guards import RoleGuard
 
 def roles(*_roles: str) -> typing.Callable:
     return set_metadata('roles', list(_roles))
 
 
-@Controller('/dogs', guards=[RoleGuard, ])
-class DogsController(ControllerBase):
+@Controller('/car')
+@Guards(RoleGuard)
+class CarController(ControllerBase):
     @post()
     @roles('admin', 'is_staff')
-    async def create(self, payload: CreateDogSerializer = Body()):
+    async def create(self, payload: CreateCarSerializer = Body()):
         result = payload.dict()
-        result.update(message='This action adds a new dog')
+        result.update(message='This action adds a new car')
         return result
 ```
 
-Also, since `RoleGuard` depends on `Reflector`, it has to be registered as a provider. And we do that in `DogsModule`:
-
-```python
-# project_name/apps/dogs/module.py
-
-from ellar.common import Module
-from ellar.core import ModuleBase
-from ellar.di import Container
-
-from .controllers import DogsController
-from .guards import RoleGuard
-
-
-@Module(
-    controllers=[DogsController],
-    providers=[RoleGuard],
-)
-class DogsModule(ModuleBase):
-    def register_providers(self, container: Container) -> None:
-        # for more complicated provider registrations
-        # container.register_instance(...)
-        pass
-```
+Also, since `RoleGuard` is marked as `injectable`, EllarInjector service will be able to resolve `RoleGuard` without `RoleGuard` registered as a provider.
```

### Comparing `ellar-0.3.4/docs/caching.md` & `ellar-0.3.6/docs/caching.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/commands/command-grouping.md` & `ellar-0.3.6/docs/commands/command-grouping.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/commands/create-module-command.md` & `ellar-0.3.6/docs/commands/create-module-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/commands/custom-commands.md` & `ellar-0.3.6/docs/commands/custom-commands.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/commands/index.md` & `ellar-0.3.6/docs/commands/index.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Introduction
+# Ellar CLI
 Ellar CLI is an abstracted tool for the Ellar web framework that helps in the standard project scaffold of the 
 framework, module project scaffold, running the project local server using UVICORN, and running custom commands registered in the application module or any Ellar module.
 
 ## Installation
 if you have [ellar](https://github.com/eadwinCode/ellar) install ready
 ```
 pip install ellar-cli
```

### Comparing `ellar-0.3.4/docs/commands/new-command.md` & `ellar-0.3.6/docs/commands/new-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/commands/runserver-command.md` & `ellar-0.3.6/docs/commands/runserver-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/configurations.md` & `ellar-0.3.6/docs/configurations.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/custom-setup.md` & `ellar-0.3.6/docs/custom-setup.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/handling-response/response-model.md` & `ellar-0.3.6/docs/handling-response/response-model.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/handling-response/response.md` & `ellar-0.3.6/docs/handling-response/response.md`

 * *Files 1% similar despite different names*

```diff
@@ -199,9 +199,7 @@
 
 @Controller
 class ItemsController(ControllerBase):
     @get("/me", response=UserSchema)
     def me(self):
         return PlainTextResponse("some text response.", status_code=200)
 ```
-
-## using serialize_object function
```

### Comparing `ellar-0.3.4/docs/img/EllarLogoB.png` & `ellar-0.3.6/docs/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/EllarLogoIconOnly.png` & `ellar-0.3.6/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/EllarLogoW.png` & `ellar-0.3.6/docs/img/EllarLogoW.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/Icon.svg` & `ellar-0.3.6/docs/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/Logo.svg` & `ellar-0.3.6/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/ModuleDescription.png` & `ellar-0.3.6/docs/img/ModuleDescription.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/body-schema-doc.png` & `ellar-0.3.6/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/body-schema-doc2.png` & `ellar-0.3.6/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/body-schema-doc3.png` & `ellar-0.3.6/docs/img/body-schema-doc3.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/car_api.png` & `ellar-0.3.6/docs/img/car_api.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/car_controller.gif` & `ellar-0.3.6/docs/img/car_controller.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/controller_description.png` & `ellar-0.3.6/docs/img/controller_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/create-car-schema.png` & `ellar-0.3.6/docs/img/create-car-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/create-dog-schema.png` & `ellar-0.3.6/docs/img/create-dog-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/ellar_demo.gif` & `ellar-0.3.6/docs/img/ellar_demo.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/ellar_framework.png` & `ellar-0.3.6/docs/img/ellar_framework.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/enum_docs_swagger.png` & `ellar-0.3.6/docs/img/enum_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/event_docs_swagger.png` & `ellar-0.3.6/docs/img/event_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/form-schema-doc.png` & `ellar-0.3.6/docs/img/form-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/json_api_response_model.png` & `ellar-0.3.6/docs/img/json_api_response_model.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/math_router.png` & `ellar-0.3.6/docs/img/math_router.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/math_router_with_request_object.png` & `ellar-0.3.6/docs/img/math_router_with_request_object.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/middleware.png` & `ellar-0.3.6/docs/img/middleware.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/query_filter_swagger.png` & `ellar-0.3.6/docs/img/query_filter_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/img/response_description.png` & `ellar-0.3.6/docs/img/response_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/controllers.md` & `ellar-0.3.6/docs/overview/controllers.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/custom_decorators.md` & `ellar-0.3.6/docs/overview/custom_decorators.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 Ellar provides a variety of function decorators in the `ellar.common` python module that can be used to modify the behavior of route functions. 
+
 These decorators can be used to change the response type of a route function, add filters to the response schema, define the OPENAPI context, and more. 
 In general, these decorators can help to simplify and streamline the process of creating routes.
 
 ## **HTTP Method Decorator**
 `@get`, `@post`, `@put`, `@patch`, `@delete`, `@trace`, `@options`, `@head` are decorators that define the standard HTTP methods for a route function. 
 They indicate the type of HTTP request that the route function can handle, such as a `GET` request or a `POST` request. 
 
@@ -53,20 +54,22 @@
 async def on_connect(self, websocket: WebSocket, code: int):
     await websocket.close(code)
 ```
 
 ## **Non Route Function Parameters Decorators**
 We discussed decorators that are used to define route function parameter dependencies in Ellar. 
 These decorators, such as `Query`, `Form`, and `Body`, etc. are pydantic models used to specify the expected parameters for a route function. 
+
 However, there are also some route parameters that are **system** dependent, such as the `request` or `websocket` object, and the `response` object. 
 These parameters are resolved by the application and supplied to the route function when needed, and are not specified with pydantic models or user input.
 
 ### Provide(Type)
 The **Provide(Type)** decorator is used to resolve a service provider and inject it into a route function parameter. 
 This can be useful when using the ModuleRouter feature in Ellar. 
+
 It allows for easy injection of services into route functions, making it easier to manage dependencies and improve code organization. 
 This can be useful for resolving database connections, external APIs, or other resources that are used by the route function.
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Provide
 from ellar.core import App, Config
@@ -104,14 +107,15 @@
     http_connection_instance = ctx.switch_to_http_connection().get_client()
     query_params = http_connection_instance.query_params
     return {'message': 'inject execution context', 'query_params': query_params}
 ```
 
 In this example, the example_endpoint function is decorated with the **Context()** decorator, which injects the current `IExecutionContext` object into the `ctx` parameter of the function. 
 The `IExecutionContext` object provides access to various resources and information related to the current execution context, such as the current HTTP connection, query parameters, and more. 
+
 In this example, the `switch_to_http_connection()` method is used to access the current HTTP connection and the `get_client()` method is used to get the client object for the connection. 
 The `query_params` attribute of the client object is then accessed and included in the response returned by the endpoint.
 
 ### Req
 **Req()** decorator injects current `Request` object to route function parameter.
 
 For example:
@@ -163,22 +167,19 @@
 async def example_endpoint(ws = Ws()):
     await ws.accept()
     await ws.send_json({'message': 'injected WebSocket object to route function'})
 ```
 The above code creates a WebSocket route '/test-ws' and when a client connects to this route, 
 the `example_endpoint` function is executed. The `Ws` decorator injects the current `WebSocket` object to the `ws` parameter of the function, which can then be used to interact with the WebSocket connection, such as accepting the connection and sending data to the client.
 
-### Host
-**Host()** decorator injects current client host address to route function parameter.
-
-### Session
-**Session()** decorator injects current Session object to route function parameter.
+The same conditions and examples applies for:
 
-### Http
-**Http()** decorator injects current HTTP connection object to route function parameter.
+- **Host()** decorator injects current client host address to route function parameter.
+- **Session()** decorator injects current Session object to route function parameter. This requires [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware) module from Starlette added in application middleware and also `SessionMiddleware` module depends on [itsdangerous](https://pypi.org/project/itsdangerous/) package.
+- **Http()** decorator injects current HTTP connection object to route function parameter.
 
 ## **Creating a Custom Parameter Decorators**
 You can still create your own route parameter decorators that suits your need. You simply need to follow a contract, `NonParameterResolver`, and override the resolve function.
 
 The `NonParameterResolver` has two attribute, `type_annotation` and `parameter_name`, that are provided automatically when computing route parameter dependencies. 
 They are gotten from the application of the NonParameterResolver, like so - `def s(parameter_name:type_annotation = NonParameterResolver())`.
 
@@ -199,14 +200,15 @@
         if user:
             return {self.parameter_name: user}, []
         return {}, [ErrorWrapper('Authenticated Users Only', loc='system')]
 ```
 
 This example defines a custom decorator called `UserParam` that inherits from `NonParameterResolver`. 
 The `resolve` method is overridden to extract the user from the current `IExecutionContext`'s request. 
+
 If the user is found, it is returned as a dict with the key as the `parameter_name` of the decorator, along with an empty list of errors. 
 If no user is found, an empty dict and a list of errors containing an ErrorWrapper object is returned. 
 
 This `UserParam` decorator can then be used to inject the user object to a route function parameter like so:
 ```python
 
 @router.get('/user')
@@ -230,14 +232,15 @@
 @render(template_name='my_template')
 def index(self):
     return {'name': 'Ellar Template'}
 ```
 
 In the example, the index function is decorated with the `render` decorator, 
 which will return a 200 status code and HTML content from my_template. 
+
 The return object from the index function will be used as the templating context for `my_template` during the template rendering process. 
 This allows the function to pass data to the template and have it rendered with the provided context, the rendered template will be the response body.
 
 See [HTML Templating](/ellar/templating/templating) for more information on `render` and HTML templating with Ellar.
 
 ### FILE
 **@file()** decorator converts a route function response to file or streaming response type. 
@@ -375,62 +378,67 @@
 ```
 In example, `serializer_filter` to filter values that are `None` and also excluded `password` property from been returned.
 See [Pydantic Model Export](https://docs.pydantic.dev/usage/exporting_models/#modeldict) for more examples.
 
 ### VERSION
 **@version()**  is a decorator that provides endpoint versioning for a route function. 
 This decorator allows you to specify the version of the endpoint that the function is associated with. 
+
 Based on the versioning scheme configuration in the application, versioned route functions are called. This can be useful for maintaining backward compatibility, or for rolling out new features to different versions of an application. 
 More information on how to use this decorator can be found in the [Versioning documentation]()
 
 A quick example on how to use `version` decorator:
 ```python
-from ellar.common import post, version
+from ellar.common import post, Version
 
 @post("/create", name='v2_v3_list')
-@version('2', '3')
+@Version('2', '3')
 async def get_item_v2_v3(self):
     return {'message': 'for v2 and v3 request'}
 ```
 
 The `version` decorator takes a list of values as an argument, for example `@version('2', '3')`. 
 This indicates that the `get_item_v2_v3` route function will handle version 2 and version 3 requests of the /create endpoint. 
 This allows for multiple versions of the same endpoint to be handled by different route functions, each with their own logic and implementation.
 
 ### GUARDS
-**@guards()**  is a decorator that applies a protection class of type GuardCanActivate to a route function. 
-These protection classes have a can_execute function that is called to determine whether a route function should be executed. 
-This decorator allows you to apply certain conditions or checks before a route function is executed, such as authentication or authorization checks. 
+**@Guards()**  is a decorator that applies a protection class of type `GuardCanActivate` to a route function. 
+These protection classes have a `can_execute` function that is called to determine whether a route function should be executed. 
+
+This decorator allows you to apply certain conditions or checks before a route function is executed, such as `authentication` or `authorization` checks. 
 This can help to ensure that only authorized users can access certain resources. 
+
 More information on how to use this decorator can be found in the [Guard Documentation]()
 
-A quick example on how to use `guards` decorator:
+A quick example on how to use `Guards` decorator:
 ```python
 import typing as t
-from ellar.common import get, guards
+from ellar.common import get, Guards
 from ellar.core.guard import APIKeyQuery
 from ellar.core.connection import HTTPConnection
 
 
 class MyAPIKeyQuery(APIKeyQuery):
     async def authenticate(self, connection: HTTPConnection, key: t.Optional[t.Any]) -> t.Optional[t.Any]:
         if key == 'supersecret':
             return True
         return False
 
 
 @get("/")
-@guards(MyAPIKeyQuery(), )
+@Guards(MyAPIKeyQuery(), )
 async def get_guarded_items(self):
     return {'message': 'worked fine with `key`=`supersecret`'}
 ```
-The `guards` decorator, like the `version` decorator, takes a list of values as an argument. 
+The `Guards` decorator, like the `version` decorator, takes a list of values as an argument. 
 During a request, the provided guards are called in the order in which they are provided. 
+
 This allows you to apply multiple guards to a single route function and have them executed in a specific order. 
 This is useful for applying multiple levels of security or access control to a single endpoint. 
+
 Each guard class has a `can_execute` function that is called in the order specified by the decorator, if any of the guard's `can_execute` function returns False, the route function will not be executed.
 
 ## **Command Decorators**
 The `command` decorator is used to convert a decorated function into a command that can be executed through the Ellar command-line interface (CLI) actions. 
 This allows you to define custom commands that can be run from the command-line, which can be useful for tasks such as running database migrations, generating code, or other tasks that can be automated.
 
 See [Ellar-CLI Custom Commands](https://eadwincode.github.io/ellar-cli/custom-commands/)
```

### Comparing `ellar-0.3.4/docs/overview/exception_handling.md` & `ellar-0.3.6/docs/overview/exception_handling.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/index.md` & `ellar-0.3.6/docs/overview/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/middleware.md` & `ellar-0.3.6/docs/overview/middleware.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/module-router.md` & `ellar-0.3.6/docs/overview/module-router.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/overview/modules.md` & `ellar-0.3.6/docs/overview/modules.md`

 * *Files 0% similar despite different names*

```diff
@@ -409,8 +409,8 @@
 During registration in `ApplicationModule`, we wrapped `MyModule` around a `ModuleSetup` and stated its dependencies in the `inject` property and also
 provided a `my_module_configuration_factory` factory that takes in module dependencies and return a `DynamicModule` configuration of `MyModule`.  
 
 When `AppFactory` starts module bootstrapping, `my_module_configuration_factory` will be called with 
 all the required **parameters** and returned a `DynamicModule` of `MyModule`.
 
 For more example, checkout [Ellar Throttle Module](https://github.com/eadwinCode/ellar-throttler/blob/master/ellar_throttler/module.py) 
-or [Ellar Cache Module]()
+or [Ellar Cache Module](../../caching)
```

### Comparing `ellar-0.3.4/docs/overview/providers.md` & `ellar-0.3.6/docs/overview/providers.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,30 @@
     def __init__(self, user_repo: UserRepository) -> None:
         self.user_repo = user_repo
 ```
 Let's refactor our `CarController` and move some actions to a service.
 
 ```python
 # project_name/apps/car/services.py
-import uuid
 import typing as t
 from ellar.di import injectable, singleton_scope
 from .schemas import CreateCarSerializer, CarSerializer
 
 
 @injectable(scope=singleton_scope)
 class CarRepository:
     def __init__(self):
         self._cars: t.List[CarSerializer] = []
 
-    def create_car(self, data: CreateCarSerializer) -> None:
-        self._cars.append(
-            CarSerializer(id=str(uuid.uuid4()), **data.dict())
-        )
-    
+    def create_car(self, data: CreateCarSerializer) -> dict:
+        data = CarSerializer(id=len(self._cars) + 1, **data.dict())
+        self._cars.append(data)
+        return data.dict()
+
+
     def get_all(self) -> t.List[CarSerializer]:
         return self._cars
 
 ```
 
 We have successfully created a `CarRepository` with a `singleton` scope.
 
@@ -74,16 +74,17 @@
 @Controller('/car')
 class CarController(ControllerBase):
     def __init__(self, repo: CarRepository):
         self.repo = repo
     
     @post()
     async def create(self, payload: CreateCarSerializer = Body()):
-        self.repo.create_car(payload)
-        return 'This action adds a new car'
+        result = self.repo.create_car(payload)
+        result.update(message='This action adds a new car')
+        return result
 
     @get()
     async def get_all(self, query: CarListFilter = Query()):
         res = dict(
             cars=self.repo.get_all(), 
             message=f'This action returns all cars at limit={query.limit}, offset={query.offset}')
         return res
```

### Comparing `ellar-0.3.4/docs/parsing-inputs/body.md` & `ellar-0.3.6/docs/parsing-inputs/body.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/cookie-params.md` & `ellar-0.3.6/docs/parsing-inputs/cookie-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/file-params.md` & `ellar-0.3.6/docs/parsing-inputs/file-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/form-params.md` & `ellar-0.3.6/docs/parsing-inputs/form-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/header-params.md` & `ellar-0.3.6/docs/parsing-inputs/header-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/index.md` & `ellar-0.3.6/docs/parsing-inputs/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/path-params.md` & `ellar-0.3.6/docs/parsing-inputs/path-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/parsing-inputs/query-params.md` & `ellar-0.3.6/docs/parsing-inputs/query-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/templating/staticfiles.md` & `ellar-0.3.6/docs/templating/staticfiles.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/docs/templating/templating.md` & `ellar-0.3.6/docs/templating/templating.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,18 @@
 and returns the rendered template as the `HTTP` response to the request.
 
 This example also shows manual setup of using `jinja2` in Ellar.
 
 
 ## **Jinja2 usage in Ellar**
 
-In Ellar, we use the `@render` decorator to convert the responses returned by the view to a Templated Response by creating an `HTMLResponseModel` with a status code of 200 to handle the response.
-Also, each registered `Module` is a `TemplateLoader` for loading templates available at `templates_folder`. And, a `Module` TemplateLoader object is created when the `template_folder` folder exists.
+In Ellar, the `@render` decorator transforms the route handler response into a Templated Response via an `HTMLResponseModel` with a status code of 200. 
+And the route handler is required to return a `dictionary` object which serves as the template's context.
 
-When using the `@render` decorator on a route handler, the function is expected to return a `dictionary` object which will be used as a template `context` to be generated.
+Additionally, each registered `Module` functions as a jinja2 `TemplateLoader` for loading templates, but only when a templates_folder is provided and exists.
 
 ### In Controller
 
 In Controllers, the `@render` decorator uses the decorated function name + controller name to generate a path to the template when creating `HTMLResponseModel` to handle the response
 
 For example:
 ```python
@@ -355,8 +355,8 @@
 In this case, when reversing the URL, you would use `request.url_for('users:user_profile', user_id=user_id)`
 which will generate `http://127.0.0.1:5000/template-reversing/profile/value_of_user_id` based on routing configuration.
 
 This allows for greater control and readability when reversing URLs, and makes it less prone to error if the function name of the route were to change in the future.
 
 
 ### Adding template filters and template globals.
-Jinja template filter and global functions can be defined at module level as shown here: [Module Templating Filters](../overview/modules/#module-templating-filters)
+Jinja template filter and global functions can be defined at module level as shown here: [Module Templating Filters](/ellar/overview/modules/#module-templating-filters)
```

### Comparing `ellar-0.3.4/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.3.6/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/base.py` & `ellar-0.3.6/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/local_cache.py` & `ellar-0.3.6/ellar/cache/backends/local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/pylib_cache.py` & `ellar-0.3.6/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/pymem_cache.py` & `ellar-0.3.6/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/redis/backend.py` & `ellar-0.3.6/ellar/cache/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/backends/serializer.py` & `ellar-0.3.6/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/decorator.py` & `ellar-0.3.6/ellar/cache/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/interface.py` & `ellar-0.3.6/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/make_key_decorator.py` & `ellar-0.3.6/ellar/cache/make_key_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/model.py` & `ellar-0.3.6/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/module.py` & `ellar-0.3.6/ellar/cache/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/schema.py` & `ellar-0.3.6/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/cache/service.py` & `ellar-0.3.6/ellar/cache/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/commands/base.py` & `ellar-0.3.6/ellar/commands/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/__init__.py` & `ellar-0.3.6/ellar/common/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import typing as t
 
 from ellar.core.params.params import Param, ParamTypes
 from ellar.core.routing import ModuleRouter
 
 from .decorators import (
     Controller,
+    Guards,
     Module,
+    Version,
     command,
     exception_handler,
     extra_args,
     file,
-    guards,
     middleware,
-    on_shutdown,
-    on_startup,
     openapi_info,
     render,
     serializer_filter,
     set_metadata,
     template_filter,
     template_global,
-    version,
 )
 from .routing import (
     Body,
     Context,
     Cookie,
     File,
     Form,
@@ -53,21 +51,21 @@
 )
 
 __all__ = [
     "command",
     "ModuleRouter",
     "render",
     "Module",
-    "guards",
+    "Guards",
     "Param",
     "ParamTypes",
     "set_metadata",
     "Controller",
     "openapi_info",
-    "version",
+    "Version",
     "delete",
     "get",
     "head",
     "http_route",
     "options",
     "patch",
     "post",
@@ -85,16 +83,14 @@
     "Context",
     "Provide",
     "Req",
     "Ws",
     "middleware",
     "exception_handler",
     "serializer_filter",
-    "on_shutdown",
-    "on_startup",
     "template_filter",
     "template_global",
     "Res",
     "Session",
     "Host",
     "Http",
     "UploadFile",
```

### Comparing `ellar-0.3.4/ellar/common/decorators/__init__.py` & `ellar-0.3.6/ellar/common/decorators/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 
 from .base import set_metadata
 from .command import command
 from .controller import Controller
 from .exception import exception_handler
 from .extra_args import extra_args
 from .file import file
-from .guards import guards
+from .guards import Guards
 from .html import render, template_filter, template_global
 from .middleware import middleware
 from .modules import Module
 from .openapi import openapi_info
-from .request import on_shutdown, on_startup
 from .serializer import serializer_filter
-from .versioning import version
+from .versioning import Version
 
 __all__ = [
     "serializer_filter",
     "Controller",
-    "version",
-    "guards",
+    "Version",
+    "Guards",
     "template_filter",
     "template_global",
     "file",
     "render",
-    "on_startup",
     "exception_handler",
-    "on_shutdown",
     "command",
     "set_metadata",
     "middleware",
     "openapi_info",
     "Module",
     "extra_args",
 ]
```

### Comparing `ellar-0.3.4/ellar/common/decorators/command.py` & `ellar-0.3.6/ellar/common/decorators/command.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/controller.py` & `ellar-0.3.6/ellar/common/decorators/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,25 @@
 
 from ellar.compatible import AttributeDict
 from ellar.constants import (
     CONTROLLER_CLASS_KEY,
     CONTROLLER_METADATA,
     CONTROLLER_OPERATION_HANDLER_KEY,
     CONTROLLER_WATERMARK,
-    GUARDS_KEY,
     NOT_SET,
     OPERATION_ENDPOINT_KEY,
     REFLECT_TYPE,
-    VERSIONING_KEY,
 )
 from ellar.core import ControllerBase
 from ellar.core.controller import ControllerType
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing.controller import ControllerRouteOperationBase
 from ellar.di import RequestScope, injectable
 from ellar.reflect import reflect
 
-if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.guard import GuardCanActivate
-
 
 def get_route_functions(
     cls: t.Type,
 ) -> t.Iterable[t.Union[t.Callable, ControllerRouteOperationBase]]:
     for method in cls.__dict__.values():
         if hasattr(method, OPERATION_ENDPOINT_KEY) or isinstance(
             method, ControllerRouteOperationBase
@@ -75,16 +70,14 @@
     prefix: t.Optional[str] = None,
     *,
     tag: str = NOT_SET,
     description: str = None,
     external_doc_description: str = None,
     external_doc_url: str = None,
     name: str = None,
-    version: t.Union[t.Tuple, str] = (),
-    guards: t.List[t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]] = None,
     include_in_schema: bool = True,
 ) -> t.Union[t.Type[ControllerBase], t.Callable[..., t.Any], t.Any]:  # pragma: no cover
     """
     ========= CLASS DECORATOR ==============
 
     Controller Class Decorator
     :param prefix: Route Prefix default=[ControllerName]
@@ -105,28 +98,24 @@
     prefix: t.Optional[str] = None,
     *,
     tag: str = NOT_SET,
     description: str = None,
     external_doc_description: str = None,
     external_doc_url: str = None,
     name: str = None,
-    version: t.Union[t.Tuple, str] = (),
-    guards: t.List[t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]] = None,
     include_in_schema: bool = True,
 ) -> t.Union[t.Type[ControllerBase], t.Callable[..., t.Any], t.Any]:
     """
     Controller Class Decorator
     :param prefix: Route Prefix default=[ControllerName]
     :param tag: OPENAPI tag
     :param description: OPENAPI description
     :param external_doc_description: OPENAPI External Doc Description
     :param external_doc_url: OPENAPI External Document URL
     :param name: route name prefix for url reversing, eg name:route_name default=controller_name
-    :param version: default URL versioning for all defined route in a controller
-    :param guards: default guard for all routes defined under this controller
     :param include_in_schema: include controller in OPENAPI schema
     :return: t.Type[ControllerBase]
     """
     _prefix: t.Optional[t.Any] = prefix if prefix is not None else NOT_SET
     if prefix and isinstance(prefix, type):
         _prefix = NOT_SET
 
@@ -140,16 +129,14 @@
             tag=tag,
             description=description,
             external_doc_description=external_doc_description,
             external_doc_url=external_doc_url,
         ),
         path=_prefix,
         name=name,
-        version=set([version] if isinstance(version, str) else version),
-        guards=guards or [],
         include_in_schema=include_in_schema,
     )
 
     def _decorator(cls: t.Type) -> t.Type[ControllerBase]:
         if not isinstance(cls, type):
             raise ImproperConfiguration(f"Controller is a class decorator - {cls}")
 
@@ -186,17 +173,14 @@
             reflect.define_metadata(CONTROLLER_WATERMARK, True, _controller_type)
             reflect_all_controller_type_routes(_controller_type)
             injectable(RequestScope)(cls)
 
             for key in CONTROLLER_METADATA.keys:
                 reflect.define_metadata(key, kwargs[key], _controller_type)
 
-            reflect.define_metadata(VERSIONING_KEY, kwargs.version, _controller_type)
-            reflect.define_metadata(GUARDS_KEY, kwargs.guards, _controller_type)
-
         if new_cls:
             # if we forced cls to inherit from ControllerBase, we need to block it from been processed
             setattr(cls, "__CONTROLLER_WATERMARK__", True)
 
         return _controller_type
 
     if callable(prefix):
```

### Comparing `ellar-0.3.4/ellar/common/decorators/exception.py` & `ellar-0.3.6/ellar/common/decorators/exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/extra_args.py` & `ellar-0.3.6/ellar/common/decorators/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/file.py` & `ellar-0.3.6/ellar/common/decorators/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/guards.py` & `ellar-0.3.6/ellar/common/decorators/guards.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from .base import set_metadata as set_meta
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.guard import GuardCanActivate
 
 
-def guards(
+def Guards(
     *_guards: t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]
 ) -> t.Callable:
     """
-    =========ROUTE FUNCTION DECORATOR ==============
+    =========CONTROLLER AND ROUTE FUNCTION DECORATOR ==============
 
     Defines list of guards for a route function
     :param _guards: Guard Type or Instance
     :return:
     """
     return set_meta(GUARDS_KEY, list(_guards))
```

### Comparing `ellar-0.3.4/ellar/common/decorators/html.py` & `ellar-0.3.6/ellar/common/decorators/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/middleware.py` & `ellar-0.3.6/ellar/common/decorators/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/modules.py` & `ellar-0.3.6/ellar/common/decorators/modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/openapi.py` & `ellar-0.3.6/ellar/common/decorators/openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/decorators/serializer.py` & `ellar-0.3.6/ellar/common/decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/routing/__init__.py` & `ellar-0.3.6/ellar/common/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/common/routing/params.py` & `ellar-0.3.6/ellar/common/routing/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/compatible/cache_properties.py` & `ellar-0.3.6/ellar/compatible/cache_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/compatible/dict.py` & `ellar-0.3.6/ellar/compatible/dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/compatible/emails.py` & `ellar-0.3.6/ellar/compatible/emails.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/constants.py` & `ellar-0.3.6/ellar/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,17 +60,14 @@
 OPENAPI_KEY = "OPENAPI"
 VERSIONING_KEY = "ROUTE_VERSIONING"
 GUARDS_KEY = "ROUTE_GUARDS"
 EXTRA_ROUTE_ARGS_KEY = "EXTRA_ROUTE_ARGS"
 RESPONSE_OVERRIDE_KEY = "RESPONSE_OVERRIDE"
 EXCEPTION_HANDLERS_KEY = "EXCEPTION_HANDLERS"
 
-ON_REQUEST_STARTUP_KEY = "ON_REQUEST_STARTUP"
-ON_REQUEST_SHUTDOWN_KEY = "ON_REQUEST_SHUTDOWN"
-
 TEMPLATE_GLOBAL_KEY = "TEMPLATE_GLOBAL_FILTERS"
 TEMPLATE_FILTER_KEY = "TEMPLATE_FILTERS"
 
 MIDDLEWARE_HANDLERS_KEY = "MIDDLEWARE"
 
 MODULE_WATERMARK = "MODULE_WATERMARK"
 MODULE_FIELDS = "__MODULE_FIELDS__"
```

### Comparing `ellar-0.3.4/ellar/core/__init__.py` & `ellar-0.3.6/ellar/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     PlainTextResponse,
     RedirectResponse,
     Response,
     StreamingResponse,
     UJSONResponse,
 )
 from .templating import render_template, render_template_string
-from .testclient import TestClient, TestClientFactory
 
 __all__ = [
     "App",
     "AppFactory",
     "render_template",
     "render_template_string",
     "ExecutionContext",
@@ -36,16 +35,14 @@
     "ModuleBase",
     "BaseAPIKey",
     "BaseAuthGuard",
     "IModuleSetup",
     "BaseHttpAuth",
     "GuardCanActivate",
     "Config",
-    "TestClientFactory",
-    "TestClient",
     "JSONResponse",
     "UJSONResponse",
     "ORJSONResponse",
     "StreamingResponse",
     "HTMLResponse",
     "FileResponse",
     "PlainTextResponse",
```

### Comparing `ellar-0.3.4/ellar/core/conf/app_settings_models.py` & `ellar-0.3.6/ellar/core/conf/app_settings_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,23 @@
 
 from ellar.constants import DEFAULT_LOGGING as default_logging, LOG_LEVELS as log_levels
 from ellar.core.response import JSONResponse, PlainTextResponse
 from ellar.core.versioning import DefaultAPIVersioning
 from ellar.serializer import Serializer, SerializerFilter
 from ellar.types import ASGIApp, TReceive, TScope, TSend
 
-from .mixins import (
-    ConfigDefaultTypesMixin,
-    TEventHandler,
-    TExceptionHandler,
-    TMiddleware,
-    TVersioning,
-)
+from .mixins import ConfigDefaultTypesMixin, TExceptionHandler, TMiddleware, TVersioning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.main import App
 
 
-async def _not_found(scope: TScope, receive: TReceive, send: TSend) -> None:
+async def _not_found(
+    scope: TScope, receive: TReceive, send: TSend
+) -> None:  # pragma: no cover
     if scope["type"] == "websocket":
         websocket_close = WebSocketClose()
         await websocket_close(scope, receive, send)
         return
 
     # If we're running inside a starlette application then raise an
     # exception, so that the configurable exception handler can deal with
@@ -109,17 +105,14 @@
     ] = encoders_by_type
 
     # logging configuration
     LOGGING_CONFIG: t.Optional[t.Dict[str, t.Any]] = default_logging
     # logging Level
     LOG_LEVEL: t.Optional[log_levels] = log_levels.info
 
-    ON_REQUEST_STARTUP: t.List[TEventHandler] = []
-    ON_REQUEST_SHUTDOWN: t.List[TEventHandler] = []
-
     TEMPLATE_FILTERS: t.Dict[str, t.Callable[..., t.Any]] = {}
     TEMPLATE_GLOBAL_FILTERS: t.Dict[str, t.Callable[..., t.Any]] = {}
 
     LOGGING: t.Optional[t.Dict[str, t.Any]] = None
     CACHES: t.Dict[str, t.Any] = {}
 
     @validator("MIDDLEWARE", pre=True)
```

### Comparing `ellar-0.3.4/ellar/core/conf/config.py` & `ellar-0.3.6/ellar/core/conf/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/conf/mixins.py` & `ellar-0.3.6/ellar/core/conf/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import inspect
 import typing as t
 
 from starlette.responses import JSONResponse
 from starlette.types import ASGIApp
 
 from ellar.constants import LOG_LEVELS as log_levels
-from ellar.core.events import EventHandler
 from ellar.core.exceptions.interfaces import IExceptionHandler
 from ellar.core.middleware import Middleware
 from ellar.core.versioning import BaseAPIVersioning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core import App
 
 __all__ = [
     "ConfigDefaultTypesMixin",
     "TVersioning",
     "TMiddleware",
-    "TEventHandler",
     "TExceptionHandler",
 ]
 
 
 class TExceptionHandler:
     @classmethod
     def __get_validators__(
@@ -66,26 +64,26 @@
         if not isinstance(v, Middleware):
             raise ValueError(
                 f"Expected Type/instance of Middleware, received: {type(v)}"
             )
         return v
 
 
-class TEventHandler(EventHandler):
-    @classmethod
-    def __get_validators__(
-        cls: t.Type["TEventHandler"],
-    ) -> t.Iterable[t.Callable[..., t.Any]]:
-        yield cls.validate
-
-    @classmethod
-    def validate(cls: t.Type["EventHandler"], v: t.Any) -> t.Any:
-        if not isinstance(v, EventHandler):
-            raise ValueError(f"Expected EventHandler, received: {type(v)}")
-        return v
+# class TEventHandler(EventHandler):
+#     @classmethod
+#     def __get_validators__(
+#         cls: t.Type["TEventHandler"],
+#     ) -> t.Iterable[t.Callable[..., t.Any]]:
+#         yield cls.validate
+#
+#     @classmethod
+#     def validate(cls: t.Type["EventHandler"], v: t.Any) -> t.Any:
+#         if not isinstance(v, EventHandler):
+#             raise ValueError(f"Expected EventHandler, received: {type(v)}")
+#         return v
 
 
 class ConfigDefaultTypesMixin:
     SECRET_KEY: str
     DEBUG: bool
     # injector auto_bind = True allows you to resolve types that are not registered on the container
     # For more info, read: https://injector.readthedocs.io/en/latest/index.html
@@ -122,20 +120,14 @@
 
     # static route
     STATIC_MOUNT_PATH: str
 
     # defines other custom json encoders
     SERIALIZER_CUSTOM_ENCODER: t.Dict[t.Any, t.Callable[[t.Any], t.Any]]
 
-    # will be set automatically when @on_startup is found in a Module class
-    ON_REQUEST_STARTUP: t.List[TEventHandler]
-
-    # will be set automatically when @on_shutdown is found in a Module class
-    ON_REQUEST_SHUTDOWN: t.List[TEventHandler]
-
     # will be set automatically when @template_filter is found in a Module class
     TEMPLATE_FILTERS: t.Dict[str, t.Callable[..., t.Any]]
 
     # will be set automatically when @template_global is found in a Module class
     TEMPLATE_GLOBAL_FILTERS: t.Dict[str, t.Callable[..., t.Any]]
 
     # Default not found handler
```

### Comparing `ellar-0.3.4/ellar/core/connection/http.py` & `ellar-0.3.6/ellar/core/connection/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/__init__.py` & `ellar-0.3.6/ellar/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/execution.py` & `ellar-0.3.6/ellar/core/context/execution.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/factory.py` & `ellar-0.3.6/ellar/core/context/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/host.py` & `ellar-0.3.6/ellar/core/context/host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/http.py` & `ellar-0.3.6/ellar/core/context/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/interface.py` & `ellar-0.3.6/ellar/core/context/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/context/websocket.py` & `ellar-0.3.6/ellar/core/context/websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/controller/model.py` & `ellar-0.3.6/ellar/core/controller/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/converters.py` & `ellar-0.3.6/ellar/core/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/datastructures.py` & `ellar-0.3.6/ellar/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/events.py` & `ellar-0.3.6/ellar/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/exceptions/base.py` & `ellar-0.3.6/ellar/core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/exceptions/callable_exceptions.py` & `ellar-0.3.6/ellar/core/exceptions/callable_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 from starlette.concurrency import run_in_threadpool
 from starlette.responses import Response
 
+from ellar.core.context import IHostContext
 from ellar.helper import is_async_callable
 
-from ..context import IHostContext
 from .interfaces import IExceptionHandler
 
 
 class CallableExceptionHandler(IExceptionHandler):
     """
     Default Exception Handler Setup for functions
```

### Comparing `ellar-0.3.4/ellar/core/exceptions/handlers.py` & `ellar-0.3.6/ellar/core/exceptions/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from starlette.exceptions import (
     HTTPException as StarletteHTTPException,
     WebSocketException as StarletteWebSocketException,
 )
 from starlette.responses import Response
 
 from ellar.core.context import IHostContext
-from ellar.core.exceptions import APIException, RequestValidationError
 from ellar.serializer import serialize_object
 
+from .base import APIException
 from .interfaces import IExceptionHandler
+from .validation import RequestValidationError
 
 
 class HTTPExceptionHandler(IExceptionHandler):
     exception_type_or_code = StarletteHTTPException
 
     async def catch(
         self, ctx: IHostContext, exc: StarletteHTTPException
```

### Comparing `ellar-0.3.4/ellar/core/exceptions/interfaces.py` & `ellar-0.3.6/ellar/core/exceptions/interfaces.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/exceptions/service.py` & `ellar-0.3.6/ellar/core/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/exceptions/validation.py` & `ellar-0.3.6/ellar/core/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/factory.py` & `ellar-0.3.6/ellar/core/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from collections import OrderedDict
 from pathlib import Path
 from uuid import uuid4
 
 from starlette.routing import Host, Mount
 
 from ellar.constants import MODULE_METADATA, MODULE_WATERMARK
-from ellar.core import Config
 from ellar.core.main import App
 from ellar.core.modules import DynamicModule, ModuleBase, ModuleSetup
 from ellar.di import EllarInjector, ProviderConfig
 from ellar.reflect import reflect
 
-from .services import CoreServiceRegistration
+from .conf import Config
+from .core_service_registration import CoreServiceRegistration
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.commands import EllarTyper
     from ellar.core import GuardCanActivate
     from ellar.core.routing import ModuleMount, ModuleRouter
 
 
@@ -46,29 +46,30 @@
         """
         modules = (
             reflect.get_metadata(MODULE_METADATA.MODULES, module_config.module) or []
         )
         module_dependency = OrderedDict()
         for module in modules:
             if isinstance(module, DynamicModule):
+                module.apply_configuration()
                 module_config = ModuleSetup(module.module)
             elif isinstance(module, ModuleSetup):
                 module_config = module
             else:
                 module_config = ModuleSetup(module)
 
             module_dependency[module_config.module] = module_config
             module_dependency.update(cls.read_all_module(module_config))
         return module_dependency
 
     @classmethod
     def _build_modules(
         cls,
         app_module: t.Type[t.Union[ModuleBase, t.Any]],
-        config: Config,
+        config: "Config",
         injector: EllarInjector,
     ) -> None:
         """
         builds application module and registers them to EllarInjector
         :param app_module: Root App Module
         :param config: App Configuration instance
         :param injector: App Injector instance
@@ -132,22 +133,17 @@
         config = Config(app_configured=True, **_get_config_kwargs())
         injector = EllarInjector(auto_bind=config.INJECTOR_AUTO_BIND)
         injector.container.register_instance(config, concrete_type=Config)
         CoreServiceRegistration(injector, config).register_all()
 
         cls._build_modules(app_module=module, injector=injector, config=config)
 
-        shutdown_event = config.ON_REQUEST_STARTUP
-        startup_event = config.ON_REQUEST_SHUTDOWN
-
         app = App(
             config=config,
             injector=injector,
-            on_shutdown_event_handlers=shutdown_event if shutdown_event else None,
-            on_startup_event_handlers=startup_event if startup_event else None,
             lifespan=config.DEFAULT_LIFESPAN_HANDLER,
             global_guards=global_guards,
         )
 
         routes = []
         module_changed = False
```

### Comparing `ellar-0.3.4/ellar/core/guard/apikey.py` & `ellar-0.3.6/ellar/core/guard/apikey.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/guard/base.py` & `ellar-0.3.6/ellar/core/guard/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class GuardCanActivate(ABC, metaclass=ABCMeta):
     exception_class: t.Union[
         t.Type[HTTPException], t.Type[APIException]
     ] = HTTPException
     status_code: int = HTTP_403_FORBIDDEN
-    detail: str = "Not authenticated"
+    detail: str = "Forbidden"
 
     @abstractmethod
     async def can_activate(self, context: IExecutionContext) -> bool:
         pass
 
     def raise_exception(self) -> None:
         raise self.exception_class(status_code=self.status_code, detail=self.detail)
```

### Comparing `ellar-0.3.4/ellar/core/guard/http.py` & `ellar-0.3.6/ellar/core/guard/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/main.py` & `ellar-0.3.6/ellar/core/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 import typing as t
 
 from starlette.routing import BaseRoute, Mount
 
 from ellar.constants import LOG_LEVELS
-from ellar.core.conf import Config
 from ellar.core.datastructures import State, URLPath
-from ellar.core.events import EventHandler, RouterEventManager
 from ellar.core.exceptions.interfaces import (
     IExceptionHandler,
     IExceptionMiddlewareService,
 )
 from ellar.core.guard import GuardCanActivate
 from ellar.core.middleware import (
     CORSMiddleware,
@@ -25,75 +23,54 @@
     ModuleBase,
     ModuleRefBase,
     ModuleSetup,
     ModuleTemplateRef,
 )
 from ellar.core.routing import ApplicationRouter
 from ellar.core.templating import AppTemplating, Environment
-from ellar.core.versioning import VERSIONING, BaseAPIVersioning
+from ellar.core.versioning import BaseAPIVersioning, VersioningSchemes
 from ellar.di.injector import EllarInjector
 from ellar.logger import logger
 from ellar.types import ASGIApp, T, TReceive, TScope, TSend
 
+from .conf import Config
+
 
 class App(AppTemplating):
     def __init__(
         self,
-        config: Config,
+        config: "Config",
         injector: EllarInjector,
-        on_startup_event_handlers: t.Optional[t.Sequence[EventHandler]] = None,
-        on_shutdown_event_handlers: t.Optional[t.Sequence[EventHandler]] = None,
         lifespan: t.Optional[t.Callable[["App"], t.AsyncContextManager]] = None,
         global_guards: t.List[
             t.Union[t.Type[GuardCanActivate], GuardCanActivate]
         ] = None,
     ):
         assert isinstance(config, Config), "config must instance of Config"
         assert isinstance(
             injector, EllarInjector
         ), "injector must instance of EllarInjector"
 
-        # The lifespan context function is a newer style that replaces
-        # on_startup / on_shutdown handlers. Use one or the other, not both.
-        assert lifespan is None or (
-            on_startup_event_handlers is None and on_shutdown_event_handlers is None
-        ), "Use either 'lifespan' or 'on_startup'/'on_shutdown', not both."
-
         self._config = config
         self._injector: EllarInjector = injector
 
         self._global_guards = [] if global_guards is None else list(global_guards)
         self._exception_handlers = list(self.config.EXCEPTION_HANDLERS)
 
         self._user_middleware = list(t.cast(list, self.config.MIDDLEWARE))
 
-        self.on_startup = RouterEventManager(
-            [] if on_startup_event_handlers is None else list(on_startup_event_handlers)
-        )
-        self.on_shutdown = RouterEventManager(
-            []
-            if on_shutdown_event_handlers is None
-            else list(on_shutdown_event_handlers)
-        )
-
         self._static_app: t.Optional[ASGIApp] = None
 
         self.state = State()
         self.config.DEFAULT_LIFESPAN_HANDLER = (
             lifespan or self.config.DEFAULT_LIFESPAN_HANDLER
         )
         self.router = ApplicationRouter(
             routes=self._get_module_routes(),
             redirect_slashes=self.config.REDIRECT_SLASHES,
-            on_startup=[self.on_startup.async_run]
-            if self.config.DEFAULT_LIFESPAN_HANDLER is None
-            else None,
-            on_shutdown=[self.on_shutdown.async_run]
-            if self.config.DEFAULT_LIFESPAN_HANDLER is None
-            else None,
             default=self.config.DEFAULT_NOT_FOUND_HANDLER,  # type: ignore
             lifespan=self.config.DEFAULT_LIFESPAN_HANDLER,
         )
         self.middleware_stack = self.build_middleware_stack()
         self._finalize_app_initialization()
         self._config_logging()
 
@@ -134,14 +111,15 @@
 
     def install_module(
         self,
         module: t.Union[t.Type[T], t.Type[ModuleBase], DynamicModule],
         **init_kwargs: t.Any,
     ) -> t.Union[T, ModuleBase]:
         if isinstance(module, DynamicModule):
+            module.apply_configuration()
             module_config = ModuleSetup(module.module, init_kwargs=init_kwargs)
         else:
             module_config = ModuleSetup(module, init_kwargs=init_kwargs)
 
         module_ref = self.injector.get_module(module_config.module)
         if module_ref:
             return module_ref.get_module_instance()
@@ -181,15 +159,15 @@
     @property
     def has_static_files(self) -> bool:  # type: ignore
         return (
             True if self.static_files or self.config.STATIC_FOLDER_PACKAGES else False
         )
 
     @property
-    def config(self) -> Config:  # type: ignore
+    def config(self) -> "Config":  # type: ignore
         return self._config
 
     def build_middleware_stack(self) -> ASGIApp:
         service_middleware = self.injector.get(IExceptionMiddlewareService)
         service_middleware.build_exception_handlers(*self._exception_handlers)
         error_handler = service_middleware.get_500_error_handler()
         allowed_hosts = self.config.ALLOWED_HOSTS
@@ -248,15 +226,15 @@
         return self.router.routes.get_routes()
 
     def url_path_for(self, name: str, **path_params: t.Any) -> URLPath:
         return self.router.url_path_for(name, **path_params)
 
     def enable_versioning(
         self,
-        schema: VERSIONING,
+        schema: VersioningSchemes,
         version_parameter: str = "version",
         default_version: t.Optional[str] = None,
         **init_kwargs: t.Any,
     ) -> None:
         self.config.VERSIONING_SCHEME = schema.value(
             version_parameter=version_parameter,
             default_version=default_version,
```

### Comparing `ellar-0.3.4/ellar/core/middleware/__init__.py` & `ellar-0.3.6/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/middleware/di.py` & `ellar-0.3.6/ellar/core/middleware/di.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/middleware/exceptions.py` & `ellar-0.3.6/ellar/core/middleware/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from starlette.exceptions import HTTPException
 
 from ellar.constants import SCOPE_SERVICE_PROVIDER
 from ellar.core.context import IHostContextFactory
 from ellar.types import ASGIApp, TMessage, TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.exceptions.service import ExceptionMiddlewareService
     from ellar.di import EllarInjector
+    from ellar.exceptions.service import ExceptionMiddlewareService
 
 
 class ExceptionMiddleware:
     def __init__(
         self,
         app: ASGIApp,
         exception_middleware_service: "ExceptionMiddlewareService",
```

### Comparing `ellar-0.3.4/ellar/core/middleware/function.py` & `ellar-0.3.6/ellar/core/middleware/function.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/middleware/versioning.py` & `ellar-0.3.6/ellar/core/middleware/versioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from starlette.types import ASGIApp
 
 from ellar.constants import SCOPE_API_VERSIONING_RESOLVER
 from ellar.core.versioning import BaseAPIVersioning
 from ellar.types import TReceive, TScope, TSend
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core.conf import Config
+    from ellar.conf import Config
 
 
 class RequestVersioningMiddleware:
     def __init__(self, app: ASGIApp, *, debug: bool, config: "Config") -> None:
         self.app = app
         self.debug = debug
         self.config = config
```

### Comparing `ellar-0.3.4/ellar/core/modules/base.py` & `ellar-0.3.6/ellar/core/modules/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import typing as t
 
 from injector import Binder, Module as _InjectorModule
 
 from ellar.constants import MODULE_FIELDS
-from ellar.core.conf import Config
 from ellar.core.modules.builder import ModuleBaseBuilder
 from ellar.di.injector import Container
 
+if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.conf import Config
+
 
 class ModuleBaseMeta(type):
     __MODULE_FIELDS__: t.Dict = {}
 
     @t.no_type_check
     def __init__(cls, name, bases, namespace) -> None:
         super().__init__(name, bases, namespace)
@@ -19,15 +21,15 @@
         for base in reversed(bases):
             ModuleBaseBuilder(cls).build(getattr(base, MODULE_FIELDS, dict()))
         ModuleBaseBuilder(cls).build(namespace)
 
 
 class ModuleBase(_InjectorModule, metaclass=ModuleBaseMeta):
     @classmethod
-    def before_init(cls, config: Config) -> t.Dict:
+    def before_init(cls, config: "Config") -> t.Dict:
         """Before Module initialisation. Whatever value that is returned here will be passed
         to the Module constructor during initialisation"""
         return {}
 
     def register_services(self, container: Container) -> None:
         """Register other services manually"""
```

### Comparing `ellar-0.3.4/ellar/core/modules/config.py` & `ellar-0.3.6/ellar/core/modules/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
 import typing as t
 
 from starlette.routing import BaseRoute
 
-import ellar.core.conf as conf
 import ellar.core.main as main
 import ellar.di as di
 from ellar.constants import MODULE_METADATA, MODULE_REF_TYPES
+from ellar.core.conf import Config
 from ellar.reflect import reflect
 
 from .base import ModuleBase
 from .ref import ModuleRefBase, create_module_ref_factor
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.commands import EllarTyper
@@ -33,19 +33,24 @@
     routers: t.Sequence[t.Union[BaseRoute]] = dataclasses.field(
         default_factory=lambda: tuple()
     )
 
     commands: t.Sequence[t.Union[t.Callable, "EllarTyper"]] = dataclasses.field(
         default_factory=lambda: tuple()
     )
+    _is_configured: bool = False
 
     def __post_init__(self) -> None:
         if not isinstance(self.module, type) or not issubclass(self.module, ModuleBase):
             raise Exception(f"{self.module.__name__} is not a valid Module")
 
+    def apply_configuration(self) -> None:
+        if self._is_configured:
+            return
+
         kwargs = dict(
             controllers=list(self.controllers),
             routers=list(self.routers),
             providers=list(self.providers),
             commands=list(self.commands),
         )
         for key in [
@@ -55,14 +60,16 @@
             MODULE_METADATA.COMMANDS,
         ]:
             value = kwargs[key]
             if value:
                 reflect.delete_metadata(key, self.module)
                 reflect.define_metadata(key, value, self.module)
 
+        self._is_configured = True
+
 
 @dataclasses.dataclass
 class ModuleSetup:
     """
     ModuleSetup is a way to configure a module based on its dependencies.
     This is necessary for Module that requires some services available to configure them.
     For example:
@@ -111,42 +118,43 @@
             # if we have a factory function, we need to check if the services to inject is just config
             # if so, then we can go ahead and have the configuration executed since at this level,
             # the config service is available to be injected.
             inject_size = len(self.inject)
             if inject_size == 0:
                 return False
 
-            if inject_size == 1 and self.inject[0] == conf.Config:
+            if inject_size == 1 and self.inject[0] == Config:
                 return False
             return True
 
     def get_module_ref(
-        self, config: conf.Config, container: di.Container
+        self, config: "Config", container: di.Container
     ) -> t.Union[ModuleRefBase, "ModuleSetup"]:
         if self.has_factory_function or self.ref_type == MODULE_REF_TYPES.APP_DEPENDENT:
             return self
 
         if self.factory:
             return self.configure_with_factory(config, container)
 
         return create_module_ref_factor(
             self.module, config, container, **self.init_kwargs
         )
 
     def configure_with_factory(
-        self, config: conf.Config, container: di.Container
+        self, config: "Config", container: di.Container
     ) -> ModuleRefBase:
         services = self._get_services(container.injector)
 
         res = self.factory(self.module, *services)
         if not isinstance(res, DynamicModule):
             raise Exception(
                 f"Factory function for {self.module.__name__} module "
                 f"configuration must return `DynamicModule` instance"
             )
+        res.apply_configuration()
 
         init_kwargs = dict(self.init_kwargs)
         return create_module_ref_factor(self.module, config, container, **init_kwargs)
 
     def _get_services(self, injector: di.EllarInjector) -> t.List:
         """
         Get list of services to be injected to the factory function.
```

### Comparing `ellar-0.3.4/ellar/core/modules/helper.py` & `ellar-0.3.6/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/modules/ref.py` & `ellar-0.3.6/ellar/core/modules/ref.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,41 +8,38 @@
 from ellar.constants import (
     CONTROLLER_WATERMARK,
     EXCEPTION_HANDLERS_KEY,
     MIDDLEWARE_HANDLERS_KEY,
     MODULE_METADATA,
     MODULE_REF_TYPES,
     MODULE_WATERMARK,
-    ON_REQUEST_SHUTDOWN_KEY,
-    ON_REQUEST_STARTUP_KEY,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
 from ellar.core.controller import ControllerType
 from ellar.core.routing import ModuleMount
 from ellar.core.routing.router.module import controller_router_factory
 from ellar.core.templating import ModuleTemplating
 from ellar.di import Container, ProviderConfig, injectable, is_decorated_with_injectable
 from ellar.di.providers import ModuleProvider
 from ellar.reflect import reflect
 
-from .. import Config
 from .base import ModuleBase, ModuleBaseMeta
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.core import ControllerBase
+    from ellar.core import Config, ControllerBase
 
 
 class InvalidModuleTypeException(Exception):
     pass
 
 
 def create_module_ref_factor(
     module_type: t.Union[t.Type, t.Type[ModuleBase]],
-    config: Config,
+    config: "Config",
     container: Container,
     **init_kwargs: t.Any,
 ) -> t.Union["ModuleRefBase", "ModuleTemplateRef"]:
     module_ref: t.Union["ModuleRefBase", "ModuleTemplateRef"]
     if reflect.get_metadata(MODULE_WATERMARK, module_type):
         module_ref = ModuleTemplateRef(
             module_type,
@@ -70,15 +67,15 @@
     @property
     @abstractmethod
     def container(self) -> Container:
         """gets module ref container"""
 
     @property
     @abstractmethod
-    def config(self) -> Config:
+    def config(self) -> "Config":
         """gets module ref config"""
 
     @property
     @abstractmethod
     def module(self) -> t.Union[t.Type[ModuleBase], t.Type]:
         """gets module ref container"""
 
@@ -117,15 +114,15 @@
     ref_type: str = MODULE_REF_TYPES.PLAIN
 
     def __init__(
         self,
         module_type: t.Union[t.Type[ModuleBase], t.Type],
         *,
         container: Container,
-        config: Config,
+        config: "Config",
         **kwargs: t.Any,
     ) -> None:
         assert (
             type(module_type) == ModuleBaseMeta
         ), f"Module Type must be a subclass of ModuleBase;\n Invalid Type[{module_type}]"
         self._module_type: t.Type[ModuleBase] = module_type
         self._init_kwargs = self._build_init_kwargs(kwargs)
@@ -138,15 +135,15 @@
         return self._module_type
 
     @property
     def container(self) -> Container:
         return self._container
 
     @property
-    def config(self) -> Config:
+    def config(self) -> "Config":
         return self._config
 
     def _register_module(self) -> None:
         _module = self.module
         if not is_decorated_with_injectable(self.module):
             _module = injectable()(self.module)
         self.container.register(
@@ -158,15 +155,15 @@
     ref_type: str = MODULE_REF_TYPES.TEMPLATE
 
     def __init__(
         self,
         module_type: t.Union[t.Type[ModuleBase], t.Type],
         *,
         container: Container,
-        config: Config,
+        config: "Config",
         **kwargs: t.Any,
     ) -> None:
         assert (
             type(module_type) == ModuleBaseMeta
         ), f"Module Type must be a subclass of ModuleBase;\n Invalid Type[{module_type}]"
 
         self._module_type: t.Type[ModuleBase] = module_type
@@ -190,15 +187,14 @@
 
         self._routers: t.Sequence[
             t.Union[BaseRoute, ModuleMount, Mount]
         ] = self._get_all_routers()
         self._flatten_routes: t.List[BaseRoute] = []
 
         self.scan_templating_filters()
-        self.scan_request_events()
         self.scan_exceptions_handlers()
         self.scan_middleware()
         self.register_providers()
         self.register_controllers()
         self._build_flatten_routes()
 
     @property
@@ -206,15 +202,15 @@
         return self._module_type
 
     @property
     def container(self) -> Container:
         return self._container
 
     @property
-    def config(self) -> Config:
+    def config(self) -> "Config":
         return self._config
 
     @property
     def routers(self) -> t.Sequence[t.Union[BaseRoute, ModuleMount, Mount]]:
         return self._routers
 
     @property
@@ -297,26 +293,7 @@
         )
         for controller in self._controllers:
             assert reflect.get_metadata(
                 CONTROLLER_WATERMARK, controller
             ) and isinstance(controller, ControllerType), "Invalid Controller Type."
             _routers.append(controller_router_factory(controller))
         return _routers
-
-    def scan_request_events(self) -> None:
-        request_startup = (
-            reflect.get_metadata(ON_REQUEST_STARTUP_KEY, self._module_type) or []
-        )
-        if not self._config.get(ON_REQUEST_STARTUP_KEY) or not isinstance(
-            self._config[ON_REQUEST_STARTUP_KEY], list
-        ):
-            self._config[ON_REQUEST_STARTUP_KEY] = []
-        self._config[ON_REQUEST_STARTUP_KEY].extend(request_startup)
-
-        request_shutdown = (
-            reflect.get_metadata(ON_REQUEST_SHUTDOWN_KEY, self._module_type) or []
-        )
-        if not self._config.get(ON_REQUEST_SHUTDOWN_KEY) or not isinstance(
-            self._config[ON_REQUEST_SHUTDOWN_KEY], list
-        ):
-            self._config[ON_REQUEST_SHUTDOWN_KEY] = []
-        self._config[ON_REQUEST_SHUTDOWN_KEY].extend(request_shutdown)
```

### Comparing `ellar-0.3.4/ellar/core/params/__init__.py` & `ellar-0.3.6/ellar/core/params/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/base.py` & `ellar-0.3.6/ellar/core/params/args/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/extra_args.py` & `ellar-0.3.6/ellar/core/params/args/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/factory.py` & `ellar-0.3.6/ellar/core/params/args/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/request_model.py` & `ellar-0.3.6/ellar/core/params/args/request_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/resolver_generators.py` & `ellar-0.3.6/ellar/core/params/args/resolver_generators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/args/websocket_model.py` & `ellar-0.3.6/ellar/core/params/args/websocket_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/helpers.py` & `ellar-0.3.6/ellar/core/params/helpers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/params.py` & `ellar-0.3.6/ellar/core/params/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/__init__.py` & `ellar-0.3.6/ellar/core/params/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/base.py` & `ellar-0.3.6/ellar/core/params/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/bulk_parameter.py` & `ellar-0.3.6/ellar/core/params/resolvers/bulk_parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/non_parameter/__init__.py` & `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/non_parameter/base.py` & `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/non_parameter/inject.py` & `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/inject.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/non_parameter/session.py` & `ellar-0.3.6/ellar/core/params/resolvers/non_parameter/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/params/resolvers/parameter.py` & `ellar-0.3.6/ellar/core/params/resolvers/parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/__init__.py` & `ellar-0.3.6/ellar/core/response/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/__init__.py` & `ellar-0.3.6/ellar/core/response/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/base.py` & `ellar-0.3.6/ellar/core/response/model/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/factory.py` & `ellar-0.3.6/ellar/core/response/model/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/file.py` & `ellar-0.3.6/ellar/core/response/model/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/html.py` & `ellar-0.3.6/ellar/core/response/model/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/interface.py` & `ellar-0.3.6/ellar/core/response/model/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/json.py` & `ellar-0.3.6/ellar/core/response/model/json.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/model/route.py` & `ellar-0.3.6/ellar/core/response/model/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/response/response_types.py` & `ellar-0.3.6/ellar/core/response/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/base.py` & `ellar-0.3.6/ellar/core/routing/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/controller/base.py` & `ellar-0.3.6/ellar/core/routing/controller/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/controller/route.py` & `ellar-0.3.6/ellar/core/routing/controller/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/controller/websocket/handler.py` & `ellar-0.3.6/ellar/core/routing/controller/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/controller/websocket/route.py` & `ellar-0.3.6/ellar/core/routing/controller/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/operation_definitions.py` & `ellar-0.3.6/ellar/core/routing/operation_definitions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,80 @@
+import functools
 import typing as t
 from functools import partial
+from types import FunctionType
 
 from ellar.constants import (
+    CONTROLLER_OPERATION_HANDLER_KEY,
     DELETE,
     GET,
     HEAD,
     OPERATION_ENDPOINT_KEY,
     OPTIONS,
     PATCH,
     POST,
     PUT,
     TRACE,
 )
 from ellar.core.schema import RouteParameters, WsRouteParameters
 from ellar.helper import class_base_function_regex
+from ellar.reflect import reflect
 from ellar.types import TCallable
 
 from .controller.route import ControllerRouteOperation
 from .controller.websocket.route import ControllerWebsocketRouteOperation
 from .route import RouteOperation
 from .websocket import WebsocketRouteOperation
 
 TOperation = t.Union[RouteOperation, ControllerRouteOperation]
 TWebsocketOperation = t.Union[
     WebsocketRouteOperation, ControllerWebsocketRouteOperation
 ]
 
 
+def _websocket_connection_attributes(func: t.Callable) -> t.Callable:
+    def _advance_function(
+        websocket_handler: t.Callable, handler_name: str
+    ) -> t.Callable:
+        def _wrap(connect_handler: t.Callable) -> t.Callable:
+            if not (
+                callable(websocket_handler) and type(websocket_handler) == FunctionType
+            ):
+                raise Exception(
+                    "Invalid type. Please make sure you passed the websocket handler."
+                )
+
+            _item: t.Optional[WebsocketRouteOperation] = reflect.get_metadata(
+                CONTROLLER_OPERATION_HANDLER_KEY, websocket_handler
+            )
+
+            if not _item or not isinstance(_item, WebsocketRouteOperation):
+                raise Exception(
+                    "Invalid type. Please make sure you passed the websocket handler."
+                )
+
+            _item.add_websocket_handler(
+                handler_name=handler_name, handler=connect_handler
+            )
+
+            return connect_handler
+
+        return _wrap
+
+    setattr(
+        func, "connect", functools.partial(_advance_function, handler_name="on_connect")
+    )
+    setattr(
+        func,
+        "disconnect",
+        functools.partial(_advance_function, handler_name="on_disconnect"),
+    )
+    return func
+
+
 class OperationDefinitions:
     __slots__ = ()
 
     def _get_http_operations_class(self, func: t.Callable) -> t.Type[TOperation]:
         if class_base_function_regex.match(repr(func)):
             return ControllerRouteOperation
         return RouteOperation
@@ -76,15 +120,15 @@
     def get(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [GET]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -96,15 +140,15 @@
     def post(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [POST]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -116,15 +160,15 @@
     def put(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [PUT]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -136,15 +180,15 @@
     def patch(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [PATCH]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -156,15 +200,15 @@
     def delete(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [DELETE]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -176,15 +220,15 @@
     def head(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [HEAD]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -196,15 +240,15 @@
     def options(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [OPTIONS]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -216,15 +260,15 @@
     def trace(
         self,
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         methods = [TRACE]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
@@ -237,15 +281,15 @@
         self,
         path: str = "/",
         *,
         methods: t.List[str],
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
-            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, None
+            t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
     ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
         def _decorator(endpoint_handler: TCallable) -> TCallable:
             endpoint_parameter = RouteParameters(
                 name=name,
                 path=path,
                 methods=methods,
@@ -254,14 +298,15 @@
                 endpoint=endpoint_handler,
             )
             self._get_operation(route_parameter=endpoint_parameter)
             return endpoint_handler
 
         return _decorator
 
+    @_websocket_connection_attributes
     def ws_route(
         self,
         path: str = "/",
         *,
         name: str = None,
         encoding: t.Optional[str] = "json",
         use_extra_handler: bool = False,
@@ -274,13 +319,11 @@
                 name=name,
                 path=path,
                 endpoint=endpoint_handler,
                 encoding=encoding,
                 use_extra_handler=use_extra_handler,
                 extra_handler_type=extra_handler_type,
             )
-            operation = self._get_ws_operation(ws_route_parameters=endpoint_parameter)
-            if use_extra_handler:
-                return operation
+            self._get_ws_operation(ws_route_parameters=endpoint_parameter)
             return endpoint_handler
 
         return _decorator
```

### Comparing `ellar-0.3.4/ellar/core/routing/route.py` & `ellar-0.3.6/ellar/core/routing/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/router/app.py` & `ellar-0.3.6/ellar/core/routing/router/app.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/router/module.py` & `ellar-0.3.6/ellar/core/routing/router/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     controller: t.Union[t.Type[ControllerBase], t.Any]
 ) -> "ModuleMount":
     openapi = reflect.get_metadata(CONTROLLER_METADATA.OPENAPI, controller) or dict()
     routes = reflect.get_metadata(CONTROLLER_OPERATION_HANDLER_KEY, controller) or []
     app = Router()
     app.routes = RouteCollection(routes)  # type:ignore
 
-    reflect.get_metadata_or_raise_exception(VERSIONING_KEY, controller)
     include_in_schema = reflect.get_metadata_or_raise_exception(
         CONTROLLER_METADATA.INCLUDE_IN_SCHEMA, controller
     )
     router = ModuleMount(
         app=app,
         path=reflect.get_metadata_or_raise_exception(
             CONTROLLER_METADATA.PATH, controller
```

### Comparing `ellar-0.3.4/ellar/core/routing/router/route_collections.py` & `ellar-0.3.6/ellar/core/routing/router/route_collections.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/websocket/handler.py` & `ellar-0.3.6/ellar/core/routing/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/routing/websocket/route.py` & `ellar-0.3.6/ellar/core/routing/websocket/route.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,28 @@
 from starlette.websockets import WebSocketState
 
 from ellar.constants import (
     CONTROLLER_OPERATION_HANDLER_KEY,
     EXTRA_ROUTE_ARGS_KEY,
     NOT_SET,
 )
-from ellar.core.connection import WebSocket
 from ellar.core.context import IExecutionContext
 from ellar.core.exceptions import ImproperConfiguration, WebSocketRequestValidationError
 from ellar.core.params import WebsocketEndpointArgsModel
 from ellar.helper import get_name
 from ellar.reflect import reflect
 
 from ..base import WebsocketRouteOperationBase
 from .handler import WebSocketExtraHandler
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.params import ExtraEndpointArg
 
 
-class WebSocketOperationMixin:
-    _handlers_kwargs: t.Dict
-
-    def connect(self, func: t.Callable[[WebSocket], None]) -> t.Callable:
-        self._handlers_kwargs.update(on_connect=func)
-        return func
-
-    def disconnect(self, func: t.Callable[[WebSocket, int], None]) -> t.Callable:
-        self._handlers_kwargs.update(on_disconnect=func)
-        return func
-
-
-class WebsocketRouteOperation(
-    WebSocketOperationMixin, WebsocketRouteOperationBase, StarletteWebSocketRoute
-):
+class WebsocketRouteOperation(WebsocketRouteOperationBase, StarletteWebSocketRoute):
     websocket_endpoint_args_model: t.Type[
         WebsocketEndpointArgsModel
     ] = WebsocketEndpointArgsModel
 
     __slots__ = (
         "endpoint",
         "_handlers_kwargs",
@@ -88,14 +73,21 @@
             self._handlers_kwargs.update(on_receive=self.endpoint)
         self._load_model()
 
     @classmethod
     def get_websocket_handler(cls) -> t.Type[WebSocketExtraHandler]:
         return WebSocketExtraHandler
 
+    def add_websocket_handler(self, handler_name: str, handler: t.Callable) -> None:
+        if handler_name not in self._handlers_kwargs:
+            raise Exception(
+                f"Invalid Handler Name. Handler Name must be in {list(self._handlers_kwargs.keys())}"
+            )
+        self._handlers_kwargs.update({handler_name: handler})
+
     async def _handle_request(self, context: IExecutionContext) -> None:
         func_kwargs, errors = await self.endpoint_parameter_model.resolve_dependencies(
             ctx=context
         )
         if errors:
             websocket = context.switch_to_websocket().get_client()
             exc = WebSocketRequestValidationError(errors)
```

### Comparing `ellar-0.3.4/ellar/core/schema.py` & `ellar-0.3.6/ellar/core/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/services.py` & `ellar-0.3.6/ellar/core/core_service_registration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+import typing as t
+
 from ellar.di import EllarInjector
 from ellar.services.reflector import Reflector
 
-from .conf import Config
 from .context import (
     ExecutionContextFactory,
     HostContextFactory,
     IExecutionContextFactory,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IWebSocketContextFactory,
 )
 from .context.factory import HTTPConnectionContextFactory, WebSocketContextFactory
 from .exceptions.interfaces import IExceptionMiddlewareService
 from .exceptions.service import ExceptionMiddlewareService
 
+if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core.conf import Config
+
 
 class CoreServiceRegistration:
     """Create Binding for all application service"""
 
     __slots__ = ("injector", "config")
 
-    def __init__(self, injector: EllarInjector, config: Config) -> None:
+    def __init__(self, injector: EllarInjector, config: "Config") -> None:
         self.injector = injector
         self.config = config
 
     def register_all(self) -> None:
         self.injector.container.register(
             IExceptionMiddlewareService, ExceptionMiddlewareService
         )
@@ -38,8 +42,8 @@
             IHTTPConnectionContextFactory, HTTPConnectionContextFactory
         )
 
         self.injector.container.register_scoped(
             IWebSocketContextFactory, WebSocketContextFactory
         )
 
-        self.injector.container.register_instance(Reflector())
+        self.injector.container.register(Reflector)
```

### Comparing `ellar-0.3.4/ellar/core/staticfiles.py` & `ellar-0.3.6/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/templating/__init__.py` & `ellar-0.3.6/ellar/core/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/templating/interface.py` & `ellar-0.3.6/ellar/core/templating/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from jinja2 import Environment as BaseEnvironment, FileSystemLoader
 from starlette.templating import pass_context
 
 from ellar.compatible import cached_property
 from ellar.constants import TEMPLATE_FILTER_KEY, TEMPLATE_GLOBAL_KEY
 from ellar.core.connection import Request
+from ellar.core.datastructures import URL
 from ellar.core.staticfiles import StaticFiles
 from ellar.types import ASGIApp, TemplateFilterCallable, TemplateGlobalCallable
 
-from ..conf import Config
 from .environment import Environment
 from .loader import JinjaLoader
 
 if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.core.conf import Config
     from ellar.core.main import App
     from ellar.di import EllarInjector
 
 
 class TemplateFunctionData(t.NamedTuple):
     func: t.Callable
     name: t.Optional[str]
@@ -127,15 +128,15 @@
             path = os.path.join(str(self.root_path), self._static_folder)
             if os.path.exists(path):
                 return path
         return None
 
 
 class AppTemplating(JinjaTemplating):
-    config: Config
+    config: "Config"
     _static_app: t.Optional[ASGIApp]
     _injector: "EllarInjector"
     has_static_files: bool
 
     @abstractmethod
     def build_middleware_stack(self) -> t.Callable:  # pragma: no cover
         pass
@@ -178,15 +179,15 @@
             t.Dict, self.config.JINJA_TEMPLATES_OPTIONS or {}
         )
 
         for k, v in options_defaults.items():
             jinja_options.setdefault(k, v)
 
         @pass_context
-        def url_for(context: dict, name: str, **path_params: t.Any) -> str:
+        def url_for(context: dict, name: str, **path_params: t.Any) -> URL:
             request = t.cast(Request, context["request"])
             return request.url_for(name, **path_params)
 
         app: App = t.cast("App", self)
 
         jinja_env = Environment(app, **jinja_options)
         jinja_env.globals.update(
```

### Comparing `ellar-0.3.4/ellar/core/templating/loader.py` & `ellar-0.3.6/ellar/core/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/templating/renderer.py` & `ellar-0.3.6/ellar/core/templating/renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/versioning/__init__.py` & `ellar-0.3.6/ellar/core/versioning/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,13 @@
     HeaderAPIVersioning as HeaderAPIVersioning,
     HostNameAPIVersioning as HostNameAPIVersioning,
     QueryParameterAPIVersioning as QueryParameterAPIVersioning,
     UrlPathAPIVersioning as UrlPathAPIVersioning,
 )
 
 
-class VERSIONING(Enum):
+class VersioningSchemes(Enum):
     URL = UrlPathAPIVersioning
     QUERY = QueryParameterAPIVersioning
     HEADER = HeaderAPIVersioning
     HOST = HostNameAPIVersioning
     NONE = DefaultAPIVersioning
```

### Comparing `ellar-0.3.4/ellar/core/versioning/base.py` & `ellar-0.3.6/ellar/core/versioning/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/core/versioning/resolver.py` & `ellar-0.3.6/ellar/core/versioning/resolver.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/__init__.py` & `ellar-0.3.6/ellar/di/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/injector/container.py` & `ellar-0.3.6/ellar/di/injector/container.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/injector/ellar_injector.py` & `ellar-0.3.6/ellar/di/injector/ellar_injector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/providers.py` & `ellar-0.3.6/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/scopes.py` & `ellar-0.3.6/ellar/di/scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/di/service_config.py` & `ellar-0.3.6/ellar/di/service_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/helper/__init__.py` & `ellar-0.3.6/ellar/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/helper/enums.py` & `ellar-0.3.6/ellar/helper/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/helper/importer.py` & `ellar-0.3.6/ellar/helper/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/helper/modelfield.py` & `ellar-0.3.6/ellar/helper/modelfield.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/helper/module_loading.py` & `ellar-0.3.6/ellar/helper/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/__init__.py` & `ellar-0.3.6/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/builder.py` & `ellar-0.3.6/ellar/openapi/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/docs_generators/base.py` & `ellar-0.3.6/ellar/openapi/docs_generators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/docs_generators/redocs.py` & `ellar-0.3.6/ellar/openapi/docs_generators/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/docs_generators/swagger.py` & `ellar-0.3.6/ellar/openapi/docs_generators/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/module.py` & `ellar-0.3.6/ellar/openapi/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/openapi_v3.py` & `ellar-0.3.6/ellar/openapi/openapi_v3.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/route_doc_models.py` & `ellar-0.3.6/ellar/openapi/route_doc_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/templates/redocs.html` & `ellar-0.3.6/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/openapi/templates/swagger.html` & `ellar-0.3.6/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/reflect.py` & `ellar-0.3.6/ellar/reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.3.6/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.3.6/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.3.6/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/samples/static/img/Icon.svg` & `ellar-0.3.6/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/samples/templates/home/index.html` & `ellar-0.3.6/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/serializer.py` & `ellar-0.3.6/ellar/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/ellar/services/reflector.py` & `ellar-0.3.6/ellar/services/reflector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 import typing as t
 
+from ellar.di import injectable
 from ellar.reflect import reflect
 
 
+@injectable()
 class Reflector:
     __slots__ = ()
 
     def get(self, metadata_key: str, target: t.Union[t.Type, t.Callable]) -> t.Any:
         return reflect.get_metadata(metadata_key, target)
 
     def get_all(
```

### Comparing `ellar-0.3.4/ellar/types.py` & `ellar-0.3.6/ellar/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/examples/catapp/application/cats/statics/blog/blog.css` & `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/examples/catapp/application/cats/statics/blog/blog.rtl.css` & `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/examples/catapp/application/cats/statics/brand/bootstrap-logo-white.svg` & `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/examples/catapp/application/cats/statics/brand/bootstrap-logo.svg` & `ellar-0.3.6/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/examples/catapp/application/cats/views/index.html` & `ellar-0.3.6/examples/01-carapp/carapp/apps/car/views/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/mkdocs.yml` & `ellar-0.3.6/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       - Providers:  overview/providers.md
       - Modules:  overview/modules.md
       - Middlewares:  overview/middleware.md
       - Exception Handling:  overview/exception_handling.md
       - Guards:  overview/guards.md
       - Custom Decorators:  overview/custom_decorators.md
       - Module Router:  overview/module-router.md
+  - Execution Context: basics/execution-context.md
   - Configuration: configurations.md
   - How-to Guides:
       - Input Parsing: parsing-inputs/index.md
       - Path: parsing-inputs/path-params.md
       - Query: parsing-inputs/query-params.md
       - Header: parsing-inputs/header-params.md
       - Cookie: parsing-inputs/cookie-params.md
@@ -84,28 +85,26 @@
   - Templating:
     - html: templating/templating.md
     - Static Files: templating/staticfiles.md
 
   - Caching: caching.md
   - Rate Limiting: throttling.md
 #  - Injection Scopes: basics/injection-scope.md
-#  - Model View Controller: basics/model-view-controller.md
 #  - Events: basics/events.md
   - Commands:
     - Introduction: commands/index.md
-    - Commands:
+    - CLI Commands:
         - new: commands/new-command.md
         - create project: commands/create-project-command.md
         - create module: commands/create-module-command.md
         - runserver: commands/runserver-command.md
     - Custom Commands: commands/custom-commands.md
     - Command Grouping: commands/command-grouping.md
   - Versioning: basics/versioning.md
   - Testing: basics/testing.md
-  - OpenAPI: openapi/index.md
   - WebSockets: websockets.md
   - Mount: mount.md
   - Background Tasks: background-task.md
   - Release Notes: release-notes.md
 
 markdown_extensions:
   - attr_list
```

#### html2text {}

```diff
@@ -15,29 +15,29 @@
 separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-z])' -
 minify: minify_html: true - git-revision-date-localized: enable_creation_date:
 false nav: - Introduction: index.md - Overview: - Step One: overview/index.md -
 Controllers: overview/controllers.md - Providers: overview/providers.md -
 Modules: overview/modules.md - Middlewares: overview/middleware.md - Exception
 Handling: overview/exception_handling.md - Guards: overview/guards.md - Custom
 Decorators: overview/custom_decorators.md - Module Router: overview/module-
-router.md - Configuration: configurations.md - How-to Guides: - Input Parsing:
-parsing-inputs/index.md - Path: parsing-inputs/path-params.md - Query: parsing-
-inputs/query-params.md - Header: parsing-inputs/header-params.md - Cookie:
-parsing-inputs/cookie-params.md - Body: parsing-inputs/body.md - Form: parsing-
-inputs/form-params.md - File: parsing-inputs/file-params.md - Handling
-Response: - Response Schema: handling-response/response.md - Response Model:
-handling-response/response-model.md - Templating: - html: templating/
-templating.md - Static Files: templating/staticfiles.md - Caching: caching.md -
-Rate Limiting: throttling.md # - Injection Scopes: basics/injection-scope.md #
-- Model View Controller: basics/model-view-controller.md # - Events: basics/
-events.md - Commands: - Introduction: commands/index.md - Commands: - new:
-commands/new-command.md - create project: commands/create-project-command.md -
-create module: commands/create-module-command.md - runserver: commands/
-runserver-command.md - Custom Commands: commands/custom-commands.md - Command
-Grouping: commands/command-grouping.md - Versioning: basics/versioning.md -
-Testing: basics/testing.md - OpenAPI: openapi/index.md - WebSockets:
-websockets.md - Mount: mount.md - Background Tasks: background-task.md -
-Release Notes: release-notes.md markdown_extensions: - attr_list - toc:
-permalink: true - admonition - def_list - tables - abbr - footnotes -
-md_in_html - codehilite - pymdownx.superfences: custom_fences: - name: mermaid
-class: mermaid - pymdownx.details - pymdownx.tabbed: alternate_style: true -
-pymdownx.saneheaders extra_css: - stylesheets/extra.css
+router.md - Execution Context: basics/execution-context.md - Configuration:
+configurations.md - How-to Guides: - Input Parsing: parsing-inputs/index.md -
+Path: parsing-inputs/path-params.md - Query: parsing-inputs/query-params.md -
+Header: parsing-inputs/header-params.md - Cookie: parsing-inputs/cookie-
+params.md - Body: parsing-inputs/body.md - Form: parsing-inputs/form-params.md
+- File: parsing-inputs/file-params.md - Handling Response: - Response Schema:
+handling-response/response.md - Response Model: handling-response/response-
+model.md - Templating: - html: templating/templating.md - Static Files:
+templating/staticfiles.md - Caching: caching.md - Rate Limiting: throttling.md
+# - Injection Scopes: basics/injection-scope.md # - Events: basics/events.md -
+Commands: - Introduction: commands/index.md - CLI Commands: - new: commands/
+new-command.md - create project: commands/create-project-command.md - create
+module: commands/create-module-command.md - runserver: commands/runserver-
+command.md - Custom Commands: commands/custom-commands.md - Command Grouping:
+commands/command-grouping.md - Versioning: basics/versioning.md - Testing:
+basics/testing.md - WebSockets: websockets.md - Mount: mount.md - Background
+Tasks: background-task.md - Release Notes: release-notes.md
+markdown_extensions: - attr_list - toc: permalink: true - admonition - def_list
+- tables - abbr - footnotes - md_in_html - codehilite - pymdownx.superfences:
+custom_fences: - name: mermaid class: mermaid - pymdownx.details -
+pymdownx.tabbed: alternate_style: true - pymdownx.saneheaders extra_css: -
+stylesheets/extra.css
```

### Comparing `ellar-0.3.4/mypy.ini` & `ellar-0.3.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/pyproject.toml` & `ellar-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     "injector == 0.20.1",
-    "starlette == 0.23.1",
+    "starlette == 0.26.1",
     "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
     "jinja2",
     # cli
     "typer >=0.6.1,<0.8.0",
     # testing
     "httpx >= 0.22.0"
 ]
@@ -74,24 +74,24 @@
     "email_validator >=1.1.1",
     "pylibmc",
     "pymemcache",
     "aiomcache",
     "redis",
 
     # types
-    "types-ujson ==5.7.0.0",
+    "types-ujson ==5.7.0.1",
     "types-orjson ==3.6.2",
     "types-dataclasses ==0.6.6",
 ]
 dev = [
     "pre-commit"
 ]
 
 all = [
-    "python-multipart >=0.0.5,<0.0.6",
+    "python-multipart >=0.0.5,<0.0.7",
     "itsdangerous >=1.1.0,<3.0.0",
     "pyyaml >=5.3.1,<7.0.0",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,<6.0.0",
     "orjson >=3.2.1,<4.0.0",
     "email_validator >=1.1.1,<2.0.0",
 ]
 doc = [
```

### Comparing `ellar-0.3.4/tests/conftest.py` & `ellar-0.3.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/injector_module.py` & `ellar-0.3.6/tests/injector_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/main.py` & `ellar-0.3.6/tests/main.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/schema.py` & `ellar-0.3.6/tests/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_application/sample.py` & `ellar-0.3.6/tests/test_application/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_application/test_application_factory.py` & `ellar-0.3.6/tests/test_application/test_application_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from starlette.routing import Host, Mount
 
 from ellar.common import Module
-from ellar.core import AppFactory, Config, ModuleBase, ModuleSetup, TestClient
+from ellar.core import AppFactory, Config, ModuleBase, ModuleSetup
 from ellar.di import EllarInjector
+from ellar.testing import TestClient
 
 from .sample import (
     AppAPIKey,
     ApplicationModule,
     ClassBaseController,
     create_tmp_template_and_static_dir,
     router,
```

### Comparing `ellar-0.3.4/tests/test_application/test_application_functions.py` & `ellar-0.3.6/tests/test_application/test_application_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,147 +1,118 @@
 import os
 import typing as t
 
 from starlette.responses import JSONResponse, PlainTextResponse, Response
 
 from ellar.common import Module, get, template_filter, template_global
 from ellar.compatible import asynccontextmanager
-from ellar.core import (
-    App,
-    AppFactory,
-    Config,
-    ModuleBase,
-    TestClient,
-    TestClientFactory,
-)
+from ellar.core import App, AppFactory, Config, ModuleBase
 from ellar.core.connection import Request
 from ellar.core.context import IExecutionContext
-from ellar.core.events import EventHandler
+from ellar.core.core_service_registration import CoreServiceRegistration
 from ellar.core.exceptions.interfaces import IExceptionHandler
 from ellar.core.modules import ModuleTemplateRef
-from ellar.core.services import CoreServiceRegistration
 from ellar.core.staticfiles import StaticFiles
 from ellar.core.templating import Environment
-from ellar.core.versioning import VERSIONING, DefaultAPIVersioning, UrlPathAPIVersioning
+from ellar.core.versioning import (
+    DefaultAPIVersioning,
+    UrlPathAPIVersioning,
+    VersioningSchemes as VERSIONING,
+)
 from ellar.di import EllarInjector
 from ellar.helper.importer import get_class_import
 from ellar.openapi import OpenAPIDocumentModule
 from ellar.services.reflector import Reflector
+from ellar.testing import Test, TestClient
 
 from .config import ConfigTrustHostConfigure
 from .sample import AppAPIKey, ApplicationModule
 
-test_module = TestClientFactory.create_test_module_from_module(
-    module=ApplicationModule, config_module=get_class_import(ConfigTrustHostConfigure)
+test_module = Test.create_test_module(
+    modules=(ApplicationModule,),
+    config_module=get_class_import(ConfigTrustHostConfigure),
 )
 
 
 class TestStarletteCompatibility:
     def test_func_route(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/func")
         assert response.status_code == 200
         assert response.text == "Hello, world!"
 
         response = client.head("/func")
         assert response.status_code == 200
         assert response.text == ""
 
     def test_async_route(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/async")
         assert response.status_code == 200
         assert response.text == "Hello, world!"
 
     def test_class_route(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/classbase/class")
         assert response.status_code == 200
         assert response.text == "Hello, world!"
 
     def test_mounted_route(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/users/")
         assert response.status_code == 200
         assert response.text == "Hello, everyone!"
 
     def test_mounted_route_path_params(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/users/tomchristie")
         assert response.status_code == 200
         assert response.text == "Hello, tomchristie!"
 
     def test_subdomain_route(self):
-        client = test_module.get_client(base_url="https://foo.example.org/")
+        client = test_module.get_test_client(base_url="https://foo.example.org/")
 
         response = client.get("/")
         assert response.status_code == 200
         assert response.text == "Subdomain: foo"
 
     def test_websocket_route(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         with client.websocket_connect("/ws") as session:
             text = session.receive_text()
             assert text == "Hello, world!"
 
     def test_400(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.get("/404")
         assert response.status_code == 404
         assert response.json() == {"detail": "Not Found"}
 
     def test_405(self):
-        client = test_module.get_client()
+        client = test_module.get_test_client()
         response = client.post("/func")
         assert response.status_code == 405
         assert response.json() == {"detail": "Custom message"}
 
         response = client.post("/classbase/class")
         assert response.status_code == 405
         assert response.json() == {"detail": "Custom message"}
 
     def test_500(self):
-        client = test_module.get_client(raise_server_exceptions=False)
+        client = test_module.get_test_client(raise_server_exceptions=False)
         response = client.get("/classbase/500")
         assert response.status_code == 500
         assert response.json() == {"detail": "Server Error"}
 
     def test_middleware(self):
-        client = test_module.get_client(base_url="http://incorrecthost")
+        client = test_module.get_test_client(base_url="http://incorrecthost")
         response = client.get("/func")
         assert response.status_code == 400
         assert response.text == "Invalid host header"
 
-    def test_app_add_event_handler(self, test_client_factory):
-        startup_complete = False
-        cleanup_complete = False
-
-        def run_startup():
-            nonlocal startup_complete
-            startup_complete = True
-
-        def run_cleanup():
-            nonlocal cleanup_complete
-            cleanup_complete = True
-
-        app = App(
-            config=Config(),
-            injector=EllarInjector(),
-            on_startup_event_handlers=[EventHandler(run_startup)],
-            on_shutdown_event_handlers=[EventHandler(run_cleanup)],
-        )
-
-        assert not startup_complete
-        assert not cleanup_complete
-        with test_client_factory(app):
-            assert startup_complete
-            assert not cleanup_complete
-        assert startup_complete
-        assert cleanup_complete
-
     def test_app_async_cm_lifespan(self, test_client_factory):
         startup_complete = False
         cleanup_complete = False
 
         @asynccontextmanager
         async def lifespan(app):
             nonlocal startup_complete, cleanup_complete
@@ -201,14 +172,25 @@
         app = AppFactory.create_app()
         app.router.append(homepage)
         client = TestClient(app)
         response = client.get("/")
         assert response.status_code == 200
         assert response.text == "Ellar Route Handler as an ASGI app"
 
+    def test_ellar_app_url_for(self):
+        @get("/homepage-url", name="homepage")
+        async def homepage(request: Request, ctx: IExecutionContext):
+            res = PlainTextResponse("Ellar Route Handler as an ASGI app")
+            return res
+
+        app = AppFactory.create_app()
+        app.router.append(homepage)
+        result = app.url_path_for("homepage")
+        assert result == "/homepage-url"
+
     def test_app_staticfiles_route(self, tmpdir):
         path = os.path.join(tmpdir, "example.txt")
         with open(path, "w") as file:
             file.write("<file content>")
 
         config = Config(STATIC_DIRECTORIES=[tmpdir])
         injector = EllarInjector()
```

### Comparing `ellar-0.3.4/tests/test_application/test_cors.py` & `ellar-0.3.6/tests/test_application/test_cors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 
 from ellar.common import http_route
-from ellar.core import TestClientFactory
+from ellar.testing import Test
 
 
 def test_cors_allow_all():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_EXPOSE_HEADERS = ["X-Status"]
-    tm.app.config.CORS_ALLOW_HEADERS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["*"]
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.config.CORS_ALLOW_CREDENTIALS = True
-
-    tm.app.rebuild_middleware_stack()
-    client = tm.get_client()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_EXPOSE_HEADERS=["X-Status"],
+            CORS_ALLOW_HEADERS=["*"],
+            CORS_ALLOW_METHODS=["*"],
+            CORS_ALLOW_ORIGINS=["*"],
+            CORS_ALLOW_CREDENTIALS=True,
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     # Test pre-flight response
     headers = {
         "Origin": "https://example.org",
         "Access-Control-Request-Method": "GET",
         "Access-Control-Request-Headers": "X-Example",
     }
@@ -60,25 +61,26 @@
     assert "access-control-allow-origin" not in response.headers
 
 
 def test_cors_allow_all_except_credentials():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_EXPOSE_HEADERS = ["X-Status"]
-    tm.app.config.CORS_ALLOW_HEADERS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["*"]
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_EXPOSE_HEADERS=["X-Status"],
+            CORS_ALLOW_HEADERS=["*"],
+            CORS_ALLOW_METHODS=["*"],
+            CORS_ALLOW_ORIGINS=["*"],
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     # Test pre-flight response
     headers = {
         "Origin": "https://example.org",
         "Access-Control-Request-Method": "GET",
         "Access-Control-Request-Headers": "X-Example",
     }
@@ -106,23 +108,25 @@
     assert "access-control-allow-origin" not in response.headers
 
 
 def test_cors_allow_specific_origin():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_HEADERS = ["X-Example", "Content-Type"]
-    tm.app.config.CORS_ALLOW_ORIGINS = ["https://example.org"]
-    tm.app.config.CORS_ALLOW_CREDENTIALS = False
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_HEADERS=["X-Example", "Content-Type"],
+            CORS_ALLOW_ORIGINS=["https://example.org"],
+            CORS_ALLOW_CREDENTIALS=False,
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     # Test pre-flight response
     headers = {
         "Origin": "https://example.org",
         "Access-Control-Request-Method": "GET",
         "Access-Control-Request-Headers": "X-Example, Content-Type",
     }
@@ -150,22 +154,23 @@
     assert "access-control-allow-origin" not in response.headers
 
 
 def test_cors_disallowed_preflight():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-
-    tm.app.config.CORS_ALLOW_HEADERS = ["X-Example"]
-    tm.app.config.CORS_ALLOW_ORIGINS = ["https://example.org"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_HEADERS=["X-Example"], CORS_ALLOW_ORIGINS=["https://example.org"]
+        )
+    )
+    app = tm.create_application()
 
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-    client = tm.get_client()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     # Test pre-flight response
     headers = {
         "Origin": "https://another.org",
         "Access-Control-Request-Method": "POST",
         "Access-Control-Request-Headers": "X-Nope",
     }
@@ -185,23 +190,25 @@
     assert response.text == "Disallowed CORS headers"
 
 
 def test_preflight_allows_request_origin_if_origins_wildcard_and_credentials_allowed():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["POST"]
-    tm.app.config.CORS_ALLOW_CREDENTIALS = True
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_ORIGINS=["*"],
+            CORS_ALLOW_METHODS=["POST"],
+            CORS_ALLOW_CREDENTIALS=True,
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     # Test pre-flight response
     headers = {
         "Origin": "https://example.org",
         "Access-Control-Request-Method": "POST",
     }
 
@@ -215,22 +222,21 @@
     assert response.headers["vary"] == "Origin"
 
 
 def test_cors_preflight_allow_all_methods():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["*"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(CORS_ALLOW_ORIGINS=["*"], CORS_ALLOW_METHODS=["*"])
+    )
+    app = tm.create_application()
 
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-    client = tm.get_client()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     headers = {
         "Origin": "https://example.org",
         "Access-Control-Request-Method": "POST",
     }
 
     for method in ("DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"):
@@ -240,21 +246,20 @@
 
 
 def test_cors_allow_all_methods():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
     methods = ["delete", "get", "head", "options", "patch", "post", "put"]
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=methods)(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["*"]
-    tm.app.rebuild_middleware_stack()
-    client = tm.get_client()
+    tm = Test.create_test_module(
+        config_module=dict(CORS_ALLOW_ORIGINS=["*"], CORS_ALLOW_METHODS=["*"])
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=methods)(homepage))
+    client = tm.get_test_client()
 
     headers = {"Origin": "https://example.org"}
 
     for method in ("patch", "post", "put"):
         response = getattr(client, method)("/", headers=headers, json={})
         assert response.status_code == 200
     for method in ("delete", "get", "head", "options"):
@@ -262,23 +267,25 @@
         assert response.status_code == 200
 
 
 def test_cors_allow_origin_regex():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGIN_REGEX = "https://.*"
-    tm.app.config.CORS_ALLOW_HEADERS = ["X-Example", "Content-Type"]
-    tm.app.config.CORS_ALLOW_CREDENTIALS = True
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_ORIGIN_REGEX="https://.*",
+            CORS_ALLOW_HEADERS=["X-Example", "Content-Type"],
+            CORS_ALLOW_CREDENTIALS=True,
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     # Test standard response
     headers = {"Origin": "https://example.org"}
     response = client.get("/", headers=headers)
     assert response.status_code == 200
     assert response.text == "Homepage"
     assert response.headers["access-control-allow-origin"] == "https://example.org"
@@ -328,22 +335,24 @@
     assert "access-control-allow-origin" not in response.headers
 
 
 def test_cors_allow_origin_regex_fullmatch():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGIN_REGEX = r"https://.*\.example.org"
-    tm.app.config.CORS_ALLOW_HEADERS = ["X-Example", "Content-Type"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_ORIGIN_REGEX=r"https://.*\.example.org",
+            CORS_ALLOW_HEADERS=["X-Example", "Content-Type"],
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     # Test standard response
     headers = {"Origin": "https://subdomain.example.org"}
     response = client.get("/", headers=headers)
     assert response.status_code == 200
     assert response.text == "Homepage"
     assert (
@@ -360,119 +369,113 @@
     assert "access-control-allow-origin" not in response.headers
 
 
 def test_cors_credentialed_requests_return_specific_origin():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.rebuild_middleware_stack()
-    client = tm.get_client()
+    tm = Test.create_test_module(config_module=dict(CORS_ALLOW_ORIGINS=["*"]))
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     # Test credentialed request
     headers = {"Origin": "https://example.org", "Cookie": "star_cookie=sugar"}
     response = client.get("/", headers=headers)
     assert response.status_code == 200
     assert response.text == "Homepage"
     assert response.headers["access-control-allow-origin"] == "https://example.org"
     assert "access-control-allow-credentials" not in response.headers
 
 
 def test_cors_vary_header_defaults_to_origin():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["https://example.org"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(CORS_ALLOW_ORIGINS=["https://example.org"])
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     headers = {"Origin": "https://example.org"}
 
     response = client.get("/", headers=headers)
     assert response.status_code == 200
     assert response.headers["vary"] == "Origin"
 
 
 def test_cors_vary_header_is_not_set_for_non_credentialed_request():
     def homepage(request: Request):
         return PlainTextResponse(
             "Homepage", status_code=200, headers={"Vary": "Accept-Encoding"}
         )
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(config_module=dict(CORS_ALLOW_ORIGINS=["*"]))
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     response = client.get("/", headers={"Origin": "https://someplace.org"})
     assert response.status_code == 200
     assert response.headers["vary"] == "Accept-Encoding"
 
 
 def test_cors_vary_header_is_properly_set_for_credentialed_request():
     def homepage(request: Request):
         return PlainTextResponse(
             "Homepage", status_code=200, headers={"Vary": "Accept-Encoding"}
         )
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.rebuild_middleware_stack()
-    client = tm.get_client()
+    tm = Test.create_test_module(config_module=dict(CORS_ALLOW_ORIGINS=["*"]))
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     response = client.get(
         "/", headers={"Cookie": "foo=bar", "Origin": "https://someplace.org"}
     )
     assert response.status_code == 200
     assert response.headers["vary"] == "Accept-Encoding, Origin"
 
 
 def test_cors_vary_header_is_properly_set_when_allow_origins_is_not_wildcard():
     def homepage(request: Request):
         return PlainTextResponse(
             "Homepage", status_code=200, headers={"Vary": "Accept-Encoding"}
         )
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-
-    tm.app.config.CORS_ALLOW_ORIGINS = ["https://example.org"]
-    tm.app.rebuild_middleware_stack()
+    tm = Test.create_test_module(
+        config_module=dict(CORS_ALLOW_ORIGINS=["https://example.org"])
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     response = client.get("/", headers={"Origin": "https://example.org"})
     assert response.status_code == 200
     assert response.headers["vary"] == "Accept-Encoding, Origin"
 
 
 def test_cors_allowed_origin_does_not_leak_between_credentialed_requests():
     def homepage(request: Request):
         return PlainTextResponse("Homepage", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.config.CORS_ALLOW_ORIGINS = ["*"]
-    tm.app.config.CORS_ALLOW_HEADERS = ["*"]
-    tm.app.config.CORS_ALLOW_METHODS = ["*"]
-    tm.app.rebuild_middleware_stack()
-
-    tm.app.router.append(http_route(methods=["GET"])(homepage))
-    client = tm.get_client()
+    tm = Test.create_test_module(
+        config_module=dict(
+            CORS_ALLOW_ORIGINS=["*"], CORS_ALLOW_HEADERS=["*"], CORS_ALLOW_METHODS=["*"]
+        )
+    )
+    app = tm.create_application()
+    app.router.append(http_route(methods=["GET"])(homepage))
+    client = tm.get_test_client()
 
     response = client.get("/", headers={"Origin": "https://someplace.org"})
     assert response.headers["access-control-allow-origin"] == "*"
     assert "access-control-allow-credentials" not in response.headers
 
     response = client.get(
         "/", headers={"Cookie": "foo=bar", "Origin": "https://someplace.org"}
```

### Comparing `ellar-0.3.4/tests/test_application/test_replacing_app_services.py` & `ellar-0.3.6/tests/test_application/test_replacing_app_services.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from starlette.exceptions import HTTPException
 from starlette.responses import PlainTextResponse
 
 from ellar.common import Controller, Module, exception_handler, get
-from ellar.core import TestClientFactory
 from ellar.core.context import (
     ExecutionContext,
     HostContext,
     IExecutionContext,
     IExecutionContextFactory,
     IHostContext,
     IHostContextFactory,
 )
 from ellar.core.exceptions import IExceptionMiddlewareService
 from ellar.core.exceptions.service import ExceptionMiddlewareService
 from ellar.di import ProviderConfig, injectable
 from ellar.services import Reflector
+from ellar.testing import Test
 
 
 @Controller
 class ExampleController:
     @get()
     def index(self):
         return self.context.__class__.__name__
@@ -75,19 +75,20 @@
 class NewExceptionMiddlewareService(ExceptionMiddlewareService):
     def lookup_status_code_exception_handler(self, status_code: int):
         self.__class__.worked = True
         return self._status_handlers.get(status_code)
 
 
 def test_can_replace_host_context():
-    tm = TestClientFactory.create_test_module(controllers=[ExampleController])
-    tm.app.injector.container.register(IHostContextFactory, NewHostContextFactory)
+    tm = Test.create_test_module(controllers=[ExampleController]).override_provider(
+        IHostContextFactory, use_class=NewHostContextFactory
+    )
 
     assert hasattr(NewHostContext, "worked") is False
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/example/exception")
     assert res.json() == {"detail": "Bad Request", "status_code": 400}
 
     assert hasattr(NewHostContext, "worked") is True
     assert NewHostContext.worked is True
 
 
@@ -103,33 +104,32 @@
     class ExampleModule:
         @exception_handler(400)
         def exception_400(self, context: IHostContext, exc: Exception):
             return PlainTextResponse(
                 "Exception 400 handled by ExampleModule.exception_400"
             )
 
-    tm = TestClientFactory.create_test_module_from_module(ExampleModule)
+    tm = Test.create_test_module(modules=[ExampleModule])
 
     assert hasattr(NewExceptionMiddlewareService, "worked") is False
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/example/exception")
     assert res.status_code == 200
     assert res.text == "Exception 400 handled by ExampleModule.exception_400"
 
     assert hasattr(NewExceptionMiddlewareService, "worked") is True
     assert NewExceptionMiddlewareService.worked is True
 
 
 def test_can_replace_execution_context():
-    tm = TestClientFactory.create_test_module(controllers=[ExampleController])
-    tm.app.injector.container.register(
-        IExecutionContextFactory, NewExecutionHostFactory
+    tm = Test.create_test_module(controllers=[ExampleController]).override_provider(
+        IExecutionContextFactory, use_class=NewExecutionHostFactory
     )
 
     assert hasattr(NewExecutionContext, "worked") is False
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/example/")
     assert res.status_code == 200
     assert res.text == '"NewExecutionContext"'
 
     assert hasattr(NewExecutionContext, "worked") is True
     assert NewExecutionContext.worked is True
```

### Comparing `ellar-0.3.4/tests/test_application/test_testclient_factory.py` & `ellar-0.3.6/tests/test_testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import abstractmethod
 
 from starlette.routing import Host, Mount
 
 from ellar.constants import MODULE_METADATA
-from ellar.core import TestClientFactory
 from ellar.di import ProviderConfig
 from ellar.reflect import reflect
+from ellar.testing import Test
 
-from .sample import (
+from .test_application.sample import (
     ApplicationModule,
     ClassBaseController,
     create_tmp_template_and_static_dir,
     router,
     sub_domain,
     users,
 )
@@ -41,60 +41,55 @@
 
     def get_full_name(self):
         return "some full name"
 
 
 def test_test_client_factory_create_test_module(tmpdir):
     create_tmp_template_and_static_dir(tmpdir)
-    tm = TestClientFactory.create_test_module(
+    tm = Test.create_test_module(
         controllers=(ClassBaseController,),
         routers=[
             Host("{subdomain}.example.org", app=sub_domain),
             Mount("/users", app=users),
             router,
         ],
         template_folder="templates",
         static_folder="statics",
         base_directory=tmpdir,
     )
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/static/example.txt")
     assert res.status_code == 200
     assert res.text == "<file content>"
 
-    template = tm.app.jinja_environment.get_template("example.html")
+    template = tm.create_application().jinja_environment.get_template("example.html")
     result = template.render()
     assert result == "<html>Hello World<html/>"
 
-    client = tm.get_client(base_url="https://foo.example.org/")
+    client = tm.get_test_client(base_url="https://foo.example.org/")
 
     response = client.get("/")
     assert response.status_code == 200
     assert response.text == "Subdomain: foo"
 
 
 def test_client_factory_create_test_module_from_module():
     reflect.metadata(
         metadata_key=MODULE_METADATA.PROVIDERS,
         metadata_value=[ProviderConfig(base_type=IFoo, use_class=Foo)],
     )(
         ApplicationModule
     )  # dynamically add IFoo to ApplicationModule Providers
 
-    tm = TestClientFactory.create_test_module_from_module(
-        module=ApplicationModule,
-        mock_providers=(
-            ProviderConfig(
-                base_type=IFoo, use_value=MockFoo()
-            ),  # force provider override
-        ),
-    )
+    tm = Test.create_test_module(
+        modules=[ApplicationModule],
+    ).override_provider(IFoo, use_value=MockFoo())
 
-    client = tm.get_client(base_url="https://foo.example.org/")
+    client = tm.get_test_client(base_url="https://foo.example.org/")
 
     response = client.get("/")
     assert response.status_code == 200
     assert response.text == "Subdomain: foo"
 
-    ifoo: IFoo = tm.app.injector.get(IFoo)
+    ifoo: IFoo = tm.get(IFoo)
     assert isinstance(ifoo, MockFoo)
```

### Comparing `ellar-0.3.4/tests/test_application/test_trusted_host.py` & `ellar-0.3.6/tests/test_application/test_trusted_host.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 
 from ellar.common import get
-from ellar.core import TestClientFactory
+from ellar.testing import Test
 
 
 def test_trusted_host_middleware(test_client_factory):
     @get()
     def homepage(request: Request):
         return PlainTextResponse("OK", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.config.ALLOWED_HOSTS = ["testserver", "*.testserver"]
+    tm = Test.create_test_module(
+        config_module=dict(ALLOWED_HOSTS=["testserver", "*.testserver"])
+    )
+    app = tm.create_application()
+    app.router.append(homepage)
 
-    tm.app.rebuild_middleware_stack()
-    assert tm.app.debug is False
+    assert app.debug is False
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     response = client.get("/")
     assert response.status_code == 200
 
-    client = tm.get_client(base_url="http://subdomain.testserver")
+    client = tm.get_test_client(base_url="http://subdomain.testserver")
     response = client.get("/")
     assert response.status_code == 200
 
-    client = tm.get_client(base_url="http://invalidhost")
+    client = tm.get_test_client(base_url="http://invalidhost")
     response = client.get("/")
     assert response.status_code == 400
 
 
 def test_trusted_host_middleware_works_for_debug_true(test_client_factory):
     @get()
     def homepage(request: Request):
         return PlainTextResponse("OK", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
+    tm = Test.create_test_module(
+        config_module=dict(ALLOWED_HOSTS=["testserver", "*.testserver"])
+    )
+    app = tm.create_application()
+    app.router.append(homepage)
 
-    tm.app.config.ALLOWED_HOSTS = ["testserver", "*.testserver"]
-    assert tm.app.debug is False
-    tm.app.debug = True
+    assert app.debug is False
+    app.debug = True
 
-    client = tm.get_client()
+    client = tm.get_test_client()
 
     response = client.get("/")
     assert response.status_code == 200
 
-    client = tm.get_client(base_url="http://subdomain.testserver")
+    client = tm.get_test_client(base_url="http://subdomain.testserver")
     response = client.get("/")
     assert response.status_code == 200
 
-    client = tm.get_client(base_url="http://invalidhost")
+    client = tm.get_test_client(base_url="http://invalidhost")
     response = client.get("/")
     assert response.status_code == 200
 
 
 def test_default_allowed_hosts():
-    tm = TestClientFactory.create_test_module()
-    assert tm.app.config.ALLOWED_HOSTS == ["*"]
+    tm = Test.create_test_module()
+    assert tm.create_application().config.ALLOWED_HOSTS == ["*"]
 
 
 def test_www_redirect(test_client_factory):
     @get()
     def homepage(request: Request):
         return PlainTextResponse("OK", status_code=200)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
+    tm = Test.create_test_module(config_module=dict(ALLOWED_HOSTS=["www.example.com"]))
+    app = tm.create_application()
+    app.router.append(homepage)
 
-    tm.app.config.ALLOWED_HOSTS = ["www.example.com"]
-
-    tm.app.rebuild_middleware_stack()
-
-    client = tm.get_client(base_url="https://example.com")
+    client = tm.get_test_client(base_url="https://example.com")
     response = client.get("/")
     assert response.status_code == 200
     assert response.url == "https://www.example.com/"
```

### Comparing `ellar-0.3.4/tests/test_attribute_dict.py` & `ellar-0.3.6/tests/test_attribute_dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_cache/_test_aio_memcache.py.ellar` & `ellar-0.3.6/tests/test_cache/_test_aio_memcache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_cache/pylib_mock.py` & `ellar-0.3.6/tests/test_cache/pylib_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_cache/redis_mock.py` & `ellar-0.3.6/tests/test_cache/redis_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_cache/test_cache_many_config.py` & `ellar-0.3.6/tests/test_cache/test_cache_many_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ellar.cache import CacheModule, ICacheService, cache
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
 from ellar.common import Controller, get
-from ellar.core import TestClientFactory
 from ellar.core.response import PlainTextResponse
+from ellar.testing import Test
 
 
 @Controller("")
 class ExampleController:
     @get("/index-1")
     @cache(ttl=1, backend="another")
     def index_1(self):
@@ -14,35 +14,35 @@
 
     @get("/index-2")
     @cache(ttl=1, backend="default")
     def index_2(self):
         return dict(message="ExampleController cache 2")
 
 
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     controllers=[ExampleController],
     modules=(CacheModule.register_setup(),),
     config_module=dict(
         CACHES={
             "default": LocalMemCacheBackend(),
             "another": LocalMemCacheBackend(key_prefix="another", version=2),
         }
     ),
 )
 
 
 def test_cache_backend_has_many_cache_backend():
-    cache_service = tm.app.injector.get(ICacheService)
+    cache_service = tm.get(ICacheService)
     assert isinstance(cache_service.get_backend("another"), LocalMemCacheBackend)
     assert isinstance(cache_service.get_backend("default"), LocalMemCacheBackend)
 
 
 def test_cache_operation_with_backend_works():
-    cache_service = tm.app.injector.get(ICacheService)
-    client = tm.get_client(base_url="http://testserver")
+    cache_service = tm.get(ICacheService)
+    client = tm.get_test_client(base_url="http://testserver")
 
     response = client.get("/index-1")
     assert response.text == "ExampleController cache 1"
     result = cache_service.get("http://testserver/index-1:another", backend="another")
     assert result.body == b"ExampleController cache 1"
 
     response = client.get("/index-2")
```

### Comparing `ellar-0.3.4/tests/test_cache/test_cache_service.py` & `ellar-0.3.6/tests/test_cache/test_cache_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
 from ellar.cache.service import CacheService, InvalidCacheBackendKeyException
 
 
 class TestCacheService:
-    def setup(self):
+    def setup_method(self):
         self.cache_service = CacheService(dict(default=LocalMemCacheBackend()))
 
     def test_set(self):
         assert self.cache_service.set("test", "1", 0.1)
         value = self.cache_service.get("test")
         assert value == "1"
 
@@ -57,15 +57,15 @@
         assert isinstance(backend, LocalMemCacheBackend) and backend == backend_default
 
         with pytest.raises(InvalidCacheBackendKeyException):
             self.cache_service.get_backend("what_doesnot_exist_will_raise_exception")
 
 
 class TestCacheServiceAsync:
-    def setup(self):
+    def setup_method(self):
         self.cache_service = CacheService(dict(default=LocalMemCacheBackend()))
 
     async def test_set_async(self, anyio_backend):
         assert await self.cache_service.set_async("test", "1", 0.1)
         value = await self.cache_service.get_async("test")
         assert value == "1"
```

### Comparing `ellar-0.3.4/tests/test_cache/test_local_cache.py` & `ellar-0.3.6/tests/test_cache/test_local_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
 
 
 class TestLocalMemCacheBackend:
-    def setup(self):
+    def setup_method(self):
         self.backend = LocalMemCacheBackend()
 
     def test_set(self):
         assert self.backend.set("test", "1", 0.1)
         value = self.backend.get("test")
         assert value == "1"
 
@@ -50,15 +50,15 @@
 
         self.backend.decr("test-decr-backend", 2, version="1")
         self.backend.decr("test-decr-backend", 3, version="1")
         assert self.backend.get("test-decr-backend") == 0
 
 
 class TestLocalMemCacheBackendAsync:
-    def setup(self):
+    def setup_method(self):
         self.backend = LocalMemCacheBackend()
 
     async def test_set_async(self, anyio_backend):
         assert await self.backend.set_async("test", "1", 0.1)
         value = await self.backend.get_async("test")
         assert value == "1"
```

### Comparing `ellar-0.3.4/tests/test_cache/test_module_setup.py` & `ellar-0.3.6/tests/test_cache/test_module_setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ellar.cache import CacheModule, ICacheService
 from ellar.cache.backends.local_cache import LocalMemCacheBackend
-from ellar.core import TestClientFactory
+from ellar.testing import Test
 
 
 def test_cache_module_setup_works():
-    tm = TestClientFactory.create_test_module(
+    tm = Test.create_test_module(
         modules=[
             CacheModule.setup(
                 default=LocalMemCacheBackend(),
                 local=LocalMemCacheBackend(version=2, ttl=400),
             )
         ]
     )
 
-    cache_service = tm.app.injector.get(ICacheService)
+    cache_service = tm.get(ICacheService)
     assert cache_service
     local = cache_service.get_backend("local")
 
     assert local._version == 2
     assert local._default_ttl == 400
```

### Comparing `ellar-0.3.4/tests/test_cache/test_pylibmc_cache.py` & `ellar-0.3.6/tests/test_cache/test_pylibmc_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     assert value == "Wanaka"
     sleep(1.1)
     value = await backend.get_async("test")
     assert not value
 
 
 class TestPyLibMCCacheBackend:
-    def setup(self):
+    def setup_method(self):
         self.backend = PyLibMCCacheBackendMock(servers=["127.0.0.1:11211"])
 
     def test_set(self):
         assert self.backend.set("test", "1", 1)
         value = self.backend.get("test")
         assert value == "1"
 
@@ -109,15 +109,15 @@
         )
         with pytest.warns(CacheKeyWarning) as wa:
             self.backend.set(key, "value")
         assert str(wa.list[0].message) == str(CacheKeyWarning(expected_warning))
 
 
 class TestPyLibMCCacheBackendAsync:
-    def setup(self):
+    def setup_method(self):
         self.backend = PyLibMCCacheBackendMock(servers=["127.0.0.1:11211"])
 
     async def test_set_async(self, anyio_backend):
         assert await self.backend.set_async("test", "1", 1)
         value = await self.backend.get_async("test")
         assert value == "1"
```

### Comparing `ellar-0.3.4/tests/test_cache/test_redis_cache.py` & `ellar-0.3.6/tests/test_cache/test_redis_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     assert value == "Wanaka"
     sleep(1.1)
     value = await backend.get_async("test")
     assert not value
 
 
 class TestRedisCacheBackend:
-    def setup(self):
+    def setup_method(self):
         self.backend = RedisCacheBackendMock(
             servers=[
                 "redis://localhost:6379/0",
                 "redis://localhost:6379/1",
                 "redis://localhost:6379/2",
             ]
         )
@@ -88,15 +88,15 @@
         )
         with pytest.warns(CacheKeyWarning) as wa:
             self.backend.set(key, "value")
         assert str(wa.list[0].message) == str(CacheKeyWarning(expected_warning))
 
 
 class TestRedisCacheBackendAsync:
-    def setup(self):
+    def setup_method(self):
         self.backend = RedisCacheBackendMock(
             servers=[
                 "redis://localhost:6379/0",
                 "redis://localhost:6379/1",
                 "redis://localhost:6379/2",
             ]
         )
```

### Comparing `ellar-0.3.4/tests/test_cache/test_schema.py` & `ellar-0.3.6/tests/test_cache/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_cache.py` & `ellar-0.3.6/tests/test_cache/test_cache_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from time import sleep
 
 from ellar.cache import CacheModule, cache
 from ellar.common import ModuleRouter
-from ellar.core import TestClientFactory
 from ellar.core.response import PlainTextResponse
+from ellar.testing import Test
 
 
 def test_cache_route_function_return_data():
     called_count = 0
 
     mr = ModuleRouter()
 
@@ -15,20 +15,20 @@
     @cache(ttl=0.12)  # cache for 3sec
     def homepage():
         nonlocal called_count
 
         called_count += 1
         return dict(message="Response Information cached.")
 
-    client = TestClientFactory.create_test_module(
+    client = Test.create_test_module(
         modules=[CacheModule.register_setup()],
         routers=[
             mr,
         ],
-    ).get_client()
+    ).get_test_client()
 
     for i in range(2):
         client.get("/index")
 
     sleep(0.22)
     res = client.get("/index")
 
@@ -46,20 +46,20 @@
     @cache(ttl=3)  # cache for 3sec
     async def homepage():
         nonlocal called_count
 
         called_count += 1
         return dict(message="Response Information cached Async")
 
-    client = TestClientFactory.create_test_module(
+    client = Test.create_test_module(
         modules=[CacheModule.register_setup()],
         routers=[
             mr,
         ],
-    ).get_client()
+    ).get_test_client()
     res = client.get("/index")
     for i in range(2):
         res = client.get("/index")
 
     assert res.json() == dict(message="Response Information cached Async")
     assert res.status_code == 200
     assert called_count == 1
@@ -74,20 +74,20 @@
     @cache(ttl=3)  # cache for 3sec
     async def homepage():
         nonlocal called_count
 
         called_count += 1
         return PlainTextResponse("Response Information cached Async")
 
-    client = TestClientFactory.create_test_module(
+    client = Test.create_test_module(
         modules=[CacheModule.register_setup()],
         routers=[
             mr,
         ],
-    ).get_client()
+    ).get_test_client()
 
     res = client.get("/index")
 
     assert res.text == "Response Information cached Async"
     assert res.status_code == 200
     assert called_count == 1
 
@@ -101,19 +101,19 @@
     @cache(ttl=2)  # cache for 3sec
     def homepage():
         nonlocal called_count
 
         called_count += 1
         return PlainTextResponse("Response Information cached")
 
-    client = TestClientFactory.create_test_module(
+    client = Test.create_test_module(
         modules=[CacheModule.register_setup()],
         routers=[
             mr,
         ],
-    ).get_client()
+    ).get_test_client()
 
     res = client.get("/index")
 
     assert res.text == "Response Information cached"
     assert res.status_code == 200
     assert called_count == 1
```

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_controller.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
 
-from ellar.common import Controller, set_metadata
+from ellar.common import Controller, Guards, Version, set_metadata
 from ellar.constants import CONTROLLER_METADATA, GUARDS_KEY, NOT_SET, VERSIONING_KEY
 from ellar.core import ControllerBase
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.reflect import reflect
 
 
 @set_metadata("OtherAttributes", "Something")
 @Controller(
     prefix="/decorator",
     description="Some description",
     external_doc_description="external",
-    guards=[],
-    version=("v1",),
     tag="dec",
     external_doc_url="https://example.com",
     name="test",
 )
+@Version("v1")
+@Guards()
 class ControllerDecorationTest:
     pass
 
 
 @Controller
 class ControllerDefaultTest:
     pass
@@ -47,16 +47,16 @@
 
     assert reflect.get_metadata(CONTROLLER_METADATA.OPENAPI, ControllerDefaultTest) == {
         "tag": NOT_SET,
         "description": None,
         "external_doc_description": None,
         "external_doc_url": None,
     }
-    assert reflect.get_metadata(GUARDS_KEY, ControllerDefaultTest) == []
-    assert reflect.get_metadata(VERSIONING_KEY, ControllerDefaultTest) == set()
+    assert reflect.get_metadata(GUARDS_KEY, ControllerDefaultTest) is None
+    assert reflect.get_metadata(VERSIONING_KEY, ControllerDefaultTest) is None
     assert (
         reflect.get_metadata(CONTROLLER_METADATA.PATH, ControllerDefaultTest)
         == "/defaulttest"
     )
     assert (
         reflect.get_metadata(
             CONTROLLER_METADATA.INCLUDE_IN_SCHEMA, ControllerDefaultTest
```

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_exception.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_file.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_guards.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_guards.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ellar.common import guards
+from ellar.common import Guards
 from ellar.constants import GUARDS_KEY
 from ellar.core import ExecutionContext
 from ellar.core.connection import Request
 from ellar.core.guard import GuardCanActivate
 from ellar.reflect import reflect
 
 
@@ -12,20 +12,20 @@
 
 
 class SomeGuard2(SomeGuard):
     async def can_activate(self, context: ExecutionContext) -> bool:
         return False  # pragma: no cover
 
 
-@guards(SomeGuard)
+@Guards(SomeGuard)
 def endpoint(request: Request):
     return "foo"  # pragma: no cover
 
 
-@guards(SomeGuard, SomeGuard2)
+@Guards(SomeGuard, SomeGuard2)
 def endpoint2(request: Request):
     return "foo"  # pragma: no cover
 
 
 def test_guard_decorator_applies_guards_key_to_reflect():
     guard_info = reflect.get_metadata(GUARDS_KEY, endpoint)
     assert guard_info
```

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_html.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_middleware.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_modules.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_openapi.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_common/test_decorators/test_serializer.py` & `ellar-0.3.6/tests/test_common/test_decorators/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_conf/test_default_conf.py` & `ellar-0.3.6/tests/test_conf/test_default_conf.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_conf/test_mixins.py` & `ellar-0.3.6/tests/test_conf/test_mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,13 +28,7 @@
 
 def test_invalid_middleware_config():
     invalid_type = type("whatever", (), {})
     with pytest.raises(
         ValueError, match=r"Expected Type/instance of Middleware, received: "
     ):
         Config(MIDDLEWARE=[invalid_type()])
-
-
-def test_invalid_event_handler_config():
-    invalid_type = type("whatever", (), {})
-    with pytest.raises(ValueError, match=r"Expected EventHandler, received:"):
-        Config(ON_REQUEST_STARTUP=[invalid_type()])
```

### Comparing `ellar-0.3.4/tests/test_controller/test_controller_decorator.py` & `ellar-0.3.6/tests/test_controller/test_controller_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_controller/test_controller_inheritance.py` & `ellar-0.3.6/tests/test_controller/test_controller_inheritance.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_controller/test_module_router.py` & `ellar-0.3.6/tests/test_controller/test_module_router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_controller/test_route_collection.py` & `ellar-0.3.6/tests/test_controller/test_route_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import List
 
 import pytest
 from starlette.responses import JSONResponse
 from starlette.routing import Host, Mount
 
-from ellar.common import get, http_route, version as version_decorator, ws_route
+from ellar.common import Version as version_decorator, get, http_route, ws_route
 from ellar.constants import CONTROLLER_CLASS_KEY, CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core import TestClientFactory
 from ellar.core.routing import RouteOperation, WebsocketRouteOperation
 from ellar.core.routing.router import RouteCollection
 from ellar.core.versioning import UrlPathAPIVersioning
 from ellar.helper import generate_controller_operation_unique_id
 from ellar.reflect import reflect
+from ellar.testing import Test
 
 
 class Configuration:
     VERSIONING_SCHEME = UrlPathAPIVersioning()
 
 
 config_path = "tests.test_controller.test_route_collection:Configuration"
@@ -68,17 +68,17 @@
     routes = collection_model()
     routes.append(create_route_operation("/sample", methods=["post"], versions=[]))
     routes.append(create_route_operation("/sample", methods=["post"], versions=["1"]))
     assert len(routes) == 2
     for route in routes:
         assert route.path == "/sample"
 
-    tm = TestClientFactory.create_test_module(config_module=config_path)
-    tm.app.router.extend(routes)
-    client = tm.get_client()
+    tm = Test.create_test_module(config_module=config_path)
+    tm.create_application().router.extend(routes)
+    client = tm.get_test_client()
 
     response = client.post("/sample")
     assert response.status_code == 200
     assert response.json() == {"path": "/sample", "methods": ["post"], "versioning": []}
 
     response = client.post("/v1/sample")
     assert response.status_code == 200
@@ -167,17 +167,17 @@
     routes.append(create_route_operation("/sample", methods=["post"], versions=[]))
     routes.append(
         create_route_operation("/sample", methods=["post", "get"], versions=[])
     )
 
     assert len(routes) == 2
 
-    tm = TestClientFactory.create_test_module(config_module=config_path)
-    tm.app.router.extend(routes)
-    client = tm.get_client()
+    tm = Test.create_test_module(config_module=config_path)
+    tm.create_application().router.extend(routes)
+    client = tm.get_test_client()
 
     response = client.get("/sample")
     assert response.status_code == 200
     assert response.json() == {
         "path": "/sample",
         "methods": ["post", "get"],
         "versioning": [],
```

### Comparing `ellar-0.3.4/tests/test_di/examples.py` & `ellar-0.3.6/tests/test_di/examples.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_di/test_injectable_resolving.py` & `ellar-0.3.6/tests/test_di/test_injectable_resolving.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_di/test_injector.py` & `ellar-0.3.6/tests/test_di/test_injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         assert isinstance(asgi_context.context[Foo], ClassProvider)
 
     injector.update_scoped_context(Foo1, Foo1())
     assert SCOPED_CONTEXT_VAR.get() is None
 
 
 class TestInjectorModuleFunctions:
-    def setup(self):
+    def setup_method(self):
         self.injector = EllarInjector()
         config = Config()
 
         assert isinstance(
             self.injector._modules[MODULE_REF_TYPES.TEMPLATE], OrderedDict
         )
         assert isinstance(self.injector._modules[MODULE_REF_TYPES.PLAIN], OrderedDict)
```

### Comparing `ellar-0.3.4/tests/test_di/test_provider_scopes.py` & `ellar-0.3.6/tests/test_di/test_provider_scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_di/test_providers.py` & `ellar-0.3.6/tests/test_di/test_providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_events.py` & `ellar-0.3.6/tests/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from ellar.constants import NOT_SET
 from ellar.core import Config
-from ellar.core.events import EventHandler, RouterEventManager
+from ellar.events import EventHandler, RouterEventManager
 
 
 @pytest.mark.anyio
 async def test_router_event_manager():
     called = 0
 
     def valid_function_1():
```

### Comparing `ellar-0.3.4/tests/test_exceptions/test_api_exception.py` & `ellar-0.3.6/tests/test_exceptions/test_api_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import http
 
 import pytest
 
 from ellar.common import get
-from ellar.core import TestClientFactory
 from ellar.core.exceptions import (
     APIException,
     AuthenticationFailed,
     MethodNotAllowed,
     NotAcceptable,
     NotAuthenticated,
     NotFound,
     PermissionDenied,
     UnsupportedMediaType,
 )
+from ellar.testing import Test
 
 from .exception_runner import ExceptionRunner
 
-test_module = TestClientFactory.create_test_module()
+test_module = Test.create_test_module()
 
 
 _exception_runner = ExceptionRunner(APIException)
 
 
 @get("/exception")
 def exception_():
     _exception_runner.run()
 
 
-test_module.app.router.append(exception_)
-client = test_module.get_client()
+test_module.create_application().router.append(exception_)
+client = test_module.get_test_client()
 
 
 @pytest.mark.parametrize(
     "exception, status_code, default_detail",
     [
         (
             APIException,
```

### Comparing `ellar-0.3.4/tests/test_exceptions/test_custom_exceptions.py` & `ellar-0.3.6/tests/test_exceptions/test_custom_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 import pytest
 from pydantic.error_wrappers import ValidationError
 from starlette.exceptions import HTTPException
 from starlette.responses import JSONResponse, Response
 
 from ellar.common import get
-from ellar.core import Config, TestClientFactory
+from ellar.core import Config
 from ellar.core.context import IHostContext
 from ellar.core.exceptions.callable_exceptions import CallableExceptionHandler
 from ellar.core.exceptions.handlers import APIException, APIExceptionHandler
 from ellar.core.exceptions.interfaces import IExceptionHandler
 from ellar.core.exceptions.service import ExceptionMiddlewareService
 from ellar.core.middleware import ExceptionMiddleware
+from ellar.testing import Test
 
 
 class InvalidExceptionHandler:
     pass
 
 
 class NewException(Exception):
@@ -132,34 +133,36 @@
 
 
 def test_custom_exception_works():
     @get()
     def homepage():
         raise NewException("New Exception")
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.add_exception_handler(NewExceptionHandler())
+    tm = Test.create_test_module()
+    app = tm.create_application()
+    app.router.append(homepage)
+    app.add_exception_handler(NewExceptionHandler())
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/")
     assert res.status_code == 400
     assert res.json() == {"detail": "New Exception"}
 
 
 def test_exception_override_works():
     @get()
     def homepage():
         raise APIException("New APIException")
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.add_exception_handler(OverrideAPIExceptionHandler())
+    tm = Test.create_test_module()
+    app = tm.create_application()
+    app.router.append(homepage)
+    app.add_exception_handler(OverrideAPIExceptionHandler())
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/")
     assert res.status_code == 404
     assert res.json() == {"detail": "New APIException"}
 
 
 @pytest.mark.parametrize(
     "exception_handler",
@@ -171,47 +174,53 @@
     ],
 )
 def test_500_error_as_a_function(exception_handler):
     @get()
     def homepage():
         raise RuntimeError("Server Error")
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.add_exception_handler(exception_handler)
+    tm = Test.create_test_module()
+    app = tm.create_application()
 
-    client = tm.get_client(raise_server_exceptions=False)
+    app.router.append(homepage)
+    app.add_exception_handler(exception_handler)
+
+    client = tm.get_test_client(raise_server_exceptions=False)
     res = client.get("/")
     assert res.status_code == 500
     assert res.json() == {"detail": "Server Error"}
 
 
 def test_raise_default_http_exception():
     @get()
     def homepage():
         raise HTTPException(detail="Bad Request", status_code=400)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    client = tm.get_client()
+    tm = Test.create_test_module()
+    app = tm.create_application()
+
+    app.router.append(homepage)
+    client = tm.get_test_client()
     res = client.get("/")
     assert res.status_code == 400
     assert res.json() == {"detail": "Bad Request", "status_code": 400}
 
 
 @pytest.mark.parametrize("status_code", [204, 304])
 def test_raise_default_http_exception_for_204_and_304(status_code):
     @get()
     def homepage():
         raise HTTPException(detail="Server Error", status_code=status_code)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
+    tm = Test.create_test_module()
+    app = tm.create_application()
+
+    app.router.append(homepage)
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     res = client.get("/")
     assert res.status_code == status_code
     assert res.text == ""
 
 
 def test_debug_after_response_sent(test_client_factory):
     async def app(scope, receive, send):
@@ -230,45 +239,50 @@
 
 
 def test_application_add_exception_handler():
     @get()
     def homepage():
         raise HTTPException(detail="Bad Request", status_code=400)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.add_exception_handler(OverrideHTTPException())
+    tm = Test.create_test_module()
+    app = tm.create_application()
 
-    client = tm.get_client()
+    app.router.append(homepage)
+    app.add_exception_handler(OverrideHTTPException())
+
+    client = tm.get_test_client()
     res = client.get("/")
 
     assert res.status_code == 400
     assert res.json() == {"detail": "HttpException Override"}
 
 
 def test_application_http_exception_handler_raise_exception_for_returning_none():
     @get()
     def homepage():
         raise HTTPException(detail="Bad Request", status_code=400)
 
-    tm = TestClientFactory.create_test_module()
-    tm.app.router.append(homepage)
-    tm.app.add_exception_handler(RuntimeHTTPException())
+    tm = Test.create_test_module()
+    app = tm.create_application()
+
+    app.router.append(homepage)
+    app.add_exception_handler(RuntimeHTTPException())
     with pytest.raises(
         RuntimeError, match="HTTP ExceptionHandler must return a response."
     ):
-        tm.get_client().get("/")
+        tm.get_test_client().get("/")
 
 
 def test_application_adding_same_exception_twice():
-    tm = TestClientFactory.create_test_module()
+    tm = Test.create_test_module()
+    app = tm.create_application()
     with patch.object(
-        tm.app.__class__, "rebuild_middleware_stack"
+        app.__class__, "rebuild_middleware_stack"
     ) as rebuild_middleware_stack_mock:
-        tm.app.add_exception_handler(OverrideHTTPException())
+        app.add_exception_handler(OverrideHTTPException())
     rebuild_middleware_stack_mock.assert_called()
 
     with patch.object(
-        tm.app.__class__, "rebuild_middleware_stack"
+        app.__class__, "rebuild_middleware_stack"
     ) as rebuild_middleware_stack_mock:
-        tm.app.add_exception_handler(OverrideHTTPException())
+        app.add_exception_handler(OverrideHTTPException())
     assert rebuild_middleware_stack_mock.call_count == 0
```

### Comparing `ellar-0.3.4/tests/test_exceptions/test_error_details.py` & `ellar-0.3.6/tests/test_exceptions/test_error_details.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_exceptions/test_validation_exception.py` & `ellar-0.3.6/tests/test_exceptions/test_validation_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 from pydantic.error_wrappers import ErrorWrapper
 
 from ellar.common import Ws, WsBody, get, ws_route
-from ellar.core import TestClientFactory
 from ellar.core.exceptions.validation import (
     RequestValidationError,
     WebSocketRequestValidationError,
 )
+from ellar.testing import Test
 
 from .exception_runner import ExceptionRunner
 
-test_module = TestClientFactory.create_test_module()
+test_module = Test.create_test_module()
 
 _exception_runner = ExceptionRunner(RequestValidationError)
 
 
 @get("/exception-validation")
 def exception_http():
     _exception_runner.run()
@@ -27,16 +27,18 @@
 
 @ws_route("/exception-Ws-2", use_extra_handler=True)
 async def exception_ws_2(*, websocket=Ws(), data: dict = WsBody()):
     assert data == {"hello": "world"}
     _exception_runner.run()
 
 
-test_module.app.router.extend([exception_http, exception_ws_2, exception_ws])
-client = test_module.get_client()
+test_module.create_application().router.extend(
+    [exception_http, exception_ws_2, exception_ws]
+)
+client = test_module.get_test_client()
 
 
 def test_request_validation_error():
     global _exception_runner
     _exception_runner = ExceptionRunner(
         RequestValidationError,
         errors=[
```

### Comparing `ellar-0.3.4/tests/test_guard.py` & `ellar-0.3.6/tests/test_guard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pytest
 from starlette.status import HTTP_401_UNAUTHORIZED
 
-from ellar.common import Req, get, guards
-from ellar.core import AppFactory, TestClient
+from ellar.common import Guards, Req, get
+from ellar.core import AppFactory
 from ellar.core.exceptions import APIException
 from ellar.core.guard import (
     APIKeyCookie,
     APIKeyHeader,
     APIKeyQuery,
     HttpBasicAuth,
     HttpBearerAuth,
     HttpDigestAuth,
 )
 from ellar.di import injectable
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
 from ellar.services import Reflector
+from ellar.testing import TestClient
 
 
 class CustomException(APIException):
     pass
 
 
 @injectable()
@@ -93,23 +94,23 @@
     ("basic", BasicAuth()),
     ("bearer", BearerAuth),
     ("digest", DigestAuth),
     ("customexception", HeaderSecretKeyCustomException),
 ]:
 
     @get(f"/{_path}")
-    @guards(auth)
+    @Guards(auth)
     def auth_demo_endpoint(request=Req()):
         return {"authentication": request.user}
 
     app.router.append(auth_demo_endpoint)
 
 client = TestClient(app)
 
-BODY_UNAUTHORIZED_DEFAULT = {"detail": "Not authenticated"}
+BODY_UNAUTHORIZED_DEFAULT = {"detail": "Forbidden"}
 
 
 @pytest.mark.parametrize(
     "path,kwargs,expected_code,expected_body",
     [
         ("/apikeyquery", {}, HTTP_401_UNAUTHORIZED, BODY_UNAUTHORIZED_DEFAULT),
         (
```

### Comparing `ellar-0.3.4/tests/test_helper/test_enum.py` & `ellar-0.3.6/tests/test_helper/test_enum.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_helper/test_model_field.py` & `ellar-0.3.6/tests/test_helper/test_model_field.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_middleware/test_functional_middleware.py` & `ellar-0.3.6/tests/test_middleware/test_functional_middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 
 from ellar.common import Module, ModuleRouter, middleware
-from ellar.core import TestClientFactory
 from ellar.core.context import IHostContext
+from ellar.testing import Test
 
 mr = ModuleRouter()
 
 
 @mr.get()
 def homepage(request: Request):
     if request.headers.get("modified_header"):
@@ -39,31 +39,31 @@
         request = context.switch_to_http_connection().get_request()
         if request.headers.get("ellar"):
             return PlainTextResponse("middleware_return_response returned a response")
         await call_next()
 
 
 def test_middleware_modifying_response():
-    tm = TestClientFactory.create_test_module_from_module(ModuleMiddleware)
-    client = tm.get_client()
+    tm = Test.create_test_module(modules=[ModuleMiddleware])
+    client = tm.get_test_client()
 
     response = client.get("/")
     assert response.status_code == 200
     assert response.headers["modified-header"] == "Ellar"
 
 
 def test_middleware_modifying_request():
-    tm = TestClientFactory.create_test_module_from_module(ModuleMiddleware)
-    client = tm.get_client()
+    tm = Test.create_test_module(modules=[ModuleMiddleware])
+    client = tm.get_test_client()
 
     response = client.get("/", headers={"set-user": "set"})
     assert response.status_code == 200
     assert response.json() == {"username": "Ellar"}
 
 
 def test_middleware_returns_response():
-    tm = TestClientFactory.create_test_module_from_module(ModuleMiddleware)
-    client = tm.get_client()
+    tm = Test.create_test_module(modules=[ModuleMiddleware])
+    client = tm.get_test_client()
 
     response = client.get("/", headers={"ellar": "set"})
     assert response.status_code == 200
     assert response.text == "middleware_return_response returned a response"
```

### Comparing `ellar-0.3.4/tests/test_middleware/test_service_provider_middleware.py` & `ellar-0.3.6/tests/test_middleware/test_service_provider_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
 import pytest
 
 from ellar.constants import SCOPE_SERVICE_PROVIDER
 from ellar.core import Config
 from ellar.core.context import HostContextException, IHostContextFactory
+from ellar.core.core_service_registration import CoreServiceRegistration
 from ellar.core.middleware import RequestServiceProviderMiddleware
-from ellar.core.services import CoreServiceRegistration
 from ellar.di import EllarInjector
 
 from ..injector_module import Configuration, DummyModule
 
 
 async def assert_service_provider_app(scope, receive, send):
     assert scope[SCOPE_SERVICE_PROVIDER]
```

### Comparing `ellar-0.3.4/tests/test_middleware/test_versioning_middleware.py` & `ellar-0.3.6/tests/test_middleware/test_versioning_middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 import pytest
 
 from ellar.constants import SCOPE_API_VERSIONING_RESOLVER
-from ellar.core import Config, TestClient
+from ellar.core import Config
 from ellar.core.middleware import RequestVersioningMiddleware
 from ellar.core.versioning import (
     DefaultAPIVersioning,
     HeaderAPIVersioning,
     HostNameAPIVersioning,
     QueryParameterAPIVersioning,
     UrlPathAPIVersioning,
@@ -15,14 +15,15 @@
 from ellar.core.versioning.resolver import (
     DefaultAPIVersionResolver,
     HeaderVersionResolver,
     HostNameAPIVersionResolver,
     QueryParameterAPIVersionResolver,
     UrlPathVersionResolver,
 )
+from ellar.testing import TestClient
 
 config = Config(VERSION_RESOLVER_TYPE=DefaultAPIVersionResolver)
 
 
 async def assert_version_middleware_app(scope, receive, send):
     assert scope[SCOPE_API_VERSIONING_RESOLVER]
```

### Comparing `ellar-0.3.4/tests/test_modules/sample.py` & `ellar-0.3.6/tests/test_modules/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_modules/test_module_config.py` & `ellar-0.3.6/tests/test_modules/test_module_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from abc import ABC
+from unittest.mock import patch
 
 import pytest
 
 from ellar.common import Controller, Module, ModuleRouter, get
 from ellar.constants import MODULE_METADATA
 from ellar.core import (
     App,
     Config,
     ControllerBase,
     DynamicModule,
     IModuleSetup,
     ModuleBase,
     ModuleSetup,
-    TestClientFactory,
 )
 from ellar.di import EllarInjector, ProviderConfig
 from ellar.reflect import reflect
 from ellar.services import Reflector
+from ellar.testing import Test
 
 from ..main import router
 
 
 class IDynamic(ABC):
     a: int
     b: float
@@ -76,54 +77,55 @@
         return module.setup(config.a, config.b)
 
 
 def test_dynamic_module_haves_routes():
     routers = reflect.get_metadata(MODULE_METADATA.ROUTERS, DynamicInstantiatedModule)
     assert len(routers) == 1
     assert len(routers[0].routes) == 39
-    TestClientFactory.create_test_module(
+    tm = Test.create_test_module(
         modules=(DynamicInstantiatedModule.setup(a=233, b=344),)
     )
+    tm.create_application()
     routers = reflect.get_metadata(MODULE_METADATA.ROUTERS, DynamicInstantiatedModule)
     assert len(routers) == 1
     assert len(routers[0].routes) == 1
 
 
 def test_dynamic_module_setup_providers_works():
-    test_module = TestClientFactory.create_test_module(
+    test_module = Test.create_test_module(
         modules=(DynamicInstantiatedModule.setup(a=233, b=344),)
     )
-    dynamic_object = test_module.app.injector.get(IDynamic)
+    dynamic_object = test_module.get(IDynamic)
     assert dynamic_object.a == 233 and dynamic_object.b == 344
 
 
 def test_dynamic_module_setup_router_controllers_works():
-    test_module = TestClientFactory.create_test_module(
+    test_module = Test.create_test_module(
         modules=(DynamicInstantiatedModule.setup(a=233, b=344),)
     )
-    assert len(test_module.app.routes) == 2
-    client = test_module.get_client()
+    assert len(test_module.create_application().routes) == 2
+    client = test_module.get_test_client()
 
     res = client.get("/dynamic/index")
     assert res.status_code == 200
     assert res.json() == {"message": 'You have reached "dynamic" home route'}
 
     res = client.get("/dynamic-controller/sample")
     assert res.status_code == 200
     assert res.json() == {"message": 'You have reached "sample_example" home route'}
 
 
 def test_dynamic_module_setup_register_works():
     with reflect.context():
-        test_module = TestClientFactory.create_test_module(
+        test_module = Test.create_test_module(
             modules=(DynamicModuleSetupRegisterModule.setup_register(),),
             config_module=dict(a=24555, b=8899900),
         )
-        assert len(test_module.app.routes) == 0
-        dynamic_instance = test_module.app.injector.get(IDynamic)
+        assert len(test_module.create_application().routes) == 0
+        dynamic_instance = test_module.get(IDynamic)
         assert dynamic_instance.a == 24555
         assert dynamic_instance.b == 8899900
 
 
 @pytest.mark.parametrize(
     "name, dependencies",
     [
@@ -138,27 +140,27 @@
 )
 def test_module_setup_with_factory_works(name, dependencies):
     def dynamic_instantiate_factory(module: DynamicInstantiatedModule, *args):
         for _type, instance in zip(dependencies, args):
             assert isinstance(instance, _type)
         return module.setup(a=233, b=344)
 
-    test_module = TestClientFactory.create_test_module(
+    test_module = Test.create_test_module(
         modules=[
             ModuleSetup(
                 DynamicInstantiatedModule,
                 factory=dynamic_instantiate_factory,
                 inject=dependencies,
             )
         ]
     )
 
-    dynamic_object = test_module.app.injector.get(IDynamic)
+    dynamic_object = test_module.get(IDynamic)
     assert dynamic_object.a == 233 and dynamic_object.b == 344
-    client = test_module.get_client()
+    client = test_module.get_test_client()
 
     res = client.get("/dynamic/index")
     assert res.status_code == 200
     assert res.json() == {"message": 'You have reached "dynamic" home route'}
 
 
 def test_invalid_module_setup():
@@ -184,7 +186,22 @@
     )
 
 
 def test_invalid_dynamic_module_setup():
     with pytest.raises(Exception) as ex:
         DynamicModule(module=IDynamic)
     assert str(ex.value) == "IDynamic is not a valid Module"
+
+
+def test_can_not_apply_dynamic_module_twice():
+    dynamic_type = type("DynamicSample", (IDynamic,), {"a": "1222", "b": "121212"})
+    with patch.object(reflect.__class__, "define_metadata") as mock_define_metadata:
+        dynamic_module = DynamicModule(
+            module=DynamicInstantiatedModule,
+            providers=[ProviderConfig(IDynamic, use_class=dynamic_type)],
+        )
+        dynamic_module.apply_configuration()
+        assert mock_define_metadata.called
+
+    with patch.object(reflect.__class__, "define_metadata") as mock_define_metadata:
+        dynamic_module.apply_configuration()
+        assert mock_define_metadata.called is False
```

### Comparing `ellar-0.3.4/tests/test_openapi/test_builder.py` & `ellar-0.3.6/tests/test_openapi/test_builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_openapi/test_module.py` & `ellar-0.3.6/tests/test_openapi/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import os
 
 import pytest
 
-from ellar.core import (
-    AppFactory,
-    Config,
-    ExecutionContext,
-    GuardCanActivate,
-    TestClient,
-)
+from ellar.core import AppFactory, Config, ExecutionContext, GuardCanActivate
 from ellar.core.modules.ref import create_module_ref_factor
 from ellar.di import EllarInjector
 from ellar.openapi import (
     OpenAPIDocumentBuilder,
     OpenAPIDocumentModule,
     ReDocDocumentGenerator,
     SwaggerDocumentGenerator,
 )
+from ellar.testing import TestClient
 
 
 class CustomDocsGuard(GuardCanActivate):
     detail: str = "Not Allowed"
 
     async def can_activate(self, context: ExecutionContext) -> bool:
         return False
```

### Comparing `ellar-0.3.4/tests/test_openapi/test_open_api_route_documentation.py` & `ellar-0.3.6/tests/test_openapi/test_open_api_route_documentation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_reflect.py` & `ellar-0.3.6/tests/test_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_reflector.py` & `ellar-0.3.6/tests/test_reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_response/test_defined_response_model.py` & `ellar-0.3.6/tests/test_response/test_defined_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_response/test_pydantic_response_model.py` & `ellar-0.3.6/tests/test_response/test_pydantic_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_response/test_response_file.py` & `ellar-0.3.6/tests/test_response/test_response_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
 import pytest
 
 from ellar.common import Controller, file, get
-from ellar.core import TestClientFactory
 from ellar.core.response.model import FileResponseModel
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 FILE_RESPONSE_SCHEMA = {
     "200": {
         "description": "Successful Response",
         "content": {"text/css": {"schema": {"type": "string"}}},
     }
@@ -55,32 +55,33 @@
         return {
             "path": f"{BASEDIR}/private/test.css",
             "filename": "file-test-css.css",
             "content_disposition_type": "whatever",
         }
 
 
-test_module = TestClientFactory.create_test_module(
+test_module = Test.create_test_module(
     controllers=(EllarController,),
     routers=(mr,),
 )
-document = serialize_object(OpenAPIDocumentBuilder().build_document(test_module.app))
+app = test_module.create_application()
+document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
 
 
 @pytest.mark.parametrize(
     "path",
     [
         "/ellar/index-manual",
         "/ellar/index-decorator",
         "/mr/index-manual",
         "/mr/index-decorator",
     ],
 )
 def test_file_response_for_module_router_and_controller(path):
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get(path)
     response.raise_for_status()
     assert (
         response.headers["content-disposition"]
         == 'attachment; filename="file-test-css.css"'
     )
     assert response.headers["content-length"] == "23"
@@ -99,15 +100,15 @@
 )
 def test_response_schema(path):
     path_response = document["paths"][path]["get"]["responses"]
     assert path_response == FILE_RESPONSE_SCHEMA
 
 
 def test_invalid_parameter_returned():
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get("/ellar/index-invalid")
     assert response.status_code == 422
 
     assert response.json() == {
         "detail": [
             {
                 "loc": ["response_model", "content_disposition_type"],
```

### Comparing `ellar-0.3.4/tests/test_response/test_response_html.py` & `ellar-0.3.6/tests/test_response/test_response_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from pathlib import Path
 
 import pytest
 from jinja2 import TemplateNotFound
 
 from ellar.common import Controller, get, render
 from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY
-from ellar.core import TestClientFactory
 from ellar.core.response.model import HTMLResponseModel
 from ellar.core.response.model.html import HTMLResponseModelRuntimeError
 from ellar.core.routing import ModuleRouter
 from ellar.reflect import reflect
+from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 
 
 @Controller
 class EllarController:
     @get(
@@ -58,15 +58,15 @@
 
 @mr.get("/render_template2")
 @render(template_name="index")
 def render_template():
     return {}
 
 
-test_module = TestClientFactory.create_test_module(
+test_module = Test.create_test_module(
     template_folder="templates",
     base_directory=BASEDIR,
     controllers=(EllarController,),
     routers=(mr,),
 )
 
 
@@ -76,15 +76,15 @@
         ("/ellar/index", "ellar/index.html"),
         ("/ellar/index2", "ellar/index.html"),
         ("/ellar/another_index", "ellar/index.html"),
         ("/ellar/another_index2", "ellar/index.html"),
     ],
 )
 def test_ellar_index_should_use_controller_name_with_function_name(path, template):
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get(path)
     response.raise_for_status()
     content = re.sub("\\s+", " ", response.text).strip()
     assert (
         content == '<html lang="en"> <head> <meta charset="UTF-8"> '
         '<title>Ellar Index Page</title> </head> <a href="http://testserver/ellar/another_index">world</a> '
         "</html>"
@@ -97,15 +97,15 @@
     "path, template",
     [
         ("/render_template", "index.html"),
         ("/render_template2", "index.html"),
     ],
 )
 def test_function_template_rendering(path, template):
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get(path)
     response.raise_for_status()
     content = re.sub("\\s+", " ", response.text).strip()
     assert (
         content == '<!DOCTYPE html> <html lang="en"> '
         '<head> <meta charset="UTF-8"> <title>Index Page</title> </head> <body> </body> </html>'
     )
@@ -145,15 +145,15 @@
     @get(
         "/runtime_controller_error_1",
         response=HTMLResponseModel(template_name="index2", use_mvc=True),
     )
     def runtime_controller_error_1():
         pass
 
-    test_module.app.router.extend(
+    test_module.create_application().router.extend(
         [runtime_error_1, runtime_error_2, runtime_controller_error_1]
     )
     runtime_error_1_handler = reflect.get_metadata(
         CONTROLLER_OPERATION_HANDLER_KEY, runtime_error_1
     )
     runtime_error_2_handler = reflect.get_metadata(
         CONTROLLER_OPERATION_HANDLER_KEY, runtime_error_2
@@ -161,15 +161,15 @@
 
     assert isinstance(
         runtime_error_1_handler.response_model.models[200], HTMLResponseModel
     )
     assert isinstance(
         runtime_error_2_handler.response_model.models[200], HTMLResponseModel
     )
-    client = test_module.get_client()
+    client = test_module.get_test_client()
 
     with pytest.raises(TemplateNotFound):
         client.get("/runtime_error_1")
 
     with pytest.raises(TemplateNotFound):
         client.get("/runtime_error_2")
```

### Comparing `ellar-0.3.4/tests/test_response/test_response_streaming.py` & `ellar-0.3.6/tests/test_response/test_response_streaming.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 from pathlib import Path
 
 import pytest
 
 from ellar.common import Controller, file, get
-from ellar.core import TestClientFactory
 from ellar.core.response.model import (
     StreamingResponseModel,
     StreamingResponseModelInvalidContent,
 )
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 FILE_RESPONSE_SCHEMA = {
     "200": {
         "description": "Successful Response",
         "content": {"text/html": {"schema": {"type": "string"}}},
     }
@@ -69,32 +69,33 @@
         return {
             "path": f"{BASEDIR}/private/test.css",
             "filename": "file-test-css.css",
             "content_disposition_type": "whatever",
         }
 
 
-test_module = TestClientFactory.create_test_module(
+test_module = Test.create_test_module(
     controllers=(EllarController,),
     routers=(streaming_mr,),
 )
-document = serialize_object(OpenAPIDocumentBuilder().build_document(test_module.app))
+app = test_module.create_application()
+document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
 
 
 @pytest.mark.parametrize(
     "path",
     [
         "/ellar/index-manual",
         "/ellar/index-decorator",
         "/mr/index-manual",
         "/mr/index-decorator",
     ],
 )
 def test_file_stream_response_for_module_router_and_controller(path):
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get(path)
     response.raise_for_status()
     assert response.status_code == 200
     assert (
         response.text
         == "<html><body><ul><li>1</li><li>2</li><li>3</li><li>4</li></ul></body></html>"
     )
@@ -111,13 +112,13 @@
 )
 def test_response_schema(path):
     path_response = document["paths"][path]["get"]["responses"]
     assert path_response == FILE_RESPONSE_SCHEMA
 
 
 def test_invalid_parameter_returned():
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     with pytest.raises(
         StreamingResponseModelInvalidContent,
         match="Content must typing.AsyncIterable OR typing.Iterable",
     ):
         client.get("/ellar/index-invalid")
```

### Comparing `ellar-0.3.4/tests/test_response/test_response_type_definition_converter.py` & `ellar-0.3.6/tests/test_response/test_response_type_definition_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_response/test_route_response_model.py` & `ellar-0.3.6/tests/test_response/test_route_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_routing/sample.py` & `ellar-0.3.6/tests/test_routing/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_routing/test_body_schema.py` & `ellar-0.3.6/tests/test_routing/test_body_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_routing/test_body_schema_extra_properties.py` & `ellar-0.3.6/tests/test_routing/test_body_schema_extra_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from ellar.common import post
-from ellar.core import TestClientFactory
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
 
 
 class Items_(BaseModel):
     items: Dict[str, int]
 
 
 @post("/foo")
 def foo(items: Items_):
     return items.items
 
 
-tm.app.router.append(foo)
-client = tm.get_client()
+app = tm.create_application()
+app.router.append(foo)
+client = tm.get_test_client()
 
 
 item_openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/foo": {
@@ -104,15 +105,15 @@
         }
     },
     "tags": [],
 }
 
 
 def test_body_extra_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == item_openapi_schema
 
 
 def test_additional_properties_post():
     response = client.post("/foo", json={"items": {"foo": 1, "bar": 2}})
     assert response.status_code == 200, response.text
     assert response.json() == {"foo": 1, "bar": 2}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_body_union_schema.py` & `ellar-0.3.6/tests/test_routing/test_body_union_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Union
 
 from ellar.common import post
-from ellar.core import TestClientFactory
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Item, OtherItem
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
 
 
 @post("/items/")
 def save_union_body(item: Union[OtherItem, Item]):
     return {"item": item}
 
 
-tm.app.router.append(save_union_body)
-client = tm.get_client()
+app = tm.create_application()
+app.router.append(save_union_body)
+
+client = tm.get_test_client()
 
 
 item_openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/items/": {
@@ -105,15 +107,15 @@
         }
     },
     "tags": [],
 }
 
 
 def test_item_openapi_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == item_openapi_schema
 
 
 def test_post_other_item():
     response = client.post("/items/", json={"price": 100})
     assert response.status_code == 200, response.text
     assert response.json() == {"item": {"price": 100}}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_cookie_schema.py` & `ellar-0.3.6/tests/test_routing/test_cookie_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from ellar.common import Cookie, get
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Data, Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 router = ModuleRouter("")
 
 
 @router.get("/test/cookie")
@@ -26,19 +26,20 @@
     request: Request,
     filters: Filter = Cookie(...),
     data: Data = Cookie(...),
 ):
     return dict(filters=filters.dict(), data=data.dict())
 
 
-tm = TestClientFactory.create_test_module(routers=(router,))
+tm = Test.create_test_module(routers=(router,))
+app = tm.create_application()
 
 
 def test_cookie_request():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test/cookie",
         cookies={"from": "1", "to": "2", "range": "20", "foo": "1", "range2": "50"},
     )
     assert response.status_code == 200
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
@@ -49,15 +50,15 @@
     response = client.get(
         "/test/cookie", cookies={"from": "1", "to": "2", "range": "21"}
     )
     assert response.status_code == 422
 
 
 def test_cookie_request_mixed():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test-mixed/cookie",
         cookies={
             "from": "1",
             "to": "2",
             "range": "20",
             "foo": "1",
@@ -79,15 +80,15 @@
     response = client.get(
         "/test-mixed/cookie", cookies={"from": "1", "to": "2", "range": "21"}
     )
     assert response.status_code == 422
 
 
 def test_cookie_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     params = document["paths"]["/test/cookie"]["get"]["parameters"]
     assert params == [
         {
             "required": False,
             "schema": {"title": "To", "type": "string", "format": "date-time"},
             "name": "to",
             "in": "cookie",
```

### Comparing `ellar-0.3.4/tests/test_routing/test_extra_args.py` & `ellar-0.3.6/tests/test_routing/test_extra_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from functools import wraps
 
 from starlette.responses import Response
 
 from ellar.common import Context, Query, Res, extra_args, get
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.context import IExecutionContext
 from ellar.core.params import ExtraEndpointArg
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Filter
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
+app = tm.create_application()
 
 
 def add_additional_signature_to_endpoint(func):
     # EXTRA ARGS SETUP
     query1 = ExtraEndpointArg(name="query1", annotation=str, default_value=Query())
     query2 = ExtraEndpointArg(
         name="query2", annotation=str
@@ -70,15 +71,15 @@
 def query_params_extra(
     request: Request,
     filters: Filter = Query(),
 ):
     return filters.dict()
 
 
-tm.app.router.append(query_params_extra)
+app.router.append(query_params_extra)
 
 openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/test": {
             "get": {
@@ -186,20 +187,20 @@
         }
     },
     "tags": [],
 }
 
 
 def test_openapi_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == openapi_schema
 
 
 def test_query_params_extra():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test?from=1&to=2&range=20&foo=1&range2=50&query1=somequery1&query2=somequery2"
     )
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
         "from_datetime": "1970-01-01T00:00:01+00:00",
         "range": 20,
```

### Comparing `ellar-0.3.4/tests/test_routing/test_form_schema.py` & `ellar-0.3.6/tests/test_routing/test_form_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import pytest
 
 from ellar.common import Form, post
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
 
 @mr.post("/form-schema")
 def form_params_schema(
     request: Request,
     filters: Filter = Form(..., alias="will_not_work_for_schema_with_many_field"),
 ):
     return filters.dict()
 
 
-test_module = TestClientFactory.create_test_module(routers=(mr,))
+test_module = Test.create_test_module(routers=(mr,))
+app = test_module.create_application()
 
 
 def test_request():
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.post("/form-schema", data={"from": "1", "to": "2", "range": "20"})
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
         "from_datetime": "1970-01-01T00:00:01+00:00",
         "range": 20,
     }
 
@@ -47,17 +48,15 @@
                 "ctx": {"enum_values": [20, 50, 200]},
             }
         ]
     }
 
 
 def test_schema():
-    document = serialize_object(
-        OpenAPIDocumentBuilder().build_document(test_module.app)
-    )
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     params = document["paths"]["/form-schema"]["post"]["requestBody"]
     assert params == {
         "content": {
             "application/x-www-form-urlencoded": {
                 "schema": {"$ref": "#/components/schemas/Filter"}
             }
         },
```

### Comparing `ellar-0.3.4/tests/test_routing/test_formparsers.py` & `ellar-0.3.6/tests/test_routing/test_formparsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import sys
 from typing import List, Union
 
 import pytest
 from starlette.formparsers import UploadFile as StarletteUploadFile
 
 from ellar.common import File, Form
-from ellar.core import TestClientFactory
 from ellar.core.datastructures import UploadFile
 from ellar.core.routing import ModuleRouter
+from ellar.testing import Test
 
 router = ModuleRouter("")
 
 
 class ForceMultipartDict(dict):
     def __bool__(self):
         return True
@@ -89,24 +89,24 @@
     return dict(
         file=_file,
         field0=field,
         field1=field_2,
     )
 
 
-tm = TestClientFactory.create_test_module(routers=(router,))
+tm = Test.create_test_module(routers=(router,))
 
 
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="requires python >= 3.7")
 def test_multipart_request_files(tmpdir):
     path = os.path.join(tmpdir, "test.txt")
     with open(path, "wb") as file:
         file.write(b"<file content>")
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     with open(path, "rb") as f:
         response = client.post("/", files={"test": f})
         assert response.json() == {
             "test": {
                 "filename": "test.txt",
                 "content": "<file content>",
                 "content_type": "text/plain",
@@ -115,15 +115,15 @@
 
 
 def test_multipart_request_files_with_content_type(tmpdir):
     path = os.path.join(tmpdir, "test.txt")
     with open(path, "wb") as file:
         file.write(b"<file content>")
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     with open(path, "rb") as f:
         response = client.post("/", files={"test": ("test.txt", f, "text/plain")})
         assert response.json() == {
             "test": {
                 "filename": "test.txt",
                 "content": "<file content>",
                 "content_type": "text/plain",
@@ -137,15 +137,15 @@
     with open(path1, "wb") as file:
         file.write(b"<file1 content>")
 
     path2 = os.path.join(tmpdir, "test2.txt")
     with open(path2, "wb") as file:
         file.write(b"<file2 content>")
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     with open(path1, "rb") as f1, open(path2, "rb") as f2:
         response = client.post(
             "/mixed", files={"test1": f1, "test2": ("test2.txt", f2, "text/plain")}
         )
         assert response.json() == {
             "test1": {
                 "filename": "test1.txt",
@@ -166,15 +166,15 @@
     with open(path1, "wb") as file:
         file.write(b"<file1 content>")
 
     path2 = os.path.join(tmpdir, "test2.txt")
     with open(path2, "wb") as file:
         file.write(b"<file2 content>")
 
-    client = tm.get_client()
+    client = tm.get_test_client()
     with open(path1, "rb") as f1, open(path2, "rb") as f2:
         response = client.post(
             "/multiple",
             data={"test1": "abc"},
             files=[("test1", f1), ("test1", ("test2.txt", f2, "text/plain"))],
         )
         assert response.json() == {
@@ -191,15 +191,15 @@
                     "content_type": "text/plain",
                 },
             ]
         }
 
 
 def test_multipart_request_mixed_files_and_data(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post(
         "/mixed-optional",
         data=(
             # data
             b"--a7f7ac8d4e2e437c877bb7b8d7cc549c\r\n"
             b'Content-Disposition: form-data; name="field0"\r\n\r\n'
             b"value0\r\n"
@@ -228,15 +228,15 @@
         },
         "field0": "value0",
         "field1": "value1",
     }
 
 
 def test_multipart_request_with_charset_for_filename(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post(
         "/mixed-optional",
         data=(
             # file
             b"--a7f7ac8d4e2e437c877bb7b8d7cc549c\r\n"
             b'Content-Disposition: form-data; name="file"; filename="\xe6\x96\x87\xe6\x9b\xb8.txt"\r\n'
             b"Content-Type: text/plain\r\n\r\n"
@@ -258,15 +258,15 @@
         },
         "field0": "",
         "field1": None,
     }
 
 
 def test_multipart_request_without_charset_for_filename(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post(
         "/mixed-optional",
         data=(
             # file
             b"--a7f7ac8d4e2e437c877bb7b8d7cc549c\r\n"
             b'Content-Disposition: form-data; name="file"; filename="\xe7\x94\xbb\xe5\x83\x8f.jpg"\r\n'
             b"Content-Type: image/jpeg\r\n\r\n"
@@ -287,15 +287,15 @@
         },
         "field0": "",
         "field1": None,
     }
 
 
 def test_multipart_request_with_encoded_value(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post(
         "/multiple",
         data=(
             b"--20b303e711c4ab8c443184ac833ab00f\r\n"
             b"Content-Disposition: form-data; "
             b'name="test1"\r\n\r\n'
             b"Transf\xc3\xa9rer\r\n"
@@ -308,30 +308,30 @@
             )
         },
     )
     assert response.json() == {"test1": ["Transférer"]}
 
 
 def test_urlencoded_request_data(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post("/multiple", data={"test1": "data"})
     assert response.json() == {"test1": ["data"]}
 
 
 def test_no_request_data(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post("/mixed-optional")
     assert response.json() == {"file": None, "field0": "", "field1": None}
 
 
 def test_urlencoded_percent_encoding(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post("/multiple", data={"test1": "da ta"})
     assert response.json() == {"test1": ["da ta"]}
 
 
 def test_multipart_multi_field_app_reads_body(tmpdir):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.post(
         "/multiple", data={"test1": "key pair"}, files=FORCE_MULTIPART
     )
     assert response.json() == {"test1": ["key pair"]}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_forms.py` & `ellar-0.3.6/tests/test_routing/test_forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ellar.common import Form
-from ellar.core import TestClientFactory
 from ellar.core.routing import ModuleRouter
+from ellar.testing import Test
 
 router = ModuleRouter("")
 
 
 @router.post("/form/python-list")
 def post_form_param_list(items: list = Form(...)):
     return items
@@ -16,16 +16,16 @@
 
 
 @router.post("/form/python-tuple")
 def post_form_param_tuple(items: tuple = Form(...)):
     return items
 
 
-tm = TestClientFactory.create_test_module(routers=(router,))
-client = tm.get_client()
+tm = Test.create_test_module(routers=(router,))
+client = tm.get_test_client()
 
 
 def test_python_list_param_as_form():
     response = client.post(
         "/form/python-list", data={"items": ["first", "second", "third"]}
     )
     assert response.status_code == 200, response.text
```

### Comparing `ellar-0.3.4/tests/test_routing/test_forms_from_non_typing_sequences.py` & `ellar-0.3.6/tests/test_routing/test_forms_from_non_typing_sequences.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ellar.common import Form
-from ellar.core import AppFactory, TestClient
+from ellar.core import AppFactory
 from ellar.core.routing import ModuleRouter
+from ellar.testing import TestClient
 
 mr = ModuleRouter("")
 
 
 @mr.post("/form/python-list")
 def post_form_param_list(items: list = Form(...)):
     return items
```

### Comparing `ellar-0.3.4/tests/test_routing/test_header_schema.py` & `ellar-0.3.6/tests/test_routing/test_header_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from ellar.common import Header, get
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
 
 @mr.get("/test/header")
@@ -26,19 +26,20 @@
     request: Request,
     filters: Filter = Header(...),
     data: Data = Header(...),
 ):
     return dict(filters=filters.dict(), data=data.dict())
 
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
 
 
 def test_header_request():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test/header",
         headers={"from": "1", "to": "2", "range": "20", "foo": "1", "range2": "50"},
     )
     assert response.status_code == 200
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
@@ -49,15 +50,15 @@
     response = client.get(
         "/test/header", headers={"from": "1", "to": "2", "range": "21"}
     )
     assert response.status_code == 422
 
 
 def test_request_mixed():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test-mixed/header",
         headers={
             "from": "1",
             "to": "2",
             "range": "20",
             "foo": "1",
@@ -79,15 +80,15 @@
     response = client.get(
         "/test-mixed/header", headers={"from": "1", "to": "2", "range": "21"}
     )
     assert response.status_code == 422
 
 
 def test_header_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     params = document["paths"]["/test/header"]["get"]["parameters"]
     assert params == [
         {
             "required": False,
             "schema": {"title": "To", "type": "string", "format": "date-time"},
             "name": "to",
             "in": "header",
```

### Comparing `ellar-0.3.4/tests/test_routing/test_invalid_path_param.py` & `ellar-0.3.6/tests/test_routing/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_routing/test_invalid_sequence_param.py` & `ellar-0.3.6/tests/test_routing/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_routing/test_multi_body_errors.py` & `ellar-0.3.6/tests/test_routing/test_multi_body_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from decimal import Decimal
 from typing import List
 
 from pydantic import BaseModel, condecimal
 
 from ellar.common import post
-from ellar.core import TestClientFactory
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
+app = tm.create_application()
 
 
 class Item2(BaseModel):
     name: str
     age: condecimal(gt=Decimal(0.0))  # type: ignore
 
 
 @post("/items/")
 def save_item_no_body(item: List[Item2]):
     return {"item": item}
 
 
-tm.app.router.append(save_item_no_body)
-client = tm.get_client()
+app.router.append(save_item_no_body)
+client = tm.get_test_client()
 
 
 openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/items/": {
@@ -143,15 +144,15 @@
             "type": "type_error.decimal",
         },
     ]
 }
 
 
 def test_openapi_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == openapi_schema
 
 
 def test_put_correct_body():
     response = client.post("/items/", json=[{"name": "Foo", "age": 5}])
     assert response.status_code == 200, response.text
     assert response.json() == {"item": [{"name": "Foo", "age": 5}]}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_multi_query_errors.py` & `ellar-0.3.6/tests/test_routing/test_multi_query_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import List
 
 from ellar.common import Query, get
-from ellar.core import TestClientFactory
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
+app = tm.create_application()
 
 
 @get("/items/")
 def read_items(q: List[int] = Query(None)):
     return {"q": q}
 
 
-tm.app.router.append(read_items)
-client = tm.get_client()
+app.router.append(read_items)
+client = tm.get_test_client()
 
 
 openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/items/": {
@@ -105,15 +106,15 @@
             "type": "type_error.integer",
         },
     ]
 }
 
 
 def test_openapi_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == openapi_schema
 
 
 def test_multi_query():
     response = client.get("/items/?q=5&q=6")
     assert response.status_code == 200, response.text
     assert response.json() == {"q": [5, 6]}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_path.py` & `ellar-0.3.6/tests/test_routing/test_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.core.testclient import TestClient
+from ellar.testing import TestClient
 
 from ..main import app
 
 client = TestClient(app)
 
 
 def test_text_get():
```

### Comparing `ellar-0.3.4/tests/test_routing/test_path_with_schema.py` & `ellar-0.3.6/tests/test_routing/test_path_with_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import pytest
 
 from ellar.common import Path, get
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
 
 @mr.get("/path-with-schema/{from}/{to}/{range}")
 def path_params_schema(
     request: Request,
     filters: Filter = Path(..., alias="will_not_work_for_schema_with_many_field"),
 ):
     return filters.dict()
 
 
-test_module = TestClientFactory.create_test_module(routers=(mr,))
+test_module = Test.create_test_module(routers=(mr,))
+app = test_module.create_application()
 
 
 def test_request():
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get("/path-with-schema/1/2/20")
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
         "from_datetime": "1970-01-01T00:00:01+00:00",
         "range": 20,
     }
 
@@ -44,17 +45,15 @@
                 "ctx": {"enum_values": [20, 50, 200]},
             }
         ]
     }
 
 
 def test_schema():
-    document = serialize_object(
-        OpenAPIDocumentBuilder().build_document(test_module.app)
-    )
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     params = document["paths"]["/path-with-schema/{from}/{to}/{range}"]["get"][
         "parameters"
     ]
     assert params == [
         {
             "required": True,
             "schema": {"title": "To", "type": "string", "format": "date-time"},
```

### Comparing `ellar-0.3.4/tests/test_routing/test_put_with_no_body_schema.py` & `ellar-0.3.6/tests/test_routing/test_put_with_no_body_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from ellar.common import put
-from ellar.core import TestClientFactory
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
-tm = TestClientFactory.create_test_module()
+tm = Test.create_test_module()
+app = tm.create_application()
 
 
 @put("/items/{item_id}")
 def save_item_no_body(item_id: str):
     return {"item_id": item_id}
 
 
-tm.app.router.append(save_item_no_body)
-client = tm.get_client()
+app.router.append(save_item_no_body)
+client = tm.get_test_client()
 
 
 openapi_schema = {
     "openapi": "3.0.2",
     "info": {"title": "Ellar API Docs", "version": "1.0.0"},
     "paths": {
         "/items/{item_id}": {
@@ -84,15 +85,15 @@
         }
     },
     "tags": [],
 }
 
 
 def test_openapi_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     assert document == openapi_schema
 
 
 def test_put_no_body():
     response = client.put("/items/foo")
     assert response.status_code == 200, response.text
     assert response.json() == {"item_id": "foo"}
```

### Comparing `ellar-0.3.4/tests/test_routing/test_query.py` & `ellar-0.3.6/tests/test_routing/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.core.testclient import TestClient
+from ellar.testing import TestClient
 
 from ..main import app
 
 client = TestClient(app)
 
 response_missing = {
     "detail": [
```

### Comparing `ellar-0.3.4/tests/test_routing/test_query_schema.py` & `ellar-0.3.6/tests/test_routing/test_query_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from ellar.common import Query, get
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.exceptions import ImproperConfiguration
 from ellar.core.routing import ModuleRouter
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.serializer import serialize_object
+from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
 
 @mr.get("/test")
@@ -28,32 +28,33 @@
     query2: int = 5,
     filters: Filter = Query(...),
     data: Data = Query(...),
 ):
     return dict(query1=query1, query2=query2, filters=filters.dict(), data=data.dict())
 
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
 
 
 def test_request():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get("/test?from=1&to=2&range=20&foo=1&range2=50")
     assert response.json() == {
         "to_datetime": "1970-01-01T00:00:02+00:00",
         "from_datetime": "1970-01-01T00:00:01+00:00",
         "range": 20,
     }
 
     response = client.get("/test?from=1&to=2&range=21")
     assert response.status_code == 422
 
 
 def test_request_mixed():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(
         "/test-mixed?from=1&to=2&range=20&foo=1&range2=50&query1=2&int=3&float=1.6"
     )
     assert response.json() == {
         "query1": 2,
         "query2": 5,
         "filters": {
@@ -79,15 +80,15 @@
     }
 
     response = client.get("/test-mixed?from=1&to=2")
     assert response.status_code == 422
 
 
 def test_schema():
-    document = serialize_object(OpenAPIDocumentBuilder().build_document(tm.app))
+    document = serialize_object(OpenAPIDocumentBuilder().build_document(app))
     params = document["paths"]["/test"]["get"]["parameters"]
     assert params == [
         {
             "required": False,
             "schema": {"title": "To", "type": "string", "format": "date-time"},
             "name": "to",
             "in": "query",
```

### Comparing `ellar-0.3.4/tests/test_routing/test_request.py` & `ellar-0.3.6/tests/test_routing/test_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from ellar.common import Cookie, Header
-from ellar.core import TestClientFactory
 from ellar.core.connection import Request
 from ellar.core.routing import ModuleRouter
+from ellar.testing import Test
 
 mr = ModuleRouter("")
 
 
 @mr.get("/headers1")
 def headers1(request: Request, user_agent: str = Header(...)):
     return user_agent
@@ -39,16 +39,16 @@
 
 
 @mr.get("/cookies2")
 def cookies2(request: Request, wpn: str = Cookie(..., alias="weapon")):
     return wpn
 
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
-client = tm.get_client()
+tm = Test.create_test_module(routers=(mr,))
+client = tm.get_test_client()
 
 
 @pytest.mark.parametrize(
     "path,expected_status,expected_response",
     [
         ("/headers1", 200, "Ellar"),
         ("/headers2", 200, "Ellar"),
```

### Comparing `ellar-0.3.4/tests/test_routing/test_route_endpoint_params.py` & `ellar-0.3.6/tests/test_routing/test_route_endpoint_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,25 @@
     HTTPConnection as StarletteHTTPConnection,
     Request as StarletteRequest,
 )
 from starlette.responses import Response as StarletteResponse
 from starlette.websockets import WebSocket as StarletteWebSocket
 
 from ellar.common import Context, Host, Http, Provide, Req, Res, Session, Ws
-from ellar.core import Config, ExecutionContext, TestClientFactory
+from ellar.core import Config, ExecutionContext
 from ellar.core.connection import (
     HTTPConnection as EllarHTTPConnection,
     Request as EllarRequest,
     WebSocket as EllarWebSocket,
 )
 from ellar.core.context import IExecutionContext
 from ellar.core.middleware import Middleware
 from ellar.core.middleware.sessions import SessionMiddleware
 from ellar.core.routing import ModuleRouter
+from ellar.testing import Test
 
 router = ModuleRouter()
 
 
 @router.get("/starlette-request")
 def get_requests(request: StarletteRequest, req=Req()):
     assert isinstance(request, EllarRequest)  # True
@@ -61,22 +62,22 @@
     assert isinstance(websocket, EllarWebSocket)
     await ws.accept()
     await ws.send_json(ws == websocket)
     await ws.close()
 
 
 SECRET_KEY = "ellar_cf303596-e51a-441a-ba67-5da42dbffb07"
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     routers=[router],
     config_module=dict(
         SECRET_KEY=SECRET_KEY,
         MIDDLEWARE=[Middleware(SessionMiddleware, secret_key=SECRET_KEY)],
     ),
 )
-client = tm.get_client()
+client = tm.get_test_client()
 
 
 def test_get_connections():
     response = client.get("/starlette-connection")
     assert response.status_code == 200
     assert response.json() is True
```

### Comparing `ellar-0.3.4/tests/test_schema.py` & `ellar-0.3.6/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_serializer.py` & `ellar-0.3.6/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_shortcuts.py` & `ellar-0.3.6/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_staticfiles.py` & `ellar-0.3.6/tests/test_staticfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import time
 
 import anyio
 import pytest
 from starlette.exceptions import HTTPException
 from starlette.routing import Mount
 
-from ellar.core import AppFactory, TestClient
+from ellar.core import AppFactory
 from ellar.core.staticfiles import StaticFiles
+from ellar.testing import TestClient
 
 
 def test_staticfiles(tmpdir):
     path = os.path.join(tmpdir, "example.txt")
     with open(path, "w") as file:
         file.write("<file content>")
```

### Comparing `ellar-0.3.4/tests/test_templating/test_module_templating.py` & `ellar-0.3.6/tests/test_templating/test_module_templating.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 import pytest
 
 from ellar.common import Module, template_filter, template_global
-from ellar.core import Config, TestClientFactory
+from ellar.core import Config
 from ellar.core.modules import ModuleBase, ModuleTemplateRef
 from ellar.di import EllarInjector
+from ellar.testing import Test
 
 
 @Module(template_folder="views")
 class SomeModule(ModuleBase):
     @template_global("dec_global")
     def double_global_dec(cls, n):
         return n * 2
@@ -36,19 +37,19 @@
         return n * 2
 
     @template_filter("dec_filter")
     def double_filter_dec(cls, n):
         return n * 2
 
 
-tm = TestClientFactory.create_test_module_from_module(module=SomeModule)
+tm = Test.create_test_module(modules=[SomeModule])
+app = tm.create_application()
 
 
 def test_template_globals_and_template_filters_computation():
-    app = tm.app
     app.install_module(SomeModule2)
     environment = app.jinja_environment
 
     for item in ["double_filter", "dec_filter", "double_filter_dec_2"]:
         assert item in environment.filters
 
     for item in ["double_global", "dec_global", "double_global_dec_2"]:
```

### Comparing `ellar-0.3.4/tests/test_templating/test_renderer.py` & `ellar-0.3.6/tests/test_templating/test_renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 from pathlib import Path
 
 from ellar.common import Controller, get, render
-from ellar.core import ControllerBase, TestClientFactory
+from ellar.core import ControllerBase
 from ellar.core.templating import (
     TemplateResponse,
     render_template,
     render_template_string,
 )
+from ellar.testing import Test
 
 BASEDIR = Path(__file__).resolve().parent.parent
 
 
 @Controller
 class EllarController(ControllerBase):
     @get("/index", response={200: TemplateResponse})
@@ -37,45 +38,45 @@
     @get("/index", response={200: TemplateResponse})
     @render("watever.html")
     def index(self):
         """Looks for ellar/index since use_mvc=True"""
         return {}
 
 
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     controllers=(EllarController,), base_directory=BASEDIR, template_folder="templates"
 )
 
 
 def test_render_template_string():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get("/ellar/another_index2?first_name=Eadwin&last_name=Eadwin")
     assert response.status_code == 200
     content = re.sub("\\s+", " ", response.text).strip()
     assert content == '"Hi Eadwin Eadwin!.\\nWelcome to Ellar Framework"'
 
 
 def test_render_template():
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get("/ellar/index")
     assert response.status_code == 200
     content = re.sub("\\s+", " ", response.text).strip()
     assert (
         content == '<!DOCTYPE html> <html lang="en"> '
         '<head> <meta charset="UTF-8"> <title>Index Page</title> </head> <body> </body> </html>'
     )
 
 
 def test_render_template_with_static_ref():
-    test_module = TestClientFactory.create_test_module(
+    test_module = Test.create_test_module(
         controllers=(TemplateWithStaticsController,),
         template_folder="templates",
         base_directory=Path(__file__).resolve().parent,
     )
-    client = test_module.get_client()
+    client = test_module.get_test_client()
     response = client.get("/template-static/index")
     assert response.status_code == 200
     content = re.sub("\\s+", " ", response.text).strip()
     assert (
         content
         == '<!DOCTYPE html> <head> <title>Welcome - Ellar ASGI Python Framework</title> <link rel="stylesheet" href="http://testserver/static/watever.txt"/> </head>'
     )
```

### Comparing `ellar-0.3.4/tests/test_versioning/operations.py` & `ellar-0.3.6/tests/test_versioning/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from ellar.common import Controller, ModuleRouter, get, version
+from ellar.common import Controller, ModuleRouter, Version, get
 
 mr = ModuleRouter("")
 
 
 @mr.get("/version")
 def default_version():
     return dict(version="default")
 
 
 @mr.get("/version")
-@version("1", 1)
+@Version("1", 1)
 def default_version_1():
     return dict(version="v1")
 
 
 @mr.get("/version")
-@version("2", 2)
+@Version("2", 2)
 def default_version_2():
     return dict(version="v2")
 
 
 @mr.get("/version")
-@version("3", 3)
+@Version("3", 3)
 def default_version_3():
     return dict(version="v3")
 
 
 mr_with_version = ModuleRouter("/with-version", version="1")
 
 
 @mr_with_version.get("/version")
 def default_version():
     return dict(version="v1 only")
 
 
 @mr_with_version.get("/version")
-@version("2", "3")
+@Version("2", "3")
 def default_version_1():
     return dict(version="v2 and v3 only")
 
 
 mr_with_version_list = ModuleRouter("/with-version-list", version=["1", "2"])
 
 
@@ -51,44 +51,46 @@
 @Controller("/individual")
 class ControllerIndividualVersioning:
     @get("/version")
     def default_version(self):
         return dict(version="default")
 
     @get("/version")
-    @version("1", 1)
+    @Version("1", 1)
     def default_version_1(self):
         return dict(version="v1")
 
     @get("/version")
-    @version("2", 2)
+    @Version("2", 2)
     def default_version_2(self):
         return dict(version="v2")
 
     @get("/version")
-    @version("3", 3)
+    @Version("3", 3)
     def default_version_3(self):
         return dict(version="v3")
 
 
-@Controller("/controller-versioning", version="1")
+@Controller("/controller-versioning")
+@Version("1")
 class ControllerVersioning:
     @get("/version")
     def default_version(self):
         return dict(version="default")
 
     @get("/version")
-    @version("2")
+    @Version("2")
     def default_version_2(self):
         return dict(version="v2")
 
 
-@Controller("/controller-versioning-list", version=["1", "2"])
+@Version("1", "2")
+@Controller("/controller-versioning-list")
 class ControllerListVersioning:
     @get("/version")
     def default_version(self):
         return dict(version="default")
 
     @get("/version")
-    @version("3")
+    @Version("3")
     def default_version_3(self):
         return dict(version="v3")
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_default_versioning.py` & `ellar-0.3.6/tests/test_versioning/test_default_versioning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import pytest
 
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import (
     ControllerIndividualVersioning,
     ControllerListVersioning,
     ControllerVersioning,
     mr,
 )
 
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     routers=(mr,),
     controllers=[
         ControllerVersioning,
         ControllerIndividualVersioning,
         ControllerListVersioning,
     ],
 )
-tm.app.enable_versioning(VERSIONING.NONE)
+app = tm.create_application()
+app.enable_versioning(VERSIONING.NONE)
 
 
 @pytest.mark.parametrize(
     "path, expected_result",
     [
         ("/version", dict(version="default")),
         ("/version?v=1", dict(version="default")),
         ("/version?v=2", dict(version="default")),
         ("/version?v=3", dict(version="default")),
     ],
 )
 def test_default_route_versioning_query(path, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
@@ -43,15 +44,15 @@
         ("/version", "", dict(version="default")),
         ("/version", "v=1", dict(version="default")),
         ("/version", "v=2", dict(version="default")),
         ("/version", "v=3", dict(version="default")),
     ],
 )
 def test_default_route_versioning_header(path, header, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, host, expected_result",
@@ -59,11 +60,11 @@
         ("/version", "testserver.org", dict(version="default")),
         ("/version", "v1.testserver.org", dict(version="default")),
         ("/version", "v2.testserver.org", dict(version="default")),
         ("/version", "v3.testserver.org", dict(version="default")),
     ],
 )
 def test_default_route_versioning_host(path, host, expected_result):
-    client = tm.get_client(base_url=f"http://{host}")
+    client = tm.get_test_client(base_url=f"http://{host}")
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_default_versioning_for_controllers.py` & `ellar-0.3.6/tests/test_versioning/test_default_versioning_for_controllers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
 
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import (
     ControllerIndividualVersioning,
     ControllerListVersioning,
     ControllerVersioning,
 )
 
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     controllers=[
         ControllerVersioning,
         ControllerIndividualVersioning,
         ControllerListVersioning,
     ]
 )
-
-tm.app.enable_versioning(VERSIONING.NONE)
+app = tm.create_application()
+app.enable_versioning(VERSIONING.NONE)
 
 
 @pytest.mark.parametrize(
     "path, expected_result",
     [
         ("/individual/version", dict(version="default")),
         ("/individual/version?v=1", dict(version="default")),
@@ -33,15 +33,15 @@
         ("/controller-versioning/version?v=3", dict(version="default")),
         ("/controller-versioning-list/version?v=1", dict(version="default")),
         ("/controller-versioning-list/version?v=2", dict(version="default")),
         ("/controller-versioning-list/version?v=3", dict(version="default")),
     ],
 )
 def test_default_route_versioning_query(path, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
@@ -57,15 +57,15 @@
         ("/controller-versioning-list/version", "", dict(version="default")),
         ("/controller-versioning-list/version", "v=1", dict(version="default")),
         ("/controller-versioning-list/version", "v=2", dict(version="default")),
         ("/controller-versioning-list/version", "v=3", dict(version="default")),
     ],
 )
 def test_default_route_versioning_header(path, header, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, host, expected_result",
@@ -109,11 +109,11 @@
             "/controller-versioning-list/version",
             "v3.testserver.org",
             dict(version="default"),
         ),
     ],
 )
 def test_default_route_versioning_host(path, host, expected_result):
-    client = tm.get_client(base_url=f"http://{host}")
+    client = tm.get_test_client(base_url=f"http://{host}")
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_header_versioning.py` & `ellar-0.3.6/tests/test_versioning/test_header_versioning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pytest
 
 from ellar.constants import NOT_SET
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import mr
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
-
-tm.app.enable_versioning(
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
+app.enable_versioning(
     VERSIONING.HEADER, version_parameter="v", header_parameter="accept"
 )
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
     [
         ("/version", "", dict(version="default")),
         ("/version", "v=1", dict(version="v1")),
         ("/version", "v=2", dict(version="v2")),
         ("/version", "v=3", dict(version="v3")),
     ],
 )
 def test_header_route_versioning(path, header, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, header, default, expected_result",
@@ -53,29 +53,29 @@
         ("/version", "v=2", NOT_SET, dict(version="v2")),
         ("/version", "v=3", NOT_SET, dict(version="v3")),
     ],
 )
 def test_header_route_versioning_with_default_version(
     path, header, default, expected_result
 ):
-    tm.app.enable_versioning(
+    app.enable_versioning(
         VERSIONING.HEADER,
         version_parameter="v",
         header_parameter="accept",
         default_version=default,
     )
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 def test_header_versioning_version_parameter():
-    tm.app.enable_versioning(VERSIONING.HEADER)
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER)
+    client = tm.get_test_client()
 
     response = client.get(
         "/version", headers={"accept": "application/json; v=4"}
     )  # version_parameter for query lookup is 'version'
     assert response.status_code == 200
     assert response.json() == dict(version="default")
 
@@ -94,24 +94,24 @@
         ({"accept": "application/json; v=4"}),
         ({"accept": "application/json; v=1.0"}),
         ({"accept": "application/json; v=2.0"}),
         ({"accept": "application/json; v=3.0"}),
     ],
 )
 def test_header_route_versioning_fails_for_float_versions(headers):
-    tm.app.enable_versioning(VERSIONING.HEADER, version_parameter="v")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER, version_parameter="v")
+    client = tm.get_test_client()
     response = client.get("/version", headers=headers)
     assert response.status_code == 406
     assert response.json() == {"detail": 'Invalid version in "accept" header.'}
 
 
 def test_header_route_versioning_with_different_header_key():
-    tm.app.enable_versioning(VERSIONING.HEADER, header_parameter="custom_parameter")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER, header_parameter="custom_parameter")
+    client = tm.get_test_client()
     response = client.get("/version", headers={"custom_parameter": "version=1;"})
     assert response.status_code == 200
     assert response.json() == dict(version="v1")
 
     response = client.get("/version", headers={"custom_parameter": "version=2;"})
     assert response.status_code == 200
     assert response.json() == dict(version="v2")
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_header_versioning_controller.py` & `ellar-0.3.6/tests/test_versioning/test_header_versioning_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pytest
 
 from ellar.constants import NOT_SET
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import (
     ControllerIndividualVersioning,
     ControllerListVersioning,
     ControllerVersioning,
     mr_with_version,
     mr_with_version_list,
 )
 
-tm = TestClientFactory.create_test_module(
+tm = Test.create_test_module(
     controllers=[
         ControllerVersioning,
         ControllerIndividualVersioning,
         ControllerListVersioning,
     ]
 )
-
-tm.app.enable_versioning(
+app = tm.create_application()
+app.enable_versioning(
     VERSIONING.HEADER, version_parameter="v", header_parameter="accept"
 )
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
     [
@@ -35,15 +35,15 @@
         ("/controller-versioning/version", "v=2", dict(version="v2")),
         ("/controller-versioning-list/version", "v=1", dict(version="default")),
         ("/controller-versioning-list/version", "v=2", dict(version="default")),
         ("/controller-versioning-list/version", "v=3", dict(version="v3")),
     ],
 )
 def test_header_route_versioning(path, header, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, header, default, expected_result",
@@ -69,21 +69,21 @@
         ("/individual/version", "v=2", NOT_SET, dict(version="v2")),
         ("/individual/version", "v=3", NOT_SET, dict(version="v3")),
     ],
 )
 def test_header_route_versioning_with_default_version(
     path, header, default, expected_result
 ):
-    tm.app.enable_versioning(
+    app.enable_versioning(
         VERSIONING.HEADER,
         version_parameter="v",
         header_parameter="accept",
         default_version=default,
     )
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result, status",
@@ -116,16 +116,16 @@
             "version=1",
             dict(version="default"),
             200,
         ),
     ],
 )
 def test_header_versioning_version_parameter(path, header, expected_result, status):
-    tm.app.enable_versioning(VERSIONING.HEADER)
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER)
+    client = tm.get_test_client()
 
     response = client.get(
         path, headers={"accept": f"application/json; {header}"}
     )  # version_parameter for query lookup is 'version'
     assert response.status_code == status
     assert response.json() == expected_result
 
@@ -136,16 +136,16 @@
         ({"accept": "application/json; v=4"}),
         ({"accept": "application/json; v=1.0"}),
         ({"accept": "application/json; v=2.0"}),
         ({"accept": "application/json; v=3.0"}),
     ],
 )
 def test_header_route_versioning_fails_for_float_versions(headers):
-    tm.app.enable_versioning(VERSIONING.HEADER, version_parameter="v")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER, version_parameter="v")
+    client = tm.get_test_client()
     response = client.get("/individual/version", headers=headers)
     assert response.status_code == 406
     assert response.json() == {"detail": 'Invalid version in "accept" header.'}
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
@@ -179,25 +179,24 @@
             dict(version="v3"),
         ),
     ],
 )
 def test_header_route_versioning_with_different_header_key(
     path, header, expected_result
 ):
-    tm.app.enable_versioning(VERSIONING.HEADER, header_parameter="custom_parameter")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.HEADER, header_parameter="custom_parameter")
+    client = tm.get_test_client()
     response = client.get(path, headers=header)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
-new_tm = TestClientFactory.create_test_module(
-    routers=(mr_with_version, mr_with_version_list)
-)
-new_tm.app.enable_versioning(
+new_tm = Test.create_test_module(routers=(mr_with_version, mr_with_version_list))
+new_app = new_tm.create_application()
+new_app.enable_versioning(
     VERSIONING.HEADER, version_parameter="v", header_parameter="accept"
 )
 
 
 @pytest.mark.parametrize(
     "path, header, expected_result",
     [
@@ -207,11 +206,11 @@
         ("/with-version-list/version", "v=1", dict(version="v1 and v2")),
         ("/with-version-list/version", "v=2", dict(version="v1 and v2")),
     ],
 )
 def test_header_route_versioning_for_module_router_versions_and_version_list(
     path, header, expected_result
 ):
-    client = new_tm.get_client()
+    client = new_tm.get_test_client()
     response = client.get(path, headers={"accept": f"application/json; {header}"})
     assert response.status_code == 200
     assert response.json() == expected_result
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_host_versioning.py` & `ellar-0.3.6/tests/test_versioning/test_host_versioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pytest
 
 from ellar.constants import NOT_SET
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import mr
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
-
-tm.app.enable_versioning(VERSIONING.HOST, version_parameter="v")
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
+app.enable_versioning(VERSIONING.HOST, version_parameter="v")
 
 
 @pytest.mark.parametrize(
     "path, host, expected_result",
     [
         ("/version", "testserver.org", dict(version="default")),
         ("/version", "v1.testserver.org", dict(version="v1")),
         ("/version", "v2.testserver.org", dict(version="v2")),
         ("/version", "v3.testserver.org", dict(version="v3")),
     ],
 )
 def test_host_route_versioning(path, host, expected_result):
-    client = tm.get_client(base_url=f"http://{host}")
+    client = tm.get_test_client(base_url=f"http://{host}")
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, host, default, expected_result",
@@ -51,16 +51,16 @@
         ("/version", "v2.testserver.org", NOT_SET, dict(version="v2")),
         ("/version", "v3.testserver.org", NOT_SET, dict(version="v3")),
     ],
 )
 def test_host_route_versioning_with_default_version(
     path, host, default, expected_result
 ):
-    tm.app.enable_versioning(VERSIONING.HOST, default_version=default)
-    client = tm.get_client(base_url=f"http://{host}")
+    app.enable_versioning(VERSIONING.HOST, default_version=default)
+    client = tm.get_test_client(base_url=f"http://{host}")
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "host, version_parameter",
@@ -69,16 +69,16 @@
         ("http://b2.testserver.org", "v"),
         ("http://b3.testserver.org", "v"),
         ("http://b4.testserver.org", "v"),
         ("http://b4.testserver.org", "b"),
     ],
 )
 def test_host_route_versioning_not_found(host, version_parameter):
-    tm.app.enable_versioning(VERSIONING.HOST, version_parameter=version_parameter)
-    client = tm.get_client(base_url=host)
+    app.enable_versioning(VERSIONING.HOST, version_parameter=version_parameter)
+    client = tm.get_test_client(base_url=host)
 
     response = client.get("/version")
     assert response.status_code == 404
     assert response.json() == {"detail": "Invalid version in hostname."}
 
 
 @pytest.mark.parametrize(
@@ -88,13 +88,13 @@
         ("http://b2.testserver.org", "b", dict(version="v2")),
         ("http://b3.testserver.org", "b", dict(version="v3")),
     ],
 )
 def test_host_route_versioning_different_version_parameter(
     host, version_parameter, expected_result
 ):
-    tm.app.enable_versioning(VERSIONING.HOST, version_parameter=version_parameter)
-    client = tm.get_client(base_url=host)
+    app.enable_versioning(VERSIONING.HOST, version_parameter=version_parameter)
+    client = tm.get_test_client(base_url=host)
 
     response = client.get("/version")
     assert response.status_code == 200
     assert response.json() == expected_result
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_query_versioning.py` & `ellar-0.3.6/tests/test_versioning/test_query_versioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pytest
 
 from ellar.constants import NOT_SET
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING
+from ellar.core.versioning import VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import mr
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
-
-tm.app.enable_versioning(VERSIONING.QUERY, version_parameter="v")
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
+app.enable_versioning(VERSIONING.QUERY, version_parameter="v")
 
 
 @pytest.mark.parametrize(
     "path, expected_result",
     [
         ("/version", dict(version="default")),
         ("/version?v=1", dict(version="v1")),
         ("/version?v=2", dict(version="v2")),
         ("/version?v=3", dict(version="v3")),
     ],
 )
 def test_query_route_versioning(path, expected_result):
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, default, expected_result",
@@ -49,26 +49,26 @@
         ("/version", NOT_SET, dict(version="default")),
         ("/version?v=1", NOT_SET, dict(version="v1")),
         ("/version?v=2", NOT_SET, dict(version="v2")),
         ("/version?v=3", NOT_SET, dict(version="v3")),
     ],
 )
 def test_query_route_versioning_with_default_version(path, default, expected_result):
-    tm.app.enable_versioning(
+    app.enable_versioning(
         VERSIONING.QUERY, version_parameter="v", default_version=default
     )
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 def test_query_versioning_version_parameter():
-    tm.app.enable_versioning(VERSIONING.QUERY)
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.QUERY)
+    client = tm.get_test_client()
 
     response = client.get(
         "/version?v=4"
     )  # version_parameter for query lookup is 'version'
     assert response.status_code == 200
     assert response.json() == dict(version="default")
 
@@ -87,13 +87,13 @@
         "/version?v=4",
         "/version?v=1.0",
         "/version?v=2.0",
         "/version?v=3.0",
     ],
 )
 def test_query_route_versioning_not_found(path):
-    tm.app.enable_versioning(VERSIONING.QUERY, version_parameter="v")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.QUERY, version_parameter="v")
+    client = tm.get_test_client()
 
     response = client.get(path)
     assert response.status_code == 404
     assert response.json() == {"detail": "Invalid version in query parameter."}
```

### Comparing `ellar-0.3.4/tests/test_versioning/test_url_versioning.py` & `ellar-0.3.6/tests/test_versioning/test_url_versioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 from ellar.constants import NOT_SET
-from ellar.core import TestClientFactory
-from ellar.core.versioning import VERSIONING, UrlPathAPIVersioning
+from ellar.core.versioning import UrlPathAPIVersioning, VersioningSchemes as VERSIONING
+from ellar.testing import Test
 
 from .operations import mr
 
-tm = TestClientFactory.create_test_module(routers=(mr,))
-
-tm.app.enable_versioning(VERSIONING.URL, version_parameter="v")
+tm = Test.create_test_module(routers=(mr,))
+app = tm.create_application()
+app.enable_versioning(VERSIONING.URL, version_parameter="v")
 
 
 @pytest.mark.parametrize(
     "path, expected_result",
     [
         ("/version", dict(version="default")),
         ("/v1/version", dict(version="v1")),
@@ -20,16 +20,16 @@
         ("/v3/version", dict(version="v3")),
         ("/1/version", dict(version="v1")),
         ("/2/version", dict(version="v2")),
         ("/3/version", dict(version="v3")),
     ],
 )
 def test_url_route_versioning(path, expected_result):
-    assert isinstance(tm.app.versioning_scheme, UrlPathAPIVersioning)
-    client = tm.get_client()
+    assert isinstance(app.versioning_scheme, UrlPathAPIVersioning)
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path, default, expected_result",
@@ -53,19 +53,19 @@
         ("/version", NOT_SET, dict(version="default")),
         ("/v1/version", NOT_SET, dict(version="v1")),
         ("/v2/version", NOT_SET, dict(version="v2")),
         ("/v3/version", NOT_SET, dict(version="v3")),
     ],
 )
 def test_url_route_versioning_with_default_version(path, default, expected_result):
-    tm.app.enable_versioning(
+    app.enable_versioning(
         VERSIONING.URL,
         default_version=default,
     )
-    client = tm.get_client()
+    client = tm.get_test_client()
     response = client.get(path)
     assert response.status_code == 200
     assert response.json() == expected_result
 
 
 @pytest.mark.parametrize(
     "path",
@@ -76,13 +76,13 @@
         "/v3.0/version",
         "/1.0/version",
         "/2.0/version",
         "/3.0/version",
     ],
 )
 def test_url_route_versioning_not_found(path):
-    tm.app.enable_versioning(VERSIONING.URL, version_parameter="v")
-    client = tm.get_client()
+    app.enable_versioning(VERSIONING.URL, version_parameter="v")
+    client = tm.get_test_client()
 
     response = client.get(path)
     assert response.status_code == 404
     assert response.json() == {"detail": "Invalid version in URL path."}
```

### Comparing `ellar-0.3.4/tests/test_websocket.py` & `ellar-0.3.6/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.4/tests/test_websocket_handler.py` & `ellar-0.3.6/tests/test_websocket_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 from starlette.websockets import WebSocket, WebSocketState
 
 from ellar.common import Controller, ModuleRouter, WsBody, ws_route
-from ellar.core import TestClientFactory
+from ellar.constants import CONTROLLER_OPERATION_HANDLER_KEY
 from ellar.core.exceptions import ImproperConfiguration
+from ellar.reflect import reflect
+from ellar.testing import Test
 
 from .schema import Item
 
 router = ModuleRouter("/router")
 
 
 @router.ws_route("/ws-with-handler", use_extra_handler=True)
@@ -15,20 +17,20 @@
     websocket: WebSocket, query: str, data: Item = WsBody()
 ):
     assert query == "my-query"
     await websocket.send_json(data.dict())
     await websocket.close()
 
 
-@websocket_with_handler.connect
+@router.ws_route.connect(websocket_with_handler)
 async def websocket_with_handler_connect(websocket: WebSocket):
     await websocket.accept()
 
 
-@websocket_with_handler.disconnect
+@router.ws_route.disconnect(websocket_with_handler)
 async def websocket_with_handler_connect(websocket: WebSocket, code: int):
     # await websocket.close(code=code)
     assert websocket.client_state == WebSocketState.DISCONNECTED
 
 
 @router.ws_route("/ws")
 async def websocket_without_handler(websocket: WebSocket, query: str):
@@ -45,36 +47,34 @@
     async def websocket_with_handler_c(
         self, websocket: WebSocket, query: str, data: Item = WsBody()
     ):
         assert query == "my-query"
         await websocket.send_json(data.dict())
         await websocket.close()
 
-    @websocket_with_handler_c.connect
+    @ws_route.connect(websocket_with_handler_c)
     async def websocket_with_handler_connect(self, websocket: WebSocket):
         await websocket.accept()
 
-    @websocket_with_handler_c.disconnect
+    @ws_route.disconnect(websocket_with_handler_c)
     async def websocket_with_handler_connect(self, websocket: WebSocket, code: int):
         # await websocket.close(code=code)
         assert websocket.client_state == WebSocketState.DISCONNECTED
 
     @ws_route("/ws")
     async def websocket_without_handler_c(self, websocket: WebSocket, query: str):
         assert query == "my-query"
         await websocket.accept()
         message = await websocket.receive_text()
         await websocket.send_json({"message": f"Thanks. {message}"})
         await websocket.close()
 
 
-tm = TestClientFactory.create_test_module(
-    routers=[router], controllers=(WebsocketController,)
-)
-client = tm.get_client()
+tm = Test.create_test_module(routers=[router], controllers=(WebsocketController,))
+client = tm.get_test_client()
 
 
 @pytest.mark.parametrize("prefix", ["/router", "/controller"])
 def test_websocket_with_handler_works(prefix):
     with client.websocket_connect(
         f"{prefix}/ws-with-handler?query=my-query"
     ) as session:
@@ -155,36 +155,32 @@
 def test_websocket_endpoint_on_connect():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True)
         async def ws(self, websocket: WebSocket):
             pass
 
-        @ws.connect
+        @ws_route.connect(ws)
         async def on_connect(self, websocket):
             assert websocket["subprotocols"] == ["soap", "wamp"]
             await websocket.accept(subprotocol="wamp")
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
     with _client.websocket_connect("/ws/", subprotocols=["soap", "wamp"]) as websocket:
         assert websocket.accepted_subprotocol == "wamp"
 
 
 def test_websocket_endpoint_on_receive_bytes():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding="bytes")
         async def ws(self, websocket: WebSocket, data: bytes = WsBody()):
             await websocket.send_bytes(b"Message bytes was: " + data)
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_bytes(b"Hello, world!")
         _bytes = websocket.receive_bytes()
         assert _bytes == b"Message bytes was: Hello, world!"
 
     with pytest.raises(RuntimeError):
         with _client.websocket_connect("/ws/") as websocket:
@@ -194,17 +190,15 @@
 def test_websocket_endpoint_on_receive_json():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding="json")
         async def ws(self, websocket: WebSocket, data=WsBody()):
             await websocket.send_json({"message": data})
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
 
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_json({"hello": "world"})
         data = websocket.receive_json()
         assert data == {"message": {"hello": "world"}}
 
     with pytest.raises(RuntimeError):
@@ -215,34 +209,30 @@
 def test_websocket_endpoint_on_receive_json_binary():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding="json")
         async def ws(self, websocket: WebSocket, data=WsBody()):
             await websocket.send_json({"message": data}, mode="binary")
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
 
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_json({"hello": "world"}, mode="binary")
         data = websocket.receive_json(mode="binary")
         assert data == {"message": {"hello": "world"}}
 
 
 def test_websocket_endpoint_on_receive_text():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding="text")
         async def ws(self, websocket: WebSocket, data: str = WsBody()):
             await websocket.send_text(f"Message text was: {data}")
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
 
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_text("Hello, world!")
         _text = websocket.receive_text()
         assert _text == "Message text was: Hello, world!"
 
     with pytest.raises(RuntimeError):
@@ -253,36 +243,68 @@
 def test_websocket_endpoint_on_default():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding=None)
         async def ws(self, websocket: WebSocket, data: str = WsBody()):
             await websocket.send_text(f"Message text was: {data}")
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
 
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_text("Hello, world!")
         _text = websocket.receive_text()
         assert _text == "Message text was: Hello, world!"
 
 
 def test_websocket_endpoint_on_disconnect():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True, encoding=None)
         async def ws(self, websocket: WebSocket, data: str = WsBody()):
             await websocket.send_text(f"Message text was: {data}")
 
-        @ws.disconnect
+        @ws_route.disconnect(ws)
         async def on_disconnect(self, websocket: WebSocket, close_code):
             assert close_code == 1001
             await websocket.close(code=close_code)
 
-    _client = TestClientFactory.create_test_module(
-        controllers=(WebSocketSample,)
-    ).get_client()
+    _client = Test.create_test_module(controllers=(WebSocketSample,)).get_test_client()
 
     with _client.websocket_connect("/ws/") as websocket:
         websocket.send_text("Hello, world!")
         websocket.close(code=1001)
+
+
+def test_ws_route_connect_raise_exception_for_invalid_type():
+    with pytest.raises(
+        Exception,
+        match="Invalid type. Please make sure you passed the websocket handler.",
+    ):
+
+        @router.ws_route.connect(ModuleRouter)
+        def some_example_connect():
+            pass
+
+
+def test_ws_route_connect_raise_exception_for_invalid_operation():
+    with pytest.raises(
+        Exception,
+        match="Invalid type. Please make sure you passed the websocket handler.",
+    ):
+
+        @router.ws_route.connect(websocket_with_handler_connect)
+        def some_example_connect():
+            pass
+
+
+def test_add_websocket_handler_raise_exception_for_wrong_handler_name():
+    websocket_operation = reflect.get_metadata(
+        CONTROLLER_OPERATION_HANDLER_KEY, websocket_with_handler
+    )
+    with pytest.raises(Exception) as ex:
+        websocket_operation.add_websocket_handler(
+            handler_name="mycustomname", handler=websocket_with_handler_connect
+        )
+    assert (
+        str(ex.value)
+        == "Invalid Handler Name. Handler Name must be in ['encoding', 'on_receive', 'on_connect', 'on_disconnect']"
+    )
```

### Comparing `ellar-0.3.4/PKG-INFO` & `ellar-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 656c 6c61  : 2.1.Name: ella
-00000020: 720a 5665 7273 696f 6e3a 2030 2e33 2e34  r.Version: 0.3.4
+00000020: 720a 5665 7273 696f 6e3a 2030 2e33 2e36  r.Version: 0.3.6
 00000030: 0a53 756d 6d61 7279 3a20 456c 6c61 7220  .Summary: Ellar 
 00000040: 2d20 5079 7468 6f6e 2041 5347 4920 7765  - Python ASGI we
 00000050: 6220 6672 616d 6577 6f72 6b20 666f 7220  b framework for 
 00000060: 6275 696c 6469 6e67 2066 6173 742c 2065  building fast, e
 00000070: 6666 6963 6965 6e74 2061 6e64 2073 6361  fficient and sca
 00000080: 6c61 626c 6520 5245 5354 4150 4973 2061  lable RESTAPIs a
 00000090: 6e64 2073 6572 7665 722d 7369 6465 2061  nd server-side a
@@ -84,29 +84,29 @@
 00000530: 5450 203a 3a20 4854 5450 2053 6572 7665  TP :: HTTP Serve
 00000540: 7273 0a43 6c61 7373 6966 6965 723a 2054  rs.Classifier: T
 00000550: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
 00000560: 203a 3a20 5757 572f 4854 5450 0a52 6571   :: WWW/HTTP.Req
 00000570: 7569 7265 732d 4469 7374 3a20 696e 6a65  uires-Dist: inje
 00000580: 6374 6f72 203d 3d20 302e 3230 2e31 0a52  ctor == 0.20.1.R
 00000590: 6571 7569 7265 732d 4469 7374 3a20 7374  equires-Dist: st
-000005a0: 6172 6c65 7474 6520 3d3d 2030 2e32 332e  arlette == 0.23.
+000005a0: 6172 6c65 7474 6520 3d3d 2030 2e32 362e  arlette == 0.26.
 000005b0: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
 000005c0: 2070 7964 616e 7469 6320 3e3d 312e 362e   pydantic >=1.6.
 000005d0: 322c 213d 312e 372c 213d 312e 372e 312c  2,!=1.7,!=1.7.1,
 000005e0: 213d 312e 372e 322c 213d 312e 372e 332c  !=1.7.2,!=1.7.3,
 000005f0: 213d 312e 382c 213d 312e 382e 312c 3c32  !=1.8,!=1.8.1,<2
 00000600: 2e30 2e30 0a52 6571 7569 7265 732d 4469  .0.0.Requires-Di
 00000610: 7374 3a20 6a69 6e6a 6132 0a52 6571 7569  st: jinja2.Requi
 00000620: 7265 732d 4469 7374 3a20 7479 7065 7220  res-Dist: typer 
 00000630: 3e3d 302e 362e 312c 3c30 2e38 2e30 0a52  >=0.6.1,<0.8.0.R
 00000640: 6571 7569 7265 732d 4469 7374 3a20 6874  equires-Dist: ht
 00000650: 7470 7820 3e3d 2030 2e32 322e 300a 5265  tpx >= 0.22.0.Re
 00000660: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
 00000670: 686f 6e2d 6d75 6c74 6970 6172 7420 3e3d  hon-multipart >=
-00000680: 302e 302e 352c 3c30 2e30 2e36 203b 2065  0.0.5,<0.0.6 ; e
+00000680: 302e 302e 352c 3c30 2e30 2e37 203b 2065  0.0.5,<0.0.7 ; e
 00000690: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
 000006a0: 7175 6972 6573 2d44 6973 743a 2069 7473  quires-Dist: its
 000006b0: 6461 6e67 6572 6f75 7320 3e3d 312e 312e  dangerous >=1.1.
 000006c0: 302c 3c33 2e30 2e30 203b 2065 7874 7261  0,<3.0.0 ; extra
 000006d0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
 000006e0: 6573 2d44 6973 743a 2070 7979 616d 6c20  es-Dist: pyyaml 
 000006f0: 3e3d 352e 332e 312c 3c37 2e30 2e30 203b  >=5.3.1,<7.0.0 ;
@@ -211,15 +211,15 @@
 00000d20: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
 00000d30: 4469 7374 3a20 6169 6f6d 6361 6368 6520  Dist: aiomcache 
 00000d40: 3b20 6578 7472 6120 3d3d 2022 7465 7374  ; extra == "test
 00000d50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
 00000d60: 2072 6564 6973 203b 2065 7874 7261 203d   redis ; extra =
 00000d70: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
 00000d80: 732d 4469 7374 3a20 7479 7065 732d 756a  s-Dist: types-uj
-00000d90: 736f 6e20 3d3d 352e 372e 302e 3020 3b20  son ==5.7.0.0 ; 
+00000d90: 736f 6e20 3d3d 352e 372e 302e 3120 3b20  son ==5.7.0.1 ; 
 00000da0: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
 00000db0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
 00000dc0: 7970 6573 2d6f 726a 736f 6e20 3d3d 332e  ypes-orjson ==3.
 00000dd0: 362e 3220 3b20 6578 7472 6120 3d3d 2022  6.2 ; extra == "
 00000de0: 7465 7374 220a 5265 7175 6972 6573 2d44  test".Requires-D
 00000df0: 6973 743a 2074 7970 6573 2d64 6174 6163  ist: types-datac
 00000e00: 6c61 7373 6573 203d 3d30 2e36 2e36 203b  lasses ==0.6.6 ;
@@ -304,558 +304,627 @@
 000012f0: 7470 733a 2f2f 7777 772e 7374 6172 6c65  tps://www.starle
 00001300: 7474 652e 696f 2f29 2c20 6120 6c69 6768  tte.io/), a ligh
 00001310: 7477 6569 6768 7420 4153 4749 2066 7261  tweight ASGI fra
 00001320: 6d65 776f 726b 2f74 6f6f 6c6b 6974 2077  mework/toolkit w
 00001330: 656c 6c2d 7375 6974 6564 2066 6f72 2064  ell-suited for d
 00001340: 6576 656c 6f70 696e 6720 6173 796e 6368  eveloping asynch
 00001350: 726f 6e6f 7573 2077 6562 2073 6572 7669  ronous web servi
-00001360: 6365 7320 696e 2050 7974 686f 6e2e 200a  ces in Python. .
-00001370: 5768 696c 6520 456c 6c61 7220 7072 6f76  While Ellar prov
-00001380: 6964 6573 2061 2068 6967 6820 6c65 7665  ides a high leve
-00001390: 6c20 6f66 2061 6273 7472 6163 7469 6f6e  l of abstraction
-000013a0: 206f 6e20 746f 7020 6f66 2053 7461 726c   on top of Starl
-000013b0: 6574 7465 2c20 6974 2073 7469 6c6c 2069  ette, it still i
-000013c0: 6e63 6f72 706f 7261 7465 7320 736f 6d65  ncorporates some
-000013d0: 206f 6620 6974 7320 6665 6174 7572 6573   of its features
-000013e0: 2c20 6173 2077 656c 6c20 6173 2074 686f  , as well as tho
-000013f0: 7365 206f 6620 4661 7374 4150 492e 200a  se of FastAPI. .
-00001400: 4966 2079 6f75 2061 7265 2066 616d 696c  If you are famil
-00001410: 6961 7220 7769 7468 2074 6865 7365 2066  iar with these f
-00001420: 7261 6d65 776f 726b 732c 2079 6f75 2077  rameworks, you w
-00001430: 696c 6c20 6669 6e64 2069 7420 6561 7379  ill find it easy
-00001440: 2074 6f20 756e 6465 7273 7461 6e64 2061   to understand a
-00001450: 6e64 2075 7365 2045 6c6c 6172 2e0a 0a23  nd use Ellar...#
-00001460: 2320 4465 7065 6e64 656e 6369 6573 0a2d  # Dependencies.-
-00001470: 2050 7974 686f 6e20 3e3d 2033 2e37 0a2d   Python >= 3.7.-
-00001480: 2053 7461 726c 6574 7465 0a2d 2049 6e6a   Starlette.- Inj
-00001490: 6563 746f 720a 2d20 5079 6461 6e74 6963  ector.- Pydantic
-000014a0: 0a0a 2323 2046 6561 7475 7265 7320 5375  ..## Features Su
-000014b0: 6d6d 6172 790a 2d20 6050 7964 616e 7469  mmary.- `Pydanti
-000014c0: 6320 696e 7465 6772 6174 696f 6e60 0a2d  c integration`.-
-000014d0: 2060 4465 7065 6e64 656e 6379 2049 6e6a   `Dependency Inj
-000014e0: 6563 7469 6f6e 2028 4449 2960 0a2d 2060  ection (DI)`.- `
-000014f0: 5465 6d70 6c61 7469 6e67 2077 6974 6820  Templating with 
-00001500: 4a69 6e6a 6132 600a 2d20 604f 7065 6e41  Jinja2`.- `OpenA
-00001510: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
-00001520: 2028 5377 6167 6765 7220 616e 6420 5265   (Swagger and Re
-00001530: 446f 6329 600a 2d20 6043 6f6e 7472 6f6c  Doc)`.- `Control
-00001540: 6c65 7220 284d 5643 2960 0a2d 2060 4775  ler (MVC)`.- `Gu
-00001550: 6172 6473 2028 6175 7468 656e 7469 6361  ards (authentica
-00001560: 7469 6f6e 732c 2072 6f6c 6573 2061 6e64  tions, roles and
-00001570: 2070 6572 6d69 7373 696f 6e73 2960 0a2d   permissions)`.-
-00001580: 2060 4d6f 6475 6c61 7269 7a61 7469 6f6e   `Modularization
-00001590: 2028 6567 3a20 666c 6173 6b20 626c 7565   (eg: flask blue
-000015a0: 7072 696e 7429 600a 2d20 6057 6562 736f  print)`.- `Webso
-000015b0: 636b 6574 2073 7570 706f 7274 600a 2d20  cket support`.- 
-000015c0: 6053 6573 7369 6f6e 2061 6e64 2043 6f6f  `Session and Coo
-000015d0: 6b69 6520 7375 7070 6f72 7460 0a2d 2060  kie support`.- `
-000015e0: 434f 5253 2c20 475a 6970 2c20 5374 6174  CORS, GZip, Stat
-000015f0: 6963 2046 696c 6573 2c20 5374 7265 616d  ic Files, Stream
-00001600: 696e 6720 7265 7370 6f6e 7365 7360 0a0a  ing responses`..
-00001610: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00001620: 2323 2320 506f 6574 7279 2049 6e73 7461  ### Poetry Insta
-00001630: 6c6c 6174 696f 6e0a 466f 7220 5b50 6f65  llation.For [Poe
-00001640: 7472 795d 2868 7474 7073 3a2f 2f70 7974  try](https://pyt
-00001650: 686f 6e2d 706f 6574 7279 2e6f 7267 2f29  hon-poetry.org/)
-00001660: 2075 7361 6765 730a 0a60 6060 7368 656c   usages..```shel
-00001670: 6c0a 706f 6574 7279 2061 6464 2065 6c6c  l.poetry add ell
-00001680: 6172 2d63 6c69 0a60 6060 0a0a 2323 2320  ar-cli.```..### 
-00001690: 5069 7020 496e 7374 616c 6c61 7469 6f6e  Pip Installation
-000016a0: 0a46 6f72 206e 6f72 6d61 6c20 7069 7020  .For normal pip 
-000016b0: 696e 7374 616c 6c61 7469 6f6e 0a60 6060  installation.```
-000016c0: 7368 656c 6c0a 7069 7020 696e 7374 616c  shell.pip instal
-000016d0: 6c20 656c 6c61 722d 636c 690a 6060 600a  l ellar-cli.```.
-000016e0: 0a23 2320 4372 6561 7465 2061 2070 726f  .## Create a pro
-000016f0: 6a65 6374 0a54 6f20 6372 6561 7465 2061  ject.To create a
-00001700: 6e20 656c 6c61 7220 7072 6f6a 6563 742c  n ellar project,
-00001710: 2079 6f75 206e 6565 6420 746f 2068 6176   you need to hav
-00001720: 6520 6120 6070 7970 726f 6a65 6374 2e74  e a `pyproject.t
-00001730: 6f6d 6c60 2061 7661 696c 6162 6c65 206f  oml` available o
-00001740: 6e20 796f 7572 2072 6f6f 7420 6469 7265  n your root dire
-00001750: 6374 6f72 792e 0a54 6869 7320 6973 206e  ctory..This is n
-00001760: 6563 6573 7361 7279 2066 6f72 2065 6c6c  ecessary for ell
-00001770: 6172 2074 6f20 7374 6f72 6520 736f 6d65  ar to store some
-00001780: 2060 6d65 7461 6461 7461 6020 6162 6f75   `metadata` abou
-00001790: 7420 796f 7572 2070 726f 6a65 6374 2e20  t your project. 
-000017a0: 0a0a 2323 2320 4372 6561 7465 2061 2070  ..### Create a p
-000017b0: 726f 6a65 6374 0a46 6f72 2050 6970 2055  roject.For Pip U
-000017c0: 7365 7273 2c20 796f 7520 6e65 6564 2074  sers, you need t
-000017d0: 6f20 6372 6561 7465 2060 7079 7072 6f6a  o create `pyproj
-000017e0: 6563 742e 746f 6d6c 6020 6669 6c65 0a60  ect.toml` file.`
-000017f0: 6060 7368 656c 6c0a 656c 6c61 7220 6e65  ``shell.ellar ne
-00001800: 7720 6361 7273 6974 650a 6060 600a 4966  w carsite.```.If
-00001810: 2079 6f75 2061 7265 2075 7369 6e67 2060   you are using `
-00001820: 506f 6574 7279 602c 2061 7420 796f 7572  Poetry`, at your
-00001830: 2070 726f 6a65 6374 2072 6f6f 7420 6469   project root di
-00001840: 7265 6374 6f72 7920 7769 7468 2060 7079  rectory with `py
-00001850: 7072 6f6a 6563 742e 746f 6d6c 602c 0a72  project.toml`,.r
-00001860: 756e 2074 6865 2065 6c6c 6172 2063 7265  un the ellar cre
-00001870: 6174 6520 7072 6f6a 6563 7420 636c 6920  ate project cli 
-00001880: 636f 6d6d 616e 642c 0a60 6060 7368 656c  command,.```shel
-00001890: 6c0a 656c 6c61 7220 6372 6561 7465 2d70  l.ellar create-p
-000018a0: 726f 6a65 6374 2063 6172 7369 7465 0a60  roject carsite.`
-000018b0: 6060 0a0a 2323 2052 756e 2079 6f75 7220  ``..## Run your 
-000018c0: 7072 6f6a 6563 740a 456c 6c61 7220 7275  project.Ellar ru
-000018d0: 6e73 205b 5556 4943 4f52 4e20 2d20 4153  ns [UVICORN - AS
-000018e0: 4749 2053 6572 7665 725d 2868 7474 7073  GI Server](https
-000018f0: 3a2f 2f77 7777 2e75 7669 636f 726e 2e6f  ://www.uvicorn.o
-00001900: 7267 2f29 2075 6e64 6572 2074 6865 2068  rg/) under the h
-00001910: 6f6f 642e 0a60 6060 7368 656c 6c0a 656c  ood..```shell.el
-00001920: 6c61 7220 7275 6e73 6572 7665 7220 2d2d  lar runserver --
-00001930: 7265 6c6f 6164 0a60 6060 0a60 2d2d 7265  reload.```.`--re
-00001940: 6c6f 6164 6020 6973 2074 6f20 7761 7463  load` is to watc
-00001950: 6820 666f 7220 6669 6c65 2063 6861 6e67  h for file chang
-00001960: 6573 0a0a 4e6f 7720 676f 2074 6f20 5b68  es..Now go to [h
-00001970: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00001980: 3830 3030 5d28 6874 7470 3a2f 2f31 3237  8000](http://127
-00001990: 2e30 2e30 2e31 3a38 3030 3029 0a21 5b53  .0.0.1:8000).![S
-000019a0: 7761 6767 6572 2055 495d 2864 6f63 732f  wagger UI](docs/
-000019b0: 696d 672f 656c 6c61 725f 6672 616d 6577  img/ellar_framew
-000019c0: 6f72 6b2e 706e 6729 0a0a 466f 7220 6d6f  ork.png)..For mo
-000019d0: 7265 2069 6e66 6f20 6f6e 2045 6c6c 6172  re info on Ellar
-000019e0: 2043 4c49 2c20 636c 6963 6b20 5b68 6572   CLI, click [her
-000019f0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00001a00: 622e 636f 6d2f 6561 6477 696e 436f 6465  b.com/eadwinCode
-00001a10: 2f65 6c6c 6172 2d63 6c69 290a 0a23 2320  /ellar-cli)..## 
-00001a20: 4372 6561 7465 2061 2070 726f 6a65 6374  Create a project
-00001a30: 206d 6f64 756c 650a 4120 7072 6f6a 6563   module.A projec
-00001a40: 7420 6d6f 6475 6c65 2069 7320 6120 7072  t module is a pr
-00001a50: 6f6a 6563 7420 6170 7020 6465 6669 6e69  oject app defini
-00001a60: 6e67 2061 2067 726f 7570 206f 6620 636f  ng a group of co
-00001a70: 6e74 726f 6c6c 6572 7320 6f72 2073 6572  ntrollers or ser
-00001a80: 7669 6365 7320 696e 636c 7564 696e 6720  vices including 
-00001a90: 7465 6d70 6c61 7465 7320 616e 6420 7374  templates and st
-00001aa0: 6174 6963 2066 696c 6573 2e0a 536f 2c20  atic files..So, 
-00001ab0: 6e6f 7720 7765 2068 6176 6520 6120 7072  now we have a pr
-00001ac0: 6f6a 6563 7420 6372 6561 7465 642c 206c  oject created, l
-00001ad0: 6574 7320 6164 6420 616e 2061 7070 2074  ets add an app t
-00001ae0: 6f20 7468 6520 7072 6f6a 6563 742e 0a60  o the project..`
-00001af0: 6060 7368 656c 6c0a 656c 6c61 7220 6372  ``shell.ellar cr
-00001b00: 6561 7465 2d6d 6f64 756c 6520 6361 720a  eate-module car.
-00001b10: 6060 600a 0a23 2320 4164 6420 5363 6865  ```..## Add Sche
-00001b20: 6d61 0a49 6e20 6063 6172 2f73 6368 656d  ma.In `car/schem
-00001b30: 612e 7079 602c 206c 6574 7320 6164 6420  a.py`, lets add 
-00001b40: 736f 6d65 2073 6572 6961 6c69 7a65 7220  some serializer 
-00001b50: 666f 7220 6361 7220 696e 7075 7420 616e  for car input an
-00001b60: 6420 6f75 7470 7574 2064 6174 610a 6060  d output data.``
-00001b70: 6070 7974 686f 6e0a 6672 6f6d 2065 6c6c  `python.from ell
-00001b80: 6172 2e73 6572 6961 6c69 7a65 7220 696d  ar.serializer im
-00001b90: 706f 7274 2053 6572 6961 6c69 7a65 720a  port Serializer.
-00001ba0: 0a63 6c61 7373 2043 6172 5365 7269 616c  .class CarSerial
-00001bb0: 697a 6572 2853 6572 6961 6c69 7a65 7229  izer(Serializer)
-00001bc0: 3a0a 2020 2020 6e61 6d65 3a20 7374 720a  :.    name: str.
-00001bd0: 2020 2020 6d6f 6465 6c3a 2073 7472 0a20      model: str. 
-00001be0: 2020 2062 7261 6e64 3a20 7374 720a 0a0a     brand: str...
-00001bf0: 636c 6173 7320 5265 7472 6965 7665 4361  class RetrieveCa
-00001c00: 7253 6572 6961 6c69 7a65 7228 4361 7253  rSerializer(CarS
-00001c10: 6572 6961 6c69 7a65 7229 3a0a 2020 2020  erializer):.    
-00001c20: 706b 3a20 7374 720a 6060 600a 0a23 2320  pk: str.```..## 
-00001c30: 4164 6420 5365 7276 6963 6573 0a49 6e20  Add Services.In 
-00001c40: 6063 6172 2f73 6572 7669 6365 732e 7079  `car/services.py
-00001c50: 602c 206c 6574 7320 6372 6561 7465 2061  `, lets create a
-00001c60: 2064 756d 6d79 2072 6570 6f73 6974 6f72   dummy repositor
-00001c70: 7920 6043 6172 4475 6d6d 7944 4260 2074  y `CarDummyDB` t
-00001c80: 6f20 6d61 6e61 6765 206f 7572 2063 6172  o manage our car
-00001c90: 2064 6174 612e 0a60 6060 7079 7468 6f6e   data..```python
-00001ca0: 0a69 6d70 6f72 7420 7479 7069 6e67 2061  .import typing a
-00001cb0: 7320 740a 696d 706f 7274 2075 7569 640a  s t.import uuid.
-00001cc0: 6672 6f6d 2065 6c6c 6172 2e64 6920 696d  from ellar.di im
-00001cd0: 706f 7274 2069 6e6a 6563 7461 626c 652c  port injectable,
-00001ce0: 2073 696e 676c 6574 6f6e 5f73 636f 7065   singleton_scope
-00001cf0: 0a0a 0a40 696e 6a65 6374 6162 6c65 2873  ...@injectable(s
-00001d00: 636f 7065 3d73 696e 676c 6574 6f6e 5f73  cope=singleton_s
-00001d10: 636f 7065 290a 636c 6173 7320 4361 7244  cope).class CarD
-00001d20: 756d 6d79 4442 3a0a 2020 2020 636c 6173  ummyDB:.    clas
-00001d30: 7320 4361 7244 756d 6d79 4442 4974 656d  s CarDummyDBItem
-00001d40: 3a0a 2020 2020 2020 2020 706b 3a20 7374  :.        pk: st
-00001d50: 720a 0a20 2020 2020 2020 2064 6566 205f  r..        def _
-00001d60: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a2a  _init__(self, **
-00001d70: 6461 7461 3a20 742e 4469 6374 2920 2d3e  data: t.Dict) ->
-00001d80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00001d90: 2020 2073 656c 662e 5f5f 6469 6374 5f5f     self.__dict__
-00001da0: 203d 2064 6174 610a 0a20 2020 2020 2020   = data..       
-00001db0: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-00001dc0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00001dd0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00001de0: 6e63 6528 6f74 6865 722c 2043 6172 4475  nce(other, CarDu
-00001df0: 6d6d 7944 422e 4361 7244 756d 6d79 4442  mmyDB.CarDummyDB
-00001e00: 4974 656d 293a 0a20 2020 2020 2020 2020  Item):.         
-00001e10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001e20: 6c66 2e70 6b20 3d3d 206f 7468 6572 2e70  lf.pk == other.p
-00001e30: 6b0a 2020 2020 2020 2020 2020 2020 7265  k.            re
-00001e40: 7475 726e 2073 656c 662e 706b 203d 3d20  turn self.pk == 
-00001e50: 7374 7228 6f74 6865 7229 0a0a 2020 2020  str(other)..    
-00001e60: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001e70: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00001e80: 2020 2020 7365 6c66 2e5f 6461 7461 3a20      self._data: 
-00001e90: 742e 4c69 7374 5b43 6172 4475 6d6d 7944  t.List[CarDummyD
-00001ea0: 422e 4361 7244 756d 6d79 4442 4974 656d  B.CarDummyDBItem
-00001eb0: 5d20 3d20 5b5d 0a0a 2020 2020 6465 6620  ] = []..    def 
-00001ec0: 6164 645f 6361 7228 7365 6c66 2c20 6461  add_car(self, da
-00001ed0: 7461 3a20 742e 4469 6374 2920 2d3e 2073  ta: t.Dict) -> s
-00001ee0: 7472 3a0a 2020 2020 2020 2020 706b 203d  tr:.        pk =
-00001ef0: 2075 7569 642e 7575 6964 3428 290a 2020   uuid.uuid4().  
-00001f00: 2020 2020 2020 5f64 6174 6120 3d20 6469        _data = di
-00001f10: 6374 2864 6174 6129 0a20 2020 2020 2020  ct(data).       
-00001f20: 205f 6461 7461 2e75 7064 6174 6528 706b   _data.update(pk
-00001f30: 3d73 7472 2870 6b29 290a 2020 2020 2020  =str(pk)).      
-00001f40: 2020 6974 656d 203d 2073 656c 662e 4361    item = self.Ca
-00001f50: 7244 756d 6d79 4442 4974 656d 282a 2a5f  rDummyDBItem(**_
-00001f60: 6461 7461 290a 2020 2020 2020 2020 7365  data).        se
-00001f70: 6c66 2e5f 6461 7461 2e61 7070 656e 6428  lf._data.append(
-00001f80: 6974 656d 290a 2020 2020 2020 2020 7265  item).        re
-00001f90: 7475 726e 2069 7465 6d2e 706b 0a0a 2020  turn item.pk..  
-00001fa0: 2020 6465 6620 6c69 7374 2873 656c 6629    def list(self)
-00001fb0: 202d 3e20 742e 4c69 7374 5b22 4361 7244   -> t.List["CarD
-00001fc0: 756d 6d79 4442 2e43 6172 4475 6d6d 7944  ummyDB.CarDummyD
-00001fd0: 4249 7465 6d22 5d3a 0a20 2020 2020 2020  BItem"]:.       
-00001fe0: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
-00001ff0: 7461 0a0a 2020 2020 6465 6620 7570 6461  ta..    def upda
-00002000: 7465 2873 656c 662c 2063 6172 5f69 643a  te(self, car_id:
-00002010: 2073 7472 2c20 6461 7461 3a20 742e 4469   str, data: t.Di
-00002020: 6374 2920 2d3e 2074 2e4f 7074 696f 6e61  ct) -> t.Optiona
-00002030: 6c5b 2243 6172 4475 6d6d 7944 422e 4361  l["CarDummyDB.Ca
-00002040: 7244 756d 6d79 4442 4974 656d 225d 3a0a  rDummyDBItem"]:.
-00002050: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
-00002060: 6c66 2e5f 6461 7461 2e69 6e64 6578 2863  lf._data.index(c
-00002070: 6172 5f69 6429 0a20 2020 2020 2020 2069  ar_id).        i
-00002080: 6620 6964 7820 3e3d 2030 3a0a 2020 2020  f idx >= 0:.    
-00002090: 2020 2020 2020 2020 5f64 6174 6120 3d20          _data = 
-000020a0: 6469 6374 2864 6174 6129 0a20 2020 2020  dict(data).     
-000020b0: 2020 2020 2020 205f 6461 7461 2e75 7064         _data.upd
-000020c0: 6174 6528 706b 3d73 7472 2863 6172 5f69  ate(pk=str(car_i
-000020d0: 6429 290a 2020 2020 2020 2020 2020 2020  d)).            
-000020e0: 7365 6c66 2e5f 6461 7461 5b69 6478 5d20  self._data[idx] 
-000020f0: 3d20 7365 6c66 2e43 6172 4475 6d6d 7944  = self.CarDummyD
-00002100: 4249 7465 6d28 2a2a 5f64 6174 6129 0a20  BItem(**_data). 
-00002110: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002120: 6e20 7365 6c66 2e5f 6461 7461 5b69 6478  n self._data[idx
-00002130: 5d0a 0a20 2020 2064 6566 2067 6574 2873  ]..    def get(s
-00002140: 656c 662c 2063 6172 5f69 643a 2073 7472  elf, car_id: str
-00002150: 2920 2d3e 2074 2e4f 7074 696f 6e61 6c5b  ) -> t.Optional[
-00002160: 2243 6172 4475 6d6d 7944 422e 4361 7244  "CarDummyDB.CarD
-00002170: 756d 6d79 4442 4974 656d 225d 3a0a 2020  ummyDBItem"]:.  
-00002180: 2020 2020 2020 6964 7820 3d20 7365 6c66        idx = self
-00002190: 2e5f 6461 7461 2e69 6e64 6578 2863 6172  ._data.index(car
-000021a0: 5f69 6429 0a20 2020 2020 2020 2069 6620  _id).        if 
-000021b0: 6964 7820 3e3d 2030 3a0a 2020 2020 2020  idx >= 0:.      
-000021c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000021d0: 662e 5f64 6174 615b 6964 785d 0a0a 2020  f._data[idx]..  
-000021e0: 2020 6465 6620 7265 6d6f 7665 2873 656c    def remove(sel
-000021f0: 662c 2063 6172 5f69 643a 2073 7472 2920  f, car_id: str) 
-00002200: 2d3e 2074 2e4f 7074 696f 6e61 6c5b 2243  -> t.Optional["C
-00002210: 6172 4475 6d6d 7944 422e 4361 7244 756d  arDummyDB.CarDum
-00002220: 6d79 4442 4974 656d 225d 3a0a 2020 2020  myDBItem"]:.    
-00002230: 2020 2020 6964 7820 3d20 7365 6c66 2e5f      idx = self._
-00002240: 6461 7461 2e69 6e64 6578 2863 6172 5f69  data.index(car_i
-00002250: 6429 0a20 2020 2020 2020 2069 6620 6964  d).        if id
-00002260: 7820 3e3d 2030 3a0a 2020 2020 2020 2020  x >= 0:.        
-00002270: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002280: 5f64 6174 612e 706f 7028 6964 7829 0a60  _data.pop(idx).`
-00002290: 6060 0a23 2320 4164 6420 436f 6e74 726f  ``.## Add Contro
-000022a0: 6c6c 6572 0a49 6e20 6063 6172 2f63 6f6e  ller.In `car/con
-000022b0: 7472 6f6c 6c65 7273 2e70 7960 2c20 6c65  trollers.py`, le
-000022c0: 7473 2063 7265 6174 6520 6043 6172 436f  ts create `CarCo
-000022d0: 6e74 726f 6c6c 6572 600a 0a60 6060 7079  ntroller`..```py
-000022e0: 7468 6f6e 0a69 6d70 6f72 7420 7479 7069  thon.import typi
-000022f0: 6e67 2061 7320 740a 6672 6f6d 2065 6c6c  ng as t.from ell
-00002300: 6172 2e63 6f6d 6d6f 6e20 696d 706f 7274  ar.common import
-00002310: 2043 6f6e 7472 6f6c 6c65 722c 2064 656c   Controller, del
-00002320: 6574 652c 2067 6574 2c20 7075 742c 2070  ete, get, put, p
-00002330: 6f73 740a 6672 6f6d 2065 6c6c 6172 2e63  ost.from ellar.c
-00002340: 6f72 6520 696d 706f 7274 2043 6f6e 7472  ore import Contr
-00002350: 6f6c 6c65 7242 6173 650a 6672 6f6d 2065  ollerBase.from e
-00002360: 6c6c 6172 2e63 6f72 652e 6578 6365 7074  llar.core.except
-00002370: 696f 6e73 2069 6d70 6f72 7420 4e6f 7446  ions import NotF
-00002380: 6f75 6e64 0a66 726f 6d20 2e73 6368 656d  ound.from .schem
-00002390: 6173 2069 6d70 6f72 7420 4361 7253 6572  as import CarSer
-000023a0: 6961 6c69 7a65 722c 2052 6574 7269 6576  ializer, Retriev
-000023b0: 6543 6172 5365 7269 616c 697a 6572 0a66  eCarSerializer.f
-000023c0: 726f 6d20 2e73 6572 7669 6365 7320 696d  rom .services im
-000023d0: 706f 7274 2043 6172 4475 6d6d 7944 420a  port CarDummyDB.
-000023e0: 0a0a 4043 6f6e 7472 6f6c 6c65 720a 636c  ..@Controller.cl
-000023f0: 6173 7320 4361 7243 6f6e 7472 6f6c 6c65  ass CarControlle
-00002400: 7228 436f 6e74 726f 6c6c 6572 4261 7365  r(ControllerBase
-00002410: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00002420: 745f 5f28 7365 6c66 2c20 6462 3a20 4361  t__(self, db: Ca
-00002430: 7244 756d 6d79 4442 2920 2d3e 204e 6f6e  rDummyDB) -> Non
-00002440: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
-00002450: 6361 725f 6462 203d 2064 620a 0a20 2020  car_db = db..   
-00002460: 2040 706f 7374 2822 2f63 7265 6174 6522   @post("/create"
-00002470: 2c20 7265 7370 6f6e 7365 3d7b 3230 303a  , response={200:
-00002480: 2073 7472 7d29 0a20 2020 2061 7379 6e63   str}).    async
-00002490: 2064 6566 2063 7265 6174 655f 6361 7428   def create_cat(
-000024a0: 7365 6c66 2c20 7061 796c 6f61 643a 2043  self, payload: C
-000024b0: 6172 5365 7269 616c 697a 6572 293a 0a20  arSerializer):. 
-000024c0: 2020 2020 2020 2070 6b20 3d20 7365 6c66         pk = self
-000024d0: 2e63 6172 5f64 622e 6164 645f 6361 7228  .car_db.add_car(
-000024e0: 7061 796c 6f61 642e 6469 6374 2829 290a  payload.dict()).
-000024f0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00002500: 6b0a 0a20 2020 2040 7075 7428 222f 7b63  k..    @put("/{c
-00002510: 6172 5f69 643a 7374 727d 222c 2072 6573  ar_id:str}", res
-00002520: 706f 6e73 653d 7b32 3030 3a20 5265 7472  ponse={200: Retr
-00002530: 6965 7665 4361 7253 6572 6961 6c69 7a65  ieveCarSerialize
-00002540: 727d 290a 2020 2020 6173 796e 6320 6465  r}).    async de
-00002550: 6620 7570 6461 7465 5f63 6174 2873 656c  f update_cat(sel
-00002560: 662c 2063 6172 5f69 643a 2073 7472 2c20  f, car_id: str, 
-00002570: 7061 796c 6f61 643a 2043 6172 5365 7269  payload: CarSeri
-00002580: 616c 697a 6572 293a 0a20 2020 2020 2020  alizer):.       
-00002590: 2063 6172 203d 2073 656c 662e 6361 725f   car = self.car_
-000025a0: 6462 2e75 7064 6174 6528 6361 725f 6964  db.update(car_id
-000025b0: 2c20 7061 796c 6f61 642e 6469 6374 2829  , payload.dict()
-000025c0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-000025d0: 2063 6172 3a0a 2020 2020 2020 2020 2020   car:.          
-000025e0: 2020 7261 6973 6520 4e6f 7446 6f75 6e64    raise NotFound
-000025f0: 2822 4974 656d 206e 6f74 2066 6f75 6e64  ("Item not found
-00002600: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00002610: 6e20 6361 720a 0a20 2020 2040 6765 7428  n car..    @get(
-00002620: 222f 7b63 6172 5f69 643a 7374 727d 222c  "/{car_id:str}",
-00002630: 2072 6573 706f 6e73 653d 7b32 3030 3a20   response={200: 
-00002640: 5265 7472 6965 7665 4361 7253 6572 6961  RetrieveCarSeria
-00002650: 6c69 7a65 727d 290a 2020 2020 6173 796e  lizer}).    asyn
-00002660: 6320 6465 6620 6765 745f 6361 725f 6279  c def get_car_by
-00002670: 5f69 6428 7365 6c66 2c20 6361 725f 6964  _id(self, car_id
-00002680: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-00002690: 6361 7220 3d20 7365 6c66 2e63 6172 5f64  car = self.car_d
-000026a0: 622e 6765 7428 6361 725f 6964 290a 2020  b.get(car_id).  
-000026b0: 2020 2020 2020 6966 206e 6f74 2063 6172        if not car
-000026c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000026d0: 6973 6520 4e6f 7446 6f75 6e64 2827 4974  ise NotFound('It
-000026e0: 656d 206e 6f74 2066 6f75 6e64 2e27 290a  em not found.').
-000026f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00002700: 6172 0a0a 2020 2020 4064 656c 6574 6528  ar..    @delete(
-00002710: 222f 7b63 6172 5f69 643a 7374 727d 222c  "/{car_id:str}",
-00002720: 2072 6573 706f 6e73 653d 7b32 3034 3a20   response={204: 
-00002730: 6469 6374 7d29 0a20 2020 2061 7379 6e63  dict}).    async
-00002740: 2064 6566 2064 656c 6574 6564 5f63 6174   def deleted_cat
-00002750: 2873 656c 662c 2063 6172 5f69 643a 2073  (self, car_id: s
-00002760: 7472 293a 0a20 2020 2020 2020 2063 6172  tr):.        car
-00002770: 203d 2073 656c 662e 6361 725f 6462 2e72   = self.car_db.r
-00002780: 656d 6f76 6528 6361 725f 6964 290a 2020  emove(car_id).  
-00002790: 2020 2020 2020 6966 206e 6f74 2063 6172        if not car
-000027a0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000027b0: 6973 6520 4e6f 7446 6f75 6e64 2827 4974  ise NotFound('It
-000027c0: 656d 206e 6f74 2066 6f75 6e64 2e27 290a  em not found.').
-000027d0: 2020 2020 2020 2020 7265 7475 726e 2032          return 2
-000027e0: 3034 2c20 7b7d 0a0a 2020 2020 4067 6574  04, {}..    @get
-000027f0: 2822 2f22 2c20 7265 7370 6f6e 7365 3d7b  ("/", response={
-00002800: 3230 303a 2074 2e4c 6973 745b 5265 7472  200: t.List[Retr
-00002810: 6965 7665 4361 7253 6572 6961 6c69 7a65  ieveCarSerialize
-00002820: 725d 7d29 0a20 2020 2061 7379 6e63 2064  r]}).    async d
-00002830: 6566 206c 6973 7428 7365 6c66 293a 0a20  ef list(self):. 
-00002840: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00002850: 6c66 2e63 6172 5f64 622e 6c69 7374 2829  lf.car_db.list()
-00002860: 0a0a 6060 600a 2323 2052 6567 6973 7465  ..```.## Registe
-00002870: 7220 5365 7276 6963 6520 616e 6420 436f  r Service and Co
-00002880: 6e74 726f 6c6c 6572 0a49 6e20 6063 6172  ntroller.In `car
-00002890: 2f6d 6f64 756c 652e 7079 602c 206c 6574  /module.py`, let
-000028a0: 7320 7265 6769 7374 6572 2060 4361 7243  s register `CarC
-000028b0: 6f6e 7472 6f6c 6c65 7260 2061 6e64 2060  ontroller` and `
-000028c0: 4361 7244 756d 6d79 4442 600a 0a60 6060  CarDummyDB`..```
-000028d0: 7079 7468 6f6e 0a66 726f 6d20 656c 6c61  python.from ella
-000028e0: 722e 636f 6d6d 6f6e 2069 6d70 6f72 7420  r.common import 
-000028f0: 4d6f 6475 6c65 0a66 726f 6d20 656c 6c61  Module.from ella
-00002900: 722e 636f 7265 2069 6d70 6f72 7420 4d6f  r.core import Mo
-00002910: 6475 6c65 4261 7365 0a66 726f 6d20 656c  duleBase.from el
-00002920: 6c61 722e 6469 2069 6d70 6f72 7420 436f  lar.di import Co
-00002930: 6e74 6169 6e65 720a 0a66 726f 6d20 2e63  ntainer..from .c
-00002940: 6f6e 7472 6f6c 6c65 7273 2069 6d70 6f72  ontrollers impor
-00002950: 7420 4361 7243 6f6e 7472 6f6c 6c65 720a  t CarController.
-00002960: 6672 6f6d 202e 7365 7276 6963 6573 2069  from .services i
-00002970: 6d70 6f72 7420 4361 7244 756d 6d79 4442  mport CarDummyDB
-00002980: 0a0a 0a40 4d6f 6475 6c65 280a 2020 2020  ...@Module(.    
-00002990: 636f 6e74 726f 6c6c 6572 733d 5b43 6172  controllers=[Car
-000029a0: 436f 6e74 726f 6c6c 6572 5d2c 0a20 2020  Controller],.   
-000029b0: 2070 726f 7669 6465 7273 3d5b 4361 7244   providers=[CarD
-000029c0: 756d 6d79 4442 5d2c 0a20 2020 2072 6f75  ummyDB],.    rou
-000029d0: 7465 7273 3d5b 5d2c 0a29 0a63 6c61 7373  ters=[],.).class
-000029e0: 2043 6172 4d6f 6475 6c65 284d 6f64 756c   CarModule(Modul
-000029f0: 6542 6173 6529 3a0a 2020 2020 6465 6620  eBase):.    def 
-00002a00: 7265 6769 7374 6572 5f70 726f 7669 6465  register_provide
-00002a10: 7273 2873 656c 662c 2063 6f6e 7461 696e  rs(self, contain
-00002a20: 6572 3a20 436f 6e74 6169 6e65 7229 202d  er: Container) -
-00002a30: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00002a40: 2320 666f 7220 6d6f 7265 2063 6f6d 706c  # for more compl
-00002a50: 6963 6174 6564 2070 726f 7669 6465 7220  icated provider 
-00002a60: 7265 6769 7374 7261 7469 6f6e 730a 2020  registrations.  
-00002a70: 2020 2020 2020 2320 636f 6e74 6169 6e65        # containe
-00002a80: 722e 7265 6769 7374 6572 5f69 6e73 7461  r.register_insta
-00002a90: 6e63 6528 2e2e 2e29 0a20 2020 2020 2020  nce(...).       
-00002aa0: 2070 6173 730a 6060 600a 0a23 2320 5265   pass.```..## Re
-00002ab0: 6769 7374 6572 696e 6720 4d6f 6475 6c65  gistering Module
-00002ac0: 0a45 6c6c 6172 2069 7320 6e6f 7420 6177  .Ellar is not aw
-00002ad0: 6172 6520 6f66 2060 4361 724d 6f64 756c  are of `CarModul
-00002ae0: 6560 2079 6574 2c20 736f 2077 6520 6e65  e` yet, so we ne
-00002af0: 6564 2074 6f20 6164 6420 6974 2074 6f20  ed to add it to 
-00002b00: 7468 6520 606d 6f64 756c 6573 6020 6c69  the `modules` li
-00002b10: 7374 206f 6620 6041 7070 6c69 6361 7469  st of `Applicati
-00002b20: 6f6e 4d6f 6475 6c65 6020 6174 2074 6865  onModule` at the
-00002b30: 2060 6361 7273 6974 652f 726f 6f74 5f6d   `carsite/root_m
-00002b40: 6f64 756c 652e 7079 602e 0a60 6060 7079  odule.py`..```py
-00002b50: 7468 6f6e 0a66 726f 6d20 656c 6c61 722e  thon.from ellar.
-00002b60: 636f 6d6d 6f6e 2069 6d70 6f72 7420 4d6f  common import Mo
-00002b70: 6475 6c65 2c20 6578 6365 7074 696f 6e5f  dule, exception_
-00002b80: 6861 6e64 6c65 720a 6672 6f6d 2065 6c6c  handler.from ell
-00002b90: 6172 2e63 6f72 6520 696d 706f 7274 2049  ar.core import I
-00002ba0: 486f 7374 436f 6e74 6578 742c 204d 6f64  HostContext, Mod
-00002bb0: 756c 6542 6173 650a 6672 6f6d 2065 6c6c  uleBase.from ell
-00002bc0: 6172 2e63 6f72 652e 7265 7370 6f6e 7365  ar.core.response
-00002bd0: 2069 6d70 6f72 7420 4a53 4f4e 5265 7370   import JSONResp
-00002be0: 6f6e 7365 2c20 5265 7370 6f6e 7365 0a0a  onse, Response..
-00002bf0: 6672 6f6d 2065 6c6c 6172 2e73 616d 706c  from ellar.sampl
-00002c00: 6573 2e6d 6f64 756c 6573 2069 6d70 6f72  es.modules impor
-00002c10: 7420 486f 6d65 4d6f 6475 6c65 0a66 726f  t HomeModule.fro
-00002c20: 6d20 2e61 7070 732e 6361 722e 6d6f 6475  m .apps.car.modu
-00002c30: 6c65 2069 6d70 6f72 7420 4361 724d 6f64  le import CarMod
-00002c40: 756c 650a 0a0a 404d 6f64 756c 6528 6d6f  ule...@Module(mo
-00002c50: 6475 6c65 733d 5b48 6f6d 654d 6f64 756c  dules=[HomeModul
-00002c60: 652c 2043 6172 4d6f 6475 6c65 5d29 0a63  e, CarModule]).c
-00002c70: 6c61 7373 2041 7070 6c69 6361 7469 6f6e  lass Application
-00002c80: 4d6f 6475 6c65 284d 6f64 756c 6542 6173  Module(ModuleBas
-00002c90: 6529 3a0a 2020 2020 4065 7863 6570 7469  e):.    @excepti
-00002ca0: 6f6e 5f68 616e 646c 6572 2834 3034 290a  on_handler(404).
-00002cb0: 2020 2020 6465 6620 6578 6365 7074 696f      def exceptio
-00002cc0: 6e5f 3430 345f 6861 6e64 6c65 7228 636c  n_404_handler(cl
-00002cd0: 732c 2063 6f6e 7465 7874 3a20 4948 6f73  s, context: IHos
-00002ce0: 7443 6f6e 7465 7874 2c20 6578 633a 2045  tContext, exc: E
-00002cf0: 7863 6570 7469 6f6e 2920 2d3e 2052 6573  xception) -> Res
-00002d00: 706f 6e73 653a 0a20 2020 2020 2020 2072  ponse:.        r
-00002d10: 6574 7572 6e20 4a53 4f4e 5265 7370 6f6e  eturn JSONRespon
-00002d20: 7365 2864 6963 7428 6465 7461 696c 3d22  se(dict(detail="
-00002d30: 5265 736f 7572 6365 206e 6f74 2066 6f75  Resource not fou
-00002d40: 6e64 2e22 2929 0a0a 6060 600a 2323 2045  nd."))..```.## E
-00002d50: 6e61 626c 696e 6720 4f70 656e 4150 4920  nabling OpenAPI 
-00002d60: 446f 6373 0a54 6f20 7374 6172 7420 7570  Docs.To start up
-00002d70: 206f 7065 6e61 7069 2c20 7765 206e 6565   openapi, we nee
-00002d80: 6420 746f 2067 6f20 6261 636b 2074 6f20  d to go back to 
-00002d90: 7072 6f6a 6563 7420 666f 6c64 6572 2069  project folder i
-00002da0: 6e20 7468 6520 6073 6572 7665 722e 7079  n the `server.py
-00002db0: 600a 7468 656e 2061 6464 2074 6865 2066  `.then add the f
-00002dc0: 6f6c 6c6f 7769 6e67 2062 656c 6f77 2e0a  ollowing below..
-00002dd0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00002de0: 206f 730a 0a66 726f 6d20 656c 6c61 722e   os..from ellar.
-00002df0: 636f 6e73 7461 6e74 7320 696d 706f 7274  constants import
-00002e00: 2045 4c4c 4152 5f43 4f4e 4649 475f 4d4f   ELLAR_CONFIG_MO
-00002e10: 4455 4c45 0a66 726f 6d20 656c 6c61 722e  DULE.from ellar.
-00002e20: 636f 7265 2e66 6163 746f 7279 2069 6d70  core.factory imp
-00002e30: 6f72 7420 4170 7046 6163 746f 7279 0a66  ort AppFactory.f
-00002e40: 726f 6d20 656c 6c61 722e 6f70 656e 6170  rom ellar.openap
-00002e50: 6920 696d 706f 7274 204f 7065 6e41 5049  i import OpenAPI
-00002e60: 446f 6375 6d65 6e74 4d6f 6475 6c65 2c20  DocumentModule, 
-00002e70: 4f70 656e 4150 4944 6f63 756d 656e 7442  OpenAPIDocumentB
-00002e80: 7569 6c64 6572 2c20 5377 6167 6765 7244  uilder, SwaggerD
-00002e90: 6f63 756d 656e 7447 656e 6572 6174 6f72  ocumentGenerator
-00002ea0: 0a66 726f 6d20 2e72 6f6f 745f 6d6f 6475  .from .root_modu
-00002eb0: 6c65 2069 6d70 6f72 7420 4170 706c 6963  le import Applic
-00002ec0: 6174 696f 6e4d 6f64 756c 650a 0a61 7070  ationModule..app
-00002ed0: 6c69 6361 7469 6f6e 203d 2041 7070 4661  lication = AppFa
-00002ee0: 6374 6f72 792e 6372 6561 7465 5f66 726f  ctory.create_fro
-00002ef0: 6d5f 6170 705f 6d6f 6475 6c65 280a 2020  m_app_module(.  
-00002f00: 2020 4170 706c 6963 6174 696f 6e4d 6f64    ApplicationMod
-00002f10: 756c 652c 0a20 2020 2063 6f6e 6669 675f  ule,.    config_
-00002f20: 6d6f 6475 6c65 3d6f 732e 656e 7669 726f  module=os.enviro
-00002f30: 6e2e 6765 7428 0a20 2020 2020 2020 2045  n.get(.        E
-00002f40: 4c4c 4152 5f43 4f4e 4649 475f 4d4f 4455  LLAR_CONFIG_MODU
-00002f50: 4c45 2c20 2263 6172 7369 7465 2e63 6f6e  LE, "carsite.con
-00002f60: 6669 673a 4465 7665 6c6f 706d 656e 7443  fig:DevelopmentC
-00002f70: 6f6e 6669 6722 0a20 2020 2029 2c0a 290a  onfig".    ),.).
-00002f80: 0a64 6f63 756d 656e 745f 6275 696c 6465  .document_builde
-00002f90: 7220 3d20 4f70 656e 4150 4944 6f63 756d  r = OpenAPIDocum
-00002fa0: 656e 7442 7569 6c64 6572 2829 0a64 6f63  entBuilder().doc
-00002fb0: 756d 656e 745f 6275 696c 6465 722e 7365  ument_builder.se
-00002fc0: 745f 7469 746c 6528 2743 6172 5369 7465  t_title('CarSite
-00002fd0: 2041 5049 2729 205c 0a20 2020 202e 7365   API') \.    .se
-00002fe0: 745f 7665 7273 696f 6e28 2731 2e30 2e30  t_version('1.0.0
-00002ff0: 2729 205c 0a20 2020 202e 7365 745f 636f  ') \.    .set_co
-00003000: 6e74 6163 7428 6e61 6d65 3d27 4561 6477  ntact(name='Eadw
-00003010: 696e 272c 2075 726c 3d27 6874 7470 733a  in', url='https:
-00003020: 2f2f 7777 772e 7961 686f 6f2e 636f 6d27  //www.yahoo.com'
-00003030: 2c20 656d 6169 6c3d 2765 6164 7769 6e40  , email='eadwin@
-00003040: 676d 6169 6c2e 636f 6d27 2920 5c0a 2020  gmail.com') \.  
-00003050: 2020 2e73 6574 5f6c 6963 656e 7365 2827    .set_license('
-00003060: 4d49 5420 4c69 6365 6e63 6527 2c20 7572  MIT Licence', ur
-00003070: 6c3d 2768 7474 7073 3a2f 2f77 7777 2e67  l='https://www.g
-00003080: 6f6f 676c 652e 636f 6d27 290a 0a64 6f63  oogle.com')..doc
-00003090: 756d 656e 7420 3d20 646f 6375 6d65 6e74  ument = document
-000030a0: 5f62 7569 6c64 6572 2e62 7569 6c64 5f64  _builder.build_d
-000030b0: 6f63 756d 656e 7428 6170 706c 6963 6174  ocument(applicat
-000030c0: 696f 6e29 0a6d 6f64 756c 6520 3d20 4f70  ion).module = Op
-000030d0: 656e 4150 4944 6f63 756d 656e 744d 6f64  enAPIDocumentMod
-000030e0: 756c 652e 7365 7475 7028 0a20 2020 2064  ule.setup(.    d
-000030f0: 6f63 756d 656e 743d 646f 6375 6d65 6e74  ocument=document
-00003100: 2c0a 2020 2020 646f 6375 6d65 6e74 5f67  ,.    document_g
-00003110: 656e 6572 6174 6f72 3d53 7761 6767 6572  enerator=Swagger
-00003120: 446f 6375 6d65 6e74 4765 6e65 7261 746f  DocumentGenerato
-00003130: 7228 292c 0a20 2020 2067 7561 7264 733d  r(),.    guards=
-00003140: 5b5d 0a29 0a61 7070 6c69 6361 7469 6f6e  [].).application
-00003150: 2e69 6e73 7461 6c6c 5f6d 6f64 756c 6528  .install_module(
-00003160: 6d6f 6475 6c65 290a 6060 600a 0a4e 6f77  module).```..Now
-00003170: 2077 6520 6361 6e20 7465 7374 206f 7572   we can test our
-00003180: 2041 5049 2061 7420 5b68 7474 703a 2f2f   API at [http://
-00003190: 3132 372e 302e 302e 313a 3830 3030 2f64  127.0.0.1:8000/d
-000031a0: 6f63 735d 2868 7474 703a 2f2f 3132 372e  ocs](http://127.
-000031b0: 302e 302e 313a 3830 3030 2f64 6f63 7323  0.0.1:8000/docs#
-000031c0: 2f29 0a50 6c65 6173 6520 656e 7375 7265  /).Please ensure
-000031d0: 2079 6f75 7220 7365 7276 6572 2069 7320   your server is 
-000031e0: 7275 6e6e 696e 670a 215b 5377 6167 6765  running.![Swagge
-000031f0: 7220 5549 5d28 646f 6373 2f69 6d67 2f63  r UI](docs/img/c
-00003200: 6172 5f61 7069 2e70 6e67 290a 0a23 2320  ar_api.png)..## 
-00003210: 4854 4d4c 2054 656d 706c 6174 696e 670a  HTML Templating.
-00003220: 456c 6c61 7220 6861 7320 6275 696c 742d  Ellar has built-
-00003230: 696e 2073 7570 706f 7274 2066 6f72 204a  in support for J
-00003240: 696e 6a61 322c 2077 6869 6368 2069 7320  inja2, which is 
-00003250: 6120 706f 7075 6c61 7220 7465 6d70 6c61  a popular templa
-00003260: 7465 2065 6e67 696e 6520 666f 7220 4854  te engine for HT
-00003270: 4d4c 2e20 5468 6973 2066 6561 7475 7265  ML. This feature
-00003280: 2061 6c6c 6f77 7320 666f 7220 6561 7379   allows for easy
-00003290: 2061 6e64 2065 6666 6963 6965 6e74 2048   and efficient H
-000032a0: 544d 4c20 7465 6d70 6c61 7469 6e67 2073  TML templating s
-000032b0: 696d 696c 6172 2074 6f20 7468 6174 206f  imilar to that o
-000032c0: 6620 466c 6173 6b2e 204a 696e 6a61 3220  f Flask. Jinja2 
-000032d0: 6361 6e20 6265 2075 7365 6420 746f 2063  can be used to c
-000032e0: 7265 6174 6520 7265 7573 6162 6c65 2074  reate reusable t
-000032f0: 656d 706c 6174 6573 2c20 616e 6420 746f  emplates, and to
-00003300: 2069 6e73 6572 7420 6479 6e61 6d69 6320   insert dynamic 
-00003310: 6461 7461 2069 6e74 6f20 4854 4d4c 2070  data into HTML p
-00003320: 6167 6573 2e20 4974 2061 6c73 6f20 6861  ages. It also ha
-00003330: 7320 7375 7070 6f72 7420 666f 7220 7465  s support for te
-00003340: 6d70 6c61 7465 2069 6e68 6572 6974 616e  mplate inheritan
-00003350: 6365 2c20 636f 6e74 726f 6c20 7374 7275  ce, control stru
-00003360: 6374 7572 6573 2c20 616e 6420 6f74 6865  ctures, and othe
-00003370: 7220 7573 6566 756c 2066 6561 7475 7265  r useful feature
-00003380: 7320 7468 6174 2063 616e 2068 656c 7020  s that can help 
-00003390: 746f 2073 696d 706c 6966 7920 616e 6420  to simplify and 
-000033a0: 7374 7265 616d 6c69 6e65 2074 6865 2070  streamline the p
-000033b0: 726f 6365 7373 206f 6620 6372 6561 7469  rocess of creati
-000033c0: 6e67 2048 544d 4c20 7465 6d70 6c61 7465  ng HTML template
-000033d0: 732e 0a0a 6060 6068 746d 6c0a 3c68 746d  s...```html.<htm
-000033e0: 6c3e 0a20 203c 626f 6479 3e0a 2020 2020  l>.  <body>.    
-000033f0: 3c75 6c3e 0a20 2020 2020 207b 2520 666f  <ul>.      {% fo
-00003400: 7220 6974 656d 2069 6e20 6974 656d 7320  r item in items 
-00003410: 257d 0a20 2020 2020 203c 6c69 3e7b 7b20  %}.      <li>{{ 
-00003420: 6974 656d 207d 7d3c 2f6c 693e 0a20 2020  item }}</li>.   
-00003430: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
-00003440: 2020 2020 3c2f 756c 3e0a 2020 3c2f 626f      </ul>.  </bo
-00003450: 6479 3e0a 3c2f 6874 6d6c 3e0a 6060 600a  dy>.</html>.```.
-00003460: 0a53 6565 2074 6865 205b 446f 635d 2868  .See the [Doc](h
-00003470: 7474 7073 3a2f 2f65 6164 7769 6e63 6f64  ttps://eadwincod
-00003480: 652e 6769 7468 7562 2e69 6f2f 656c 6c61  e.github.io/ella
-00003490: 722f 7465 6d70 6c61 7469 6e67 2f74 656d  r/templating/tem
-000034a0: 706c 6174 696e 672f 2920 666f 7220 6d6f  plating/) for mo
-000034b0: 7265 2065 7861 6d70 6c65 732e 0a0a 2323  re examples...##
-000034c0: 2050 726f 6a65 6374 2053 7461 7475 730a   Project Status.
-000034d0: 5072 6f6a 6563 7420 6973 2073 7469 6c6c  Project is still
-000034e0: 2069 6e20 6465 7665 6c6f 706d 656e 740a   in development.
-000034f0: 2d20 446f 6375 6d65 6e74 6174 696f 6e20  - Documentation 
-00003500: 2d20 2869 6e20 7072 6f67 7265 7373 290a  - (in progress).
-00003510: 2d20 496e 7465 7263 6570 746f 7273 2020  - Interceptors  
-00003520: 2d20 205b 4173 7065 6374 204f 7269 656e  -  [Aspect Orien
-00003530: 7465 6420 5072 6f67 7261 6d6d 696e 675d  ted Programming]
-00003540: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
-00003550: 7065 6469 612e 6f72 672f 7769 6b69 2f41  pedia.org/wiki/A
-00003560: 7370 6563 742d 6f72 6965 6e74 6564 5f70  spect-oriented_p
-00003570: 726f 6772 616d 6d69 6e67 2920 2841 4f50  rogramming) (AOP
-00003580: 2920 7465 6368 6e69 7175 650a 2d20 4461  ) technique.- Da
-00003590: 7461 6261 7365 2050 6c75 6769 6e20 7769  tabase Plugin wi
-000035a0: 7468 205b 456e 636f 6465 2f4f 524d 5d28  th [Encode/ORM](
-000035b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000035c0: 6f6d 2f65 6e63 6f64 652f 6f72 6d29 0a0a  om/encode/orm)..
+00001360: 6365 7320 7769 7468 2050 7974 686f 6e2e  ces with Python.
+00001370: 200a 5768 696c 6520 456c 6c61 7220 7072   .While Ellar pr
+00001380: 6f76 6964 6573 2061 2068 6967 6820 6c65  ovides a high le
+00001390: 7665 6c20 6f66 2061 6273 7472 6163 7469  vel of abstracti
+000013a0: 6f6e 206f 6e20 746f 7020 6f66 2053 7461  on on top of Sta
+000013b0: 726c 6574 7465 2c20 6974 2073 7469 6c6c  rlette, it still
+000013c0: 2069 6e63 6f72 706f 7261 7465 7320 736f   incorporates so
+000013d0: 6d65 206f 6620 6974 7320 6665 6174 7572  me of its featur
+000013e0: 6573 2c20 6173 2077 656c 6c20 6173 2074  es, as well as t
+000013f0: 686f 7365 206f 6620 4661 7374 4150 492e  hose of FastAPI.
+00001400: 200a 4966 2079 6f75 2061 7265 2066 616d   .If you are fam
+00001410: 696c 6961 7220 7769 7468 2074 6865 7365  iliar with these
+00001420: 2066 7261 6d65 776f 726b 732c 2079 6f75   frameworks, you
+00001430: 2077 696c 6c20 6669 6e64 2069 7420 6561   will find it ea
+00001440: 7379 2074 6f20 756e 6465 7273 7461 6e64  sy to understand
+00001450: 2061 6e64 2075 7365 2045 6c6c 6172 2e0a   and use Ellar..
+00001460: 0a23 2320 4665 6174 7572 6573 2053 756d  .## Features Sum
+00001470: 6d61 7279 0a0a 2d20 2a2a 4561 7379 2074  mary..- **Easy t
+00001480: 6f20 5573 652a 2a3a 2045 6c6c 6172 2068  o Use**: Ellar h
+00001490: 6173 2061 2073 696d 706c 6520 616e 6420  as a simple and 
+000014a0: 696e 7475 6974 6976 6520 4150 4920 7468  intuitive API th
+000014b0: 6174 206d 616b 6573 2069 7420 6561 7379  at makes it easy
+000014c0: 2074 6f20 6765 7420 7374 6172 7465 6420   to get started 
+000014d0: 7769 7468 2062 7569 6c64 696e 6720 6120  with building a 
+000014e0: 6661 7374 2061 6e64 2073 6361 6c61 626c  fast and scalabl
+000014f0: 6520 7765 6220 6170 706c 6963 6174 696f  e web applicatio
+00001500: 6e73 206f 7220 7765 6220 4150 4973 2069  ns or web APIs i
+00001510: 6e20 5079 7468 6f6e 2e0a 2d20 2a2a 4465  n Python..- **De
+00001520: 7065 6e64 656e 6379 2049 6e6a 6563 7469  pendency Injecti
+00001530: 6f6e 2028 4449 292a 2a3a 2049 7420 636f  on (DI)**: It co
+00001540: 6d65 7320 7769 7468 2044 4920 7379 7374  mes with DI syst
+00001550: 656d 206d 616b 6573 2069 7420 6561 7379  em makes it easy
+00001560: 2074 6f20 6d61 6e61 6765 2064 6570 656e   to manage depen
+00001570: 6465 6e63 6965 7320 616e 6420 7265 6475  dencies and redu
+00001580: 6365 2063 6f75 706c 696e 6720 6265 7477  ce coupling betw
+00001590: 6565 6e20 636f 6d70 6f6e 656e 7473 2e0a  een components..
+000015a0: 2d20 2a2a 5079 6461 6e74 6963 2049 6e74  - **Pydantic Int
+000015b0: 6567 7261 7469 6f6e 2a2a 3a20 4974 2069  egration**: It i
+000015c0: 7320 7072 6f70 6572 6c79 2069 6e74 6567  s properly integ
+000015d0: 7261 7465 6420 7769 7468 2050 7964 616e  rated with Pydan
+000015e0: 7469 632c 2061 2070 6f70 756c 6172 2050  tic, a popular P
+000015f0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00001600: 7220 6461 7461 2076 616c 6964 6174 696f  r data validatio
+00001610: 6e2c 2074 6f20 656e 7375 7265 2074 6861  n, to ensure tha
+00001620: 7420 696e 7075 7420 6461 7461 2069 7320  t input data is 
+00001630: 7661 6c69 642e 0a2d 202a 2a54 656d 706c  valid..- **Templ
+00001640: 6174 696e 6720 7769 7468 204a 696e 6a61  ating with Jinja
+00001650: 322a 2a3a 2045 6c6c 6172 2070 726f 7669  2**: Ellar provi
+00001660: 6465 7320 6275 696c 742d 696e 2073 7570  des built-in sup
+00001670: 706f 7274 2066 6f72 204a 696e 6a61 3220  port for Jinja2 
+00001680: 7465 6d70 6c61 7465 732c 206d 616b 696e  templates, makin
+00001690: 6720 6974 2065 6173 7920 746f 2063 7265  g it easy to cre
+000016a0: 6174 6520 6479 6e61 6d69 6320 7765 6220  ate dynamic web 
+000016b0: 7061 6765 732e 0a2d 202a 2a4f 7065 6e41  pages..- **OpenA
+000016c0: 5049 2044 6f63 756d 656e 7461 7469 6f6e  PI Documentation
+000016d0: 2a2a 3a20 4974 2063 6f6d 6573 2077 6974  **: It comes wit
+000016e0: 6820 6275 696c 742d 696e 2073 7570 706f  h built-in suppo
+000016f0: 7274 2066 6f72 204f 7065 6e41 5049 2064  rt for OpenAPI d
+00001700: 6f63 756d 656e 7461 7469 6f6e 2c20 6d61  ocumentation, ma
+00001710: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
+00001720: 6765 6e65 7261 7465 2060 5377 6167 6765  generate `Swagge
+00001730: 7260 206f 7220 6052 6544 6f63 6020 646f  r` or `ReDoc` do
+00001740: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
+00001750: 796f 7572 2041 5049 2e20 416e 6420 6d6f  your API. And mo
+00001760: 7265 2063 616e 2062 6520 6164 6465 6420  re can be added 
+00001770: 7769 7468 2065 6173 6520 6966 206e 6563  with ease if nec
+00001780: 6573 7361 7279 2e0a 2d20 2a2a 436f 6e74  essary..- **Cont
+00001790: 726f 6c6c 6572 2028 4d56 4329 2041 7263  roller (MVC) Arc
+000017a0: 6869 7465 6374 7572 652a 2a3a 2045 6c6c  hitecture**: Ell
+000017b0: 6172 2773 2063 6f6e 7472 6f6c 6c65 7220  ar's controller 
+000017c0: 6172 6368 6974 6563 7475 7265 2066 6f6c  architecture fol
+000017d0: 6c6f 7773 2074 6865 204d 6f64 656c 2d56  lows the Model-V
+000017e0: 6965 772d 436f 6e74 726f 6c6c 6572 2028  iew-Controller (
+000017f0: 4d56 4329 2070 6174 7465 726e 2c20 6d61  MVC) pattern, ma
+00001800: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
+00001810: 6f72 6761 6e69 7a65 2079 6f75 7220 636f  organize your co
+00001820: 6465 2e0a 2d20 2a2a 4775 6172 6473 2066  de..- **Guards f
+00001830: 6f72 2041 7574 6865 6e74 6963 6174 696f  or Authenticatio
+00001840: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
+00001850: 696f 6e2a 2a3a 2049 7420 7072 6f76 6964  ion**: It provid
+00001860: 6573 2062 7569 6c74 2d69 6e20 7375 7070  es built-in supp
+00001870: 6f72 7420 666f 7220 6775 6172 6473 2c20  ort for guards, 
+00001880: 616c 6c6f 7769 6e67 2079 6f75 2074 6f20  allowing you to 
+00001890: 6561 7369 6c79 2069 6d70 6c65 6d65 6e74  easily implement
+000018a0: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+000018b0: 616e 6420 6175 7468 6f72 697a 6174 696f  and authorizatio
+000018c0: 6e20 696e 2079 6f75 7220 6170 706c 6963  n in your applic
+000018d0: 6174 696f 6e2e 0a2d 202a 2a4d 6f64 756c  ation..- **Modul
+000018e0: 6172 6974 792a 2a3a 2045 6c6c 6172 2066  arity**: Ellar f
+000018f0: 6f6c 6c6f 7773 2061 206d 6f64 756c 6172  ollows a modular
+00001900: 2061 7263 6869 7465 6374 7572 6520 696e   architecture in
+00001910: 7370 6972 6564 2062 7920 4e65 7374 4a53  spired by NestJS
+00001920: 2c20 6d61 6b69 6e67 2069 7420 6561 7379  , making it easy
+00001930: 2074 6f20 6f72 6761 6e69 7a65 2079 6f75   to organize you
+00001940: 7220 636f 6465 2069 6e74 6f20 7265 7573  r code into reus
+00001950: 6162 6c65 206d 6f64 756c 6573 2e0a 2d20  able modules..- 
+00001960: 2a2a 4173 796e 6368 726f 6e6f 7573 2070  **Asynchronous p
+00001970: 726f 6772 616d 6d69 6e67 2a2a 3a20 4974  rogramming**: It
+00001980: 2061 6c6c 6f77 7320 796f 7520 746f 2074   allows you to t
+00001990: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
+000019a0: 6620 5079 7468 6f6e 2773 2060 6173 796e  f Python's `asyn
+000019b0: 632f 6177 6169 7460 2066 6561 7475 7265  c/await` feature
+000019c0: 2074 6f20 7772 6974 6520 6566 6669 6369   to write effici
+000019d0: 656e 7420 616e 6420 6661 7374 2063 6f64  ent and fast cod
+000019e0: 6520 7468 6174 2063 616e 2068 616e 646c  e that can handl
+000019f0: 6520 6c61 7267 6520 6e75 6d62 6572 7320  e large numbers 
+00001a00: 6f66 2063 6f6e 6375 7272 656e 7420 7265  of concurrent re
+00001a10: 7175 6573 7473 0a0a 2323 2044 6570 656e  quests..## Depen
+00001a20: 6465 6e63 6965 730a 2d20 5079 7468 6f6e  dencies.- Python
+00001a30: 203e 3d20 332e 370a 2d20 5374 6172 6c65   >= 3.7.- Starle
+00001a40: 7474 650a 2d20 496e 6a65 6374 6f72 0a2d  tte.- Injector.-
+00001a50: 2050 7964 616e 7469 630a 0a23 2320 496e   Pydantic..## In
+00001a60: 7374 616c 6c61 7469 6f6e 0a23 2323 2050  stallation.### P
+00001a70: 6f65 7472 7920 496e 7374 616c 6c61 7469  oetry Installati
+00001a80: 6f6e 0a46 6f72 205b 506f 6574 7279 5d28  on.For [Poetry](
+00001a90: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
+00001aa0: 6f65 7472 792e 6f72 672f 2920 7573 6167  oetry.org/) usag
+00001ab0: 6573 0a0a 6060 6073 6865 6c6c 0a70 6f65  es..```shell.poe
+00001ac0: 7472 7920 6164 6420 656c 6c61 722d 636c  try add ellar-cl
+00001ad0: 690a 6060 600a 0a23 2323 2050 6970 2049  i.```..### Pip I
+00001ae0: 6e73 7461 6c6c 6174 696f 6e0a 466f 7220  nstallation.For 
+00001af0: 6e6f 726d 616c 2070 6970 2069 6e73 7461  normal pip insta
+00001b00: 6c6c 6174 696f 6e0a 6060 6073 6865 6c6c  llation.```shell
+00001b10: 0a70 6970 2069 6e73 7461 6c6c 2065 6c6c  .pip install ell
+00001b20: 6172 2d63 6c69 0a60 6060 0a0a 2323 2043  ar-cli.```..## C
+00001b30: 7265 6174 6520 6120 7072 6f6a 6563 740a  reate a project.
+00001b40: 546f 2063 7265 6174 6520 616e 2065 6c6c  To create an ell
+00001b50: 6172 2070 726f 6a65 6374 2c20 796f 7520  ar project, you 
+00001b60: 6e65 6564 2074 6f20 6861 7665 2061 2060  need to have a `
+00001b70: 7079 7072 6f6a 6563 742e 746f 6d6c 6020  pyproject.toml` 
+00001b80: 6176 6169 6c61 626c 6520 6f6e 2079 6f75  available on you
+00001b90: 7220 726f 6f74 2064 6972 6563 746f 7279  r root directory
+00001ba0: 2e0a 5468 6973 2069 7320 6e65 6365 7373  ..This is necess
+00001bb0: 6172 7920 666f 7220 656c 6c61 7220 746f  ary for ellar to
+00001bc0: 2073 746f 7265 2073 6f6d 6520 606d 6574   store some `met
+00001bd0: 6164 6174 6160 2061 626f 7574 2079 6f75  adata` about you
+00001be0: 7220 7072 6f6a 6563 742e 200a 0a23 2323  r project. ..###
+00001bf0: 2043 7265 6174 6520 6120 7072 6f6a 6563   Create a projec
+00001c00: 740a 466f 7220 5069 7020 5573 6572 732c  t.For Pip Users,
+00001c10: 2079 6f75 206e 6565 6420 746f 2063 7265   you need to cre
+00001c20: 6174 6520 6070 7970 726f 6a65 6374 2e74  ate `pyproject.t
+00001c30: 6f6d 6c60 2066 696c 650a 6060 6073 6865  oml` file.```she
+00001c40: 6c6c 0a65 6c6c 6172 206e 6577 2063 6172  ll.ellar new car
+00001c50: 7369 7465 0a60 6060 0a49 6620 796f 7520  site.```.If you 
+00001c60: 6172 6520 7573 696e 6720 6050 6f65 7472  are using `Poetr
+00001c70: 7960 2c20 6174 2079 6f75 7220 7072 6f6a  y`, at your proj
+00001c80: 6563 7420 726f 6f74 2064 6972 6563 746f  ect root directo
+00001c90: 7279 2077 6974 6820 6070 7970 726f 6a65  ry with `pyproje
+00001ca0: 6374 2e74 6f6d 6c60 2c0a 7275 6e20 7468  ct.toml`,.run th
+00001cb0: 6520 656c 6c61 7220 6372 6561 7465 2070  e ellar create p
+00001cc0: 726f 6a65 6374 2063 6c69 2063 6f6d 6d61  roject cli comma
+00001cd0: 6e64 2c0a 6060 6073 6865 6c6c 0a65 6c6c  nd,.```shell.ell
+00001ce0: 6172 2063 7265 6174 652d 7072 6f6a 6563  ar create-projec
+00001cf0: 7420 6361 7273 6974 650a 6060 600a 0a23  t carsite.```..#
+00001d00: 2320 5275 6e20 796f 7572 2070 726f 6a65  # Run your proje
+00001d10: 6374 0a45 6c6c 6172 2072 756e 7320 5b55  ct.Ellar runs [U
+00001d20: 5649 434f 524e 202d 2041 5347 4920 5365  VICORN - ASGI Se
+00001d30: 7276 6572 5d28 6874 7470 733a 2f2f 7777  rver](https://ww
+00001d40: 772e 7576 6963 6f72 6e2e 6f72 672f 2920  w.uvicorn.org/) 
+00001d50: 756e 6465 7220 7468 6520 686f 6f64 2e0a  under the hood..
+00001d60: 6060 6073 6865 6c6c 0a65 6c6c 6172 2072  ```shell.ellar r
+00001d70: 756e 7365 7276 6572 202d 2d72 656c 6f61  unserver --reloa
+00001d80: 640a 6060 600a 602d 2d72 656c 6f61 6460  d.```.`--reload`
+00001d90: 2069 7320 746f 2077 6174 6368 2066 6f72   is to watch for
+00001da0: 2066 696c 6520 6368 616e 6765 730a 0a4e   file changes..N
+00001db0: 6f77 2067 6f20 746f 205b 6874 7470 3a2f  ow go to [http:/
+00001dc0: 2f31 3237 2e30 2e30 2e31 3a38 3030 305d  /127.0.0.1:8000]
+00001dd0: 2868 7474 703a 2f2f 3132 372e 302e 302e  (http://127.0.0.
+00001de0: 313a 3830 3030 290a 215b 5377 6167 6765  1:8000).![Swagge
+00001df0: 7220 5549 5d28 646f 6373 2f69 6d67 2f65  r UI](docs/img/e
+00001e00: 6c6c 6172 5f66 7261 6d65 776f 726b 2e70  llar_framework.p
+00001e10: 6e67 290a 0a46 6f72 206d 6f72 6520 696e  ng)..For more in
+00001e20: 666f 206f 6e20 456c 6c61 7220 434c 492c  fo on Ellar CLI,
+00001e30: 2063 6c69 636b 205b 6865 7265 5d28 6874   click [here](ht
+00001e40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001e50: 2f65 6164 7769 6e43 6f64 652f 656c 6c61  /eadwinCode/ella
+00001e60: 722d 636c 6929 0a0a 2323 2043 7265 6174  r-cli)..## Creat
+00001e70: 6520 6120 7072 6f6a 6563 7420 6d6f 6475  e a project modu
+00001e80: 6c65 0a41 2070 726f 6a65 6374 206d 6f64  le.A project mod
+00001e90: 756c 6520 6973 2061 2070 726f 6a65 6374  ule is a project
+00001ea0: 2061 7070 2064 6566 696e 696e 6720 6120   app defining a 
+00001eb0: 6772 6f75 7020 6f66 2063 6f6e 7472 6f6c  group of control
+00001ec0: 6c65 7273 206f 7220 7365 7276 6963 6573  lers or services
+00001ed0: 2069 6e63 6c75 6469 6e67 2074 656d 706c   including templ
+00001ee0: 6174 6573 2061 6e64 2073 7461 7469 6320  ates and static 
+00001ef0: 6669 6c65 732e 0a53 6f2c 206e 6f77 2077  files..So, now w
+00001f00: 6520 6861 7665 2061 2070 726f 6a65 6374  e have a project
+00001f10: 2063 7265 6174 6564 2c20 6c65 7473 2061   created, lets a
+00001f20: 6464 2061 6e20 6170 7020 746f 2074 6865  dd an app to the
+00001f30: 2070 726f 6a65 6374 2e0a 6060 6073 6865   project..```she
+00001f40: 6c6c 0a65 6c6c 6172 2063 7265 6174 652d  ll.ellar create-
+00001f50: 6d6f 6475 6c65 2063 6172 0a60 6060 0a0a  module car.```..
+00001f60: 2323 2041 6464 2053 6368 656d 610a 496e  ## Add Schema.In
+00001f70: 2060 6361 722f 7363 6865 6d61 2e70 7960   `car/schema.py`
+00001f80: 2c20 6c65 7473 2061 6464 2073 6f6d 6520  , lets add some 
+00001f90: 7365 7269 616c 697a 6572 2066 6f72 2063  serializer for c
+00001fa0: 6172 2069 6e70 7574 2061 6e64 206f 7574  ar input and out
+00001fb0: 7075 7420 6461 7461 0a60 6060 7079 7468  put data.```pyth
+00001fc0: 6f6e 0a66 726f 6d20 656c 6c61 722e 7365  on.from ellar.se
+00001fd0: 7269 616c 697a 6572 2069 6d70 6f72 7420  rializer import 
+00001fe0: 5365 7269 616c 697a 6572 0a0a 636c 6173  Serializer..clas
+00001ff0: 7320 4361 7253 6572 6961 6c69 7a65 7228  s CarSerializer(
+00002000: 5365 7269 616c 697a 6572 293a 0a20 2020  Serializer):.   
+00002010: 206e 616d 653a 2073 7472 0a20 2020 206d   name: str.    m
+00002020: 6f64 656c 3a20 7374 720a 2020 2020 6272  odel: str.    br
+00002030: 616e 643a 2073 7472 0a0a 0a63 6c61 7373  and: str...class
+00002040: 2052 6574 7269 6576 6543 6172 5365 7269   RetrieveCarSeri
+00002050: 616c 697a 6572 2843 6172 5365 7269 616c  alizer(CarSerial
+00002060: 697a 6572 293a 0a20 2020 2070 6b3a 2073  izer):.    pk: s
+00002070: 7472 0a60 6060 0a0a 2323 2041 6464 2053  tr.```..## Add S
+00002080: 6572 7669 6365 730a 496e 2060 6361 722f  ervices.In `car/
+00002090: 7365 7276 6963 6573 2e70 7960 2c20 6c65  services.py`, le
+000020a0: 7473 2063 7265 6174 6520 6120 6475 6d6d  ts create a dumm
+000020b0: 7920 7265 706f 7369 746f 7279 2060 4361  y repository `Ca
+000020c0: 7244 756d 6d79 4442 6020 746f 206d 616e  rDummyDB` to man
+000020d0: 6167 6520 6f75 7220 6361 7220 6461 7461  age our car data
+000020e0: 2e0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+000020f0: 7274 2074 7970 696e 6720 6173 2074 0a69  rt typing as t.i
+00002100: 6d70 6f72 7420 7575 6964 0a66 726f 6d20  mport uuid.from 
+00002110: 656c 6c61 722e 6469 2069 6d70 6f72 7420  ellar.di import 
+00002120: 696e 6a65 6374 6162 6c65 2c20 7369 6e67  injectable, sing
+00002130: 6c65 746f 6e5f 7363 6f70 650a 0a0a 4069  leton_scope...@i
+00002140: 6e6a 6563 7461 626c 6528 7363 6f70 653d  njectable(scope=
+00002150: 7369 6e67 6c65 746f 6e5f 7363 6f70 6529  singleton_scope)
+00002160: 0a63 6c61 7373 2043 6172 4475 6d6d 7944  .class CarDummyD
+00002170: 423a 0a20 2020 2063 6c61 7373 2043 6172  B:.    class Car
+00002180: 4475 6d6d 7944 4249 7465 6d3a 0a20 2020  DummyDBItem:.   
+00002190: 2020 2020 2070 6b3a 2073 7472 0a0a 2020       pk: str..  
+000021a0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+000021b0: 5f5f 2873 656c 662c 202a 2a64 6174 613a  __(self, **data:
+000021c0: 2074 2e44 6963 7429 202d 3e20 4e6f 6e65   t.Dict) -> None
+000021d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000021e0: 6c66 2e5f 5f64 6963 745f 5f20 3d20 6461  lf.__dict__ = da
+000021f0: 7461 0a0a 2020 2020 2020 2020 6465 6620  ta..        def 
+00002200: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
+00002210: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
+00002220: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
+00002230: 7468 6572 2c20 4361 7244 756d 6d79 4442  ther, CarDummyDB
+00002240: 2e43 6172 4475 6d6d 7944 4249 7465 6d29  .CarDummyDBItem)
+00002250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002260: 2020 7265 7475 726e 2073 656c 662e 706b    return self.pk
+00002270: 203d 3d20 6f74 6865 722e 706b 0a20 2020   == other.pk.   
+00002280: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002290: 7365 6c66 2e70 6b20 3d3d 2073 7472 286f  self.pk == str(o
+000022a0: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
+000022b0: 5f69 6e69 745f 5f28 7365 6c66 2920 2d3e  _init__(self) ->
+000022c0: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+000022d0: 656c 662e 5f64 6174 613a 2074 2e4c 6973  elf._data: t.Lis
+000022e0: 745b 4361 7244 756d 6d79 4442 2e43 6172  t[CarDummyDB.Car
+000022f0: 4475 6d6d 7944 4249 7465 6d5d 203d 205b  DummyDBItem] = [
+00002300: 5d0a 0a20 2020 2064 6566 2061 6464 5f63  ]..    def add_c
+00002310: 6172 2873 656c 662c 2064 6174 613a 2074  ar(self, data: t
+00002320: 2e44 6963 7429 202d 3e20 7374 723a 0a20  .Dict) -> str:. 
+00002330: 2020 2020 2020 2070 6b20 3d20 7575 6964         pk = uuid
+00002340: 2e75 7569 6434 2829 0a20 2020 2020 2020  .uuid4().       
+00002350: 205f 6461 7461 203d 2064 6963 7428 6461   _data = dict(da
+00002360: 7461 290a 2020 2020 2020 2020 5f64 6174  ta).        _dat
+00002370: 612e 7570 6461 7465 2870 6b3d 7374 7228  a.update(pk=str(
+00002380: 706b 2929 0a20 2020 2020 2020 2069 7465  pk)).        ite
+00002390: 6d20 3d20 7365 6c66 2e43 6172 4475 6d6d  m = self.CarDumm
+000023a0: 7944 4249 7465 6d28 2a2a 5f64 6174 6129  yDBItem(**_data)
+000023b0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+000023c0: 6174 612e 6170 7065 6e64 2869 7465 6d29  ata.append(item)
+000023d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000023e0: 6974 656d 2e70 6b0a 0a20 2020 2064 6566  item.pk..    def
+000023f0: 206c 6973 7428 7365 6c66 2920 2d3e 2074   list(self) -> t
+00002400: 2e4c 6973 745b 2243 6172 4475 6d6d 7944  .List["CarDummyD
+00002410: 422e 4361 7244 756d 6d79 4442 4974 656d  B.CarDummyDBItem
+00002420: 225d 3a0a 2020 2020 2020 2020 7265 7475  "]:.        retu
+00002430: 726e 2073 656c 662e 5f64 6174 610a 0a20  rn self._data.. 
+00002440: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
+00002450: 6c66 2c20 6361 725f 6964 3a20 7374 722c  lf, car_id: str,
+00002460: 2064 6174 613a 2074 2e44 6963 7429 202d   data: t.Dict) -
+00002470: 3e20 742e 4f70 7469 6f6e 616c 5b22 4361  > t.Optional["Ca
+00002480: 7244 756d 6d79 4442 2e43 6172 4475 6d6d  rDummyDB.CarDumm
+00002490: 7944 4249 7465 6d22 5d3a 0a20 2020 2020  yDBItem"]:.     
+000024a0: 2020 2069 6478 203d 2073 656c 662e 5f64     idx = self._d
+000024b0: 6174 612e 696e 6465 7828 6361 725f 6964  ata.index(car_id
+000024c0: 290a 2020 2020 2020 2020 6966 2069 6478  ).        if idx
+000024d0: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
+000024e0: 2020 205f 6461 7461 203d 2064 6963 7428     _data = dict(
+000024f0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+00002500: 2020 5f64 6174 612e 7570 6461 7465 2870    _data.update(p
+00002510: 6b3d 7374 7228 6361 725f 6964 2929 0a20  k=str(car_id)). 
+00002520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002530: 5f64 6174 615b 6964 785d 203d 2073 656c  _data[idx] = sel
+00002540: 662e 4361 7244 756d 6d79 4442 4974 656d  f.CarDummyDBItem
+00002550: 282a 2a5f 6461 7461 290a 2020 2020 2020  (**_data).      
+00002560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002570: 662e 5f64 6174 615b 6964 785d 0a0a 2020  f._data[idx]..  
+00002580: 2020 6465 6620 6765 7428 7365 6c66 2c20    def get(self, 
+00002590: 6361 725f 6964 3a20 7374 7229 202d 3e20  car_id: str) -> 
+000025a0: 742e 4f70 7469 6f6e 616c 5b22 4361 7244  t.Optional["CarD
+000025b0: 756d 6d79 4442 2e43 6172 4475 6d6d 7944  ummyDB.CarDummyD
+000025c0: 4249 7465 6d22 5d3a 0a20 2020 2020 2020  BItem"]:.       
+000025d0: 2069 6478 203d 2073 656c 662e 5f64 6174   idx = self._dat
+000025e0: 612e 696e 6465 7828 6361 725f 6964 290a  a.index(car_id).
+000025f0: 2020 2020 2020 2020 6966 2069 6478 203e          if idx >
+00002600: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00002610: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
+00002620: 7461 5b69 6478 5d0a 0a20 2020 2064 6566  ta[idx]..    def
+00002630: 2072 656d 6f76 6528 7365 6c66 2c20 6361   remove(self, ca
+00002640: 725f 6964 3a20 7374 7229 202d 3e20 742e  r_id: str) -> t.
+00002650: 4f70 7469 6f6e 616c 5b22 4361 7244 756d  Optional["CarDum
+00002660: 6d79 4442 2e43 6172 4475 6d6d 7944 4249  myDB.CarDummyDBI
+00002670: 7465 6d22 5d3a 0a20 2020 2020 2020 2069  tem"]:.        i
+00002680: 6478 203d 2073 656c 662e 5f64 6174 612e  dx = self._data.
+00002690: 696e 6465 7828 6361 725f 6964 290a 2020  index(car_id).  
+000026a0: 2020 2020 2020 6966 2069 6478 203e 3d20        if idx >= 
+000026b0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+000026c0: 6574 7572 6e20 7365 6c66 2e5f 6461 7461  eturn self._data
+000026d0: 2e70 6f70 2869 6478 290a 6060 600a 2323  .pop(idx).```.##
+000026e0: 2041 6464 2043 6f6e 7472 6f6c 6c65 720a   Add Controller.
+000026f0: 496e 2060 6361 722f 636f 6e74 726f 6c6c  In `car/controll
+00002700: 6572 732e 7079 602c 206c 6574 7320 6372  ers.py`, lets cr
+00002710: 6561 7465 2060 4361 7243 6f6e 7472 6f6c  eate `CarControl
+00002720: 6c65 7260 0a0a 6060 6070 7974 686f 6e0a  ler`..```python.
+00002730: 696d 706f 7274 2074 7970 696e 6720 6173  import typing as
+00002740: 2074 0a66 726f 6d20 656c 6c61 722e 636f   t.from ellar.co
+00002750: 6d6d 6f6e 2069 6d70 6f72 7420 436f 6e74  mmon import Cont
+00002760: 726f 6c6c 6572 2c20 6465 6c65 7465 2c20  roller, delete, 
+00002770: 6765 742c 2070 7574 2c20 706f 7374 0a66  get, put, post.f
+00002780: 726f 6d20 656c 6c61 722e 636f 7265 2069  rom ellar.core i
+00002790: 6d70 6f72 7420 436f 6e74 726f 6c6c 6572  mport Controller
+000027a0: 4261 7365 0a66 726f 6d20 656c 6c61 722e  Base.from ellar.
+000027b0: 636f 7265 2e65 7863 6570 7469 6f6e 7320  core.exceptions 
+000027c0: 696d 706f 7274 204e 6f74 466f 756e 640a  import NotFound.
+000027d0: 6672 6f6d 202e 7363 6865 6d61 7320 696d  from .schemas im
+000027e0: 706f 7274 2043 6172 5365 7269 616c 697a  port CarSerializ
+000027f0: 6572 2c20 5265 7472 6965 7665 4361 7253  er, RetrieveCarS
+00002800: 6572 6961 6c69 7a65 720a 6672 6f6d 202e  erializer.from .
+00002810: 7365 7276 6963 6573 2069 6d70 6f72 7420  services import 
+00002820: 4361 7244 756d 6d79 4442 0a0a 0a40 436f  CarDummyDB...@Co
+00002830: 6e74 726f 6c6c 6572 0a63 6c61 7373 2043  ntroller.class C
+00002840: 6172 436f 6e74 726f 6c6c 6572 2843 6f6e  arController(Con
+00002850: 7472 6f6c 6c65 7242 6173 6529 3a0a 2020  trollerBase):.  
+00002860: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00002870: 656c 662c 2064 623a 2043 6172 4475 6d6d  elf, db: CarDumm
+00002880: 7944 4229 202d 3e20 4e6f 6e65 3a0a 2020  yDB) -> None:.  
+00002890: 2020 2020 2020 7365 6c66 2e63 6172 5f64        self.car_d
+000028a0: 6220 3d20 6462 0a0a 2020 2020 4070 6f73  b = db..    @pos
+000028b0: 7428 222f 6372 6561 7465 222c 2072 6573  t("/create", res
+000028c0: 706f 6e73 653d 7b32 3030 3a20 7374 727d  ponse={200: str}
+000028d0: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
+000028e0: 6372 6561 7465 5f63 6174 2873 656c 662c  create_cat(self,
+000028f0: 2070 6179 6c6f 6164 3a20 4361 7253 6572   payload: CarSer
+00002900: 6961 6c69 7a65 7229 3a0a 2020 2020 2020  ializer):.      
+00002910: 2020 706b 203d 2073 656c 662e 6361 725f    pk = self.car_
+00002920: 6462 2e61 6464 5f63 6172 2870 6179 6c6f  db.add_car(paylo
+00002930: 6164 2e64 6963 7428 2929 0a20 2020 2020  ad.dict()).     
+00002940: 2020 2072 6574 7572 6e20 706b 0a0a 2020     return pk..  
+00002950: 2020 4070 7574 2822 2f7b 6361 725f 6964    @put("/{car_id
+00002960: 3a73 7472 7d22 2c20 7265 7370 6f6e 7365  :str}", response
+00002970: 3d7b 3230 303a 2052 6574 7269 6576 6543  ={200: RetrieveC
+00002980: 6172 5365 7269 616c 697a 6572 7d29 0a20  arSerializer}). 
+00002990: 2020 2061 7379 6e63 2064 6566 2075 7064     async def upd
+000029a0: 6174 655f 6361 7428 7365 6c66 2c20 6361  ate_cat(self, ca
+000029b0: 725f 6964 3a20 7374 722c 2070 6179 6c6f  r_id: str, paylo
+000029c0: 6164 3a20 4361 7253 6572 6961 6c69 7a65  ad: CarSerialize
+000029d0: 7229 3a0a 2020 2020 2020 2020 6361 7220  r):.        car 
+000029e0: 3d20 7365 6c66 2e63 6172 5f64 622e 7570  = self.car_db.up
+000029f0: 6461 7465 2863 6172 5f69 642c 2070 6179  date(car_id, pay
+00002a00: 6c6f 6164 2e64 6963 7428 2929 0a20 2020  load.dict()).   
+00002a10: 2020 2020 2069 6620 6e6f 7420 6361 723a       if not car:
+00002a20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00002a30: 7365 204e 6f74 466f 756e 6428 2249 7465  se NotFound("Ite
+00002a40: 6d20 6e6f 7420 666f 756e 6422 290a 2020  m not found").  
+00002a50: 2020 2020 2020 7265 7475 726e 2063 6172        return car
+00002a60: 0a0a 2020 2020 4067 6574 2822 2f7b 6361  ..    @get("/{ca
+00002a70: 725f 6964 3a73 7472 7d22 2c20 7265 7370  r_id:str}", resp
+00002a80: 6f6e 7365 3d7b 3230 303a 2052 6574 7269  onse={200: Retri
+00002a90: 6576 6543 6172 5365 7269 616c 697a 6572  eveCarSerializer
+00002aa0: 7d29 0a20 2020 2061 7379 6e63 2064 6566  }).    async def
+00002ab0: 2067 6574 5f63 6172 5f62 795f 6964 2873   get_car_by_id(s
+00002ac0: 656c 662c 2063 6172 5f69 643a 2073 7472  elf, car_id: str
+00002ad0: 293a 0a20 2020 2020 2020 2063 6172 203d  ):.        car =
+00002ae0: 2073 656c 662e 6361 725f 6462 2e67 6574   self.car_db.get
+00002af0: 2863 6172 5f69 6429 0a20 2020 2020 2020  (car_id).       
+00002b00: 2069 6620 6e6f 7420 6361 723a 0a20 2020   if not car:.   
+00002b10: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+00002b20: 6f74 466f 756e 6428 2749 7465 6d20 6e6f  otFound('Item no
+00002b30: 7420 666f 756e 642e 2729 0a20 2020 2020  t found.').     
+00002b40: 2020 2072 6574 7572 6e20 6361 720a 0a20     return car.. 
+00002b50: 2020 2040 6465 6c65 7465 2822 2f7b 6361     @delete("/{ca
+00002b60: 725f 6964 3a73 7472 7d22 2c20 7265 7370  r_id:str}", resp
+00002b70: 6f6e 7365 3d7b 3230 343a 2064 6963 747d  onse={204: dict}
+00002b80: 290a 2020 2020 6173 796e 6320 6465 6620  ).    async def 
+00002b90: 6465 6c65 7465 645f 6361 7428 7365 6c66  deleted_cat(self
+00002ba0: 2c20 6361 725f 6964 3a20 7374 7229 3a0a  , car_id: str):.
+00002bb0: 2020 2020 2020 2020 6361 7220 3d20 7365          car = se
+00002bc0: 6c66 2e63 6172 5f64 622e 7265 6d6f 7665  lf.car_db.remove
+00002bd0: 2863 6172 5f69 6429 0a20 2020 2020 2020  (car_id).       
+00002be0: 2069 6620 6e6f 7420 6361 723a 0a20 2020   if not car:.   
+00002bf0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+00002c00: 6f74 466f 756e 6428 2749 7465 6d20 6e6f  otFound('Item no
+00002c10: 7420 666f 756e 642e 2729 0a20 2020 2020  t found.').     
+00002c20: 2020 2072 6574 7572 6e20 3230 342c 207b     return 204, {
+00002c30: 7d0a 0a20 2020 2040 6765 7428 222f 222c  }..    @get("/",
+00002c40: 2072 6573 706f 6e73 653d 7b32 3030 3a20   response={200: 
+00002c50: 742e 4c69 7374 5b52 6574 7269 6576 6543  t.List[RetrieveC
+00002c60: 6172 5365 7269 616c 697a 6572 5d7d 290a  arSerializer]}).
+00002c70: 2020 2020 6173 796e 6320 6465 6620 6c69      async def li
+00002c80: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
+00002c90: 2020 7265 7475 726e 2073 656c 662e 6361    return self.ca
+00002ca0: 725f 6462 2e6c 6973 7428 290a 0a60 6060  r_db.list()..```
+00002cb0: 0a23 2320 5265 6769 7374 6572 2053 6572  .## Register Ser
+00002cc0: 7669 6365 2061 6e64 2043 6f6e 7472 6f6c  vice and Control
+00002cd0: 6c65 720a 496e 2060 6361 722f 6d6f 6475  ler.In `car/modu
+00002ce0: 6c65 2e70 7960 2c20 6c65 7473 2072 6567  le.py`, lets reg
+00002cf0: 6973 7465 7220 6043 6172 436f 6e74 726f  ister `CarContro
+00002d00: 6c6c 6572 6020 616e 6420 6043 6172 4475  ller` and `CarDu
+00002d10: 6d6d 7944 4260 0a0a 6060 6070 7974 686f  mmyDB`..```pytho
+00002d20: 6e0a 6672 6f6d 2065 6c6c 6172 2e63 6f6d  n.from ellar.com
+00002d30: 6d6f 6e20 696d 706f 7274 204d 6f64 756c  mon import Modul
+00002d40: 650a 6672 6f6d 2065 6c6c 6172 2e63 6f72  e.from ellar.cor
+00002d50: 6520 696d 706f 7274 204d 6f64 756c 6542  e import ModuleB
+00002d60: 6173 650a 6672 6f6d 2065 6c6c 6172 2e64  ase.from ellar.d
+00002d70: 6920 696d 706f 7274 2043 6f6e 7461 696e  i import Contain
+00002d80: 6572 0a0a 6672 6f6d 202e 636f 6e74 726f  er..from .contro
+00002d90: 6c6c 6572 7320 696d 706f 7274 2043 6172  llers import Car
+00002da0: 436f 6e74 726f 6c6c 6572 0a66 726f 6d20  Controller.from 
+00002db0: 2e73 6572 7669 6365 7320 696d 706f 7274  .services import
+00002dc0: 2043 6172 4475 6d6d 7944 420a 0a0a 404d   CarDummyDB...@M
+00002dd0: 6f64 756c 6528 0a20 2020 2063 6f6e 7472  odule(.    contr
+00002de0: 6f6c 6c65 7273 3d5b 4361 7243 6f6e 7472  ollers=[CarContr
+00002df0: 6f6c 6c65 725d 2c0a 2020 2020 7072 6f76  oller],.    prov
+00002e00: 6964 6572 733d 5b43 6172 4475 6d6d 7944  iders=[CarDummyD
+00002e10: 425d 2c0a 2020 2020 726f 7574 6572 733d  B],.    routers=
+00002e20: 5b5d 2c0a 290a 636c 6173 7320 4361 724d  [],.).class CarM
+00002e30: 6f64 756c 6528 4d6f 6475 6c65 4261 7365  odule(ModuleBase
+00002e40: 293a 0a20 2020 2064 6566 2072 6567 6973  ):.    def regis
+00002e50: 7465 725f 7072 6f76 6964 6572 7328 7365  ter_providers(se
+00002e60: 6c66 2c20 636f 6e74 6169 6e65 723a 2043  lf, container: C
+00002e70: 6f6e 7461 696e 6572 2920 2d3e 204e 6f6e  ontainer) -> Non
+00002e80: 653a 0a20 2020 2020 2020 2023 2066 6f72  e:.        # for
+00002e90: 206d 6f72 6520 636f 6d70 6c69 6361 7465   more complicate
+00002ea0: 6420 7072 6f76 6964 6572 2072 6567 6973  d provider regis
+00002eb0: 7472 6174 696f 6e73 0a20 2020 2020 2020  trations.       
+00002ec0: 2023 2063 6f6e 7461 696e 6572 2e72 6567   # container.reg
+00002ed0: 6973 7465 725f 696e 7374 616e 6365 282e  ister_instance(.
+00002ee0: 2e2e 290a 2020 2020 2020 2020 7061 7373  ..).        pass
+00002ef0: 0a60 6060 0a0a 2323 2052 6567 6973 7465  .```..## Registe
+00002f00: 7269 6e67 204d 6f64 756c 650a 456c 6c61  ring Module.Ella
+00002f10: 7220 6973 206e 6f74 2061 7761 7265 206f  r is not aware o
+00002f20: 6620 6043 6172 4d6f 6475 6c65 6020 7965  f `CarModule` ye
+00002f30: 742c 2073 6f20 7765 206e 6565 6420 746f  t, so we need to
+00002f40: 2061 6464 2069 7420 746f 2074 6865 2060   add it to the `
+00002f50: 6d6f 6475 6c65 7360 206c 6973 7420 6f66  modules` list of
+00002f60: 2060 4170 706c 6963 6174 696f 6e4d 6f64   `ApplicationMod
+00002f70: 756c 6560 2061 7420 7468 6520 6063 6172  ule` at the `car
+00002f80: 7369 7465 2f72 6f6f 745f 6d6f 6475 6c65  site/root_module
+00002f90: 2e70 7960 2e0a 6060 6070 7974 686f 6e0a  .py`..```python.
+00002fa0: 6672 6f6d 2065 6c6c 6172 2e63 6f6d 6d6f  from ellar.commo
+00002fb0: 6e20 696d 706f 7274 204d 6f64 756c 652c  n import Module,
+00002fc0: 2065 7863 6570 7469 6f6e 5f68 616e 646c   exception_handl
+00002fd0: 6572 0a66 726f 6d20 656c 6c61 722e 636f  er.from ellar.co
+00002fe0: 7265 2069 6d70 6f72 7420 4948 6f73 7443  re import IHostC
+00002ff0: 6f6e 7465 7874 2c20 4d6f 6475 6c65 4261  ontext, ModuleBa
+00003000: 7365 0a66 726f 6d20 656c 6c61 722e 636f  se.from ellar.co
+00003010: 7265 2e72 6573 706f 6e73 6520 696d 706f  re.response impo
+00003020: 7274 204a 534f 4e52 6573 706f 6e73 652c  rt JSONResponse,
+00003030: 2052 6573 706f 6e73 650a 0a66 726f 6d20   Response..from 
+00003040: 656c 6c61 722e 7361 6d70 6c65 732e 6d6f  ellar.samples.mo
+00003050: 6475 6c65 7320 696d 706f 7274 2048 6f6d  dules import Hom
+00003060: 654d 6f64 756c 650a 6672 6f6d 202e 6170  eModule.from .ap
+00003070: 7073 2e63 6172 2e6d 6f64 756c 6520 696d  ps.car.module im
+00003080: 706f 7274 2043 6172 4d6f 6475 6c65 0a0a  port CarModule..
+00003090: 0a40 4d6f 6475 6c65 286d 6f64 756c 6573  .@Module(modules
+000030a0: 3d5b 486f 6d65 4d6f 6475 6c65 2c20 4361  =[HomeModule, Ca
+000030b0: 724d 6f64 756c 655d 290a 636c 6173 7320  rModule]).class 
+000030c0: 4170 706c 6963 6174 696f 6e4d 6f64 756c  ApplicationModul
+000030d0: 6528 4d6f 6475 6c65 4261 7365 293a 0a20  e(ModuleBase):. 
+000030e0: 2020 2040 6578 6365 7074 696f 6e5f 6861     @exception_ha
+000030f0: 6e64 6c65 7228 3430 3429 0a20 2020 2064  ndler(404).    d
+00003100: 6566 2065 7863 6570 7469 6f6e 5f34 3034  ef exception_404
+00003110: 5f68 616e 646c 6572 2863 6c73 2c20 636f  _handler(cls, co
+00003120: 6e74 6578 743a 2049 486f 7374 436f 6e74  ntext: IHostCont
+00003130: 6578 742c 2065 7863 3a20 4578 6365 7074  ext, exc: Except
+00003140: 696f 6e29 202d 3e20 5265 7370 6f6e 7365  ion) -> Response
+00003150: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00003160: 204a 534f 4e52 6573 706f 6e73 6528 6469   JSONResponse(di
+00003170: 6374 2864 6574 6169 6c3d 2252 6573 6f75  ct(detail="Resou
+00003180: 7263 6520 6e6f 7420 666f 756e 642e 2229  rce not found.")
+00003190: 290a 0a60 6060 0a23 2320 456e 6162 6c69  )..```.## Enabli
+000031a0: 6e67 204f 7065 6e41 5049 2044 6f63 730a  ng OpenAPI Docs.
+000031b0: 546f 2073 7461 7274 2075 7020 6f70 656e  To start up open
+000031c0: 6170 692c 2077 6520 6e65 6564 2074 6f20  api, we need to 
+000031d0: 676f 2062 6163 6b20 746f 2070 726f 6a65  go back to proje
+000031e0: 6374 2066 6f6c 6465 7220 696e 2074 6865  ct folder in the
+000031f0: 2060 7365 7276 6572 2e70 7960 0a74 6865   `server.py`.the
+00003200: 6e20 6164 6420 7468 6520 666f 6c6c 6f77  n add the follow
+00003210: 696e 6720 6265 6c6f 772e 0a60 6060 7079  ing below..```py
+00003220: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a0a  thon.import os..
+00003230: 6672 6f6d 2065 6c6c 6172 2e63 6f6e 7374  from ellar.const
+00003240: 616e 7473 2069 6d70 6f72 7420 454c 4c41  ants import ELLA
+00003250: 525f 434f 4e46 4947 5f4d 4f44 554c 450a  R_CONFIG_MODULE.
+00003260: 6672 6f6d 2065 6c6c 6172 2e63 6f72 652e  from ellar.core.
+00003270: 6661 6374 6f72 7920 696d 706f 7274 2041  factory import A
+00003280: 7070 4661 6374 6f72 790a 6672 6f6d 2065  ppFactory.from e
+00003290: 6c6c 6172 2e6f 7065 6e61 7069 2069 6d70  llar.openapi imp
+000032a0: 6f72 7420 4f70 656e 4150 4944 6f63 756d  ort OpenAPIDocum
+000032b0: 656e 744d 6f64 756c 652c 204f 7065 6e41  entModule, OpenA
+000032c0: 5049 446f 6375 6d65 6e74 4275 696c 6465  PIDocumentBuilde
+000032d0: 722c 2053 7761 6767 6572 446f 6375 6d65  r, SwaggerDocume
+000032e0: 6e74 4765 6e65 7261 746f 720a 6672 6f6d  ntGenerator.from
+000032f0: 202e 726f 6f74 5f6d 6f64 756c 6520 696d   .root_module im
+00003300: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
+00003310: 4d6f 6475 6c65 0a0a 6170 706c 6963 6174  Module..applicat
+00003320: 696f 6e20 3d20 4170 7046 6163 746f 7279  ion = AppFactory
+00003330: 2e63 7265 6174 655f 6672 6f6d 5f61 7070  .create_from_app
+00003340: 5f6d 6f64 756c 6528 0a20 2020 2041 7070  _module(.    App
+00003350: 6c69 6361 7469 6f6e 4d6f 6475 6c65 2c0a  licationModule,.
+00003360: 2020 2020 636f 6e66 6967 5f6d 6f64 756c      config_modul
+00003370: 653d 6f73 2e65 6e76 6972 6f6e 2e67 6574  e=os.environ.get
+00003380: 280a 2020 2020 2020 2020 454c 4c41 525f  (.        ELLAR_
+00003390: 434f 4e46 4947 5f4d 4f44 554c 452c 2022  CONFIG_MODULE, "
+000033a0: 6361 7273 6974 652e 636f 6e66 6967 3a44  carsite.config:D
+000033b0: 6576 656c 6f70 6d65 6e74 436f 6e66 6967  evelopmentConfig
+000033c0: 220a 2020 2020 292c 0a29 0a0a 646f 6375  ".    ),.)..docu
+000033d0: 6d65 6e74 5f62 7569 6c64 6572 203d 204f  ment_builder = O
+000033e0: 7065 6e41 5049 446f 6375 6d65 6e74 4275  penAPIDocumentBu
+000033f0: 696c 6465 7228 290a 646f 6375 6d65 6e74  ilder().document
+00003400: 5f62 7569 6c64 6572 2e73 6574 5f74 6974  _builder.set_tit
+00003410: 6c65 2827 4361 7253 6974 6520 4150 4927  le('CarSite API'
+00003420: 2920 5c0a 2020 2020 2e73 6574 5f76 6572  ) \.    .set_ver
+00003430: 7369 6f6e 2827 312e 302e 3027 2920 5c0a  sion('1.0.0') \.
+00003440: 2020 2020 2e73 6574 5f63 6f6e 7461 6374      .set_contact
+00003450: 286e 616d 653d 2745 6164 7769 6e27 2c20  (name='Eadwin', 
+00003460: 7572 6c3d 2768 7474 7073 3a2f 2f77 7777  url='https://www
+00003470: 2e79 6168 6f6f 2e63 6f6d 272c 2065 6d61  .yahoo.com', ema
+00003480: 696c 3d27 6561 6477 696e 4067 6d61 696c  il='eadwin@gmail
+00003490: 2e63 6f6d 2729 205c 0a20 2020 202e 7365  .com') \.    .se
+000034a0: 745f 6c69 6365 6e73 6528 274d 4954 204c  t_license('MIT L
+000034b0: 6963 656e 6365 272c 2075 726c 3d27 6874  icence', url='ht
+000034c0: 7470 733a 2f2f 7777 772e 676f 6f67 6c65  tps://www.google
+000034d0: 2e63 6f6d 2729 0a0a 646f 6375 6d65 6e74  .com')..document
+000034e0: 203d 2064 6f63 756d 656e 745f 6275 696c   = document_buil
+000034f0: 6465 722e 6275 696c 645f 646f 6375 6d65  der.build_docume
+00003500: 6e74 2861 7070 6c69 6361 7469 6f6e 290a  nt(application).
+00003510: 6d6f 6475 6c65 203d 204f 7065 6e41 5049  module = OpenAPI
+00003520: 446f 6375 6d65 6e74 4d6f 6475 6c65 2e73  DocumentModule.s
+00003530: 6574 7570 280a 2020 2020 646f 6375 6d65  etup(.    docume
+00003540: 6e74 3d64 6f63 756d 656e 742c 0a20 2020  nt=document,.   
+00003550: 2064 6f63 756d 656e 745f 6765 6e65 7261   document_genera
+00003560: 746f 723d 5377 6167 6765 7244 6f63 756d  tor=SwaggerDocum
+00003570: 656e 7447 656e 6572 6174 6f72 2829 2c0a  entGenerator(),.
+00003580: 2020 2020 6775 6172 6473 3d5b 5d0a 290a      guards=[].).
+00003590: 6170 706c 6963 6174 696f 6e2e 696e 7374  application.inst
+000035a0: 616c 6c5f 6d6f 6475 6c65 286d 6f64 756c  all_module(modul
+000035b0: 6529 0a60 6060 0a0a 4e6f 7720 7765 2063  e).```..Now we c
+000035c0: 616e 2074 6573 7420 6f75 7220 4150 4920  an test our API 
+000035d0: 6174 205b 6874 7470 3a2f 2f31 3237 2e30  at [http://127.0
+000035e0: 2e30 2e31 3a38 3030 302f 646f 6373 5d28  .0.1:8000/docs](
+000035f0: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
+00003600: 3a38 3030 302f 646f 6373 232f 290a 506c  :8000/docs#/).Pl
+00003610: 6561 7365 2065 6e73 7572 6520 796f 7572  ease ensure your
+00003620: 2073 6572 7665 7220 6973 2072 756e 6e69   server is runni
+00003630: 6e67 0a21 5b53 7761 6767 6572 2055 495d  ng.![Swagger UI]
+00003640: 2864 6f63 732f 696d 672f 6361 725f 6170  (docs/img/car_ap
+00003650: 692e 706e 6729 0a0a 2323 2048 544d 4c20  i.png)..## HTML 
+00003660: 5465 6d70 6c61 7469 6e67 0a45 6c6c 6172  Templating.Ellar
+00003670: 2068 6173 2062 7569 6c74 2d69 6e20 7375   has built-in su
+00003680: 7070 6f72 7420 666f 7220 4a69 6e6a 6132  pport for Jinja2
+00003690: 2c20 7768 6963 6820 6973 2061 2070 6f70  , which is a pop
+000036a0: 756c 6172 2074 656d 706c 6174 6520 656e  ular template en
+000036b0: 6769 6e65 2066 6f72 2048 544d 4c2e 2054  gine for HTML. T
+000036c0: 6869 7320 6665 6174 7572 6520 616c 6c6f  his feature allo
+000036d0: 7773 2066 6f72 2065 6173 7920 616e 6420  ws for easy and 
+000036e0: 6566 6669 6369 656e 7420 4854 4d4c 2074  efficient HTML t
+000036f0: 656d 706c 6174 696e 6720 7369 6d69 6c61  emplating simila
+00003700: 7220 746f 2074 6861 7420 6f66 2046 6c61  r to that of Fla
+00003710: 736b 2e20 4a69 6e6a 6132 2063 616e 2062  sk. Jinja2 can b
+00003720: 6520 7573 6564 2074 6f20 6372 6561 7465  e used to create
+00003730: 2072 6575 7361 626c 6520 7465 6d70 6c61   reusable templa
+00003740: 7465 732c 2061 6e64 2074 6f20 696e 7365  tes, and to inse
+00003750: 7274 2064 796e 616d 6963 2064 6174 6120  rt dynamic data 
+00003760: 696e 746f 2048 544d 4c20 7061 6765 732e  into HTML pages.
+00003770: 2049 7420 616c 736f 2068 6173 2073 7570   It also has sup
+00003780: 706f 7274 2066 6f72 2074 656d 706c 6174  port for templat
+00003790: 6520 696e 6865 7269 7461 6e63 652c 2063  e inheritance, c
+000037a0: 6f6e 7472 6f6c 2073 7472 7563 7475 7265  ontrol structure
+000037b0: 732c 2061 6e64 206f 7468 6572 2075 7365  s, and other use
+000037c0: 6675 6c20 6665 6174 7572 6573 2074 6861  ful features tha
+000037d0: 7420 6361 6e20 6865 6c70 2074 6f20 7369  t can help to si
+000037e0: 6d70 6c69 6679 2061 6e64 2073 7472 6561  mplify and strea
+000037f0: 6d6c 696e 6520 7468 6520 7072 6f63 6573  mline the proces
+00003800: 7320 6f66 2063 7265 6174 696e 6720 4854  s of creating HT
+00003810: 4d4c 2074 656d 706c 6174 6573 2e0a 0a60  ML templates...`
+00003820: 6060 6874 6d6c 0a3c 6874 6d6c 3e0a 2020  ``html.<html>.  
+00003830: 3c62 6f64 793e 0a20 2020 203c 756c 3e0a  <body>.    <ul>.
+00003840: 2020 2020 2020 7b25 2066 6f72 2069 7465        {% for ite
+00003850: 6d20 696e 2069 7465 6d73 2025 7d0a 2020  m in items %}.  
+00003860: 2020 2020 3c6c 693e 7b7b 2069 7465 6d20      <li>{{ item 
+00003870: 7d7d 3c2f 6c69 3e0a 2020 2020 2020 7b25  }}</li>.      {%
+00003880: 2065 6e64 666f 7220 257d 0a20 2020 203c   endfor %}.    <
+00003890: 2f75 6c3e 0a20 203c 2f62 6f64 793e 0a3c  /ul>.  </body>.<
+000038a0: 2f68 746d 6c3e 0a60 6060 0a0a 5365 6520  /html>.```..See 
+000038b0: 7468 6520 5b44 6f63 5d28 6874 7470 733a  the [Doc](https:
+000038c0: 2f2f 6561 6477 696e 636f 6465 2e67 6974  //eadwincode.git
+000038d0: 6875 622e 696f 2f65 6c6c 6172 2f74 656d  hub.io/ellar/tem
+000038e0: 706c 6174 696e 672f 7465 6d70 6c61 7469  plating/templati
+000038f0: 6e67 2f29 2066 6f72 206d 6f72 6520 6578  ng/) for more ex
+00003900: 616d 706c 6573 2e0a 0a23 2320 5072 6f6a  amples...## Proj
+00003910: 6563 7420 5374 6174 7573 0a50 726f 6a65  ect Status.Proje
+00003920: 6374 2069 7320 7374 696c 6c20 696e 2064  ct is still in d
+00003930: 6576 656c 6f70 6d65 6e74 0a2d 2044 6f63  evelopment.- Doc
+00003940: 756d 656e 7461 7469 6f6e 202d 2028 696e  umentation - (in
+00003950: 2070 726f 6772 6573 7329 0a2d 2049 6e74   progress).- Int
+00003960: 6572 6365 7074 6f72 7320 202d 2020 5b41  erceptors  -  [A
+00003970: 7370 6563 7420 4f72 6965 6e74 6564 2050  spect Oriented P
+00003980: 726f 6772 616d 6d69 6e67 5d28 6874 7470  rogramming](http
+00003990: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+000039a0: 2e6f 7267 2f77 696b 692f 4173 7065 6374  .org/wiki/Aspect
+000039b0: 2d6f 7269 656e 7465 645f 7072 6f67 7261  -oriented_progra
+000039c0: 6d6d 696e 6729 2028 414f 5029 2074 6563  mming) (AOP) tec
+000039d0: 686e 6971 7565 0a2d 2044 6174 6162 6173  hnique.- Databas
+000039e0: 6520 506c 7567 696e 2077 6974 6820 5b45  e Plugin with [E
+000039f0: 6e63 6f64 652f 4f52 4d5d 2868 7474 7073  ncode/ORM](https
+00003a00: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
+00003a10: 636f 6465 2f6f 726d 290a 0a              code/orm)..
```

