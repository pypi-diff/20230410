# Comparing `tmp/loguru-0.6.0.tar.gz` & `tmp/loguru-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loguru-0.6.0.tar", last modified: Sat Jan 29 13:46:22 2022, max compression
+gzip compressed data, was "loguru-0.7.0.tar", last modified: Mon Apr 10 09:00:17 2023, max compression
```

## Comparing `loguru-0.6.0.tar` & `loguru-0.7.0.tar`

### file list

```diff
@@ -1,247 +1,253 @@
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.306522 loguru-0.6.0/
--rw-r--r--   0 delgan    (1000) users      (985)     1057 2019-05-06 19:50:53.000000 loguru-0.6.0/LICENSE
--rw-r--r--   0 delgan    (1000) users      (985)       51 2020-04-24 17:19:57.000000 loguru-0.6.0/MANIFEST.in
--rw-r--r--   0 delgan    (1000) users      (985)    20315 2022-01-29 13:46:22.306522 loguru-0.6.0/PKG-INFO
--rw-r--r--   0 delgan    (1000) users      (985)    18849 2022-01-29 13:42:43.000000 loguru-0.6.0/README.rst
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.889854 loguru-0.6.0/loguru/
--rw-r--r--   0 delgan    (1000) users      (985)      627 2022-01-29 13:36:34.000000 loguru-0.6.0/loguru/__init__.py
--rw-r--r--   0 delgan    (1000) users      (985)    13585 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/__init__.pyi
--rw-r--r--   0 delgan    (1000) users      (985)      597 2022-01-24 09:18:54.000000 loguru-0.6.0/loguru/_asyncio_loop.py
--rw-r--r--   0 delgan    (1000) users      (985)    15946 2022-01-20 12:32:57.000000 loguru-0.6.0/loguru/_better_exceptions.py
--rw-r--r--   0 delgan    (1000) users      (985)      760 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_colorama.py
--rw-r--r--   0 delgan    (1000) users      (985)    14587 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_colorizer.py
--rw-r--r--   0 delgan    (1000) users      (985)      321 2022-01-20 17:37:05.000000 loguru-0.6.0/loguru/_contextvars.py
--rw-r--r--   0 delgan    (1000) users      (985)     1331 2022-01-20 17:37:05.000000 loguru-0.6.0/loguru/_ctime_functions.py
--rw-r--r--   0 delgan    (1000) users      (985)     3165 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_datetime.py
--rw-r--r--   0 delgan    (1000) users      (985)     2840 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_defaults.py
--rw-r--r--   0 delgan    (1000) users      (985)     1107 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_error_interceptor.py
--rw-r--r--   0 delgan    (1000) users      (985)    12714 2022-01-24 10:14:42.000000 loguru-0.6.0/loguru/_file_sink.py
--rw-r--r--   0 delgan    (1000) users      (985)      618 2021-03-19 15:18:07.000000 loguru-0.6.0/loguru/_filters.py
--rw-r--r--   0 delgan    (1000) users      (985)      458 2022-01-20 17:37:05.000000 loguru-0.6.0/loguru/_get_frame.py
--rw-r--r--   0 delgan    (1000) users      (985)    11164 2022-01-24 09:41:39.000000 loguru-0.6.0/loguru/_handler.py
--rw-r--r--   0 delgan    (1000) users      (985)     1307 2022-01-20 17:37:05.000000 loguru-0.6.0/loguru/_locks_machinery.py
--rw-r--r--   0 delgan    (1000) users      (985)    93071 2022-01-28 07:37:02.000000 loguru-0.6.0/loguru/_logger.py
--rw-r--r--   0 delgan    (1000) users      (985)     2174 2022-01-24 09:18:54.000000 loguru-0.6.0/loguru/_recattrs.py
--rw-r--r--   0 delgan    (1000) users      (985)     3160 2022-01-24 09:18:54.000000 loguru-0.6.0/loguru/_simple_sinks.py
--rw-r--r--   0 delgan    (1000) users      (985)     4709 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/_string_parsers.py
--rw-r--r--   0 delgan    (1000) users      (985)        0 2021-03-13 14:44:16.000000 loguru-0.6.0/loguru/py.typed
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.896521 loguru-0.6.0/loguru.egg-info/
--rw-r--r--   0 delgan    (1000) users      (985)    20315 2022-01-29 13:46:21.000000 loguru-0.6.0/loguru.egg-info/PKG-INFO
--rw-r--r--   0 delgan    (1000) users      (985)    10604 2022-01-29 13:46:21.000000 loguru-0.6.0/loguru.egg-info/SOURCES.txt
--rw-r--r--   0 delgan    (1000) users      (985)        1 2022-01-29 13:46:21.000000 loguru-0.6.0/loguru.egg-info/dependency_links.txt
--rw-r--r--   0 delgan    (1000) users      (985)      331 2022-01-29 13:46:21.000000 loguru-0.6.0/loguru.egg-info/requires.txt
--rw-r--r--   0 delgan    (1000) users      (985)        7 2022-01-29 13:46:21.000000 loguru-0.6.0/loguru.egg-info/top_level.txt
--rw-r--r--   0 delgan    (1000) users      (985)       38 2022-01-29 13:46:22.306522 loguru-0.6.0/setup.cfg
--rw-r--r--   0 delgan    (1000) users      (985)     2714 2022-01-21 20:50:01.000000 loguru-0.6.0/setup.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.963188 loguru-0.6.0/tests/
--rw-r--r--   0 delgan    (1000) users      (985)        0 2019-11-11 21:50:18.000000 loguru-0.6.0/tests/__init__.py
--rw-r--r--   0 delgan    (1000) users      (985)     4698 2022-01-20 17:37:05.000000 loguru-0.6.0/tests/conftest.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.853188 loguru-0.6.0/tests/exceptions/
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.853188 loguru-0.6.0/tests/exceptions/output/
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.996521 loguru-0.6.0/tests/exceptions/output/backtrace/
--rw-r--r--   0 delgan    (1000) users      (985)     1990 2022-01-19 18:34:46.000000 loguru-0.6.0/tests/exceptions/output/backtrace/chained_expression_direct.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1636 2022-01-19 18:34:46.000000 loguru-0.6.0/tests/exceptions/output/backtrace/chained_expression_indirect.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1327 2022-01-19 18:34:46.000000 loguru-0.6.0/tests/exceptions/output/backtrace/chaining_first.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1409 2022-01-19 18:34:46.000000 loguru-0.6.0/tests/exceptions/output/backtrace/chaining_second.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1467 2022-01-19 18:34:46.000000 loguru-0.6.0/tests/exceptions/output/backtrace/chaining_third.txt
--rw-r--r--   0 delgan    (1000) users      (985)      157 2022-01-19 18:34:47.000000 loguru-0.6.0/tests/exceptions/output/backtrace/enqueue.txt
--rw-r--r--   0 delgan    (1000) users      (985)      179 2022-01-19 18:34:47.000000 loguru-0.6.0/tests/exceptions/output/backtrace/enqueue_with_others_handlers.txt
--rw-r--r--   0 delgan    (1000) users      (985)      456 2022-01-19 18:34:47.000000 loguru-0.6.0/tests/exceptions/output/backtrace/frame_values_backward.txt
--rw-r--r--   0 delgan    (1000) users      (985)      452 2022-01-19 18:34:47.000000 loguru-0.6.0/tests/exceptions/output/backtrace/frame_values_forward.txt
--rw-r--r--   0 delgan    (1000) users      (985)      711 2022-01-19 18:34:47.000000 loguru-0.6.0/tests/exceptions/output/backtrace/function.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3852 2022-01-19 18:34:48.000000 loguru-0.6.0/tests/exceptions/output/backtrace/head_recursion.txt
--rw-r--r--   0 delgan    (1000) users      (985)      411 2022-01-19 18:34:48.000000 loguru-0.6.0/tests/exceptions/output/backtrace/missing_attributes_traceback_objects.txt
--rw-r--r--   0 delgan    (1000) users      (985)      963 2022-01-19 18:34:48.000000 loguru-0.6.0/tests/exceptions/output/backtrace/nested.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1428 2022-01-19 18:34:48.000000 loguru-0.6.0/tests/exceptions/output/backtrace/nested_chained_catch_up.txt
--rw-r--r--   0 delgan    (1000) users      (985)      748 2022-01-19 18:34:48.000000 loguru-0.6.0/tests/exceptions/output/backtrace/nested_decorator_catch_up.txt
--rw-r--r--   0 delgan    (1000) users      (985)      742 2022-01-19 18:34:49.000000 loguru-0.6.0/tests/exceptions/output/backtrace/nested_explicit_catch_up.txt
--rw-r--r--   0 delgan    (1000) users      (985)      842 2022-01-19 18:34:49.000000 loguru-0.6.0/tests/exceptions/output/backtrace/nested_wrapping.txt
--rw-r--r--   0 delgan    (1000) users      (985)       42 2022-01-19 18:34:49.000000 loguru-0.6.0/tests/exceptions/output/backtrace/no_tb.txt
--rw-r--r--   0 delgan    (1000) users      (985)      670 2022-01-19 18:34:49.000000 loguru-0.6.0/tests/exceptions/output/backtrace/not_enough_arguments.txt
--rw-r--r--   0 delgan    (1000) users      (985)     9672 2022-01-19 18:34:49.000000 loguru-0.6.0/tests/exceptions/output/backtrace/raising_recursion.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2356 2022-01-19 18:34:50.000000 loguru-0.6.0/tests/exceptions/output/backtrace/suppressed_expression_direct.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2278 2022-01-19 18:34:50.000000 loguru-0.6.0/tests/exceptions/output/backtrace/suppressed_expression_indirect.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3852 2022-01-19 18:34:50.000000 loguru-0.6.0/tests/exceptions/output/backtrace/tail_recursion.txt
--rw-r--r--   0 delgan    (1000) users      (985)      640 2022-01-19 18:34:50.000000 loguru-0.6.0/tests/exceptions/output/backtrace/too_many_arguments.txt
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.016521 loguru-0.6.0/tests/exceptions/output/diagnose/
--rw-r--r--   0 delgan    (1000) users      (985)      800 2022-01-19 18:34:50.000000 loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error.txt
--rw-r--r--   0 delgan    (1000) users      (985)      760 2022-01-19 18:34:51.000000 loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error_custom.txt
--rw-r--r--   0 delgan    (1000) users      (985)      588 2022-01-19 18:34:51.000000 loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error_in_string.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1931 2022-01-19 18:34:51.000000 loguru-0.6.0/tests/exceptions/output/diagnose/attributes.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2027 2022-01-19 18:34:51.000000 loguru-0.6.0/tests/exceptions/output/diagnose/chained_both.txt
--rw-r--r--   0 delgan    (1000) users      (985)      820 2022-01-19 18:34:51.000000 loguru-0.6.0/tests/exceptions/output/diagnose/encoding.txt
--rw-r--r--   0 delgan    (1000) users      (985)      712 2022-01-19 18:34:52.000000 loguru-0.6.0/tests/exceptions/output/diagnose/global_variable.txt
--rw-r--r--   0 delgan    (1000) users      (985)      502 2022-01-19 18:34:52.000000 loguru-0.6.0/tests/exceptions/output/diagnose/indentation_error.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1232 2022-01-19 18:34:52.000000 loguru-0.6.0/tests/exceptions/output/diagnose/keyword_argument.txt
--rw-r--r--   0 delgan    (1000) users      (985)      780 2022-01-19 18:34:52.000000 loguru-0.6.0/tests/exceptions/output/diagnose/multilines_repr.txt
--rw-r--r--   0 delgan    (1000) users      (985)      696 2022-01-19 18:34:53.000000 loguru-0.6.0/tests/exceptions/output/diagnose/no_error_message.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3109 2022-01-19 18:34:53.000000 loguru-0.6.0/tests/exceptions/output/diagnose/parenthesis.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2589 2022-01-19 18:34:53.000000 loguru-0.6.0/tests/exceptions/output/diagnose/source_multilines.txt
--rw-r--r--   0 delgan    (1000) users      (985)      543 2022-01-19 18:34:53.000000 loguru-0.6.0/tests/exceptions/output/diagnose/source_strings.txt
--rw-r--r--   0 delgan    (1000) users      (985)      393 2022-01-19 18:34:53.000000 loguru-0.6.0/tests/exceptions/output/diagnose/syntax_error.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2717 2022-01-19 18:34:54.000000 loguru-0.6.0/tests/exceptions/output/diagnose/syntax_highlighting.txt
--rw-r--r--   0 delgan    (1000) users      (985)      695 2022-01-19 18:34:54.000000 loguru-0.6.0/tests/exceptions/output/diagnose/truncating.txt
--rw-r--r--   0 delgan    (1000) users      (985)      368 2022-01-19 18:34:54.000000 loguru-0.6.0/tests/exceptions/output/diagnose/unprintable_object.txt
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.186521 loguru-0.6.0/tests/exceptions/output/others/
--rw-r--r--   0 delgan    (1000) users      (985)      116 2022-01-19 18:34:57.000000 loguru-0.6.0/tests/exceptions/output/others/assertionerror_without_traceback.txt
--rw-r--r--   0 delgan    (1000) users      (985)      172 2022-01-19 18:34:57.000000 loguru-0.6.0/tests/exceptions/output/others/catch_as_context_manager.txt
--rw-r--r--   0 delgan    (1000) users      (985)      291 2022-01-19 18:34:57.000000 loguru-0.6.0/tests/exceptions/output/others/catch_as_decorator_with_parentheses.txt
--rw-r--r--   0 delgan    (1000) users      (985)      292 2022-01-19 18:34:57.000000 loguru-0.6.0/tests/exceptions/output/others/catch_as_decorator_without_parentheses.txt
--rw-r--r--   0 delgan    (1000) users      (985)      249 2022-01-19 18:34:57.000000 loguru-0.6.0/tests/exceptions/output/others/catch_as_function.txt
--rw-r--r--   0 delgan    (1000) users      (985)      526 2022-01-19 18:34:58.000000 loguru-0.6.0/tests/exceptions/output/others/catch_message.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1394 2022-01-19 18:34:58.000000 loguru-0.6.0/tests/exceptions/output/others/exception_formatting_coroutine.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1236 2022-01-19 18:34:58.000000 loguru-0.6.0/tests/exceptions/output/others/exception_formatting_function.txt
--rw-r--r--   0 delgan    (1000) users      (985)     1330 2022-01-19 18:34:58.000000 loguru-0.6.0/tests/exceptions/output/others/exception_formatting_generator.txt
--rw-r--r--   0 delgan    (1000) users      (985)      378 2022-01-19 18:34:58.000000 loguru-0.6.0/tests/exceptions/output/others/exception_in_property.txt
--rw-r--r--   0 delgan    (1000) users      (985)      236 2022-01-21 20:50:01.000000 loguru-0.6.0/tests/exceptions/output/others/handler_formatting_with_context_manager.txt
--rw-r--r--   0 delgan    (1000) users      (985)      338 2022-01-19 18:34:59.000000 loguru-0.6.0/tests/exceptions/output/others/handler_formatting_with_decorator.txt
--rw-r--r--   0 delgan    (1000) users      (985)      161 2022-01-19 18:34:59.000000 loguru-0.6.0/tests/exceptions/output/others/level_name.txt
--rw-r--r--   0 delgan    (1000) users      (985)      166 2022-01-19 18:34:59.000000 loguru-0.6.0/tests/exceptions/output/others/level_number.txt
--rw-r--r--   0 delgan    (1000) users      (985)      236 2022-01-21 20:50:01.000000 loguru-0.6.0/tests/exceptions/output/others/message_formatting_with_context_manager.txt
--rw-r--r--   0 delgan    (1000) users      (985)      338 2022-01-19 18:35:00.000000 loguru-0.6.0/tests/exceptions/output/others/message_formatting_with_decorator.txt
--rw-r--r--   0 delgan    (1000) users      (985)     4582 2022-01-19 18:35:00.000000 loguru-0.6.0/tests/exceptions/output/others/nested_with_reraise.txt
--rw-r--r--   0 delgan    (1000) users      (985)      388 2022-01-19 18:35:00.000000 loguru-0.6.0/tests/exceptions/output/others/syntaxerror_without_traceback.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2356 2022-01-19 18:35:00.000000 loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit.txt
--rw-r--r--   0 delgan    (1000) users      (985)      148 2022-01-19 18:35:01.000000 loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit_negative.txt
--rw-r--r--   0 delgan    (1000) users      (985)     5076 2022-01-19 18:35:01.000000 loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit_none.txt
--rw-r--r--   0 delgan    (1000) users      (985)     5120 2022-01-19 18:35:01.000000 loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit_unset.txt
--rw-r--r--   0 delgan    (1000) users      (985)      232 2022-01-19 18:35:02.000000 loguru-0.6.0/tests/exceptions/output/others/zerodivisionerror_without_traceback.txt
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.203188 loguru-0.6.0/tests/exceptions/output/ownership/
--rw-r--r--   0 delgan    (1000) users      (985)     2964 2022-01-19 18:34:54.000000 loguru-0.6.0/tests/exceptions/output/ownership/assertion_from_lib.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2204 2022-01-19 18:34:54.000000 loguru-0.6.0/tests/exceptions/output/ownership/assertion_from_local.txt
--rw-r--r--   0 delgan    (1000) users      (985)     4172 2022-01-19 18:34:55.000000 loguru-0.6.0/tests/exceptions/output/ownership/callback.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3478 2022-01-19 18:34:55.000000 loguru-0.6.0/tests/exceptions/output/ownership/catch_decorator.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3740 2022-01-19 18:34:55.000000 loguru-0.6.0/tests/exceptions/output/ownership/catch_decorator_from_lib.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3127 2022-01-19 18:34:55.000000 loguru-0.6.0/tests/exceptions/output/ownership/decorated_callback.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2573 2022-01-19 18:34:56.000000 loguru-0.6.0/tests/exceptions/output/ownership/direct.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3268 2022-01-19 18:34:56.000000 loguru-0.6.0/tests/exceptions/output/ownership/indirect.txt
--rw-r--r--   0 delgan    (1000) users      (985)     3095 2022-01-19 18:34:56.000000 loguru-0.6.0/tests/exceptions/output/ownership/string_lib.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2922 2022-01-19 18:34:56.000000 loguru-0.6.0/tests/exceptions/output/ownership/string_source.txt
--rw-r--r--   0 delgan    (1000) users      (985)     2693 2022-01-19 18:34:56.000000 loguru-0.6.0/tests/exceptions/output/ownership/syntaxerror.txt
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.853188 loguru-0.6.0/tests/exceptions/source/
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.239855 loguru-0.6.0/tests/exceptions/source/backtrace/
--rw-r--r--   0 delgan    (1000) users      (985)      642 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/chained_expression_direct.py
--rw-r--r--   0 delgan    (1000) users      (985)      360 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/chained_expression_indirect.py
--rw-r--r--   0 delgan    (1000) users      (985)      393 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/chaining_first.py
--rw-r--r--   0 delgan    (1000) users      (985)      516 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/chaining_second.py
--rw-r--r--   0 delgan    (1000) users      (985)      624 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/chaining_third.py
--rw-r--r--   0 delgan    (1000) users      (985)      223 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/enqueue.py
--rw-r--r--   0 delgan    (1000) users      (985)      618 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/enqueue_with_others_handlers.py
--rw-r--r--   0 delgan    (1000) users      (985)      237 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/frame_values_backward.py
--rw-r--r--   0 delgan    (1000) users      (985)      237 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/frame_values_forward.py
--rw-r--r--   0 delgan    (1000) users      (985)      317 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/function.py
--rw-r--r--   0 delgan    (1000) users      (985)      466 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/head_recursion.py
--rw-r--r--   0 delgan    (1000) users      (985)     1020 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/missing_attributes_traceback_objects.py
--rw-r--r--   0 delgan    (1000) users      (985)      457 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/nested.py
--rw-r--r--   0 delgan    (1000) users      (985)      418 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/nested_chained_catch_up.py
--rw-r--r--   0 delgan    (1000) users      (985)      342 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/nested_decorator_catch_up.py
--rw-r--r--   0 delgan    (1000) users      (985)      369 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/nested_explicit_catch_up.py
--rw-r--r--   0 delgan    (1000) users      (985)      409 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/nested_wrapping.py
--rw-r--r--   0 delgan    (1000) users      (985)      335 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/no_tb.py
--rw-r--r--   0 delgan    (1000) users      (985)      353 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/not_enough_arguments.py
--rw-r--r--   0 delgan    (1000) users      (985)      464 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/raising_recursion.py
--rw-r--r--   0 delgan    (1000) users      (985)      693 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/suppressed_expression_direct.py
--rw-r--r--   0 delgan    (1000) users      (985)      480 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/suppressed_expression_indirect.py
--rw-r--r--   0 delgan    (1000) users      (985)      408 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/tail_recursion.py
--rw-r--r--   0 delgan    (1000) users      (985)      339 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/backtrace/too_many_arguments.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.263188 loguru-0.6.0/tests/exceptions/source/diagnose/
--rw-r--r--   0 delgan    (1000) users      (985)      261 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/assertion_error.py
--rw-r--r--   0 delgan    (1000) users      (985)      285 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/assertion_error_custom.py
--rw-r--r--   0 delgan    (1000) users      (985)      269 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/assertion_error_in_string.py
--rw-r--r--   0 delgan    (1000) users      (985)      431 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/attributes.py
--rw-r--r--   0 delgan    (1000) users      (985)      467 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/chained_both.py
--rw-r--r--   0 delgan    (1000) users      (985)      270 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/encoding.py
--rw-r--r--   0 delgan    (1000) users      (985)      296 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/global_variable.py
--rw-r--r--   0 delgan    (1000) users      (985)      316 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/indentation_error.py
--rw-r--r--   0 delgan    (1000) users      (985)      246 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/keyword_argument.py
--rw-r--r--   0 delgan    (1000) users      (985)      341 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/multilines_repr.py
--rw-r--r--   0 delgan    (1000) users      (985)      258 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/no_error_message.py
--rw-r--r--   0 delgan    (1000) users      (985)      627 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/parenthesis.py
--rw-r--r--   0 delgan    (1000) users      (985)      773 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/source_multilines.py
--rw-r--r--   0 delgan    (1000) users      (985)      261 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/source_strings.py
--rw-r--r--   0 delgan    (1000) users      (985)      251 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/syntax_error.py
--rw-r--r--   0 delgan    (1000) users      (985)      504 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/syntax_highlighting.py
--rw-r--r--   0 delgan    (1000) users      (985)      248 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/truncating.py
--rw-r--r--   0 delgan    (1000) users      (985)      307 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/diagnose/unprintable_object.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.286522 loguru-0.6.0/tests/exceptions/source/others/
--rw-r--r--   0 delgan    (1000) users      (985)      418 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/assertionerror_without_traceback.py
--rw-r--r--   0 delgan    (1000) users      (985)      171 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/catch_as_context_manager.py
--rw-r--r--   0 delgan    (1000) users      (985)      191 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/catch_as_decorator_with_parentheses.py
--rw-r--r--   0 delgan    (1000) users      (985)      186 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/catch_as_decorator_without_parentheses.py
--rw-r--r--   0 delgan    (1000) users      (985)      187 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/catch_as_function.py
--rw-r--r--   0 delgan    (1000) users      (985)      290 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/catch_message.py
--rw-r--r--   0 delgan    (1000) users      (985)      500 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/exception_formatting_coroutine.py
--rw-r--r--   0 delgan    (1000) users      (985)      432 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/exception_formatting_function.py
--rw-r--r--   0 delgan    (1000) users      (985)      495 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/exception_formatting_generator.py
--rw-r--r--   0 delgan    (1000) users      (985)      373 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/exception_in_property.py
--rw-r--r--   0 delgan    (1000) users      (985)      253 2022-01-20 12:33:10.000000 loguru-0.6.0/tests/exceptions/source/others/handler_formatting_with_context_manager.py
--rw-r--r--   0 delgan    (1000) users      (985)      238 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/handler_formatting_with_decorator.py
--rw-r--r--   0 delgan    (1000) users      (985)      238 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/level_name.py
--rw-r--r--   0 delgan    (1000) users      (985)      233 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/level_number.py
--rw-r--r--   0 delgan    (1000) users      (985)      295 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/message_formatting_with_context_manager.py
--rw-r--r--   0 delgan    (1000) users      (985)      268 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/message_formatting_with_decorator.py
--rw-r--r--   0 delgan    (1000) users      (985)      625 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/nested_with_reraise.py
--rw-r--r--   0 delgan    (1000) users      (985)      416 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/syntaxerror_without_traceback.py
--rw-r--r--   0 delgan    (1000) users      (985)      673 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit.py
--rw-r--r--   0 delgan    (1000) users      (985)      674 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_negative.py
--rw-r--r--   0 delgan    (1000) users      (985)      676 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_none.py
--rw-r--r--   0 delgan    (1000) users      (985)      714 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_unset.py
--rw-r--r--   0 delgan    (1000) users      (985)      414 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/others/zerodivisionerror_without_traceback.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.303188 loguru-0.6.0/tests/exceptions/source/ownership/
--rw-r--r--   0 delgan    (1000) users      (985)      208 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/_init.py
--rw-r--r--   0 delgan    (1000) users      (985)      629 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/assertion_from_lib.py
--rw-r--r--   0 delgan    (1000) users      (985)      622 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/assertion_from_local.py
--rw-r--r--   0 delgan    (1000) users      (985)      650 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/callback.py
--rw-r--r--   0 delgan    (1000) users      (985)      572 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/catch_decorator.py
--rw-r--r--   0 delgan    (1000) users      (985)      596 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/catch_decorator_from_lib.py
--rw-r--r--   0 delgan    (1000) users      (985)      609 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/decorated_callback.py
--rw-r--r--   0 delgan    (1000) users      (985)      597 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/direct.py
--rw-r--r--   0 delgan    (1000) users      (985)      615 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/indirect.py
--rw-r--r--   0 delgan    (1000) users      (985)      594 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/string_lib.py
--rw-r--r--   0 delgan    (1000) users      (985)      586 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/string_source.py
--rw-r--r--   0 delgan    (1000) users      (985)      596 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/exceptions/source/ownership/syntaxerror.py
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:21.853188 loguru-0.6.0/tests/exceptions/source/ownership/usersite/
-drwxr-xr-x   0 delgan    (1000) users      (985)        0 2022-01-29 13:46:22.303188 loguru-0.6.0/tests/exceptions/source/ownership/usersite/somelib/
--rw-r--r--   0 delgan    (1000) users      (985)      240 2021-03-13 14:44:16.000000 loguru-0.6.0/tests/exceptions/source/ownership/usersite/somelib/__init__.py
--rw-r--r--   0 delgan    (1000) users      (985)     3667 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_activation.py
--rw-r--r--   0 delgan    (1000) users      (985)      579 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_backtrace.py
--rw-r--r--   0 delgan    (1000) users      (985)     3718 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_catch.py
--rw-r--r--   0 delgan    (1000) users      (985)     6124 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_colorize.py
--rw-r--r--   0 delgan    (1000) users      (985)      576 2021-03-13 14:44:16.000000 loguru-0.6.0/tests/test_add_option_diagnose.py
--rw-r--r--   0 delgan    (1000) users      (985)     6368 2022-01-24 09:18:54.000000 loguru-0.6.0/tests/test_add_option_enqueue.py
--rw-r--r--   0 delgan    (1000) users      (985)     3427 2021-03-19 15:18:07.000000 loguru-0.6.0/tests/test_add_option_filter.py
--rw-r--r--   0 delgan    (1000) users      (985)     2590 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_format.py
--rw-r--r--   0 delgan    (1000) users      (985)     1641 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_kwargs.py
--rw-r--r--   0 delgan    (1000) users      (985)      815 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_add_option_level.py
--rw-r--r--   0 delgan    (1000) users      (985)     4171 2022-01-24 09:41:39.000000 loguru-0.6.0/tests/test_add_option_serialize.py
--rw-r--r--   0 delgan    (1000) users      (985)     5760 2022-01-24 10:14:42.000000 loguru-0.6.0/tests/test_add_sinks.py
--rw-r--r--   0 delgan    (1000) users      (985)     5597 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_ansimarkup_basic.py
--rw-r--r--   0 delgan    (1000) users      (985)     6370 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_ansimarkup_extended.py
--rw-r--r--   0 delgan    (1000) users      (985)     2046 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_bind.py
--rw-r--r--   0 delgan    (1000) users      (985)     5238 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_configure.py
--rw-r--r--   0 delgan    (1000) users      (985)     5606 2022-01-20 17:37:05.000000 loguru-0.6.0/tests/test_contextualize.py
--rw-r--r--   0 delgan    (1000) users      (985)    15009 2022-01-24 09:18:54.000000 loguru-0.6.0/tests/test_coroutine_sink.py
--rw-r--r--   0 delgan    (1000) users      (985)     5220 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_datetime.py
--rw-r--r--   0 delgan    (1000) users      (985)     1173 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_deepcopy.py
--rw-r--r--   0 delgan    (1000) users      (985)     1155 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_defaults.py
--rw-r--r--   0 delgan    (1000) users      (985)    10741 2022-01-24 09:18:54.000000 loguru-0.6.0/tests/test_exceptions_catch.py
--rw-r--r--   0 delgan    (1000) users      (985)     6876 2022-01-21 20:50:01.000000 loguru-0.6.0/tests/test_exceptions_formatting.py
--rw-r--r--   0 delgan    (1000) users      (985)    10155 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_filesink_compression.py
--rw-r--r--   0 delgan    (1000) users      (985)     3270 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_filesink_delay.py
--rw-r--r--   0 delgan    (1000) users      (985)    10394 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_filesink_retention.py
--rw-r--r--   0 delgan    (1000) users      (985)    21755 2022-01-20 17:37:05.000000 loguru-0.6.0/tests/test_filesink_rotation.py
--rw-r--r--   0 delgan    (1000) users      (985)     7023 2021-03-13 18:38:43.000000 loguru-0.6.0/tests/test_formatting.py
--rw-r--r--   0 delgan    (1000) users      (985)      818 2022-01-20 17:37:05.000000 loguru-0.6.0/tests/test_get_frame.py
--rw-r--r--   0 delgan    (1000) users      (985)     5190 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_interception.py
--rw-r--r--   0 delgan    (1000) users      (985)     6960 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_levels.py
--rw-r--r--   0 delgan    (1000) users      (985)    16673 2022-01-24 09:18:54.000000 loguru-0.6.0/tests/test_multiprocessing.py
--rw-r--r--   0 delgan    (1000) users      (985)    20870 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_opt.py
--rw-r--r--   0 delgan    (1000) users      (985)     4411 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_parse.py
--rw-r--r--   0 delgan    (1000) users      (985)     2050 2021-03-13 14:44:16.000000 loguru-0.6.0/tests/test_patch.py
--rw-r--r--   0 delgan    (1000) users      (985)    10202 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_pickling.py
--rw-r--r--   0 delgan    (1000) users      (985)     2725 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_propagation.py
--rw-r--r--   0 delgan    (1000) users      (985)     2158 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_recattr.py
--rw-r--r--   0 delgan    (1000) users      (985)     2678 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_remove.py
--rw-r--r--   0 delgan    (1000) users      (985)     5877 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_repr.py
--rw-r--r--   0 delgan    (1000) users      (985)     4822 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_standard_handler.py
--rw-r--r--   0 delgan    (1000) users      (985)     3696 2021-03-13 18:38:44.000000 loguru-0.6.0/tests/test_threading.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.477029 loguru-0.7.0/
+-rw-r--r--   0 delgan    (1000) users      (985)     1056 2022-08-08 09:02:07.000000 loguru-0.7.0/LICENSE
+-rw-r--r--   0 delgan    (1000) users      (985)       57 2022-08-08 09:02:07.000000 loguru-0.7.0/MANIFEST.in
+-rw-r--r--   0 delgan    (1000) users      (985)    20466 2023-04-10 09:00:17.477029 loguru-0.7.0/PKG-INFO
+-rw-r--r--   0 delgan    (1000) users      (985)    18969 2023-04-10 08:56:14.000000 loguru-0.7.0/README.rst
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.893695 loguru-0.7.0/loguru/
+-rw-r--r--   0 delgan    (1000) users      (985)      626 2023-04-10 08:50:51.000000 loguru-0.7.0/loguru/__init__.py
+-rw-r--r--   0 delgan    (1000) users      (985)    13934 2022-12-30 19:41:32.000000 loguru-0.7.0/loguru/__init__.pyi
+-rw-r--r--   0 delgan    (1000) users      (985)      597 2022-04-23 10:51:55.000000 loguru-0.7.0/loguru/_asyncio_loop.py
+-rw-r--r--   0 delgan    (1000) users      (985)    16003 2023-03-18 08:13:39.000000 loguru-0.7.0/loguru/_better_exceptions.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1431 2022-08-08 09:02:07.000000 loguru-0.7.0/loguru/_colorama.py
+-rw-r--r--   0 delgan    (1000) users      (985)    14601 2023-04-10 08:41:53.000000 loguru-0.7.0/loguru/_colorizer.py
+-rw-r--r--   0 delgan    (1000) users      (985)      321 2022-04-23 10:51:55.000000 loguru-0.7.0/loguru/_contextvars.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1531 2022-08-08 09:02:07.000000 loguru-0.7.0/loguru/_ctime_functions.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3220 2022-08-08 09:02:07.000000 loguru-0.7.0/loguru/_datetime.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2879 2023-04-10 08:40:38.000000 loguru-0.7.0/loguru/_defaults.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1107 2023-03-26 10:22:40.000000 loguru-0.7.0/loguru/_error_interceptor.py
+-rw-r--r--   0 delgan    (1000) users      (985)    14586 2023-01-07 08:31:47.000000 loguru-0.7.0/loguru/_file_sink.py
+-rw-r--r--   0 delgan    (1000) users      (985)      618 2022-04-23 10:51:55.000000 loguru-0.7.0/loguru/_filters.py
+-rw-r--r--   0 delgan    (1000) users      (985)      458 2022-04-23 10:51:55.000000 loguru-0.7.0/loguru/_get_frame.py
+-rw-r--r--   0 delgan    (1000) users      (985)    11952 2023-04-10 08:40:38.000000 loguru-0.7.0/loguru/_handler.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1307 2022-09-30 12:29:04.000000 loguru-0.7.0/loguru/_locks_machinery.py
+-rw-r--r--   0 delgan    (1000) users      (985)    94321 2023-04-10 08:40:38.000000 loguru-0.7.0/loguru/_logger.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2174 2022-06-19 08:22:29.000000 loguru-0.7.0/loguru/_recattrs.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3160 2022-06-19 08:22:29.000000 loguru-0.7.0/loguru/_simple_sinks.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4707 2022-08-08 09:02:07.000000 loguru-0.7.0/loguru/_string_parsers.py
+-rw-r--r--   0 delgan    (1000) users      (985)        0 2021-03-13 14:44:16.000000 loguru-0.7.0/loguru/py.typed
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.900362 loguru-0.7.0/loguru.egg-info/
+-rw-r--r--   0 delgan    (1000) users      (985)    20466 2023-04-10 09:00:16.000000 loguru-0.7.0/loguru.egg-info/PKG-INFO
+-rw-r--r--   0 delgan    (1000) users      (985)    10748 2023-04-10 09:00:16.000000 loguru-0.7.0/loguru.egg-info/SOURCES.txt
+-rw-r--r--   0 delgan    (1000) users      (985)        1 2023-04-10 09:00:16.000000 loguru-0.7.0/loguru.egg-info/dependency_links.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      692 2023-04-10 09:00:16.000000 loguru-0.7.0/loguru.egg-info/requires.txt
+-rw-r--r--   0 delgan    (1000) users      (985)        7 2023-04-10 09:00:16.000000 loguru-0.7.0/loguru.egg-info/top_level.txt
+-rw-r--r--   0 delgan    (1000) users      (985)       38 2023-04-10 09:00:17.477029 loguru-0.7.0/setup.cfg
+-rw-r--r--   0 delgan    (1000) users      (985)     3550 2023-04-10 08:41:53.000000 loguru-0.7.0/setup.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.017029 loguru-0.7.0/tests/
+-rw-r--r--   0 delgan    (1000) users      (985)        0 2019-11-11 21:50:18.000000 loguru-0.7.0/tests/__init__.py
+-rw-r--r--   0 delgan    (1000) users      (985)     7755 2023-01-07 08:31:47.000000 loguru-0.7.0/tests/conftest.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.853695 loguru-0.7.0/tests/exceptions/
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.853695 loguru-0.7.0/tests/exceptions/output/
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.117029 loguru-0.7.0/tests/exceptions/output/backtrace/
+-rw-r--r--   0 delgan    (1000) users      (985)     1990 2022-06-19 16:19:30.000000 loguru-0.7.0/tests/exceptions/output/backtrace/chained_expression_direct.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1636 2022-06-19 16:19:30.000000 loguru-0.7.0/tests/exceptions/output/backtrace/chained_expression_indirect.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1327 2022-06-19 16:19:31.000000 loguru-0.7.0/tests/exceptions/output/backtrace/chaining_first.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1409 2022-06-19 16:19:31.000000 loguru-0.7.0/tests/exceptions/output/backtrace/chaining_second.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1467 2022-06-19 16:19:31.000000 loguru-0.7.0/tests/exceptions/output/backtrace/chaining_third.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      157 2022-06-19 16:19:31.000000 loguru-0.7.0/tests/exceptions/output/backtrace/enqueue.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      179 2022-06-19 16:19:32.000000 loguru-0.7.0/tests/exceptions/output/backtrace/enqueue_with_others_handlers.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      456 2022-06-19 16:19:32.000000 loguru-0.7.0/tests/exceptions/output/backtrace/frame_values_backward.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      452 2022-06-19 16:19:32.000000 loguru-0.7.0/tests/exceptions/output/backtrace/frame_values_forward.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      711 2022-06-19 16:19:32.000000 loguru-0.7.0/tests/exceptions/output/backtrace/function.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3852 2022-06-19 16:19:33.000000 loguru-0.7.0/tests/exceptions/output/backtrace/head_recursion.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      411 2022-06-19 16:19:33.000000 loguru-0.7.0/tests/exceptions/output/backtrace/missing_attributes_traceback_objects.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      963 2022-06-19 16:19:33.000000 loguru-0.7.0/tests/exceptions/output/backtrace/nested.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1428 2022-06-19 16:19:33.000000 loguru-0.7.0/tests/exceptions/output/backtrace/nested_chained_catch_up.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      748 2022-06-19 16:19:33.000000 loguru-0.7.0/tests/exceptions/output/backtrace/nested_decorator_catch_up.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      742 2022-06-19 16:19:34.000000 loguru-0.7.0/tests/exceptions/output/backtrace/nested_explicit_catch_up.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      842 2022-06-19 16:19:34.000000 loguru-0.7.0/tests/exceptions/output/backtrace/nested_wrapping.txt
+-rw-r--r--   0 delgan    (1000) users      (985)       42 2022-06-19 16:19:34.000000 loguru-0.7.0/tests/exceptions/output/backtrace/no_tb.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      670 2022-06-19 16:19:34.000000 loguru-0.7.0/tests/exceptions/output/backtrace/not_enough_arguments.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     9672 2022-06-19 16:19:34.000000 loguru-0.7.0/tests/exceptions/output/backtrace/raising_recursion.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2356 2022-06-19 16:19:35.000000 loguru-0.7.0/tests/exceptions/output/backtrace/suppressed_expression_direct.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2278 2022-06-19 16:19:35.000000 loguru-0.7.0/tests/exceptions/output/backtrace/suppressed_expression_indirect.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3852 2022-06-19 16:19:35.000000 loguru-0.7.0/tests/exceptions/output/backtrace/tail_recursion.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      640 2022-06-19 16:19:35.000000 loguru-0.7.0/tests/exceptions/output/backtrace/too_many_arguments.txt
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.167029 loguru-0.7.0/tests/exceptions/output/diagnose/
+-rw-r--r--   0 delgan    (1000) users      (985)      800 2022-06-19 16:19:35.000000 loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      760 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error_custom.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      588 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error_in_string.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1931 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/attributes.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2027 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/chained_both.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      820 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/encoding.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      712 2022-06-19 16:19:36.000000 loguru-0.7.0/tests/exceptions/output/diagnose/global_variable.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      502 2022-06-19 16:19:37.000000 loguru-0.7.0/tests/exceptions/output/diagnose/indentation_error.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1232 2022-06-19 16:19:37.000000 loguru-0.7.0/tests/exceptions/output/diagnose/keyword_argument.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      780 2022-06-19 16:19:37.000000 loguru-0.7.0/tests/exceptions/output/diagnose/multilines_repr.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      696 2022-06-19 16:19:37.000000 loguru-0.7.0/tests/exceptions/output/diagnose/no_error_message.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3109 2022-06-19 16:19:37.000000 loguru-0.7.0/tests/exceptions/output/diagnose/parenthesis.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2589 2022-06-19 16:19:38.000000 loguru-0.7.0/tests/exceptions/output/diagnose/source_multilines.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      543 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/diagnose/source_strings.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      393 2022-06-19 16:19:38.000000 loguru-0.7.0/tests/exceptions/output/diagnose/syntax_error.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2717 2022-06-19 16:19:38.000000 loguru-0.7.0/tests/exceptions/output/diagnose/syntax_highlighting.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      695 2022-06-19 16:19:38.000000 loguru-0.7.0/tests/exceptions/output/diagnose/truncating.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      368 2022-06-19 16:19:39.000000 loguru-0.7.0/tests/exceptions/output/diagnose/unprintable_object.txt
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.250362 loguru-0.7.0/tests/exceptions/output/others/
+-rw-r--r--   0 delgan    (1000) users      (985)      116 2022-06-19 16:19:41.000000 loguru-0.7.0/tests/exceptions/output/others/assertionerror_without_traceback.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      172 2022-06-19 16:19:42.000000 loguru-0.7.0/tests/exceptions/output/others/catch_as_context_manager.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      291 2022-06-19 16:19:42.000000 loguru-0.7.0/tests/exceptions/output/others/catch_as_decorator_with_parentheses.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      292 2022-06-19 16:19:42.000000 loguru-0.7.0/tests/exceptions/output/others/catch_as_decorator_without_parentheses.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      249 2022-06-19 16:19:42.000000 loguru-0.7.0/tests/exceptions/output/others/catch_as_function.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      526 2022-06-19 16:19:42.000000 loguru-0.7.0/tests/exceptions/output/others/catch_message.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1394 2022-06-19 16:19:43.000000 loguru-0.7.0/tests/exceptions/output/others/exception_formatting_coroutine.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1236 2022-06-19 16:19:43.000000 loguru-0.7.0/tests/exceptions/output/others/exception_formatting_function.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     1330 2022-06-19 16:19:43.000000 loguru-0.7.0/tests/exceptions/output/others/exception_formatting_generator.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      378 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/others/exception_in_property.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      236 2022-06-19 16:19:43.000000 loguru-0.7.0/tests/exceptions/output/others/handler_formatting_with_context_manager.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      338 2022-06-19 16:19:44.000000 loguru-0.7.0/tests/exceptions/output/others/handler_formatting_with_decorator.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      161 2022-06-19 16:19:44.000000 loguru-0.7.0/tests/exceptions/output/others/level_name.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      166 2022-06-19 16:19:44.000000 loguru-0.7.0/tests/exceptions/output/others/level_number.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      236 2022-06-19 16:19:44.000000 loguru-0.7.0/tests/exceptions/output/others/message_formatting_with_context_manager.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      338 2022-06-19 16:19:44.000000 loguru-0.7.0/tests/exceptions/output/others/message_formatting_with_decorator.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     4582 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/others/nested_with_reraise.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      388 2022-06-19 16:19:45.000000 loguru-0.7.0/tests/exceptions/output/others/syntaxerror_without_traceback.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2356 2022-06-19 16:19:45.000000 loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      148 2022-06-19 16:19:45.000000 loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit_negative.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     5076 2022-06-19 16:19:45.000000 loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit_none.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     5120 2022-06-19 16:19:46.000000 loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit_unset.txt
+-rw-r--r--   0 delgan    (1000) users      (985)      232 2022-06-19 16:19:46.000000 loguru-0.7.0/tests/exceptions/output/others/zerodivisionerror_without_traceback.txt
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.290362 loguru-0.7.0/tests/exceptions/output/ownership/
+-rw-r--r--   0 delgan    (1000) users      (985)     2964 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/assertion_from_lib.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2204 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/assertion_from_local.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     4172 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/callback.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3478 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/catch_decorator.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3740 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/catch_decorator_from_lib.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3127 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/decorated_callback.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2573 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/direct.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3268 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/indirect.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     3095 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/string_lib.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2922 2022-06-19 16:19:41.000000 loguru-0.7.0/tests/exceptions/output/ownership/string_source.txt
+-rw-r--r--   0 delgan    (1000) users      (985)     2693 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/output/ownership/syntaxerror.txt
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.853695 loguru-0.7.0/tests/exceptions/source/
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.360362 loguru-0.7.0/tests/exceptions/source/backtrace/
+-rw-r--r--   0 delgan    (1000) users      (985)      642 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/chained_expression_direct.py
+-rw-r--r--   0 delgan    (1000) users      (985)      360 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/chained_expression_indirect.py
+-rw-r--r--   0 delgan    (1000) users      (985)      393 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/chaining_first.py
+-rw-r--r--   0 delgan    (1000) users      (985)      516 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/chaining_second.py
+-rw-r--r--   0 delgan    (1000) users      (985)      624 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/chaining_third.py
+-rw-r--r--   0 delgan    (1000) users      (985)      223 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/enqueue.py
+-rw-r--r--   0 delgan    (1000) users      (985)      618 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/enqueue_with_others_handlers.py
+-rw-r--r--   0 delgan    (1000) users      (985)      237 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/frame_values_backward.py
+-rw-r--r--   0 delgan    (1000) users      (985)      237 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/frame_values_forward.py
+-rw-r--r--   0 delgan    (1000) users      (985)      317 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/function.py
+-rw-r--r--   0 delgan    (1000) users      (985)      466 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/head_recursion.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1136 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/backtrace/missing_attributes_traceback_objects.py
+-rw-r--r--   0 delgan    (1000) users      (985)      457 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/nested.py
+-rw-r--r--   0 delgan    (1000) users      (985)      418 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/nested_chained_catch_up.py
+-rw-r--r--   0 delgan    (1000) users      (985)      342 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/nested_decorator_catch_up.py
+-rw-r--r--   0 delgan    (1000) users      (985)      369 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/nested_explicit_catch_up.py
+-rw-r--r--   0 delgan    (1000) users      (985)      409 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/nested_wrapping.py
+-rw-r--r--   0 delgan    (1000) users      (985)      335 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/no_tb.py
+-rw-r--r--   0 delgan    (1000) users      (985)      353 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/not_enough_arguments.py
+-rw-r--r--   0 delgan    (1000) users      (985)      464 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/raising_recursion.py
+-rw-r--r--   0 delgan    (1000) users      (985)      693 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/suppressed_expression_direct.py
+-rw-r--r--   0 delgan    (1000) users      (985)      480 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/suppressed_expression_indirect.py
+-rw-r--r--   0 delgan    (1000) users      (985)      408 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/tail_recursion.py
+-rw-r--r--   0 delgan    (1000) users      (985)      339 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/backtrace/too_many_arguments.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.403696 loguru-0.7.0/tests/exceptions/source/diagnose/
+-rw-r--r--   0 delgan    (1000) users      (985)      261 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/assertion_error.py
+-rw-r--r--   0 delgan    (1000) users      (985)      285 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/assertion_error_custom.py
+-rw-r--r--   0 delgan    (1000) users      (985)      269 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/assertion_error_in_string.py
+-rw-r--r--   0 delgan    (1000) users      (985)      445 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/diagnose/attributes.py
+-rw-r--r--   0 delgan    (1000) users      (985)      467 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/chained_both.py
+-rw-r--r--   0 delgan    (1000) users      (985)      270 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/encoding.py
+-rw-r--r--   0 delgan    (1000) users      (985)      296 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/global_variable.py
+-rw-r--r--   0 delgan    (1000) users      (985)      316 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/indentation_error.py
+-rw-r--r--   0 delgan    (1000) users      (985)      246 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/keyword_argument.py
+-rw-r--r--   0 delgan    (1000) users      (985)      341 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/multilines_repr.py
+-rw-r--r--   0 delgan    (1000) users      (985)      258 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/no_error_message.py
+-rw-r--r--   0 delgan    (1000) users      (985)      641 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/diagnose/parenthesis.py
+-rw-r--r--   0 delgan    (1000) users      (985)      787 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/diagnose/source_multilines.py
+-rw-r--r--   0 delgan    (1000) users      (985)      260 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/diagnose/source_strings.py
+-rw-r--r--   0 delgan    (1000) users      (985)      251 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/syntax_error.py
+-rw-r--r--   0 delgan    (1000) users      (985)      518 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/diagnose/syntax_highlighting.py
+-rw-r--r--   0 delgan    (1000) users      (985)      248 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/truncating.py
+-rw-r--r--   0 delgan    (1000) users      (985)      307 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/diagnose/unprintable_object.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.447029 loguru-0.7.0/tests/exceptions/source/others/
+-rw-r--r--   0 delgan    (1000) users      (985)      433 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/others/assertionerror_without_traceback.py
+-rw-r--r--   0 delgan    (1000) users      (985)      171 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/catch_as_context_manager.py
+-rw-r--r--   0 delgan    (1000) users      (985)      191 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/catch_as_decorator_with_parentheses.py
+-rw-r--r--   0 delgan    (1000) users      (985)      186 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/catch_as_decorator_without_parentheses.py
+-rw-r--r--   0 delgan    (1000) users      (985)      187 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/catch_as_function.py
+-rw-r--r--   0 delgan    (1000) users      (985)      290 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/catch_message.py
+-rw-r--r--   0 delgan    (1000) users      (985)      500 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/exception_formatting_coroutine.py
+-rw-r--r--   0 delgan    (1000) users      (985)      432 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/exception_formatting_function.py
+-rw-r--r--   0 delgan    (1000) users      (985)      495 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/exception_formatting_generator.py
+-rw-r--r--   0 delgan    (1000) users      (985)      388 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/others/exception_in_property.py
+-rw-r--r--   0 delgan    (1000) users      (985)      253 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/handler_formatting_with_context_manager.py
+-rw-r--r--   0 delgan    (1000) users      (985)      238 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/handler_formatting_with_decorator.py
+-rw-r--r--   0 delgan    (1000) users      (985)      238 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/level_name.py
+-rw-r--r--   0 delgan    (1000) users      (985)      233 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/level_number.py
+-rw-r--r--   0 delgan    (1000) users      (985)      295 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/message_formatting_with_context_manager.py
+-rw-r--r--   0 delgan    (1000) users      (985)      268 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/message_formatting_with_decorator.py
+-rw-r--r--   0 delgan    (1000) users      (985)      640 2022-08-08 09:02:07.000000 loguru-0.7.0/tests/exceptions/source/others/nested_with_reraise.py
+-rw-r--r--   0 delgan    (1000) users      (985)      416 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/syntaxerror_without_traceback.py
+-rw-r--r--   0 delgan    (1000) users      (985)      673 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit.py
+-rw-r--r--   0 delgan    (1000) users      (985)      674 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_negative.py
+-rw-r--r--   0 delgan    (1000) users      (985)      676 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_none.py
+-rw-r--r--   0 delgan    (1000) users      (985)      714 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_unset.py
+-rw-r--r--   0 delgan    (1000) users      (985)      414 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/others/zerodivisionerror_without_traceback.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.470363 loguru-0.7.0/tests/exceptions/source/ownership/
+-rw-r--r--   0 delgan    (1000) users      (985)      208 2022-06-19 16:08:49.000000 loguru-0.7.0/tests/exceptions/source/ownership/_init.py
+-rw-r--r--   0 delgan    (1000) users      (985)      644 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/assertion_from_lib.py
+-rw-r--r--   0 delgan    (1000) users      (985)      637 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/assertion_from_local.py
+-rw-r--r--   0 delgan    (1000) users      (985)      665 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/callback.py
+-rw-r--r--   0 delgan    (1000) users      (985)      587 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/catch_decorator.py
+-rw-r--r--   0 delgan    (1000) users      (985)      611 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/catch_decorator_from_lib.py
+-rw-r--r--   0 delgan    (1000) users      (985)      624 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/decorated_callback.py
+-rw-r--r--   0 delgan    (1000) users      (985)      612 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/direct.py
+-rw-r--r--   0 delgan    (1000) users      (985)      630 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/indirect.py
+-rw-r--r--   0 delgan    (1000) users      (985)      609 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/string_lib.py
+-rw-r--r--   0 delgan    (1000) users      (985)      586 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/exceptions/source/ownership/string_source.py
+-rw-r--r--   0 delgan    (1000) users      (985)      611 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/exceptions/source/ownership/syntaxerror.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:16.853695 loguru-0.7.0/tests/exceptions/source/ownership/usersite/
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.473696 loguru-0.7.0/tests/exceptions/source/ownership/usersite/somelib/
+-rw-r--r--   0 delgan    (1000) users      (985)      240 2021-03-13 14:44:16.000000 loguru-0.7.0/tests/exceptions/source/ownership/usersite/somelib/__init__.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3667 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_activation.py
+-rw-r--r--   0 delgan    (1000) users      (985)      579 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_add_option_backtrace.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3737 2023-03-28 18:20:47.000000 loguru-0.7.0/tests/test_add_option_catch.py
+-rw-r--r--   0 delgan    (1000) users      (985)     7849 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_add_option_colorize.py
+-rw-r--r--   0 delgan    (1000) users      (985)      576 2021-03-13 14:44:16.000000 loguru-0.7.0/tests/test_add_option_diagnose.py
+-rw-r--r--   0 delgan    (1000) users      (985)     8060 2023-03-28 18:20:47.000000 loguru-0.7.0/tests/test_add_option_enqueue.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3427 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_add_option_filter.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2590 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_add_option_format.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1656 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_add_option_kwargs.py
+-rw-r--r--   0 delgan    (1000) users      (985)      815 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_add_option_level.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4171 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_add_option_serialize.py
+-rw-r--r--   0 delgan    (1000) users      (985)     5744 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_add_sinks.py
+-rw-r--r--   0 delgan    (1000) users      (985)     6003 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_ansimarkup_basic.py
+-rw-r--r--   0 delgan    (1000) users      (985)     6585 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_ansimarkup_extended.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2046 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_bind.py
+-rw-r--r--   0 delgan    (1000) users      (985)     5238 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_configure.py
+-rw-r--r--   0 delgan    (1000) users      (985)     5606 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_contextualize.py
+-rw-r--r--   0 delgan    (1000) users      (985)    14904 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_coroutine_sink.py
+-rw-r--r--   0 delgan    (1000) users      (985)     5403 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_datetime.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1173 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_deepcopy.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1155 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_defaults.py
+-rw-r--r--   0 delgan    (1000) users      (985)    11028 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_exceptions_catch.py
+-rw-r--r--   0 delgan    (1000) users      (985)     6886 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_exceptions_formatting.py
+-rw-r--r--   0 delgan    (1000) users      (985)     9353 2023-03-18 08:13:39.000000 loguru-0.7.0/tests/test_filesink_compression.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3435 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_filesink_delay.py
+-rw-r--r--   0 delgan    (1000) users      (985)     1304 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_filesink_permissions.py
+-rw-r--r--   0 delgan    (1000) users      (985)     9949 2023-03-18 08:13:39.000000 loguru-0.7.0/tests/test_filesink_retention.py
+-rw-r--r--   0 delgan    (1000) users      (985)    31722 2023-03-18 08:13:39.000000 loguru-0.7.0/tests/test_filesink_rotation.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4502 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_filesink_watch.py
+-rw-r--r--   0 delgan    (1000) users      (985)     7015 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_formatting.py
+-rw-r--r--   0 delgan    (1000) users      (985)      818 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_get_frame.py
+-rw-r--r--   0 delgan    (1000) users      (985)     5207 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_interception.py
+-rw-r--r--   0 delgan    (1000) users      (985)     8029 2022-12-30 19:41:32.000000 loguru-0.7.0/tests/test_levels.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3736 2022-12-30 19:41:32.000000 loguru-0.7.0/tests/test_locks.py
+-rw-r--r--   0 delgan    (1000) users      (985)    16055 2023-03-28 18:20:47.000000 loguru-0.7.0/tests/test_multiprocessing.py
+-rw-r--r--   0 delgan    (1000) users      (985)    20870 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_opt.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4419 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_parse.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2430 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_patch.py
+-rw-r--r--   0 delgan    (1000) users      (985)    10198 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_pickling.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2725 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_propagation.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2158 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_recattr.py
+-rw-r--r--   0 delgan    (1000) users      (985)     2670 2023-03-18 08:13:39.000000 loguru-0.7.0/tests/test_remove.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4969 2022-12-30 19:41:32.000000 loguru-0.7.0/tests/test_repr.py
+-rw-r--r--   0 delgan    (1000) users      (985)     4832 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_standard_handler.py
+-rw-r--r--   0 delgan    (1000) users      (985)     3696 2022-04-23 10:51:55.000000 loguru-0.7.0/tests/test_threading.py
+-rw-r--r--   0 delgan    (1000) users      (985)      295 2022-08-08 09:02:08.000000 loguru-0.7.0/tests/test_type_hinting.py
+drwxr-xr-x   0 delgan    (1000) users      (985)        0 2023-04-10 09:00:17.473696 loguru-0.7.0/tests/typesafety/
+-rw-r--r--   0 delgan    (1000) users      (985)     9500 2022-12-30 19:41:32.000000 loguru-0.7.0/tests/typesafety/test_logger.yml
```

### Comparing `loguru-0.6.0/LICENSE` & `loguru-0.7.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017 
+Copyright (c) 2017
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `loguru-0.6.0/PKG-INFO` & `loguru-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: loguru
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python logging made (stupidly) simple
 Home-page: https://github.com/Delgan/loguru
+Download-URL: https://github.com/Delgan/loguru/archive/0.7.0.tar.gz
 Author: Delgan
 Author-email: delgan.py@gmail.com
 License: MIT license
-Download-URL: https://github.com/Delgan/loguru/archive/0.6.0.tar.gz
 Project-URL: Changelog, https://github.com/Delgan/loguru/blob/master/CHANGELOG.rst
 Project-URL: Documentation, https://loguru.readthedocs.io/en/stable/index.html
 Keywords: loguru,logging,logger,log
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Logging
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -54,15 +54,15 @@
     :alt: Python versions
 
 .. image:: https://img.shields.io/readthedocs/loguru.svg
     :target: https://loguru.readthedocs.io/en/stable/index.html
     :alt: Docs
 
 .. image:: https://img.shields.io/github/workflow/status/Delgan/loguru/Tests/master
-    :target: https://github.com/Delgan/loguru/actions/workflows/tests.yml?query=branch:master
+    :target: https://img.shields.io/github/actions/workflow/status/Delgan/loguru/tests.yml?branch=master
     :alt: Build status
 
 .. image:: https://img.shields.io/codecov/c/github/delgan/loguru/master.svg
     :target: https://codecov.io/gh/delgan/loguru/branch/master
     :alt: Coverage
 
 .. image:: https://img.shields.io/codacy/grade/be7337df3c0d40d1929eb7f79b1671a6.svg
@@ -314,14 +314,16 @@
       File "test.py", line 4, in func
         return a / b
                │   └ 0
                └ 5
 
     ZeroDivisionError: division by zero
 
+Note that this feature won't work on default Python REPL due to unavailable frame data.
+
 
 Structured logging as needed
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Want your logs to be serialized for easier parsing or to pass them around? Using the ``serialize`` argument, each log message will be converted to a JSON string before being sent to the configured sink.
 
 ::
@@ -401,15 +403,15 @@
 
     logger.add("file.log", format="{time:YYYY-MM-DD at HH:mm:ss} | {level} | {message}")
 
 
 Suitable for scripts and libraries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, he can |enable|_ it again.
+Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, they can |enable|_ it again.
 
 ::
 
     # For scripts
     config = {
         "handlers": [
             {"sink": sys.stdout, "format": "{time} - {message}"},
@@ -448,29 +450,29 @@
 
 Want to intercept standard `logging` messages toward your `Loguru` sinks?
 
 ::
 
     class InterceptHandler(logging.Handler):
         def emit(self, record):
-            # Get corresponding Loguru level if it exists
+            # Get corresponding Loguru level if it exists.
             try:
                 level = logger.level(record.levelname).name
             except ValueError:
                 level = record.levelno
 
-            # Find caller from where originated the logged message
-            frame, depth = logging.currentframe(), 2
-            while frame.f_code.co_filename == logging.__file__:
+            # Find caller from where originated the logged message.
+            frame, depth = sys._getframe(6), 6
+            while frame and frame.f_code.co_filename == logging.__file__:
                 frame = frame.f_back
                 depth += 1
 
             logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
-    logging.basicConfig(handlers=[InterceptHandler()], level=0)
+    logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
 
 
 Personalizable defaults through environment variables
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Don't like the default logger formatting? Would prefer another ``DEBUG`` color? `No problem`_::
 
@@ -536,9 +538,7 @@
 
 * `API Reference <https://loguru.readthedocs.io/en/stable/api/logger.html>`_
 * `Help & Guides <https://loguru.readthedocs.io/en/stable/resources.html>`_
 * `Type hints <https://loguru.readthedocs.io/en/stable/api/type_hints.html>`_
 * `Contributing <https://loguru.readthedocs.io/en/stable/project/contributing.html>`_
 * `License <https://loguru.readthedocs.io/en/stable/project/license.html>`_
 * `Changelog <https://loguru.readthedocs.io/en/stable/project/changelog.html>`_
-
-
```

### Comparing `loguru-0.6.0/README.rst` & `loguru-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :alt: Python versions
 
 .. image:: https://img.shields.io/readthedocs/loguru.svg
     :target: https://loguru.readthedocs.io/en/stable/index.html
     :alt: Docs
 
 .. image:: https://img.shields.io/github/workflow/status/Delgan/loguru/Tests/master
-    :target: https://github.com/Delgan/loguru/actions/workflows/tests.yml?query=branch:master
+    :target: https://img.shields.io/github/actions/workflow/status/Delgan/loguru/tests.yml?branch=master
     :alt: Build status
 
 .. image:: https://img.shields.io/codecov/c/github/delgan/loguru/master.svg
     :target: https://codecov.io/gh/delgan/loguru/branch/master
     :alt: Coverage
 
 .. image:: https://img.shields.io/codacy/grade/be7337df3c0d40d1929eb7f79b1671a6.svg
@@ -279,14 +279,16 @@
       File "test.py", line 4, in func
         return a / b
                │   └ 0
                └ 5
 
     ZeroDivisionError: division by zero
 
+Note that this feature won't work on default Python REPL due to unavailable frame data.
+
 
 Structured logging as needed
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Want your logs to be serialized for easier parsing or to pass them around? Using the ``serialize`` argument, each log message will be converted to a JSON string before being sent to the configured sink.
 
 ::
@@ -366,15 +368,15 @@
 
     logger.add("file.log", format="{time:YYYY-MM-DD at HH:mm:ss} | {level} | {message}")
 
 
 Suitable for scripts and libraries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, he can |enable|_ it again.
+Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, they can |enable|_ it again.
 
 ::
 
     # For scripts
     config = {
         "handlers": [
             {"sink": sys.stdout, "format": "{time} - {message}"},
@@ -413,29 +415,29 @@
 
 Want to intercept standard `logging` messages toward your `Loguru` sinks?
 
 ::
 
     class InterceptHandler(logging.Handler):
         def emit(self, record):
-            # Get corresponding Loguru level if it exists
+            # Get corresponding Loguru level if it exists.
             try:
                 level = logger.level(record.levelname).name
             except ValueError:
                 level = record.levelno
 
-            # Find caller from where originated the logged message
-            frame, depth = logging.currentframe(), 2
-            while frame.f_code.co_filename == logging.__file__:
+            # Find caller from where originated the logged message.
+            frame, depth = sys._getframe(6), 6
+            while frame and frame.f_code.co_filename == logging.__file__:
                 frame = frame.f_back
                 depth += 1
 
             logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
-    logging.basicConfig(handlers=[InterceptHandler()], level=0)
+    logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
 
 
 Personalizable defaults through environment variables
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Don't like the default logger formatting? Would prefer another ``DEBUG`` color? `No problem`_::
```

### Comparing `loguru-0.6.0/loguru/__init__.py` & `loguru-0.7.0/loguru/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import atexit as _atexit
 import sys as _sys
 
 from . import _defaults
 from ._logger import Core as _Core
 from ._logger import Logger as _Logger
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 __all__ = ["logger"]
 
 logger = _Logger(
     core=_Core(),
     exception=None,
     depth=0,
     record=False,
     lazy=False,
     colors=False,
     raw=False,
     capture=True,
-    patcher=None,
+    patchers=[],
     extra={},
 )
 
 if _defaults.LOGURU_AUTOINIT and _sys.stderr:
     logger.add(_sys.stderr)
 
 _atexit.register(logger.remove)
```

### Comparing `loguru-0.6.0/loguru/__init__.pyi` & `loguru-0.7.0/loguru/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     BinaryIO,
     Callable,
     Dict,
     Generator,
     Generic,
     List,
     NamedTuple,
+    NewType,
     Optional,
     Pattern,
     Sequence,
     TextIO,
     Tuple,
     Type,
     TypeVar,
@@ -116,34 +117,42 @@
     from typing import Awaitable
 else:
     from typing_extensions import Awaitable
 
 if sys.version_info >= (3, 6):
     from os import PathLike
     from typing import ContextManager
+
+    PathLikeStr = PathLike[str]
 else:
-    from pathlib import PurePath as PathLike
+    from pathlib import PurePath as PathLikeStr
 
     from typing_extensions import ContextManager
 
 if sys.version_info >= (3, 8):
     from typing import Protocol, TypedDict
 else:
     from typing_extensions import Protocol, TypedDict
 
 _T = TypeVar("_T")
 _F = TypeVar("_F", bound=Callable[..., Any])
 ExcInfo = Tuple[Optional[Type[BaseException]], Optional[BaseException], Optional[TracebackType]]
 
 class _GeneratorContextManager(ContextManager[_T], Generic[_T]):
     def __call__(self, func: _F) -> _F: ...
-
-Catcher = _GeneratorContextManager[None]
-Contextualizer = _GeneratorContextManager[None]
-AwaitableCompleter = Awaitable
+    def __exit__(
+        self,
+        typ: Optional[Type[BaseException]],
+        value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Optional[bool]: ...
+
+Catcher = NewType("Catcher", _GeneratorContextManager[None])
+Contextualizer = NewType("Contextualizer", _GeneratorContextManager[None])
+AwaitableCompleter = Awaitable[None]
 
 class Level(NamedTuple):
     name: str
     no: int
     color: str
     icon: str
 
@@ -200,15 +209,15 @@
 PatcherFunction = Callable[[Record], None]
 RotationFunction = Callable[[Message, TextIO], bool]
 RetentionFunction = Callable[[List[str]], None]
 CompressionFunction = Callable[[str], None]
 
 # Actually unusable because TypedDict can't allow extra keys: python/mypy#4617
 class _HandlerConfig(TypedDict, total=False):
-    sink: Union[str, PathLike[str], TextIO, Writable, Callable[[Message], None], Handler]
+    sink: Union[str, PathLikeStr, TextIO, Writable, Callable[[Message], None], Handler]
     level: Union[str, int]
     format: Union[str, FormatFunction]
     filter: Optional[Union[str, FilterFunction, FilterDict]]
     colorize: Optional[bool]
     serialize: bool
     backtrace: bool
     diagnose: bool
@@ -254,38 +263,39 @@
         enqueue: bool = ...,
         catch: bool = ...,
         loop: Optional[AbstractEventLoop] = ...
     ) -> int: ...
     @overload
     def add(
         self,
-        sink: Union[str, PathLike[str]],
+        sink: Union[str, PathLikeStr],
         *,
         level: Union[str, int] = ...,
         format: Union[str, FormatFunction] = ...,
         filter: Optional[Union[str, FilterFunction, FilterDict]] = ...,
         colorize: Optional[bool] = ...,
         serialize: bool = ...,
         backtrace: bool = ...,
         diagnose: bool = ...,
         enqueue: bool = ...,
         catch: bool = ...,
         rotation: Optional[Union[str, int, time, timedelta, RotationFunction]] = ...,
         retention: Optional[Union[str, int, timedelta, RetentionFunction]] = ...,
         compression: Optional[Union[str, CompressionFunction]] = ...,
         delay: bool = ...,
+        watch: bool = ...,
         mode: str = ...,
         buffering: int = ...,
         encoding: str = ...,
         **kwargs: Any
     ) -> int: ...
     def remove(self, handler_id: Optional[int] = ...) -> None: ...
     def complete(self) -> AwaitableCompleter: ...
     @overload
-    def catch(
+    def catch(  # type: ignore[misc]
         self,
         exception: Union[Type[BaseException], Tuple[Type[BaseException], ...]] = ...,
         *,
         level: Union[str, int] = ...,
         reraise: bool = ...,
         onerror: Optional[Callable[[BaseException], None]] = ...,
         exclude: Optional[Union[Type[BaseException], Tuple[Type[BaseException], ...]]] = ...,
@@ -337,15 +347,15 @@
     # @staticmethod cannot be used with @overload in mypy (python/mypy#7781).
     # However Logger is not exposed and logger is an instance of Logger
     # so for type checkers it is all the same whether it is defined here
     # as a static method or an instance method.
     @overload
     def parse(
         self,
-        file: Union[str, PathLike[str], TextIO],
+        file: Union[str, PathLikeStr, TextIO],
         pattern: Union[str, Pattern[str]],
         *,
         cast: Union[Dict[str, Callable[[str], Any]], Callable[[Dict[str, str]], None]] = ...,
         chunk: int = ...
     ) -> Generator[Dict[str, Any], None, None]: ...
     @overload
     def parse(
@@ -390,11 +400,11 @@
     def exception(__self, __message: Any) -> None: ...
     @overload
     def log(
         __self, __level: Union[int, str], __message: str, *args: Any, **kwargs: Any
     ) -> None: ...
     @overload
     def log(__self, __level: Union[int, str], __message: Any) -> None: ...
-    def start(self, *args: Any, **kwargs: Any): ...
-    def stop(self, *args: Any, **kwargs: Any): ...
+    def start(self, *args: Any, **kwargs: Any) -> int: ...
+    def stop(self, *args: Any, **kwargs: Any) -> None: ...
 
 logger: Logger
```

### Comparing `loguru-0.6.0/loguru/_asyncio_loop.py` & `loguru-0.7.0/loguru/_asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_better_exceptions.py` & `loguru-0.7.0/loguru/_better_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import sys
 import sysconfig
 import tokenize
 import traceback
 
 
 class SyntaxHighlighter:
-
     _default_style = {
         "comment": "\x1b[30m\x1b[1m{}\x1b[0m",
         "keyword": "\x1b[35m\x1b[1m{}\x1b[0m",
         "builtin": "\x1b[1m{}\x1b[0m",
         "string": "\x1b[36m{}\x1b[0m",
         "number": "\x1b[34m\x1b[1m{}\x1b[0m",
         "operator": "\x1b[35m\x1b[1m{}\x1b[0m",
@@ -90,15 +89,14 @@
         try:
             yield from tokenize.tokenize(source.readline)
         except tokenize.TokenError:
             return
 
 
 class ExceptionFormatter:
-
     _default_theme = {
         "introduction": "\x1b[33m\x1b[1m{}\x1b[0m",
         "cause": "\x1b[1m{}\x1b[0m",
         "context": "\x1b[1m{}\x1b[0m",
         "dirname": "\x1b[32m{}\x1b[0m",
         "basename": "\x1b[32m\x1b[1m{}\x1b[0m",
         "line": "\x1b[33m{}\x1b[0m",
@@ -343,15 +341,16 @@
                 location = pattern.format(file, line, function)
                 frame = location + frame[match.end() :]
                 prepend_with_new_line = is_mine
 
             yield frame
 
     def _format_exception(self, value, tb, *, seen=None, is_first=False, from_decorator=False):
-        # Implemented from built-in traceback module: https://git.io/fhHKw
+        # Implemented from built-in traceback module:
+        # https://github.com/python/cpython/blob/a5b76167/Lib/traceback.py#L468
         exc_type, exc_value, exc_traceback = type(value), value, tb
 
         if seen is None:
             seen = set()
 
         seen.add(id(exc_value))
```

### Comparing `loguru-0.6.0/loguru/_colorizer.py` & `loguru-0.7.0/loguru/_colorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     TEXT = 1
     ANSI = 2
     LEVEL = 3
     CLOSING = 4
 
 
 class AnsiParser:
-
     _style = ansi_escape(
         {
             "b": Style.BOLD,
             "d": Style.DIM,
             "n": Style.NORMAL,
             "h": Style.HIDE,
             "i": Style.ITALIC,
@@ -247,15 +246,15 @@
             if tag in {"lvl", "level"}:
                 token = (TokenType.LEVEL, None)
             else:
                 ansi = self._get_ansicode(tag)
 
                 if ansi is None:
                     raise ValueError(
-                        'Tag "%s" does not correspond to any known ansi directive, '
+                        'Tag "%s" does not correspond to any known color directive, '
                         "make sure you did not misspelled it (or prepend '\\' to escape it)"
                         % markup
                     )
 
                 token = (TokenType.ANSI, ansi)
 
             self._tags.append(tag)
@@ -355,15 +354,15 @@
 class Colorizer:
     @staticmethod
     def prepare_format(string):
         tokens, messages_color_tokens = Colorizer._parse_without_formatting(string)
         return ColoredFormat(tokens, messages_color_tokens)
 
     @staticmethod
-    def prepare_message(string, args=(), kwargs={}):
+    def prepare_message(string, args=(), kwargs={}):  # noqa: B006
         tokens = Colorizer._parse_with_formatting(string, args, kwargs)
         return ColoredMessage(tokens)
 
     @staticmethod
     def prepare_simple_message(string):
         parser = AnsiParser()
         parser.feed(string)
```

### Comparing `loguru-0.6.0/loguru/_ctime_functions.py` & `loguru-0.7.0/loguru/_ctime_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import os
 
 
 def load_ctime_functions():
     if os.name == "nt":
         import win32_setctime
 
-        def get_ctime(filepath):
+        def get_ctime_windows(filepath):
             return os.stat(filepath).st_ctime
 
-        def set_ctime(filepath, timestamp):
+        def set_ctime_windows(filepath, timestamp):
             if not win32_setctime.SUPPORTED:
                 return
 
             try:
                 win32_setctime.setctime(filepath, timestamp)
             except (OSError, ValueError):
                 pass
 
+        return get_ctime_windows, set_ctime_windows
+
     elif hasattr(os.stat_result, "st_birthtime"):
 
-        def get_ctime(filepath):
+        def get_ctime_macos(filepath):
             return os.stat(filepath).st_birthtime
 
-        def set_ctime(filepath, timestamp):
+        def set_ctime_macos(filepath, timestamp):
             pass
 
+        return get_ctime_macos, set_ctime_macos
+
     elif hasattr(os, "getxattr") and hasattr(os, "setxattr"):
 
-        def get_ctime(filepath):
+        def get_ctime_linux(filepath):
             try:
                 return float(os.getxattr(filepath, b"user.loguru_crtime"))
             except OSError:
                 return os.stat(filepath).st_mtime
 
-        def set_ctime(filepath, timestamp):
+        def set_ctime_linux(filepath, timestamp):
             try:
                 os.setxattr(filepath, b"user.loguru_crtime", str(timestamp).encode("ascii"))
             except OSError:
                 pass
 
-    else:
+        return get_ctime_linux, set_ctime_linux
 
-        def get_ctime(filepath):
-            return os.stat(filepath).st_mtime
+    def get_ctime_fallback(filepath):
+        return os.stat(filepath).st_mtime
 
-        def set_ctime(filepath, timestamp):
-            pass
+    def set_ctime_fallback(filepath, timestamp):
+        pass
 
-    return get_ctime, set_ctime
+    return get_ctime_fallback, set_ctime_fallback
 
 
 get_ctime, set_ctime = load_ctime_functions()
```

### Comparing `loguru-0.6.0/loguru/_datetime.py` & `loguru-0.7.0/loguru/_datetime.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from time import localtime, strftime
 
 tokens = r"H{1,2}|h{1,2}|m{1,2}|s{1,2}|S{1,6}|YYYY|YY|M{1,4}|D{1,4}|Z{1,2}|zz|A|X|x|E|Q|dddd|ddd|d"
 
 pattern = re.compile(r"(?:{0})|\[(?:{0}|!UTC)\]".format(tokens))
 
 
-class datetime(datetime_):
+class datetime(datetime_):  # noqa: N801
     def __format__(self, spec):
         if spec.endswith("!UTC"):
             dt = self.astimezone(timezone.utc)
             spec = spec[:-4]
         else:
             dt = self
 
@@ -75,21 +75,22 @@
             except KeyError:
                 return m.group(0)[1:-1]
 
         return pattern.sub(get, spec)
 
 
 def aware_now():
-    now = datetime.now()
+    now = datetime_.now()
     timestamp = now.timestamp()
     local = localtime(timestamp)
 
     try:
         seconds = local.tm_gmtoff
         zone = local.tm_zone
     except AttributeError:
-        offset = datetime.fromtimestamp(timestamp) - datetime.utcfromtimestamp(timestamp)
+        offset = datetime_.fromtimestamp(timestamp) - datetime_.utcfromtimestamp(timestamp)
         seconds = offset.total_seconds()
         zone = strftime("%Z")
 
     tzinfo = timezone(timedelta(seconds=seconds), zone)
-    return now.replace(tzinfo=tzinfo)
+
+    return datetime.combine(now.date(), now.time().replace(tzinfo=tzinfo))
```

### Comparing `loguru-0.6.0/loguru/_defaults.py` & `loguru-0.7.0/loguru/_defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,32 +42,32 @@
 LOGURU_BACKTRACE = env("LOGURU_BACKTRACE", bool, True)
 LOGURU_DIAGNOSE = env("LOGURU_DIAGNOSE", bool, True)
 LOGURU_ENQUEUE = env("LOGURU_ENQUEUE", bool, False)
 LOGURU_CATCH = env("LOGURU_CATCH", bool, True)
 
 LOGURU_TRACE_NO = env("LOGURU_TRACE_NO", int, 5)
 LOGURU_TRACE_COLOR = env("LOGURU_TRACE_COLOR", str, "<cyan><bold>")
-LOGURU_TRACE_ICON = env("LOGURU_TRACE_ICON", str, "✏️")  # Pencil
+LOGURU_TRACE_ICON = env("LOGURU_TRACE_ICON", str, "\u270F\uFE0F")  # Pencil
 
 LOGURU_DEBUG_NO = env("LOGURU_DEBUG_NO", int, 10)
 LOGURU_DEBUG_COLOR = env("LOGURU_DEBUG_COLOR", str, "<blue><bold>")
-LOGURU_DEBUG_ICON = env("LOGURU_DEBUG_ICON", str, "🐞")  # Lady Beetle
+LOGURU_DEBUG_ICON = env("LOGURU_DEBUG_ICON", str, "\U0001F41E")  # Lady Beetle
 
 LOGURU_INFO_NO = env("LOGURU_INFO_NO", int, 20)
 LOGURU_INFO_COLOR = env("LOGURU_INFO_COLOR", str, "<bold>")
-LOGURU_INFO_ICON = env("LOGURU_INFO_ICON", str, "ℹ️")  # Information
+LOGURU_INFO_ICON = env("LOGURU_INFO_ICON", str, "\u2139\uFE0F")  # Information
 
 LOGURU_SUCCESS_NO = env("LOGURU_SUCCESS_NO", int, 25)
 LOGURU_SUCCESS_COLOR = env("LOGURU_SUCCESS_COLOR", str, "<green><bold>")
-LOGURU_SUCCESS_ICON = env("LOGURU_SUCCESS_ICON", str, "✔️")  # Heavy Check Mark
+LOGURU_SUCCESS_ICON = env("LOGURU_SUCCESS_ICON", str, "\u2705")  # White Heavy Check Mark
 
 LOGURU_WARNING_NO = env("LOGURU_WARNING_NO", int, 30)
 LOGURU_WARNING_COLOR = env("LOGURU_WARNING_COLOR", str, "<yellow><bold>")
-LOGURU_WARNING_ICON = env("LOGURU_WARNING_ICON", str, "⚠️")  # Warning
+LOGURU_WARNING_ICON = env("LOGURU_WARNING_ICON", str, "\u26A0\uFE0F")  # Warning
 
 LOGURU_ERROR_NO = env("LOGURU_ERROR_NO", int, 40)
 LOGURU_ERROR_COLOR = env("LOGURU_ERROR_COLOR", str, "<red><bold>")
-LOGURU_ERROR_ICON = env("LOGURU_ERROR_ICON", str, "❌")  # Cross Mark
+LOGURU_ERROR_ICON = env("LOGURU_ERROR_ICON", str, "\u274C")  # Cross Mark
 
 LOGURU_CRITICAL_NO = env("LOGURU_CRITICAL_NO", int, 50)
 LOGURU_CRITICAL_COLOR = env("LOGURU_CRITICAL_COLOR", str, "<RED><bold>")
-LOGURU_CRITICAL_ICON = env("LOGURU_CRITICAL_ICON", str, "☠️")  # Skull and Crossbones
+LOGURU_CRITICAL_ICON = env("LOGURU_CRITICAL_ICON", str, "\u2620\uFE0F")  # Skull and Crossbones
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `loguru-0.6.0/loguru/_error_interceptor.py` & `loguru-0.7.0/loguru/_error_interceptor.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_file_sink.py` & `loguru-0.7.0/loguru/_file_sink.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import datetime as datetime_
+import datetime
 import decimal
 import glob
 import numbers
 import os
 import shutil
 import string
 from functools import partial
+from stat import ST_DEV, ST_INO
 
 from . import _string_parsers as string_parsers
 from ._ctime_functions import get_ctime, set_ctime
-from ._datetime import aware_now, datetime
+from ._datetime import aware_now
 
 
 def generate_rename_path(root, ext, creation_time):
-    creation_datetime = datetime.fromtimestamp(creation_time)
+    creation_datetime = datetime.datetime.fromtimestamp(creation_time)
     date = FileDateFormatter(creation_datetime)
 
     renamed_path = "{}.{}{}".format(root, date, ext)
     counter = 1
 
     while os.path.exists(renamed_path):
         counter += 1
@@ -73,29 +74,29 @@
             return (-os.stat(log).st_mtime, log)
 
         for log in sorted(logs, key=key_log)[number:]:
             os.remove(log)
 
     @staticmethod
     def retention_age(logs, seconds):
-        t = datetime.now().timestamp()
+        t = datetime.datetime.now().timestamp()
         for log in logs:
             if os.stat(log).st_mtime <= t - seconds:
                 os.remove(log)
 
 
 class Rotation:
     @staticmethod
     def forward_day(t):
-        return t + datetime_.timedelta(days=1)
+        return t + datetime.timedelta(days=1)
 
     @staticmethod
     def forward_weekday(t, weekday):
         while True:
-            t += datetime_.timedelta(days=1)
+            t += datetime.timedelta(days=1)
             if t.weekday() == weekday:
                 return t
 
     @staticmethod
     def forward_interval(t, interval):
         return t + interval
 
@@ -107,31 +108,52 @@
     class RotationTime:
         def __init__(self, step_forward, time_init=None):
             self._step_forward = step_forward
             self._time_init = time_init
             self._limit = None
 
         def __call__(self, message, file):
+            record_time = message.record["time"]
+
             if self._limit is None:
                 filepath = os.path.realpath(file.name)
                 creation_time = get_ctime(filepath)
                 set_ctime(filepath, creation_time)
-                start_time = limit = datetime.fromtimestamp(creation_time)
-                if self._time_init is not None:
-                    limit = limit.replace(
-                        hour=self._time_init.hour,
-                        minute=self._time_init.minute,
-                        second=self._time_init.second,
-                        microsecond=self._time_init.microsecond,
-                    )
-                if limit <= start_time:
+                start_time = datetime.datetime.fromtimestamp(
+                    creation_time, tz=datetime.timezone.utc
+                )
+
+                time_init = self._time_init
+
+                if time_init is None:
+                    limit = start_time.astimezone(record_time.tzinfo).replace(tzinfo=None)
                     limit = self._step_forward(limit)
+                else:
+                    limit = datetime.datetime(
+                        start_time.year,
+                        start_time.month,
+                        start_time.day,
+                        time_init.hour,
+                        time_init.minute,
+                        time_init.second,
+                        time_init.microsecond,
+                        record_time.tzinfo if time_init.tzinfo is None else time_init.tzinfo,
+                    )
+
+                    if limit <= start_time:
+                        limit = self._step_forward(limit)
+
+                    if time_init.tzinfo is None:
+                        limit = limit.replace(tzinfo=None)
+
                 self._limit = limit
 
-            record_time = message.record["time"].replace(tzinfo=None)
+            if self._limit.tzinfo is None:
+                record_time = record_time.replace(tzinfo=None)
+
             if record_time >= self._limit:
                 while self._limit <= record_time:
                     self._limit = self._step_forward(self._limit)
                 return True
             return False
 
 
@@ -140,14 +162,15 @@
         self,
         path,
         *,
         rotation=None,
         retention=None,
         compression=None,
         delay=False,
+        watch=False,
         mode="a",
         buffering=1,
         encoding="utf8",
         **kwargs
     ):
         self.encoding = encoding
 
@@ -158,48 +181,100 @@
         self._rotation_function = self._make_rotation_function(rotation)
         self._retention_function = self._make_retention_function(retention)
         self._compression_function = self._make_compression_function(compression)
 
         self._file = None
         self._file_path = None
 
+        self._watch = watch
+        self._file_dev = -1
+        self._file_ino = -1
+
         if not delay:
-            self._initialize_file()
+            path = self._create_path()
+            self._create_dirs(path)
+            self._create_file(path)
 
     def write(self, message):
         if self._file is None:
-            self._initialize_file()
+            path = self._create_path()
+            self._create_dirs(path)
+            self._create_file(path)
+
+        if self._watch:
+            self._reopen_if_needed()
 
         if self._rotation_function is not None and self._rotation_function(message, self._file):
             self._terminate_file(is_rotating=True)
 
         self._file.write(message)
 
-    def _prepare_new_path(self):
+    def stop(self):
+        if self._watch:
+            self._reopen_if_needed()
+
+        self._terminate_file(is_rotating=False)
+
+    async def complete(self):
+        pass
+
+    def _create_path(self):
         path = self._path.format_map({"time": FileDateFormatter()})
-        path = os.path.abspath(path)
+        return os.path.abspath(path)
+
+    def _create_dirs(self, path):
         dirname = os.path.dirname(path)
         os.makedirs(dirname, exist_ok=True)
-        return path
 
-    def _initialize_file(self):
-        path = self._prepare_new_path()
+    def _create_file(self, path):
         self._file = open(path, **self._kwargs)
         self._file_path = path
 
+        if self._watch:
+            fileno = self._file.fileno()
+            result = os.fstat(fileno)
+            self._file_dev = result[ST_DEV]
+            self._file_ino = result[ST_INO]
+
+    def _close_file(self):
+        self._file.flush()
+        self._file.close()
+
+        self._file = None
+        self._file_path = None
+        self._file_dev = -1
+        self._file_ino = -1
+
+    def _reopen_if_needed(self):
+        # Implemented based on standard library:
+        # https://github.com/python/cpython/blob/cb589d1b/Lib/logging/handlers.py#L486
+        if not self._file:
+            return
+
+        filepath = self._file_path
+
+        try:
+            result = os.stat(filepath)
+        except FileNotFoundError:
+            result = None
+
+        if not result or result[ST_DEV] != self._file_dev or result[ST_INO] != self._file_ino:
+            self._close_file()
+            self._create_dirs(filepath)
+            self._create_file(filepath)
+
     def _terminate_file(self, *, is_rotating=False):
         old_path = self._file_path
 
         if self._file is not None:
-            self._file.close()
-            self._file = None
-            self._file_path = None
+            self._close_file()
 
         if is_rotating:
-            new_path = self._prepare_new_path()
+            new_path = self._create_path()
+            self._create_dirs(new_path)
 
             if new_path == old_path:
                 creation_time = get_ctime(old_path)
                 root, ext = os.path.splitext(old_path)
                 renamed_path = generate_rename_path(root, ext, creation_time)
                 os.rename(old_path, renamed_path)
                 old_path = renamed_path
@@ -214,25 +289,16 @@
                     for pattern in self._glob_patterns
                     for file in glob.glob(pattern)
                     if os.path.isfile(file)
                 }
                 self._retention_function(list(logs))
 
         if is_rotating:
-            file = open(new_path, **self._kwargs)
-            set_ctime(new_path, datetime.now().timestamp())
-
-            self._file_path = new_path
-            self._file = file
-
-    def stop(self):
-        self._terminate_file(is_rotating=False)
-
-    async def complete(self):
-        pass
+            self._create_file(new_path)
+            set_ctime(new_path, datetime.datetime.now().timestamp())
 
     @staticmethod
     def _make_glob_patterns(path):
         formatter = string.Formatter()
         tokens = formatter.parse(path)
         escaped = "".join(glob.escape(text) + "*" * (name is not None) for text, name, *_ in tokens)
 
@@ -259,23 +325,23 @@
                 return Rotation.RotationTime(frequency)
             daytime = string_parsers.parse_daytime(rotation)
             if daytime is not None:
                 day, time = daytime
                 if day is None:
                     return FileSink._make_rotation_function(time)
                 if time is None:
-                    time = datetime_.time(0, 0, 0)
+                    time = datetime.time(0, 0, 0)
                 step_forward = partial(Rotation.forward_weekday, weekday=day)
                 return Rotation.RotationTime(step_forward, time)
             raise ValueError("Cannot parse rotation from: '%s'" % rotation)
         elif isinstance(rotation, (numbers.Real, decimal.Decimal)):
             return partial(Rotation.rotation_size, size_limit=rotation)
-        elif isinstance(rotation, datetime_.time):
+        elif isinstance(rotation, datetime.time):
             return Rotation.RotationTime(Rotation.forward_day, rotation)
-        elif isinstance(rotation, datetime_.timedelta):
+        elif isinstance(rotation, datetime.timedelta):
             step_forward = partial(Rotation.forward_interval, interval=rotation)
             return Rotation.RotationTime(step_forward)
         elif callable(rotation):
             return rotation
         else:
             raise TypeError(
                 "Cannot infer rotation for objects of type: '%s'" % type(rotation).__name__
@@ -288,15 +354,15 @@
         elif isinstance(retention, str):
             interval = string_parsers.parse_duration(retention)
             if interval is None:
                 raise ValueError("Cannot parse retention from: '%s'" % retention)
             return FileSink._make_retention_function(interval)
         elif isinstance(retention, int):
             return partial(Retention.retention_count, number=retention)
-        elif isinstance(retention, datetime_.timedelta):
+        elif isinstance(retention, datetime.timedelta):
             return partial(Retention.retention_age, seconds=retention.total_seconds())
         elif callable(retention):
             return retention
         else:
             raise TypeError(
                 "Cannot infer retention for objects of type: '%s'" % type(retention).__name__
             )
```

### Comparing `loguru-0.6.0/loguru/_filters.py` & `loguru-0.7.0/loguru/_filters.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_handler.py` & `loguru-0.7.0/loguru/_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import functools
 import json
 import multiprocessing
 import os
+import threading
+from contextlib import contextmanager
 from threading import Thread
 
 from ._colorizer import Colorizer
 from ._locks_machinery import create_handler_lock
 
 
 def prepare_colored_format(format_, ansi_level):
@@ -60,14 +62,15 @@
 
         self._decolorized_format = None
         self._precolorized_formats = {}
         self._memoize_dynamic_format = None
 
         self._stopped = False
         self._lock = create_handler_lock()
+        self._lock_acquired = threading.local()
         self._queue = None
         self._confirmation_event = None
         self._confirmation_lock = None
         self._owner_process_pid = None
         self._thread = None
 
         if self._is_formatter_dynamic:
@@ -91,14 +94,31 @@
                 target=self._queued_writer, daemon=True, name="loguru-writer-%d" % self._id
             )
             self._thread.start()
 
     def __repr__(self):
         return "(id=%d, level=%d, sink=%s)" % (self._id, self._levelno, self._name)
 
+    @contextmanager
+    def _protected_lock(self):
+        """Acquire the lock, but fail fast if its already acquired by the current thread."""
+        if getattr(self._lock_acquired, "acquired", False):
+            raise RuntimeError(
+                "Could not acquire internal lock because it was already in use (deadlock avoided). "
+                "This likely happened because the logger was re-used inside a sink, a signal "
+                "handler or a '__del__' method. This is not permitted because the logger and its "
+                "handlers are not re-entrant."
+            )
+        self._lock_acquired.acquired = True
+        try:
+            with self._lock:
+                yield
+        finally:
+            self._lock_acquired.acquired = False
+
     def emit(self, record, level_id, from_decorator, is_raw, colored_message):
         try:
             if self._levelno > record["level"].no:
                 return
 
             if self._filter is not None:
                 if not self._filter(record):
@@ -164,29 +184,28 @@
 
             if self._serialize:
                 formatted = self._serialize_record(formatted, record)
 
             str_record = Message(formatted)
             str_record.record = record
 
-            with self._lock:
+            with self._protected_lock():
                 if self._stopped:
                     return
                 if self._enqueue:
                     self._queue.put(str_record)
                 else:
                     self._sink.write(str_record)
-
         except Exception:
             if not self._error_interceptor.should_catch():
                 raise
             self._error_interceptor.print(record)
 
     def stop(self):
-        with self._lock:
+        with self._protected_lock():
             self._stopped = True
             if self._enqueue:
                 if self._owner_process_pid != os.getpid():
                     return
                 self._queue.put(None)
                 self._thread.join()
                 if hasattr(self._queue, "close"):
@@ -203,15 +222,15 @@
             self._confirmation_event.wait()
             self._confirmation_event.clear()
 
     async def complete_async(self):
         if self._enqueue and self._owner_process_pid != os.getpid():
             return
 
-        with self._lock:
+        with self._protected_lock():
             await self._sink.complete()
 
     def update_format(self, level_id):
         if not self._colorize or self._is_formatter_dynamic:
             return
         ansi_code = self._levels_ansi_codes[level_id]
         self._precolorized_formats[level_id] = self._formatter.colorize(ansi_code)
@@ -224,15 +243,15 @@
     def _serialize_record(text, record):
         exception = record["exception"]
 
         if exception is not None:
             exception = {
                 "type": None if exception.type is None else exception.type.__name__,
                 "value": exception.value,
-                "traceback": bool(record["exception"].traceback),
+                "traceback": bool(exception.traceback),
             }
 
         serializable = {
             "text": text,
             "record": {
                 "elapsed": {
                     "repr": record["elapsed"],
@@ -268,45 +287,43 @@
         lock = create_handler_lock()
 
         while True:
             try:
                 message = queue.get()
             except Exception:
                 with lock:
-                    if not self._error_interceptor.should_catch():
-                        raise
                     self._error_interceptor.print(None)
                 continue
 
             if message is None:
                 break
 
             if message is True:
                 self._confirmation_event.set()
                 continue
 
             with lock:
                 try:
                     self._sink.write(message)
                 except Exception:
-                    if not self._error_interceptor.should_catch():
-                        raise
                     self._error_interceptor.print(message.record)
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state["_lock"] = None
+        state["_lock_acquired"] = None
         state["_memoize_dynamic_format"] = None
         if self._enqueue:
             state["_sink"] = None
             state["_thread"] = None
             state["_owner_process"] = None
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._lock = create_handler_lock()
+        self._lock_acquired = threading.local()
         if self._is_formatter_dynamic:
             if self._colorize:
                 self._memoize_dynamic_format = memoize(prepare_colored_format)
             else:
                 self._memoize_dynamic_format = memoize(prepare_stripped_format)
```

### Comparing `loguru-0.6.0/loguru/_locks_machinery.py` & `loguru-0.7.0/loguru/_locks_machinery.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_logger.py` & `loguru-0.7.0/loguru/_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .. |patch| replace:: :meth:`~Logger.patch()`
 .. |opt| replace:: :meth:`~Logger.opt()`
 .. |log| replace:: :meth:`~Logger.log()`
 .. |level| replace:: :meth:`~Logger.level()`
 .. |enable| replace:: :meth:`~Logger.enable()`
 .. |disable| replace:: :meth:`~Logger.disable()`
 
+.. |Any| replace:: :obj:`~typing.Any`
 .. |str| replace:: :class:`str`
 .. |int| replace:: :class:`int`
 .. |bool| replace:: :class:`bool`
 .. |tuple| replace:: :class:`tuple`
 .. |namedtuple| replace:: :func:`namedtuple<collections.namedtuple>`
 .. |list| replace:: :class:`list`
 .. |dict| replace:: :class:`dict`
@@ -64,15 +65,15 @@
 
 .. |better_exceptions| replace:: ``better_exceptions``
 .. _better_exceptions: https://github.com/Qix-/better-exceptions
 
 .. _Pendulum: https://pendulum.eustace.io/docs/#tokens
 .. _@sdispater: https://github.com/sdispater
 .. _@Qix-: https://github.com/Qix-
-.. _Formatting directives: https://docs.python.org/3/library/string.html#format-string-syntax
+.. _formatting directives: https://docs.python.org/3/library/string.html#format-string-syntax
 .. _reentrant: https://en.wikipedia.org/wiki/Reentrancy_(computing)
 """
 import builtins
 import contextlib
 import functools
 import itertools
 import logging
@@ -155,17 +156,24 @@
                 _defaults.LOGURU_CRITICAL_NO,
                 _defaults.LOGURU_CRITICAL_COLOR,
                 _defaults.LOGURU_CRITICAL_ICON,
             ),
         ]
         self.levels = {level.name: level for level in levels}
         self.levels_ansi_codes = {
-            name: Colorizer.ansify(level.color) for name, level in self.levels.items()
+            **{name: Colorizer.ansify(level.color) for name, level in self.levels.items()},
+            None: "",
+        }
+
+        # Cache used internally to quickly access level attributes based on their name or severity.
+        # It can also contain integers as keys, it serves to avoid calling "isinstance()" repeatedly
+        # when "logger.log()" is used.
+        self.levels_lookup = {
+            name: (name, name, level.no, level.icon) for name, level in self.levels.items()
         }
-        self.levels_ansi_codes[None] = ""
 
         self.handlers_count = itertools.count()
         self.handlers = {}
 
         self.extra = {}
         self.patcher = None
 
@@ -205,17 +213,17 @@
     When a message is logged, a "record" is associated with it. This record is a dict which contains
     information about the logging context: time, function, file, line, thread, level... It also
     contains the ``__name__`` of the module, this is why you don't need named loggers.
 
     You should not instantiate a |Logger| by yourself, use ``from loguru import logger`` instead.
     """
 
-    def __init__(self, core, exception, depth, record, lazy, colors, raw, capture, patcher, extra):
+    def __init__(self, core, exception, depth, record, lazy, colors, raw, capture, patchers, extra):
         self._core = core
-        self._options = (exception, depth, record, lazy, colors, raw, capture, patcher, extra)
+        self._options = (exception, depth, record, lazy, colors, raw, capture, patchers, extra)
 
     def __repr__(self):
         return "<loguru.logger handlers=%r>" % list(self._core.handlers.values())
 
     def add(
         self,
         sink,
@@ -255,15 +263,15 @@
         backtrace : |bool|, optional
             Whether the exception trace formatted should be extended upward, beyond the catching
             point, to show the full stacktrace which generated the error.
         diagnose : |bool|, optional
             Whether the exception trace should display the variables values to eases the debugging.
             This should be set to ``False`` in production to avoid leaking sensitive data.
         enqueue : |bool|, optional
-            Whether the messages to be logged should first pass through a multiprocess-safe queue
+            Whether the messages to be logged should first pass through a multiprocessing-safe queue
             before reaching the sink. This is useful while logging to a file through multiple
             processes. This also has the advantage of making logging calls non-blocking.
         catch : |bool|, optional
             Whether errors occurring while sink handles logs messages should be automatically
             caught. If ``True``, an exception message is displayed on |sys.stderr| but the exception
             is not propagated to the caller, preventing your app to crash.
         **kwargs
@@ -292,14 +300,17 @@
             A directive filtering old files that should be removed during rotation or end of
             program.
         compression : |str| or |callable|_, optional
             A compression or archive format to which log files should be converted at closure.
         delay : |bool|, optional
             Whether the file should be created as soon as the sink is configured, or delayed until
             first logged message. It defaults to ``False``.
+        watch : |bool|, optional
+            Whether or not the file should be watched and re-opened when deleted or changed (based
+            on its device and inode properties) by an external program. It defaults to ``False``.
         mode : |str|, optional
             The opening mode as for built-in |open| function. It defaults to ``"a"`` (open the
             file in appending mode).
         buffering : |int|, optional
             The buffering policy as for built-in |open| function. It defaults to ``1`` (line
             buffered file).
         encoding : |str|, optional
@@ -418,19 +429,22 @@
         .. _record:
 
         .. rubric:: The record dict
 
         The record is just a Python dict, accessible from sinks by ``message.record``. It contains
         all contextual information of the logging call (time, function, file, line, level, etc.).
 
-        Each of its key can be used in the handler's ``format`` so the corresponding value is
-        properly displayed in the logged message (e.g. ``"{level}"`` -> ``"INFO"``). Some record's
-        values are objects with two or more attributes, these can be formatted with ``"{key.attr}"``
-        (``"{key}"`` would display one by default). `Formatting directives`_ like ``"{key: >3}"``
-        also works and is particularly useful for time (see below).
+        Each of the record keys can be used in the handler's ``format`` so the corresponding value
+        is properly displayed in the logged message (e.g. ``"{level}"`` will return ``"INFO"``).
+        Some records' values are objects with two or more attributes. These can be formatted with
+        ``"{key.attr}"`` (``"{key}"`` would display one by default).
+
+        Note that you can use any `formatting directives`_ available in Python's ``str.format()``
+        method (e.g. ``"{key: >3}"`` will right-align and pad to a width of 3 characters). This is
+        particularly useful for time formatting (see below).
 
         +------------+---------------------------------+----------------------------+
         | Key        | Description                     | Attributes                 |
         +============+=================================+============================+
         | elapsed    | The time elapsed since the      | See |timedelta|            |
         |            | start of the program            |                            |
         +------------+---------------------------------+----------------------------+
@@ -785,15 +799,17 @@
             if colorize is None:
                 colorize = False
 
             wrapped_sink = StandardSink(sink)
             encoding = getattr(sink, "encoding", None)
             terminator = ""
             exception_prefix = "\n"
-        elif iscoroutinefunction(sink) or iscoroutinefunction(getattr(sink, "__call__", None)):
+        elif iscoroutinefunction(sink) or iscoroutinefunction(
+            getattr(sink, "__call__", None)  # noqa: B004
+        ):
             name = getattr(sink, "__name__", None) or repr(sink)
 
             if colorize is None:
                 colorize = False
 
             loop = kwargs.pop("loop", None)
 
@@ -804,15 +820,15 @@
             # running loop in Python 3.5.2 and earlier versions, see python/asyncio#452.
             if enqueue and loop is None:
                 try:
                     loop = _asyncio_loop.get_running_loop()
                 except RuntimeError as e:
                     raise ValueError(
                         "An event loop is required to add a coroutine sink with `enqueue=True`, "
-                        "but but none has been passed as argument and none is currently running."
+                        "but none has been passed as argument and none is currently running."
                     ) from e
 
             coro = sink if iscoroutinefunction(sink) else sink.__call__
             wrapped_sink = AsyncSink(coro, loop, error_interceptor)
             encoding = "utf8"
             terminator = "\n"
             exception_prefix = ""
@@ -1067,18 +1083,20 @@
         """
 
         with self._core.lock:
             handlers = self._core.handlers.copy()
             for handler in handlers.values():
                 handler.complete_queue()
 
+        logger = self
+
         class AwaitableCompleter:
-            def __await__(self_):
-                with self._core.lock:
-                    handlers = self._core.handlers.copy()
+            def __await__(self):
+                with logger._core.lock:
+                    handlers = logger._core.handlers.copy()
                     for handler in handlers.values():
                         yield from handler.complete_async().__await__()
 
         return AwaitableCompleter()
 
     def catch(
         self,
@@ -1115,15 +1133,15 @@
             Whether the exception should be raised again and hence propagated to the caller.
         onerror : |callable|_, optional
             A function that will be called if an error occurs, once the message has been logged.
             It should accept the exception instance as it sole argument.
         exclude : |Exception|, optional
             A type of exception (or a tuple of types) that will be purposely ignored and hence
             propagated to the caller without being logged.
-        default : optional
+        default : |Any|, optional
             The value to be returned by the decorated function if an error occurred without being
             re-raised.
         message : |str|, optional
             The message that will be automatically logged if an exception occurs. Note that it will
             be formatted with the ``record`` attribute.
 
         Returns
@@ -1166,47 +1184,54 @@
         ...     1 / 0
         """
         if callable(exception) and (
             not isclass(exception) or not issubclass(exception, BaseException)
         ):
             return self.catch()(exception)
 
+        logger = self
+
         class Catcher:
-            def __init__(self_, from_decorator):
-                self_._from_decorator = from_decorator
+            def __init__(self, from_decorator):
+                self._from_decorator = from_decorator
 
-            def __enter__(self_):
+            def __enter__(self):
                 return None
 
-            def __exit__(self_, type_, value, traceback_):
+            def __exit__(self, type_, value, traceback_):
                 if type_ is None:
                     return
 
                 if not issubclass(type_, exception):
                     return False
 
                 if exclude is not None and issubclass(type_, exclude):
                     return False
 
-                from_decorator = self_._from_decorator
-                _, depth, _, *options = self._options
+                from_decorator = self._from_decorator
+                _, depth, _, *options = logger._options
 
                 if from_decorator:
                     depth += 1
 
                 catch_options = [(type_, value, traceback_), depth, True] + options
-                level_id, static_level_no = self._dynamic_level(level)
-                self._log(level_id, static_level_no, from_decorator, catch_options, message, (), {})
+                logger._log(level, from_decorator, catch_options, message, (), {})
 
                 if onerror is not None:
                     onerror(value)
 
                 return not reraise
 
-            def __call__(_, function):
+            def __call__(self, function):
+                if isclass(function):
+                    raise TypeError(
+                        "Invalid object decorated with 'catch()', it must be a function, "
+                        "not a class (tried to wrap '%s')" % function.__name__
+                    )
+
                 catcher = Catcher(True)
 
                 if iscoroutinefunction(function):
 
                     async def catch_wrapper(*args, **kwargs):
                         with catcher:
                             return await function(*args, **kwargs)
@@ -1326,15 +1351,15 @@
                 "The 'ansi' parameter is deprecated, please use 'colors' instead",
                 DeprecationWarning,
             )
 
         args = self._options[-2:]
         return Logger(self._core, exception, depth, record, lazy, colors, raw, capture, *args)
 
-    def bind(__self, **kwargs):
+    def bind(__self, **kwargs):  # noqa: N805
         """Bind attributes to the ``extra`` dict of each logged message record.
 
         This is used to add custom context to each logging call.
 
         Parameters
         ----------
         **kwargs
@@ -1363,15 +1388,15 @@
         >>> instance_2.call("Second instance")
         127.0.0.1 - Second instance
         """
         *options, extra = __self._options
         return Logger(__self._core, *options, {**extra, **kwargs})
 
     @contextlib.contextmanager
-    def contextualize(__self, **kwargs):
+    def contextualize(__self, **kwargs):  # noqa: N805
         """Bind attributes to the context-local ``extra`` dict while inside the ``with`` block.
 
         Contrary to |bind| there is no ``logger`` returned, the ``extra`` dict is modified in-place
         and updated globally. Most importantly, it uses |contextvars| which means that
         contextualized values are unique to each threads and asynchronous tasks.
 
         The ``extra`` dict will retrieve its initial state once the context manager is exited.
@@ -1419,14 +1444,17 @@
         advanced modifications of the record emitted while logging a message. The function is called
         once before sending the log message to the different handlers.
 
         It is recommended to apply modification on the ``record["extra"]`` dict rather than on the
         ``record`` dict itself, as some values are used internally by `Loguru`, and modify them may
         produce unexpected results.
 
+        The logger can be patched multiple times. In this case, the functions are called in the
+        same order as they are added.
+
         Parameters
         ----------
         patcher: |callable|_
             The function to which the record dict will be passed as the sole argument. This function
             is in charge of updating the record in-place, the function does not need to return any
             value, the modified record object will be re-used.
 
@@ -1450,16 +1478,16 @@
         ...     return wrapped
 
         >>> def recv_record_from_network(pipe):
         ...     record = pickle.loads(pipe.read())
         ...     level, message = record["level"], record["message"]
         ...     logger.patch(lambda r: r.update(record)).log(level, message)
         """
-        *options, _, extra = self._options
-        return Logger(self._core, *options, patcher, extra)
+        *options, patchers, extra = self._options
+        return Logger(self._core, *options, patchers + [patcher], extra)
 
     def level(self, name, no=None, color=None, icon=None):
         """Add, update or retrieve a logging level.
 
         Logging levels are defined by their ``name`` to which a severity ``no``, an ansi ``color``
         tag and an ``icon`` are associated and possibly modified at run-time. To |log| to a custom
         level, you should necessarily use its name, the severity number is not linked back to levels
@@ -1550,14 +1578,15 @@
 
         ansi = Colorizer.ansify(color)
         level = Level(name, no, color, icon)
 
         with self._core.lock:
             self._core.levels[name] = level
             self._core.levels_ansi_codes[name] = ansi
+            self._core.levels_lookup[name] = (name, name, no, icon)
             for handler in self._core.handlers.values():
                 handler.update_format(name)
 
         return level
 
     def disable(self, name):
         """Disable logging of messages coming from ``name`` module and its children.
@@ -1731,15 +1760,15 @@
                 if n is not None and (n + ".")[: len(name)] == name:
                     enabled[n] = status
 
             self._core.activation_list = activation_list
             self._core.enabled = enabled
 
     @staticmethod
-    def parse(file, pattern, *, cast={}, chunk=2 ** 16):
+    def parse(file, pattern, *, cast={}, chunk=2**16):  # noqa: B006
         """Parse raw logs and extract each entry as a |dict|.
 
         The logging format has to be specified as the regex ``pattern``, it will then be
         used to parse the ``file`` and retrieve each entry based on the named groups present
         in the regex.
 
         Parameters
@@ -1840,21 +1869,42 @@
                 break
 
             if len(matches) > 1:
                 end = matches[-2].end()
                 buffer = buffer[end:]
                 yield from matches[:-1]
 
-    def _log(self, level_id, static_level_no, from_decorator, options, message, args, kwargs):
+    def _log(self, level, from_decorator, options, message, args, kwargs):
         core = self._core
 
         if not core.handlers:
             return
 
-        (exception, depth, record, lazy, colors, raw, capture, patcher, extra) = options
+        try:
+            level_id, level_name, level_no, level_icon = core.levels_lookup[level]
+        except (KeyError, TypeError):
+            if isinstance(level, str):
+                raise ValueError("Level '%s' does not exist" % level) from None
+            if not isinstance(level, int):
+                raise TypeError(
+                    "Invalid level, it should be an integer or a string, not: '%s'"
+                    % type(level).__name__
+                ) from None
+            if level < 0:
+                raise ValueError(
+                    "Invalid level value, it should be a positive integer, not: %d" % level
+                ) from None
+            cache = (None, "Level %d" % level, level, " ")
+            level_id, level_name, level_no, level_icon = cache
+            core.levels_lookup[level] = cache
+
+        if level_no < core.min_level:
+            return
+
+        (exception, depth, record, lazy, colors, raw, capture, patchers, extra) = options
 
         frame = get_frame(depth + 2)
 
         try:
             name = frame.f_globals["__name__"]
         except KeyError:
             name = None
@@ -1877,27 +1927,14 @@
                             break
                         enabled[name] = False
                         return
                 enabled[name] = True
 
         current_datetime = aware_now()
 
-        if level_id is None:
-            level_icon = " "
-            level_no = static_level_no
-            level_name = "Level %d" % level_no
-        else:
-            try:
-                level_name, level_no, _, level_icon = core.levels[level_id]
-            except KeyError:
-                raise ValueError("Level '%s' does not exist" % level_id) from None
-
-        if level_no < core.min_level:
-            return
-
         code = frame.f_code
         file_path = code.co_filename
         file_name = basename(file_path)
         thread = current_thread()
         process = current_process()
         elapsed = current_datetime - start_time
 
@@ -1954,75 +1991,56 @@
             log_record["message"] = message.format(*args, **kwargs)
         else:
             colored_message = None
 
         if core.patcher:
             core.patcher(log_record)
 
-        if patcher:
+        for patcher in patchers:
             patcher(log_record)
 
         for handler in core.handlers.values():
             handler.emit(log_record, level_id, from_decorator, raw, colored_message)
 
-    def trace(__self, __message, *args, **kwargs):
+    def trace(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'TRACE'``."""
-        __self._log("TRACE", None, False, __self._options, __message, args, kwargs)
+        __self._log("TRACE", False, __self._options, __message, args, kwargs)
 
-    def debug(__self, __message, *args, **kwargs):
+    def debug(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'DEBUG'``."""
-        __self._log("DEBUG", None, False, __self._options, __message, args, kwargs)
+        __self._log("DEBUG", False, __self._options, __message, args, kwargs)
 
-    def info(__self, __message, *args, **kwargs):
+    def info(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'INFO'``."""
-        __self._log("INFO", None, False, __self._options, __message, args, kwargs)
+        __self._log("INFO", False, __self._options, __message, args, kwargs)
 
-    def success(__self, __message, *args, **kwargs):
+    def success(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'SUCCESS'``."""
-        __self._log("SUCCESS", None, False, __self._options, __message, args, kwargs)
+        __self._log("SUCCESS", False, __self._options, __message, args, kwargs)
 
-    def warning(__self, __message, *args, **kwargs):
+    def warning(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'WARNING'``."""
-        __self._log("WARNING", None, False, __self._options, __message, args, kwargs)
+        __self._log("WARNING", False, __self._options, __message, args, kwargs)
 
-    def error(__self, __message, *args, **kwargs):
+    def error(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'ERROR'``."""
-        __self._log("ERROR", None, False, __self._options, __message, args, kwargs)
+        __self._log("ERROR", False, __self._options, __message, args, kwargs)
 
-    def critical(__self, __message, *args, **kwargs):
+    def critical(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``'CRITICAL'``."""
-        __self._log("CRITICAL", None, False, __self._options, __message, args, kwargs)
+        __self._log("CRITICAL", False, __self._options, __message, args, kwargs)
 
-    def exception(__self, __message, *args, **kwargs):
+    def exception(__self, __message, *args, **kwargs):  # noqa: N805
         r"""Convenience method for logging an ``'ERROR'`` with exception information."""
         options = (True,) + __self._options[1:]
-        __self._log("ERROR", None, False, options, __message, args, kwargs)
+        __self._log("ERROR", False, options, __message, args, kwargs)
 
-    def log(__self, __level, __message, *args, **kwargs):
+    def log(__self, __level, __message, *args, **kwargs):  # noqa: N805
         r"""Log ``message.format(*args, **kwargs)`` with severity ``level``."""
-        level_id, static_level_no = __self._dynamic_level(__level)
-        __self._log(level_id, static_level_no, False, __self._options, __message, args, kwargs)
-
-    @staticmethod
-    @functools.lru_cache(maxsize=32)
-    def _dynamic_level(level):
-
-        if isinstance(level, str):
-            return (level, None)
-
-        if isinstance(level, int):
-            if level < 0:
-                raise ValueError(
-                    "Invalid level value, it should be a positive integer, not: %d" % level
-                )
-            return (None, level)
-
-        raise TypeError(
-            "Invalid level, it should be an integer or a string, not: '%s'" % type(level).__name__
-        )
+        __self._log(__level, False, __self._options, __message, args, kwargs)
 
     def start(self, *args, **kwargs):
         """Deprecated function to |add| a new handler.
 
         Warnings
         --------
         .. deprecated:: 0.2.2
```

### Comparing `loguru-0.6.0/loguru/_recattrs.py` & `loguru-0.7.0/loguru/_recattrs.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_simple_sinks.py` & `loguru-0.7.0/loguru/_simple_sinks.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/loguru/_string_parsers.py` & `loguru-0.7.0/loguru/_string_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         s = float(s)
     except ValueError as e:
         raise ValueError("Invalid float value while parsing size: '%s'" % s) from e
 
     u = "kmgtpezy".index(u.lower()) + 1 if u else 0
     i = 1024 if i else 1000
     b = {"b": 8, "B": 1}[b] if b else 1
-    size = s * i ** u / b
+    size = s * i**u / b
 
     return size
 
 
 def parse_duration(duration):
     duration = duration.strip()
     reg = r"(?:([e\+\-\.\d]+)\s*([a-z]+)[\s\,]*)"
```

### Comparing `loguru-0.6.0/loguru.egg-info/PKG-INFO` & `loguru-0.7.0/loguru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: loguru
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python logging made (stupidly) simple
 Home-page: https://github.com/Delgan/loguru
+Download-URL: https://github.com/Delgan/loguru/archive/0.7.0.tar.gz
 Author: Delgan
 Author-email: delgan.py@gmail.com
 License: MIT license
-Download-URL: https://github.com/Delgan/loguru/archive/0.6.0.tar.gz
 Project-URL: Changelog, https://github.com/Delgan/loguru/blob/master/CHANGELOG.rst
 Project-URL: Documentation, https://loguru.readthedocs.io/en/stable/index.html
 Keywords: loguru,logging,logger,log
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Logging
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -54,15 +54,15 @@
     :alt: Python versions
 
 .. image:: https://img.shields.io/readthedocs/loguru.svg
     :target: https://loguru.readthedocs.io/en/stable/index.html
     :alt: Docs
 
 .. image:: https://img.shields.io/github/workflow/status/Delgan/loguru/Tests/master
-    :target: https://github.com/Delgan/loguru/actions/workflows/tests.yml?query=branch:master
+    :target: https://img.shields.io/github/actions/workflow/status/Delgan/loguru/tests.yml?branch=master
     :alt: Build status
 
 .. image:: https://img.shields.io/codecov/c/github/delgan/loguru/master.svg
     :target: https://codecov.io/gh/delgan/loguru/branch/master
     :alt: Coverage
 
 .. image:: https://img.shields.io/codacy/grade/be7337df3c0d40d1929eb7f79b1671a6.svg
@@ -314,14 +314,16 @@
       File "test.py", line 4, in func
         return a / b
                │   └ 0
                └ 5
 
     ZeroDivisionError: division by zero
 
+Note that this feature won't work on default Python REPL due to unavailable frame data.
+
 
 Structured logging as needed
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Want your logs to be serialized for easier parsing or to pass them around? Using the ``serialize`` argument, each log message will be converted to a JSON string before being sent to the configured sink.
 
 ::
@@ -401,15 +403,15 @@
 
     logger.add("file.log", format="{time:YYYY-MM-DD at HH:mm:ss} | {level} | {message}")
 
 
 Suitable for scripts and libraries
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, he can |enable|_ it again.
+Using the logger in your scripts is easy, and you can |configure|_ it at start. To use `Loguru` from inside a library, remember to never call |add|_ but use |disable|_ instead so logging functions become no-op. If a developer wishes to see your library's logs, they can |enable|_ it again.
 
 ::
 
     # For scripts
     config = {
         "handlers": [
             {"sink": sys.stdout, "format": "{time} - {message}"},
@@ -448,29 +450,29 @@
 
 Want to intercept standard `logging` messages toward your `Loguru` sinks?
 
 ::
 
     class InterceptHandler(logging.Handler):
         def emit(self, record):
-            # Get corresponding Loguru level if it exists
+            # Get corresponding Loguru level if it exists.
             try:
                 level = logger.level(record.levelname).name
             except ValueError:
                 level = record.levelno
 
-            # Find caller from where originated the logged message
-            frame, depth = logging.currentframe(), 2
-            while frame.f_code.co_filename == logging.__file__:
+            # Find caller from where originated the logged message.
+            frame, depth = sys._getframe(6), 6
+            while frame and frame.f_code.co_filename == logging.__file__:
                 frame = frame.f_back
                 depth += 1
 
             logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
-    logging.basicConfig(handlers=[InterceptHandler()], level=0)
+    logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
 
 
 Personalizable defaults through environment variables
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Don't like the default logger formatting? Would prefer another ``DEBUG`` color? `No problem`_::
 
@@ -536,9 +538,7 @@
 
 * `API Reference <https://loguru.readthedocs.io/en/stable/api/logger.html>`_
 * `Help & Guides <https://loguru.readthedocs.io/en/stable/resources.html>`_
 * `Type hints <https://loguru.readthedocs.io/en/stable/api/type_hints.html>`_
 * `Contributing <https://loguru.readthedocs.io/en/stable/project/contributing.html>`_
 * `License <https://loguru.readthedocs.io/en/stable/project/license.html>`_
 * `Changelog <https://loguru.readthedocs.io/en/stable/project/changelog.html>`_
-
-
```

### Comparing `loguru-0.6.0/loguru.egg-info/SOURCES.txt` & `loguru-0.7.0/loguru.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,31 +51,35 @@
 tests/test_datetime.py
 tests/test_deepcopy.py
 tests/test_defaults.py
 tests/test_exceptions_catch.py
 tests/test_exceptions_formatting.py
 tests/test_filesink_compression.py
 tests/test_filesink_delay.py
+tests/test_filesink_permissions.py
 tests/test_filesink_retention.py
 tests/test_filesink_rotation.py
+tests/test_filesink_watch.py
 tests/test_formatting.py
 tests/test_get_frame.py
 tests/test_interception.py
 tests/test_levels.py
+tests/test_locks.py
 tests/test_multiprocessing.py
 tests/test_opt.py
 tests/test_parse.py
 tests/test_patch.py
 tests/test_pickling.py
 tests/test_propagation.py
 tests/test_recattr.py
 tests/test_remove.py
 tests/test_repr.py
 tests/test_standard_handler.py
 tests/test_threading.py
+tests/test_type_hinting.py
 tests/exceptions/output/backtrace/chained_expression_direct.txt
 tests/exceptions/output/backtrace/chained_expression_indirect.txt
 tests/exceptions/output/backtrace/chaining_first.txt
 tests/exceptions/output/backtrace/chaining_second.txt
 tests/exceptions/output/backtrace/chaining_third.txt
 tests/exceptions/output/backtrace/enqueue.txt
 tests/exceptions/output/backtrace/enqueue_with_others_handlers.txt
@@ -221,8 +225,9 @@
 tests/exceptions/source/ownership/catch_decorator_from_lib.py
 tests/exceptions/source/ownership/decorated_callback.py
 tests/exceptions/source/ownership/direct.py
 tests/exceptions/source/ownership/indirect.py
 tests/exceptions/source/ownership/string_lib.py
 tests/exceptions/source/ownership/string_source.py
 tests/exceptions/source/ownership/syntaxerror.py
-tests/exceptions/source/ownership/usersite/somelib/__init__.py
+tests/exceptions/source/ownership/usersite/somelib/__init__.py
+tests/typesafety/test_logger.yml
```

### Comparing `loguru-0.6.0/setup.py` & `loguru-0.7.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -41,33 +41,47 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     install_requires=[
         "colorama>=0.3.4 ; sys_platform=='win32'",
         "aiocontextvars>=0.2.0 ; python_version<'3.7'",
         "win32-setctime>=1.0.0 ; sys_platform=='win32'",
     ],
     extras_require={
         "dev": [
-            "black>=19.10b0 ; python_version>='3.6'",
-            "colorama>=0.3.4",
-            "docutils==0.16",
-            "flake8>=3.7.7",
-            "isort>=5.1.1 ; python_version>='3.6'",
-            "tox>=3.9.0",
-            "pytest>=4.6.2",
-            "pytest-cov>=2.7.1",
-            "Sphinx>=4.1.1 ; python_version>='3.6'",
-            "sphinx-autobuild>=0.7.1 ; python_version>='3.6'",
-            "sphinx-rtd-theme>=0.4.3 ; python_version>='3.6'",
+            # Setup.
+            "pre-commit==3.2.1 ; python_version>='3.8'",
+            "tox==3.27.1 ; python_version<'3.8'",
+            "tox==4.4.6 ; python_version>='3.8'",
+            # Testing framework.
+            "pytest==6.1.2 ; python_version<'3.8'",
+            "pytest==7.2.1 ; python_version>='3.8'",
+            "pytest-cov==2.12.1 ; python_version<'3.8'",
+            "pytest-cov==4.0.0 ; python_version>='3.8'",
+            "pytest-mypy-plugins==1.9.3 ; python_version>='3.6' and python_version<'3.8'",
+            "pytest-mypy-plugins==1.10.1 ; python_version>='3.8'",
+            # Testing utils.
+            "colorama==0.4.5 ; python_version<'3.8'",
+            "colorama==0.4.6 ; python_version>='3.8'",
+            "freezegun==1.1.0 ; python_version<'3.8'",
+            "freezegun==1.2.2 ; python_version>='3.8'",
+            # Type checking.
+            "mypy==v0.910 ; python_version<'3.6'",
+            "mypy==v0.971 ; python_version>='3.6' and python_version<'3.7'",
+            "mypy==v0.990 ; python_version>='3.7'",
+            # Docs.
+            "Sphinx==5.3.0 ; python_version>='3.8'",
+            "sphinx-autobuild==2021.3.14 ; python_version>='3.8'",
+            "sphinx-rtd-theme==1.2.0 ; python_version>='3.8'",
         ]
     },
     python_requires=">=3.5",
 )
```

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/chained_expression_direct.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/chained_expression_direct.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/chained_expression_indirect.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/chained_expression_indirect.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/chaining_first.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/chaining_first.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/chaining_second.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/chaining_second.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/chaining_third.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/chaining_third.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/function.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/function.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/head_recursion.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/head_recursion.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/nested.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/nested.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/nested_chained_catch_up.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/nested_chained_catch_up.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/nested_decorator_catch_up.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/nested_decorator_catch_up.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/nested_explicit_catch_up.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/nested_explicit_catch_up.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/nested_wrapping.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/nested_wrapping.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/not_enough_arguments.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/not_enough_arguments.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/raising_recursion.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/raising_recursion.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/suppressed_expression_direct.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/suppressed_expression_direct.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/suppressed_expression_indirect.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/suppressed_expression_indirect.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/tail_recursion.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/tail_recursion.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/backtrace/too_many_arguments.txt` & `loguru-0.7.0/tests/exceptions/output/backtrace/too_many_arguments.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error_custom.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error_custom.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/assertion_error_in_string.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/assertion_error_in_string.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/attributes.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/attributes.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/chained_both.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/chained_both.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/encoding.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/encoding.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/global_variable.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/global_variable.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/keyword_argument.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/keyword_argument.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/multilines_repr.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/multilines_repr.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/no_error_message.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/no_error_message.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/parenthesis.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/parenthesis.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/source_multilines.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/source_multilines.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/syntax_highlighting.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/syntax_highlighting.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/diagnose/truncating.txt` & `loguru-0.7.0/tests/exceptions/output/diagnose/truncating.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/catch_message.txt` & `loguru-0.7.0/tests/exceptions/output/others/catch_message.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/exception_formatting_coroutine.txt` & `loguru-0.7.0/tests/exceptions/output/others/exception_formatting_coroutine.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/exception_formatting_function.txt` & `loguru-0.7.0/tests/exceptions/output/others/exception_formatting_function.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/exception_formatting_generator.txt` & `loguru-0.7.0/tests/exceptions/output/others/exception_formatting_generator.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/nested_with_reraise.txt` & `loguru-0.7.0/tests/exceptions/output/others/nested_with_reraise.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,154 +1,154 @@
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
 ZeroDivisionError: division by zero
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
         │   │  └ 0
         │   └ 1
         └ <function foo at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
     │   └ 0
     └ 1
 
 ZeroDivisionError: division by zero
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 30, in <module>
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 31, in <module>
     baz()
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
-> File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+> File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
 ZeroDivisionError: division by zero
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 30, in <module>
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 31, in <module>
     baz()
     └ <function baz at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
     └ <function bar at 0xDEADBEEF>
 
-> File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+> File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
         │   │  └ 0
         │   └ 1
         └ <function foo at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
     │   └ 0
     └ 1
 
 ZeroDivisionError: division by zero
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
 ZeroDivisionError: division by zero
 
 The above exception was the direct cause of the following exception:
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 22, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 23, in bar
     raise ValueError from e
 ValueError
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
         │   │  └ 0
         │   └ 1
         └ <function foo at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
     │   └ 0
     └ 1
 
 ZeroDivisionError: division by zero
 
 
 The above exception was the direct cause of the following exception:
 
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
     └ <function bar at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 22, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 23, in bar
     raise ValueError from e
 
 ValueError
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
 ZeroDivisionError: division by zero
 
 The above exception was the direct cause of the following exception:
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 30, in <module>
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 31, in <module>
     baz()
-> File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+> File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 22, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 23, in bar
     raise ValueError from e
 ValueError
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 20, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 21, in bar
     f = foo(x, y)
         │   │  └ 0
         │   └ 1
         └ <function foo at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 14, in foo
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 15, in foo
     a / b
     │   └ 0
     └ 1
 
 ZeroDivisionError: division by zero
 
 
 The above exception was the direct cause of the following exception:
 
 
 Traceback (most recent call last):
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 30, in <module>
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 31, in <module>
     baz()
     └ <function baz at 0xDEADBEEF>
 
-> File "tests/exceptions/source/others/nested_with_reraise.py", line 26, in baz
+> File "tests/exceptions/source/others/nested_with_reraise.py", line 27, in baz
     bar(1, 0)
     └ <function bar at 0xDEADBEEF>
 
-  File "tests/exceptions/source/others/nested_with_reraise.py", line 22, in bar
+  File "tests/exceptions/source/others/nested_with_reraise.py", line 23, in bar
     raise ValueError from e
 
 ValueError
```

### Comparing `loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit.txt` & `loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit_none.txt` & `loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit_none.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/others/sys_tracebacklimit_unset.txt` & `loguru-0.7.0/tests/exceptions/output/others/sys_tracebacklimit_unset.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/assertion_from_lib.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/assertion_from_lib.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m20[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m21[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m15[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m16[0m, in [35mtest[0m
     [1massertionerror[0m[1m([0m[1ma[0m[1m,[0m [1mb[0m[1m)[0m
     [36m│              │  └ [0m[36m[1m2[0m
     [36m│              └ [0m[36m[1m1[0m
     [36m└ [0m[36m[1m<function assertionerror at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 22, in assertionerror
     assert x == y
            │    └ 2
            └ 1
 
 [31m[1mAssertionError[0m: [35m[1massert[0m [1mx[0m [35m[1m==[0m [1my[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m15[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m16[0m, in [35mtest[0m
     [1massertionerror[0m[1m([0m[1ma[0m[1m,[0m [1mb[0m[1m)[0m
     [36m│              │  └ [0m[36m[1m2[0m
     [36m│              └ [0m[36m[1m1[0m
     [36m└ [0m[36m[1m<function assertionerror at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 22, in assertionerror
     assert x == y
            │    └ 2
            └ 1
 
 [31m[1mAssertionError[0m: [35m[1massert[0m [1mx[0m [35m[1m==[0m [1my[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m22[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m23[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m15[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m16[0m, in [35mtest[0m
     [1massertionerror[0m[1m([0m[1ma[0m[1m,[0m [1mb[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 22, in assertionerror
     assert x == y
 [31m[1mAssertionError[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m15[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_lib.py[0m", line [33m16[0m, in [35mtest[0m
     [1massertionerror[0m[1m([0m[1ma[0m[1m,[0m [1mb[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 22, in assertionerror
     assert x == y
 [31m[1mAssertionError[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/assertion_from_lib.py", line 15, in test
+  File "tests/exceptions/source/ownership/assertion_from_lib.py", line 16, in test
     assertionerror(a, b)
   File "/usr/lib/python/somelib/__init__.py", line 22, in assertionerror
     assert x == y
 AssertionError
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/assertion_from_local.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/assertion_from_local.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m20[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m21[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m15[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m16[0m, in [35mtest[0m
     [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
     [36m       │    └ [0m[36m[1m2[0m
     [36m       └ [0m[36m[1m1[0m
 
 [31m[1mAssertionError[0m: [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m15[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m16[0m, in [35mtest[0m
     [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
     [36m       │    └ [0m[36m[1m2[0m
     [36m       └ [0m[36m[1m1[0m
 
 [31m[1mAssertionError[0m: [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m22[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m23[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m15[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m16[0m, in [35mtest[0m
     [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
 [31m[1mAssertionError[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m15[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1massertion_from_local.py[0m", line [33m16[0m, in [35mtest[0m
     [35m[1massert[0m [1ma[0m [35m[1m==[0m [1mb[0m
 [31m[1mAssertionError[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/assertion_from_local.py", line 15, in test
+  File "tests/exceptions/source/ownership/assertion_from_local.py", line 16, in test
     assert a == b
 AssertionError
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/callback.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/callback.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m22[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m23[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m17[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
     [36m│      └ [0m[36m[1m<function test.<locals>.callback at 0xDEADBEEF>[0m
     [36m└ [0m[36m[1m<function callme at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m14[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m15[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
     [36m│      └ [0m[36m[1m<function test.<locals>.callback at 0xDEADBEEF>[0m
     [36m└ [0m[36m[1m<function callme at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m14[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m15[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m24[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m25[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m17[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m14[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m15[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m14[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcallback.py[0m", line [33m15[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/callback.py", line 17, in test
+  File "tests/exceptions/source/ownership/callback.py", line 18, in test
     callme(callback)
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "tests/exceptions/source/ownership/callback.py", line 14, in callback
+  File "tests/exceptions/source/ownership/callback.py", line 15, in callback
     divide(1, 0)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/catch_decorator.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/catch_decorator.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m20[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m21[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m17[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m18[0m, in [35mtest[0m
     [1mfoo[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function test.<locals>.foo at 0xDEADBEEF>[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m15[0m, in [35mfoo[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m16[0m, in [35mfoo[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m18[0m, in [35mtest[0m
     [1mfoo[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function test.<locals>.foo at 0xDEADBEEF>[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m15[0m, in [35mfoo[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m16[0m, in [35mfoo[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m22[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m23[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m17[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m18[0m, in [35mtest[0m
     [1mfoo[0m[1m([0m[1m)[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m15[0m, in [35mfoo[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m16[0m, in [35mfoo[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m18[0m, in [35mtest[0m
     [1mfoo[0m[1m([0m[1m)[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m15[0m, in [35mfoo[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator.py[0m", line [33m16[0m, in [35mfoo[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/catch_decorator.py", line 17, in test
+  File "tests/exceptions/source/ownership/catch_decorator.py", line 18, in test
     foo()
-  File "tests/exceptions/source/ownership/catch_decorator.py", line 15, in foo
+  File "tests/exceptions/source/ownership/catch_decorator.py", line 16, in foo
     divide(1, 0)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/catch_decorator_from_lib.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/catch_decorator_from_lib.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m20[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m21[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
     [36m│      └ [0m[36m[1m<function test.<locals>.callback at 0xDEADBEEF>[0m
     [36m└ [0m[36m[1m<function callme at 0xDEADBEEF>[0m
 
 > File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m15[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m16[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
@@ -27,48 +27,48 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m15[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m16[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m22[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m23[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m17[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m18[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
 > File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m15[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m16[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m15[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mcatch_decorator_from_lib.py[0m", line [33m16[0m, in [35mcallback[0m
     [1mdivide[0m[1m([0m[34m[1m1[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "tests/exceptions/source/ownership/catch_decorator_from_lib.py", line 15, in callback
+  File "tests/exceptions/source/ownership/catch_decorator_from_lib.py", line 16, in callback
     divide(1, 0)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/decorated_callback.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/decorated_callback.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m21[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m22[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m18[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m19[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
     [36m│      └ [0m[36m[1m<function test.<locals>.callback at 0xDEADBEEF>[0m
     [36m└ [0m[36m[1m<function callme at 0xDEADBEEF>[0m
 
 > File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m16[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m17[0m, in [35mcallback[0m
     [1ma[0m [35m[1m/[0m [1mb[0m
     [36m│   └ [0m[36m[1m0[0m
     [36m└ [0m[36m[1m1[0m
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
     └ <function test.<locals>.callback at 0xDEADBEEF>
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m16[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m17[0m, in [35mcallback[0m
     [1ma[0m [35m[1m/[0m [1mb[0m
     [36m│   └ [0m[36m[1m0[0m
     [36m└ [0m[36m[1m1[0m
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m23[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m24[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m18[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m19[0m, in [35mtest[0m
     [1mcallme[0m[1m([0m[1mcallback[0m[1m)[0m
 > File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m16[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m17[0m, in [35mcallback[0m
     [1ma[0m [35m[1m/[0m [1mb[0m
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m16[0m, in [35mcallback[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdecorated_callback.py[0m", line [33m17[0m, in [35mcallback[0m
     [1ma[0m [35m[1m/[0m [1mb[0m
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
   File "/usr/lib/python/somelib/__init__.py", line 10, in callme
     callback()
-  File "tests/exceptions/source/ownership/decorated_callback.py", line 16, in callback
+  File "tests/exceptions/source/ownership/decorated_callback.py", line 17, in callback
     a / b
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/direct.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/direct.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m19[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m20[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 10
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 10
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m21[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m22[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mdirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/direct.py", line 14, in test
+  File "tests/exceptions/source/ownership/direct.py", line 15, in test
     divide(10, 0)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/indirect.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/indirect.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m19[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m20[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide_indirect[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide_indirect at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 6, in divide_indirect
     divide(a, b)
     │      │  └ 0
     │      └ 10
@@ -19,15 +19,15 @@
     │   └ 0
     └ 10
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide_indirect[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
     [36m└ [0m[36m[1m<function divide_indirect at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 6, in divide_indirect
     divide(a, b)
     │      │  └ 0
     │      └ 10
@@ -36,34 +36,34 @@
     x / y
     │   └ 0
     └ 10
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m21[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m22[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide_indirect[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 6, in divide_indirect
     divide(a, b)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mindirect.py[0m", line [33m15[0m, in [35mtest[0m
     [1mdivide_indirect[0m[1m([0m[34m[1m10[0m[1m,[0m [34m[1m0[0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 6, in divide_indirect
     divide(a, b)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/indirect.py", line 14, in test
+  File "tests/exceptions/source/ownership/indirect.py", line 15, in test
     divide_indirect(10, 0)
   File "/usr/lib/python/somelib/__init__.py", line 6, in divide_indirect
     divide(a, b)
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/string_lib.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/string_lib.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m19[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m20[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m15[0m, in [35mtest[0m
     [1mexecute[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function execute at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 14, in execute
     exec("divide(1, 0)")
   File "<string>", line 1, in <module>
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
@@ -17,52 +17,52 @@
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m15[0m, in [35mtest[0m
     [1mexecute[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function execute at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 14, in execute
     exec("divide(1, 0)")
   File "<string>", line 1, in <module>
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
     │   └ 0
     └ 1
 
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m21[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m22[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m15[0m, in [35mtest[0m
     [1mexecute[0m[1m([0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 14, in execute
     exec("divide(1, 0)")
   File "<string>", line 1, in <module>
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1mstring_lib.py[0m", line [33m15[0m, in [35mtest[0m
     [1mexecute[0m[1m([0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 14, in execute
     exec("divide(1, 0)")
   File "<string>", line 1, in <module>
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 [31m[1mZeroDivisionError[0m:[1m division by zero[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/string_lib.py", line 14, in test
+  File "tests/exceptions/source/ownership/string_lib.py", line 15, in test
     execute()
   File "/usr/lib/python/somelib/__init__.py", line 14, in execute
     exec("divide(1, 0)")
   File "<string>", line 1, in <module>
   File "/usr/lib/python/somelib/__init__.py", line 2, in divide
     x / y
 ZeroDivisionError: division by zero
```

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/string_source.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/string_source.txt`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/output/ownership/syntaxerror.txt` & `loguru-0.7.0/tests/exceptions/output/ownership/syntaxerror.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m19[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m20[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mTrue[0m[1m)[0m
     [36m└ [0m[36m[1m<function test at 0xDEADBEEF>[0m
 
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m15[0m, in [35mtest[0m
     [1msyntaxerror[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function syntaxerror at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 18, in syntaxerror
     exec("foo =")
   File "<string>", line 1
     foo =
          ^
 
 [31m[1mSyntaxError[0m:[1m invalid syntax[0m
 
 [33m[1mTraceback (most recent call last):[0m
 
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m15[0m, in [35mtest[0m
     [1msyntaxerror[0m[1m([0m[1m)[0m
     [36m└ [0m[36m[1m<function syntaxerror at 0xDEADBEEF>[0m
 
   File "/usr/lib/python/somelib/__init__.py", line 18, in syntaxerror
     exec("foo =")
   File "<string>", line 1
     foo =
          ^
 
 [31m[1mSyntaxError[0m:[1m invalid syntax[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m21[0m, in [35m<module>[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m22[0m, in [35m<module>[0m
     [1mtest[0m[1m([0m[1mbacktrace[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mcolorize[0m[35m[1m=[0m[36m[1mTrue[0m[1m,[0m [1mdiagnose[0m[35m[1m=[0m[36m[1mFalse[0m[1m)[0m
-> File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m14[0m, in [35mtest[0m
+> File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m15[0m, in [35mtest[0m
     [1msyntaxerror[0m[1m([0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 18, in syntaxerror
     exec("foo =")
   File "<string>", line 1
     foo =
          ^
 [31m[1mSyntaxError[0m:[1m invalid syntax[0m
 
 [33m[1mTraceback (most recent call last):[0m
-  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m14[0m, in [35mtest[0m
+  File "[32mtests/exceptions/source/ownership/[0m[32m[1msyntaxerror.py[0m", line [33m15[0m, in [35mtest[0m
     [1msyntaxerror[0m[1m([0m[1m)[0m
   File "/usr/lib/python/somelib/__init__.py", line 18, in syntaxerror
     exec("foo =")
   File "<string>", line 1
     foo =
          ^
 [31m[1mSyntaxError[0m:[1m invalid syntax[0m
 
 Traceback (most recent call last):
-  File "tests/exceptions/source/ownership/syntaxerror.py", line 14, in test
+  File "tests/exceptions/source/ownership/syntaxerror.py", line 15, in test
     syntaxerror()
   File "/usr/lib/python/somelib/__init__.py", line 18, in syntaxerror
     exec("foo =")
   File "<string>", line 1
     foo =
          ^
 SyntaxError: invalid syntax
```

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/chained_expression_direct.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/chained_expression_direct.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/chaining_second.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/chaining_second.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/chaining_third.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/chaining_third.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/enqueue_with_others_handlers.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/enqueue_with_others_handlers.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/missing_attributes_traceback_objects.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/missing_attributes_traceback_objects.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     x / y
 
 
 def foo():
     div(a, b)
 
 
-# See Twisted: https://git.io/fjJ48
-# See Billiard: https://git.io/fjJ44
+# See Twisted: https://github.com/twisted/twisted/blob/29cbe/src/twisted/python/failure.py#L175-L181
+# See Billiard: https://github.com/celery/billiard/blob/529a3/billiard/einfo.py#L11-L26
 fake_code = namedtuple("fake_code", ("co_filename", "co_name"))
 fake_frame = namedtuple("fake_frame", ("f_back", "f_code", "f_globals", "f_lineno", "f_locals"))
 fake_traceback = namedtuple("fake_traceback", ("tb_frame", "tb_lasti", "tb_lineno", "tb_next"))
 
 
 def make_fake(tb):
     if not tb:
```

### Comparing `loguru-0.6.0/tests/exceptions/source/backtrace/suppressed_expression_direct.py` & `loguru-0.7.0/tests/exceptions/source/backtrace/suppressed_expression_direct.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/diagnose/parenthesis.py` & `loguru-0.7.0/tests/exceptions/source/diagnose/parenthesis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+# fmt: off
+# flake8: noqa
 import sys
 
 from loguru import logger
 
-# fmt: off
-
 logger.remove()
 logger.add(sys.stderr, format="", colorize=True, backtrace=False, diagnose=True)
 
 
 class XYZ:
     pass
```

### Comparing `loguru-0.6.0/tests/exceptions/source/diagnose/source_multilines.py` & `loguru-0.7.0/tests/exceptions/source/diagnose/source_multilines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+# fmt: off
+# flake8: noqa
 import sys
 
 from loguru import logger
 
-# fmt: off
-
 logger.remove()
 logger.add(sys.stderr, format="", colorize=True, backtrace=False, diagnose=True)
 
 
 def bug_1(n):
     return ("""multi-lines
 """ + n / 0)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/others/nested_with_reraise.py` & `loguru-0.7.0/tests/exceptions/source/others/nested_with_reraise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 import sys
 
 from loguru import logger
 
 logger.remove()
 logger.add(sys.stderr, format="", diagnose=False, backtrace=False, colorize=False)
 logger.add(sys.stderr, format="", diagnose=True, backtrace=False, colorize=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit.py` & `loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_negative.py` & `loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_negative.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_none.py` & `loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_none.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/others/sys_tracebacklimit_unset.py` & `loguru-0.7.0/tests/exceptions/source/others/sys_tracebacklimit_unset.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/assertion_from_lib.py` & `loguru-0.7.0/tests/exceptions/source/ownership/string_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import sys
 
-import _init
-from somelib import assertionerror
-
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
+    def foo():
+        1 / 0
+
     try:
-        a, b = 1, 2
-        assertionerror(a, b)
-    except AssertionError:
+        exec("foo()")
+    except ZeroDivisionError:
         logger.exception("")
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/assertion_from_local.py` & `loguru-0.7.0/tests/exceptions/source/ownership/assertion_from_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 import sys
 
 import _init
 from somelib import assertionerror
 
 from loguru import logger
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/callback.py` & `loguru-0.7.0/tests/exceptions/source/ownership/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 import sys
 
 import _init
 from somelib import callme, divide
 
 from loguru import logger
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/catch_decorator.py` & `loguru-0.7.0/tests/exceptions/source/ownership/decorated_callback.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import divide
+from somelib import callme, divide
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
     @logger.catch
-    def foo():
-        divide(1, 0)
+    def callback():
+        a, b = 1, 0
+        a / b
 
-    foo()
+    callme(callback)
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
 test(backtrace=False, colorize=False, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/catch_decorator_from_lib.py` & `loguru-0.7.0/tests/exceptions/source/ownership/catch_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import callme, divide
+from somelib import divide
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
     @logger.catch
-    def callback():
+    def foo():
         divide(1, 0)
 
-    callme(callback)
+    foo()
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
 test(backtrace=False, colorize=False, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/decorated_callback.py` & `loguru-0.7.0/tests/exceptions/source/ownership/string_lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import callme, divide
+from somelib import execute
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
-    @logger.catch
-    def callback():
-        a, b = 1, 0
-        a / b
-
-    callme(callback)
+    try:
+        execute()
+    except ZeroDivisionError:
+        logger.exception("")
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
 test(backtrace=False, colorize=False, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/direct.py` & `loguru-0.7.0/tests/exceptions/source/ownership/syntaxerror.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import divide
+from somelib import syntaxerror
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
     try:
-        divide(10, 0)
-    except ZeroDivisionError:
+        syntaxerror()
+    except SyntaxError:
         logger.exception("")
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/indirect.py` & `loguru-0.7.0/tests/exceptions/source/ownership/indirect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 import sys
 
 import _init
 from somelib import divide_indirect
 
 from loguru import logger
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/string_lib.py` & `loguru-0.7.0/tests/exceptions/source/ownership/assertion_from_lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import execute
+from somelib import assertionerror
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
     try:
-        execute()
-    except ZeroDivisionError:
+        a, b = 1, 2
+        assertionerror(a, b)
+    except AssertionError:
         logger.exception("")
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/string_source.py` & `loguru-0.7.0/tests/exceptions/source/ownership/catch_decorator_from_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+# flake8: noqa
 import sys
 
+import _init
+from somelib import callme, divide
+
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
-    def foo():
-        1 / 0
+    @logger.catch
+    def callback():
+        divide(1, 0)
 
-    try:
-        exec("foo()")
-    except ZeroDivisionError:
-        logger.exception("")
+    callme(callback)
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
 test(backtrace=False, colorize=False, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/exceptions/source/ownership/syntaxerror.py` & `loguru-0.7.0/tests/exceptions/source/ownership/direct.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+# flake8: noqa
 import sys
 
 import _init
-from somelib import syntaxerror
+from somelib import divide
 
 from loguru import logger
 
 
 def test(*, backtrace, colorize, diagnose):
     logger.remove()
     logger.add(sys.stderr, format="", colorize=colorize, backtrace=backtrace, diagnose=diagnose)
 
     try:
-        syntaxerror()
-    except SyntaxError:
+        divide(10, 0)
+    except ZeroDivisionError:
         logger.exception("")
 
 
 test(backtrace=True, colorize=True, diagnose=True)
 test(backtrace=False, colorize=True, diagnose=True)
 test(backtrace=True, colorize=True, diagnose=False)
 test(backtrace=False, colorize=True, diagnose=False)
```

### Comparing `loguru-0.6.0/tests/test_activation.py` & `loguru-0.7.0/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_backtrace.py` & `loguru-0.7.0/tests/test_add_option_backtrace.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_catch.py` & `loguru-0.7.0/tests/test_add_option_catch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 from loguru import logger
 
 from .conftest import default_threading_excepthook
 
 
 def broken_sink(m):
-    raise Exception("Error!")
+    raise ValueError("Error!")
 
 
 def test_catch_is_true(capsys):
     logger.add(broken_sink, catch=True)
     logger.debug("Fail")
     out, err = capsys.readouterr()
     assert out == ""
     assert err != ""
 
 
 def test_catch_is_false(capsys):
     logger.add(broken_sink, catch=False)
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError, match="Error!"):
         logger.debug("Fail")
     out, err = capsys.readouterr()
     assert out == err == ""
 
 
 def test_no_sys_stderr(capsys, monkeypatch):
     monkeypatch.setattr(sys, "stderr", None)
@@ -97,15 +97,15 @@
 
     out, err = capsys.readouterr()
     lines = err.strip().splitlines()
 
     assert out == ""
     assert lines[0] == "--- Logging error in Loguru Handler #0 ---"
     assert re.match(r"Record was: \{.*Oops.*\}", lines[1])
-    assert lines[-2].startswith("Exception: Error!")
+    assert lines[-2].startswith("ValueError: Error!")
     assert lines[-1] == "--- End of logging error ---"
 
 
 @pytest.mark.parametrize("enqueue", [False, True])
 def test_broken_sink_caught_keep_working(enqueue):
     output = ""
 
@@ -136,8 +136,8 @@
     logger.add(broken_sink, format="{message}", enqueue=True, catch=False)
 
     with default_threading_excepthook():
         logger.info("A")
         logger.info("B")
         time.sleep(0.1)
 
-    assert called == 1
+    assert called == 2
```

### Comparing `loguru-0.6.0/tests/test_add_option_colorize.py` & `loguru-0.7.0/tests/test_add_option_colorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,33 +57,34 @@
     logger.add(writer, format=format, colorize=False)
     logger.debug(message)
     assert writer.read() == expected
 
 
 @pytest.fixture
 def patch_colorama(monkeypatch):
-    AnsiToWin32_instance = MagicMock()
-    AnsiToWin32_class = MagicMock(return_value=AnsiToWin32_instance)
+    instance = MagicMock()
+    class_ = MagicMock(return_value=instance)
     winapi_test = MagicMock(return_value=True)
     win32 = MagicMock(winapi_test=winapi_test)
-    colorama = MagicMock(AnsiToWin32=AnsiToWin32_class, win32=win32)
+    colorama = MagicMock(AnsiToWin32=class_, win32=win32)
     monkeypatch.setitem(sys.modules, "colorama", colorama)
     monkeypatch.setitem(sys.modules, "colorama.win32", win32)
     yield colorama
 
 
 @pytest.mark.parametrize("colorize", [True, False, None])
 @pytest.mark.parametrize("tty", [True, False])
 @pytest.mark.parametrize("replace_original", [True, False])
-def test_colorize_stream(patch_colorama, monkeypatch, colorize, tty, replace_original):
+@pytest.mark.skipif(os.name == "nt", reason="Colorama is required on Windows")
+def test_colorize_stream_linux(patch_colorama, monkeypatch, colorize, tty, replace_original):
     stream = Stream(tty)
 
     monkeypatch.delenv("TERM", raising=False)
     monkeypatch.delenv("PYCHARM_HOSTED", raising=False)
-    monkeypatch.setattr(os, "name", "unix")
+
     if replace_original:
         monkeypatch.setattr(sys, "__stdout__", stream)
 
     logger.add(stream, format="<red>{message}</red>", colorize=colorize, catch=False)
     logger.debug("Message")
 
     winapi_test = patch_colorama.win32.winapi_test
@@ -97,20 +98,21 @@
     else:
         assert stream.out == "Message\n"
 
 
 @pytest.mark.parametrize("colorize", [True, False, None])
 @pytest.mark.parametrize("tty", [True, False])
 @pytest.mark.parametrize("replace_original", [True, False])
+@pytest.mark.skipif(os.name != "nt", reason="Only Windows requires Colorama")
 def test_colorize_stream_windows(patch_colorama, monkeypatch, colorize, tty, replace_original):
     stream = Stream(tty)
 
     monkeypatch.delenv("TERM", raising=False)
     monkeypatch.delenv("PYCHARM_HOSTED", raising=False)
-    monkeypatch.setattr(os, "name", "nt")
+
     if replace_original:
         monkeypatch.setattr(sys, "__stdout__", stream)
 
     logger.add(stream, format="<blue>{message}</blue>", colorize=colorize, catch=False)
     logger.debug("Message")
 
     winapi_test = patch_colorama.win32.winapi_test
@@ -121,16 +123,15 @@
         assert stream_write.called
     else:
         assert not winapi_test.called
         assert not stream_write.called
 
 
 @pytest.mark.parametrize("colorize", [True, False, None])
-def test_isatty_error(monkeypatch, colorize):
-    monkeypatch.setattr(os, "name", "posix")
+def test_isatty_error(colorize):
     stream = Stream(None)
     logger.add(stream, format="<blue>{message}</blue>", colorize=colorize)
     logger.debug("Message")
 
     if colorize is True:
         assert stream.out == parse("<blue>Message</blue>\n")
     else:
@@ -147,37 +148,94 @@
 
 @pytest.mark.parametrize("stream", [None, Stream(False), Stream(None)])
 def test_pycharm_ignored(monkeypatch, stream):
     monkeypatch.setitem(os.environ, "PYCHARM_HOSTED", "1")
     assert not loguru._colorama.should_colorize(stream)
 
 
+def test_jupyter_fixed(monkeypatch):
+    class Shell:
+        pass
+
+    class Out:
+        pass
+
+    stream = MagicMock()
+    stream.__class__ = Out
+    stream.isatty.return_value = False
+    ipython = MagicMock()
+    ipykernel = MagicMock()
+    instance = MagicMock()
+    instance.__class__ = Shell
+    ipython.get_ipython.return_value = instance
+    ipykernel.zmqshell.ZMQInteractiveShell = Shell
+    ipykernel.iostream.OutStream = Out
+
+    monkeypatch.setitem(sys.modules, "IPython", ipython)
+    monkeypatch.setitem(sys.modules, "ipykernel", ipykernel)
+    monkeypatch.setattr(sys, "stdout", stream)
+
+    assert not stream.isatty()
+    assert loguru._colorama.should_colorize(stream)
+
+
+@pytest.mark.parametrize("stream", [None, Stream(False), Stream(None)])
+def test_jupyter_ignored(monkeypatch, stream):
+    class Shell:
+        pass
+
+    class Out:
+        pass
+
+    ipython = MagicMock()
+    ipykernel = MagicMock()
+    instance = MagicMock()
+    instance.__class__ = Shell
+    ipython.get_ipython.return_value = instance
+    ipykernel.zmqshell.ZMQInteractiveShell = Shell
+    ipykernel.iostream.OutStream = Out
+
+    monkeypatch.setitem(sys.modules, "IPython", ipython)
+    monkeypatch.setitem(sys.modules, "ipykernel", ipykernel)
+    monkeypatch.setattr(sys, "stdout", stream)
+
+    assert not loguru._colorama.should_colorize(stream)
+
+
 @pytest.mark.parametrize("stream", [sys.__stdout__, sys.__stderr__])
-def test_mintty_fixed_windows(monkeypatch, stream):
-    monkeypatch.setattr(os, "name", "nt")
-    monkeypatch.setitem(os.environ, "TERM", "xterm")
+def test_github_actions_fixed(monkeypatch, stream):
+    monkeypatch.setitem(os.environ, "CI", "1")
+    monkeypatch.setitem(os.environ, "GITHUB_ACTIONS", "1")
     monkeypatch.setattr(stream, "isatty", lambda: False)
     assert not stream.isatty()
     assert loguru._colorama.should_colorize(stream)
 
 
 @pytest.mark.parametrize("stream", [None, Stream(False), Stream(None)])
-def test_mintty_ignored_windows(monkeypatch, stream):
-    monkeypatch.setattr(os, "name", "nt")
-    monkeypatch.setitem(os.environ, "TERM", "xterm")
+def test_github_actions_ignored(monkeypatch, stream):
+    monkeypatch.setitem(os.environ, "CI", "1")
+    monkeypatch.setitem(os.environ, "GITHUB_ACTIONS", "1")
     assert not loguru._colorama.should_colorize(stream)
 
 
 @pytest.mark.parametrize("stream", [sys.__stdout__, sys.__stderr__])
+@pytest.mark.skipif(os.name != "nt", reason="The fix is applied only on Windows")
+def test_mintty_fixed_windows(monkeypatch, stream):
+    monkeypatch.setitem(os.environ, "TERM", "xterm")
+    monkeypatch.setattr(stream, "isatty", lambda: False)
+    assert not stream.isatty()
+    assert loguru._colorama.should_colorize(stream)
+
+
+@pytest.mark.parametrize("stream", [sys.__stdout__, sys.__stderr__])
+@pytest.mark.skipif(os.name == "nt", reason="The fix will be applied on Windows")
 def test_mintty_not_fixed_linux(monkeypatch, stream):
-    monkeypatch.setattr(os, "name", "posix")
     monkeypatch.setitem(os.environ, "TERM", "xterm")
     monkeypatch.setattr(stream, "isatty", lambda: False)
     assert not stream.isatty()
     assert not loguru._colorama.should_colorize(stream)
 
 
 @pytest.mark.parametrize("stream", [None, Stream(False), Stream(None)])
-def test_mintty_ignored_linux(monkeypatch, stream):
-    monkeypatch.setattr(os, "name", "posix")
+def test_mintty_ignored(monkeypatch, stream):
     monkeypatch.setitem(os.environ, "TERM", "xterm")
     assert not loguru._colorama.should_colorize(stream)
```

### Comparing `loguru-0.6.0/tests/test_add_option_diagnose.py` & `loguru-0.7.0/tests/test_add_option_diagnose.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_enqueue.py` & `loguru-0.7.0/tests/test_add_option_enqueue.py`

 * *Files 16% similar despite different names*

```diff
@@ -142,39 +142,80 @@
 
 def test_not_caught_exception_queue_get(writer, capsys):
     logger.add(writer, enqueue=True, catch=False, format="{message}")
 
     with default_threading_excepthook():
         logger.info("It's fine")
         logger.bind(broken=NotUnpicklable()).info("Bye bye...")
-        logger.info("It's not fine")
+        logger.info("It's fine again")
         logger.remove()
 
     out, err = capsys.readouterr()
     lines = err.strip().splitlines()
-    assert writer.read() == "It's fine\n"
+    assert writer.read() == "It's fine\nIt's fine again\n"
     assert out == ""
-    assert lines[0].startswith("Exception")
-    assert lines[-1].endswith("UnpicklingError: You shall not de-serialize me!")
+    assert lines[0] == "--- Logging error in Loguru Handler #0 ---"
+    assert lines[1] == "Record was: None"
+    assert lines[-2].endswith("UnpicklingError: You shall not de-serialize me!")
+    assert lines[-1] == "--- End of logging error ---"
 
 
 def test_not_caught_exception_sink_write(capsys):
     logger.add(NotWritable(), enqueue=True, catch=False, format="{message}")
 
     with default_threading_excepthook():
         logger.info("It's fine")
         logger.bind(fail=True).info("Bye bye...")
-        logger.info("It's not fine")
+        logger.info("It's fine again")
         logger.remove()
 
     out, err = capsys.readouterr()
     lines = err.strip().splitlines()
-    assert out == "It's fine\n"
-    assert lines[0].startswith("Exception")
-    assert lines[-1] == "RuntimeError: You asked me to fail..."
+    assert out == "It's fine\nIt's fine again\n"
+    assert lines[0] == "--- Logging error in Loguru Handler #0 ---"
+    assert re.match(r"Record was: \{.*Bye bye.*\}", lines[1])
+    assert lines[-2] == "RuntimeError: You asked me to fail..."
+    assert lines[-1] == "--- End of logging error ---"
+
+
+def test_not_caught_exception_sink_write_then_complete(capsys):
+    logger.add(NotWritable(), enqueue=True, catch=False, format="{message}")
+
+    with default_threading_excepthook():
+        logger.bind(fail=True).info("Bye bye...")
+        logger.complete()
+        logger.complete()  # Called twice to ensure it's re-usable.
+        logger.remove()
+
+    out, err = capsys.readouterr()
+    lines = err.strip().splitlines()
+    assert out == ""
+    assert lines[0] == "--- Logging error in Loguru Handler #0 ---"
+    assert re.match(r"Record was: \{.*Bye bye.*\}", lines[1])
+    assert lines[-2] == "RuntimeError: You asked me to fail..."
+    assert lines[-1] == "--- End of logging error ---"
+
+
+def test_not_caught_exception_queue_get_then_complete(writer, capsys):
+    logger.add(writer, enqueue=True, catch=False, format="{message}")
+
+    with default_threading_excepthook():
+        logger.bind(broken=NotUnpicklable()).info("Bye bye...")
+        logger.complete()
+        logger.complete()
+        logger.remove()
+
+    out, err = capsys.readouterr()
+    lines = err.strip().splitlines()
+    assert writer.read() == ""
+    assert out == ""
+    assert lines[0] == "--- Logging error in Loguru Handler #0 ---"
+    assert lines[1] == "Record was: None"
+    assert lines[-2].endswith("UnpicklingError: You shall not de-serialize me!")
+    assert lines[-1] == "--- End of logging error ---"
 
 
 def test_wait_for_all_messages_enqueued(capsys):
     def slow_sink(message):
         time.sleep(0.01)
         sys.stderr.write(message)
```

### Comparing `loguru-0.6.0/tests/test_add_option_filter.py` & `loguru-0.7.0/tests/test_add_option_filter.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_format.py` & `loguru-0.7.0/tests/test_add_option_format.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_kwargs.py` & `loguru-0.7.0/tests/test_add_option_kwargs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import io
 
 import pytest
 
 from loguru import logger
 
 
-def test_file_mode_a(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("base\n")
-    logger.add(str(file), format="{message}", mode="a")
+def test_file_mode_a(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("base\n")
+    logger.add(file, format="{message}", mode="a")
     logger.debug("msg")
-    assert file.read() == "base\nmsg\n"
+    assert file.read_text() == "base\nmsg\n"
 
 
-def test_file_mode_w(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("base\n")
-    logger.add(str(file), format="{message}", mode="w")
+def test_file_mode_w(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("base\n")
+    logger.add(file, format="{message}", mode="w")
     logger.debug("msg")
-    assert file.read() == "msg\n"
+    assert file.read_text() == "msg\n"
 
 
-def test_file_buffering(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="{message}", buffering=-1)
+def test_file_buffering(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{message}", buffering=-1)
     logger.debug("x" * (io.DEFAULT_BUFFER_SIZE // 2))
-    assert file.read() == ""
+    assert file.read_text() == ""
     logger.debug("x" * (io.DEFAULT_BUFFER_SIZE * 2))
-    assert file.read() != ""
+    assert file.read_text() != ""
 
 
 def test_invalid_function_kwargs():
     def function(message):
         pass
 
     with pytest.raises(TypeError, match=r"add\(\) got an unexpected keyword argument"):
```

### Comparing `loguru-0.6.0/tests/test_add_option_level.py` & `loguru-0.7.0/tests/test_add_option_level.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_option_serialize.py` & `loguru-0.7.0/tests/test_add_option_serialize.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_add_sinks.py` & `loguru-0.7.0/tests/test_add_sinks.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,26 +55,26 @@
 
 
 @repetitions
 @pytest.mark.parametrize(
     "sink_from_path",
     [str, pathlib.Path, lambda path: open(path, "a"), lambda path: pathlib.Path(path).open("a")],
 )
-def test_file_sink(rep, sink_from_path, tmpdir):
-    file = tmpdir.join("test.log")
+def test_file_sink(rep, sink_from_path, tmp_path):
+    file = tmp_path / "test.log"
     sink = sink_from_path(str(file))
     log(sink, rep)
-    assert file.read() == expected * rep
+    assert file.read_text() == expected * rep
 
 
 @repetitions
-def test_file_sink_folder_creation(rep, tmpdir):
-    file = tmpdir.join("some", "sub", "folder", "not", "existing", "test.log")
-    log(str(file), rep)
-    assert file.read() == expected * rep
+def test_file_sink_folder_creation(rep, tmp_path):
+    file = tmp_path.joinpath("some", "sub", "folder", "not", "existing", "test.log")
+    log(file, rep)
+    assert file.read_text() == expected * rep
 
 
 @repetitions
 def test_function_sink(rep):
     a = []
 
     def func(log_message):
@@ -137,35 +137,33 @@
         def flush(self):
             flushed.append(out[-1])
 
     log(A(), rep)
     assert flushed == [expected] * rep
 
 
-def test_file_sink_ascii_encoding(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(
-        str(file), encoding="ascii", format="{message}", errors="backslashreplace", catch=False
-    )
+def test_file_sink_ascii_encoding(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, encoding="ascii", format="{message}", errors="backslashreplace", catch=False)
     logger.info("天")
     logger.remove()
     assert file.read_text("ascii") == "\\u5929\n"
 
 
-def test_file_sink_utf8_encoding(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), encoding="utf8", format="{message}", errors="strict", catch=False)
+def test_file_sink_utf8_encoding(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, encoding="utf8", format="{message}", errors="strict", catch=False)
     logger.info("天")
     logger.remove()
     assert file.read_text("utf8") == "天\n"
 
 
-def test_file_sink_default_encoding(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="{message}", errors="strict", catch=False)
+def test_file_sink_default_encoding(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{message}", errors="strict", catch=False)
     logger.info("天")
     logger.remove()
     assert file.read_text("utf8") == "天\n"
 
 
 def test_disabled_logger_in_sink(sink_with_logger):
     sink = sink_with_logger(logger)
```

### Comparing `loguru-0.6.0/tests/test_ansimarkup_extended.py` & `loguru-0.7.0/tests/test_ansimarkup_extended.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,88 @@
 import pytest
-from colorama import Back as B
-from colorama import Fore as F
-from colorama import Style as S
+from colorama import Back, Fore, Style
 
 from .conftest import parse
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<bg red>1</bg red>", B.RED + "1" + S.RESET_ALL),
-        ("<bg BLACK>1</bg BLACK>", B.BLACK + "1" + S.RESET_ALL),
-        ("<bg light-green>1</bg light-green>", B.LIGHTGREEN_EX + "1" + S.RESET_ALL),
-        ("<bg LIGHT-MAGENTA>1</bg LIGHT-MAGENTA>", B.LIGHTMAGENTA_EX + "1" + S.RESET_ALL),
+        ("<bg red>1</bg red>", Back.RED + "1" + Style.RESET_ALL),
+        ("<bg BLACK>1</bg BLACK>", Back.BLACK + "1" + Style.RESET_ALL),
+        ("<bg light-green>1</bg light-green>", Back.LIGHTGREEN_EX + "1" + Style.RESET_ALL),
+        ("<bg LIGHT-MAGENTA>1</bg LIGHT-MAGENTA>", Back.LIGHTMAGENTA_EX + "1" + Style.RESET_ALL),
     ],
 )
 def test_background_colors(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<fg yellow>1</fg yellow>", F.YELLOW + "1" + S.RESET_ALL),
-        ("<fg BLUE>1</fg BLUE>", F.BLUE + "1" + S.RESET_ALL),
-        ("<fg light-white>1</fg light-white>", F.LIGHTWHITE_EX + "1" + S.RESET_ALL),
-        ("<fg LIGHT-CYAN>1</fg LIGHT-CYAN>", F.LIGHTCYAN_EX + "1" + S.RESET_ALL),
+        ("<fg yellow>1</fg yellow>", Fore.YELLOW + "1" + Style.RESET_ALL),
+        ("<fg BLUE>1</fg BLUE>", Fore.BLUE + "1" + Style.RESET_ALL),
+        ("<fg light-white>1</fg light-white>", Fore.LIGHTWHITE_EX + "1" + Style.RESET_ALL),
+        ("<fg LIGHT-CYAN>1</fg LIGHT-CYAN>", Fore.LIGHTCYAN_EX + "1" + Style.RESET_ALL),
     ],
 )
 def test_foreground_colors(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<fg #ff0000>1</fg #ff0000>", "\x1b[38;2;255;0;0m" "1" + S.RESET_ALL),
-        ("<bg #00A000>1</bg #00A000>", "\x1b[48;2;0;160;0m" "1" + S.RESET_ALL),
-        ("<fg #F12>1</fg #F12>", "\x1b[38;2;241;47;18m" "1" + S.RESET_ALL),
+        ("<fg #ff0000>1</fg #ff0000>", "\x1b[38;2;255;0;0m" "1" + Style.RESET_ALL),
+        ("<bg #00A000>1</bg #00A000>", "\x1b[48;2;0;160;0m" "1" + Style.RESET_ALL),
+        ("<fg #F12>1</fg #F12>", "\x1b[38;2;241;47;18m" "1" + Style.RESET_ALL),
     ],
 )
 def test_8bit_colors(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<fg #ff0000>1</fg #ff0000>", "\x1b[38;2;255;0;0m" "1" + S.RESET_ALL),
-        ("<bg #00A000>1</bg #00A000>", "\x1b[48;2;0;160;0m" "1" + S.RESET_ALL),
-        ("<fg #F12>1</fg #F12>", "\x1b[38;2;241;47;18m" "1" + S.RESET_ALL),
-        ("<bg #BEE>1</bg #BEE>", "\x1b[48;2;190;235;238m" "1" + S.RESET_ALL),
+        ("<fg #ff0000>1</fg #ff0000>", "\x1b[38;2;255;0;0m" "1" + Style.RESET_ALL),
+        ("<bg #00A000>1</bg #00A000>", "\x1b[48;2;0;160;0m" "1" + Style.RESET_ALL),
+        ("<fg #F12>1</fg #F12>", "\x1b[38;2;241;47;18m" "1" + Style.RESET_ALL),
+        ("<bg #BEE>1</bg #BEE>", "\x1b[48;2;190;235;238m" "1" + Style.RESET_ALL),
     ],
 )
 def test_hex_colors(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<fg 200>1</fg 200>", "\x1b[38;5;200m" "1" + S.RESET_ALL),
-        ("<bg 49>1</bg 49>", "\x1b[48;5;49m" "1" + S.RESET_ALL),
+        ("<fg 200>1</fg 200>", "\x1b[38;5;200m" "1" + Style.RESET_ALL),
+        ("<bg 49>1</bg 49>", "\x1b[48;5;49m" "1" + Style.RESET_ALL),
     ],
 )
 def test_rgb_colors(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
         (
             "<red><b><bg #00A000>1</bg #00A000></b></red>",
-            F.RED + S.BRIGHT + "\x1b[48;2;0;160;0m"
-            "1" + S.RESET_ALL + F.RED + S.BRIGHT + S.RESET_ALL + F.RED + S.RESET_ALL,
+            Fore.RED + Style.BRIGHT + "\x1b[48;2;0;160;0m"
+            "1"
+            + Style.RESET_ALL
+            + Fore.RED
+            + Style.BRIGHT
+            + Style.RESET_ALL
+            + Fore.RED
+            + Style.RESET_ALL,
         ),
         (
             "<bg 100><fg 200>1</fg 200></bg 100>",
             "\x1b[48;5;100m" "\x1b[38;5;200m" "1" "\x1b[0m" "\x1b[48;5;100m" "\x1b[0m",
         ),
         (
             "<bg #00a000><fg #FF0000>1</fg #FF0000></bg #00a000>",
@@ -93,25 +97,25 @@
 def test_nested(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
-        ("<r>2 > 1</r>", F.RED + "2 > 1" + S.RESET_ALL),
-        ("<r>1 < 2</r>", F.RED + "1 < 2" + S.RESET_ALL),
-        ("<r>1 </ 2</r>", F.RED + "1 </ 2" + S.RESET_ALL),
-        ("{: <10}<r>1</r>", "{: <10}" + F.RED + "1" + S.RESET_ALL),
-        ("{: </10}<r>1</r>", "{: </10}" + F.RED + "1" + S.RESET_ALL),
-        ("<r>1</r>{: >10}", F.RED + "1" + S.RESET_ALL + "{: >10}"),
-        ("<1<r>2</r>3>", "<1" + F.RED + "2" + S.RESET_ALL + "3>"),
-        ("</1<r>2</r>3>", "</1" + F.RED + "2" + S.RESET_ALL + "3>"),
-        ("<1<r>2 < 3</r>4>", "<1" + F.RED + "2 < 3" + S.RESET_ALL + "4>"),
-        ("<1<r>2 </ 3</r>4>", "<1" + F.RED + "2 </ 3" + S.RESET_ALL + "4>"),
-        ("<1<r>3 > 2</r>4>", "<1" + F.RED + "3 > 2" + S.RESET_ALL + "4>"),
+        ("<r>2 > 1</r>", Fore.RED + "2 > 1" + Style.RESET_ALL),
+        ("<r>1 < 2</r>", Fore.RED + "1 < 2" + Style.RESET_ALL),
+        ("<r>1 </ 2</r>", Fore.RED + "1 </ 2" + Style.RESET_ALL),
+        ("{: <10}<r>1</r>", "{: <10}" + Fore.RED + "1" + Style.RESET_ALL),
+        ("{: </10}<r>1</r>", "{: </10}" + Fore.RED + "1" + Style.RESET_ALL),
+        ("<r>1</r>{: >10}", Fore.RED + "1" + Style.RESET_ALL + "{: >10}"),
+        ("<1<r>2</r>3>", "<1" + Fore.RED + "2" + Style.RESET_ALL + "3>"),
+        ("</1<r>2</r>3>", "</1" + Fore.RED + "2" + Style.RESET_ALL + "3>"),
+        ("<1<r>2 < 3</r>4>", "<1" + Fore.RED + "2 < 3" + Style.RESET_ALL + "4>"),
+        ("<1<r>2 </ 3</r>4>", "<1" + Fore.RED + "2 </ 3" + Style.RESET_ALL + "4>"),
+        ("<1<r>3 > 2</r>4>", "<1" + Fore.RED + "3 > 2" + Style.RESET_ALL + "4>"),
     ],
 )
 def test_tricky_parse(text, expected):
     assert parse(text, strip=False) == expected
 
 
 @pytest.mark.parametrize(
```

### Comparing `loguru-0.6.0/tests/test_bind.py` & `loguru-0.7.0/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_configure.py` & `loguru-0.7.0/tests/test_configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import sys
 
 import pytest
 
 from loguru import logger
 
 
-def test_handlers(capsys, tmpdir):
-    file = tmpdir.join("test.log")
+def test_handlers(capsys, tmp_path):
+    file = tmp_path / "test.log"
 
     handlers = [
-        {"sink": str(file), "format": "FileSink: {message}"},
+        {"sink": file, "format": "FileSink: {message}"},
         {"sink": sys.stdout, "format": "StdoutSink: {message}"},
     ]
 
     logger.configure(handlers=handlers)
     logger.debug("test")
 
     out, err = capsys.readouterr()
 
-    assert file.read() == "FileSink: test\n"
+    assert file.read_text() == "FileSink: test\n"
     assert out == "StdoutSink: test\n"
     assert err == ""
 
 
 def test_levels(writer):
     levels = [{"name": "my_level", "icon": "X", "no": 12}, {"name": "DEBUG", "icon": "!"}]
```

### Comparing `loguru-0.6.0/tests/test_contextualize.py` & `loguru-0.7.0/tests/test_contextualize.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_coroutine_sink.py` & `loguru-0.7.0/tests/test_coroutine_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 import logging
 import multiprocessing
-import platform
 import re
 import sys
 import threading
 
 import pytest
 
 import loguru
@@ -259,30 +258,30 @@
     logger.info("D")
 
     out, err = capsys.readouterr()
     assert out == ""
     assert err == "A\nB\nC\nD\n"
 
 
-def test_complete_file_noop(tmpdir):
-    filepath = tmpdir.join("test.log")
+def test_complete_file_noop(tmp_path):
+    filepath = tmp_path / "test.log"
 
-    logger.add(str(filepath), format="{message}", catch=False)
+    logger.add(filepath, format="{message}", catch=False)
     logger.info("A")
 
     async def worker():
         logger.info("B")
         await logger.complete()
         logger.info("C")
 
     asyncio.run(worker())
 
     logger.info("D")
 
-    assert filepath.read() == "A\nB\nC\nD\n"
+    assert filepath.read_text() == "A\nB\nC\nD\n"
 
 
 def test_complete_function_noop():
     out = ""
 
     def write(msg):
         nonlocal out
@@ -503,15 +502,15 @@
     out, err = capsys.readouterr()
     assert out == "A\n"
     assert err == ""
 
 
 def test_complete_from_multiple_threads_loop_is_none(capsys):
     async def worker(i):
-        for j in range(100):
+        for _ in range(100):
             await asyncio.sleep(0)
             logger.info("{:03}", i)
         await logger.complete()
 
     async def sink(msg):
         print(msg, end="")
 
@@ -531,15 +530,15 @@
     out, err = capsys.readouterr()
     assert sorted(out.splitlines()) == ["{:03}".format(i) for i in range(10) for _ in range(100)]
     assert err == ""
 
 
 def test_complete_from_multiple_threads_loop_is_not_none(capsys):
     async def worker(i):
-        for j in range(100):
+        for _ in range(100):
             await asyncio.sleep(0)
             logger.info("{:03}", i)
         await logger.complete()
 
     async def sink(msg):
         print(msg, end="")
 
@@ -586,15 +585,14 @@
     def __init__(self):
         self.output = ""
 
     async def write(self, message):
         self.output += message
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_complete_with_sub_processes(monkeypatch, capsys):
     ctx = multiprocessing.get_context("spawn")
     monkeypatch.setattr(loguru._handler, "multiprocessing", ctx)
 
     loop = asyncio.new_event_loop()
     writer = Writer()
     logger.add(writer.write, format="{message}", enqueue=True, loop=loop)
```

### Comparing `loguru-0.6.0/tests/test_deepcopy.py` & `loguru-0.7.0/tests/test_deepcopy.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_defaults.py` & `loguru-0.7.0/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_exceptions_catch.py` & `loguru-0.7.0/tests/test_exceptions_catch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import site
 import sys
 import sysconfig
 import types
 
 import pytest
 
-import loguru
 from loguru import logger
 
 
 @pytest.mark.parametrize("diagnose", [False, True])
 def test_caret_not_masked(writer, diagnose):
     logger.add(writer, backtrace=True, diagnose=diagnose, colorize=False, format="")
 
@@ -61,33 +60,33 @@
         bar(4)
     except ZeroDivisionError:
         logger.exception("")
 
     assert writer.output.endswith("ZeroDivisionError: division by zero\n")
 
 
-def test_file_sink_ascii_encoding(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="", encoding="ascii", errors="backslashreplace", catch=False)
+def test_file_sink_ascii_encoding(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, format="", encoding="ascii", errors="backslashreplace", catch=False)
     a = "天"
 
     try:
         "天" * a
     except Exception:
         logger.exception("")
 
     logger.remove()
     result = file.read_text("ascii")
     assert result.count('"\\u5929" * a') == 1
     assert result.count("-> '\\u5929'") == 1
 
 
-def test_file_sink_utf8_encoding(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="", encoding="utf8", errors="strict", catch=False)
+def test_file_sink_utf8_encoding(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, format="", encoding="utf8", errors="strict", catch=False)
     a = "天"
 
     try:
         "天" * a
     except Exception:
         logger.exception("")
 
@@ -425,7 +424,23 @@
 
 def test_default_with_coroutine():
     @logger.catch(default=42)
     async def foo():
         return 1 / 0
 
     assert asyncio.run(foo()) == 42
+
+
+def test_error_when_decorating_class_without_parentheses():
+    with pytest.raises(TypeError):
+
+        @logger.catch
+        class Foo:
+            pass
+
+
+def test_error_when_decorating_class_with_parentheses():
+    with pytest.raises(TypeError):
+
+        @logger.catch()
+        class Foo:
+            pass
```

### Comparing `loguru-0.6.0/tests/test_exceptions_formatting.py` & `loguru-0.7.0/tests/test_exceptions_formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def generate(output, outpath):
     """Generate new output file if exception formatting is updated"""
     os.makedirs(os.path.dirname(outpath), exist_ok=True)
     with open(outpath, "w") as file:
         file.write(output)
-    assert False  # Avoid forgetting to remove "generate()" inadvertently
+    raise AssertionError("The method 'generate()' was called while running tests.")
 
 
 def compare_exception(dirname, filename):
     cwd = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     python = sys.executable or "python"
     filepath = os.path.join("tests", "exceptions", "source", dirname, filename + ".py")
     outpath = os.path.join(cwd, "tests", "exceptions", "output", dirname, filename + ".txt")
```

### Comparing `loguru-0.6.0/tests/test_filesink_compression.py` & `loguru-0.7.0/tests/test_filesink_compression.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,271 @@
-import datetime
 import os
 import sys
 import threading
 import time
+from unittest.mock import Mock
 
 import pytest
 
-import loguru
 from loguru import logger
 
+from .conftest import check_dir
+
 
 @pytest.mark.parametrize(
     "compression", ["gz", "bz2", "zip", "xz", "lzma", "tar", "tar.gz", "tar.bz2", "tar.xz"]
 )
-def test_compression_ext(tmpdir, compression):
-    i = logger.add(str(tmpdir.join("file.log")), compression=compression)
+def test_compression_ext(tmp_path, compression):
+    i = logger.add(tmp_path / "file.log", compression=compression)
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
-    assert tmpdir.join("file.log.%s" % compression).check(exists=1)
+    check_dir(tmp_path, files=[("file.log.%s" % compression, None)])
 
 
-def test_compression_function(tmpdir):
+def test_compression_function(tmp_path):
     def compress(file):
         os.replace(file, file + ".rar")
 
-    i = logger.add(str(tmpdir.join("file.log")), compression=compress)
+    i = logger.add(tmp_path / "file.log", compression=compress)
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
-    assert tmpdir.join("file.log.rar").check(exists=1)
+    check_dir(tmp_path, files=[("file.log.rar", None)])
 
 
 @pytest.mark.parametrize("mode", ["a", "a+", "w", "x"])
-def test_compression_at_rotation(tmpdir, mode):
-    logger.add(
-        str(tmpdir.join("file.log")), format="{message}", rotation=0, compression="gz", mode=mode
-    )
-    logger.debug("After compression")
-
-    files = sorted(tmpdir.listdir())
-
-    assert len(files) == 2
-    assert files[0].fnmatch(
-        "file.{0}-{1}-{1}_{1}-{1}-{1}_{2}.log.gz".format("[0-9]" * 4, "[0-9]" * 2, "[0-9]" * 6)
+def test_compression_at_rotation(tmp_path, mode, freeze_time):
+    with freeze_time("2010-10-09 11:30:59"):
+        logger.add(
+            tmp_path / "file.log", format="{message}", rotation=0, compression="gz", mode=mode
+        )
+        logger.debug("After compression")
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("file.2010-10-09_11-30-59_000000.log.gz", None),
+            ("file.log", "After compression\n"),
+        ],
     )
-    assert files[1].basename == "file.log"
-    assert files[1].read() == "After compression\n"
 
 
 @pytest.mark.parametrize("mode", ["a", "a+", "w", "x"])
-def test_compression_at_remove_without_rotation(tmpdir, mode):
-    i = logger.add(str(tmpdir.join("file.log")), compression="gz", mode=mode)
+def test_compression_at_remove_without_rotation(tmp_path, mode):
+    i = logger.add(tmp_path / "file.log", compression="gz", mode=mode)
     logger.debug("test")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
-    assert tmpdir.join("file.log.gz").check(exists=1)
+    check_dir(tmp_path, files=[("file.log.gz", None)])
 
 
 @pytest.mark.parametrize("mode", ["a", "a+", "w", "x"])
-def test_no_compression_at_remove_with_rotation(tmpdir, mode):
-    i = logger.add(str(tmpdir.join("test.log")), compression="gz", rotation="100 MB", mode=mode)
+def test_no_compression_at_remove_with_rotation(tmp_path, mode):
+    i = logger.add(tmp_path / "test.log", compression="gz", rotation="100 MB", mode=mode)
     logger.debug("test")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
-    assert tmpdir.join("test.log").check(exists=1)
-
+    check_dir(tmp_path, files=[("test.log", None)])
 
-def test_rename_existing_with_creation_time(monkeypatch, tmpdir):
-    def creation_time(filepath):
-        assert os.path.isfile(filepath)
-        assert os.path.basename(filepath) == "test.log.tar.gz"
-        return datetime.datetime(2018, 1, 1, 0, 0, 0, 0).timestamp()
 
-    i = logger.add(str(tmpdir.join("test.log")), compression="tar.gz")
-    logger.debug("test")
-    logger.remove(i)
-    j = logger.add(str(tmpdir.join("test.log")), compression="tar.gz")
-    logger.debug("test")
-
-    monkeypatch.setattr(loguru._file_sink, "get_ctime", creation_time)
+def test_rename_existing_with_creation_time(tmp_path, freeze_time):
+    with freeze_time("2018-01-01") as frozen:
+        i = logger.add(tmp_path / "test.log", compression="tar.gz")
+        logger.debug("test")
+        logger.remove(i)
+        frozen.tick()
+        j = logger.add(tmp_path / "test.log", compression="tar.gz")
+        logger.debug("test")
+        logger.remove(j)
+
+    check_dir(
+        tmp_path,
+        files=[("test.2018-01-01_00-00-00_000000.log.tar.gz", None), ("test.log.tar.gz", None)],
+    )
 
-    logger.remove(j)
 
-    assert len(tmpdir.listdir()) == 2
-    assert tmpdir.join("test.log.tar.gz").check(exists=1)
-    assert tmpdir.join("test.2018-01-01_00-00-00_000000.log.tar.gz").check(exists=1)
-
-
-def test_renaming_compression_dest_exists(monkeypatch, monkeypatch_date, tmpdir):
-    date = (2019, 1, 2, 3, 4, 5, 6)
-    timestamp = datetime.datetime(*date).timestamp()
-    monkeypatch_date(*date)
-    monkeypatch.setattr(loguru._file_sink, "get_ctime", lambda _: timestamp)
-
-    for i in range(4):
-        logger.add(str(tmpdir.join("rotate.log")), compression=".tar.gz", format="{message}")
-        logger.info(str(i))
-        logger.remove()
-
-    assert len(tmpdir.listdir()) == 4
-    assert tmpdir.join("rotate.log.tar.gz").check(exists=1)
-    assert tmpdir.join("rotate.2019-01-02_03-04-05_000006.log.tar.gz").check(exists=1)
-    assert tmpdir.join("rotate.2019-01-02_03-04-05_000006.2.log.tar.gz").check(exists=1)
-    assert tmpdir.join("rotate.2019-01-02_03-04-05_000006.3.log.tar.gz").check(exists=1)
-
-
-def test_renaming_compression_dest_exists_with_time(monkeypatch, monkeypatch_date, tmpdir):
-    date = (2019, 1, 2, 3, 4, 5, 6)
-    timestamp = datetime.datetime(*date).timestamp()
-    monkeypatch_date(*date)
-    monkeypatch.setattr(loguru._file_sink, "get_ctime", lambda _: timestamp)
-
-    for i in range(4):
-        logger.add(str(tmpdir.join("rotate.{time}.log")), compression=".tar.gz", format="{message}")
-        logger.info(str(i))
-        logger.remove()
-
-    assert len(tmpdir.listdir()) == 4
-    assert tmpdir.join("rotate.2019-01-02_03-04-05_000006.log.tar.gz").check(exists=1)
-    assert tmpdir.join(
-        "rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.log.tar.gz"
-    ).check(exists=1)
-    assert tmpdir.join(
-        "rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.2.log.tar.gz"
-    ).check(exists=1)
-    assert tmpdir.join(
-        "rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.3.log.tar.gz"
-    ).check(exists=1)
+def test_renaming_compression_dest_exists(freeze_time, tmp_path):
+    with freeze_time("2019-01-02 03:04:05.000006"):
+        for i in range(4):
+            logger.add(tmp_path / "rotate.log", compression=".tar.gz", format="{message}")
+            logger.info(str(i))
+            logger.remove()
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("rotate.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.2.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.3.log.tar.gz", None),
+        ],
+    )
 
 
-def test_compression_use_renamed_file_after_rotation(tmpdir):
-    compressed_file = None
+def test_renaming_compression_dest_exists_with_time(freeze_time, tmp_path):
+    with freeze_time("2019-01-02 03:04:05.000006"):
+        for i in range(4):
+            logger.add(tmp_path / "rotate.{time}.log", compression=".tar.gz", format="{message}")
+            logger.info(str(i))
+            logger.remove()
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("rotate.2019-01-02_03-04-05_000006.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.2.log.tar.gz", None),
+            ("rotate.2019-01-02_03-04-05_000006.2019-01-02_03-04-05_000006.3.log.tar.gz", None),
+        ],
+    )
 
-    def compression(filepath):
-        nonlocal compressed_file
-        compressed_file = filepath
 
+def test_compression_use_renamed_file_after_rotation(tmp_path, freeze_time):
     def rotation(message, _):
         return message.record["extra"].get("rotate", False)
 
-    filepath = tmpdir.join("test.log")
-    logger.add(str(filepath), format="{message}", compression=compression, rotation=rotation)
-
-    logger.info("Before")
-    logger.bind(rotate=True).info("Rotation")
-    logger.info("After")
+    compression = Mock()
 
-    assert compressed_file != str(filepath)
-    assert open(compressed_file, "r").read() == "Before\n"
-    assert filepath.read() == "Rotation\nAfter\n"
+    with freeze_time("2020-01-02"):
+        logger.add(
+            tmp_path / "test.log", format="{message}", compression=compression, rotation=rotation
+        )
+
+        logger.info("Before")
+        logger.bind(rotate=True).info("Rotation")
+        logger.info("After")
+
+    compression.assert_called_once_with(str(tmp_path / "test.2020-01-02_00-00-00_000000.log"))
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.2020-01-02_00-00-00_000000.log", "Before\n"),
+            ("test.log", "Rotation\nAfter\n"),
+        ],
+    )
 
 
-def test_threaded_compression_after_rotation(tmpdir):
+def test_threaded_compression_after_rotation(tmp_path):
     thread = None
 
     def rename(filepath):
         time.sleep(1)
-        os.rename(filepath, str(tmpdir.join("test.log.mv")))
+        os.rename(filepath, str(tmp_path / "test.log.mv"))
 
     def compression(filepath):
         nonlocal thread
         thread = threading.Thread(target=rename, args=(filepath,))
         thread.start()
 
     def rotation(message, _):
         return message.record["extra"].get("rotate", False)
 
     logger.add(
-        str(tmpdir.join("test.log")), format="{message}", compression=compression, rotation=rotation
+        tmp_path / "test.log", format="{message}", compression=compression, rotation=rotation
     )
 
     logger.info("Before")
     logger.bind(rotate=True).info("Rotation")
     logger.info("After")
 
     thread.join()
 
-    assert tmpdir.join("test.log").read() == "Rotation\nAfter\n"
-    assert tmpdir.join("test.log.mv").read() == "Before\n"
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.log", "Rotation\nAfter\n"),
+            ("test.log.mv", "Before\n"),
+        ],
+    )
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_compression_at_rotation(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_compression(file):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Compression error")
+def test_exception_during_compression_at_rotation(freeze_time, tmp_path, capsys, delay):
+    with freeze_time("2017-07-01") as frozen:
+        logger.add(
+            tmp_path / "test.log",
+            format="{message}",
+            compression=Mock(side_effect=[Exception("Compression error"), None]),
+            rotation=0,
+            catch=True,
+            delay=delay,
+        )
+        logger.debug("AAA")
+        frozen.tick()
+        logger.debug("BBB")
 
-    logger.add(
-        str(tmpdir.join("test.log")),
-        format="{message}",
-        compression=failing_compression,
-        rotation=0,
-        catch=True,
-        delay=delay,
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.2017-07-01_00-00-00_000000.log", ""),
+            ("test.2017-07-01_00-00-01_000000.log", ""),
+            ("test.log", "BBB\n"),
+        ],
     )
-    logger.debug("AAA")
-    logger.debug("BBB")
 
-    files = sorted(tmpdir.listdir())
     out, err = capsys.readouterr()
-
-    assert len(files) == 3
-    assert [file.read() for file in files] == ["", "", "BBB\n"]
     assert out == ""
     assert err.count("Logging error in Loguru Handler") == 1
     assert err.count("Exception: Compression error") == 1
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_compression_at_rotation_not_caught(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_compression(file):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Compression error")
-
-    logger.add(
-        str(tmpdir.join("test.log")),
-        format="{message}",
-        compression=failing_compression,
-        rotation=0,
-        catch=False,
-        delay=delay,
+def test_exception_during_compression_at_rotation_not_caught(freeze_time, tmp_path, capsys, delay):
+    with freeze_time("2017-07-01") as frozen:
+        logger.add(
+            tmp_path / "test.log",
+            format="{message}",
+            compression=Mock(side_effect=[OSError("Compression error"), None]),
+            rotation=0,
+            catch=False,
+            delay=delay,
+        )
+        with pytest.raises(OSError, match="Compression error"):
+            logger.debug("AAA")
+
+        frozen.tick()
+        logger.debug("BBB")
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.2017-07-01_00-00-00_000000.log", ""),
+            ("test.2017-07-01_00-00-01_000000.log", ""),
+            ("test.log", "BBB\n"),
+        ],
     )
-    with pytest.raises(Exception, match="Compression error"):
-        logger.debug("AAA")
-    logger.debug("BBB")
 
-    files = sorted(tmpdir.listdir())
     out, err = capsys.readouterr()
-
-    assert len(files) == 3
-    assert [file.read() for file in files] == ["", "", "BBB\n"]
     assert out == err == ""
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_compression_at_remove(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_compression(file):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Compression error")
-
+def test_exception_during_compression_at_remove(tmp_path, capsys, delay):
     i = logger.add(
-        str(tmpdir.join("test.log")),
+        tmp_path / "test.log",
         format="{message}",
-        compression=failing_compression,
+        compression=Mock(side_effect=[OSError("Compression error"), None]),
         catch=True,
         delay=delay,
     )
     logger.debug("AAA")
 
-    with pytest.raises(Exception, match=r"Compression error"):
+    with pytest.raises(OSError, match=r"Compression error"):
         logger.remove(i)
 
     logger.debug("Nope")
 
-    files = sorted(tmpdir.listdir())
-    out, err = capsys.readouterr()
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.log", "AAA\n"),
+        ],
+    )
 
-    assert len(files) == 1
-    assert tmpdir.join("test.log").read() == "AAA\n"
+    out, err = capsys.readouterr()
     assert out == err == ""
 
 
 @pytest.mark.parametrize("compression", [0, True, os, object(), {"zip"}])
 def test_invalid_compression(compression):
     with pytest.raises(TypeError):
         logger.add("test.log", compression=compression)
```

### Comparing `loguru-0.6.0/tests/test_filesink_retention.py` & `loguru-0.7.0/tests/test_filesink_retention.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import datetime
 import os
+from unittest.mock import Mock
 
 import pytest
 
 from loguru import logger
 
+from .conftest import check_dir
+
 
 @pytest.mark.parametrize("retention", ["1 hour", "1H", " 1 h ", datetime.timedelta(hours=1)])
-def test_retention_time(monkeypatch_date, tmpdir, retention):
-    i = logger.add(str(tmpdir.join("test.log.x")), retention=retention)
+def test_retention_time(freeze_time, tmp_path, retention):
+    i = logger.add(tmp_path / "test.log.x", retention=retention)
     logger.debug("test")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
+    check_dir(tmp_path, size=1)
 
     future = datetime.datetime.now() + datetime.timedelta(days=1)
-    monkeypatch_date(
-        future.year,
-        future.month,
-        future.day,
-        future.hour,
-        future.minute,
-        future.second,
-        future.microsecond,
-    )
-
-    i = logger.add(str(tmpdir.join("test.log")), retention=retention)
-    logger.debug("test")
+    with freeze_time(future):
+        i = logger.add(tmp_path / "test.log", retention=retention)
+        logger.debug("test")
 
-    assert len(tmpdir.listdir()) == 2
-    logger.remove(i)
-    assert len(tmpdir.listdir()) == 0
+        check_dir(tmp_path, size=2)
+        logger.remove(i)
+        check_dir(tmp_path, size=0)
 
 
 @pytest.mark.parametrize("retention", [0, 1, 10])
-def test_retention_count(tmpdir, retention):
-    file = tmpdir.join("test.log")
+def test_retention_count(tmp_path, retention):
+    file = tmp_path / "test.log"
 
     for i in range(retention):
-        tmpdir.join("test.2011-01-01_01-01-%d_000001.log" % i).write("test")
+        tmp_path.joinpath("test.2011-01-01_01-01-%d_000001.log" % i).write_text("test")
 
-    i = logger.add(str(file), retention=retention)
+    i = logger.add(file, retention=retention)
     logger.debug("test")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == retention
+    check_dir(tmp_path, size=retention)
 
 
-def test_retention_function(tmpdir):
+def test_retention_function(tmp_path):
     def func(logs):
         for log in logs:
             os.rename(log, log + ".xyz")
 
-    tmpdir.join("test.log.1").write("")
-    tmpdir.join("test").write("")
+    tmp_path.joinpath("test.log.1").write_text("A")
+    tmp_path.joinpath("test").write_text("B")
 
-    i = logger.add(str(tmpdir.join("test.log")), retention=func)
+    i = logger.add(tmp_path / "test.log", retention=func)
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 3
-    assert tmpdir.join("test.log.1.xyz").check(exists=1)
-    assert tmpdir.join("test.log.xyz").check(exists=1)
-    assert tmpdir.join("test").check(exists=1)
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.log.1.xyz", "A"),
+            ("test", "B"),
+            ("test.log.xyz", ""),
+        ],
+    )
 
 
-def test_managed_files(tmpdir):
+def test_managed_files(tmp_path):
     others = {
         "test.log",
         "test.log.1",
         "test.log.1.gz",
         "test.log.rar",
         "test.log",
         "test.2019-11-12_03-22-07_018985.log",
@@ -80,23 +78,23 @@
         "test.2019-11-12_03-22-07_018985.abc.log",
         "test.2019-11-12_03-22-07_018985.123.abc.log",
         "test.foo.log.bar",
         "test.log.log",
     }
 
     for other in others:
-        tmpdir.join(other).write(other)
+        tmp_path.joinpath(other).write_text(other)
 
-    i = logger.add(str(tmpdir.join("test.log")), retention=0, catch=False)
+    i = logger.add(tmp_path / "test.log", retention=0, catch=False)
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 0
+    check_dir(tmp_path, size=0)
 
 
-def test_not_managed_files(tmpdir):
+def test_not_managed_files(tmp_path):
     others = {
         "test_.log",
         "_test.log",
         "tes.log",
         "te.st.log",
         "testlog",
         "test",
@@ -109,268 +107,244 @@
         "foo.test.log.zip",
     }
 
     if os.name != "nt":
         others.add("test.")
 
     for other in others:
-        tmpdir.join(other).write(other)
+        tmp_path.joinpath(other).write_text(other)
 
-    i = logger.add(str(tmpdir.join("test.log")), retention=0, catch=False)
+    i = logger.add(tmp_path / "test.log", retention=0, catch=False)
     logger.remove(i)
 
-    assert set(f.basename for f in tmpdir.listdir()) == others
+    assert set(f.name for f in tmp_path.iterdir()) == others
 
 
 @pytest.mark.parametrize("filename", ["test", "test.log"])
-def test_no_duplicates_in_listed_files(tmpdir, filename):
-    matching_files = None
+def test_no_duplicates_in_listed_files(tmp_path, filename):
     others = [
         "test.log",
         "test.log.log",
         "test.log.log.log",
         "test",
         "test..",
         "test.log..",
         "test..log",
         "test...log",
         "test.log..",
         "test.log.a.log.b",
     ]
 
-    def retention(files):
-        nonlocal matching_files
-        matching_files = files
-
     for other in others:
-        tmpdir.join(other).write(other)
+        tmp_path.joinpath(other).write_text(other)
 
-    i = logger.add(str(tmpdir.join(filename)), retention=retention, catch=False)
+    retention = Mock()
+    i = logger.add(tmp_path / filename, retention=retention, catch=False)
     logger.remove(i)
 
-    assert matching_files is not None
-    assert len(matching_files) == len(set(matching_files))
+    assert retention.call_count == 1
+    assert len(retention.call_args.args[0]) == len(set(retention.call_args.args[0]))
 
 
-def test_directories_ignored(tmpdir):
+def test_directories_ignored(tmp_path):
     others = ["test.log.2", "test.123.log", "test.log.tar.gz", "test.archive"]
 
     for other in others:
-        tmpdir.join(other).mkdir()
+        tmp_path.joinpath(other).mkdir()
 
-    i = logger.add(str(tmpdir.join("test.log")), retention=0, catch=False)
+    i = logger.add(tmp_path / "test.log", retention=0, catch=False)
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == len(others)
+    check_dir(tmp_path, size=len(others))
 
 
-def test_manage_formatted_files(monkeypatch_date, tmpdir):
-    monkeypatch_date(2018, 1, 1, 0, 0, 0, 0)
+def test_manage_formatted_files(freeze_time, tmp_path):
+    with freeze_time("2018-01-01 00:00:00"):
+        f1 = tmp_path / "temp/2018/file.log"
+        f2 = tmp_path / "temp/file2018.log"
+        f3 = tmp_path / "temp/d2018/f2018.2018.log"
 
-    f1 = tmpdir.join("temp/2018/file.log")
-    f2 = tmpdir.join("temp/file2018.log")
-    f3 = tmpdir.join("temp/d2018/f2018.2018.log")
+        a = logger.add(tmp_path / "temp/{time:YYYY}/file.log", retention=0)
+        b = logger.add(tmp_path / "temp/file{time:YYYY}.log", retention=0)
+        c = logger.add(tmp_path / "temp/d{time:YYYY}/f{time:YYYY}.{time:YYYY}.log", retention=0)
 
-    a = logger.add(str(tmpdir.join("temp/{time:YYYY}/file.log")), retention=0)
-    b = logger.add(str(tmpdir.join("temp/file{time:YYYY}.log")), retention=0)
-    c = logger.add(str(tmpdir.join("temp/d{time:YYYY}/f{time:YYYY}.{time:YYYY}.log")), retention=0)
+        logger.debug("test")
 
-    logger.debug("test")
+        assert f1.exists()
+        assert f2.exists()
+        assert f3.exists()
+
+        logger.remove(a)
+        logger.remove(b)
+        logger.remove(c)
 
-    assert f1.check(exists=1)
-    assert f2.check(exists=1)
-    assert f3.check(exists=1)
-
-    logger.remove(a)
-    logger.remove(b)
-    logger.remove(c)
-
-    assert f1.check(exists=0)
-    assert f2.check(exists=0)
-    assert f3.check(exists=0)
+        assert not f1.exists()
+        assert not f2.exists()
+        assert not f3.exists()
 
 
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support '*' in filename")
-def test_date_with_dot_after_extension(monkeypatch_date, tmpdir):
-    file = tmpdir.join("file.{time:YYYY.MM}_log")
+def test_date_with_dot_after_extension(tmp_path):
+    file = tmp_path / "file.{time:YYYY.MM}_log"
 
-    i = logger.add(str(tmpdir.join("file*.log")), retention=0, catch=False)
+    i = logger.add(tmp_path / "file*.log", retention=0, catch=False)
     logger.remove(i)
 
-    assert file.check(exists=0)
+    assert not file.exists()
 
 
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support '*' in filename")
-def test_symbol_in_filename(tmpdir):
-    file = tmpdir.join("file123.log")
-    file.write("")
+def test_symbol_in_filename(tmp_path):
+    file = tmp_path / "file123.log"
+    file.touch()
 
-    i = logger.add(str(tmpdir.join("file*.log")), retention=0, catch=False)
+    i = logger.add(tmp_path / "file*.log", retention=0, catch=False)
     logger.remove(i)
 
-    assert file.check(exists=1)
+    assert file.exists()
 
 
-def test_manage_file_without_extension(tmpdir):
-    file = tmpdir.join("file")
+def test_manage_file_without_extension(tmp_path):
+    file = tmp_path / "file"
 
-    i = logger.add(str(file), retention=0)
+    i = logger.add(file, retention=0)
     logger.debug("?")
-
-    assert len(tmpdir.listdir()) == 1
-    assert file.check(exists=1)
+    check_dir(tmp_path, files=[("file", None)])
     logger.remove(i)
-    assert len(tmpdir.listdir()) == 0
-    assert file.check(exists=0)
+    check_dir(tmp_path, files=[])
 
 
-def test_manage_formatted_files_without_extension(tmpdir):
-    tmpdir.join("file_8").write("")
-    tmpdir.join("file_7").write("")
-    tmpdir.join("file_6").write("")
+def test_manage_formatted_files_without_extension(tmp_path):
+    tmp_path.joinpath("file_8").touch()
+    tmp_path.joinpath("file_7").touch()
+    tmp_path.joinpath("file_6").touch()
 
-    i = logger.add(str(tmpdir.join("file_{time}")), retention=0)
+    i = logger.add(tmp_path / "file_{time}", retention=0)
     logger.debug("1")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 0
+    check_dir(tmp_path, size=0)
 
 
 @pytest.mark.parametrize("mode", ["a", "a+", "w", "x"])
-def test_retention_at_rotation(tmpdir, mode):
-    tmpdir.join("test.log.1").write("")
-    tmpdir.join("test.log.2").write("")
-    tmpdir.join("test.log.3").write("")
+def test_retention_at_rotation(tmp_path, mode):
+    tmp_path.joinpath("test.log.1").touch()
+    tmp_path.joinpath("test.log.2").touch()
+    tmp_path.joinpath("test.log.3").touch()
 
-    logger.add(str(tmpdir.join("test.log")), retention=1, rotation=0, mode=mode)
+    logger.add(tmp_path / "test.log", retention=1, rotation=0, mode=mode)
     logger.debug("test")
 
-    assert len(tmpdir.listdir()) == 2
+    check_dir(tmp_path, size=2)
 
 
 @pytest.mark.parametrize("mode", ["a", "a+", "w", "x"])
-def test_retention_at_remove_without_rotation(tmpdir, mode):
-    i = logger.add(str(tmpdir.join("file.log")), retention=0, mode=mode)
+def test_retention_at_remove_without_rotation(tmp_path, mode):
+    i = logger.add(tmp_path / "file.log", retention=0, mode=mode)
     logger.debug("1")
-    assert len(tmpdir.listdir()) == 1
+    check_dir(tmp_path, size=1)
     logger.remove(i)
-    assert len(tmpdir.listdir()) == 0
+    check_dir(tmp_path, size=0)
 
 
 @pytest.mark.parametrize("mode", ["w", "x", "a", "a+"])
-def test_no_retention_at_remove_with_rotation(tmpdir, mode):
-    i = logger.add(str(tmpdir.join("file.log")), retention=0, rotation="100 MB", mode=mode)
+def test_no_retention_at_remove_with_rotation(tmp_path, mode):
+    i = logger.add(tmp_path / "file.log", retention=0, rotation="100 MB", mode=mode)
     logger.debug("1")
-    assert len(tmpdir.listdir()) == 1
+    check_dir(tmp_path, size=1)
     logger.remove(i)
-    assert len(tmpdir.listdir()) == 1
+    check_dir(tmp_path, size=1)
 
 
-def test_no_renaming(tmpdir):
-    i = logger.add(str(tmpdir.join("test.log")), format="{message}", retention=10)
+def test_no_renaming(tmp_path):
+    i = logger.add(tmp_path / "test.log", format="{message}", retention=10)
     logger.debug("test")
     logger.remove(i)
 
-    assert len(tmpdir.listdir()) == 1
-    assert tmpdir.join("test.log").read() == "test\n"
+    check_dir(tmp_path, files=[("test.log", "test\n")])
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_retention_at_rotation(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_retention(files):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Retention error")
+def test_exception_during_retention_at_rotation(freeze_time, tmp_path, capsys, delay):
+    with freeze_time("2022-02-22") as frozen:
+        logger.add(
+            tmp_path / "test.log",
+            format="{message}",
+            retention=Mock(side_effect=[Exception("Retention error"), None]),
+            rotation=0,
+            catch=True,
+            delay=delay,
+        )
+        logger.debug("AAA")
+        frozen.tick()
+        logger.debug("BBB")
 
-    logger.add(
-        str(tmpdir.join("test.log")),
-        format="{message}",
-        retention=failing_retention,
-        rotation=0,
-        catch=True,
-        delay=delay,
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.2022-02-22_00-00-00_000000.log", ""),
+            ("test.2022-02-22_00-00-01_000000.log", ""),
+            ("test.log", "BBB\n"),
+        ],
     )
 
-    logger.debug("AAA")
-    logger.debug("BBB")
-
-    files = sorted(tmpdir.listdir())
     out, err = capsys.readouterr()
-
-    assert len(files) == 3
-    assert [file.read() for file in files] == ["", "", "BBB\n"]
     assert out == ""
     assert err.count("Logging error in Loguru Handler") == 1
     assert err.count("Exception: Retention error") == 1
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_retention_at_rotation_not_caught(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_retention(files):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Retention error")
-
-    logger.add(
-        str(tmpdir.join("test.log")),
-        format="{message}",
-        retention=failing_retention,
-        rotation=0,
-        catch=False,
-        delay=delay,
+def test_exception_during_retention_at_rotation_not_caught(freeze_time, tmp_path, capsys, delay):
+    with freeze_time("2022-02-22") as frozen:
+        logger.add(
+            tmp_path / "test.log",
+            format="{message}",
+            retention=Mock(side_effect=[OSError("Retention error"), None]),
+            rotation=0,
+            catch=False,
+            delay=delay,
+        )
+        with pytest.raises(OSError, match=r"Retention error"):
+            logger.debug("AAA")
+        frozen.tick()
+        logger.debug("BBB")
+
+    check_dir(
+        tmp_path,
+        files=[
+            ("test.2022-02-22_00-00-00_000000.log", ""),
+            ("test.2022-02-22_00-00-01_000000.log", ""),
+            ("test.log", "BBB\n"),
+        ],
     )
 
-    with pytest.raises(Exception, match=r"Retention error"):
-        logger.debug("AAA")
-
-    logger.debug("BBB")
-
-    files = sorted(tmpdir.listdir())
     out, err = capsys.readouterr()
-
-    assert len(files) == 3
-    assert [file.read() for file in files] == ["", "", "BBB\n"]
     assert out == err == ""
 
 
 @pytest.mark.parametrize("delay", [True, False])
-def test_exception_during_retention_at_remove(tmpdir, capsys, delay):
-    raising = True
-
-    def failing_retention(files):
-        nonlocal raising
-        if raising:
-            raising = False
-            raise Exception("Retention error")
-
+def test_exception_during_retention_at_remove(tmp_path, capsys, delay):
     i = logger.add(
-        str(tmpdir.join("test.log")),
+        tmp_path / "test.log",
         format="{message}",
-        retention=failing_retention,
+        retention=Mock(side_effect=[OSError("Retention error"), None]),
         catch=False,
         delay=delay,
     )
     logger.debug("AAA")
 
-    with pytest.raises(Exception, match=r"Retention error"):
+    with pytest.raises(OSError, match=r"Retention error"):
         logger.remove(i)
 
     logger.debug("Nope")
 
-    files = sorted(tmpdir.listdir())
-    out, err = capsys.readouterr()
+    check_dir(tmp_path, files=[("test.log", "AAA\n")])
 
-    assert len(files) == 1
-    assert tmpdir.join("test.log").read() == "AAA\n"
+    out, err = capsys.readouterr()
     assert out == err == ""
 
 
 @pytest.mark.parametrize("retention", [datetime.time(12, 12, 12), os, object()])
 def test_invalid_retention(retention):
     with pytest.raises(TypeError):
         logger.add("test.log", retention=retention)
```

### Comparing `loguru-0.6.0/tests/test_formatting.py` & `loguru-0.7.0/tests/test_formatting.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,39 +51,39 @@
     "format, validator",
     [
         ("{time}.log", lambda r: re.fullmatch(r"\d+-\d+-\d+_\d+-\d+-\d+\_\d+.log", r)),
         ("%s_{{a}}_天_{{1}}_%d", lambda r: r == "%s_{a}_天_{1}_%d"),
     ],
 )
 @pytest.mark.parametrize("part", ["file", "dir", "both"])
-def test_file_formatters(tmpdir, format, validator, part):
+def test_file_formatters(tmp_path, format, validator, part):
     if part == "file":
-        file = tmpdir.join(format)
+        file = tmp_path.joinpath(format)
     elif part == "dir":
-        file = tmpdir.join(format, "log.log")
+        file = tmp_path.joinpath(format, "log.log")
     elif part == "both":
-        file = tmpdir.join(format, format)
+        file = tmp_path.joinpath(format, format)
 
-    logger.add(str(file))
+    logger.add(file)
     logger.debug("Message")
 
-    files = [f for f in tmpdir.visit() if f.check(file=1)]
+    files = [f for f in tmp_path.glob("**/*") if f.is_file()]
 
     assert len(files) == 1
 
     file = files[0]
 
     if part == "file":
-        assert validator(file.basename)
+        assert validator(file.name)
     elif part == "dir":
-        assert file.basename == "log.log"
-        assert validator(file.dirpath().basename)
+        assert file.name == "log.log"
+        assert validator(file.parent.name)
     elif part == "both":
-        assert validator(file.basename)
-        assert validator(file.dirpath().basename)
+        assert validator(file.name)
+        assert validator(file.parent.name)
 
 
 @pytest.mark.parametrize(
     "message, args, kwargs, expected",
     [
         ("{1, 2, 3} - {0} - {", [], {}, "{1, 2, 3} - {0} - {"),
         ("{} + {} = {}", [1, 2, 3], {}, "1 + 2 = 3"),
```

### Comparing `loguru-0.6.0/tests/test_get_frame.py` & `loguru-0.7.0/tests/test_get_frame.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_interception.py` & `loguru-0.7.0/tests/test_interception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import logging
+import sys
 
 from loguru import logger
 
 from .conftest import make_logging_logger
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
-        # Get corresponding Loguru level if it exists
+        # Get corresponding Loguru level if it exists.
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
-        # Find caller from where originated the logged message
-        frame, depth = logging.currentframe(), 2
-        while frame.f_code.co_filename == logging.__file__:
+        # Find caller from where originated the logged message.
+        frame, depth = sys._getframe(6), 6
+        while frame and frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def test_formatting(writer):
     fmt = (
         "{name} - {file.name} - {function} - {level.name} - "
         "{level.no} - {line} - {module} - {message}"
     )
 
     expected = (
         "tests.test_interception - test_interception.py - test_formatting - DEBUG - "
-        "10 - 38 - test_interception - This is the message\n"
+        "10 - 39 - test_interception - This is the message\n"
     )
 
     with make_logging_logger("tests", InterceptHandler()) as logging_logger:
         logger.add(writer, format=fmt)
         logging_logger.debug("This is the %s", "message")
 
     result = writer.read()
@@ -153,8 +154,8 @@
 
 def test_using_logging_function(writer):
     with make_logging_logger(None, InterceptHandler()):
         logger.add(writer, format="{function} {line} {module} {file.name} {message}")
         logging.warning("ABC")
 
     result = writer.read()
-    assert result == "test_using_logging_function 157 test_interception test_interception.py ABC\n"
+    assert result == "test_using_logging_function 158 test_interception test_interception.py ABC\n"
```

### Comparing `loguru-0.6.0/tests/test_levels.py` & `loguru-0.7.0/tests/test_levels.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,26 +65,26 @@
     logger.log(15, " A ")
     logger.log(name, " B ")
 
     assert writer.read() == parse("Level 15 & 15 &  A \x1b[0m\nLevel 15 & 45 & <red> B </red>\n")
 
 
 def test_add_existing_level(writer):
-    logger.level("INFO", color="<red>")
+    logger.level("DEBUG", color="<red>")
     fmt = "{level.icon} + <level>{level.name}</level> + {level.no} = {message}"
     logger.add(writer, format=fmt, colorize=True)
 
-    logger.info("a")
-    logger.log("INFO", "b")
+    logger.debug("a")
+    logger.log("DEBUG", "b")
     logger.log(10, "c")
     logger.log(20, "d")
 
     assert writer.read() == parse(
-        "ℹ️ + <red>INFO</red> + 20 = a\n"
-        "ℹ️ + <red>INFO</red> + 20 = b\n"
+        "🐞 + <red>DEBUG</red> + 10 = a\n"
+        "🐞 + <red>DEBUG</red> + 10 = b\n"
         "  + Level 10\x1b[0m + 10 = c\n"
         "  + Level 20\x1b[0m + 20 = d\n"
     )
 
 
 def test_blank_color(writer):
     logger.level("INFO", color=" ")
@@ -176,69 +176,84 @@
     logger.bind(something="otherthing").foobar("Another message")
     assert writer.read() == parse(
         "<blue>foobar 33 🤖 Logged message {}</blue>\n"
         "<blue>foobar 33 🤖 Another message {'something': 'otherthing'}</blue>\n"
     )
 
 
-def test_updating_level_no_not_allowed():
-    with pytest.raises(TypeError, match=r".*can't update its severity"):
+def test_updating_level_no_not_allowed_default():
+    with pytest.raises(TypeError, match="can't update its severity"):
         logger.level("DEBUG", 100)
 
 
-@pytest.mark.parametrize("level", [3.4, object()])
-def test_log_invalid_level(writer, level):
+def test_updating_level_no_not_allowed_custom():
+    logger.level("foobar", no=33)
+    with pytest.raises(TypeError, match="can't update its severity"):
+        logger.level("foobar", 100)
+
+
+@pytest.mark.parametrize("level", [3.4, object(), set()])
+def test_log_invalid_level_type(writer, level):
+    logger.add(writer)
+    with pytest.raises(TypeError, match="Invalid level, it should be an integer or a string"):
+        logger.log(level, "test")
+
+
+@pytest.mark.parametrize("level", [-1, -999])
+def test_log_invalid_level_value(writer, level):
     logger.add(writer)
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError, match="Invalid level value, it should be a positive integer"):
         logger.log(level, "test")
 
 
-@pytest.mark.parametrize("level", ["foo", "debug", -1])
+@pytest.mark.parametrize("level", ["foo", "debug"])
 def test_log_unknown_level(writer, level):
     logger.add(writer)
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Level '[^']+' does not exist"):
         logger.log(level, "test")
 
 
-@pytest.mark.parametrize("level_name", [10, object()])
+@pytest.mark.parametrize("level_name", [10, object(), set()])
 def test_add_invalid_level_name(level_name):
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match="Invalid level name, it should be a string"):
         logger.level(level_name, 11)
 
 
-@pytest.mark.parametrize("level_value", ["1", object(), 3.4])
+@pytest.mark.parametrize("level_value", ["1", object(), 3.4, set()])
 def test_add_invalid_level_type(level_value):
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match="Invalid level no, it should be an integer"):
         logger.level("test", level_value)
 
 
-def test_add_invalid_level_value():
-    with pytest.raises(ValueError):
-        logger.level("test", -1)
+@pytest.mark.parametrize("level_value", [-1, -999])
+def test_add_invalid_level_value(level_value):
+    with pytest.raises(ValueError, match="Invalid level no, it should be a positive integer"):
+        logger.level("test", level_value)
 
 
-@pytest.mark.parametrize("level", [10, object()])
+@pytest.mark.parametrize("level", [10, object(), set()])
 def test_get_invalid_level(level):
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match="Invalid level name, it should be a string"):
         logger.level(level)
 
 
 def test_get_unknown_level():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=r"Level '[^']+' does not exist"):
         logger.level("foo")
 
 
-@pytest.mark.parametrize("level", [10, object()])
+@pytest.mark.parametrize("level", [10, object(), set()])
 def test_edit_invalid_level(level):
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match="Invalid level name, it should be a string"):
         logger.level(level, icon="?")
 
 
-def test_edit_unknown_level():
-    with pytest.raises(ValueError):
-        logger.level("foo", icon="?")
+@pytest.mark.parametrize("level_name", ["foo", "debug"])
+def test_edit_unknown_level(level_name):
+    with pytest.raises(ValueError, match=r"Level '[^']+' does not exist"):
+        logger.level(level_name, icon="?")
 
 
 @pytest.mark.parametrize("color", ["</>", "<foo>", "</red>", "<lvl>", " <level> "])
 def test_add_invalid_level_color(color):
     with pytest.raises(ValueError):
         logger.level("foobar", no=20, icon="", color=color)
```

### Comparing `loguru-0.6.0/tests/test_multiprocessing.py` & `loguru-0.7.0/tests/test_multiprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     def write(self, message):
         self._output += message
 
     def read(self):
         return self._output
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_apply_spawn(spawn_context):
     writer = Writer()
 
     logger.add(writer, format="{message}", enqueue=True, catch=False)
 
     with spawn_context.Pool(1, set_logger, [logger]) as pool:
         for i in range(3):
@@ -152,15 +151,14 @@
 
     logger.info("Done!")
     logger.remove()
 
     assert writer.read() == "#0\n#1\n#2\nDone!\n"
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_apply_async_spawn(spawn_context):
     writer = Writer()
 
     logger.add(writer, format="{message}", enqueue=True, catch=False)
 
     with spawn_context.Pool(1, set_logger, [logger]) as pool:
         for i in range(3):
@@ -209,15 +207,14 @@
 
     logger.info("Done!")
     logger.remove()
 
     assert writer.read() == "#0\n#1\n#2\nDone!\n"
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_process_spawn(spawn_context):
     writer = Writer()
 
     logger.add(writer, format="{message}", enqueue=True, catch=False)
 
     process = spawn_context.Process(target=subworker, args=(logger,))
     process.start()
@@ -263,15 +260,14 @@
 
     logger.info("Main")
     logger.remove()
 
     assert writer.read() == "Child\nMain\n"
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_remove_in_child_process_spawn(spawn_context):
     writer = Writer()
 
     logger.add(writer, format="{message}", enqueue=True, catch=False)
 
     process = spawn_context.Process(target=subworker_remove, args=(logger,))
     process.start()
@@ -317,15 +313,14 @@
 
     logger.info("Main")
     logger.remove()
 
     assert writer.read() == "Child\nMain\n"
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_remove_in_main_process_spawn(spawn_context):
     # Actually, this test may fail if sleep time in main process is too small (and no barrier used)
     # In such situation, it seems the child process has not enough time to initialize itself
     # It may fail with an "EOFError" during unpickling of the (garbage collected / closed) Queue
     writer = Writer()
     barrier = spawn_context.Barrier(2)
 
@@ -377,15 +372,14 @@
     process.join()
 
     assert process.exitcode == 0
 
     assert writer.read() == "Child\nMain\n"
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
 def test_await_complete_spawn(capsys, spawn_context):
     async def writer(msg):
         print(msg, end="")
 
     loop = asyncio.new_event_loop()
 
     logger.add(writer, format="{message}", loop=loop, enqueue=True, catch=False)
@@ -452,106 +446,105 @@
     loop.run_until_complete(local())
 
     out, err = capsys.readouterr()
     assert out == "Child\n"
     assert err == ""
 
 
-@pytest.mark.skipif(platform.python_implementation() == "PyPy", reason="PyPy bug #3630")
-def test_not_picklable_sinks_spawn(spawn_context, tmpdir, capsys):
-    filepath = tmpdir.join("test.log")
+def test_not_picklable_sinks_spawn(spawn_context, tmp_path, capsys):
+    filepath = tmp_path / "test.log"
     stream = sys.stderr
     output = []
 
-    logger.add(str(filepath), format="{message}", enqueue=True, catch=False)
+    logger.add(filepath, format="{message}", enqueue=True, catch=False)
     logger.add(stream, format="{message}", enqueue=True)
     logger.add(lambda m: output.append(m), format="{message}", enqueue=True)
 
     process = spawn_context.Process(target=subworker, args=[logger])
     process.start()
     process.join()
 
     assert process.exitcode == 0
 
     logger.info("Main")
     logger.remove()
 
     out, err = capsys.readouterr()
 
-    assert filepath.read() == "Child\nMain\n"
+    assert filepath.read_text() == "Child\nMain\n"
     assert out == ""
     assert err == "Child\nMain\n"
     assert output == ["Child\n", "Main\n"]
 
 
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support forking")
-def test_not_picklable_sinks_fork(capsys, tmpdir, fork_context):
-    filepath = tmpdir.join("test.log")
+def test_not_picklable_sinks_fork(capsys, tmp_path, fork_context):
+    filepath = tmp_path / "test.log"
     stream = sys.stderr
     output = []
 
-    logger.add(str(filepath), format="{message}", enqueue=True, catch=False)
+    logger.add(filepath, format="{message}", enqueue=True, catch=False)
     logger.add(stream, format="{message}", enqueue=True, catch=False)
     logger.add(lambda m: output.append(m), format="{message}", enqueue=True, catch=False)
 
     process = fork_context.Process(target=subworker, args=[logger])
     process.start()
     process.join()
 
     assert process.exitcode == 0
 
     logger.info("Main")
     logger.remove()
 
     out, err = capsys.readouterr()
 
-    assert filepath.read() == "Child\nMain\n"
+    assert filepath.read_text() == "Child\nMain\n"
     assert out == ""
     assert err == "Child\nMain\n"
     assert output == ["Child\n", "Main\n"]
 
 
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support forking")
-def test_not_picklable_sinks_inheritance(capsys, tmpdir, fork_context):
-    filepath = tmpdir.join("test.log")
+def test_not_picklable_sinks_inheritance(capsys, tmp_path, fork_context):
+    filepath = tmp_path / "test.log"
     stream = sys.stderr
     output = []
 
-    logger.add(str(filepath), format="{message}", enqueue=True, catch=False)
+    logger.add(filepath, format="{message}", enqueue=True, catch=False)
     logger.add(stream, format="{message}", enqueue=True, catch=False)
     logger.add(lambda m: output.append(m), format="{message}", enqueue=True, catch=False)
 
     process = fork_context.Process(target=subworker_inheritance)
     process.start()
     process.join()
 
     assert process.exitcode == 0
 
     logger.info("Main")
     logger.remove()
 
     out, err = capsys.readouterr()
 
-    assert filepath.read() == "Child\nMain\n"
+    assert filepath.read_text() == "Child\nMain\n"
     assert out == ""
     assert err == "Child\nMain\n"
     assert output == ["Child\n", "Main\n"]
 
 
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support forking")
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="No 'os.register_at_fork()' function")
 @pytest.mark.parametrize("enqueue", [True, False])
 @pytest.mark.parametrize("deepcopied", [True, False])
-def test_no_deadlock_if_internal_lock_in_use(tmpdir, enqueue, deepcopied, fork_context):
+def test_no_deadlock_if_internal_lock_in_use(tmp_path, enqueue, deepcopied, fork_context):
     if deepcopied:
         logger_ = copy.deepcopy(logger)
     else:
         logger_ = logger
 
-    output = tmpdir.join("stdout.txt")
+    output = tmp_path / "stdout.txt"
     stdout = output.open("w")
 
     def slow_sink(msg):
         time.sleep(0.5)
         stdout.write(msg)
         stdout.flush()
 
@@ -566,21 +559,21 @@
     thread = threading.Thread(target=main)
     thread.start()
 
     process = fork_context.Process(target=worker)
     process.start()
 
     thread.join()
-    process.join(1)
+    process.join(2)
 
     assert process.exitcode == 0
 
     logger_.remove()
 
-    assert output.read() in ("Main\nChild\n", "Child\nMain\n")
+    assert output.read_text() in ("Main\nChild\n", "Child\nMain\n")
 
 
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="No 'os.register_at_fork()' function")
 @pytest.mark.skipif(os.name == "nt", reason="Windows does not support forking")
 @pytest.mark.parametrize("enqueue", [True, False])
 def test_no_deadlock_if_external_lock_in_use(enqueue, capsys, fork_context):
     # Can't reproduce the bug on pytest (even if stderr is not wrapped), but let it anyway
```

### Comparing `loguru-0.6.0/tests/test_opt.py` & `loguru-0.7.0/tests/test_opt.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_parse.py` & `loguru-0.7.0/tests/test_parse.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 
 @pytest.fixture
 def fileobj():
     with io.StringIO(TEXT) as file:
         yield file
 
 
-def test_parse_file(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write(TEXT)
-    result, *_ = list(logger.parse(str(file), r"(?P<num>\d+)"))
+def test_parse_file(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text(TEXT)
+    result, *_ = list(logger.parse(file, r"(?P<num>\d+)"))
     assert result == dict(num="123456789")
 
 
-def test_parse_fileobj(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write(TEXT)
+def test_parse_fileobj(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text(TEXT)
     result, *_ = list(logger.parse(open(str(file)), r"^(?P<t>\w+)"))
     assert result == dict(t="This")
 
 
-def test_parse_pathlib(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write(TEXT)
+def test_parse_pathlib(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text(TEXT)
     result, *_ = list(logger.parse(pathlib.Path(str(file)), r"(?P<r>Random)"))
     assert result == dict(r="Random")
 
 
 def test_parse_string_pattern(fileobj):
     result, *_ = list(logger.parse(fileobj, r"(?P<num>\d+)"))
     assert result == dict(num="123456789")
@@ -56,19 +56,19 @@
 def test_parse_without_group(fileobj):
     result, *_ = list(logger.parse(fileobj, r"\d+"))
     assert result == {}
 
 
 def test_parse_bytes():
     with io.BytesIO(b"Testing bytes!") as fileobj:
-        result, *_ = list(logger.parse(fileobj, br"(?P<ponct>[?!:])"))
+        result, *_ = list(logger.parse(fileobj, rb"(?P<ponct>[?!:])"))
     assert result == dict(ponct=b"!")
 
 
-@pytest.mark.parametrize("chunk", [-1, 1, 2 ** 16])
+@pytest.mark.parametrize("chunk", [-1, 1, 2**16])
 def test_chunk(fileobj, chunk):
     result, *_ = list(logger.parse(fileobj, r"(?P<a>[ABC]+)", chunk=chunk))
     assert result == dict(a="ABC")
 
 
 def test_positive_lookbehind_pattern():
     text = "ab" * 100
@@ -82,52 +82,52 @@
     text = ("\n" + "a" * 100) * 1000
     pattern = r"\n(?P<a>a+)"
     with io.StringIO(text) as file:
         result = list(logger.parse(file, pattern, chunk=30))
     assert result == [dict(a="a" * 100)] * 1000
 
 
-def test_cast_dict(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("[123] [1.1] [2017-03-29 11:11:11]\n")
+def test_cast_dict(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("[123] [1.1] [2017-03-29 11:11:11]\n")
     regex = r"\[(?P<num>.*)\] \[(?P<val>.*)\] \[(?P<date>.*)\]"
     caster = dict(num=int, val=float, date=lambda d: datetime.strptime(d, "%Y-%m-%d %H:%M:%S"))
-    result = next(logger.parse(str(file), regex, cast=caster))
+    result = next(logger.parse(file, regex, cast=caster))
     assert result == dict(num=123, val=1.1, date=datetime(2017, 3, 29, 11, 11, 11))
 
 
-def test_cast_function(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("[123] [1.1] [2017-03-29 11:11:11]\n")
+def test_cast_function(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("[123] [1.1] [2017-03-29 11:11:11]\n")
     regex = r"\[(?P<num>.*)\] \[(?P<val>.*)\] \[(?P<date>.*)\]"
 
     def caster(groups):
         groups["num"] = int(groups["num"])
         groups["val"] = float(groups["val"])
         groups["date"] = datetime.strptime(groups["date"], "%Y-%m-%d %H:%M:%S")
 
-    result = next(logger.parse(str(file), regex, cast=caster))
+    result = next(logger.parse(file, regex, cast=caster))
     assert result == dict(num=123, val=1.1, date=datetime(2017, 3, 29, 11, 11, 11))
 
 
-def test_cast_with_irrelevant_arg(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("[123] Blabla")
+def test_cast_with_irrelevant_arg(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("[123] Blabla")
     regex = r"\[(?P<a>\d+)\] .*"
     caster = dict(a=int, b=float)
-    result = next(logger.parse(str(file), regex, cast=caster))
+    result = next(logger.parse(file, regex, cast=caster))
     assert result == dict(a=123)
 
 
-def test_cast_with_irrelevant_value(tmpdir):
-    file = tmpdir.join("test.log")
-    file.write("[123] Blabla")
+def test_cast_with_irrelevant_value(tmp_path):
+    file = tmp_path / "test.log"
+    file.write_text("[123] Blabla")
     regex = r"\[(?P<a>\d+)\] (?P<b>.*)"
     caster = dict(a=int)
-    result = next(logger.parse(str(file), regex, cast=caster))
+    result = next(logger.parse(file, regex, cast=caster))
     assert result == dict(a=123, b="Blabla")
 
 
 @pytest.mark.parametrize("file", [object(), 123, dict])
 def test_invalid_file(file):
     with pytest.raises(TypeError):
         next(logger.parse(file, r"pattern"))
```

### Comparing `loguru-0.6.0/tests/test_pickling.py` & `loguru-0.7.0/tests/test_pickling.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def emit(self, record):
         self.written += record.getMessage()
 
     def acquire(self):
         pass
 
-    def createLock(self):
+    def createLock(self):  # noqa: N802
         return None
 
 
 def format_function(record):
     return "-> <red>{message}</red>"
 
 
@@ -127,39 +127,39 @@
     unpickled = pickle.loads(pickled)
     unpickled.debug("A message")
     handler = next(iter(unpickled._core.handlers.values()))._sink._handler
     assert handler.written == "DEBUG - test_pickling_standard_handler - A message"
 
 
 def test_pickling_standard_handler_root_logger_not_picklable(monkeypatch, capsys):
-    def __reduce__():
+    def reduce_protocol():
         raise TypeError("Not picklable")
 
-    monkeypatch.setattr(logging.getLogger(), "__reduce__", __reduce__, raising=False)
+    monkeypatch.setattr(logging.getLogger(), "__reduce__", reduce_protocol, raising=False)
 
     handler = StandardHandler(logging.NOTSET)
     logger.add(handler, format="=> {message}", catch=False)
 
     pickled = pickle.dumps(logger)
     pickle.loads(pickled)
 
     logger.info("Ok")
     out, err = capsys.readouterr()
     assert out == ""
     assert err == ""
     assert handler.written == "=> Ok"
 
 
-def test_pickling_file_handler(tmpdir):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="{level} - {function} - {message}", delay=True)
+def test_pickling_file_handler(tmp_path):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{level} - {function} - {message}", delay=True)
     pickled = pickle.dumps(logger)
     unpickled = pickle.loads(pickled)
     unpickled.debug("A message")
-    assert file.read() == "DEBUG - test_pickling_file_handler - A message\n"
+    assert file.read_text() == "DEBUG - test_pickling_file_handler - A message\n"
 
 
 @pytest.mark.parametrize(
     "rotation",
     [
         1000,
         "daily",
@@ -167,47 +167,43 @@
         datetime.time(hour=12, minute=00, second=00),
         "200 MB",
         "10:00",
         "5 hours",
         rotation_function,
     ],
 )
-def test_pickling_file_handler_rotation(tmpdir, rotation):
-    file = tmpdir.join("test.log")
-    logger.add(str(file), format="{level} - {function} - {message}", delay=True, rotation=rotation)
+def test_pickling_file_handler_rotation(tmp_path, rotation):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{level} - {function} - {message}", delay=True, rotation=rotation)
     pickled = pickle.dumps(logger)
     unpickled = pickle.loads(pickled)
     unpickled.debug("A message")
-    assert file.read() == "DEBUG - test_pickling_file_handler_rotation - A message\n"
+    assert file.read_text() == "DEBUG - test_pickling_file_handler_rotation - A message\n"
 
 
 @pytest.mark.parametrize(
     "retention", [1000, datetime.timedelta(hours=13), "10 days", retention_function]
 )
-def test_pickling_file_handler_retention(tmpdir, retention):
-    file = tmpdir.join("test.log")
-    logger.add(
-        str(file), format="{level} - {function} - {message}", delay=True, retention=retention
-    )
+def test_pickling_file_handler_retention(tmp_path, retention):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{level} - {function} - {message}", delay=True, retention=retention)
     pickled = pickle.dumps(logger)
     unpickled = pickle.loads(pickled)
     unpickled.debug("A message")
-    assert file.read() == "DEBUG - test_pickling_file_handler_retention - A message\n"
+    assert file.read_text() == "DEBUG - test_pickling_file_handler_retention - A message\n"
 
 
 @pytest.mark.parametrize("compression", ["zip", "gz", "tar", compression_function])
-def test_pickling_file_handler_compression(tmpdir, compression):
-    file = tmpdir.join("test.log")
-    logger.add(
-        str(file), format="{level} - {function} - {message}", delay=True, compression=compression
-    )
+def test_pickling_file_handler_compression(tmp_path, compression):
+    file = tmp_path / "test.log"
+    logger.add(file, format="{level} - {function} - {message}", delay=True, compression=compression)
     pickled = pickle.dumps(logger)
     unpickled = pickle.loads(pickled)
     unpickled.debug("A message")
-    assert file.read() == "DEBUG - test_pickling_file_handler_compression - A message\n"
+    assert file.read_text() == "DEBUG - test_pickling_file_handler_compression - A message\n"
 
 
 def test_pickling_no_handler(writer):
     pickled = pickle.dumps(logger)
     unpickled = pickle.loads(pickled)
     unpickled.add(writer, format="{level} - {function} - {message}")
     unpickled.debug("A message")
```

### Comparing `loguru-0.6.0/tests/test_propagation.py` & `loguru-0.7.0/tests/test_propagation.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_recattr.py` & `loguru-0.7.0/tests/test_recattr.py`

 * *Files identical despite different names*

### Comparing `loguru-0.6.0/tests/test_remove.py` & `loguru-0.7.0/tests/test_remove.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 
 class StopSinkError:
     def write(self, message):
         print(message, end="")
 
     def stop(self):
-        raise Exception("Stop error")
+        raise OSError("Stop error")
 
 
-def test_remove_all(tmpdir, writer, capsys):
-    file = tmpdir.join("test.log")
+def test_remove_all(tmp_path, writer, capsys):
+    file = tmp_path / "test.log"
 
     logger.debug("This shouldn't be printed.")
 
-    logger.add(str(file), format="{message}")
+    logger.add(file, format="{message}")
     logger.add(sys.stdout, format="{message}")
     logger.add(sys.stderr, format="{message}")
     logger.add(writer, format="{message}")
 
     message = "some message"
     expected = message + "\n"
 
@@ -31,15 +31,15 @@
 
     logger.remove()
 
     logger.debug("This shouldn't be printed neither.")
 
     out, err = capsys.readouterr()
 
-    assert file.read() == expected
+    assert file.read_text() == expected
     assert out == expected
     assert err == expected
     assert writer.read() == expected
 
 
 def test_remove_simple(writer):
     i = logger.add(writer, format="{message}")
@@ -54,45 +54,45 @@
     logger.debug("1")
     time.sleep(0.1)
     logger.remove(i)
     logger.debug("2")
     assert writer.read() == "1\n"
 
 
-def test_remove_enqueue_filesink(tmpdir):
-    file = tmpdir.join("test.log")
-    i = logger.add(str(file), format="{message}", enqueue=True)
+def test_remove_enqueue_filesink(tmp_path):
+    file = tmp_path / "test.log"
+    i = logger.add(file, format="{message}", enqueue=True)
     logger.debug("1")
     logger.remove(i)
-    assert file.read() == "1\n"
+    assert file.read_text() == "1\n"
 
 
 def test_exception_in_stop_during_remove_one(capsys):
     i = logger.add(StopSinkError(), catch=False, format="{message}")
     logger.info("A")
-    with pytest.raises(Exception, match=r"Stop error"):
+    with pytest.raises(OSError, match=r"Stop error"):
         logger.remove(i)
     logger.info("Nope")
 
     out, err = capsys.readouterr()
 
     assert out == "A\n"
     assert err == ""
 
 
 def test_exception_in_stop_not_caught_during_remove_all(capsys):
     logger.add(StopSinkError(), catch=False, format="{message}")
     logger.add(StopSinkError(), catch=False, format="{message}")
 
-    with pytest.raises(Exception, match=r"Stop error"):
+    with pytest.raises(OSError, match=r"Stop error"):
         logger.remove()
 
     logger.info("A")
 
-    with pytest.raises(Exception, match=r"Stop error"):
+    with pytest.raises(OSError, match=r"Stop error"):
         logger.remove()
 
     logger.info("Nope")
 
     out, err = capsys.readouterr()
 
     assert out == "A\n"
```

### Comparing `loguru-0.6.0/tests/test_repr.py` & `loguru-0.7.0/tests/test_repr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,44 @@
-import builtins
 import logging
 import pathlib
 import re
 import sys
-from inspect import iscoroutinefunction
 
-import loguru
 from loguru import logger
 
 
-class Wrapper:
-    def __init__(self, wrapped, *, repr, name):
-        self._wrapped = wrapped
-        self._repr = repr
-        self._name = name
-        self.raised = False
-
-    def __repr__(self):
-        return self._repr
-
-    def __getattr__(self, name):
-        if name == "__name__":
-            if self._name is None:
-                self.raised = True
-                raise AttributeError
-            else:
-                return self._name
-        return getattr(self._wrapped, name)
-
-
 def test_no_handler():
     assert repr(logger) == "<loguru.logger handlers=[]>"
 
 
 def test_stderr():
     logger.add(sys.__stderr__)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<stderr>)]>"
 
 
 def test_stdout():
     logger.add(sys.__stdout__)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<stdout>)]>"
 
 
-def test_file_object(tmpdir):
-    path = str(tmpdir.join("test.log"))
+def test_file_object(tmp_path):
+    path = str(tmp_path / "test.log")
     file = open(path, "w")
     logger.add(file)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=%s)]>" % path
 
 
-def test_file_str(tmpdir):
-    path = str(tmpdir.join("test.log"))
+def test_file_str(tmp_path):
+    path = str(tmp_path / "test.log")
     logger.add(path)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink='%s')]>" % path
 
 
-def test_file_pathlib(tmpdir):
-    path = str(tmpdir.join("test.log"))
+def test_file_pathlib(tmp_path):
+    path = str(tmp_path / "test.log")
     logger.add(pathlib.Path(path))
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink='%s')]>" % path
 
 
 def test_stream_object():
     class MyStream:
         def __init__(self, name):
@@ -108,66 +85,74 @@
     def my_function(message):
         pass
 
     logger.add(my_function)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=my_function)]>"
 
 
-def test_function_without_name(monkeypatch):
-    function = Wrapper(lambda _: None, repr="<FunctionWithout>", name=None)
-    monkeypatch.setattr(builtins, "callable", lambda x: x is function or callable(x))
+def test_callable_without_name():
+    class Function:
+        def __call__(self):
+            pass
+
+        def __repr__(self):
+            return "<FunctionWithout>"
 
-    logger.add(function)
+    logger.add(Function())
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<FunctionWithout>)]>"
-    assert function.raised
 
 
-def test_function_with_empty_name(monkeypatch):
-    function = Wrapper(lambda _: None, repr="<FunctionEmpty>", name="")
-    monkeypatch.setattr(builtins, "callable", lambda x: x is function or callable(x))
+def test_callable_with_empty_name():
+    class Function:
+        __name__ = ""
+
+        def __call__(self):
+            pass
+
+        def __repr__(self):
+            return "<FunctionEmpty>"
 
-    logger.add(function)
+    logger.add(Function())
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<FunctionEmpty>)]>"
-    assert not function.raised
 
 
 def test_coroutine_function():
     async def my_async_function(message):
         pass
 
     logger.add(my_async_function)
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=my_async_function)]>"
 
 
-def test_coroutine_function_without_name(monkeypatch):
-    async_function = Wrapper(lambda _: None, repr="<AsyncFunctionWithout>", name=None)
-    monkeypatch.setattr(
-        loguru._logger,
-        "iscoroutinefunction",
-        lambda x: x is async_function or iscoroutinefunction(x),
-    )
+def test_coroutine_callable_without_name():
+    class CoroutineFunction:
+        async def __call__(self):
+            pass
 
-    logger.add(async_function)
+        def __repr__(self):
+            return "<AsyncFunctionWithout>"
+
+    logger.add(CoroutineFunction())
     assert (
         repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<AsyncFunctionWithout>)]>"
     )
-    assert async_function.raised
 
 
-def test_coroutine_function_with_empty_name(monkeypatch):
-    async_function = Wrapper(lambda _: None, repr="<AsyncFunctionEmpty>", name="")
-    monkeypatch.setattr(
-        loguru._logger,
-        "iscoroutinefunction",
-        lambda x: x is async_function or iscoroutinefunction(x),
-    )
+def test_coroutine_function_with_empty_name():
+    class CoroutineFunction:
+        __name__ = ""
+
+        def __call__(self):
+            pass
+
+        def __repr__(self):
+            return "<AsyncFunctionEmpty>"
 
-    logger.add(async_function)
+    logger.add(CoroutineFunction())
     assert repr(logger) == "<loguru.logger handlers=[(id=0, level=10, sink=<AsyncFunctionEmpty>)]>"
-    assert not async_function.raised
 
 
 def test_standard_handler():
     handler = logging.StreamHandler(sys.__stderr__)
     logger.add(handler)
     if sys.version_info >= (3, 6):
         r = "<loguru.logger handlers=[(id=0, level=10, sink=<StreamHandler <stderr> (NOTSET)>)]>"
```

### Comparing `loguru-0.6.0/tests/test_standard_handler.py` & `loguru-0.7.0/tests/test_standard_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     logger.warning("nope")
 
     out, err = capsys.readouterr()
     assert out == ""
     assert err == "INFO test\n"
 
 
-def test_file_handler(tmpdir):
-    file = tmpdir.join("test.log")
+def test_file_handler(tmp_path):
+    file = tmp_path / "test.log"
     logger.add(FileHandler(str(file)), format="{message} {level.name}")
     logger.info("test")
     logger.remove()
     logger.warning("nope")
 
-    assert file.read() == "test INFO\n"
+    assert file.read_text() == "test INFO\n"
 
 
 def test_null_handler(capsys):
     logger.add(NullHandler())
     logger.error("nope")
     logger.remove()
 
@@ -89,24 +89,24 @@
         1 / 0
     except ZeroDivisionError:
         logger.exception("Error")
 
     assert result is True
 
 
-def test_exception_formatting(tmpdir):
-    file = tmpdir.join("test.log")
+def test_exception_formatting(tmp_path):
+    file = tmp_path / "test.log"
     logger.add(FileHandler(str(file)), format="{message}")
 
     try:
         1 / 0
     except ZeroDivisionError:
         logger.exception("Error")
 
-    result = file.read()
+    result = file.read_text()
     lines = result.strip().splitlines()
 
     error = "ZeroDivisionError: division by zero"
 
     assert lines[1].startswith("Traceback")
     assert lines[-1] == error
     assert result.count(error) == 1
```

### Comparing `loguru-0.6.0/tests/test_threading.py` & `loguru-0.7.0/tests/test_threading.py`

 * *Files identical despite different names*

