# Comparing `tmp/pymmcore_plus-0.6.6.tar.gz` & `tmp/pymmcore_plus-0.6.7.tar.gz`

## Comparing `pymmcore_plus-0.6.6.tar` & `pymmcore_plus-0.6.7.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/codecov.yml
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/mkdocs.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/.github/dependabot.yml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/_hooks.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/contributing.md
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/index.md
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/install.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/cmmcoreplus.md
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/configuration.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/constants.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/device.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/events.md
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/mda.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/metadata.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/api/utils.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/examples/context-set.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/examples/following_changes_in_core.md
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/examples/integration-with-qt.md
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/examples/mda.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/examples/napari-micromanager.md
--rw-r--r--   0        0        0    79333 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/images/components.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/images/favicon.ico
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/basic_client.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/napari.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/properties_and_state_events.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/qt_integration.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/run_mda.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/examples/set_as_context.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/__init__.py
--rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/_cli.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/_logger.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/_version.py
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/install.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/py.typed
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/__init__.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_config.py
--rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_config_group.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_constants.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_device.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_metadata.py
--rw-r--r--   0        0        0    65537 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_mmcore_plus.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/_property.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_device_signal_view.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_norm_slot.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_prop_event_mixin.py
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_protocol.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_psygnal.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_qsignals.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_engine.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_protocol.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_runner.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/_protocol.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/_psygnal.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/_qsignals.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/__init__.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/_serialize.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/_util.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/__init__.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/_client.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/callbacks/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/callbacks/basic.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/callbacks/qcallback.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/__main__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/_pyrocore.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/_server.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/conftest.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/local_config.cfg
--rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_cli.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_config_group_class.py
--rw-r--r--   0        0        0    15154 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_core.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_device_class.py
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_events.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_mda.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/test_property_class.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/remote/test_client.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/remote/test_serialize.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/tests/remote/test_server.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/LICENSE
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/README.md
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/codecov.yml
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/mkdocs.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/_hooks.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/contributing.md
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/index.md
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/install.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/cmmcoreplus.md
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/configuration.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/constants.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/device.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/events.md
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/mda.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/metadata.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/api/utils.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/examples/context-set.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/examples/following_changes_in_core.md
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/examples/integration-with-qt.md
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/examples/mda.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/examples/napari-micromanager.md
+-rw-r--r--   0        0        0    79333 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/images/components.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/basic_client.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/napari.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/properties_and_state_events.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/qt_integration.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/run_mda.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/examples/set_as_context.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/__init__.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/_cli.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/_logger.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/_version.py
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/install.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/py.typed
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/__init__.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_config.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_config_group.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_constants.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_device.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_metadata.py
+-rw-r--r--   0        0        0    65616 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_mmcore_plus.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/_property.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/__init__.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_device_signal_view.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_norm_slot.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_prop_event_mixin.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_protocol.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_psygnal.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_qsignals.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_engine.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_protocol.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_runner.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/_protocol.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/_psygnal.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/_qsignals.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/__init__.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/_serialize.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/_util.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/__init__.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/_client.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/callbacks/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/callbacks/basic.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/callbacks/qcallback.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/__main__.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/_pyrocore.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/_server.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/conftest.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/local_config.cfg
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_cli.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_config_group_class.py
+-rw-r--r--   0        0        0    15260 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_core.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_device_class.py
+-rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_events.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_mda.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/test_property_class.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/remote/test_client.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/remote/test_serialize.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/tests/remote/test_server.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/LICENSE
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/README.md
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 pymmcore_plus-0.6.7/PKG-INFO
```

### Comparing `pymmcore_plus-0.6.6/.pre-commit-config.yaml` & `pymmcore_plus-0.6.7/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.220
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pymmcore
           - useq-schema
           - psygnal
           - typer
```

### Comparing `pymmcore_plus-0.6.6/mkdocs.yml` & `pymmcore_plus-0.6.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/setup.py` & `pymmcore_plus-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/.github/workflows/test_and_deploy.yml` & `pymmcore_plus-0.6.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/_hooks.py` & `pymmcore_plus-0.6.7/docs/_hooks.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/contributing.md` & `pymmcore_plus-0.6.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/index.md` & `pymmcore_plus-0.6.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/install.md` & `pymmcore_plus-0.6.7/docs/install.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/api/cmmcoreplus.md` & `pymmcore_plus-0.6.7/docs/api/cmmcoreplus.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/api/configuration.md` & `pymmcore_plus-0.6.7/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/api/constants.md` & `pymmcore_plus-0.6.7/docs/api/constants.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/api/device.md` & `pymmcore_plus-0.6.7/docs/api/device.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/examples/context-set.md` & `pymmcore_plus-0.6.7/docs/examples/context-set.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/examples/following_changes_in_core.md` & `pymmcore_plus-0.6.7/docs/examples/following_changes_in_core.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/examples/integration-with-qt.md` & `pymmcore_plus-0.6.7/docs/examples/integration-with-qt.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/examples/mda.md` & `pymmcore_plus-0.6.7/docs/examples/mda.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/examples/napari-micromanager.md` & `pymmcore_plus-0.6.7/docs/examples/napari-micromanager.md`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/images/components.png` & `pymmcore_plus-0.6.7/docs/images/components.png`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/images/favicon.ico` & `pymmcore_plus-0.6.7/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/docs/stylesheets/extra.css` & `pymmcore_plus-0.6.7/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/examples/properties_and_state_events.py` & `pymmcore_plus-0.6.7/examples/properties_and_state_events.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/examples/qt_integration.py` & `pymmcore_plus-0.6.7/examples/qt_integration.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/examples/run_mda.py` & `pymmcore_plus-0.6.7/examples/run_mda.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     z_plan={"range": 4, "step": 0.5},
     axis_order="tpcz",
 )
 
 mmc = CMMCorePlus.instance()  # (2)!
 mmc.loadSystemConfiguration()  #  load demo configuration (3)
 
+
 # connect callback using a decorator (4)
 @mmc.mda.events.frameReady.connect
 def new_frame(img: np.ndarray, event: MDAEvent):
     print(img.shape)
 
 
 # or connect callback using a function
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/__init__.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "RemoteMMCore",
     "server",
     "__version__",
 ]
 
 
 def __dir__() -> List[str]:
-    return list(globals()) + ["RemoteMMCore", "server"]
+    return [*list(globals()), "RemoteMMCore", "server"]
 
 
 def __getattr__(name: str) -> Any:
     if name in {"RemoteMMCore", "server"}:
         try:
             from . import remote
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/_cli.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/_cli.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/_logger.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/_logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import atexit
+import contextlib
 import os
 import sys
 from typing import TYPE_CHECKING
 
 __all__ = ["logger"]
 
 if TYPE_CHECKING:
     from loguru import logger
 else:
+    from loguru import __version__
     from loguru._logger import Core, Logger
 
+    PATCHERS = {"patchers": []}
+    with contextlib.suppress(Exception):
+        if tuple(int(x) for x in __version__.split("."))[:2] < (0, 7):
+            PATCHERS = {"patcher": None}
+
     # avoid using the global loguru logger in case other packages are using it.
     logger = Logger(
         core=Core(),
         exception=None,
         depth=0,
         record=False,
         lazy=False,
         colors=False,
         raw=False,
         capture=True,
-        patcher=None,
         extra={},
+        **PATCHERS,
     )
 
 DEBUG = os.getenv("MM_DEBUG", "0") in ("1", "true", "True", "yes")
 DEFAULT_LOG_LEVEL = "DEBUG" if DEBUG else "INFO"
 
 
 def set_log_level(level: str = DEFAULT_LOG_LEVEL) -> None:
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/_util.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/_util.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/install.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/install.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/__init__.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_config.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_config.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_config_group.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         but it is not guaranteed.  Use `is_consistent` to check if all presets in this
         ConfigGroup have the same properties.
         """
         presets = self._mmc.getAvailableConfigs(self._name)
         if not presets:
             return  # pragma: no cover
 
-        for (dev, prop, _) in self._mmc.getConfigData(self._name, presets[0]):
+        for dev, prop, _ in self._mmc.getConfigData(self._name, presets[0]):
             yield DeviceProperty(dev, prop, self._mmc)
 
     @property
     def is_consistent(self) -> bool:
         """Return `True` if all presets in this group have the same properties.
 
         Note that a group with 0 or 1 presets is always considered consistent.  If two
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_constants.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_constants.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_device.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         except RuntimeError as e:
             msg = str(e)
             if self.isLoaded():
                 if adapter_name == self.library() and device_name == self.name():
                     msg += f". Device {self.label!r} appears to be loaded already."
                     import warnings
 
-                    warnings.warn(msg)
+                    warnings.warn(msg, stacklevel=2)
                     return
                 lib = self._mmc.getDeviceLibrary(self.label)
                 name = self._mmc.getDeviceName(self.label)
                 msg += f". Device {self.label!r} is already taken by {lib}::{name}"
             else:
                 adapters = self._mmc.getDeviceAdapterNames()
                 if adapter_name not in adapters:
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_metadata.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_metadata.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_mmcore_plus.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_mmcore_plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from threading import RLock, Thread
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Iterator,
+    Literal,
     Pattern,
     Sequence,
     TypeVar,
     cast,
     overload,
 )
 
 import pymmcore
 from psygnal import SignalInstance
-from typing_extensions import Literal
 
 from pymmcore_plus.core.events import PCoreSignaler
 
 from .._logger import logger
 from .._util import find_micromanager
 from ..mda import MDAEngine, MDARunner, PMDAEngine
 from ._config import Configuration
@@ -1271,15 +1271,15 @@
         -------
         np.ndarray
             output image (possibly new shape and dtype)
         """
         if ncomponents is None:
             ncomponents = self.getNumberOfComponents()
         if ncomponents == 4:
-            new_shape = img.shape + (4,)
+            new_shape = (*img.shape, 4)
             img = img.view(dtype=f"u{img.dtype.itemsize//4}")
             img = img.reshape(new_shape)[:, :, (2, 1, 0, 3)]  # mmcore gives bgra
         return img
 
     def snap(self, numChannel: int | None = None, *, fix: bool = True) -> np.ndarray:
         """Snap and return an image.
 
@@ -1446,15 +1446,15 @@
     ) -> None:
         """Delete `configName` from `groupName`.
 
         **Why Override?** To emit a `configDeleted` event.
         """
         args: tuple[str, ...] = (groupName, configName)
         if deviceLabel is not None and propName is not None:
-            args = args + (deviceLabel, propName)
+            args = (*args, deviceLabel, propName)
         super().deleteConfig(*args)
         self.events.configDeleted.emit(groupName, configName)
 
     def deleteConfigGroup(self, group: str) -> None:
         """Deletes an entire configuration `group`.
 
         **Why Override?** To emit a `configGroupDeleted` event.
@@ -1553,15 +1553,15 @@
     def setROI(self, *args: Any, **kwargs: Any) -> None:
         """Set the camera Region of Interest (ROI).
 
         **Why Override?** To emit a `roiSet` event.
         """
         super().setROI(*args, **kwargs)
         if len(args) == 4:
-            args = (super().getCameraDevice(),) + args
+            args = (super().getCameraDevice(), *args)
         self.events.roiSet.emit(*args)
 
     def setChannelGroup(self, channelGroup: str) -> None:
         """Specifies the group determining the channel selection.
 
         ...and send a channelGroupChanged signal.
         """
@@ -1618,15 +1618,18 @@
         ):
             if attr not in exclude:
                 if attr == "Datetime":
                     state[attr] = str(datetime.now())
                 elif attr == "PixelSizeUm":
                     state[attr] = self.getPixelSizeUm(True)  # True==cached
                 else:
-                    state[attr] = getattr(self, f"get{attr}")()
+                    try:
+                        state[attr] = getattr(self, f"get{attr}")()
+                    except RuntimeError:
+                        continue
         return cast("StateDict", state)
 
     @contextmanager
     def _property_change_emission_ensured(
         self, device: str, properties: Sequence[str]
     ) -> Iterator[None]:
         """Context that emits events if any of `properties` change on device.
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/_property.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     >>> prop.range()
     >>> prop.dict()  # all the info in one dict.
     """
 
     def __init__(
         self, device_label: str, property_name: str, mmcore: CMMCorePlus
     ) -> None:
-
         self.device = device_label
         self.name = property_name
         self._mmc = mmcore
 
     @cached_property
     def valueChanged(self) -> _DevicePropValueSignal:
         return _DevicePropValueSignal(self.device, self.name, self._mmc)
@@ -97,15 +96,17 @@
         return self._mmc.getPropertyFromCache(self.device, self.name)
 
     def setValue(self, val: Any) -> None:
         """Functional alternate to property setter."""
         if self.isReadOnly():
             import warnings
 
-            warnings.warn(f"'{self.device}::{self.name}' is a read-only property.")
+            warnings.warn(
+                f"'{self.device}::{self.name}' is a read-only property.", stacklevel=2
+            )
         try:
             self._mmc.setProperty(self.device, self.name, val)
         except RuntimeError as e:
             msg = str(e)
             if allowed := self.allowedValues():
                 msg += f". Allowed values: {allowed}"
             raise RuntimeError(msg) from None
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/__init__.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         return QCoreSignaler
 
     return default
 
 
 def __dir__() -> List[str]:
-    return list(globals()) + ["QCoreSignaler"]
+    return [*list(globals()), "QCoreSignaler"]
 
 
 def __getattr__(name: str) -> Any:
     if name == "QCoreSignaler":
         try:
             from ._qsignals import QCoreSignaler
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_device_signal_view.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_device_signal_view.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_norm_slot.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_norm_slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     NormedCallback = Union[MethodRef, Callable]
     StoredSlot = Tuple[NormedCallback, int | None]
     ReducerFunc = Callable[[tuple, tuple], tuple]
 
 
 def normalize_slot(slot: Callable | NormedCallback) -> NormedCallback:
     if isinstance(slot, MethodType):
-        return _get_method_name(slot) + (None,)
+        return (*_get_method_name(slot), None)
     if _is_partial_method(slot):
         return _partial_weakref(slot)
     if isinstance(slot, tuple) and not isinstance(slot[0], weakref.ref):
         return (weakref.ref(slot[0]), slot[1], slot[2])
     return slot
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_prop_event_mixin.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_prop_event_mixin.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_protocol.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_psygnal.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_psygnal.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/core/events/_qsignals.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/core/events/_qsignals.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ._prop_event_mixin import _PropertySignal
 
 if TYPE_CHECKING:
     from ._prop_event_mixin import PropKeyDict
 
 
 class QCoreSignaler(QObject):
-
     # native MMCore callback events
     propertiesChanged = Signal()
     propertyChanged = Signal(str, str, object)
     channelGroupChanged = Signal(str)
     configGroupChanged = Signal(str, str)
     configSet = Signal(str, str)
     systemConfigurationLoaded = Signal()
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_engine.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_engine.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_protocol.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/mda/_runner.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/mda/_runner.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/__init__.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         return QMDASignaler
 
     return default
 
 
 def __dir__() -> list[str]:
-    return list(globals()) + ["QMDASignaler"]
+    return [*list(globals()), "QMDASignaler"]
 
 
 def __getattr__(name: str) -> object:
     if name == "QMDASignaler":
         try:
             from ._qsignals import QMDASignaler
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/mda/events/_protocol.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/mda/events/_protocol.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/_serialize.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/_serialize.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/_util.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/_util.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/_client.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import atexit
 import contextlib
 import subprocess
 import sys
 import threading
 import time
-from typing import Optional
+from typing import Optional, Protocol
 
 from Pyro5 import api, core, errors
-from typing_extensions import Protocol
 
 from ..._logger import logger
 from .. import server
 from .._serialize import register_serializers
 
 
 class CallbackProtocol(Protocol):
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/client/callbacks/qcallback.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/client/callbacks/qcallback.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/_pyrocore.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/_pyrocore.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     @oneway
     def run_mda(self, sequence) -> Thread:  # pragma: no cover
         return super().run_mda(sequence)
 
     @oneway
     def emit_signal(self, signal_name: str, *args):
-
         logger.debug("{}: {}", signal_name, args)
         for handler in list(self._callback_handlers):
             try:
                 handler._pyroClaimOwnership()  # type: ignore
                 handler.receive_core_callback(signal_name, args)
             except errors.CommunicationError:  # pragma: no cover
                 self.disconnect_remote_callback(handler)
```

### Comparing `pymmcore_plus-0.6.6/src/pymmcore_plus/remote/server/_server.py` & `pymmcore_plus-0.6.7/src/pymmcore_plus/remote/server/_server.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/conftest.py` & `pymmcore_plus-0.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/local_config.cfg` & `pymmcore_plus-0.6.7/tests/local_config.cfg`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/test_cli.py` & `pymmcore_plus-0.6.7/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     {"z_plan": {"step": 0.24}},
     {"z_plan": {"step": 0.24, "range": 4}, "time_plan": {"interval": 0.2, "loops": 20}},
     {"time_plan": {"interval": 0.2}},
     {"axis_order": "TPCZ", "time_plan": {"interval": 0.2, "loops": 20}},
 ]
 
 
+@pytest.mark.filterwarnings("ignore:.*got unknown keyword arguments:UserWarning:useq")
 @pytest.mark.parametrize("args", ARGS)
 @pytest.mark.parametrize("with_file", (True, False))
 def test_run_mda(tmp_path: Path, with_file: bool, args: dict[str, dict | str]) -> None:
     """Just runs a simple MDA."""
 
     cmd: list[str] = ["run"]
     for k, v in args.items():
```

### Comparing `pymmcore_plus-0.6.6/tests/test_config_group_class.py` & `pymmcore_plus-0.6.7/tests/test_config_group_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/test_core.py` & `pymmcore_plus-0.6.7/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         "Shutter",
         "Autofocus",
         "Core",
     )
 
 
 def test_cb_exceptions(core: CMMCorePlus, caplog, qtbot: "QtBot"):
+    if not isinstance(core.events, QObject):
+        pytest.skip(reason="Skip cb exceptions on psygnal.")
+
     @core.events.propertyChanged.connect
     def _raze():
         raise ValueError("Boom")
 
     # using this to avoid our setProperty override... which would immediately
     # raise the exception (we want it to be raised deeper)
     if isinstance(core.events, CMMCoreSignaler):
@@ -378,15 +381,14 @@
     core.objective_device_pattern = re.compile("Objective")
     devices = core.guessObjectiveDevices()
     assert len(devices) == 1
     assert devices[0] == "Objective"
 
 
 def test_guess_channel_group(core: CMMCorePlus):
-
     chan_group = core.getChannelGroup()
     assert chan_group == "Channel"
 
     assert core.getOrGuessChannelGroup() == ["Channel"]
 
     with patch.object(core, "getChannelGroup", return_value=""):
         assert core.getOrGuessChannelGroup() == ["Channel", "Channel-Multiband"]
```

### Comparing `pymmcore_plus-0.6.6/tests/test_device_class.py` & `pymmcore_plus-0.6.7/tests/test_device_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/test_events.py` & `pymmcore_plus-0.6.7/tests/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     core.events.devicePropertyChanged("Camera").disconnect(mock2)
     core.setProperty("Camera", "Gain", "5")
     mock1.assert_not_called()
     mock2.assert_not_called()
 
 
 def test_sequence_acquisition_events(core: CMMCorePlus):
-
     mock1 = Mock()
     mock2 = Mock()
     mock3 = Mock()
 
     core.events.continuousSequenceAcquisitionStarted.connect(mock1)
     core.events.sequenceAcquisitionStopped.connect(mock2)
     core.events.sequenceAcquisitionStarted.connect(mock3)
```

### Comparing `pymmcore_plus-0.6.6/tests/test_mda.py` & `pymmcore_plus-0.6.7/tests/test_mda.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/test_property_class.py` & `pymmcore_plus-0.6.7/tests/test_property_class.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/remote/test_client.py` & `pymmcore_plus-0.6.7/tests/remote/test_client.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/remote/test_serialize.py` & `pymmcore_plus-0.6.7/tests/remote/test_serialize.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/tests/remote/test_server.py` & `pymmcore_plus-0.6.7/tests/remote/test_server.py`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/.gitignore` & `pymmcore_plus-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/LICENSE` & `pymmcore_plus-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymmcore_plus-0.6.6/README.md` & `pymmcore_plus-0.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 core = CMMCorePlus()
 ...
 ```
 
 ### Examples
 
 See a number of [usage examples in the
-documentation](http://127.0.0.1:8000/pymmcore-plus/examples/mda/).
+documentation](http://pymmcore-plus.github.io/pymmcore-plus/examples/mda/).
 
 You can find some basic python scripts in the [examples](examples) directory of
 this repository
 
 ## Contributing
 
-Contributions are welcome!  See [contributing guide](http://127.0.0.1:8000/pymmcore-plus/contributing/).
+Contributions are welcome!  See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
```

### Comparing `pymmcore_plus-0.6.6/pyproject.toml` & `pymmcore_plus-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     "D100", # Missing docstring in public module
     "D104", # Missing docstring in public package
     "D107", # Missing docstring in __init__
     "D203", # 1 blank line required before class docstring
     "D212", # Multi-line docstring summary should start at the first line
     "D213", # Multi-line docstring summary should start at the second line
     "D400", # First line should end with a period
+    "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
     "C901", # Function is too complex
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D"]
```

### Comparing `pymmcore_plus-0.6.6/PKG-INFO` & `pymmcore_plus-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmcore-plus
-Version: 0.6.6
+Version: 0.6.7
 Summary: pymmcore superset providing improved APIs, event connection, and a pure python acquisition engine
 Project-URL: Source, https://github.com/pymmcore-plus/pymmcore-plus
 Project-URL: Tracker, https://github.com/pymmcore-plus/pymmcore-plus/issues
 Project-URL: Documentation, https://pymmcore-plus.github.io/pymmcore-plus
 Author: Ian Hunt-Isaak
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
@@ -175,15 +175,15 @@
 core = CMMCorePlus()
 ...
 ```
 
 ### Examples
 
 See a number of [usage examples in the
-documentation](http://127.0.0.1:8000/pymmcore-plus/examples/mda/).
+documentation](http://pymmcore-plus.github.io/pymmcore-plus/examples/mda/).
 
 You can find some basic python scripts in the [examples](examples) directory of
 this repository
 
 ## Contributing
 
-Contributions are welcome!  See [contributing guide](http://127.0.0.1:8000/pymmcore-plus/contributing/).
+Contributions are welcome!  See [contributing guide](http://pymmcore-plus.github.io/pymmcore-plus/contributing/).
```

