# Comparing `tmp/tansy-0.5.2.tar.gz` & `tmp/tansy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tansy-0.5.2.tar", last modified: Tue Jan  3 04:59:15 2023, max compression
+gzip compressed data, was "tansy-0.6.0.tar", last modified: Mon Apr 10 18:47:48 2023, max compression
```

## Comparing `tansy-0.5.2.tar` & `tansy-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 04:59:15.763511 tansy-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-03 04:59:01.000000 tansy-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-03 04:59:15.763511 tansy-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-03 04:59:01.000000 tansy-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-03 04:59:01.000000 tansy-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 04:59:15.763511 tansy-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-03 04:59:01.000000 tansy-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 04:59:15.763511 tansy-0.5.2/tansy/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/slash_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/slash_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 04:59:15.763511 tansy-0.5.2/tansy/speedup/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/speedup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/speedup/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/speedup/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/speedup/interaction_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/speedup/orjson_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-01-03 04:59:01.000000 tansy-0.5.2/tansy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 04:59:15.763511 tansy-0.5.2/tansy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-03 04:59:15.000000 tansy-0.5.2/tansy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-03 04:59:15.000000 tansy-0.5.2/tansy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 04:59:15.000000 tansy-0.5.2/tansy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-03 04:59:15.000000 tansy-0.5.2/tansy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-03 04:59:15.000000 tansy-0.5.2/tansy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 18:47:29.000000 tansy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 18:47:48.498643 tansy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-10 18:47:29.000000 tansy-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 18:47:29.000000 tansy-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:47:48.498643 tansy-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 18:47:29.000000 tansy-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/tansy/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/class_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/slash_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/slash_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-10 18:47:29.000000 tansy-0.6.0/tansy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:48.498643 tansy-0.6.0/tansy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:47:48.000000 tansy-0.6.0/tansy.egg-info/top_level.txt
```

### Comparing `tansy-0.5.2/LICENSE` & `tansy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tansy-0.5.2/PKG-INFO` & `tansy-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.5.2
-Summary: Unstable experiments with NAFF.
+Version: 0.6.0
+Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
-Author: Astrea49
+Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tansy
 
 [![PyPI](https://img.shields.io/pypi/v/tansy)](https://pypi.org/project/tansy/)
 [![Downloads](https://static.pepy.tech/personalized-badge/tansy?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=pip%20installs)](https://pepy.tech/project/tansy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Unstable experiments with NAFF.
+Unstable experiments with interactions.py.
 
 # Commands
 
 `tansy` provides a unique way to define options for slash commands - a way that appears often in other Discord Python libraries.
 
 Instead of needing a decorator per option or to define the option in one huge list, `tansy` allows you to define each option in the function itself.
 By using a special metadata function, you can specify what each argument/parameter in a function should be like as an option, with tansy smartly handling the rest for you.
 
-## Example Command
 ```python
-import naff
+import interactions as ipy
 import tansy
 
 @tansy.slash_command(name="test", description="Nice test command, huh?")
 async def test_cmd(
-    ctx: naff.InteractionCommand,
-    the_user: naff.User = tansy.Option(name="user", description="The user to ping."),
+    ctx: ipy.InteractionContext,
+    the_user: ipy.User = tansy.Option(name="user", description="The user to ping."),
 ):
     await ctx.send(the_user.mention)
 ```
 
-# Speedups
+## Class Slash Command
 
-`tansy` also includes several patches that can speed up NAFF itself, sometimes by a signficant margin.
-However, these patches are unstable, and may break some (usually niche) parts of the things they modify.
+In case you want to try something very unique, or just want to leverage classes, `tansy` allows you to leverage its toolset to make class slash commands.
 
-To install them, use:
 ```python
+import interactions as ipy
 import tansy
 
-# this should be the first line of code you run in your main file if you want
-# everything to work correctly
-tansy.install_naff_speedups()
+@tansy.class_slash_command(name="test", description="Nice test command, huh?")
+class Test:
+    the_user: ipy.User = tansy.Option(name="user", description="The user to ping.")
+
+    async def callback(self, ctx: ipy.InteractionContext):
+        await ctx.send(self.the_user.mention)
 ```
 
-You can also toggle on or off what patches you want - take a look at the function's docstring for details.
+Note that the class is being read and adjusted to be more like a typical functional declaration, and so isn't a fully true class-based approach.
+Subclasses are not going to become subcommands (though `class_subcommand` exists), and while the class *does* get initialized on every run
+(meaning you can use custom `__init__`s, as long as they have no parameters that need to be filled in), the class is largely untouched outside
+of declaration and using `callback`.
```

### Comparing `tansy-0.5.2/setup.py` & `tansy-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 requirements = []
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="tansy",
-    description="Unstable experiments with NAFF.",
+    description="Unstable experiments with interactions.py.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
-    author="Astrea49",
+    author="AstreaTSS",
     url="https://github.com/Astrea49/tansy",
-    version="0.5.2",
+    version="0.6.0",
     packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tansy-0.5.2/tansy/slash_commands.py` & `tansy-0.6.0/tansy/slash_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 import asyncio
 import copy
 import functools
 import inspect
 import typing
+from builtins import getattr
 
 import attrs
-import naff
+import interactions as ipy
 
 from . import slash_param
 from . import utils
 
+__all__ = (
+    "TansySlashCommandParameter",
+    "TansySlashCommand",
+    "tansy_slash_command",
+    "tansy_subcommand",
+    "SlashCommand",
+    "slash_command",
+    "subcommand",
+)
+
 
 def _get_converter(anno: type, name: str):
     if typing.get_origin(anno) == typing.Annotated:
         anno = utils.get_from_anno_type(anno)
 
-    if isinstance(anno, naff.Converter):
-        return naff.BaseCommand._get_converter_function(anno, name)
+    if isinstance(anno, ipy.Converter):
+        return ipy.BaseCommand._get_converter_function(anno, name)
     elif inspect.isroutine(anno):
         if hasattr(anno, "__code__"):
             num_params: int = anno.__code__.co_argcount
         else:
             num_params = len(inspect.signature(anno).parameters.values())
 
         match num_params:
             case 2:
                 return anno
             case 1:
 
                 async def _one_arg_convert(_, arg) -> typing.Any:
-                    return await naff.utils.maybe_coroutine(anno, arg)
+                    return await ipy.utils.maybe_coroutine(anno, arg)
 
                 return _one_arg_convert
             case 0:
                 raise ValueError(
-                    f"{naff.utils.get_object_name(anno)} for {name} has 0"
+                    f"{ipy.utils.get_object_name(anno)} for {name} has 0"
                     " positional arguments, which is unsupported."
                 )
             case _:
                 raise ValueError(
-                    f"{naff.utils.get_object_name(anno)} for {name} has more than 2"
+                    f"{ipy.utils.get_object_name(anno)} for {name} has more than 2"
                     " positional arguments, which is unsupported."
                 )
     else:
         return None
 
 
 _C = typing.TypeVar("_C", bound=typing.Callable)
@@ -118,100 +129,80 @@
 
 @attrs.define(slots=True)
 class TansySlashCommandParameter:
     """An object representing parameters in a command."""
 
     name: str = attrs.field(default=None)
     argument_name: str = attrs.field(default=None)
-    default: typing.Any = attrs.field(default=naff.MISSING)
+    default: typing.Any = attrs.field(default=ipy.MISSING)
     type: typing.Type = attrs.field(default=None)
     converter: typing.Optional[typing.Callable] = attrs.field(default=None)
 
     @property
     def optional(self) -> bool:
-        return self.default != naff.MISSING
+        return self.default != ipy.MISSING
 
 
-@naff.utils.define()
-class TansySlashCommand(naff.SlashCommand):
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class TansySlashCommand(ipy.SlashCommand):
     parameters: dict[str, TansySlashCommandParameter] = attrs.field(
-        factory=dict, metadata=naff.utils.no_export_meta
+        factory=dict, metadata=ipy.utils.no_export_meta
     )
     _inspect_signature: typing.Optional[inspect.Signature] = attrs.field(
-        repr=False, default=None, metadata=naff.utils.no_export_meta
+        repr=False, default=None, metadata=ipy.utils.no_export_meta
     )
 
-    def __attrs_post_init__(self) -> None:
-        if self.callback is not None:
-            if not self._inspect_signature:
-                # qualname hack, oh how i've not missed you
-                # in case you forgot - qualname contains the full name of a function,
-                # including the class it's in
-                # it just so happens that functions in a class with be like Class.func,
-                # and functions outside of one will be like func
-                # simply put, checking if there's a dot in the qualname basically
-                # also checks if it's in a class (or module, but shh) -
-                # if it's in a class, we're assuming there's a self in there (not always
-                # true, but naff relies on that assumption anyways),
-                # which we want to ignore
-                # we also want to ignore ctx too
-                if "." in self.callback.__qualname__:
-                    callback = functools.partial(self.callback, None, None)
-                else:
-                    callback = functools.partial(self.callback, None)
-
-                self._inspect_signature = inspect.signature(callback)
-
-            # in an ideal world, we wouldn't parse until right as the command is being
-            # added, but tansy doesn't have that much control over naff to hook onto
-            # that
-            self._parse_paramters()
-
-            if self.parameters:
-                # i wont lie to you - what we're about to do is probably the
-                # most disgusting, hacky thing ive done in python, but there's a good
-                # reason for it
-                #
-                # you know how Option() exists in this lib? you know how you have to
-                # do arg: type = Option() in order to define an option usually when
-                # using tansy commands?
-                # well, now Option() is the default of arg in the command, which
-                # means if no value is provided for arg while using the raw callback,
-                # instead of erroring out or receiving the value specified in default=X
-                # (or None, if you used Optional and didn't explictly set a default value),
-                # the function will instead just pass in the ParamInfo generated by Option(),
-                # which is unintuitive and would result in a lot of bugs
-                #
-                # to prevent this, we overwrite the defaults in the function with ones
-                # that make more sense considering tansy's features
-                # explainations about the cursed _overwrite_defaults can be found
-                # in the function itself
-
-                defaults = {
-                    p.argument_name: p.default
-                    for p in self.parameters.values()
-                    if p.optional
-                }
-                self.callback = _overwrite_defaults(
-                    self.callback, defaults, self._inspect_signature.parameters
-                )
-
-            # since we're overriding __attrs_post_init__, we need to make sure
-            # we do this
-            if hasattr(self.callback, "auto_defer"):
-                self.auto_defer = self.callback.auto_defer
+    def _overwrite_with_parameters(self):
+        # i wont lie to you - what we're about to do is probably the
+        # most disgusting, hacky thing ive done in python, but there's a good
+        # reason for it
+        #
+        # you know how Option() exists in this lib? you know how you have to
+        # do arg: type = Option() in order to define an option usually when
+        # using tansy commands?
+        # well, now Option() is the default of arg in the command, which
+        # means if no value is provided for arg while using the raw callback,
+        # instead of erroring out or receiving the value specified in default=X
+        # (or None, if you used Optional and didn't explictly set a default value),
+        # the function will instead just pass in the ParamInfo generated by Option(),
+        # which is unintuitive and would result in a lot of bugs
+        #
+        # to prevent this, we overwrite the defaults in the function with ones
+        # that make more sense considering tansy's features
+        # explainations about the cursed _overwrite_defaults can be found
+        # in the function itself
+
+        defaults = {
+            p.argument_name: p.default for p in self.parameters.values() if p.optional
+        }
+        self.callback = _overwrite_defaults(
+            self.callback, defaults, self._inspect_signature.parameters
+        )
 
-        # make sure checks and the like go through
-        naff.BaseCommand.__attrs_post_init__(self)
+    def _parse_parameters(self):
+        if self.callback is None:
+            return
+
+        if self.parameters:
+            self._overwrite_with_parameters()
+            return
 
-    def _parse_paramters(self):
         self.options = []
 
         if not self._inspect_signature:
-            raise ValueError("No signature found for the callback.")
+            if self.has_binding:
+                callback = functools.partial(self.callback, None, None)
+            else:
+                callback = functools.partial(self.callback, None)
+
+            self._inspect_signature = inspect.signature(callback)
+
+        describes: dict[str, ipy.LocalisedDesc] = getattr(
+            self.callback, "__tansy_describe__", {}
+        )
 
         for param in self._inspect_signature.parameters.values():
             if param.kind == param.VAR_KEYWORD:
                 # something like **kwargs, that's fine so let it pass
                 continue
 
             if param.kind not in {
@@ -234,19 +225,22 @@
             else:
                 try:
                     option_type = utils.get_option(param.annotation)
                 except ValueError:
                     raise ValueError(
                         f"Invalid/no provided type for {param.name}"
                     ) from None
-                option = naff.SlashCommandOption(name=param.name, type=option_type)
+                option = ipy.SlashCommandOption(name=param.name, type=option_type)
 
             cmd_param.name = str(option.name) if option.name else param.name
             cmd_param.argument_name = param.name
-            option.name = option.name or naff.LocalisedName.converter(cmd_param.name)
+            option.name = option.name or ipy.LocalisedName.converter(cmd_param.name)
+
+            if desc := describes.get(option.name.default):
+                option.description = desc
 
             if option.type is None:
                 try:
                     option.type = utils.get_option(param.annotation)
                 except ValueError:
                     raise ValueError(
                         f"Invalid/no provided type for {param.name}"
@@ -254,33 +248,33 @@
 
             if param_info:
                 cmd_param.default = param_info.default
             elif param.default is not param.empty:
                 option.required = False
                 cmd_param.default = param.default
             else:
-                cmd_param.default = naff.MISSING
+                cmd_param.default = ipy.MISSING
 
             # what we're checking here is:
             # - if we don't already have a default
             # - if the user didn't already specify a type in
             #   param_info that would indicate if its optional or not
             # - if the annotation is marked as optional
             # if so, we want to make the option not required, and the default be None
             if (
-                cmd_param.default is naff.MISSING
+                cmd_param.default is ipy.MISSING
                 and (not param_info or not param_info._user_provided_type)
                 and utils.is_optional(param.annotation)
             ):
                 option.required = False
                 cmd_param.default = None
 
             if (
                 param_info
-                and option.type == naff.OptionTypes.CHANNEL
+                and option.type == ipy.OptionType.CHANNEL
                 and not option.channel_types
             ):
                 option.channel_types = utils.resolve_channel_types(param.annotation)  # type: ignore
 
             if param_info and param_info.converter:
                 if convert_func := _get_converter(param_info.converter, param.name):
                     cmd_param.converter = convert_func
@@ -298,106 +292,111 @@
             self.options.append(option)
             self.parameters[cmd_param.name] = cmd_param
 
         # make sure the options arent in an invalid order -
         # both to safeguard against invalid slash commands and because
         # we rely on optional arguments being after required arguments right after this
         attrs.validate(self)  # type: ignore
+        self._overwrite_with_parameters()
 
     async def call_callback(
-        self, callback: typing.Callable, ctx: naff.InteractionContext
+        self, callback: typing.Callable, ctx: ipy.InteractionContext
     ) -> None:
         """
         Runs the callback of this command.
         Args:
-            callback (Callable: The callback to run. This is provided for compatibility with naff.
-            ctx (naff.InteractionContext): The context to use for this command.
+            callback (Callable: The callback to run. This is provided for compatibility with ipy.
+            ctx (ipy.InteractionContext): The context to use for this command.
         """
         if not self.parameters:
             return await callback(ctx, **ctx.kwargs)
 
         new_kwargs = {}
 
         for key, value in ctx.kwargs.items():
             param = self.parameters.get(key)
             if not param:
                 # hopefully you have **kwargs
                 new_kwargs[key] = value
                 continue
 
             if param.converter:
-                converted = await naff.utils.maybe_coroutine(
-                    param.converter, ctx, value
-                )
+                converted = await ipy.utils.maybe_coroutine(param.converter, ctx, value)
             else:
                 converted = value
             new_kwargs[param.argument_name] = converted
 
         return await self.call_with_binding(callback, ctx, **new_kwargs)
 
     def group(
-        self, name: str = None, description: str = "No Description Set"
+        self,
+        name: str = None,
+        description: str = "No Description Set",
+        inherit_checks: bool = True,
     ) -> "TansySlashCommand":
         return TansySlashCommand(
             name=self.name,
             description=self.description,
             group_name=name,
             group_description=description,
             scopes=self.scopes,
+            checks=self.checks if inherit_checks else [],
         )
 
     def subcommand(
         self,
-        sub_cmd_name: naff.LocalisedName | str,
-        group_name: naff.LocalisedName | str = None,
-        sub_cmd_description: naff.Absent[naff.LocalisedDesc | str] = naff.MISSING,
-        group_description: naff.Absent[naff.LocalisedDesc | str] = naff.MISSING,
+        sub_cmd_name: ipy.LocalisedName | str,
+        group_name: ipy.LocalisedName | str = None,
+        sub_cmd_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
+        group_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
         nsfw: bool = False,
+        inherit_checks: bool = True,
     ) -> typing.Callable[..., "TansySlashCommand"]:
         def wrapper(
             call: typing.Callable[..., typing.Coroutine]
         ) -> "TansySlashCommand":
             nonlocal sub_cmd_description
 
             if not asyncio.iscoroutinefunction(call):
                 raise TypeError("Subcommand must be coroutine")
 
-            if sub_cmd_description is naff.MISSING:
+            if sub_cmd_description is ipy.MISSING:
                 sub_cmd_description = call.__doc__ or "No Description Set"
 
             return TansySlashCommand(
                 name=self.name,
                 description=self.description,
                 group_name=group_name or self.group_name,
                 group_description=group_description or self.group_description,
                 sub_cmd_name=sub_cmd_name,
                 sub_cmd_description=sub_cmd_description,
                 default_member_permissions=self.default_member_permissions,
                 dm_permission=self.dm_permission,
                 callback=call,
                 scopes=self.scopes,
                 nsfw=nsfw,
+                checks=self.checks if inherit_checks else [],
             )
 
         return wrapper
 
 
 def tansy_slash_command(
-    name: str | naff.LocalisedName,
+    name: str | ipy.LocalisedName,
     *,
-    description: naff.Absent[str | naff.LocalisedDesc] = naff.MISSING,
-    scopes: naff.Absent[typing.List["naff.Snowflake_Type"]] = naff.MISSING,
-    default_member_permissions: typing.Optional["naff.Permissions"] = None,
+    description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
+    scopes: ipy.Absent[typing.List["ipy.Snowflake_Type"]] = ipy.MISSING,
+    default_member_permissions: typing.Optional["ipy.Permissions"] = None,
     dm_permission: bool = True,
-    sub_cmd_name: str | naff.LocalisedName = None,
-    group_name: str | naff.LocalisedName = None,
-    sub_cmd_description: str | naff.LocalisedDesc = "No Description Set",
-    group_description: str | naff.LocalisedDesc = "No Description Set",
+    sub_cmd_name: str | ipy.LocalisedName = None,
+    group_name: str | ipy.LocalisedName = None,
+    sub_cmd_description: str | ipy.LocalisedDesc = "No Description Set",
+    group_description: str | ipy.LocalisedDesc = "No Description Set",
     nsfw: bool = False,
-) -> typing.Callable[[typing.Callable[..., typing.Coroutine]], TansySlashCommand]:
+) -> typing.Callable[[ipy.const.AsyncCallable], TansySlashCommand]:
     """
     A decorator to declare a coroutine as a Tansy slash command.
     note:
         While the base and group descriptions arent visible in the discord client, currently.
         We strongly advise defining them anyway, if you're using subcommands, as Discord has said they will be visible in
         one of the future ui updates.
     Args:
@@ -411,41 +410,103 @@
         group_name: 1-32 character name of the group
         group_description: 1-100 character description of the group
         nsfw: This command should only work in NSFW channels
     Returns:
         TansySlashCommand Object
     """
 
-    def wrapper(func: typing.Callable[..., typing.Coroutine]) -> TansySlashCommand:
+    def wrapper(func: ipy.const.AsyncCallable) -> TansySlashCommand:
         if not inspect.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         perm = default_member_permissions
         if hasattr(func, "default_member_permissions"):
             if perm:
                 perm = perm | func.default_member_permissions
             else:
                 perm = func.default_member_permissions
 
         _description = description
-        if _description is naff.MISSING:
+        if _description is ipy.MISSING:
             _description = func.__doc__ or "No Description Set"
 
         return TansySlashCommand(
             name=name,
             group_name=group_name,
             group_description=group_description,
             sub_cmd_name=sub_cmd_name,
             sub_cmd_description=sub_cmd_description,
             description=_description,
-            scopes=scopes or [naff.const.GLOBAL_SCOPE],
+            scopes=scopes or [ipy.const.GLOBAL_SCOPE],
             default_member_permissions=perm,
             dm_permission=dm_permission,
             nsfw=nsfw,
             callback=func,
         )
 
     return wrapper
 
 
+def tansy_subcommand(
+    base: str | ipy.LocalisedName,
+    *,
+    subcommand_group: typing.Optional[str | ipy.LocalisedName] = None,
+    name: typing.Optional[str | ipy.LocalisedName] = None,
+    description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
+    base_description: typing.Optional[str | ipy.LocalisedDesc] = None,
+    base_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
+    base_default_member_permissions: typing.Optional["ipy.Permissions"] = None,
+    base_dm_permission: bool = True,
+    subcommand_group_description: typing.Optional[str | ipy.LocalisedDesc] = None,
+    sub_group_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
+    scopes: typing.List["ipy.Snowflake_Type"] = None,
+    nsfw: bool = False,
+) -> typing.Callable[[ipy.const.AsyncCallable], TansySlashCommand]:
+    """
+    A decorator specifically tailored for creating Tansy subcommands.
+    Args:
+        base: The name of the base command
+        subcommand_group: The name of the subcommand group, if any.
+        name: The name of the subcommand, defaults to the name of the coroutine.
+        description: The description of the subcommand
+        base_description: The description of the base command
+        base_desc: An alias of `base_description`
+        base_default_member_permissions: What permissions members need to have by default to use this command.
+        base_dm_permission: Should this command be available in DMs.
+        subcommand_group_description: Description of the subcommand group
+        sub_group_desc: An alias for `subcommand_group_description`
+        scopes: The scopes of which this command is available, defaults to GLOBAL_SCOPE
+        nsfw: This command should only work in NSFW channels
+    Returns:
+        A SlashCommand object
+    """
+
+    def wrapper(func: ipy.const.AsyncCallable) -> TansySlashCommand:
+        if not asyncio.iscoroutinefunction(func):
+            raise ValueError("Commands must be coroutines")
+
+        _description = description
+        if _description is ipy.MISSING:
+            _description = func.__doc__ or "No Description Set"
+
+        cmd = TansySlashCommand(
+            name=base,
+            description=(base_description or base_desc) or "No Description Set",
+            group_name=subcommand_group,
+            group_description=(subcommand_group_description or sub_group_desc)
+            or "No Description Set",
+            sub_cmd_name=name,
+            sub_cmd_description=_description,
+            default_member_permissions=base_default_member_permissions,
+            dm_permission=base_dm_permission,
+            scopes=scopes or [ipy.const.GLOBAL_SCOPE],
+            callback=func,
+            nsfw=nsfw,
+        )
+        return cmd
+
+    return wrapper
+
+
 SlashCommand = TansySlashCommand
 slash_command = tansy_slash_command
+subcommand = tansy_subcommand
```

### Comparing `tansy-0.5.2/tansy/slash_param.py` & `tansy-0.6.0/tansy/slash_param.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,92 @@
 import typing
+from builtins import hasattr
 
 import attrs
-import naff
+import interactions as ipy
 
 from . import utils
 
+if typing.TYPE_CHECKING:
+    from .slash_commands import TansySlashCommand
+
+    SlashCommandT = typing.TypeVar(
+        "SlashCommandT", "TansySlashCommand", ipy.const.AsyncCallable
+    )
+
+__all__ = ("ParamInfo", "Option", "Param", "describe")
+
 
 @attrs.define(kw_only=True)
 class ParamInfo:
-    name: naff.LocalisedName | str | None = attrs.field(
-        default=None, converter=naff.LocalisedName.converter
+    name: ipy.LocalisedName | str | None = attrs.field(
+        default=None, converter=ipy.LocalisedName.converter
     )
-    description: naff.LocalisedDesc | str = attrs.field(
-        default="No Description Set", converter=naff.LocalisedDesc.converter
+    description: ipy.LocalisedDesc | str = attrs.field(
+        default="No Description Set", converter=ipy.LocalisedDesc.converter
     )
-    type: "naff.OptionTypes | None" = attrs.field(default=None)
-    converter: typing.Optional[naff.Converter | typing.Callable] = attrs.field(
+    type: "ipy.OptionType | None" = attrs.field(default=None)
+    converter: typing.Optional[ipy.Converter | typing.Callable] = attrs.field(
         default=None,
     )
-    default: typing.Any = attrs.field(default=naff.MISSING)
+    default: typing.Any = attrs.field(default=ipy.MISSING)
     required: bool = attrs.field(default=True)
     autocomplete: bool = attrs.field(default=False)
-    choices: list[naff.SlashCommandChoice | dict] = attrs.field(factory=list)
-    channel_types: list[naff.ChannelTypes | int] | None = attrs.field(default=None)
+    choices: list[ipy.SlashCommandChoice | dict] = attrs.field(factory=list)
+    channel_types: list[ipy.ChannelType | int] | None = attrs.field(default=None)
     min_value: typing.Optional[float] = attrs.field(default=None)
     max_value: typing.Optional[float] = attrs.field(default=None)
     min_length: typing.Optional[int] = attrs.field(repr=False, default=None)
     max_length: typing.Optional[int] = attrs.field(repr=False, default=None)
 
     _user_provided_type: typing.Any = attrs.field(repr=False, default=None)
 
     def __attrs_post_init__(self):
-        if self.default is not naff.MISSING:
+        if self.default is not ipy.MISSING:
             self.required = False
 
         if self.required and utils.is_optional(self._user_provided_type):
             self.required = False
             self.default = None
 
-        if not self.required and self.default is naff.MISSING:
+        if not self.required and self.default is ipy.MISSING:
             raise ValueError(
                 f"{self.name} is not required, but no default has been set!"
             )
 
-        if self.type == naff.OptionTypes.CHANNEL and not self.channel_types:
+        if self.type == ipy.OptionType.CHANNEL and not self.channel_types:
             self.channel_types = utils.resolve_channel_types(self._user_provided_type)  # type: ignore
 
     @channel_types.validator  # type: ignore
     def _channel_types_validator(
-        self, attribute: str, value: typing.Optional[list[naff.OptionTypes]]
+        self, attribute: str, value: typing.Optional[list[ipy.OptionType]]
     ) -> None:
         if value is not None and self.type is not None:
-            if self.type != naff.OptionTypes.CHANNEL:
+            if self.type != ipy.OptionType.CHANNEL:
                 raise ValueError("The option needs to be CHANNEL to use this")
 
-            allowed_int = [channel_type.value for channel_type in naff.ChannelTypes]
+            allowed_int = {channel_type.value for channel_type in ipy.ChannelType}
             for item in value:
-                if (item not in allowed_int) and (item not in naff.ChannelTypes):
+                if (item not in allowed_int) and (item not in ipy.ChannelType):
                     raise ValueError(f"{value} is not allowed here")
 
     @min_value.validator  # type: ignore
     def _min_value_validator(
         self, attribute: str, value: typing.Optional[float]
     ) -> None:
         if value is not None and self.type is not None:
             if self.type not in [
-                naff.OptionTypes.INTEGER,
-                naff.OptionTypes.NUMBER,
+                ipy.OptionType.INTEGER,
+                ipy.OptionType.NUMBER,
             ]:
                 raise ValueError(
                     "`min_value` can only be supplied with int or float options"
                 )
 
-            if self.type == naff.OptionTypes.INTEGER and isinstance(value, float):
+            if self.type == ipy.OptionType.INTEGER and isinstance(value, float):
                 raise ValueError("`min_value` needs to be an int in an int option")
 
             if (
                 self.max_value is not None
                 and self.min_value is not None
                 and self.max_value < self.min_value
             ):
@@ -84,33 +94,33 @@
 
     @max_value.validator  # type: ignore
     def _max_value_validator(
         self, attribute: str, value: typing.Optional[float]
     ) -> None:
         if value is not None and self.type is not None:
             if self.type not in [
-                naff.OptionTypes.INTEGER,
-                naff.OptionTypes.NUMBER,
+                ipy.OptionType.INTEGER,
+                ipy.OptionType.NUMBER,
             ]:
                 raise ValueError(
                     "`max_value` can only be supplied with int or float options"
                 )
 
-            if self.type == naff.OptionTypes.INTEGER and isinstance(value, float):
+            if self.type == ipy.OptionType.INTEGER and isinstance(value, float):
                 raise ValueError("`max_value` needs to be an int in an int option")
 
             if self.max_value and self.min_value and self.max_value < self.min_value:
                 raise ValueError("`min_value` needs to be <= than `max_value`")
 
     @min_length.validator
     def _min_length_validator(
         self, attribute: str, value: typing.Optional[int]
     ) -> None:
         if value is not None and self.type is not None:
-            if self.type != naff.OptionTypes.STRING:
+            if self.type != ipy.OptionType.STRING:
                 raise ValueError(
                     "`min_length` can only be supplied with string options"
                 )
 
             if (
                 self.max_length is not None
                 and self.min_length is not None
@@ -122,32 +132,32 @@
                 raise ValueError("`min_length` needs to be >= 0")
 
     @max_length.validator
     def _max_length_validator(
         self, attribute: str, value: typing.Optional[int]
     ) -> None:
         if value is not None and self.type is not None:
-            if self.type != naff.OptionTypes.STRING:
+            if self.type != ipy.OptionType.STRING:
                 raise ValueError(
                     "`max_length` can only be supplied with string options"
                 )
 
             if (
                 self.min_length is not None
                 and self.max_length is not None
                 and self.max_length < self.min_length
             ):
                 raise ValueError("`min_length` needs to be <= than `max_length`")
 
             if self.max_length < 1:
                 raise ValueError("`max_length` needs to be >= 1")
 
-    def generate_option(self) -> naff.SlashCommandOption:
+    def generate_option(self) -> ipy.SlashCommandOption:
         with attrs.validators.disabled():
-            return naff.SlashCommandOption(
+            return ipy.SlashCommandOption(
                 name=self.name,
                 type=self.type,
                 description=self.description,
                 required=self.required,
                 autocomplete=self.autocomplete,
                 choices=self.choices or [],
                 channel_types=self.channel_types,
@@ -155,24 +165,24 @@
                 max_value=self.max_value,
                 min_length=self.min_length,
                 max_length=self.max_length,
             )
 
 
 def Option(
-    description: naff.LocalisedDesc | str = "No Description Set",
+    description: ipy.LocalisedDesc | str = "No Description Set",
     *,
-    name: naff.LocalisedName | str | None = None,
+    name: ipy.LocalisedName | str | None = None,
     type: typing.Any = None,
-    converter: typing.Optional[naff.Converter | typing.Callable] = None,
-    default: typing.Any = naff.MISSING,
+    converter: typing.Optional[ipy.Converter | typing.Callable] = None,
+    default: typing.Any = ipy.MISSING,
     required: bool = True,
     autocomplete: bool = False,
-    choices: list[naff.SlashCommandChoice | dict] | None = None,
-    channel_types: list[naff.ChannelTypes | int] | None = None,
+    choices: list[ipy.SlashCommandChoice | dict] | None = None,
+    channel_types: list[ipy.ChannelType | int] | None = None,
     min_value: float | None = None,
     max_value: float | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
 ) -> typing.Any:
     return ParamInfo(
         name=name,
@@ -189,7 +199,32 @@
         max_value=max_value,
         min_length=min_length,
         max_length=max_length,
     )
 
 
 Param = Option
+
+
+def describe(
+    name: str, description: ipy.LocalisedDesc | str
+) -> typing.Callable[["SlashCommandT"], "SlashCommandT"]:
+    """
+    A decorator to add a description to a slash command.
+
+    Args:
+        name (str): The name of the description.
+        description (str): The description to add.
+
+    Returns:
+        Either the callback or slash command.
+    """
+
+    def decorator(func: "SlashCommandT") -> "SlashCommandT":
+        if hasattr(func, "callback"):
+            func = func.callback
+        if not hasattr(func, "__tansy_describe__"):
+            func.__tansy_describe__ = {}
+        func.__tansy_describe__[name] = ipy.LocalisedDesc.converter(description)
+        return func
+
+    return decorator
```

### Comparing `tansy-0.5.2/tansy/utils.py` & `tansy-0.6.0/tansy/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,39 @@
+import contextlib
 import itertools
 import types
 import typing
 
-import naff
+import interactions as ipy
 
-REVERSE_CHANNEL_MAPPING = {v: k for k, v in naff.TYPE_CHANNEL_MAPPING.items()}
+__all__ = (
+    "REVERSE_CHANNEL_MAPPING",
+    "UNION_TYPES",
+    "USER_TYPES",
+    "USER_PRODUCT",
+    "MENTIONABLE_UNIONS",
+    "USER_UNIONS",
+    "is_union",
+    "get_from_anno_type",
+    "issubclass_failsafe",
+    "is_optional",
+    "filter_extras",
+    "get_option",
+    "resolve_channel_types",
+)
+
+REVERSE_CHANNEL_MAPPING = {v: k for k, v in ipy.TYPE_CHANNEL_MAPPING.items()}
 
 UNION_TYPES = {typing.Union, types.UnionType}
 
-USER_TYPES = (naff.BaseUser, naff.User, naff.Member)
+USER_TYPES = (ipy.BaseUser, ipy.User, ipy.Member)
 USER_PRODUCT = itertools.product(USER_TYPES, USER_TYPES, USER_TYPES)
 
 MENTIONABLE_UNIONS = frozenset(
-    typing.Union[naff.Role, i, j, k] for i, j, k in USER_PRODUCT
+    typing.Union[ipy.Role, i, j, k] for i, j, k in USER_PRODUCT
 )
 USER_UNIONS = frozenset(typing.Union[i, j, k] for i, j, k in USER_PRODUCT)
 
 
 def is_union(anno: typing.Any):
     return typing.get_origin(anno) in UNION_TYPES
 
@@ -41,71 +58,74 @@
         return False
 
 
 def is_optional(anno: typing.Any):
     return is_union(anno) and types.NoneType in typing.get_args(anno)
 
 
-def filter_extras(t: naff.OptionTypes | type):
+def filter_extras(t: ipy.OptionType | type):
     if typing.get_origin(t) == typing.Annotated:
         t = get_from_anno_type(t)
 
     if is_optional(t):
         non_optional_args: tuple[type] = tuple(
             a for a in typing.get_args(t) if a is not types.NoneType
         )
         if len(non_optional_args) == 1:
             return non_optional_args[0]
         return typing.Union[non_optional_args]  # type: ignore
 
     return t
 
 
-def get_option(t: naff.OptionTypes | type):
+def get_option(t: ipy.OptionType | type):
     t = filter_extras(t)
 
-    if isinstance(t, naff.OptionTypes):
+    if isinstance(t, ipy.OptionType):
         return t
 
+    with contextlib.suppress(ValueError):
+        return ipy.OptionType(t)
+
     if t == str:
-        return naff.OptionTypes.STRING
+        return ipy.OptionType.STRING
     if t == int:
-        return naff.OptionTypes.INTEGER
+        return ipy.OptionType.INTEGER
     if t == bool:
-        return naff.OptionTypes.BOOLEAN
-    if issubclass_failsafe(t, (naff.BaseUser, naff.Member)) or t in USER_UNIONS:
-        return naff.OptionTypes.USER
-    if issubclass_failsafe(t, naff.BaseChannel):
-        return naff.OptionTypes.CHANNEL
-    if t == naff.Role:
-        return naff.OptionTypes.ROLE
+        return ipy.OptionType.BOOLEAN
+    if issubclass_failsafe(t, (ipy.BaseUser, ipy.Member)) or t in USER_UNIONS:
+        return ipy.OptionType.USER
+    if issubclass_failsafe(t, ipy.BaseChannel):
+        return ipy.OptionType.CHANNEL
+    if t == ipy.Role:
+        return ipy.OptionType.ROLE
     if t == float:
-        return naff.OptionTypes.NUMBER
-    if t == naff.Attachment:
-        return naff.OptionTypes.ATTACHMENT
+        return ipy.OptionType.NUMBER
+    if t == ipy.Attachment:
+        return ipy.OptionType.ATTACHMENT
     if t in MENTIONABLE_UNIONS:
-        return naff.OptionTypes.MENTIONABLE
+        return ipy.OptionType.MENTIONABLE
 
     if is_union(t):
         args = typing.get_args(t)
-        if all(issubclass_failsafe(a, naff.BaseChannel) for a in args):
-            return naff.OptionTypes.CHANNEL
+        if all(issubclass_failsafe(a, ipy.BaseChannel) for a in args):
+            return ipy.OptionType.CHANNEL
 
     raise ValueError("Invalid type provided.")
 
 
 def resolve_channel_types(anno: typing.Any):
     channel_types = []
 
     anno = filter_extras(anno)
 
-    if isinstance(anno, naff.OptionTypes):
+    if isinstance(anno, ipy.OptionType):
         return None
 
-    if issubclass_failsafe(anno, naff.BaseChannel) and (
+    if issubclass_failsafe(anno, ipy.BaseChannel) and (
         chan_type := REVERSE_CHANNEL_MAPPING.get(anno)
     ):
         channel_types = [chan_type]
     elif is_union(anno):
         for arg in typing.get_args(anno):
             if chan_type := REVERSE_CHANNEL_MAPPING.get(arg):
                 channel_types.append(chan_type)
```

### Comparing `tansy-0.5.2/tansy.egg-info/PKG-INFO` & `tansy-0.6.0/tansy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.5.2
-Summary: Unstable experiments with NAFF.
+Version: 0.6.0
+Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
-Author: Astrea49
+Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tansy
 
 [![PyPI](https://img.shields.io/pypi/v/tansy)](https://pypi.org/project/tansy/)
 [![Downloads](https://static.pepy.tech/personalized-badge/tansy?period=total&units=abbreviation&left_color=grey&right_color=green&left_text=pip%20installs)](https://pepy.tech/project/tansy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Unstable experiments with NAFF.
+Unstable experiments with interactions.py.
 
 # Commands
 
 `tansy` provides a unique way to define options for slash commands - a way that appears often in other Discord Python libraries.
 
 Instead of needing a decorator per option or to define the option in one huge list, `tansy` allows you to define each option in the function itself.
 By using a special metadata function, you can specify what each argument/parameter in a function should be like as an option, with tansy smartly handling the rest for you.
 
-## Example Command
 ```python
-import naff
+import interactions as ipy
 import tansy
 
 @tansy.slash_command(name="test", description="Nice test command, huh?")
 async def test_cmd(
-    ctx: naff.InteractionCommand,
-    the_user: naff.User = tansy.Option(name="user", description="The user to ping."),
+    ctx: ipy.InteractionContext,
+    the_user: ipy.User = tansy.Option(name="user", description="The user to ping."),
 ):
     await ctx.send(the_user.mention)
 ```
 
-# Speedups
+## Class Slash Command
 
-`tansy` also includes several patches that can speed up NAFF itself, sometimes by a signficant margin.
-However, these patches are unstable, and may break some (usually niche) parts of the things they modify.
+In case you want to try something very unique, or just want to leverage classes, `tansy` allows you to leverage its toolset to make class slash commands.
 
-To install them, use:
 ```python
+import interactions as ipy
 import tansy
 
-# this should be the first line of code you run in your main file if you want
-# everything to work correctly
-tansy.install_naff_speedups()
+@tansy.class_slash_command(name="test", description="Nice test command, huh?")
+class Test:
+    the_user: ipy.User = tansy.Option(name="user", description="The user to ping.")
+
+    async def callback(self, ctx: ipy.InteractionContext):
+        await ctx.send(self.the_user.mention)
 ```
 
-You can also toggle on or off what patches you want - take a look at the function's docstring for details.
+Note that the class is being read and adjusted to be more like a typical functional declaration, and so isn't a fully true class-based approach.
+Subclasses are not going to become subcommands (though `class_subcommand` exists), and while the class *does* get initialized on every run
+(meaning you can use custom `__init__`s, as long as they have no parameters that need to be filled in), the class is largely untouched outside
+of declaration and using `callback`.
```

