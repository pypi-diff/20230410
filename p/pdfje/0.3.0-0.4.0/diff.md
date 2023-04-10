# Comparing `tmp/pdfje-0.3.0.tar.gz` & `tmp/pdfje-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfje-0.3.0.tar", max compression
+gzip compressed data, was "pdfje-0.4.0.tar", max compression
```

## Comparing `pdfje-0.3.0.tar` & `pdfje-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,22 @@
--rw-r--r--   0        0        0      817 2022-12-02 11:08:05.801815 pdfje-0.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2931 2022-12-02 11:04:13.666253 pdfje-0.3.0/README.rst
--rw-r--r--   0        0        0     1481 2022-12-02 11:08:00.568233 pdfje-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7242 2022-12-02 11:04:13.666582 pdfje-0.3.0/src/pdfje/__init__.py
--rw-r--r--   0        0        0     5691 2022-12-02 11:04:13.666721 pdfje-0.3.0/src/pdfje/atoms.py
--rw-r--r--   0        0        0     1071 2022-12-02 11:04:13.666840 pdfje-0.3.0/src/pdfje/common.py
--rw-r--r--   0        0        0    12709 2022-12-02 11:04:13.666988 pdfje-0.3.0/src/pdfje/fonts.py
--rw-r--r--   0        0        0        0 2022-10-26 19:42:23.131874 pdfje-0.3.0/src/pdfje/py.typed
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 pdfje-0.3.0/setup.py
--rw-r--r--   0        0        0     4044 1970-01-01 00:00:00.000000 pdfje-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1556 2023-04-10 14:21:01.064991 pdfje-0.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     4556 2023-04-10 14:21:01.065651 pdfje-0.4.0/README.rst
+-rw-r--r--   0        0        0     1458 2023-04-10 14:21:01.069311 pdfje-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2111 2023-04-10 14:21:01.107672 pdfje-0.4.0/src/pdfje/__init__.py
+-rw-r--r--   0        0        0     6345 2023-04-10 14:21:01.107957 pdfje-0.4.0/src/pdfje/atoms.py
+-rw-r--r--   0        0        0    13623 2023-04-10 14:21:01.108674 pdfje-0.4.0/src/pdfje/common.py
+-rw-r--r--   0        0        0    12675 2023-04-10 14:21:01.108836 pdfje-0.4.0/src/pdfje/document.py
+-rw-r--r--   0        0        0     8139 2023-04-10 14:21:01.108951 pdfje-0.4.0/src/pdfje/draw.py
+-rw-r--r--   0        0        0      155 2023-04-10 14:21:01.109085 pdfje-0.4.0/src/pdfje/fonts/__init__.py
+-rw-r--r--   0        0        0   407594 2023-04-10 14:21:01.109836 pdfje-0.4.0/src/pdfje/fonts/builtins.py
+-rw-r--r--   0        0        0     5994 2023-04-10 14:21:01.109999 pdfje-0.4.0/src/pdfje/fonts/common.py
+-rw-r--r--   0        0        0    13573 2023-04-10 14:21:01.110157 pdfje-0.4.0/src/pdfje/fonts/embed.py
+-rw-r--r--   0        0        0     2058 2023-04-10 14:21:01.110267 pdfje-0.4.0/src/pdfje/fonts/registry.py
+-rw-r--r--   0        0        0     1789 2023-04-10 14:21:01.110446 pdfje-0.4.0/src/pdfje/layout.py
+-rw-r--r--   0        0        0     3275 2023-04-10 14:21:01.110601 pdfje-0.4.0/src/pdfje/ops.py
+-rw-r--r--   0        0        0        0 2022-10-26 19:42:23.131874 pdfje-0.4.0/src/pdfje/py.typed
+-rw-r--r--   0        0        0     7333 2023-04-10 14:21:01.110776 pdfje-0.4.0/src/pdfje/style.py
+-rw-r--r--   0        0        0     5872 2023-04-10 14:21:01.110931 pdfje-0.4.0/src/pdfje/text.py
+-rw-r--r--   0        0        0    18193 2023-04-10 14:21:01.111118 pdfje-0.4.0/src/pdfje/typeset.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:21:01.111181 pdfje-0.4.0/src/pdfje/vendor/__init__.py
+-rw-r--r--   0        0        0    13291 2023-04-10 14:21:01.111371 pdfje-0.4.0/src/pdfje/vendor/get_kerning_pairs.py
+-rw-r--r--   0        0        0     5495 1970-01-01 00:00:00.000000 pdfje-0.4.0/PKG-INFO
```

### Comparing `pdfje-0.3.0/pyproject.toml` & `pdfje-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "pdfje"
-version = "0.3.0"
+version = "0.4.0"
 description = "Tiny PDF writer"
 authors = ["Arie Bovenberg <a.c.bovenberg@gmail.com>"]
 license = "MIT"
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 packages = [
     { include = "pdfje", from = "src" },
@@ -17,34 +16,35 @@
 documentation = "https://pdfje.readthedocs.io"
 readme = "README.rst"
 include = ["CHANGELOG.rst", "README.rst"]
 repository = "https://github.com/ariebovenberg/pdfje"
 keywords = ["pdf"]
 
 [tool.poetry.dependencies]
-python = "^3.7,<4.0"
-importlib-metadata = {version = ">=1,<5", python = "<3.8"}
-fonttools = "^4.38.0"
+python = ">=3.8.1,<4.0"
+fonttools = {version="^4.38.0", optional=true}
+
+[tool.poetry.extras]
+fonts = ["fonttools"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
 pytest-benchmark = "^4.0.0"
+hypothesis = "^6.68.2"
 
 [tool.poetry.group.typecheck.dependencies]
-mypy = "^0.982"
+mypy = "^1.0.0"
 
 [tool.poetry.group.linting.dependencies]
-black = "^22.10"
-flake8 = "^5.0.4"
+black = "^23.1"
+flake8 = "^6.0.0"
 isort = "^5.7.0"
 slotscheck = "^0.16.1"
 
-[tool.poetry.group.dev.dependencies]
-tox = "^3.26"
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
   \.eggs
@@ -62,11 +62,12 @@
 line_length = 79
 profile = 'black'
 
 [tool.slotscheck]
 strict-imports = true
 require-superclass = true
 require-subclass = true
+exclude-modules = "^pdfje\\.vendor.*"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pdfje-0.3.0/src/pdfje/atoms.py` & `pdfje-0.4.0/src/pdfje/atoms.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,57 +6,55 @@
 from functools import partial
 from itertools import accumulate, chain, repeat, starmap
 from math import isfinite
 from secrets import token_bytes
 from typing import Collection, Iterable, Iterator, Sequence
 from zlib import compress
 
-from .common import add_slots
+from .common import add_slots, setattr_frozen
 
 # PDF 32000-1:2008 (7.5.2) specifies that the header must be followed
 # immediately by a comment line containing at least 4 binary characters
 # of size 0x80 or greater.
-_HEADER = b"%PDF-1.7\n%\x80\x80\x80\x80 generated by PDFje\n"
+_HEADER = b"%PDF-1.7\n%\x80\x80\x80\x80 generated by pdf'je\n"
 _FIRST_OFFSET = len(_HEADER)
-OBJ_ID_XREF, OBJ_ID_CATALOG = 0, 1
+OBJ_ID_XREF, OBJ_ID_CATALOG, OBJ_ID_PAGETREE, OBJ_ID_RESOURCES = 0, 1, 2, 3
 ASCII = bytes
 Byte = int  # 0-255
+# ID of an object in the PDF file. Always >=0 and unique within a file.
+ObjectID = int
 
 
-class Object(abc.ABC):
+class Atom(abc.ABC):
     __slots__ = ()
 
     @abc.abstractmethod
     def write(self) -> Iterable[bytes]:
         raise NotImplementedError()
 
 
-ObjectID = int
-"""ID of an object in the PDF file. Always >=0 and unique within a file."""
-
-ObjectWithID = tuple[ObjectID, Object]
+Object = tuple[ObjectID, Atom]
 
 
 @add_slots
 @dataclass(frozen=True)
-class Bool(Object):
+class Bool(Atom):
     value: bool
 
     def write(self) -> Iterable[bytes]:
         raise NotImplementedError()
 
 
 @add_slots
 @dataclass(frozen=True)
-class Name(Object):
+class Name(Atom):
     value: ASCII
 
     def write(self) -> Iterable[bytes]:
-        yield b"/"
-        yield self.value
+        return (b"/", self.value)
 
 
 def _sanitize_name_char(c: Byte) -> bytes:
     # PDF32000-1:2008 (7.3.5) says ASCII from 33-126 is OK, except "#" (0x23)
     # which is the escape character.
     if c == 0x23:
         return b"#23"
@@ -71,172 +69,191 @@
 
 def sanitize_name(s: bytes) -> bytes:
     return b"".join(map(_sanitize_name_char, s))
 
 
 @add_slots
 @dataclass(frozen=True)
-class Int(Object):
+class Int(Atom):
     value: int
 
     def write(self) -> Iterable[bytes]:
-        yield b"%i" % self.value
+        return (b"%i" % self.value,)
 
 
 @add_slots
 @dataclass(frozen=True)
-class Real(Object):
+class Real(Atom):
     value: float
 
     def write(self) -> Iterable[bytes]:
         assert isfinite(self.value), "NaN and Inf not supported"
-        yield b"%g" % self.value
-
-
-_STRING_ESCAPES = {
-    b"\\": b"\\\\",
-    b"\n": b"\\n",
-    b"\r": b"\\r",
-    b"\t": b"\\t",
-    b"\b": b"\\b",
-    b"\f": b"\\f",
-    b"(": b"\\(",
-    b")": b"\\)",
-}
-
-
-def _replace_with_escape(m: re.Match) -> bytes:
-    return _STRING_ESCAPES[m.group()]
-
-
-escape_string = partial(
-    re.compile(b"(%b)" % b"|".join(map(re.escape, _STRING_ESCAPES))).sub,
-    _replace_with_escape,
-)
+        return (b"%g" % self.value,)
 
 
 @add_slots
 @dataclass(frozen=True)
-class LiteralString(Object):
+class LiteralString(Atom):
     value: bytes
 
+    # FUTURE: support UTF-16BOM, but in a way that makes it explicit that
+    # this does not support usage in text streams.
+    # How to prevent accidential UTF-16BOM?
     def write(self) -> Iterable[bytes]:
-        yield b"("
-        yield escape_string(self.value)
-        yield b")"
+        return (b"(", _escape(self.value), b")")
 
 
 @add_slots
 @dataclass(frozen=True)
-class HexString(Object):
+class HexString(Atom):
     value: bytes
 
     def write(self) -> Iterable[bytes]:
-        yield b"<"
-        yield hexlify(self.value)
-        yield b">"
+        return (b"<", hexlify(self.value), b">")
 
 
 @add_slots
 @dataclass(frozen=True)
-class Array(Object):
-    items: Iterable[Object]
+class Array(Atom):
+    items: Iterable[Atom]
 
     def write(self) -> Iterable[bytes]:
         yield b"["
         for i in self.items:
             yield from i.write()
             yield b" "
         yield b"]"
 
 
 @add_slots
 @dataclass(frozen=True, init=False)
-class Dictionary(Object):
-    content: Collection[tuple[ASCII, Object]]
+class Dictionary(Atom):
+    content: Collection[tuple[ASCII, Atom]]
 
-    def __init__(self, *content: tuple[ASCII, Object]) -> None:
-        object.__setattr__(self, "content", content)
+    def __init__(self, *content: tuple[ASCII, Atom]) -> None:
+        setattr_frozen(self, "content", content)
 
     def write(self) -> Iterable[bytes]:
         yield from _write_dict(self.content)
 
 
-def _write_dict(d: Iterable[tuple[ASCII, Object]]) -> Iterable[bytes]:
+def _write_dict(d: Iterable[tuple[ASCII, Atom]]) -> Iterable[bytes]:
     yield b"<<\n"
     for key, value in d:
         yield b"/"
         yield key
         yield b" "
         yield from value.write()
         yield b"\n"
     yield b">>"
 
 
 @add_slots
 @dataclass(frozen=True)
-class Stream(Object):
-    content: bytes
-    meta: Collection[tuple[ASCII, Object]] = ()
+class Stream(Atom):
+    content: Iterable[bytes]
+    meta: Collection[tuple[ASCII, Atom]] = ()
 
     def write(self) -> Iterable[bytes]:
-        content = compress(self.content)
+        content = compress(b"".join(self.content))
         yield from _write_dict(
             chain(
                 self.meta,
-                [(b"Length", Int(len(content)))],
-                [(b"Filter", Name(b"FlateDecode"))],
+                [
+                    (b"Length", Int(len(content))),
+                    (b"Filter", Name(b"FlateDecode")),
+                ],
             )
         )
         yield b"\nstream\n"
         yield content
         yield b"\nendstream"
 
 
 @add_slots
 @dataclass(frozen=True)
-class Ref(Object):
+class Ref(Atom):
     target: ObjectID
 
     def write(self) -> Iterable[bytes]:
-        yield b"%i 0 R" % self.target
+        return (b"%i 0 R" % self.target,)
 
 
-def _write_obj(i: ObjectID, o: Object) -> Iterable[bytes]:
+def _write_obj(i: ObjectID, o: Atom) -> Iterable[bytes]:
     yield b"%i 0 obj\n" % i
     yield from o.write()
     yield b"\nendobj\n"
 
 
 # PDF32000:1-2008 (14.4) says the file ID must be unique byte string
 # identifying the file. They recommend MD5 hashing the contents,
-# file location, and time. We'll take a shortcut here and just use random,
-# which will do fine. We use `secrets` to ensure this randomness.
-_generate_fileid = partial(token_bytes, 16)
+# file location, and time.
+# We'll take a shortcut here and just use random, which will do fine.
+# We use `secrets` to ensure this randomness cannot be manipulated.
+_generate_file_id = partial(token_bytes, 16)
 
 
 def _write_trailer(
-    offsets: Sequence[int], xref_offset: int
+    # offsets must be already sorted continuously ascending by object ID from 1
+    offsets: Sequence[int],
+    xref_offset: int,
 ) -> Iterable[bytes]:
     yield b"xref\n%i %i\n0000000000 65535 f \n" % (
         OBJ_ID_XREF,
         len(offsets) + 1,
     )
     yield from map(b"%010i 00000 n \n".__mod__, offsets)
     yield b"trailer\n"
-    yield from Dictionary(
-        (b"Root", Ref(OBJ_ID_CATALOG)),
-        (b"Size", Int(len(offsets) + 1)),
-        (b"ID", Array(repeat(HexString(_generate_fileid()), 2))),
-    ).write()
+    yield from _write_dict(
+        (
+            (b"Root", Ref(OBJ_ID_CATALOG)),
+            (b"Size", Int(len(offsets) + 1)),
+            (b"ID", Array(repeat(HexString(_generate_file_id()), 2))),
+        )
+    )
     yield b"\nstartxref\n%i\n%%%%EOF\n" % xref_offset
 
 
-def write(objs: Iterable[ObjectWithID], /) -> Iterator[bytes]:
+def write(
+    # object IDs must ascend continuously from 4 onwards,
+    # with the last three items being catalog, pagetree,
+    # and resources (ids 1, 2, 3 respectively).
+    objs: Iterable[Object],
+) -> Iterator[bytes]:
     yield _HEADER
     offsets = [_FIRST_OFFSET]
     for chunk in map(b"".join, starmap(_write_obj, objs)):
         offsets.append(len(chunk))
         yield chunk
+    (
+        *offsets,
+        catalog_offset,
+        pagetree_offset,
+        resources_offset,
+        xref_offset,
+    ) = accumulate(offsets)
+    yield from _write_trailer(
+        [catalog_offset, pagetree_offset, resources_offset] + offsets,
+        xref_offset,
+    )
+
+
+_STRING_ESCAPES = {
+    b"\\": b"\\\\",
+    b"\n": b"\\n",
+    b"\r": b"\\r",
+    b"\t": b"\\t",
+    b"\b": b"\\b",
+    b"\f": b"\\f",
+    b"(": b"\\(",
+    b")": b"\\)",
+}
+
+
+def _replace_with_escape(m: re.Match) -> bytes:
+    return _STRING_ESCAPES[m.group()]
+
 
-    *offsets, xref_offset = accumulate(offsets)
-    yield from _write_trailer(offsets, xref_offset)
+_escape = partial(
+    re.compile(b"(%b)" % b"|".join(map(re.escape, _STRING_ESCAPES))).sub,
+    _replace_with_escape,
+)
```

### Comparing `pdfje-0.3.0/src/pdfje/fonts.py` & `pdfje-0.4.0/src/pdfje/fonts/embed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,418 +1,394 @@
 from __future__ import annotations
 
-import abc
 import enum
 from collections import defaultdict
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from io import BytesIO
-from itertools import chain, count, starmap
+from itertools import count
+from operator import methodcaller
 from pathlib import Path
-from typing import AbstractSet, Collection, Iterable, Mapping
+from typing import TYPE_CHECKING, Collection, Iterable
 
-import fontTools.subset
-from fontTools.ttLib import TTFont as FontToolsTTF
+from .. import atoms
+from ..atoms import sanitize_name
+from ..common import (
+    Char,
+    Func,
+    Ordinal,
+    Pt,
+    add_slots,
+    dictget,
+    first,
+    pipe,
+    setattr_frozen,
+)
+from .common import (
+    TEXTSPACE_TO_GLYPHSPACE,
+    Font,
+    FontID,
+    GlyphPt,
+    KerningTable,
+    kern,
+)
 
-from . import atoms
-from .atoms import ASCII, sanitize_name
-from .common import add_slots
+try:
+    import fontTools.subset
+    from fontTools.ttLib import TTFont
+except ModuleNotFoundError:  # pragma: no cover
+    HAS_FONTTOOLS = False
+else:
+    HAS_FONTTOOLS = True
+    from ..vendor import get_kerning_pairs
 
-FontID = bytes  # unique name assigned to a font within a PDF
 
-_CodePoint = int  # a unicode code point
+OBJS_PER_EMBEDDED_FONT = 7
 _GlyphName = str  # name uniquely identifying a glyph in a TTF font
-_GlyphID = int  # integer unique identifying a glyph in a TTF font
-_Char = str  # 1-length string, i.e. a unicode character
-_OBJS_PER_EMBEDDED_FONT = 7
-_CID = int  # 16-bit ID uniquely identifying a character in a PDF
+_CID = int  # CharacterID. 16-bit ID uniquely identifying a character in a PDF
 _CID_MAX = 0xFFFF  # character IDs are stored as 16-bit values
-_TEXTSPACE_TO_GLYPHSPACE = 1000  # See PDF32000-1:2008 (9.7.3)
+_REPLACEMENT_GLYPH: _GlyphName = ".notdef"
 _CIDSYS_INFO = atoms.Dictionary(
     (b"Registry", atoms.LiteralString(b"Adobe")),
     (b"Ordering", atoms.LiteralString(b"UCS")),
     (b"Supplement", atoms.Int(0)),
 )
-_EMPTY_ITERATOR = iter(())
-_SUBSET_OPTIONS = fontTools.subset.Options(
-    drop_tables=[
-        "BASE",
-        "JSTF",
-        "DSIG",
-        "EBDT",
-        "EBLC",
-        "EBSC",
-        "PCLT",
-        "LTSH",
-        "Feat",
-        "Glat",
-        "Gloc",
-        "Silf",
-        "Sill",
-        "GDEF",
-        "GSUB",
-        "GPOS",
-        "MATH",
-        "hdmx",
-    ],
-    notdef_outline=True,
-    recommended_glyphs=True,
-)
-
-
-# See PDF 32000-1:2008, section 9.8.2
-class FontDescriptorFlag(enum.IntFlag):
-    FIXED_PITCH = 1 << 0
-    SERIF = 1 << 1
-    SYMBOLIC = 1 << 2
-    SCRIPT = 1 << 3
-    NONSYMBOLIC = 1 << 5
-    ITALIC = 1 << 6
-    ALL_CAP = 1 << 16
-    SMALL_CAP = 1 << 17
-    FORCE_BOLD = 1 << 18
-
-
-class Font(abc.ABC):
-    "Base class for builtin and embedded fonts"
-    __slots__ = ()
-
-    @staticmethod
-    def from_path(p: Path) -> "TTF":
-        return TTF(p)
-
-
-@add_slots
-@dataclass(frozen=True)
-class TTF(Font):
-    path: Path
-
-
-@add_slots
-@dataclass(frozen=True, repr=False)
-class Builtin(Font):
-    name: ASCII
-
-    def __repr__(self) -> str:
-        cls = type(self)
-        return f"{cls.__module__}.{cls.__name__}({self.name.decode()})"
-
-
-class IncludedFont(abc.ABC):
-    """A font with extra information on how to include it in the document"""
-
-    __slots__ = ()
-
-    font: Font
-    id: FontID
 
-    @abc.abstractmethod
-    def to_resource(self) -> atoms.Object:
-        raise NotImplementedError()
 
-    @abc.abstractmethod
-    def to_atoms(self) -> Iterable[atoms.ObjectWithID]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def encode(self, s: str) -> bytes:
-        raise NotImplementedError()
-
-
-@add_slots
-@dataclass(frozen=True)
-class BuiltinUse(IncludedFont):
-    font: Builtin
-    id: FontID
-
-    def to_resource(self) -> atoms.Object:
-        return atoms.Dictionary(
-            (b"Type", atoms.Name(b"Font")),
-            (b"Subtype", atoms.Name(b"Type1")),
-            (b"BaseFont", atoms.Name(self.font.name)),
-            (b"Encoding", atoms.Name(b"WinAnsiEncoding")),
+def _utf16be_hex(c: Ordinal) -> bytes:
+    if c <= 0xFFFF:
+        return b"%04X" % c
+    else:
+        return b"%04X%04X" % (
+            (c - 0x10000) >> 10 | 0xD800,
+            (c & 0x3FF) | 0xDC00,
         )
 
-    def to_atoms(self) -> Iterable[atoms.ObjectWithID]:
-        return _EMPTY_ITERATOR
-
-    @staticmethod
-    def encode(s: str) -> bytes:
-        return s.encode("cp1252", errors="replace")
-
-
-@add_slots
-@dataclass(frozen=True)
-class EmbeddedSubset(IncludedFont):
-    id: FontID
-    obj_id: atoms.ObjectID
-    font: TTF
-    ttf: FontToolsTTF
-
-    # NOTE: both mappings are ordered the same
-    cids: Mapping[_CodePoint, _CID]
-    glyphs: Mapping[_CodePoint, _GlyphID]
-
-    @staticmethod
-    def from_chars(
-        id: FontID,
-        obj_id: atoms.ObjectID,
-        font: TTF,
-        chars: AbstractSet[_Char],
-    ) -> EmbeddedSubset:
-        ttf = FontToolsTTF(font.path)
-        sub = fontTools.subset.Subsetter(_SUBSET_OPTIONS)
-        # It's important for the CID/GID and unicode map that
-        # \U0000 is included
-        sub.populate(unicodes=chain(map(ord, chars), (0,)))
-        sub.subset(ttf)
-        cmap: dict[_CodePoint, _GlyphName] | None = ttf.getBestCmap()
-        assert cmap is not None, "Couldn't read font from file"
-        # PDF only supports 16-bit character/glyph entries,
-        # thus there is a theoretical limit to the number of unique characters
-        # in a document per font. There are workarounds, but most fonts don't
-        # even have this many glyphs and this many different characters
-        # seem unlikely to occur in common text. Thus, we just assert.
-        assert len(chars) < _CID_MAX
-        gname_to_gid: dict[_GlyphName, _GlyphID] = ttf.getReverseGlyphMap()
-        return EmbeddedSubset(
-            id,
-            obj_id,
-            font,
-            ttf,
-            dict(zip(cmap, count())),
-            dict(zip(cmap, map(gname_to_gid.__getitem__, cmap.values()))),
-        )
 
-    def encode(self, s: str) -> bytes:
-        return s.translate(self.cids).encode(
-            "utf-16be", errors="surrogatepass"
-        )
+if TYPE_CHECKING or HAS_FONTTOOLS:
+    _SUBSET_OPTIONS = fontTools.subset.Options(
+        drop_tables=[
+            "BASE",
+            "JSTF",
+            "DSIG",
+            "EBDT",
+            "EBLC",
+            "EBSC",
+            "PCLT",
+            "LTSH",
+            "Feat",
+            "Glat",
+            "Gloc",
+            "Silf",
+            "Sill",
+            "GDEF",
+            "GSUB",
+            "GPOS",
+            "MATH",
+            "hdmx",
+        ],
+        notdef_outline=True,
+        recommended_glyphs=True,
+    )
 
-    def to_resource(self) -> atoms.Object:
-        return atoms.Ref(self.obj_id)
+    @add_slots
+    @dataclass(frozen=True, eq=False, repr=False)
+    class Subset(Font):
+        id: FontID
+        ttf: TTFont
+        charwidth: Func[Char, GlyphPt]
+        cids: defaultdict[Ordinal, _CID]
+        scale: float  # from glyph units to GlyphPt
+        kerning: KerningTable | None
+        spacewidth: GlyphPt = field(init=False)
+
+        encoding_width = 2
+
+        def __repr__(self) -> str:
+            return (
+                f"{type(self).__name__}({self.ttf['name'].getBestFullName()})"
+            )
+
+        def __post_init__(self) -> None:
+            setattr_frozen(self, "spacewidth", self.charwidth(" "))
+
+        @staticmethod
+        def new(i: FontID, font: Path) -> Subset:
+            ttf = TTFont(font)
+            scale = TEXTSPACE_TO_GLYPHSPACE / ttf["head"].unitsPerEm
+            return Subset(
+                id=i,
+                ttf=ttf,
+                # FUTURE: cache calls to this function?
+                charwidth=pipe(
+                    ord,
+                    dictget(ttf.getBestCmap(), _REPLACEMENT_GLYPH),
+                    ttf["hmtx"].metrics.__getitem__,
+                    first,
+                    scale.__mul__,
+                ),
+                cids=defaultdict(count().__next__),
+                scale=scale,
+                kerning=(
+                    pipe(dictget(kernpairs, 0), scale.__mul__)
+                    if (kernpairs := get_kerning_pairs.for_font(ttf))
+                    else None
+                ),
+            )
 
-    def to_atoms(self) -> Iterable[atoms.ObjectWithID]:
-        scale = _TEXTSPACE_TO_GLYPHSPACE / self.ttf["head"].unitsPerEm
-        # According to PDF32000-1:2008 (9.6.4) font subsets
-        # need to begin with an arbitrary six-letter tag.
-        # The tag should be the same per font subset added by a PDF writer.
-        # We choose `PDFJE` padded with an `A` at the front.
-        tagged_name = atoms.Name(
-            b"APDFJE+"
-            + sanitize_name(self.ttf["name"].getBestFullName().encode())
-        )
+        def width(self, s: str) -> Pt:
+            return sum(map(self.charwidth, s)) / TEXTSPACE_TO_GLYPHSPACE
 
-        (
-            descendant_id,
-            unicodemap_id,
-            cidsysinfo_id,
-            descriptor_id,
-            cid_gid_map_id,
-            file_id,
-        ) = range(self.obj_id + 1, self.obj_id + _OBJS_PER_EMBEDDED_FONT)
-        # These objects are based on PDF32000-1:2008, page 293
-        yield (
-            self.obj_id,
-            atoms.Dictionary(
-                (b"Type", atoms.Name(b"Font")),
-                (b"Subtype", atoms.Name(b"Type0")),
-                (b"BaseFont", tagged_name),
-                (b"Encoding", atoms.Name(b"Identity-H")),
-                (
-                    b"DescendantFonts",
-                    atoms.Array((atoms.Ref(descendant_id),)),
-                ),
-                (b"ToUnicode", atoms.Ref(unicodemap_id)),
-            ),
-        )
-        yield (
-            descendant_id,
-            atoms.Dictionary(
-                (b"Type", atoms.Name(b"Font")),
-                (b"Subtype", atoms.Name(b"CIDFontType2")),
-                (b"BaseFont", tagged_name),
-                (b"CIDSystemInfo", atoms.Ref(cidsysinfo_id)),
-                (b"FontDescriptor", atoms.Ref(descriptor_id)),
-                (
-                    b"DW",
-                    atoms.Int(
-                        round(scale * self.ttf["hmtx"].metrics[".notdef"][0])
+        def encode(self, s: str) -> bytes:
+            return (
+                s.translate(self.cids)
+                # Encoding by UTF-16BE is a fast way to convert from CIDs
+                # to bytes. Because not all CIDs are valid codepoints,
+                # we use surrogatepass.
+                .encode("utf-16be", errors="surrogatepass")
+            )
+
+        def kern(
+            self, s: str, /, prev: Char | None, offset: int
+        ) -> Iterable[tuple[int, GlyphPt]]:
+            return (
+                kern(self.kerning, s, 2, prev, offset) if self.kerning else ()
+            )
+
+        def to_objects(self, obj_id: atoms.ObjectID) -> Iterable[atoms.Object]:
+            # PDF only supports 16-bit character/glyph entries,
+            # thus there is a theoretical limit to the number of unique
+            # characters in a document per font. There are workarounds,
+            # but most fonts don't even have this many glyphs and this many
+            # different characters seem unlikely to occur in common text.
+            # Thus, we just assert.
+            assert len(self.cids) < _CID_MAX
+            # According to PDF32000-1:2008 (9.6.4) font subsets
+            # need to begin with an arbitrary six-letter tag.
+            # The tag should be the same per font subset added by a PDF writer.
+            # We choose `PDFJE` padded with an `A` at the front.
+            tagged_name = atoms.Name(
+                b"APDFJE+"
+                # FUTURE: handle empty/duplicate name?
+                + sanitize_name(self.ttf["name"].getBestFullName().encode())
+            )
+            sub = fontTools.subset.Subsetter(_SUBSET_OPTIONS)
+            sub.populate(unicodes=self.cids)
+            sub.subset(self.ttf)
+            (
+                descendant_id,
+                unicodemap_id,
+                cidsysinfo_id,
+                descriptor_id,
+                cid_gid_map_id,
+                file_id,
+            ) = range(obj_id + 1, obj_id + OBJS_PER_EMBEDDED_FONT)
+            # These objects are based on PDF32000-1:2008, page 293
+            yield (
+                obj_id,
+                atoms.Dictionary(
+                    (b"Type", atoms.Name(b"Font")),
+                    (b"Subtype", atoms.Name(b"Type0")),
+                    (b"BaseFont", tagged_name),
+                    (b"Encoding", atoms.Name(b"Identity-H")),
+                    (
+                        b"DescendantFonts",
+                        atoms.Array((atoms.Ref(descendant_id),)),
                     ),
+                    (b"ToUnicode", atoms.Ref(unicodemap_id)),
                 ),
-                (b"W", _encode_widths(self.ttf, scale)),
-                (b"CIDToGIDMap", atoms.Ref(cid_gid_map_id)),
-            ),
-        )
-        yield (unicodemap_id, _to_unicode_map(self.cids.items()))
-        yield (cidsysinfo_id, _CIDSYS_INFO)
-        yield (
-            descriptor_id,
-            atoms.Dictionary(
-                (b"Type", atoms.Name(b"FontDescriptor")),
-                (b"FontName", tagged_name),
-                (b"Flags", _encode_flags(self.ttf)),
-                (b"FontBBox", _encode_bbox(self.ttf, scale)),
-                (
-                    b"ItalicAngle",
-                    atoms.Int(round(self.ttf["post"].italicAngle)),
-                ),
-                (
-                    b"Ascent",
-                    atoms.Int(round(self.ttf["hhea"].ascent * scale)),
+            )
+            yield (
+                descendant_id,
+                atoms.Dictionary(
+                    (b"Type", atoms.Name(b"Font")),
+                    (b"Subtype", atoms.Name(b"CIDFontType2")),
+                    (b"BaseFont", tagged_name),
+                    (b"CIDSystemInfo", atoms.Ref(cidsysinfo_id)),
+                    (b"FontDescriptor", atoms.Ref(descriptor_id)),
+                    (
+                        b"DW",
+                        atoms.Real(
+                            self.ttf["hmtx"][_REPLACEMENT_GLYPH][0]
+                            * self.scale
+                        ),
+                    ),
+                    (
+                        b"W",
+                        _encode_widths(
+                            map(pipe(chr, self.charwidth), self.cids)
+                        ),
+                    ),
+                    (b"CIDToGIDMap", atoms.Ref(cid_gid_map_id)),
                 ),
-                (
-                    b"Descent",
-                    atoms.Int(round(self.ttf["hhea"].descent * scale)),
+            )
+            yield (
+                unicodemap_id,
+                atoms.Stream(_unicode_map(self.cids.items())),
+            )
+            yield (cidsysinfo_id, _CIDSYS_INFO)
+            yield (
+                descriptor_id,
+                atoms.Dictionary(
+                    (b"Type", atoms.Name(b"FontDescriptor")),
+                    (b"FontName", tagged_name),
+                    (b"Flags", _encode_flags(self.ttf)),
+                    (b"FontBBox", _encode_bbox(self.ttf, self.scale)),
+                    (
+                        b"ItalicAngle",
+                        atoms.Int(round(self.ttf["post"].italicAngle)),
+                    ),
+                    (
+                        b"Ascent",
+                        atoms.Int(round(self.ttf["hhea"].ascent * self.scale)),
+                    ),
+                    (
+                        b"Descent",
+                        atoms.Int(
+                            round(self.ttf["hhea"].descent * self.scale)
+                        ),
+                    ),
+                    (b"CapHeight", _encode_cap_height(self.ttf, self.scale)),
+                    (b"StemV", _encode_stem_v(self.ttf)),
+                    (b"FontFile2", atoms.Ref(file_id)),
                 ),
-                (b"CapHeight", _encode_cap_height(self.ttf, scale)),
-                (b"StemV", _encode_stem_v(self.ttf)),
-                (b"FontFile2", atoms.Ref(file_id)),
-            ),
+            )
+            yield (cid_gid_map_id, _encode_cid_gid_map(self.ttf, self.cids))
+            yield (file_id, _encode_ttf_with_side_effects(self.ttf))
+
+    def _encode_bbox(f: TTFont, scale: float) -> atoms.Array:
+        head = f["head"]
+        return atoms.Array(
+            atoms.Int(round(v * scale))
+            for v in (head.xMin, head.yMin, head.xMax, head.yMax)
         )
-        yield (cid_gid_map_id, _encode_cid_gid_map(self.cids, self.glyphs))
-        yield (file_id, _encode_ttf_with_side_effects(self.ttf))
-
-
-def _encode_bbox(f: FontToolsTTF, scale: float) -> atoms.Array:
-    head = f["head"]
-    return atoms.Array(
-        atoms.Int(round(v * scale))
-        for v in (head.xMin, head.yMin, head.xMax, head.yMax)
-    )
 
+    # See PDF 32000-1:2008, section 9.8.2
+    class _FontDescriptorFlag(enum.IntFlag):
+        FIXED_PITCH = 1 << 0
+        SERIF = 1 << 1
+        SYMBOLIC = 1 << 2
+        SCRIPT = 1 << 3
+        NONSYMBOLIC = 1 << 5
+        ITALIC = 1 << 6
+        ALL_CAP = 1 << 16
+        SMALL_CAP = 1 << 17
+        FORCE_BOLD = 1 << 18
+
+    def _encode_flags(f: TTFont) -> atoms.Int:
+        return atoms.Int(
+            _FontDescriptorFlag.SYMBOLIC
+            | (f["post"].isFixedPitch and _FontDescriptorFlag.FIXED_PITCH)
+            | (bool(f["post"].italicAngle) and _FontDescriptorFlag.ITALIC)
+            | (
+                f["OS/2"].usWeightClass >= 600
+                and _FontDescriptorFlag.FORCE_BOLD
+            )
+        )
 
-def _encode_flags(f: FontToolsTTF) -> atoms.Int:
-    return atoms.Int(
-        FontDescriptorFlag.SYMBOLIC
-        | (f["post"].isFixedPitch and FontDescriptorFlag.FIXED_PITCH)
-        | (bool(f["post"].italicAngle) and FontDescriptorFlag.ITALIC)
-        | (f["OS/2"].usWeightClass >= 600 and FontDescriptorFlag.FORCE_BOLD)
-    )
-
+    # WARNING: the act of saving fontTools' TTFont leads to changed properties
+    # such as ttfont['head'].xMin. Beware of when you call this function!
+    def _encode_ttf_with_side_effects(f: TTFont) -> atoms.Stream:
+        tmp = BytesIO()
+        f.save(tmp)
+        content = tmp.getvalue()
+        return atoms.Stream([content], [(b"Length1", atoms.Int(len(content)))])
+
+    def _encode_cid_gid_map(ttf: TTFont, cids: Iterable[_CID]) -> atoms.Stream:
+        # See PDF32000-1:2008 (table 117) for instructions on how this works.
+        # Note that the Glyph IDs are different after subsetting!
+        return atoms.Stream(
+            map(
+                pipe(
+                    # CID -> Glyph name
+                    dictget(ttf.getBestCmap() or {}, _REPLACEMENT_GLYPH),
+                    # Glyph name -> Glyph ID
+                    ttf.getReverseGlyphMap().__getitem__,
+                    # Glyph ID -> bytes
+                    methodcaller("to_bytes", 2, "big"),
+                ),
+                cids,
+            )
+        )
 
-# WARNING: the act of saving fontTools' TTFont leads to changed properties
-# such as ttfont['head'].xMin. Beware of when you call this function!
-def _encode_ttf_with_side_effects(f: FontToolsTTF) -> atoms.Stream:
-    tmp = BytesIO()
-    f.save(tmp)
-    content = tmp.getvalue()
-    return atoms.Stream(content, ((b"Length1", atoms.Int(len(content))),))
-
-
-def _encode_cid_gid_map(
-    cids: Iterable[_CodePoint],  # ordered by CID (ascending)
-    glyphs: Mapping[_CodePoint, _GlyphID],
-) -> atoms.Object:
-    # See PDF32000-1:2008 (table 117) for instructions on how to encode this
-    return atoms.Stream(b"".join(glyphs[c].to_bytes(2, "big") for c in cids))
-
-
-def _encode_widths(f: FontToolsTTF, scale: float) -> atoms.Array:
-    # See PDF32000-1:2008 (9.7.4.3) for how character widths are encoded.
-    # For now we choose to simply encode all widths sequentially.
-    # It should be made more efficient in the future,
-    # especially for fixed width fonts.
-    return atoms.Array(
-        (
-            atoms.Int(0),
-            atoms.Array(
-                atoms.Int(round(scale * f["hmtx"].metrics[g][0]))
-                for g in f.getBestCmap().values()
-            ),
+    # NOTE: the given widths must be ordered by continuously ascending
+    # CID value from 0 onwards
+    def _encode_widths(widths: Iterable[GlyphPt]) -> atoms.Array:
+        # See PDF32000-1:2008 (9.7.4.3) for how character widths are encoded.
+        # For now we choose to simply encode all widths sequentially.
+        # FUTURE: It should be made more efficient for fixed width fonts.
+        return atoms.Array(
+            (atoms.Int(0), atoms.Array(map(pipe(int, atoms.Int), widths)))
         )
-    )
 
+    def _encode_cap_height(f: TTFont, scale: float) -> atoms.Int:
+        # Apparently not all TTF fonts properly have the capheight accessible.
+        # We can fall back to the ascender height, which is usually slightly
+        # lower. See https://fonts.google.com/knowledge/glossary/cap_height
+        try:
+            v = f["OS/2"].sCapHeight
+        except AttributeError:
+            v = f["hhea"].ascent
+
+        return atoms.Int(round(v * scale))
+
+    _FONTWEIGHT_TO_STEM_V_RATIO = (241 - 50) / (900 - 100)
+
+    def _encode_stem_v(f: TTFont) -> atoms.Int:
+        # See stackoverflow.com/questions/35485179.
+        # The StemV value cannot be directly retrieved from TTF type fonts.
+        # Common wisdom seems to be to map the font weight (100-900) to
+        # reasonable StemV values (50-241).
+        return atoms.Int(
+            round(50 + _FONTWEIGHT_TO_STEM_V_RATIO * f["OS/2"].usWeightClass)
+        )
 
-def _encode_cap_height(f: FontToolsTTF, scale: float) -> atoms.Int:
-    # Apparently not all TTF fonts properly have the capheight accessible.
-    # We can fall back to the ascender height, which is usually slightly lower.
-    try:
-        v = f["OS/2"].sCapHeight
-    except AttributeError:
-        v = f["hhea"].ascent
-
-    return atoms.Int(round(v * scale))
-
-
-_FONTWEIGHT_TO_STEM_V_RATIO = (241 - 50) / (900 - 100)
-
-
-def _encode_stem_v(f: FontToolsTTF) -> atoms.Int:
-    # See stackoverflow.com/questions/35485179.
-    # The StemV value cannot be directly retrieved from TTF type fonts.
-    # Common wisdom seems to be to map the font weight (100-900) to reasonable
-    # StemV values (50-241).
-    return atoms.Int(
-        round(50 + _FONTWEIGHT_TO_STEM_V_RATIO * f["OS/2"].usWeightClass)
+    def _unicode_map(m: Collection[tuple[Ordinal, _CID]]) -> Iterable[bytes]:
+        # The 'To Unicode' map ensures that the correct characters are copied
+        # from a text selection.
+        yield _TO_UNICODE_CMAP_PRE
+        yield b"%i beginbfchar\n" % len(m)
+        for code, cid in m:
+            yield b"<%04X> <%b>\n" % (cid, _utf16be_hex(code))
+        yield _TO_UNICODE_CMAP_POST
+
+    # based on PDF32000-1:2008, page 294
+    _TO_UNICODE_CMAP_PRE = b"""\
+    /CIDInit /ProcSet findresource begin
+    12 dict begin
+    begincmap
+    /CIDSystemInfo
+    %b def
+    /CMapName /Adobe-Identity-UCS def
+    /CMapType 2 def
+    1 begincodespacerange
+    <0000> <FFFF>
+    endcodespacerange
+    """ % b"".join(
+        _CIDSYS_INFO.write()
     )
-
-
-def _to_unicode_map(m: Collection[tuple[_CodePoint, _CID]]) -> atoms.Object:
-    # The 'To Unicode' map ensures that the correct characters are copied
-    # from a text selection.
-    return atoms.Stream(
-        _TO_UNICODE_CMAP
-        % (
-            b"".join(_CIDSYS_INFO.write()),
-            len(m),
-            b"\n".join(
-                b"<%04X> <%b>" % (cid, utf16be_hex(code)) for code, cid in m
-            ),
-        )
+    _TO_UNICODE_CMAP_POST = b"""\
+    endbfchar
+    endcmap
+    CMapName currentdict /CMap defineresource pop
+    end
+    end"""
+else:  # pragma: no cover
+    FONTTOOLS_MISSING_EXCEPTION = NotImplementedError(
+        "Embedded fonts require `fontTools` dependency. "
+        "Install with pdfje[fonts]"
     )
 
+    @add_slots
+    @dataclass(frozen=True)
+    class Subset(Font):
+        @staticmethod
+        def new(i: FontID, font: Path) -> Subset:
+            raise FONTTOOLS_MISSING_EXCEPTION
 
-def utf16be_hex(c: _CodePoint) -> bytes:
-    if c <= 0xFFFF:
-        return b"%04X" % c
-    else:
-        return b"%04X%04X" % (
-            (c - 0x10000) >> 10 | 0xD800,
-            (c & 0x3FF) | 0xDC00,
-        )
-
-
-def usage(
-    text: Iterable[tuple[str, Font]], first_id: atoms.ObjectID
-) -> Iterable[IncludedFont]:
-    next_name = map(b"F%i".__mod__, count()).__next__
-    next_id = count(first_id, _OBJS_PER_EMBEDDED_FONT).__next__
-    embeds: defaultdict[
-        TTF, tuple[FontID, atoms.ObjectID, set[_Char]]
-    ] = defaultdict(lambda: (next_name(), next_id(), set()))
-    builtins: defaultdict[Builtin, FontID] = defaultdict(next_name)
-
-    for content, font in text:
-        if isinstance(font, Builtin):
-            builtins[font]
-        else:
-            assert isinstance(font, TTF)
-            embeds[font][2].update(content)
-
-    return chain(
-        starmap(BuiltinUse, builtins.items()),
-        (
-            EmbeddedSubset.from_chars(name, id, font, chars)
-            for font, (name, id, chars) in embeds.items()
-        ),
-    )
+        def width(self, s: str) -> Pt:
+            raise FONTTOOLS_MISSING_EXCEPTION
 
+        def encode(self, s: str) -> bytes:
+            raise FONTTOOLS_MISSING_EXCEPTION
 
-# based on PDF32000-1:2008, page 294
-_TO_UNICODE_CMAP = b"""\
-/CIDInit /ProcSet findresource begin
-12 dict begin
-begincmap
-/CIDSystemInfo
-%b def
-/CMapName /Adobe-Identity-UCS def
-/CMapType 2 def
-1 begincodespacerange
-<0000> <FFFF>
-endcodespacerange
-%i beginbfchar
-%b
-endbfchar
-endcmap
-CMapName currentdict /CMap defineresource pop
-end
-end"""
+        def kern(self, s: str) -> Iterable[tuple[int, GlyphPt]]:
+            raise FONTTOOLS_MISSING_EXCEPTION
```

