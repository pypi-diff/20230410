# Comparing `tmp/muffin_babel-1.3.6.tar.gz` & `tmp/muffin_babel-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_babel-1.3.6.tar", max compression
+gzip compressed data, was "muffin_babel-1.4.0.tar", max compression
```

## Comparing `muffin_babel-1.3.6.tar` & `muffin_babel-1.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4396 2023-04-06 16:47:52.482546 muffin_babel-1.3.6/README.rst
--rw-r--r--   0        0        0     9094 2023-04-06 16:47:52.482546 muffin_babel-1.3.6/muffin_babel/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 16:47:52.482546 muffin_babel-1.3.6/muffin_babel/py.typed
--rw-r--r--   0        0        0     2030 2023-04-06 16:47:52.482546 muffin_babel-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 muffin_babel-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4396 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/README.rst
+-rw-r--r--   0        0        0    10134 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/muffin_babel/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/muffin_babel/py.typed
+-rw-r--r--   0        0        0     2030 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 muffin_babel-1.4.0/PKG-INFO
```

### Comparing `muffin_babel-1.3.6/README.rst` & `muffin_babel-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_babel-1.3.6/muffin_babel/__init__.py` & `muffin_babel-1.4.0/muffin_babel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Muffin-Babel -- I18n engine for Muffin framework."""
+import csv
 import logging
+import sys
 from contextlib import contextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, Optional, Tuple, TypeVar
 
 from asgi_babel import current_locale, select_locale_by_request
 from babel import Locale, support
 from babel.messages.catalog import Catalog
@@ -129,28 +131,54 @@
 
                     mo_file = po_file.with_suffix(".mo")
 
                     with mo_file.open("wb") as mo:
                         logger.info("writing MO template file to %s", mo_file)
                         write_mo(mo, catalog, use_fuzzy=use_fuzzy)
 
+        @app.manage(lifespan=False)
+        def babel_export_csv(
+            *, domain: str = self.cfg.domain, locale: str = self.cfg.default_locale
+        ):
+            """Export messages from a PO files as CSV."""
+            writer = csv.writer(sys.stdout)
+            writer.writerow(["id", "string", "context", "comment"])
+            for locales_dir in self.cfg.locale_folders:
+                po_file = Path(locales_dir) / locale / "LC_MESSAGES" / f"{domain}.po"
+                if not po_file.exists():
+                    continue
+
+                with po_file.open("rb") as po:
+                    catalog = read_po(po, locale)
+
+                for message in catalog:
+                    writer.writerow(
+                        [
+                            message.id,
+                            message.string,
+                            message.context,
+                            "\n".join(message.auto_comments),
+                        ]
+                    )
+
     async def __middleware__(
         self, handler: Callable, request: Request, receive: "TASGIReceive", send: "TASGISend"
     ) -> Any:
         """Auto detect a locale by the given request."""
         lang = await self.__locale_selector(request)
         self.current_locale = lang or self.cfg.default_locale  # type: ignore[assignment]
         return await handler(request, receive, send)
 
     async def startup(self):
         """Tune Jinja2 if the plugin is installed."""
         if self.cfg.configure_jinja2 and "jinja2" in self.app.plugins:
             jinja2 = self.app.plugins["jinja2"]
-            jinja2.env.add_extension("jinja2.ext.i18n")
-            jinja2.env.install_gettext_callables(
+            env = jinja2.env  # type: ignore[]
+            env.add_extension("jinja2.ext.i18n")
+            env.install_gettext_callables(
                 lambda x: self.get_translations().ugettext(x),
                 lambda s, p, n: self.get_translations().ungettext(s, p, n),
                 newstyle=True,
             )
 
     def locale_selector(self, fn: TVLocaleSelector) -> TVLocaleSelector:
         """Update self locale selector."""
```

### Comparing `muffin_babel-1.3.6/pyproject.toml` & `muffin_babel-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-babel"
-version = "1.3.6"
+version = "1.4.0"
 description = "Localization support for the Muffin Framework"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["localization", "internationalization", "muffin", "babel", "asyncio", "trio", "asgi"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin_babel-1.3.6/PKG-INFO` & `muffin_babel-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-babel
-Version: 1.3.6
+Version: 1.4.0
 Summary: Localization support for the Muffin Framework
 Home-page: https://github.com/klen/muffin-babel
 License: MIT
 Keywords: localization,internationalization,muffin,babel,asyncio,trio,asgi
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

