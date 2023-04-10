# Comparing `tmp/risset-2.1.1.tar.gz` & `tmp/risset-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.1.1.tar", last modified: Mon Apr  3 23:00:18 2023, max compression
+gzip compressed data, was "risset-2.2.0.tar", last modified: Mon Apr 10 12:31:18 2023, max compression
```

## Comparing `risset-2.1.1.tar` & `risset-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-03 23:00:18.090409 risset-2.1.1/
--rw-rw-r--   0 em        (1000) em        (1000)     8354 2023-04-03 23:00:18.089409 risset-2.1.1/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.1.1/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-03 23:00:18.089409 risset-2.1.1/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8354 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       39 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       16 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-03 23:00:18.000000 risset-2.1.1/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   101077 2023-04-03 22:59:37.000000 risset-2.1.1/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-03 23:00:18.090409 risset-2.1.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      865 2023-03-12 11:31:29.000000 risset-2.1.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 12:31:18.323536 risset-2.2.0/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-10 12:31:18.323536 risset-2.2.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.0/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 12:31:18.323536 risset-2.2.0/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107324 2023-04-10 12:31:10.000000 risset-2.2.0/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-10 12:31:18.323536 risset-2.2.0/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.0/setup.py
```

### Comparing `risset-2.1.1/PKG-INFO` & `risset-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: risset
-Version: 2.1.1
-Summary: A package manager for csound
-Home-page: https://github.com/csound-plugins/risset
-Author: Eduardo Moguillansky
-Author-email: eduardo.moguillansky@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
 This is the repository of risset, a package manager for csound external
 plugins and user-defined-opcodes. The index aggregating all available packages is kept 
 at [risset-data](https://github.com/csound-plugins/risset-data).
```

### Comparing `risset-2.1.1/README.md` & `risset-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: risset
+Version: 2.2.0
+Summary: A package manager for csound
+Home-page: https://github.com/csound-plugins/risset
+Author: Eduardo Moguillansky
+Author-email: eduardo.moguillansky@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
 This is the repository of risset, a package manager for csound external
 plugins and user-defined-opcodes. The index aggregating all available packages is kept 
 at [risset-data](https://github.com/csound-plugins/risset-data).
@@ -264,7 +276,9 @@
 * `repository`: the URL were the source code for this plugin is hosted, for reference
 
 ### Platform support
 
 It is desirable, but not a requirement, that all opcodes support the three major desktop
 platforms: linux, macos and windows. Support for a given platform is indicated by the availability of
 a binary for the given platform in the manifest.
+
+
```

### Comparing `risset-2.1.1/risset.egg-info/PKG-INFO` & `risset-2.2.0/risset.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.1.1
+Version: 2.2.0
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![risset](assets/risset-title.png)
 
 # risset: a package manager for csound
 
@@ -274,7 +276,9 @@
 * `repository`: the URL were the source code for this plugin is hosted, for reference
 
 ### Platform support
 
 It is desirable, but not a requirement, that all opcodes support the three major desktop
 platforms: linux, macos and windows. Support for a given platform is indicated by the availability of
 a binary for the given platform in the manifest.
+
+
```

### Comparing `risset-2.1.1/risset.py` & `risset-2.2.0/risset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
 
@@ -20,72 +20,197 @@
 import json
 from dataclasses import dataclass, asdict as _asdict
 import tempfile
 import shutil
 import subprocess
 import textwrap
 import fnmatch
+import pprint
 
 import urllib.parse
 import urllib.request
 import urllib.error
 from pathlib import Path
 from zipfile import ZipFile
 import inspect as _inspect
 import re
 from string import Template as _Template
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from typing import List, Dict, Tuple, Union, Optional, Any
+    from typing import Union, Optional, Any
 
 
 INDEX_GIT_REPOSITORY = "https://github.com/csound-plugins/risset-data"
 
 
 _UNSET = object()
 
 
-class _Register:
+def _csoundlib_version() -> tuple[int, int]:
+    import ctcsound7
+    versionid = ctcsound7.libcsound.csoundGetVersion()
+    major = versionid // 1000
+    minor = (versionid - major*1000) // 10
+    return major, minor
+
+
+def _csound_version(csoundexe='csound') -> tuple[int, int]:
+    csound_bin = _get_binary(csoundexe)
+    if not csound_bin:
+        raise OSError("csound binary not found")
+    proc = subprocess.Popen([csound_bin, "--version"], stderr=subprocess.PIPE)
+    proc.wait()
+    assert proc.stderr is not None
+    out = proc.stderr.read().decode('ascii')
+    for line in out.splitlines():
+        if match := re.search(r'--Csound\s+version\s+(\d+)\.(\d+)(.*)', line):
+            major = int(match.group(1))
+            minor = int(match.group(2))
+            rest = match.group(3)
+            return major, minor
+    raise ValueError("Could not find a version number in the output")
+
+
+class _Session:
+    """
+    Simgleton class to hold information about the session
+
+    This class keeps track of downloaded files, cloned repos, etc.
+    """
+    instance: _Session = None
+
+    def __new__(cls, *args, **kwargs):
+        if _Session.instance is not None:
+            return _Session.instance
+
+        instance = super().__new__(cls, *args, **kwargs)
+        _Session.instance = instance
+        return instance
+
     def __init__(self):
-        self.downloaded_files: Dict[str, Path] = {}
-        self.cloned_repos: Dict[str, Path]  = {}
+        self.downloaded_files: dict[str, Path] = {}
+        self.cloned_repos: dict[str, Path] = {}
         self.platform: str = {
             'linux': 'linux',
             'darwin': 'macos',
             'win32': 'windows'
         }[sys.platform]
         self.debug = False
+        major, minor = _csoundlib_version()
+        self.csound_version: int = major * 1000 + minor * 10
+        self.stop_on_errors = True
         self.cache = {}
 
 
-register = _Register()
+_session = _Session()
+
+
+@dataclass
+class _VersionRange:
+    minversion: int
+    maxversion: int
+    includemin: bool = True
+    includemax: bool = False
+
+    def __post_init__(self):
+        assert isinstance(self.minversion, int) and self.minversion >= 6000, f"Got {self.minversion}"
+        assert isinstance(self.maxversion, int) and self.maxversion >= 6000, f"Got {self.maxversion}"
+
+    def contains(self, versionid: int) -> bool:
+        """
+        Returns True if version is contained within this version range
+
+        Args:
+            version: a version id, where version id is ``int(major.minor * 1000)``
+
+        Returns:
+            True if *version* is within this range
+
+        Example
+        -------
+
+            >>> v = _VersionRange(minversion=6180, maxversion=7000, includemin=True, includemax=False)
+            >>> v.contains(6190)
+            True
+            >>> v.contains(7000)
+            False
+        """
+        if not isinstance(versionid, int) or versionid < 6000:
+            raise ValueError(f"Invalid versionid, got {versionid}")
+        a = versionid > self.minversion if not self.includemin else versionid >= self.minversion
+        maxversion = self.maxversion or 99999
+        b = versionid < maxversion if not self.includemax else versionid <= maxversion
+        return a and b
 
 
 def _get_platform() -> str:
     """
     Returns one of "linux", "macos", "windows"
 
     * all 'linux', 'macos' and 'windows' refer to x86-64
     """
     # TODO: add support for arm linux (raspi, etc.)
-    return register.platform
+    return _session.platform
 
 
-def _termsize(width=80, height=25) -> Tuple[int, int]:
+def _termsize(width=80, height=25) -> tuple[int, int]:
     if not sys.stdout.isatty():
         return width, height
 
     try:
         t = os.get_terminal_size()
         return t.columns, t.lines
     except:
         return width, height
 
 
+def _version_to_versionid(versionstr: str) -> int:
+    if '.' not in versionstr:
+        return int(versionstr)
+    majors, minors = versionstr.split('.', maxsplit=1)
+    patch = 0
+    if '.' in minors:
+        minors, patchs = minors.split('.', maxsplit=1)
+        patch = int(patchs)
+        assert 0 <= patch < 10
+    versionid = int(majors) * 1000 + int(minors) * 10 + patch
+    return versionid
+
+
+def _parse_version(versionstr: str) -> _VersionRange:
+    versionstr = versionstr.replace(' ', '')
+    if versionstr.startswith("=="):
+        exactversionstr = versionstr[2:]
+        versionid = _version_to_versionid(exactversionstr)
+        return _VersionRange(minversion=versionid, maxversion=versionid, includemin=True, includemax=True)
+
+    parts = re.split(r"(>=|<=|>|<)", versionstr)
+    parts = [p for p in parts if p]
+    if len(parts) % 2 != 0:
+        raise ParseError(f"Could not parse version range: {versionstr}, parts: {parts}")
+    minversion = 6000
+    maxversion = 9999
+    includemax = False
+    includemin = False
+    for op, version in zip(parts[::2], parts[1::2]):
+        assert op in ('<', '>', '<=', '>=')
+        if op[0] == '<':
+            maxversion = _version_to_versionid(version)
+            if op[-1] == '=':
+                includemax = True
+        elif op[0] == '>':
+            minversion = _version_to_versionid(version)
+            if op[-1] == '=':
+                includemin = True
+        else:
+            raise ParseError(f"Could not parse version range: {versionstr}, operator {op} not supported")
+    return _VersionRange(minversion=minversion, maxversion=maxversion, includemin=includemin, includemax=includemax)
+
+
 def _abbrev(s: str, maxlen: int) -> str:
     """Abbreviate string"""
     assert maxlen > 18
     l = len(s)
     if l < maxlen:
         return s
     rightlen = min(8, l // 5)
@@ -172,23 +297,25 @@
     Is `url` an url to a git repo?
     """
     return _is_url(url) and url.endswith(".git")
 
 
 def _debug(*msgs, ljust=20) -> None:
     """ Print debug info only if debugging is turned on """
-    if register.debug:
+    if _session.debug:
         caller = _abbrev(_inspect.stack()[1][3], ljust)
         print(f"DEBUG:{caller.ljust(ljust)}:", *msgs, file=sys.stderr)
 
 
 def _errormsg(msg: str) -> None:
     """ Print error message """
-    for line in msg.splitlines():
-        print("** Error: ", line, file=sys.stderr)
+    lines = msg.splitlines()
+    print("** Error:", lines[0], file=sys.stderr)
+    for line in lines[1:]:
+        print("         ", line, file=sys.stderr)
 
 
 def _info(*msgs: str) -> None:
     print(*msgs)
 
 
 class ErrorMsg(str):
@@ -213,15 +340,15 @@
         platform: if given, the platform for which this assets are valid (in the case
             of binaries of some kind)
         name: the name of the asset (optional)
     """
     source: str
     """the url where to download the assets from"""
 
-    patterns: List[str]
+    patterns: list[str]
     """the paths to extract from the url (if needed). It can be a glob pattern"""
 
     platform: str = 'all'
     """the platform for which this assets are valid"""
 
     name: str = ''
 
@@ -245,15 +372,15 @@
                 return _download_file(self.source)
         else:
             # it is a path, check that it exists
             source = Path(self.source)
             assert source.exists(), f"Assert source does not exist: {source}"
             return source
 
-    def retrieve(self) -> List[Path]:
+    def retrieve(self) -> list[Path]:
         """
         Download and resolve all files, if needed
 
         Returns:
             a (possibly empty) list of local paths which belong to this asset.
             In the case of an asset referring to a file within a zip, the
             files are extracted to a temp dir and a path to that temp dir
@@ -262,15 +389,15 @@
         assert self.source and (_is_url(self.source) or os.path.isabs(self.source)), \
             f"Source should be either a url or an absolute path: {self.source}"
         # self.url is either a git repo or a url pointing to a file
         root = self.local_path()
         if root.is_dir():
             assert _is_git_repo(root)
             _git_update(root)
-            collected_assets: List[Path] = []
+            collected_assets: list[Path] = []
             for pattern in self.patterns:
                 matchedfiles = glob.glob((root/pattern).as_posix())
                 collected_assets.extend(Path(m) for m in matchedfiles)
             return collected_assets
         elif root.suffix == '.zip':
             _debug(f"Extracting {self.patterns} from {root}")
             outfiles = _zip_extract(root, self.patterns)
@@ -295,33 +422,62 @@
             users regarding the compatibility of the binary. It can be anything but expected values
             might be something like "macOS 11.xx.
         extractpath: in the case of using a .zip file as url, the extract path should indicate
             a relative path to the binary within the .zip file structure
         post_install_script: a script to run after the binary has been installed
     """
     platform: str
+    """The platform for which this binary was compiled"""
+
     url: str
-    build_platform: str = ''
+    """The url of the binary (can be a zip file)"""
+
+    csound_version: str
+    """The version range for which this binary is valid (can be of the form >=P.q<X.y)"""
+
     extractpath: str = ''
+    """In the case of the url being an archive, this indicates the relative path of the binary within that archive"""
+
+    build_platform: str = ''
+    """If known, the platform under which this binary was built. This can be anything, it is just informative"""
+
     post_install_script: str = ''
+    """A script to run after installation"""
+
+    _csound_version_range: _VersionRange = None
+
+    def csound_version_range(self) -> _VersionRange:
+        if self._csound_version_range is None:
+            self._csound_version_range = _parse_version(self.csound_version)
+        return self._csound_version_range
+
+    def matches_versionid(self, versionid: int) -> bool:
+        """
+        Does this binary apply to the  given versionid?
+
+        Returns:
+            True if the versionid is contained within the version range of this binary
+        """
+        assert isinstance(versionid, int) and versionid >= 6000, f"Got {versionid}"
+        return self.csound_version_range().contains(versionid)
 
     def binary_filename(self) -> str:
         """
         The filename of the binary
         """
         if not self.url.endswith('.zip'):
             return os.path.split(self.url)[1]
         else:
             assert self.extractpath
             return os.path.split(self.extractpath)[1]
 
 
 @dataclass
 class ManPage:
-    syntaxes: List[str]
+    syntaxes: list[str]
     abstract: str
 
 
 @dataclass
 class IndexItem:
     """
     An  entry in the risset index
@@ -372,17 +528,14 @@
 @dataclass
 class Plugin:
     """
     Attribs:
         name: name of the plugin
         version: a version for this plugin, for update reasons
         short_description: a short description of the plugin or its opcodes
-        csound_version: csound version compatible with this plugin. Can be a specific version like '6.17' in
-            which case this is understood as >= 6.17. Also possible: '>=6.17', '==6.17', '>=6.17<7.0'.
-            The version itself must be of the format X.Y or X.Y.Z where all parts are integers.
         binaries: a dict mapping platform to a Binary, like {'windows': Binary(...), 'linux': Binary(...)}
             Possible platforms are: 'linux', 'windows', 'macos', where in each case x86_64 is implied. Other
                 platforms, when supported, will be of the form 'linux-arm64' or 'macos-arm64'
         opcodes: a list of opcodes defined in this plugin
         assets: a list of Assets
         author: the author of this plugin
         email: the email of the author
@@ -405,46 +558,38 @@
         ]
     }
     """
     name: str
     url: str
     version: str
     short_description: str
-    csound_version: str
-    binaries: Dict[str, Binary]
-    opcodes: List[str]
+    binaries: list[Binary]
+    opcodes: list[str]
     author: str
     email: str
     cloned_path: Path
     manifest_relative_path: str = ''
     long_description: str = ''
     doc_folder: str = 'doc'
-    assets: Optional[List[Asset]] = None
+    assets: Optional[list[Asset]] = None
+
+    def __post_init__(self):
+        assert isinstance(self.binaries, list)
+        assert isinstance(self.opcodes, list)
+        assert not self.assets or isinstance(self.assets, list)
 
     def __hash__(self):
         return hash((self.name, self.version))
 
     @property
-    def versiontuple(self) -> Tuple[int, int, int]:
+    def versiontuple(self) -> tuple[int, int, int]:
         if self.version:
             return _version_tuple(self.version)
         return (0, 0, 0)
 
-    def binary_filename(self, platform: str = None) -> Optional[str]:
-        """
-        The filename of the binary (a .so, .dll or .dylib file)
-
-        Returns the filename of the binary, or None if there is no
-        binary for the given/current platform
-        """
-        if platform is None:
-            platform = _get_platform()
-        binary = self.binaries.get(platform)
-        return binary.binary_filename() if binary else None
-
     def local_manifest_path(self) -> Path:
         """
         The local path to the manifest file of this plugin
         """
         return self.cloned_path / self.manifest_relative_path / "risset.json"
 
     def asdict(self) -> dict:
@@ -456,14 +601,17 @@
         Returns the path to the man page for opcode
         """
         markdownfile = opcode + ".md"
         path = self.resolve_doc_folder() / markdownfile
         return path if path.exists() else None
 
     def resolve_path(self, relpath: Union[Path, str]) -> Path:
+        """
+        Returns the absolute path relative to the manifest path of this plugin
+        """
         root = self.local_manifest_path().parent
         return _resolve_path(relpath, root)
 
     def resolve_doc_folder(self) -> Path:
         """
         Resolve the doc folder for this plugin
 
@@ -472,33 +620,51 @@
         besides the manifest
         """
         root = self.local_manifest_path().parent
         doc_folder = _resolve_path(self.doc_folder or "doc", root)
         if not doc_folder.exists():
             raise OSError(f"No doc folder found (declared as {doc_folder}")
         return doc_folder
-
-    def binarydef_for_platform(self, platform: str = None) -> Optional[Binary]:
+    
+    def find_binary(self, platform: str = None, csound_version: int = 0) -> Optional[Binary]:
         """
-        Return the Binary for the given platform
+        Find a binary for the platform and csound versions given / current
 
-        If platform is None, use the current platform
+        Returns:
+            a Binary which matches the given platform and csound version, or None
+            if no match possible
         """
-        if platform is None:
-            platform = register.platform
 
-        return self.binaries.get(platform)
+        if not csound_version:
+            csound_version = _session.csound_version
+        else:
+            assert isinstance(csound_version, int) and csound_version >= 6000, f"Got {csound_version}"
 
+        if platform is None:
+            platform = _session.platform
+
+        possible_binaries = [b for b in self.binaries
+                             if b.platform == platform and b.matches_versionid(csound_version)]
+        if not possible_binaries:
+            return None
+        else:
+            if len(possible_binaries) > 1:
+                _debug(f"Found multiple binaries for {self.name}")
+            return possible_binaries[0]
+
+    def available_binaries(self) -> list[str]:
+        return [f"{binary.platform}/csound{binary.csound_version}"
+                for binary in self.binaries]
 
 
 @dataclass
 class Opcode:
     name: str
     plugin: str
-    syntaxes: Optional[List[str]] = None
+    syntaxes: Optional[list[str]] = None
     abstract: str = ''
     installed: bool = True
 
 
 @dataclass
 class InstalledPluginInfo:
     """
@@ -514,15 +680,15 @@
     name: str
     dllpath: Path
     versionstr: Optional[str]
     installed_manifest_path: Optional[Path] = None
     installed_in_system_folder: bool = False
 
     @property
-    def versiontuple(self) -> Tuple[int, int, int]:
+    def versiontuple(self) -> tuple[int, int, int]:
         return _version_tuple(self.versionstr) if self.versionstr and self.versionstr != UNKNOWN_VERSION else (0, 0, 0)
 
 
 UNKNOWN_VERSION = "Unknown"
 
 
 class PlatformNotSupportedError(Exception):
@@ -566,73 +732,57 @@
             'linux': f'$HOME/.local/lib/csound/{majorversion}.0/plugins64',
             'win32': f'C:\\Users\\$USERNAME\\AppData\\Local\\csound\\{majorversion}.0\\plugins64',
             'darwin': f'$HOME/Library/csound/{majorversion}.0/plugins64'
         }[sys.platform]
         out = Path(os.path.expandvars(pluginsdir))
     return out
 
-def _csound_version(csoundexe='csound') -> Tuple[int, int]:
-    csound_bin = _get_binary(csoundexe)
-    if not csound_bin:
-        raise OSError("csound binary not found")
-    proc = subprocess.Popen([csound_bin, "--version"], stderr=subprocess.PIPE)
-    proc.wait()
-    assert proc.stderr is not None
-    out = proc.stderr.read().decode('ascii')
-    for line in out.splitlines():
-        if match := re.search(r'--Csound\s+version\s+(\d+)\.(\d+)(.*)', line):
-            major = int(match.group(1))
-            minor = int(match.group(2))
-            rest = match.group(3)
-            return major, minor
-    raise ValueError("Could not find a version number in the output")
-
 
 def _is_glob(s: str) -> bool:
     return "*" in s or "?" in s
 
 
 def _zip_extract_folder(zipfile: Path, folder: str, cleanup=True, destroot: Path = None) -> Path:
     foldername = os.path.split(folder)[1]
     root = Path(tempfile.mktemp())
     root.mkdir(parents=True, exist_ok=True)
     z = ZipFile(zipfile, 'r')
     pattern = folder + '/*'
     extracted = [z.extract(name, root) for name in z.namelist()
-                if fnmatch.fnmatch(name, pattern)]
+                 if fnmatch.fnmatch(name, pattern)]
     _debug(f"_zip_extract_folder: Extracted files from folder {folder}: {extracted}")
     if destroot is None:
         destroot = Path(tempfile.gettempdir())
     destfolder = destroot / foldername
     if destfolder.exists():
         _debug(f"_zip_extract_folder: Destination folder {destfolder} already exists, removing")
         _rm_dir(destfolder)
     shutil.move(root / folder, destroot)
     assert destfolder.exists() and destfolder.is_dir()
     if cleanup:
         _rm_dir(root)
     return destfolder
 
 
-def _zip_extract(zipfile: Path, patterns: List[str]) -> List[Path]:
+def _zip_extract(zipfile: Path, patterns: list[str]) -> list[Path]:
     """
     Extract multiple files from zip
 
     Args:
         zipfile: the zip file to extract from
         patterns: a list of filenames or glob patterns
 
     Returns:
         a list of output files extracted. If glob patterns were used there might be
         more output files than number of patterns. Otherwise there is a 1 to 1
         relationship between input and output
     """
     outfolder = Path(tempfile.gettempdir())
     z = ZipFile(zipfile, 'r')
-    out: List[Path] = []
+    out: list[Path] = []
     zipped = z.namelist()
     _debug(f"Inspecting zipfile {zipfile}, contents: {zipped}")
     for pattern in patterns:
         if _is_glob(pattern):
             _debug(f"Matching names against pattern {pattern}")
             for name in zipped:
                 if name.endswith("/") and fnmatch.fnmatch(name[:-1], pattern):
@@ -651,24 +801,24 @@
 def _zip_extract_file(zipfile: Path, extractpath: str) -> Path:
     """
     Extracts a file from a zipfile, returns the path to the extracted file
 
     Args:
         zipfile: the path to a local .zip file
         extractpath: the path to extract inside the .zip file
-        outfolder: where to expand the zip file
 
     Returns:
         the path of the extracted file.
 
     Raises KeyError if `extractpath` is not in `zipfile`
     """
     return _zip_extract(zipfile, [extractpath])[0]
 
-def _csound_opcodes() -> List[str]:
+
+def _csound_opcodes() -> list[str]:
     """
     Returns a list of installed opcodes
     """
     csound_bin = _get_binary("csound")
     if not csound_bin:
         raise RuntimeError("Did not find csound binary")
     proc = subprocess.run([csound_bin, "-z1"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
@@ -713,51 +863,51 @@
     shell = os.path.split(shellenv)[1].strip()
     if shell in ("bash", "zsh", "fish"):
         return shell
     return None
 
 
 def _get_binary(binary) -> Optional[str]:
-    if (out:=register.cache.get('csound-bin', _UNSET)) is _UNSET:
+    if (out := _session.cache.get('csound-bin', _UNSET)) is _UNSET:
         path = shutil.which(binary)
-        register.cache['csound-bin'] = out = path if path else None
+        _session.cache['csound-bin'] = out = path if path else None
     return out
 
 
 def _get_git_binary() -> str:
-    if (path := register.cache.get('git-binary')) is None:
+    if (path := _session.cache.get('git-binary')) is None:
         path = shutil.which("git")
         if not path or not os.path.exists(path):
             raise RuntimeError("git binary not found")
-        register.cache['git-binary'] = path
+        _session.cache['git-binary'] = path
     return path
 
 
 def _git_local_path(repo: str, update=False) -> Path:
     """
     Query the local path of the given repository, clone if needed
 
     Args:
         repo: the url of the git repository
         update: if not cloned, update the repo
     """
-    if repo in register.cloned_repos:
-        return register.cloned_repos[repo]
+    if repo in _session.cloned_repos:
+        return _session.cloned_repos[repo]
     assert repo and _is_git_url(repo), f"Invalid repository name: {repo}"
     _debug(f"Querying local path for repo {repo}")
     reponame = _git_reponame(repo)
     destination = RISSET_CLONES_PATH / reponame
     if destination.exists():
         assert _is_git_repo(destination), f"Expected {destination} to be a git repository"
-        register.cloned_repos[repo] = destination
+        _session.cloned_repos[repo] = destination
         if update:
             _git_update(destination)
     else:
         _git_clone_into(repo, destination=destination, depth=1)
-        register.cloned_repos[repo] = destination
+        _session.cloned_repos[repo] = destination
     return destination
 
 
 def _git_clone_into(repo: str, destination: Path, depth=1) -> None:
     """
     Clone the given repository to the destination.
 
@@ -792,15 +942,15 @@
     as fast as to check first and then act.
     """
     cwd = os.path.abspath(os.path.curdir)
     os.chdir(str(repopath))
     git = _get_git_binary()
     subprocess.call([git, "fetch"])
     headhash = subprocess.check_output([git, "rev-parse", "HEAD"]).decode('utf-8')
-    upstreamhash =subprocess.check_output([git, "rev-parse", "master@{upstream}"]).decode('utf-8')
+    upstreamhash = subprocess.check_output([git, "rev-parse", "master@{upstream}"]).decode('utf-8')
     _debug(f"Checking hashes, head: {headhash}, upstream: {upstreamhash}")
     os.chdir(cwd)
     return headhash != upstreamhash
 
 
 def _git_update(repopath: Path, depth=0, check_if_needed=False) -> None:
     """
@@ -814,22 +964,22 @@
         return
     gitbin = _get_git_binary()
     cwd = os.path.abspath(os.path.curdir)
     os.chdir(str(repopath))
     args = [gitbin, "pull"]
     if depth > 0:
         args.extend(['--depth', str(depth)])
-    if register.debug:
+    if _session.debug:
         subprocess.call(args)
     else:
         subprocess.call(args, stdout=subprocess.PIPE)
     os.chdir(cwd)
 
 
-def _version_tuple(versionstr: str) -> Tuple[int, int, int]:
+def _version_tuple(versionstr: str) -> tuple[int, int, int]:
     """ Convert a version string to its integer parts """
     if not versionstr:
         raise ValueError("versionstr is empty")
     parts = versionstr.split(".", maxsplit=3)
     try:
         ints = [int(part) for part in parts]
     except ValueError:
@@ -842,15 +992,15 @@
     elif len(ints) > 3:
         _debug("Too many version parts (max. 3), using the first 3")
         ints = ints[:3]
     i1, i2, i3 = ints
     return i1, i2, i3
 
 
-def _find_system_plugins_path(possible_paths: List[Path]) -> Optional[Path]:
+def _find_system_plugins_path(possible_paths: list[Path]) -> Optional[Path]:
     """
     Given a list of possible paths, find the folder where the system plugins are installed
     """
     ext = _plugin_extension()
     _debug("> Searching opcodes dir: ")
 
     if sys.platform == "win32":
@@ -869,15 +1019,15 @@
             _debug(f">>> path {d} exists, but has no plugins, skipping")
         elif any(plugin for plugin in plugins if dll == plugin.name):
             _debug(">>> Found!")
             return path
         else:
             _debug(f">>> Path exists, but it does not seem to be the systems plugin path\n"
                    f">>> ({dll} was not found there)")
-            _debug( ">>> Plugins found here: ", ', '.join(plugin.name for plugin in plugins))
+            _debug(f">>> Plugins found here: ", ', '.join(plugin.name for plugin in plugins))
     return None
 
 
 def _load_installation_manifest(path: Path) -> dict:
     """
     Load an installation manifest
 
@@ -902,15 +1052,15 @@
     Args:
         s: URL address string to validate
     """
     result = urllib.parse.urlparse(str(s))
     return bool(result.scheme and result.netloc)
 
 
-def _parse_pluginkey(pluginkey: str) -> Tuple[str, str]:
+def _parse_pluginkey(pluginkey: str) -> tuple[str, str]:
     """
     Given a key pluginname@version, return (pluginname, version)
 
     Handle cases where the pluginkey has no version
     """
     if "@" in pluginkey:
         name, version = pluginkey.split("@")
@@ -925,23 +1075,23 @@
         versiontup = _version_tuple(version)
     except ValueError as e:
         _debug(f"Error while parsing version {version}: %s", str(e))
         return default
     return ".".join(str(i) for i in versiontup)
 
 
-def _expand_substitutions(s: str, substitutions: Dict[str, str]) -> str:
+def _expand_substitutions(s: str, substitutions: dict[str, str]) -> str:
     """
     Expands variables of the form $var or ${var}
     """
     t = _Template(s)
     return t.substitute(substitutions)
 
 
-def _parse_binarydef(platform: str, binarydef: dict, substitutions: Dict[str, str]) -> Binary:
+def _parse_binarydef(binarydef: dict, substitutions: dict[str, str]) -> Binary:
     """
     Parses a binary definition within a risset.json dict
 
     A binary definition has the form
 
     "platform": {
         "url": str,
@@ -952,25 +1102,34 @@
     * url: the url where to download the binary. It can be an url to the binary itself, to a .zip file,
         or to a git repository
     * build_platform: the platform where the given binary was built. This serves as reference for
         a user. For example, in linux a build platform might be "Ubuntu 20.04"
     * extractpath: if the case where the url does not point to a binary, extractpath should be used
         to indicate the location of the binary within the .zip file or within the git repository
     """
-    assert isinstance(binarydef, dict)
+    assert isinstance(binarydef, dict), f"dict: {binarydef}"
+    platform = binarydef.get('platform')
+    if not platform:
+        raise ParseError(f"Plugin binary should have a platform key. Binary definition: {binarydef}")
+
     url = binarydef.get('url')
     if not url:
         raise ParseError(f"Plugin definition for {platform} should have an url")
+
+    csound_version = binarydef.get('csound_version')
+    if not csound_version:
+        _errormsg(f'No csound version found for binary {binarydef}')
+        csound_version = '>=6.18<7.0'
+
     url = _expand_substitutions(url, substitutions)
-    build_platform = binarydef.get('build_platform')
-    if not build_platform:
-        raise ParseError(f"Plugin definition for {platform} should have a build_platform")
+    build_platform = binarydef.get('build_platform', 'unknown')
     return Binary(platform=platform, url=url, build_platform=build_platform,
                   extractpath=binarydef.get('extractpath', ''),
-                  post_install_script=binarydef.get('post_install', ''))
+                  post_install_script=binarydef.get('post_install', ''),
+                  csound_version=csound_version)
 
 
 def _parse_asset(assetdef: dict, defaultsource: str) -> Asset:
     source = assetdef.get('url', defaultsource)
     extractpath = assetdef.get('extractpath') or assetdef.get('path')
     if not source and not extractpath:
         raise ParseError(f"Asset definition should have an URL or an extractpath key")
@@ -995,33 +1154,44 @@
     clonepath = _git_local_path(pluginurl)
     version = _normalize_version(_enforce_key(d, 'version'))
     pluginname = _enforce_key(d, 'name')
     opcodes = _enforce_key(d, 'opcodes')
     opcodes.sort()
     substitutions = {key: str(value) for key, value in d.items() if isinstance(value, (int, float, str))}
 
-    binaries: Dict[str, Binary] = {}
-    for platform, binarydef in _enforce_key(d, 'binaries').items():
+    binaries: list[Binary] = []
+    binarydefs = _enforce_key(d, 'binaries')
+    if not isinstance(binarydefs, list):
+        s = pprint.pformat(binarydefs)
+        _errormsg(f"Expected a list of binary definitions, got: ")
+        _errormsg(s)
+        raise SchemaError(f"Parsing 'binaries', expected a list of binary definitions, got a {type(binarydefs)}")
+    for binarydef in binarydefs:
+        if not isinstance(binarydef, dict):
+
+            _errormsg(f"{pluginname}: Parsing 'binaries' key, expected a dict, got")
+            raise SchemaError(f"Parsing 'binaries', Expected a dict, got {binarydef}")
         try:
-            binary = _parse_binarydef(platform, binarydef, substitutions=substitutions)
-            binaries[binary.platform] = binary
+            _debug(f"Parsing binary definition for {pluginname}: {binarydef}")
+            binary = _parse_binarydef(binarydef, substitutions=substitutions)
+            binaries.append(binary)
         except ParseError as e:
             _errormsg(f"Failed to parse binary definition for plugin {d.get('name', '??')}")
             _errormsg(f"... source data: {binarydef}")
             _errormsg(str(e))
 
     if not binaries:
         raise SchemaError("No valid binaries defined")
 
     manifest_local_folder = clonepath / subpath
     if not manifest_local_folder.exists():
         _errormsg(f"The local manifest folder corresponding to plugin {pluginname} was not found "
                   f"({manifest_local_folder})")
 
-    assets: List[Asset] = []
+    assets: list[Asset] = []
     assetdefs = d.get('assets')
     if assetdefs:
         if not isinstance(assetdefs, list):
             raise SchemaError(f"assets should hold a list of asset definitions, got {assetdefs}")
         for assetdef in assetdefs:
             try:
                 assets.append(_parse_asset(assetdef, defaultsource=manifest_local_folder.as_posix()))
@@ -1030,50 +1200,49 @@
 
     return Plugin(
         name=_enforce_key(d, 'name'),
         version=version,
         short_description=_enforce_key(d, 'short_description'),
         author=_enforce_key(d, 'author'),
         email=_enforce_key(d, 'email'),
-        csound_version=_enforce_key(d, 'csound_version'),
         opcodes=opcodes,
         binaries=binaries,
         doc_folder=d.get('doc', ''),
         long_description=d.get('long_description', ''),
         url=pluginurl,
         manifest_relative_path=subpath,
         assets=assets,
         cloned_path=_git_local_path(pluginurl)
     )
 
 
-def _resolve_path(path: Union[str, Path], basedir: Union[str, Path, None]=None
+def _resolve_path(path: Union[str, Path],
+                  basedir: Union[str, Path, None] = None
                   ) -> Path:
     """
     Convert path to absolute, use `basedir` or the cwd as base
     """
     p = Path(path)
     if p.is_absolute():
         return p.resolve()
     if basedir is None:
         return (Path.cwd()/p).resolve()
     return (Path(basedir) / p).resolve()
 
 
-
 def _rm_dir(path: Path) -> None:
 
     if not path.exists():
         return
 
     # On windows rmtree might fail when a file is marked as read-only
     # This is the case inside a git repo.
     # Solution taken from: https://bugs.python.org/issue43657
     def remove_readonly(func, path, exc_info):
-        "Clear the readonly bit and reattempt the removal"
+        """Clear the readonly bit and reattempt the removal"""
         # ERROR_ACCESS_DENIED = 5
         if func not in (os.unlink, os.rmdir) or exc_info[1].winerror != 5:
             raise exc_info[1]
         os.chmod(path, stat.S_IWRITE)
         func(path)
 
     shutil.rmtree(path.as_posix(), onerror=remove_readonly)
@@ -1094,16 +1263,16 @@
             else:
                 shutil.copy(f.as_posix(), dest.as_posix())
     else:
         _debug(f"Copying file {str(src)} to {str(dest)}")
         shutil.copy(src.as_posix(), dest.as_posix())
 
 
-
-def _read_plugindef(filepath: Union[str, Path], url: str = '',
+def _read_plugindef(filepath: Union[str, Path],
+                    url: str = '',
                     manifest_relative_path: str = ''
                     ) -> Plugin:
     """
     Create a Plugin from a plugin definition file (risset.json)
 
     Args:
         filepath: an absolute path to the plugin definition
@@ -1148,73 +1317,77 @@
 def _normalize_path(path: str) -> str:
     path = os.path.expandvars(path)
     path = os.path.expanduser(path)
     path = os.path.abspath(path)
     return path
 
 
-def _make_install_manifest(plugin: Plugin, assetfiles: List[str] = None) -> dict:
+def _make_install_manifest(plugin: Plugin, assetfiles: list[str] = None) -> dict:
     """
     Create an installation manifest dict
 
     Args:
         plugin: the Plugin corresponding to this installation manifest
         assetfiles: if given, a list of asset filenames installed by this plugin
             (only the filenames, no path: all assets are placed in a flat folder
             under the plugins prefix)
     """
     platform = _get_platform()
-    out: Dict[str, Any] = {}
+    binary = plugin.find_binary(platform=platform)
+    if not binary:
+        raise RuntimeError(f"No binary found for plugin {plugin.name} (platform: {platform}")
+
+    out: dict[str, Any] = {}
     out['name'] = plugin.name
     out['author'] = plugin.author
     out['email'] = plugin.email
     out['version'] = plugin.version
     out['opcodes'] = plugin.opcodes
     out['long_description'] = plugin.long_description
     out['short_description'] = plugin.short_description
-    out['build_platform'] = plugin.binaries[platform].build_platform
-    out['binary'] = plugin.binaries[platform].binary_filename()
+    out['build_platform'] = binary.build_platform
+    out['binary'] = binary.binary_filename()
     out['platform'] = platform
     out['assetfiles'] = assetfiles or []
     return out
 
 
 def _print_with_line_numbers(s: str) -> None:
     for i, line in enumerate(s.splitlines()):
         print(f"{i+1:003d} {line}")
 
 
 def _download_file(url: str, cache=True) -> Path:
     """
     Download the given url. Raises RuntimeError if failed
     """
-    path = register.downloaded_files.get(url)
+    path = _session.downloaded_files.get(url)
     if path is not None and cache:
         return path
     _debug("Downloading url", url)
     try:
         tmpfile, httpmsg = urllib.request.urlretrieve(url)
     except urllib.error.HTTPError as err:
         _errormsg(f"Error while trying to download url: {url}")
         raise err
 
     if not os.path.exists(tmpfile):
         raise RuntimeError(f"Error downloading file {url}")
     baseoutfile = os.path.split(url)[1]
     path = Path(tmpfile).parent / baseoutfile
     shutil.move(tmpfile, path.as_posix())
-    register.downloaded_files[url] = path
+    _session.downloaded_files[url] = path
     return path
 
 
 def _is_arm64():
     return os.uname()[4].startswith("arm")
 
 
-def default_system_plugins_path(major=6, minor=0) -> List[Path]:
+def default_system_plugins_path(major=6, minor=0) -> list[Path]:
     platform = _get_platform()
 
     if platform == 'linux':
         possible_dirs = [f"/usr/local/lib/csound/plugins64-{major}.{minor}",
                          f"/usr/lib/csound/plugins64-{major}.{minor}",
                          f"/usr/lib/x86_64-linux-gnu/csound/plugins64-{major}.{minor}"]
         if _is_arm64():
@@ -1222,15 +1395,14 @@
             # https://packages.debian.org/bullseye/armhf/libcsound64-6.0/filelist
             possible_dirs.append(f"/usr/lib/arm-linux-gnueabihf/csound/plugins64-{major}.{minor}/")
     elif platform == 'macos':
         # The path based on ~ is used when csound is compiled from source.
         # We give that priority since if a user is doing that, it is probably someone who knows
         # what she is doing
         MAC_CSOUNDLIB = 'CsoundLib64'
-        # API_VERSION = '6.0'
         API_VERSION = f'{major}.{minor}'
         HOME = os.getenv("HOME")
         possible_dirs = [
             f"/usr/local/opt/csound/Frameworks/{MAC_CSOUNDLIB}.framework/Versions/{API_VERSION}/Resources/Opcodes64",
             f"{HOME}/Library/Frameworks/{MAC_CSOUNDLIB}.framework/Versions/{API_VERSION}/Resources/Opcodes64",
             f"/Library/Frameworks/{MAC_CSOUNDLIB}.framework/Versions/{API_VERSION}/Resources/Opcodes64",
             f"/usr/local/lib/csound/plugins64-{API_VERSION}",
@@ -1244,16 +1416,16 @@
 
 
 def system_plugins_path() -> Optional[Path]:
     """
     Get the path were system plugins are installed.
     """
 
-    if (out:=register.cache.get('system_plugins_path', _UNSET)) is _UNSET:
-        register.cache['system_plugins_path'] = out = _system_plugins_path()
+    if (out := _session.cache.get('system_plugins_path', _UNSET)) is _UNSET:
+        _session.cache['system_plugins_path'] = out = _system_plugins_path()
     return out
 
 
 def _system_plugins_path(majorversion=6) -> Optional[Path]:
     # first check if the user has set OPCODE6DIR64
     opcode6dir64 = os.getenv(f"OPCODE{majorversion}DIR64")
     if opcode6dir64:
@@ -1265,49 +1437,50 @@
     if not out:
         _errormsg(f"System plugins path not found! Searched paths: {possible_paths}")
         return None
     assert out.exists() and out.is_dir() and out.is_absolute()
     return out
 
 
-def user_installed_dlls(majorversion=6) -> List[Path]:
+def user_installed_dlls(majorversion=6) -> list[Path]:
     """
     Return a list of plugins installed at the user plugin path.
     """
-    if (out := register.cache.get('user_installed_dlls', _UNSET)) is _UNSET:
+    if (out := _session.cache.get('user_installed_dlls', _UNSET)) is _UNSET:
         path = user_plugins_path(majorversion=majorversion)
         out = list(path.glob("*" + _plugin_extension())) if path and path.exists() else []
-        register.cache['user_installed_dlls'] = out
+        _session.cache['user_installed_dlls'] = out
     return out
 
 
-def system_installed_dlls() -> List[Path]:
+def system_installed_dlls() -> list[Path]:
     """
     LIst of plugins installed at the system's path
     """
-    if (out := register.cache.get('system_installed_dlls')) is None:
+    if (out := _session.cache.get('system_installed_dlls')) is None:
         path = system_plugins_path()
         out = list(path.glob("*" + _plugin_extension())) if path and path.exists() else []
-        register.cache['system_installed_dlls'] = out
+        _session.cache['system_installed_dlls'] = out
     return out
 
 
 class MainIndex:
     """
     This class holds risset's main index
     """
-    def __init__(self, datarepo: Path = None, update=False, majorversion: int | None = None):
+    def __init__(self, datarepo: Path = None, update=False, majorversion: Optional[int] = None):
         """
         Args:
             datarepo: the local path to clone the git main index repository to
             update: if True, update index prior to parsing
         """
         if majorversion is None:
-            major, minor = _csound_version()
-            if not major == 6 or major == 7:
+            # major, minor = _csound_version()
+            major, minor = _csoundlib_version()
+            if not (major == 6 or major == 7):
                 raise RuntimeError(f"Csound version {major}.{minor} not supported")
             majorversion = major
 
         if datarepo is None:
             datarepo = RISSET_ROOT / 'risset-data'
         else:
             assert isinstance(datarepo, Path)
@@ -1321,23 +1494,23 @@
         assert _is_git_repo(datarepo)
         assert self.indexfile.exists(), f"Main index file not found, searched: {self.indexfile}"
 
         self.datarepo: Path = datarepo
 
         self.majorversion: int = majorversion
 
-        self.pluginsources: Dict[str, IndexItem] = {}
-        self.plugins: Dict[str, Plugin] = {}
-        self._cache: Dict[str, Any] = {}
-        self._parse_index(updateindex=updateindex, updateplugins=update)
+        self.pluginsources: dict[str, IndexItem] = {}
+        self.plugins: dict[str, Plugin] = {}
+        self._cache: dict[str, Any] = {}
+        self._parse_index(updateindex=updateindex, updateplugins=update, stop_on_errors=False)
         self.user_plugins_path = user_plugins_path(majorversion=self.majorversion)
         if update:
             self.serialize()
 
-    def _parse_index(self, updateindex=False, updateplugins=False, fail_when_debugging=True) -> None:
+    def _parse_index(self, updateindex=False, updateplugins=False, stop_on_errors=True) -> None:
         """
         Parse the main index and each entity defined within it
 
         If there are errors for a plugin definition, this plugin is skipped and an
         error message is printed, unless fail_if_error is True, in which case the
         whole operation is cancelled
         """
@@ -1352,16 +1525,16 @@
             d = json.loads(indexstr)
         except json.JSONDecodeError as err:
             _errormsg(f"Error while parsing json index file {self.indexfile}")
             _print_with_line_numbers(indexstr)
             raise RuntimeError(f"Could not parse index file: {err}")
 
         self.version = d.get('version', '')
-        plugins = d.get('plugins', {})
-        updated = set()
+        plugins: dict[str, Plugin] = d.get('plugins', {})
+        updated: set[Path] = set()
 
         for name, plugindef in plugins.items():
             assert isinstance(name, str)
             assert isinstance(plugindef, dict)
             url = plugindef.get('url')
             if not url:
                 _errormsg(f"Invalid plugin source definition for plugin {name}: {plugindef}")
@@ -1381,24 +1554,24 @@
         if self.pluginsources:
             for name, pluginsource in self.pluginsources.items():
                 try:
                     _debug(f"Parsing plugin definition for {name}")
                     plugin = self._parse_plugin(name)
                     self.plugins[name] = plugin
                 except Exception as e:
-                    if register.debug and fail_when_debugging:
+                    if stop_on_errors:
                         raise e
                     else:
-                        _errormsg(f"Error while parsing plugin definition for {name}: {e}")
+                        _errormsg(f"Error while parsing plugin definition for '{name}': {e}")
 
     def update(self):
         """
         Update all sources and reread the index
         """
-        self._parse_index(updateindex=True, updateplugins=True, fail_when_debugging=register.debug)
+        self._parse_index(updateindex=True, updateplugins=True, stop_on_errors=_session.stop_on_errors)
         self.serialize()
 
     def build_documentation(self, dest: Path = None, buildhtml=True,  onlyinstalled=False) -> Path:
         """
         Build the documentation for the plugins indexed
 
         Arguments:
@@ -1424,35 +1597,35 @@
         pluginsource = self.pluginsources.get(pluginname)
         if pluginsource is None:
             raise KeyError(f"Plugin {pluginname} not known. Known plugins: {self.pluginsources.keys()}")
         manifestpath = pluginsource.manifest_path()
         assert manifestpath.exists()
         manifeststr = open(manifestpath).read()
         try:
-            m = json.loads(manifeststr)
+            _ = json.loads(manifeststr)
         except json.JSONDecodeError as err:
             _errormsg(f"Error while parsing plugin manifest. name={pluginname}, manifest={manifestpath}")
             _print_with_line_numbers(manifeststr)
             raise err
         return pluginsource.read_definition()
 
-    def installed_dlls(self) -> Dict[str, Tuple[Path, bool]]:
+    def installed_dlls(self) -> dict[str, tuple[Path, bool]]:
         """
         Returns a dict mapping dll name to (installed_path: str, user_installed: bool)
         """
         user_dlls = user_installed_dlls()
         system_dlls = system_installed_dlls()
         db = {}
         for dll in user_dlls:
             db[dll.name] = (dll, True)
         for dll in system_dlls:
             db[dll.name] = (dll, False)
         return db
 
-    def installed_path_for_dll(self, binary: str) -> Tuple[Optional[Path], bool]:
+    def installed_path_for_dll(self, binary: str) -> tuple[Optional[Path], bool]:
         """
         Get the installed path for a given plugin binary
 
         Returns (path to dll, user_installed). If not installed returns (None, False). A user installed
         dll has priority over system installed
 
         Args:
@@ -1463,15 +1636,15 @@
         """
         dlldb = self.installed_dlls()
         if binary in dlldb:
             path, userinstalled = dlldb[binary]
             return path, userinstalled
         else:
             _debug(f"The binary {binary} could not be found in the installed dlls. Installed dlls:")
-            if register.debug:
+            if _session.debug:
                 for dll, (path, userinstalled) in dlldb.items():
                     print(f" - {dll.ljust(28)}: {path} ", file=sys.stderr)
             return None, False
 
     def installed_manifests_path(self) -> Path:
         """
         Returns the path to were installation manifests are saved in this system
@@ -1479,15 +1652,15 @@
         Creates the path if it doesn't exist already
         """
         path = RISSET_ROOT / "installed-manifests"
         if not path.exists():
             path.mkdir(parents=True)
         return path
 
-    def installed_manifests(self) -> List[Path]:
+    def installed_manifests(self) -> list[Path]:
         """
         Return a list of all installed manifests
         """
         path = self.installed_manifests_path()
         manifests = list(path.glob("*.json"))
         return manifests
 
@@ -1505,17 +1678,20 @@
     def plugin_installed_path(self, plugin: Plugin) -> Optional[Path]:
         """
         Returns the path to the plugin's dll
 
         If the plugin is not installed or the binary is not found
         returns None
         """
-        binfile = plugin.binary_filename()
-        if not binfile:
+        binary = plugin.find_binary()
+        if not binary:
+            _debug(f"No binary found for plugin {plugin.name}")
             return None
+
+        binfile = binary.binary_filename()
         dll, user_installed = self.installed_path_for_dll(binfile)
         return dll
 
     def is_plugin_installed(self, plugin: Plugin, check=True) -> bool:
         """
         Is the given plugin installed?
 
@@ -1523,15 +1699,20 @@
         checks that the opcodes defined in the plugin are actually present
 
         Arguments:
             plugin: the plugin to query
             check: if True, we check if the opcodes declared in the plugin definition
                 are actually available
         """
-        binfile = plugin.binary_filename()
+        binary = plugin.find_binary()
+        if not binary:
+            _debug(f"No matching binary for plugin {plugin.name}")
+            return False
+
+        binfile = binary.binary_filename()
         if not binfile:
             return False
         dll, user_installed = self.installed_path_for_dll(binfile)
         if dll is None:
             return False
         return True if not check else self._check_plugin_installed(plugin)
 
@@ -1565,19 +1746,20 @@
             return None
 
     def installed_plugin_info(self, plugin: Plugin) -> Optional[InstalledPluginInfo]:
         """
         Returns an InstalledPluginInfo if found, None otherwise
         """
         _debug(f"Checking if plugin {plugin.name} is installed")
-        binfile = plugin.binary_filename()
-        if not binfile:
-            _debug(f"No binary for this platform (plugin {plugin.name} supports the "
-                   f"following platforms: {plugin.binaries.keys()})")
+        binary = plugin.find_binary()
+        if not binary:
+            _debug(f"Plugin {plugin.name} has no binary for this platform and/or csound version"
+                   f". Binaries: {plugin.binaries}")
             return None
+        binfile = binary.binary_filename()
         dll, user_installed = self.installed_path_for_dll(binfile)
         if not dll:
             # plugin is not installed
             _debug(f"plugin {plugin.name} is not installed yet")
             return None
 
         installed_version = UNKNOWN_VERSION
@@ -1593,19 +1775,19 @@
                     _errormsg(f"Could not load installation manifest for plugin {plugin.name}, skipping")
                     continue
                 installed_version = result['version']
                 installed_manifest_path = manifest
                 break
 
         out = InstalledPluginInfo(
-            name = plugin.name,
-            dllpath = dll,
-            versionstr = installed_version,
-            installed_in_system_folder = str(dll.parent) == str(system_plugins_path()),
-            installed_manifest_path = installed_manifest_path
+            name=plugin.name,
+            dllpath=dll,
+            versionstr=installed_version,
+            installed_in_system_folder=str(dll.parent) == str(system_plugins_path()),
+            installed_manifest_path=installed_manifest_path
         )
         return out
 
     def get_plugin_dll(self, plugin: Plugin) -> Path:
         """
         Returns the path to the binary as defined in the manifest
 
@@ -1617,20 +1799,20 @@
             plugin: the plugin which defines which binary to get
 
         Returns:
             the path of the binary.
         """
         assert isinstance(plugin, Plugin)
         platform = _get_platform()
-        bindef = plugin.binaries.get(platform)
+        bindef = plugin.find_binary(platform=platform)
         if not bindef:
-            defined_platforms = ", ".join(plugin.binaries.keys())
+            available = ", ".join(plugin.available_binaries())
             raise PlatformNotSupportedError(
-                f"No binary defined for platform {platform}."
-                f" Available platforms for {plugin.name}: {defined_platforms}")
+                f"No binary defined for platform {platform} / {_session.csound_version}."
+                f" Available platforms for {plugin.name}: {available}")
         # The binary defines a url / path under the "url" key. Both can be a
         # binary (a .so, .dll, .dylib file) or a .zip file. In this latter case,
         # the key "extractpath" needs to be defined, in which case it points to
         # the relative path to the binary inside the compressed file
 
         # The manifest defines a path. If it is relative, it is relative to the
         # manifest itself.
@@ -1655,15 +1837,15 @@
             try:
                 return _zip_extract_file(path, bindef.extractpath)
             except Exception as e:
                 raise RuntimeError(f"Error while extracting {bindef.extractpath} from zip {str(path)}: {e}")
         else:
             raise SchemaError(f"Suffix {path.suffix} not supported in url: {bindef.url}")
 
-    def opcodes_by_name(self) -> Dict[str, Opcode]:
+    def opcodes_by_name(self) -> dict[str, Opcode]:
         """
         Returns a dict mapping opcodename to an Opcode definition
         """
         out = self._cache.get('opcodes_by_name')
         if out:
             return out
         out = {opcode.name: opcode
@@ -1671,15 +1853,15 @@
         self._cache['opcodes_by_name'] = out
         return out
 
     def parse_manpage(self, opcode: str) -> Optional[ManPage]:
         manpage = self.find_manpage(opcode, markdown=True)
         return _manpage_parse(manpage, opcode) if manpage else None
 
-    def defined_opcodes(self) -> List[Opcode]:
+    def defined_opcodes(self) -> list[Opcode]:
         """
         Returns a list of opcodes
         """
         cached = self._cache.get('defined_opcodes')
         if cached:
             return cached
         opcodes = []
@@ -1743,19 +1925,19 @@
             shutil.copy(pluginpath.as_posix(), installpath.as_posix())
         except IOError as e:
             _debug(f"Tried to copy {pluginpath.as_posix()} to {installpath.as_posix()} but failed")
             _debug(str(e))
             return ErrorMsg("Could not copy the binary to the install path")
 
         installed_path = installpath / pluginpath.name
-        if not (installed_path).exists():
+        if not installed_path.exists():
             return ErrorMsg(f"Installation of plugin {plugin.name} failed, binary was not found in "
                             f"the expected path: {installed_path.as_posix()}")
 
-        register.cache.clear()
+        _session.cache.clear()
 
         # installation succeeded, check that it works
         if not self.is_plugin_installed(plugin, check=check):
             _debug(f"Plugin {plugin.name} does not seem to be installed")
             if not check:
                 return ErrorMsg(f"Tried to install plugin {plugin.name}, but the binary"
                                 f" is not present.")
@@ -1778,40 +1960,34 @@
         try:
             manifest_json = json.dumps(manifest, indent=True)
         except Exception as e:
             _errormsg(f"install_plugin: json error while saving manifest: {e}")
             _errormsg(f"   manifest was: \n{manifest}")
             return ErrorMsg("Error when dumping manifest to json")
 
-        binarydef = plugin.binarydef_for_platform()
+        binarydef = plugin.find_binary()
         if binarydef and binarydef.post_install_script:
             script = plugin.resolve_path(binarydef.post_install_script)
             subprocess.call(script.as_posix(), shell=True)
 
         with open(manifest_path.as_posix(), "w") as f:
             f.write(manifest_json)
         _debug(f"Saved manifest for plugin {plugin.name} to {manifest_path}")
 
         # no errors
         return None
 
-    def list_plugins_as_dict(self, installed=False, allplatforms=False) -> dict:
+    def list_plugins_as_dict(self, installed=False) -> dict:
         d = {}
-        platform = _get_platform()
         for plugin in self.plugins.values():
-            if platform not in plugin.binaries.keys():
-                if not allplatforms:
-                    _debug(f"Plugin {plugin.name} has no binary for platform {platform}")
-                    _debug("    To include it in the list, use allplatforms")
-                    continue
             info = self.installed_plugin_info(plugin)
             plugininstalled = info is not None
             if installed and not plugininstalled:
                 continue
-            plugdict: Dict[str, Any] = {}
+            plugdict: dict[str, Any] = {}
             plugdict['version'] = plugin.version
             if info:
                 plugdict['installed'] = True
                 plugdict['installed-version'] = info.versionstr
                 plugdict['path'] = info.dllpath.as_posix()
             else:
                 plugdict['installed'] = False
@@ -1819,40 +1995,34 @@
             plugdict['url'] = plugin.url
             plugdict['short_description'] = plugin.short_description
             plugdict['long_description'] = plugin.long_description
             plugdict['author'] = plugin.author
             d[plugin.name] = plugdict
         return d
 
-    def list_plugins(self, installed=False, nameonly=False, allplatforms=False,
-                     leftcolwidth=20, oneline=False, upgradable=False):
-        platform = _get_platform()
+    def list_plugins(self, installed=False, nameonly=False, leftcolwidth=20, oneline=False, upgradeable=False):
         width, height = _termsize()
         descr_max_width = width - 36
 
-        if upgradable:
+        if upgradeable:
             installed = True
-            allplatforms = False
+
+        platform = _get_platform()
+        csoundversion = _session.csound_version
 
         for plugin in self.plugins.values():
             data = []
-            if platform not in plugin.binaries.keys():
-                if not allplatforms:
-                    _debug(f"Plugin {plugin.name} has no binary for platform {platform}")
-                    _debug("    To include it in the list, use the --all flag")
-                    continue
-                data.append("platform not supported")
             info = self.installed_plugin_info(plugin)
             plugininstalled = info is not None
 
             if not plugininstalled and installed:
                 continue
 
-            if upgradable and (not info or info.versiontuple == (0, 0, 0) or
-                               plugin.versiontuple <= info.versiontuple):
+            if upgradeable and (not info or info.versiontuple == (0, 0, 0) or
+                                plugin.versiontuple <= info.versiontuple):
                 continue
 
             if nameonly:
                 print(plugin.name)
                 continue
 
             extra_lines = []
@@ -1868,14 +2038,19 @@
                     extra_lines.append(f"Path: {info.dllpath}")
             if data:
                 status = "[" + ", ".join(data) + "]"
             else:
                 status = ""
             leftcol = f"{plugin.name} /{plugin.version}"
             descr = plugin.short_description
+            bindef = plugin.find_binary()
+            if not bindef:
+                available = ', '.join(plugin.available_binaries())
+                extra_lines.append(f"-- No binaries for {platform}/{_session.csound_version}")
+                extra_lines.append(f"   Available binaries: {available}")
             if oneline and len(descr) > descr_max_width:
                 descr = descr[:descr_max_width] + "…"
             symbol = "*" if plugininstalled else "-"
             print(f"{symbol} {leftcol.ljust(leftcolwidth)} | {descr} {status}")
             if extra_lines:
                 for line in extra_lines:
                     print(" " * leftcolwidth + f"   |   ", line)
@@ -1885,41 +2060,44 @@
         """
         Show info about a plugin
 
         Returns True on success
         """
         plugdef = self.plugins.get(pluginname)
         if plugdef is None:
-            _errormsg(f"Plugin {pluginname} unknown")
+            _errormsg(f"Plugin '{pluginname}' unknown\n"
+                      f"Known plugins: {', '.join(self.plugins.keys())}")
             return False
         info = self.installed_plugin_info(plugdef)
         print("\n"
               f"Plugin        : {plugdef.name}    \n"
               f"Author        : {plugdef.author} ({plugdef.email}) \n"
               f"URL           : {plugdef.url}     \n"
               f"Version       : {plugdef.version} \n"
-              f"Csound version: >= {plugdef.csound_version}"
-        )
+              )
         if info:
+            manifest = info.installed_manifest_path.as_posix() if info.installed_manifest_path else 'No manifest (installed manually)'
             print(f"Installed     : {info.versionstr} (path: {info.dllpath.as_posix()}) \n"
-                  f"Manifest      : {info.installed_manifest_path.as_posix() if info.installed_manifest_path else 'No manifest (installed manually)'}")
+                  f"Manifest      : {manifest}")
         print(f"Abstract      : {plugdef.short_description}")
         if plugdef.long_description.strip():
             print("Description:")
             for line in textwrap.wrap(plugdef.long_description, 72):
                 print(" " * 3, line)
             # print(textwrap.wrapindent("     ", plugdef.long_description))
-        print("Platforms: ")
-        for platform, platform_info in plugdef.binaries.items():
-            print(f"    * {platform}: {platform_info.build_platform}")
         print(f"Opcodes:")
         opcstrs = textwrap.wrap(", ".join(plugdef.opcodes), 72)
         for s in opcstrs:
             print("   ", s)
 
+        if plugdef.binaries:
+            print("Binaries:")
+            for binary in plugdef.binaries:
+                print(f"    * {binary.platform}/csound{binary.csound_version}")
+
         if plugdef.assets:
             print("Assets:")
             for asset in plugdef.assets:
                 print(f"    * identifier: {_abbrev(asset.identifier(), 70)}\n"
                       f"      source: {asset.source}\n"
                       f"      patterns: {', '.join(asset.patterns)}\n"
                       f"      platform: {asset.platform}")
@@ -1966,15 +2144,15 @@
                 remainingassets = list(assetsfolder.glob("*"))
                 if remainingassets:
                     _info(f"There are remaining assets in the folder {assetsfolder}: {', '.join(p.as_posix() for p in remainingassets)}")
                     _info("... They will be removed")
                 _rm_dir(assetsfolder)
             os.remove(manifestpath.as_posix())
 
-    def install_asset(self, asset: Asset, prefix: str) -> List[str]:
+    def install_asset(self, asset: Asset, prefix: str) -> list[str]:
         """
         Install an Asset under a given prefix
 
         Args:
             asset: the Asset to install
             prefix: the prefix to install it under.
 
@@ -2018,14 +2196,15 @@
             ...
           </category>
           ...
         </opcodes>
         """
         lines =  []
         indentwidth = 2
+
         def _(s, indent=0):
             if indent > 0:
                 s = (" "*(indent*indentwidth)) + s
             lines.append(s)
 
         _('<?xml version="1.0" encoding="UTF-8"?>')
         _('<opcodes>')
@@ -2052,15 +2231,14 @@
                     _(f"<synopsis>{syntax}</synopsis>", 3)
                 _("</opcode>", 2)
             _('</category>', 1)
         _('</opcodes>')
         return "\n".join(lines)
 
 
-
 ###############################################################
 #                        Documentation                        #
 ###############################################################
 
 
 def _is_package_installed(pkg: str) -> bool:
     import importlib.util
@@ -2105,15 +2283,15 @@
         open(opcodesxml, "w").write(xmlstr)
 
     if buildhtml:
         mkdocsconfig = RISSET_DATAREPO_LOCALPATH / "assets" / "mkdocs.yml"
         if not mkdocsconfig.exists():
             raise IOError(f"Did not find mkdocs configuration file. Searched: {mkdocsconfig}")
         if not _is_mkdocs_installed():
-            raise RuntimeError("mkdocs is needed to build the html documentation")
+            raise RuntimeError("mkdocs is needed to build the html documentation. Install it via 'pip install mkdocs'")
         shutil.copy(mkdocsconfig, dest)
         _call_mkdocs(dest, "build")
 
     return dest
 
 
 def _compile_docs(index: MainIndex, dest: Path, makeindex=True,
@@ -2231,15 +2409,15 @@
     """
     Generate an index for the documentation
 
     Arguments:
         index: the main index
         outfile: the path to write the index to (normally an index.md file)
     """
-    lines: List[str] = []
+    lines: list[str] = []
     _ = lines.append
     _("# Plugins\n")
     plugins = sorted(index.plugins.values(), key=lambda plugin: plugin.name)
     for plugin in plugins:
         _(f"## {plugin.name}\n")
         _(plugin.short_description + '\n')
         opcodes = sorted(plugin.opcodes)
@@ -2265,24 +2443,23 @@
 
 
 def cmd_list(mainindex: MainIndex, args) -> None:
     """
     Lists all plugins available for download
     """
     if args.json:
-        d = mainindex.list_plugins_as_dict(installed=args.installed, allplatforms=args.all)
+        d = mainindex.list_plugins_as_dict(installed=args.installed)
         if args.outfile:
             with open(args.outfile, "w") as f:
                 json.dump(d, f, indent=2)
         else:
             print(json.dumps(d, indent=2))
     else:
-        mainindex.list_plugins(installed=args.installed, nameonly=args.nameonly,
-                               allplatforms=args.all, oneline=args.oneline,
-                               upgradable=args.upgradable)
+        mainindex.list_plugins(installed=args.installed, nameonly=args.nameonly, oneline=args.oneline,
+                               upgradeable=args.upgradeable)
 
 
 def cmd_show(index: MainIndex, args) -> bool:
     """
     Returns True on success
     """
     return index.show_plugin(args.plugin)
@@ -2293,15 +2470,15 @@
     Remove a plugin
     """
     errors = 0
     for pluginname in args.plugin:
         plugdef = index.plugins.get(pluginname)
         if not plugdef:
             _errormsg(f"Plugin {pluginname} not defined. Known plugins: {', '.join(index.plugins.keys())}")
-            errors +=1
+            errors += 1
             continue
         try:
             index.uninstall_plugin(plugdef)
         except Exception as e:
             _errormsg(str(e))
             errors += 1
     return errors == 0
@@ -2319,15 +2496,15 @@
 
     Flags:
         --force  - force installation even if plugin is already installed
 
     Args:
         plugin   - name of the plugin to install
     """
-    allplugins: List[Plugin] = []
+    allplugins: list[Plugin] = []
     for pattern in args.plugins:
         matched = [plugin for name, plugin in index.plugins.items()
                    if fnmatch.fnmatch(name, pattern)]
         if matched:
             allplugins.extend(matched)
     if not allplugins:
         _errormsg("No plugins matched")
@@ -2349,15 +2526,15 @@
             if plugin.versiontuple <= plugininfo.versiontuple:
                 _debug(f"Plugin {plugin.name}, version: {plugin.version}")
                 _debug(f"    Installed version: {plugininfo.versionstr}")
                 _info(f"Installed version of plugin {plugin.name} is up-to-date")
                 errors_found = True
                 continue
             _info(f"Updating plugin {plugin.name}: "
-                 f"{plugininfo.versionstr} -> {plugin.version}")
+                  f"{plugininfo.versionstr} -> {plugin.version}")
         error = index.install_plugin(plugin)
         if error:
             _debug(f"Errors while installing {plugin.name}")
             _errormsg(error)
     return False if errors_found else True
 
 
@@ -2386,15 +2563,15 @@
     Flags:
         --html      - Use .html file instead of .md version
         --path      - Do not open manpage, only print the path
         --external  - Open file in external app. This is only used when opening the markdown page. Without this
                       the markdown is output to the terminal
         opcode      - opcode(s) to get manpage of. Can be a wildcard
     """
-    opcodes: List[Opcode] = []
+    opcodes: list[Opcode] = []
     if args.html and not args.markdown:
         fmt = "html"
     else:
         fmt = "markdown"
     for pattern in args.opcode:
         opcodes.extend(opcode for opcode in idx.defined_opcodes()
                        if fnmatch.fnmatch(opcode.name, pattern))
@@ -2404,15 +2581,15 @@
         if not htmlidx.exists():
             _errormsg(f"Index file for the documentation not found (path: {htmlidx.as_posix()}")
             return False
         _open_in_default_application(htmlidx.as_posix())
     else:
         for opcode in opcodes:
             _debug("man: processing opcode ", opcode.name)
-            path = idx.find_manpage(opcode=opcode.name, markdown=fmt=="markdown")
+            path = idx.find_manpage(opcode=opcode.name, markdown=fmt == "markdown")
             if not path:
                 _errormsg(f"No manpage for opcode {opcode.name}")
                 continue
             if args.path:
                 # just print the path
                 print(f"{opcode.name}:{str(path)}")
             elif args.simplepath:
@@ -2450,14 +2627,15 @@
         for opcode in plugins_index.defined_opcodes():
             print(f"{opcode.name.ljust(20)}{opcode.plugin.ljust(12)}{_abbrev(opcode.abstract, 60)}")
     else:
         for opcode in plugins_index.defined_opcodes():
             print(opcode.name)
     return True
 
+
 def cmd_dev(idx: MainIndex, args) -> bool:
     if args.cmd == 'opcodesxml':
         outstr = idx.generate_opcodes_xml()
         if args.outfile:
             open(args.outfile, "w").write(outstr)
         else:
             print(outstr)
@@ -2483,14 +2661,15 @@
         _errormsg(str(e))
         return False
 
     _info(f"Documentation generated in {outfolder}")
     _info(f"Saved opcodes.xml to {opcodesxmlpath}")
     return True
 
+
 def cmd_info(idx: MainIndex, args) -> bool:
     picklefile = _MAININDEX_PICKLE_FILE
     if not picklefile.exists():
         lastupdate = 99999999
     else:
         import time
         lastupdate = int((time.time() - picklefile.stat().st_mtime) / 686400)
@@ -2584,28 +2763,28 @@
     def flag(parser, flag, help=""):
         parser.add_argument(flag, action="store_true", help=help)
 
     # Main parser
     parser = argparse.ArgumentParser()
     flag(parser, "--debug", help="Print debug information")
     flag(parser, "--update", help="Update the plugins data before any action")
+    flag(parser, "--stoponerror", help="Stop parsing if an error is detected")
+    flag(parser, "--version", help="Print version and exit")
     parser.add_argument("-c", "--csound", help="Which csound version to use (one of 0, 6, 7). Use 0 to detect the installed version",
                          default=0, type=int, )
 
-    flag(parser, "--version")
     subparsers = parser.add_subparsers(dest='command')
 
     # List command
     list_cmd = subparsers.add_parser('list', help="List packages")
 
     flag(list_cmd, "--json", help="Outputs list as json")
-    flag(list_cmd, "--all", "List all plugins, even those without a binary for the current platform")
     flag(list_cmd, "--nameonly", help="Output just the name of each plugin")
     flag(list_cmd, "--installed", help="List only installed plugins")
-    flag(list_cmd, "--upgradable", help="List only installed packages which can be upgraded")
+    flag(list_cmd, "--upgradeable", help="List only installed packages which can be upgraded")
     flag(list_cmd, "--notinstalled", help="List only plugins which are not installed")
     list_cmd.add_argument("-o", "--outfile", help="Outputs to a file")
     list_cmd.add_argument("-1", "--oneline", action="store_true", help="List each plugin in one line")
     list_cmd.set_defaults(func=cmd_list)
 
     # Install command
     install_cmd = subparsers.add_parser("install", help="Install or update a package")
@@ -2623,33 +2802,33 @@
     # show command
     show_cmd = subparsers.add_parser("show", help="Show information about a plugin")
     show_cmd.add_argument("plugin", help="Plugin to gather information about")
     show_cmd.set_defaults(func=cmd_show)
 
     # build docs
     makedocs_cmd = subparsers.add_parser("makedocs", help="Build the documentation for all defined plugins. "
-                                                            "This depends on mkdocs being installed")
+                                                          "This depends on mkdocs being installed")
     makedocs_cmd.add_argument("--onlyinstalled", action="store_true", help="Build docs only for installed plugins")
     makedocs_cmd.add_argument("-o", "--outfolder", help="Destination folder to place the documentation",
-                                default='')
+                              default='')
     makedocs_cmd.set_defaults(func=cmd_makedocs)
 
     # man command
     man_cmd = subparsers.add_parser("man", help="Open manual page for an installed opcode. "
                                                 "Multiple opcodes or a glob wildcard are allowed")
     man_cmd.add_argument("-p", "--path", action="store_true",
                          help="Only print the path of the manual page. The format is <opcode>:<path>, allowing to "
                               "query the path for multiple opcodes")
     man_cmd.add_argument("-s", "--simplepath", action="store_true",
                          help="Print just the path of the manual page")
     man_cmd.add_argument("-m", "--markdown", action="store_true",
                          help="Use the .md page instead of the .html version")
     man_cmd.add_argument("-e", "--external", action="store_true",
                          help="Open the man page in the default app. This is only"
-                                " used when opening the markdown man page.")
+                              " used when opening the markdown man page.")
     man_cmd.add_argument("--html", action="store_true",
                          help="Opens the .html version of the manpage in the default browser (or outputs the path"
                               " with the --path option)")
     man_cmd.add_argument("--theme", default="dark",
                          choices=['dark', 'light', 'gruvbox-dark', 'gruvbox-light', 'material', 'fruity', 'native'],
                          help="Style used when displaying markdown files (default=dark)")
     man_cmd.add_argument("opcode", nargs="*",
@@ -2685,45 +2864,46 @@
     dev_cmd = subparsers.add_parser("dev", help="Commands for developer use")
     dev_cmd.add_argument("--outfile", default=None,
                          help="Set the output file for any action generating output")
     dev_cmd.add_argument("cmd", choices=["opcodesxml"],
                          help="Subcommand. opcodesxml: generate xml output similar to opcodes.xml in the csound's manual")
     dev_cmd.set_defaults(func=cmd_dev)
 
-
     args = parser.parse_args()
-    register.debug = args.debug
+    _session.debug = args.debug
+    _session.stop_on_errors = args.stoponerror
 
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if not args.command:
         parser.print_help()
         sys.exit(-1)
     elif args.command == 'resetcache':
         cmd_resetcache(args)
         sys.exit(0)
 
     update = args.update or args.command == 'update'
+
     if args.csound == 0:
         csoundversion, minor = _csound_version()
     else:
         csoundversion = args.csound
 
     try:
         _debug(f"Creating main index - csound major version: {csoundversion}")
         if not update:
             mainindex = _mainindex_retrieve() or MainIndex(update=False, majorversion=csoundversion)
         else:
             # this will serialize the mainindex
             mainindex = MainIndex(update=True, majorversion=csoundversion)
     except Exception as e:
         _debug("Failed to create main index")
-        if register.debug:
+        if _session.debug:
             raise e
         else:
             _errormsg(str(e))
             sys.exit(-1)
 
     if args.command == 'update':
         sys.exit(0)
```

### Comparing `risset-2.1.1/setup.py` & `risset-2.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     author_email = "eduardo.moguillansky@gmail.com",
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     py_modules=["risset"],
 
     url="https://github.com/csound-plugins/risset",
 
-    install_requires=['mkdocs', 'pygments'],
+    install_requires=[
+        'pygments',
+        'ctcsound7>=0.3.0'
+    ],
 
     entry_points={
         "console_scripts": [
             "risset=risset:main",
         ]
     }
 )
```

