# Comparing `tmp/basecfg-1.2.0.tar.gz` & `tmp/basecfg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basecfg-1.2.0.tar", last modified: Sun Apr  9 19:02:15 2023, max compression
+gzip compressed data, was "basecfg-2.0.0.tar", last modified: Mon Apr 10 17:10:33 2023, max compression
```

## Comparing `basecfg-1.2.0.tar` & `basecfg-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-09 19:01:47.000000 basecfg-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 19:02:15.462575 basecfg-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 19:01:47.000000 basecfg-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-09 19:01:47.000000 basecfg-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:02:15.462575 basecfg-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/basecfg/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 19:01:47.000000 basecfg-1.2.0/src/basecfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-09 19:01:47.000000 basecfg-1.2.0/src/basecfg/basecfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:02:15.462575 basecfg-1.2.0/src/basecfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 19:02:15.000000 basecfg-1.2.0/src/basecfg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-10 17:10:06.000000 basecfg-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-10 17:10:33.474110 basecfg-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 17:10:06.000000 basecfg-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-10 17:10:06.000000 basecfg-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:10:33.474110 basecfg-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.470110 basecfg-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/src/basecfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 17:10:06.000000 basecfg-2.0.0/src/basecfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-04-10 17:10:06.000000 basecfg-2.0.0/src/basecfg/basecfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:10:33.474110 basecfg-2.0.0/src/basecfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:10:33.000000 basecfg-2.0.0/src/basecfg.egg-info/top_level.txt
```

### Comparing `basecfg-1.2.0/LICENSE` & `basecfg-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basecfg-1.2.0/pyproject.toml` & `basecfg-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basecfg"
-version = "1.2.0"
+version = "2.0.0"
 authors = [
   { name="Ben Burke", email="actualben@users.noreply.github.com" },
 ]
 description = "typed 12-factor app configuration helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `basecfg-1.2.0/src/basecfg/basecfg.py` & `basecfg-2.0.0/src/basecfg/basecfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,23 @@
     Any,
     Callable,
     Dict,
     List,
     NamedTuple,
     Optional,
     Sequence,
-    Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 
 # pylint: disable=invalid-name
 OptType = TypeVar("OptType")
-OptParserInput = Union[str, int, float]
+OptParserInput = Union[str, int, float, list]
 
 empty_line = re.compile(r"^\s*([#].*|$)")
 
 
 class OptionMetadata(NamedTuple):
     """
     OptionMetadata is a named tuple which encapsulates data captured by OptFunc
@@ -53,31 +52,34 @@
     BaseCfg is a base class for typed application configurations with
     automatic support for taking configuration data from config files,
     environment variables, and command-line arguments. Users of BaseCfg
     subclass basecfg.BaseCfg and add typed class attributes, defining
     them with basecfg.opt
     """
 
-    _optmeta: List[OptionMetadata]  # this is an attribute set by opt.link
+    _optmeta: List[OptionMetadata] = []
+    _optmeta_reset: bool = True
     _options: Dict[str, OptionMetadata]
     _prog: Optional[str] = None
     _prog_description: Optional[str] = None
     _prog_epilog: Optional[str] = None
+    _version: Optional[str] = None
 
     def __init__(
         self,
         json_config_path: Optional[str] = None,
         json_required=False,
         envfile_path: Optional[str] = None,
         envfile_required: bool = False,
         secrets_dir: str = "/run/secrets",
         cli_args: Optional[Sequence[str]] = None,
         prog: Optional[str] = None,
         prog_description: Optional[str] = None,
         prog_epilog: Optional[str] = None,
+        version: Optional[str] = None,
     ) -> None:
         """
         Creates a new instance of the configuration class; all arguments are optional
         json_config_path [str]: the path to a json config file to parse
         json_required [bool]: if True an exception will be raised if the given json
             config file is missing
         cli_args List[str]: instead of using sys.argv, this list of arguments will be
@@ -88,19 +90,24 @@
             usage documentation when the program is invoked with -h or --help
         prog_epilog [str]: additional text appearing at the end of the usage
             documentation that is printed when the program is invoked with -h or --help
         """
         self._prog = prog
         self._prog_description = prog_description
         self._prog_epilog = prog_epilog
+        self._version = version
 
         # step 1: enrich our metadata about the configuration options and load
         # default values. At this point we finally have the names of the fields
         # and are aware of their resolved type annotations.
-        option_metadata = iter(self._optmeta)
+
+        BaseCfg._optmeta_reset = True
+        # copying the _optmeta list from a BaseCfg class attr to an attr of this subclass
+        setattr(self.__class__, "_optmeta", BaseCfg._optmeta.copy())
+        option_metadata = iter(self.__class__._optmeta)
 
         self._options = {}
         for key, val in self.__class__.__annotations__.items():
             self._options[key] = next(option_metadata)._replace(
                 name=key,
                 option_type=val,
             )
@@ -129,51 +136,14 @@
         )
 
         # step 6: load config data from command-line arguments
         for key, val in self._parse_args(cli_args).items():
             if val is not None:
                 setattr(self, key, val)
 
-    @classmethod
-    def optfunc(cls):
-        """
-        helper function which returns a uniquely-namespaced opt function which
-        can  be used to define metadata for BaseCfg option fields
-        """
-        namespace: List[OptionMetadata] = []
-
-        def opt(
-            default: OptType,
-            doc: str,
-            required: bool = False,
-            parser: Optional[Callable[[OptParserInput], OptType]] = None,
-            choices: Optional[Sequence[OptType]] = None,
-            sep: str = ",",
-            redact: bool = False,
-        ) -> OptType:
-            """
-            opt captures data related to a BaseCfg option and returns the default
-            the annotated type of the return value is determined by the type of the
-            given default argument
-            """
-            namespace.append(
-                OptionMetadata(
-                    None, None, default, doc, required, parser, choices, sep, redact
-                )
-            )
-            return default
-
-        def link(cls) -> Type[cls]:
-            setattr(cls, "_optmeta", namespace)
-            return cls
-
-        opt.link = link
-
-        return opt
-
     def _parse_json_config(self, path: str, required: bool = False) -> Dict[str, Any]:
         """parses the configuration from the json file at the given path"""
         result: Dict[str, Any] = {}
         if not os.path.isfile(path):
             if required:
                 raise RuntimeError(f"required json config file {path} was not found")
             # no file, not required
@@ -198,15 +168,17 @@
                     "List[bool]": self._bool_list,
                     "List[float]": self._float_list,
                     "List[int]": self._int_list,
                     "List[str]": self._str_list,
                 }
 
                 coerced_value = val
-                if val_type != option_type:
+                if option.parser:
+                    coerced_value = option.parser(val)
+                elif val_type != option_type:
                     if val_type == "list":
                         if option_type not in coercions:
                             raise TypeError(
                                 f"{key}: unsupported list type {option_type}"
                             )
                     if option_type not in coercions:
                         raise TypeError(f"{key}: unsupported value type {option_type}")
@@ -250,22 +222,27 @@
     def _parse_args(self, cli_args: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         """generate an args parser and call it"""
         argp = argparse.ArgumentParser(
             prog=self._prog,
             description=self._prog_description,
             epilog=self._prog_epilog,
         )
+        if self._version:
+            argp.add_argument("--version", action="version", version=self._version)
         for optname, option in self._options.items():
             arg_name = "--" + optname.replace("_", "-")
             option_type = self._base_type(option.option_type)
 
             # use this for as little as possible (because it doesn't get type checked)
             # it could be good to switch to TypedDict for this
             arg_config: Dict[str, Any] = {"action": "store"}
-            if option_type == "bool":
+
+            if option.parser:
+                arg_config["type"] = option.parser
+            elif option_type == "bool":
                 arg_config["action"] = argparse.BooleanOptionalAction
             elif option_type == "int":
                 arg_config["type"] = int
             elif option_type == "float":
                 arg_config["type"] = float
             elif option_type == "List[str]":
                 arg_config["action"] = "append"
@@ -455,7 +432,31 @@
     def __len__(self):
         """returns the number of configuration options in the class"""
         return len(self._options)
 
     def __iter__(self):
         """returns keys iterator"""
         return iter(self._options.keys())
+
+
+def opt(
+    default: OptType,
+    doc: str,
+    required: bool = False,
+    parser: Optional[Callable[[OptParserInput], OptType]] = None,
+    choices: Optional[Sequence[OptType]] = None,
+    sep: str = ",",
+    redact: bool = False,
+) -> OptType:
+    """
+    opt captures data related to a BaseCfg option and returns the default
+    the annotated type of the return value is determined by the type of the
+    given default argument
+    """
+    # pylint: disable=protected-access
+    if BaseCfg._optmeta_reset:
+        BaseCfg._optmeta = []
+        BaseCfg._optmeta_reset = False
+    BaseCfg._optmeta.append(
+        OptionMetadata(None, None, default, doc, required, parser, choices, sep, redact)
+    )
+    return default
```

