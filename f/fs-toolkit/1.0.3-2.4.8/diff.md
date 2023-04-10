# Comparing `tmp/fs_toolkit-1.0.3.tar.gz` & `tmp/fs_toolkit-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_toolkit-1.0.3.tar", max compression
+gzip compressed data, was "fs_toolkit-2.4.8.tar", max compression
```

## Comparing `fs_toolkit-1.0.3.tar` & `fs_toolkit-2.4.8.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      663 2022-11-11 03:29:16.357925 fs_toolkit-1.0.3/LICENSE
--rw-r--r--   0        0        0      872 2022-12-24 07:03:18.454182 fs_toolkit-1.0.3/README.md
--rw-r--r--   0        0        0       83 2022-11-11 03:45:03.217325 fs_toolkit-1.0.3/fs_toolkit/__init__.py
--rw-r--r--   0        0        0     1902 2022-11-13 07:47:33.344218 fs_toolkit-1.0.3/fs_toolkit/base.py
--rw-r--r--   0        0        0      141 2022-11-11 03:33:37.421770 fs_toolkit-1.0.3/fs_toolkit/exceptions.py
--rw-r--r--   0        0        0       92 2022-11-12 19:50:47.640512 fs_toolkit-1.0.3/fs_toolkit/fstab/__init__.py
--rw-r--r--   0        0        0      309 2022-11-13 07:27:48.251713 fs_toolkit-1.0.3/fs_toolkit/fstab/constants.py
--rw-r--r--   0        0        0     6879 2022-11-15 18:00:07.019706 fs_toolkit-1.0.3/fs_toolkit/fstab/loader.py
--rw-r--r--   0        0        0        0 2022-11-11 03:41:41.222264 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/__init__.py
--rw-r--r--   0        0        0        0 2022-11-11 03:44:24.570511 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/base.py
--rw-r--r--   0        0        0        0 2022-11-11 03:43:40.451101 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/bsd.py
--rw-r--r--   0        0        0        0 2022-11-11 03:43:40.451253 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/darwin.py
--rw-r--r--   0        0        0        0 2022-11-11 03:43:40.451343 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/linux.py
--rw-r--r--   0        0        0     1278 2022-11-15 17:45:13.634911 fs_toolkit-1.0.3/fs_toolkit/fstab/platform/openbsd.py
--rw-r--r--   0        0        0      108 2022-11-12 19:50:38.741266 fs_toolkit-1.0.3/fs_toolkit/mounts/__init__.py
--rw-r--r--   0        0        0     2001 2022-11-12 15:08:20.662737 fs_toolkit-1.0.3/fs_toolkit/mounts/constants.py
--rw-r--r--   0        0        0     4156 2022-11-12 19:58:45.768368 fs_toolkit-1.0.3/fs_toolkit/mounts/loader.py
--rw-r--r--   0        0        0       61 2022-11-11 03:29:42.650348 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/__init__.py
--rw-r--r--   0        0        0     2897 2022-11-12 15:21:26.143982 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/base.py
--rw-r--r--   0        0        0     1630 2022-11-12 15:12:00.508101 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/bsd.py
--rw-r--r--   0        0        0      896 2022-11-11 03:29:42.650812 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/darwin.py
--rw-r--r--   0        0        0     1113 2022-11-11 03:29:42.651196 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/linux.py
--rw-r--r--   0        0        0      893 2022-11-11 03:29:42.649822 fs_toolkit-1.0.3/fs_toolkit/mounts/platform/openbsd.py
--rw-r--r--   0        0        0      911 2022-12-24 06:58:27.279798 fs_toolkit-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 fs_toolkit-1.0.3/setup.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fs_toolkit-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-07 06:52:58.668554 fs_toolkit-2.4.8/LICENSE
+-rw-r--r--   0        0        0      872 2022-12-24 07:03:18.454182 fs_toolkit-2.4.8/README.md
+-rw-r--r--   0        0        0      278 2023-03-18 08:10:02.537454 fs_toolkit-2.4.8/fs_toolkit/__init__.py
+-rw-r--r--   0        0        0     2209 2023-03-08 06:02:20.132140 fs_toolkit-2.4.8/fs_toolkit/base.py
+-rw-r--r--   0        0        0      244 2023-03-07 06:58:09.380541 fs_toolkit-2.4.8/fs_toolkit/exceptions.py
+-rw-r--r--   0        0        0      194 2023-03-18 11:31:52.089421 fs_toolkit-2.4.8/fs_toolkit/fstab/__init__.py
+-rw-r--r--   0        0        0      411 2023-03-07 06:56:08.859643 fs_toolkit-2.4.8/fs_toolkit/fstab/constants.py
+-rw-r--r--   0        0        0     6145 2023-03-18 11:55:41.662177 fs_toolkit-2.4.8/fs_toolkit/fstab/loader.py
+-rw-r--r--   0        0        0      143 2023-03-07 06:55:07.084543 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/__init__.py
+-rw-r--r--   0        0        0     4548 2023-03-18 08:29:31.021207 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/base.py
+-rw-r--r--   0        0        0      404 2023-03-18 11:55:41.665251 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/bsd.py
+-rw-r--r--   0        0        0      425 2023-03-08 15:10:41.108944 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/darwin.py
+-rw-r--r--   0        0        0      414 2023-03-08 15:10:34.944635 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/linux.py
+-rw-r--r--   0        0        0     1667 2023-03-08 15:10:20.638061 fs_toolkit-2.4.8/fs_toolkit/fstab/platform/openbsd.py
+-rw-r--r--   0        0        0      210 2023-03-18 08:09:42.372458 fs_toolkit-2.4.8/fs_toolkit/mounts/__init__.py
+-rw-r--r--   0        0        0     2104 2023-03-18 11:54:49.546068 fs_toolkit-2.4.8/fs_toolkit/mounts/constants.py
+-rw-r--r--   0        0        0     4483 2023-03-18 11:55:41.669721 fs_toolkit-2.4.8/fs_toolkit/mounts/loader.py
+-rw-r--r--   0        0        0      164 2023-03-07 06:57:18.575753 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/__init__.py
+-rw-r--r--   0        0        0     3742 2023-03-08 06:03:26.733364 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/base.py
+-rw-r--r--   0        0        0     2008 2023-03-18 11:55:41.671889 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/bsd.py
+-rw-r--r--   0        0        0      998 2023-03-18 11:55:41.674116 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/darwin.py
+-rw-r--r--   0        0        0     1288 2023-03-09 20:34:56.973398 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/linux.py
+-rw-r--r--   0        0        0      995 2023-03-18 11:55:41.676130 fs_toolkit-2.4.8/fs_toolkit/mounts/platform/openbsd.py
+-rw-r--r--   0        0        0      968 2023-03-07 06:53:22.741731 fs_toolkit-2.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 fs_toolkit-2.4.8/PKG-INFO
```

### Comparing `fs_toolkit-1.0.3/README.md` & `fs_toolkit-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fs_toolkit-1.0.3/fs_toolkit/base.py` & `fs_toolkit-2.4.8/fs_toolkit/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,56 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Common base class for line parser output data classes
 """
 import re
 
-from typing import List
+from typing import Iterator, List, Optional
 
 from sys_toolkit.collection import CachedMutableSequence
 from sys_toolkit.platform import detect_platform_family, detect_toolchain_family
 
 
 class LineLoader(CachedMutableSequence):
     """
     Loader for line based data to cached mutable sequence
     """
+    __platform__: str
+    __toolchain__: str
+    __iter_items__: Optional[Iterator[str]]
+
     def __init__(self) -> None:
         super().__init__()
         self.__platform__ = detect_platform_family()
         self.__toolchain__ = detect_toolchain_family()
         self.__iter_items__ = None
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         if not self.__loaded__:
             self.update()
         return iter(self.__items__)
 
-    def __next__(self):
+    def __next__(self) -> str:
         if self.__iter_items__ is None:
             if not self.__loaded__:
                 self.update()
             self.__iter_items__ = iter(self.__items__)
         try:
             return next(self.__iter_items__)
         except StopIteration as error:
             self.__iter_items__ = None
             raise StopIteration from error
 
-    def __match_pattern_list__(self, lines: List[str], patterns: List[re.Pattern]) -> List[dict]:
+    def __match_pattern_list__(self,
+                               lines: List[str],
+                               patterns: List[re.Pattern]) -> List[dict]:
         """
         Match lines to list of grouped regexp patterns, returning list
         of regexp groupdict matches.
 
         Lines must be iterable of strings and iterable of re.Pattern
         """
         assert isinstance(patterns, list)
@@ -51,12 +62,12 @@
             for pattern in patterns:
                 match = pattern.match(line)
                 if match:
                     matches.append(match.groupdict())
                     break
         return matches
 
-    def update(self):
+    def update(self) -> None:
         """
         Require update to be implemented in child class
         """
         raise NotImplementedError
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/fstab/platform/openbsd.py` & `fs_toolkit-2.4.8/fs_toolkit/fstab/platform/openbsd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,49 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
-Platform specific code to handle fstab devices on OpenBSD
+Platform specific code to handle fstab devices on OpenOpenBSD
 """
 from pathlib import Path
 from typing import Optional
 
 from sys_toolkit.collection import CachedMutableMapping
 from sys_toolkit.subprocess import run_command
 
+from .base import FstabComment, FstabEntry
+
+
+# pylint: disable=too-few-public-methods
+class OpenBSDFstabComment(FstabComment):
+    """
+    OpenBSD specific class for fstab entries
+    """
+
+
+class OpenBSDFstabEntry(FstabEntry):
+    """
+    OpenBSD specific class for fstab entries
+    """
+
 
 class DuidMap(CachedMutableMapping):
     """
-    OpenBSD Disklabel Unique Identifiers (DUIDs) mapping to device names
+    OpenOpenBSD Disklabel Unique Identifiers (DUIDs) mapping to device names
     """
     def __get_sysctl_output__(self) -> str:
         """
         Get the sysctl output lines
         """
         stdout, _stderr = run_command(*('sysctl', '-n', 'hw.disknames'))
         return [str(line, 'utf-8') for line in stdout.splitlines()]
 
-    def update(self, other=(), /, **kwds):
+    def update(self, **kwargs):
         """
         Update DUID map values
         """
         self.__items__ = {}
         self.__start_update__()
         for item in self.__get_sysctl_output__()[0].split(','):
             device, duid = item.split(':', 1)
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/constants.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Constants for parsing OS family specific mount and usage line outputs
 """
 import re
 
 GNU_MOUNT_COMMAND = ('mount',)
 # Patterns to match lines from GNU based 'mount' command
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/loader.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Mountpoints loader main class MountPoints()
 """
-from typing import List
+from re import Pattern
+from typing import List, Optional, Tuple
 
 from sys_toolkit.subprocess import run_command
 
 from ..base import LineLoader
 from ..exceptions import FilesystemError
 from .platform.base import Mountpoint
 from .platform.bsd import BSDMountpoint
@@ -26,41 +32,42 @@
 )
 
 
 class Mountpoints(LineLoader):
     """
     Filesystem mount points with usage
     """
-    __mount_command__ = None
-    __df_command__ = None
-    __re_mount_patterns__ = None
-    __re_df_patterns__ = None
+    __mountpoint_class__: Mountpoint
+    __mount_command__: Tuple[str] = None
+    __df_command__: Tuple[str] = None
+    __re_mount_patterns__: Optional[List[Pattern]] = None
+    __re_df_patterns__: Optional[List[Pattern]] = None
 
     def __init__(self):
         super().__init__()
         self.__detect_mountpoint_class__()
         self.__initialize_toolchain_based_data__()
         self.__iter_items__ = None
 
-    def __detect_mountpoint_class__(self):
+    def __detect_mountpoint_class__(self) -> None:
         """
         Detect mountpoint loader class based on platform family
         """
         if self.__platform__ == 'bsd':
             self.__mountpoint_class__ = BSDMountpoint
         elif self.__platform__ == 'darwin':
             self.__mountpoint_class__ = DarwinMountPoint
         elif self.__platform__ == 'linux':
             self.__mountpoint_class__ = LinuxMountPoint
         elif self.__platform__ == 'openbsd':
             self.__mountpoint_class__ = OpenBSDMountPoint
         else:
             raise FilesystemError(f'Unsupported OS platform: {self.__platform__}')
 
-    def __initialize_toolchain_based_data__(self):
+    def __initialize_toolchain_based_data__(self) -> None:
         """
         Initialize toolchain specific commands and regexp patterns
         """
         if self.__toolchain__ == 'bsd':
             self.__mount_command__ = BSD_MOUNT_COMMAND
             self.__df_command__ = BSD_DF_COMMAND
             self.__re_mount_patterns__ = RE_BSD_MOUNT_LINE
@@ -97,19 +104,19 @@
 
     def __get_df_data__(self, lines: List[str]) -> List[dict]:
         """
         Return lines from df command
         """
         return self.__match_pattern_list__(lines, self.__re_df_patterns__)
 
-    def append(self, value):
+    def append(self, value: Mountpoint) -> Mountpoint:
         assert isinstance(value, Mountpoint)
         return super().append(value)
 
-    def insert(self, index, value):
+    def insert(self, index: int, value: Mountpoint) -> Mountpoint:
         assert isinstance(value, Mountpoint)
         return super().insert(index, value)
 
     def update(self) -> None:
         """
         Get data for mountpoints
         """
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/platform/base.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/platform/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,140 @@
-
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+Common base classes for platform specific mounts classes
+"""
 from pathlib import Path
+from typing import List, Optional, Tuple, Union, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ..loader import Mountpoints
 
 
 # pylint: disable=too-few-public-methods
 class MountpointOptions:
     """
     Options for filesystem mount point
     """
-    def __init__(self, mountpoint, options):
+    def __init__(self,
+                 mountpoint: 'Mountpoint',
+                 options: Optional[Union[str, List[str]]]) -> None:
         self.mountpoint = mountpoint
         options = self.__parse_options__(options)
         for flag in options:
             setattr(self, flag, True)
 
     @staticmethod
-    def __parse_options__(options):
+    def __parse_options__(options: Union[str, List[str]]) -> List[str]:
         """
         Parse options from string to a list
         """
         if isinstance(options, str):
             options = options.split(', ')
         return options
 
 
 # pylint: disable=too-few-public-methods
 class MountpointUsage:
     """
-
     Mountpoint usage stats data
     """
-    def __init__(self, mountpoint):
+    mountpoint: 'Mountpoint'
+    size: Optional[int]
+    available: Optional[int]
+    used: Optional[int]
+    percent: Optional[int]
+
+    def __init__(self, mountpoint: 'Mountpoint') -> None:
         self.mountpoint = mountpoint
         self.size = None
         self.available = None
         self.used = None
         self.percent = None
 
-    def __set_value__(self, attr, value):
+    def __set_value__(self, attr: str, value: int) -> None:
         """
         Set value for usage counter
         """
         value = int(value)
         setattr(self, attr, value)
 
-    def load_data(self, data):
+    def load_data(self, data: dict) -> None:
         """
         Load usage data for mountpoint
         """
         for attr in ('size', 'available', 'used', 'percent'):
             assert attr in data
             self.__set_value__(attr, data[attr])
 
 
 # pylint: disable=too-few-public-methods
 class Filesystem:
     """
     Filesystem for a mountpoint
     """
-    virtual_filesystems = ()
+    mountpoint: 'Mountpoint'
+    name: str
+    virtual_filesystems: Tuple[str] = ()
 
-    def __init__(self, mountpoint, name):
+    def __init__(self, mountpoint: 'Mountpoint', name: str) -> None:
         self.mountpoint = mountpoint
         self.name = name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.name
 
     @property
-    def is_virtual(self):
+    def is_virtual(self) -> bool:
         """
         Return True if filesystem is a virtual filesystem
         """
         return self.name in self.virtual_filesystems
 
 
 class Mountpoint:
     """
     Filesystem mount point linked to Mountpoints
     """
-    filesystem_class = Filesystem
-    options_class = MountpointOptions
-    usage_class = MountpointUsage
+    mountpoints: 'Mountpoints'
+    filesystem_class: Filesystem
+    options_class: MountpointOptions
+    usage_class: MountpointUsage
 
     def __init__(self,
-                 mountpoints,
-                 device,
-                 mountpoint,
-                 filesystem=None,
-                 options=None):
-
+                 mountpoints: 'Mountpoints',
+                 device: str,
+                 mountpoint: str,
+                 filesystem: Optional[str] = None,
+                 options: Optional[Union[str, List[str]]] = None):
         self.mountpoints = mountpoints
         self.device = device
         self.mountpoint = mountpoint
         self.filesystem = self.filesystem_class(self, filesystem)
         self.options = self.options_class(self, options)
         self.usage = self.usage_class(self)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.device} mounted on {self.mountpoint}'
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
-        Return basename of mountpoint
+        Return basename of mountpoint as string
         """
         return Path(self.mountpoint).name
 
     @property
-    def is_virtual(self):
+    def is_virtual(self) -> bool:
         """
         Check if filesystem is virtual
         """
         return self.filesystem.is_virtual
 
-    def load_usage_data(self, data):
+    def load_usage_data(self, data: dict) -> None:
         """
         Load filesystem usage data for mountpoint
         """
         self.usage.load_data(data)
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/platform/bsd.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/platform/bsd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,57 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Generic BSD mountpoints (FreeBSD, MacOS)
 """
-
+from typing import List, Optional, Union
 from .base import Mountpoint, Filesystem, MountpointOptions, MountpointUsage
 
 BSD_VIRTUAL_FILESYSTEMS = (
     'devfs',
     'procfs',
 )
 
 
 # pylint: disable=too-few-public-methods
 class BSDMountpointUsage(MountpointUsage):
     """
     BSD specific mountpoint usage data
     """
-    def __init__(self, mountpoint):
+    inodes_used: Optional[int]
+    inodes_available: Optional[int]
+    inodes_percent: Optional[int]
+
+    def __init__(self, mountpoint: 'BSDMountpoint') -> None:
         super().__init__(mountpoint)
         self.inodes_used = None
         self.inodes_available = None
         self.inodes_percent = None
 
-    def load_data(self, data):
+    def load_data(self, data: dict) -> None:
         """
         Load BSD specific filesystem usage data
         """
         super().load_data(data)
         for attr in ('inodes_used', 'inodes_available', 'inodes_percent'):
             if attr in data:
                 self.__set_value__(attr, data[attr])
 
 
 # pylint: disable=too-few-public-methods
 class BSDMountPointOptions(MountpointOptions):
     """
     BSD specific mountpoint options
     """
-    def __init__(self, mountpoint, options=None):
+    def __init__(self,
+                 mountpoint: 'BSDMountpoint',
+                 options: Optional[Union[str, List[str]]] = None) -> None:
         options = self.__parse_options__(options)
         filesystem = options[0]
         options = options[1:]
 
         super().__init__(mountpoint, options)
         self.mountpoint.filesystem.name = filesystem
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/platform/darwin.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/platform/darwin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 MacOS Darwin mountpoints
 """
-
 from .bsd import BSDMountpoint, BSDFilesystem, BSDMountPointOptions, BSDMountpointUsage
 
 DARWIN_VIRTUAL_FILESYSTEMS = (
     'sysfs',
 )
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/platform/linux.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/platform/linux.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,43 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Linux mountpoints
 """
 from .base import Mountpoint, Filesystem, MountpointOptions, MountpointUsage
 
 LINUX_VIRTUAL_FILESYSTEMS = (
-    'proc',
-    'sysfs',
-    'cgroup',
     'autofs',
-    'hugetlbfs',
-    'mqueue',
+    'binfmt_misc',
+    'bpf',
+    'cgroup',
+    'cgroup2',
+    'configfs',
+    'debugfs',
     'devpts',
     'devtmpfs',
-    'tmpfs',
+    'efivarfs',
     'fusectl',
+    'hugetlbfs',
+    'mqueue',
+    'nsfs',
+    'overlay',
+    'proc',
+    'procfs',
     'pstore',
-    'configfs',
-    'selinuxfs',
-    'securityfs',
-    'debugfs',
+    'ramfs',
     'rpc_pipefs',
-    'binfmt_misc',
-    'nfsd',
-    'fuse.vmware-vmblock',
+    'securityfs',
+    'selinuxfs',
+    'sysfs',
+    'tmpfs',
+    'tracefs',
 )
 
 
 # pylint: disable=too-few-public-methods
 class LinuxMountpointUsage(MountpointUsage):
     """
     Linux specific mountpoint usage data
```

### Comparing `fs_toolkit-1.0.3/fs_toolkit/mounts/platform/openbsd.py` & `fs_toolkit-2.4.8/fs_toolkit/mounts/platform/openbsd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 OpenBSD mounpoints
 """
-
 from .bsd import BSDMountpoint, BSDFilesystem, BSDMountPointOptions, BSDMountpointUsage
 
 OPENBSD_VIRTUAL_FILESYSTEMS = (
     'sysfs',
     'procfs',
 )
```

### Comparing `fs_toolkit-1.0.3/pyproject.toml` & `fs_toolkit-2.4.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "fs-toolkit"
-version = "1.0.3"
+version = "2.4.8"
 description = "Classes for filesystem usage utilities"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
+homepage = "https://github.com/hile/fs-toolkit"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
-license = "BSD"
+license = "BSD-3-Clause"
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: BSD License",
     "Operating System :: MacOS",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
```

### Comparing `fs_toolkit-1.0.3/PKG-INFO` & `fs_toolkit-2.4.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fs-toolkit
-Version: 1.0.3
+Version: 2.4.8
 Summary: Classes for filesystem usage utilities
-License: BSD
+Home-page: https://github.com/hile/fs-toolkit
+License: BSD-3-Clause
 Author: Ilkka Tuohela
 Author-email: hile@iki.fi
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

