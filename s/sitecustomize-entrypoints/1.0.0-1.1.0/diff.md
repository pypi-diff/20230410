# Comparing `tmp/sitecustomize_entrypoints-1.0.0.tar.gz` & `tmp/sitecustomize-entrypoints-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitecustomize_entrypoints-1.0.0.tar", max compression
+gzip compressed data, was "sitecustomize-entrypoints-1.1.0.tar", max compression
```

## Comparing `sitecustomize_entrypoints-1.0.0.tar` & `sitecustomize-entrypoints-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1270 2023-03-10 09:32:06.984670 sitecustomize_entrypoints-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      421 2022-04-19 12:55:04.189611 sitecustomize_entrypoints-1.0.0/README.md
--rw-r--r--   0        0        0      579 2023-03-10 09:32:06.985671 sitecustomize_entrypoints-1.0.0/src/sitecustomize/__init__.py
--rw-r--r--   0        0        0        0 2022-04-19 12:55:04.498613 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/__init__.py
--rw-r--r--   0        0        0    31991 2022-04-19 12:55:04.499614 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1930 2022-04-19 12:55:04.500612 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      773 2022-04-19 12:55:04.512611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1897 2022-04-19 12:55:04.513610 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2999 2022-04-19 12:55:04.514612 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2141 2022-04-19 12:55:04.515611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1202 2022-04-19 12:55:04.521611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2265 2022-04-19 12:55:04.523611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      584 2022-04-19 12:55:04.498613 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/LICENSE
--rw-r--r--   0        0        0        0 2022-04-19 12:55:04.525611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/py.typed
--rw-r--r--   0        0        0       39 2022-04-19 12:55:04.432612 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/vendor.txt
--rw-r--r--   0        0        0     1069 2022-04-19 12:55:04.525611 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/zipp.LICENSE
--rw-r--r--   0        0        0     8341 2022-04-19 12:55:04.538615 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/zipp.py
--rw-r--r--   0        0        0       18 2022-04-19 12:55:04.540614 sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/zipp.pyi
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 sitecustomize_entrypoints-1.0.0/setup.py
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 sitecustomize_entrypoints-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6968 2023-04-10 16:52:10.577065 sitecustomize-entrypoints-1.1.0/docs/readme.md
+-rw-r--r--   0        0        0     4016 2023-04-10 16:53:14.271237 sitecustomize-entrypoints-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2337 2023-04-10 16:53:14.274525 sitecustomize-entrypoints-1.1.0/src/sitecustomize/__init__.py
+-rw-r--r--   0        0        0     1446 2023-04-10 16:52:10.580940 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:52:10.581235 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/__init__.py
+-rw-r--r--   0        0        0      571 2023-04-10 16:52:10.581673 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0        0        0    30916 2023-04-10 16:52:10.582229 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-10 16:52:10.582677 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2023-04-10 16:52:10.583017 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1826 2023-04-10 16:52:10.583342 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2023-04-10 16:52:10.583672 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2023-04-10 16:52:10.584021 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1154 2023-04-10 16:52:10.584349 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2023-04-10 16:52:10.584730 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:52:10.584954 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/py.typed
+-rw-r--r--   0        0        0       38 2023-04-10 16:52:10.585227 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/vendor.txt
+-rw-r--r--   0        0        0     1050 2023-04-10 16:52:10.585631 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/zipp.LICENSE
+-rw-r--r--   0        0        0     8029 2023-04-10 16:52:10.586026 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/zipp.py
+-rw-r--r--   0        0        0       18 2023-04-10 16:52:10.586396 sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/zipp.pyi
+-rw-r--r--   0        0        0     7944 1970-01-01 00:00:00.000000 sitecustomize-entrypoints-1.1.0/setup.py
+-rw-r--r--   0        0        0     8369 1970-01-01 00:00:00.000000 sitecustomize-entrypoints-1.1.0/PKG-INFO
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/__init__.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1075 +1,1075 @@
-import os
-import re
-import abc
-import csv
-import sys
-from sitecustomize._vendor import zipp
-import email
-import pathlib
-import operator
-import textwrap
-import warnings
-import functools
-import itertools
-import posixpath
-import collections
-
-from . import _adapters, _meta
-from ._collections import FreezableDefaultDict, Pair
-from ._compat import (
-    NullFinder,
-    install,
-    pypy_partial,
-)
-from ._functools import method_cache, pass_none
-from ._itertools import always_iterable, unique_everseen
-from ._meta import PackageMetadata, SimplePath
-
-from contextlib import suppress
-from importlib import import_module
-from importlib.abc import MetaPathFinder
-from itertools import starmap
-from typing import List, Mapping, Optional, Union
-
-
-__all__ = [
-    'Distribution',
-    'DistributionFinder',
-    'PackageMetadata',
-    'PackageNotFoundError',
-    'distribution',
-    'distributions',
-    'entry_points',
-    'files',
-    'metadata',
-    'packages_distributions',
-    'requires',
-    'version',
-]
-
-
-class PackageNotFoundError(ModuleNotFoundError):
-    """The package was not found."""
-
-    def __str__(self):
-        return f"No package metadata was found for {self.name}"
-
-    @property
-    def name(self):
-        (name,) = self.args
-        return name
-
-
-class Sectioned:
-    """
-    A simple entry point config parser for performance
-
-    >>> for item in Sectioned.read(Sectioned._sample):
-    ...     print(item)
-    Pair(name='sec1', value='# comments ignored')
-    Pair(name='sec1', value='a = 1')
-    Pair(name='sec1', value='b = 2')
-    Pair(name='sec2', value='a = 2')
-
-    >>> res = Sectioned.section_pairs(Sectioned._sample)
-    >>> item = next(res)
-    >>> item.name
-    'sec1'
-    >>> item.value
-    Pair(name='a', value='1')
-    >>> item = next(res)
-    >>> item.value
-    Pair(name='b', value='2')
-    >>> item = next(res)
-    >>> item.name
-    'sec2'
-    >>> item.value
-    Pair(name='a', value='2')
-    >>> list(res)
-    []
-    """
-
-    _sample = textwrap.dedent(
-        """
-        [sec1]
-        # comments ignored
-        a = 1
-        b = 2
-
-        [sec2]
-        a = 2
-        """
-    ).lstrip()
-
-    @classmethod
-    def section_pairs(cls, text):
-        return (
-            section._replace(value=Pair.parse(section.value))
-            for section in cls.read(text, filter_=cls.valid)
-            if section.name is not None
-        )
-
-    @staticmethod
-    def read(text, filter_=None):
-        lines = filter(filter_, map(str.strip, text.splitlines()))
-        name = None
-        for value in lines:
-            section_match = value.startswith('[') and value.endswith(']')
-            if section_match:
-                name = value.strip('[]')
-                continue
-            yield Pair(name, value)
-
-    @staticmethod
-    def valid(line):
-        return line and not line.startswith('#')
-
-
-class DeprecatedTuple:
-    """
-    Provide subscript item access for backward compatibility.
-
-    >>> recwarn = getfixture('recwarn')
-    >>> ep = EntryPoint(name='name', value='value', group='group')
-    >>> ep[:]
-    ('name', 'value', 'group')
-    >>> ep[0]
-    'name'
-    >>> len(recwarn)
-    1
-    """
-
-    _warn = functools.partial(
-        warnings.warn,
-        "EntryPoint tuple interface is deprecated. Access members by name.",
-        DeprecationWarning,
-        stacklevel=pypy_partial(2),
-    )
-
-    def __getitem__(self, item):
-        self._warn()
-        return self._key()[item]
-
-
-class EntryPoint(DeprecatedTuple):
-    """An entry point as defined by Python packaging conventions.
-
-    See `the packaging docs on entry points
-    <https://packaging.python.org/specifications/entry-points/>`_
-    for more information.
-
-    >>> ep = EntryPoint(
-    ...     name=None, group=None, value='package.module:attr [extra1, extra2]')
-    >>> ep.module
-    'package.module'
-    >>> ep.attr
-    'attr'
-    >>> ep.extras
-    ['extra1', 'extra2']
-    """
-
-    pattern = re.compile(
-        r'(?P<module>[\w.]+)\s*'
-        r'(:\s*(?P<attr>[\w.]+)\s*)?'
-        r'((?P<extras>\[.*\])\s*)?$'
-    )
-    """
-    A regular expression describing the syntax for an entry point,
-    which might look like:
-
-        - module
-        - package.module
-        - package.module:attribute
-        - package.module:object.attribute
-        - package.module:attr [extra1, extra2]
-
-    Other combinations are possible as well.
-
-    The expression is lenient about whitespace around the ':',
-    following the attr, and following any extras.
-    """
-
-    dist: Optional['Distribution'] = None
-
-    def __init__(self, name, value, group):
-        vars(self).update(name=name, value=value, group=group)
-
-    def load(self):
-        """Load the entry point from its definition. If only a module
-        is indicated by the value, return that module. Otherwise,
-        return the named object.
-        """
-        match = self.pattern.match(self.value)
-        module = import_module(match.group('module'))
-        attrs = filter(None, (match.group('attr') or '').split('.'))
-        return functools.reduce(getattr, attrs, module)
-
-    @property
-    def module(self):
-        match = self.pattern.match(self.value)
-        return match.group('module')
-
-    @property
-    def attr(self):
-        match = self.pattern.match(self.value)
-        return match.group('attr')
-
-    @property
-    def extras(self):
-        match = self.pattern.match(self.value)
-        return re.findall(r'\w+', match.group('extras') or '')
-
-    def _for(self, dist):
-        vars(self).update(dist=dist)
-        return self
-
-    def __iter__(self):
-        """
-        Supply iter so one may construct dicts of EntryPoints by name.
-        """
-        msg = (
-            "Construction of dict of EntryPoints is deprecated in "
-            "favor of EntryPoints."
-        )
-        warnings.warn(msg, DeprecationWarning)
-        return iter((self.name, self))
-
-    def matches(self, **params):
-        """
-        EntryPoint matches the given parameters.
-
-        >>> ep = EntryPoint(group='foo', name='bar', value='bing:bong [extra1, extra2]')
-        >>> ep.matches(group='foo')
-        True
-        >>> ep.matches(name='bar', value='bing:bong [extra1, extra2]')
-        True
-        >>> ep.matches(group='foo', name='other')
-        False
-        >>> ep.matches()
-        True
-        >>> ep.matches(extras=['extra1', 'extra2'])
-        True
-        >>> ep.matches(module='bing')
-        True
-        >>> ep.matches(attr='bong')
-        True
-        """
-        attrs = (getattr(self, param) for param in params)
-        return all(map(operator.eq, params.values(), attrs))
-
-    def _key(self):
-        return self.name, self.value, self.group
-
-    def __lt__(self, other):
-        return self._key() < other._key()
-
-    def __eq__(self, other):
-        return self._key() == other._key()
-
-    def __setattr__(self, name, value):
-        raise AttributeError("EntryPoint objects are immutable.")
-
-    def __repr__(self):
-        return (
-            f'EntryPoint(name={self.name!r}, value={self.value!r}, '
-            f'group={self.group!r})'
-        )
-
-    def __hash__(self):
-        return hash(self._key())
-
-
-class DeprecatedList(list):
-    """
-    Allow an otherwise immutable object to implement mutability
-    for compatibility.
-
-    >>> recwarn = getfixture('recwarn')
-    >>> dl = DeprecatedList(range(3))
-    >>> dl[0] = 1
-    >>> dl.append(3)
-    >>> del dl[3]
-    >>> dl.reverse()
-    >>> dl.sort()
-    >>> dl.extend([4])
-    >>> dl.pop(-1)
-    4
-    >>> dl.remove(1)
-    >>> dl += [5]
-    >>> dl + [6]
-    [1, 2, 5, 6]
-    >>> dl + (6,)
-    [1, 2, 5, 6]
-    >>> dl.insert(0, 0)
-    >>> dl
-    [0, 1, 2, 5]
-    >>> dl == [0, 1, 2, 5]
-    True
-    >>> dl == (0, 1, 2, 5)
-    True
-    >>> len(recwarn)
-    1
-    """
-
-    __slots__ = ()
-
-    _warn = functools.partial(
-        warnings.warn,
-        "EntryPoints list interface is deprecated. Cast to list if needed.",
-        DeprecationWarning,
-        stacklevel=pypy_partial(2),
-    )
-
-    def _wrap_deprecated_method(method_name: str):  # type: ignore
-        def wrapped(self, *args, **kwargs):
-            self._warn()
-            return getattr(super(), method_name)(*args, **kwargs)
-
-        return method_name, wrapped
-
-    locals().update(
-        map(
-            _wrap_deprecated_method,
-            '__setitem__ __delitem__ append reverse extend pop remove '
-            '__iadd__ insert sort'.split(),
-        )
-    )
-
-    def __add__(self, other):
-        if not isinstance(other, tuple):
-            self._warn()
-            other = tuple(other)
-        return self.__class__(tuple(self) + other)
-
-    def __eq__(self, other):
-        if not isinstance(other, tuple):
-            self._warn()
-            other = tuple(other)
-
-        return tuple(self).__eq__(other)
-
-
-class EntryPoints(DeprecatedList):
-    """
-    An immutable collection of selectable EntryPoint objects.
-    """
-
-    __slots__ = ()
-
-    def __getitem__(self, name):  # -> EntryPoint:
-        """
-        Get the EntryPoint in self matching name.
-        """
-        if isinstance(name, int):
-            warnings.warn(
-                "Accessing entry points by index is deprecated. "
-                "Cast to tuple if needed.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            return super().__getitem__(name)
-        try:
-            return next(iter(self.select(name=name)))
-        except StopIteration:
-            raise KeyError(name)
-
-    def select(self, **params):
-        """
-        Select entry points from self that match the
-        given parameters (typically group and/or name).
-        """
-        return EntryPoints(ep for ep in self if ep.matches(**params))
-
-    @property
-    def names(self):
-        """
-        Return the set of all names of all entry points.
-        """
-        return {ep.name for ep in self}
-
-    @property
-    def groups(self):
-        """
-        Return the set of all groups of all entry points.
-
-        For coverage while SelectableGroups is present.
-        >>> EntryPoints().groups
-        set()
-        """
-        return {ep.group for ep in self}
-
-    @classmethod
-    def _from_text_for(cls, text, dist):
-        return cls(ep._for(dist) for ep in cls._from_text(text))
-
-    @staticmethod
-    def _from_text(text):
-        return (
-            EntryPoint(name=item.value.name, value=item.value.value, group=item.name)
-            for item in Sectioned.section_pairs(text or '')
-        )
-
-
-class Deprecated:
-    """
-    Compatibility add-in for mapping to indicate that
-    mapping behavior is deprecated.
-
-    >>> recwarn = getfixture('recwarn')
-    >>> class DeprecatedDict(Deprecated, dict): pass
-    >>> dd = DeprecatedDict(foo='bar')
-    >>> dd.get('baz', None)
-    >>> dd['foo']
-    'bar'
-    >>> list(dd)
-    ['foo']
-    >>> list(dd.keys())
-    ['foo']
-    >>> 'foo' in dd
-    True
-    >>> list(dd.values())
-    ['bar']
-    >>> len(recwarn)
-    1
-    """
-
-    _warn = functools.partial(
-        warnings.warn,
-        "SelectableGroups dict interface is deprecated. Use select.",
-        DeprecationWarning,
-        stacklevel=pypy_partial(2),
-    )
-
-    def __getitem__(self, name):
-        self._warn()
-        return super().__getitem__(name)
-
-    def get(self, name, default=None):
-        self._warn()
-        return super().get(name, default)
-
-    def __iter__(self):
-        self._warn()
-        return super().__iter__()
-
-    def __contains__(self, *args):
-        self._warn()
-        return super().__contains__(*args)
-
-    def keys(self):
-        self._warn()
-        return super().keys()
-
-    def values(self):
-        self._warn()
-        return super().values()
-
-
-class SelectableGroups(Deprecated, dict):
-    """
-    A backward- and forward-compatible result from
-    entry_points that fully implements the dict interface.
-    """
-
-    @classmethod
-    def load(cls, eps):
-        by_group = operator.attrgetter('group')
-        ordered = sorted(eps, key=by_group)
-        grouped = itertools.groupby(ordered, by_group)
-        return cls((group, EntryPoints(eps)) for group, eps in grouped)
-
-    @property
-    def _all(self):
-        """
-        Reconstruct a list of all entrypoints from the groups.
-        """
-        groups = super(Deprecated, self).values()
-        return EntryPoints(itertools.chain.from_iterable(groups))
-
-    @property
-    def groups(self):
-        return self._all.groups
-
-    @property
-    def names(self):
-        """
-        for coverage:
-        >>> SelectableGroups().names
-        set()
-        """
-        return self._all.names
-
-    def select(self, **params):
-        if not params:
-            return self
-        return self._all.select(**params)
-
-
-class PackagePath(pathlib.PurePosixPath):
-    """A reference to a path in a package"""
-
-    def read_text(self, encoding='utf-8'):
-        with self.locate().open(encoding=encoding) as stream:
-            return stream.read()
-
-    def read_binary(self):
-        with self.locate().open('rb') as stream:
-            return stream.read()
-
-    def locate(self):
-        """Return a path-like object for this path"""
-        return self.dist.locate_file(self)
-
-
-class FileHash:
-    def __init__(self, spec):
-        self.mode, _, self.value = spec.partition('=')
-
-    def __repr__(self):
-        return f'<FileHash mode: {self.mode} value: {self.value}>'
-
-
-class Distribution:
-    """A Python distribution package."""
-
-    @abc.abstractmethod
-    def read_text(self, filename):
-        """Attempt to load metadata file given by the name.
-
-        :param filename: The name of the file in the distribution info.
-        :return: The text if found, otherwise None.
-        """
-
-    @abc.abstractmethod
-    def locate_file(self, path):
-        """
-        Given a path to a file in this distribution, return a path
-        to it.
-        """
-
-    @classmethod
-    def from_name(cls, name):
-        """Return the Distribution for the given package name.
-
-        :param name: The name of the distribution package to search for.
-        :return: The Distribution instance (or subclass thereof) for the named
-            package, if found.
-        :raises PackageNotFoundError: When the named package's distribution
-            metadata cannot be found.
-        """
-        for resolver in cls._discover_resolvers():
-            dists = resolver(DistributionFinder.Context(name=name))
-            dist = next(iter(dists), None)
-            if dist is not None:
-                return dist
-        else:
-            raise PackageNotFoundError(name)
-
-    @classmethod
-    def discover(cls, **kwargs):
-        """Return an iterable of Distribution objects for all packages.
-
-        Pass a ``context`` or pass keyword arguments for constructing
-        a context.
-
-        :context: A ``DistributionFinder.Context`` object.
-        :return: Iterable of Distribution objects for all packages.
-        """
-        context = kwargs.pop('context', None)
-        if context and kwargs:
-            raise ValueError("cannot accept context and kwargs")
-        context = context or DistributionFinder.Context(**kwargs)
-        return itertools.chain.from_iterable(
-            resolver(context) for resolver in cls._discover_resolvers()
-        )
-
-    @staticmethod
-    def at(path):
-        """Return a Distribution for the indicated metadata path
-
-        :param path: a string or path-like object
-        :return: a concrete Distribution instance for the path
-        """
-        return PathDistribution(pathlib.Path(path))
-
-    @staticmethod
-    def _discover_resolvers():
-        """Search the meta_path for resolvers."""
-        declared = (
-            getattr(finder, 'find_distributions', None) for finder in sys.meta_path
-        )
-        return filter(None, declared)
-
-    @property
-    def metadata(self) -> _meta.PackageMetadata:
-        """Return the parsed metadata for this Distribution.
-
-        The returned object will have keys that name the various bits of
-        metadata.  See PEP 566 for details.
-        """
-        text = (
-            self.read_text('METADATA')
-            or self.read_text('PKG-INFO')
-            # This last clause is here to support old egg-info files.  Its
-            # effect is to just end up using the PathDistribution's self._path
-            # (which points to the egg-info file) attribute unchanged.
-            or self.read_text('')
-        )
-        return _adapters.Message(email.message_from_string(text))
-
-    @property
-    def name(self):
-        """Return the 'Name' metadata for the distribution package."""
-        return self.metadata['Name']
-
-    @property
-    def _normalized_name(self):
-        """Return a normalized version of the name."""
-        return Prepared.normalize(self.name)
-
-    @property
-    def version(self):
-        """Return the 'Version' metadata for the distribution package."""
-        return self.metadata['Version']
-
-    @property
-    def entry_points(self):
-        return EntryPoints._from_text_for(self.read_text('entry_points.txt'), self)
-
-    @property
-    def files(self):
-        """Files in this distribution.
-
-        :return: List of PackagePath for this distribution or None
-
-        Result is `None` if the metadata file that enumerates files
-        (i.e. RECORD for dist-info or SOURCES.txt for egg-info) is
-        missing.
-        Result may be empty if the metadata exists but is empty.
-        """
-
-        def make_file(name, hash=None, size_str=None):
-            result = PackagePath(name)
-            result.hash = FileHash(hash) if hash else None
-            result.size = int(size_str) if size_str else None
-            result.dist = self
-            return result
-
-        @pass_none
-        def make_files(lines):
-            return list(starmap(make_file, csv.reader(lines)))
-
-        return make_files(self._read_files_distinfo() or self._read_files_egginfo())
-
-    def _read_files_distinfo(self):
-        """
-        Read the lines of RECORD
-        """
-        text = self.read_text('RECORD')
-        return text and text.splitlines()
-
-    def _read_files_egginfo(self):
-        """
-        SOURCES.txt might contain literal commas, so wrap each line
-        in quotes.
-        """
-        text = self.read_text('SOURCES.txt')
-        return text and map('"{}"'.format, text.splitlines())
-
-    @property
-    def requires(self):
-        """Generated requirements specified for this Distribution"""
-        reqs = self._read_dist_info_reqs() or self._read_egg_info_reqs()
-        return reqs and list(reqs)
-
-    def _read_dist_info_reqs(self):
-        return self.metadata.get_all('Requires-Dist')
-
-    def _read_egg_info_reqs(self):
-        source = self.read_text('requires.txt')
-        return pass_none(self._deps_from_requires_text)(source)
-
-    @classmethod
-    def _deps_from_requires_text(cls, source):
-        return cls._convert_egg_info_reqs_to_simple_reqs(Sectioned.read(source))
-
-    @staticmethod
-    def _convert_egg_info_reqs_to_simple_reqs(sections):
-        """
-        Historically, setuptools would solicit and store 'extra'
-        requirements, including those with environment markers,
-        in separate sections. More modern tools expect each
-        dependency to be defined separately, with any relevant
-        extras and environment markers attached directly to that
-        requirement. This method converts the former to the
-        latter. See _test_deps_from_requires_text for an example.
-        """
-
-        def make_condition(name):
-            return name and f'extra == "{name}"'
-
-        def quoted_marker(section):
-            section = section or ''
-            extra, sep, markers = section.partition(':')
-            if extra and markers:
-                markers = f'({markers})'
-            conditions = list(filter(None, [markers, make_condition(extra)]))
-            return '; ' + ' and '.join(conditions) if conditions else ''
-
-        def url_req_space(req):
-            """
-            PEP 508 requires a space between the url_spec and the quoted_marker.
-            Ref python/importlib_metadata#357.
-            """
-            # '@' is uniquely indicative of a url_req.
-            return ' ' * ('@' in req)
-
-        for section in sections:
-            space = url_req_space(section.value)
-            yield section.value + space + quoted_marker(section.name)
-
-
-class DistributionFinder(MetaPathFinder):
-    """
-    A MetaPathFinder capable of discovering installed distributions.
-    """
-
-    class Context:
-        """
-        Keyword arguments presented by the caller to
-        ``distributions()`` or ``Distribution.discover()``
-        to narrow the scope of a search for distributions
-        in all DistributionFinders.
-
-        Each DistributionFinder may expect any parameters
-        and should attempt to honor the canonical
-        parameters defined below when appropriate.
-        """
-
-        name = None
-        """
-        Specific name for which a distribution finder should match.
-        A name of ``None`` matches all distributions.
-        """
-
-        def __init__(self, **kwargs):
-            vars(self).update(kwargs)
-
-        @property
-        def path(self):
-            """
-            The sequence of directory path that a distribution finder
-            should search.
-
-            Typically refers to Python installed package paths such as
-            "site-packages" directories and defaults to ``sys.path``.
-            """
-            return vars(self).get('path', sys.path)
-
-    @abc.abstractmethod
-    def find_distributions(self, context=Context()):
-        """
-        Find distributions.
-
-        Return an iterable of all Distribution instances capable of
-        loading the metadata for packages matching the ``context``,
-        a DistributionFinder.Context instance.
-        """
-
-
-class FastPath:
-    """
-    Micro-optimized class for searching a path for
-    children.
-
-    >>> FastPath('').children()
-    ['...']
-    """
-
-    @functools.lru_cache()  # type: ignore
-    def __new__(cls, root):
-        return super().__new__(cls)
-
-    def __init__(self, root):
-        self.root = root
-
-    def joinpath(self, child):
-        return pathlib.Path(self.root, child)
-
-    def children(self):
-        with suppress(Exception):
-            return os.listdir(self.root or '.')
-        with suppress(Exception):
-            return self.zip_children()
-        return []
-
-    def zip_children(self):
-        zip_path = zipp.Path(self.root)
-        names = zip_path.root.namelist()
-        self.joinpath = zip_path.joinpath
-
-        return dict.fromkeys(child.split(posixpath.sep, 1)[0] for child in names)
-
-    def search(self, name):
-        return self.lookup(self.mtime).search(name)
-
-    @property
-    def mtime(self):
-        with suppress(OSError):
-            return os.stat(self.root).st_mtime
-        self.lookup.cache_clear()
-
-    @method_cache
-    def lookup(self, mtime):
-        return Lookup(self)
-
-
-class Lookup:
-    def __init__(self, path: FastPath):
-        base = os.path.basename(path.root).lower()
-        base_is_egg = base.endswith(".egg")
-        self.infos = FreezableDefaultDict(list)
-        self.eggs = FreezableDefaultDict(list)
-
-        for child in path.children():
-            low = child.lower()
-            if low.endswith((".dist-info", ".egg-info")):
-                # rpartition is faster than splitext and suitable for this purpose.
-                name = low.rpartition(".")[0].partition("-")[0]
-                normalized = Prepared.normalize(name)
-                self.infos[normalized].append(path.joinpath(child))
-            elif base_is_egg and low == "egg-info":
-                name = base.rpartition(".")[0].partition("-")[0]
-                legacy_normalized = Prepared.legacy_normalize(name)
-                self.eggs[legacy_normalized].append(path.joinpath(child))
-
-        self.infos.freeze()
-        self.eggs.freeze()
-
-    def search(self, prepared):
-        infos = (
-            self.infos[prepared.normalized]
-            if prepared
-            else itertools.chain.from_iterable(self.infos.values())
-        )
-        eggs = (
-            self.eggs[prepared.legacy_normalized]
-            if prepared
-            else itertools.chain.from_iterable(self.eggs.values())
-        )
-        return itertools.chain(infos, eggs)
-
-
-class Prepared:
-    """
-    A prepared search for metadata on a possibly-named package.
-    """
-
-    normalized = None
-    legacy_normalized = None
-
-    def __init__(self, name):
-        self.name = name
-        if name is None:
-            return
-        self.normalized = self.normalize(name)
-        self.legacy_normalized = self.legacy_normalize(name)
-
-    @staticmethod
-    def normalize(name):
-        """
-        PEP 503 normalization plus dashes as underscores.
-        """
-        return re.sub(r"[-_.]+", "-", name).lower().replace('-', '_')
-
-    @staticmethod
-    def legacy_normalize(name):
-        """
-        Normalize the package name as found in the convention in
-        older packaging tools versions and specs.
-        """
-        return name.lower().replace('-', '_')
-
-    def __bool__(self):
-        return bool(self.name)
-
-
-@install
-class MetadataPathFinder(NullFinder, DistributionFinder):
-    """A degenerate finder for distribution packages on the file system.
-
-    This finder supplies only a find_distributions() method for versions
-    of Python that do not have a PathFinder find_distributions().
-    """
-
-    def find_distributions(self, context=DistributionFinder.Context()):
-        """
-        Find distributions.
-
-        Return an iterable of all Distribution instances capable of
-        loading the metadata for packages matching ``context.name``
-        (or all names if ``None`` indicated) along the paths in the list
-        of directories ``context.path``.
-        """
-        found = self._search_paths(context.name, context.path)
-        return map(PathDistribution, found)
-
-    @classmethod
-    def _search_paths(cls, name, paths):
-        """Find metadata directories in paths heuristically."""
-        prepared = Prepared(name)
-        return itertools.chain.from_iterable(
-            path.search(prepared) for path in map(FastPath, paths)
-        )
-
-    def invalidate_caches(cls):
-        FastPath.__new__.cache_clear()
-
-
-class PathDistribution(Distribution):
-    def __init__(self, path: SimplePath):
-        """Construct a distribution.
-
-        :param path: SimplePath indicating the metadata directory.
-        """
-        self._path = path
-
-    def read_text(self, filename):
-        with suppress(
-            FileNotFoundError,
-            IsADirectoryError,
-            KeyError,
-            NotADirectoryError,
-            PermissionError,
-        ):
-            return self._path.joinpath(filename).read_text(encoding='utf-8')
-
-    read_text.__doc__ = Distribution.read_text.__doc__
-
-    def locate_file(self, path):
-        return self._path.parent / path
-
-    @property
-    def _normalized_name(self):
-        """
-        Performance optimization: where possible, resolve the
-        normalized name from the file system path.
-        """
-        stem = os.path.basename(str(self._path))
-        return self._name_from_stem(stem) or super()._normalized_name
-
-    def _name_from_stem(self, stem):
-        name, ext = os.path.splitext(stem)
-        if ext not in ('.dist-info', '.egg-info'):
-            return
-        name, sep, rest = stem.partition('-')
-        return name
-
-
-def distribution(distribution_name):
-    """Get the ``Distribution`` instance for the named package.
-
-    :param distribution_name: The name of the distribution package as a string.
-    :return: A ``Distribution`` instance (or subclass thereof).
-    """
-    return Distribution.from_name(distribution_name)
-
-
-def distributions(**kwargs):
-    """Get all ``Distribution`` instances in the current environment.
-
-    :return: An iterable of ``Distribution`` instances.
-    """
-    return Distribution.discover(**kwargs)
-
-
-def metadata(distribution_name) -> _meta.PackageMetadata:
-    """Get the metadata for the named package.
-
-    :param distribution_name: The name of the distribution package to query.
-    :return: A PackageMetadata containing the parsed metadata.
-    """
-    return Distribution.from_name(distribution_name).metadata
-
-
-def version(distribution_name):
-    """Get the version string for the named package.
-
-    :param distribution_name: The name of the distribution package to query.
-    :return: The version string for the package as defined in the package's
-        "Version" metadata key.
-    """
-    return distribution(distribution_name).version
-
-
-def entry_points(**params) -> Union[EntryPoints, SelectableGroups]:
-    """Return EntryPoint objects for all installed packages.
-
-    Pass selection parameters (group or name) to filter the
-    result to entry points matching those properties (see
-    EntryPoints.select()).
-
-    For compatibility, returns ``SelectableGroups`` object unless
-    selection parameters are supplied. In the future, this function
-    will return ``EntryPoints`` instead of ``SelectableGroups``
-    even when no selection parameters are supplied.
-
-    For maximum future compatibility, pass selection parameters
-    or invoke ``.select`` with parameters on the result.
-
-    :return: EntryPoints or SelectableGroups for all installed packages.
-    """
-    norm_name = operator.attrgetter('_normalized_name')
-    unique = functools.partial(unique_everseen, key=norm_name)
-    eps = itertools.chain.from_iterable(
-        dist.entry_points for dist in unique(distributions())
-    )
-    return SelectableGroups.load(eps).select(**params)
-
-
-def files(distribution_name):
-    """Return a list of files for the named package.
-
-    :param distribution_name: The name of the distribution package to query.
-    :return: List of files composing the distribution.
-    """
-    return distribution(distribution_name).files
-
-
-def requires(distribution_name):
-    """
-    Return a list of requirements for the named package.
-
-    :return: An iterator of requirements, suitable for
-        packaging.requirement.Requirement.
-    """
-    return distribution(distribution_name).requires
-
-
-def packages_distributions() -> Mapping[str, List[str]]:
-    """
-    Return a mapping of top-level packages to their
-    distributions.
-
-    >>> import collections.abc
-    >>> pkgs = packages_distributions()
-    >>> all(isinstance(dist, collections.abc.Sequence) for dist in pkgs.values())
-    True
-    """
-    pkg_to_dist = collections.defaultdict(list)
-    for dist in distributions():
-        for pkg in _top_level_declared(dist) or _top_level_inferred(dist):
-            pkg_to_dist[pkg].append(dist.metadata['Name'])
-    return dict(pkg_to_dist)
-
-
-def _top_level_declared(dist):
-    return (dist.read_text('top_level.txt') or '').split()
-
-
-def _top_level_inferred(dist):
-    return {
-        f.parts[0] if len(f.parts) > 1 else f.with_suffix('').name
-        for f in always_iterable(dist.files)
-        if f.suffix == ".py"
-    }
+import os
+import re
+import abc
+import csv
+import sys
+from sitecustomize._vendor import zipp
+import email
+import pathlib
+import operator
+import textwrap
+import warnings
+import functools
+import itertools
+import posixpath
+import collections
+
+from . import _adapters, _meta
+from ._collections import FreezableDefaultDict, Pair
+from ._compat import (
+    NullFinder,
+    install,
+    pypy_partial,
+)
+from ._functools import method_cache, pass_none
+from ._itertools import always_iterable, unique_everseen
+from ._meta import PackageMetadata, SimplePath
+
+from contextlib import suppress
+from importlib import import_module
+from importlib.abc import MetaPathFinder
+from itertools import starmap
+from typing import List, Mapping, Optional, Union
+
+
+__all__ = [
+    'Distribution',
+    'DistributionFinder',
+    'PackageMetadata',
+    'PackageNotFoundError',
+    'distribution',
+    'distributions',
+    'entry_points',
+    'files',
+    'metadata',
+    'packages_distributions',
+    'requires',
+    'version',
+]
+
+
+class PackageNotFoundError(ModuleNotFoundError):
+    """The package was not found."""
+
+    def __str__(self):
+        return f"No package metadata was found for {self.name}"
+
+    @property
+    def name(self):
+        (name,) = self.args
+        return name
+
+
+class Sectioned:
+    """
+    A simple entry point config parser for performance
+
+    >>> for item in Sectioned.read(Sectioned._sample):
+    ...     print(item)
+    Pair(name='sec1', value='# comments ignored')
+    Pair(name='sec1', value='a = 1')
+    Pair(name='sec1', value='b = 2')
+    Pair(name='sec2', value='a = 2')
+
+    >>> res = Sectioned.section_pairs(Sectioned._sample)
+    >>> item = next(res)
+    >>> item.name
+    'sec1'
+    >>> item.value
+    Pair(name='a', value='1')
+    >>> item = next(res)
+    >>> item.value
+    Pair(name='b', value='2')
+    >>> item = next(res)
+    >>> item.name
+    'sec2'
+    >>> item.value
+    Pair(name='a', value='2')
+    >>> list(res)
+    []
+    """
+
+    _sample = textwrap.dedent(
+        """
+        [sec1]
+        # comments ignored
+        a = 1
+        b = 2
+
+        [sec2]
+        a = 2
+        """
+    ).lstrip()
+
+    @classmethod
+    def section_pairs(cls, text):
+        return (
+            section._replace(value=Pair.parse(section.value))
+            for section in cls.read(text, filter_=cls.valid)
+            if section.name is not None
+        )
+
+    @staticmethod
+    def read(text, filter_=None):
+        lines = filter(filter_, map(str.strip, text.splitlines()))
+        name = None
+        for value in lines:
+            section_match = value.startswith('[') and value.endswith(']')
+            if section_match:
+                name = value.strip('[]')
+                continue
+            yield Pair(name, value)
+
+    @staticmethod
+    def valid(line):
+        return line and not line.startswith('#')
+
+
+class DeprecatedTuple:
+    """
+    Provide subscript item access for backward compatibility.
+
+    >>> recwarn = getfixture('recwarn')
+    >>> ep = EntryPoint(name='name', value='value', group='group')
+    >>> ep[:]
+    ('name', 'value', 'group')
+    >>> ep[0]
+    'name'
+    >>> len(recwarn)
+    1
+    """
+
+    _warn = functools.partial(
+        warnings.warn,
+        "EntryPoint tuple interface is deprecated. Access members by name.",
+        DeprecationWarning,
+        stacklevel=pypy_partial(2),
+    )
+
+    def __getitem__(self, item):
+        self._warn()
+        return self._key()[item]
+
+
+class EntryPoint(DeprecatedTuple):
+    """An entry point as defined by Python packaging conventions.
+
+    See `the packaging docs on entry points
+    <https://packaging.python.org/specifications/entry-points/>`_
+    for more information.
+
+    >>> ep = EntryPoint(
+    ...     name=None, group=None, value='package.module:attr [extra1, extra2]')
+    >>> ep.module
+    'package.module'
+    >>> ep.attr
+    'attr'
+    >>> ep.extras
+    ['extra1', 'extra2']
+    """
+
+    pattern = re.compile(
+        r'(?P<module>[\w.]+)\s*'
+        r'(:\s*(?P<attr>[\w.]+)\s*)?'
+        r'((?P<extras>\[.*\])\s*)?$'
+    )
+    """
+    A regular expression describing the syntax for an entry point,
+    which might look like:
+
+        - module
+        - package.module
+        - package.module:attribute
+        - package.module:object.attribute
+        - package.module:attr [extra1, extra2]
+
+    Other combinations are possible as well.
+
+    The expression is lenient about whitespace around the ':',
+    following the attr, and following any extras.
+    """
+
+    dist: Optional['Distribution'] = None
+
+    def __init__(self, name, value, group):
+        vars(self).update(name=name, value=value, group=group)
+
+    def load(self):
+        """Load the entry point from its definition. If only a module
+        is indicated by the value, return that module. Otherwise,
+        return the named object.
+        """
+        match = self.pattern.match(self.value)
+        module = import_module(match.group('module'))
+        attrs = filter(None, (match.group('attr') or '').split('.'))
+        return functools.reduce(getattr, attrs, module)
+
+    @property
+    def module(self):
+        match = self.pattern.match(self.value)
+        return match.group('module')
+
+    @property
+    def attr(self):
+        match = self.pattern.match(self.value)
+        return match.group('attr')
+
+    @property
+    def extras(self):
+        match = self.pattern.match(self.value)
+        return re.findall(r'\w+', match.group('extras') or '')
+
+    def _for(self, dist):
+        vars(self).update(dist=dist)
+        return self
+
+    def __iter__(self):
+        """
+        Supply iter so one may construct dicts of EntryPoints by name.
+        """
+        msg = (
+            "Construction of dict of EntryPoints is deprecated in "
+            "favor of EntryPoints."
+        )
+        warnings.warn(msg, DeprecationWarning)
+        return iter((self.name, self))
+
+    def matches(self, **params):
+        """
+        EntryPoint matches the given parameters.
+
+        >>> ep = EntryPoint(group='foo', name='bar', value='bing:bong [extra1, extra2]')
+        >>> ep.matches(group='foo')
+        True
+        >>> ep.matches(name='bar', value='bing:bong [extra1, extra2]')
+        True
+        >>> ep.matches(group='foo', name='other')
+        False
+        >>> ep.matches()
+        True
+        >>> ep.matches(extras=['extra1', 'extra2'])
+        True
+        >>> ep.matches(module='bing')
+        True
+        >>> ep.matches(attr='bong')
+        True
+        """
+        attrs = (getattr(self, param) for param in params)
+        return all(map(operator.eq, params.values(), attrs))
+
+    def _key(self):
+        return self.name, self.value, self.group
+
+    def __lt__(self, other):
+        return self._key() < other._key()
+
+    def __eq__(self, other):
+        return self._key() == other._key()
+
+    def __setattr__(self, name, value):
+        raise AttributeError("EntryPoint objects are immutable.")
+
+    def __repr__(self):
+        return (
+            f'EntryPoint(name={self.name!r}, value={self.value!r}, '
+            f'group={self.group!r})'
+        )
+
+    def __hash__(self):
+        return hash(self._key())
+
+
+class DeprecatedList(list):
+    """
+    Allow an otherwise immutable object to implement mutability
+    for compatibility.
+
+    >>> recwarn = getfixture('recwarn')
+    >>> dl = DeprecatedList(range(3))
+    >>> dl[0] = 1
+    >>> dl.append(3)
+    >>> del dl[3]
+    >>> dl.reverse()
+    >>> dl.sort()
+    >>> dl.extend([4])
+    >>> dl.pop(-1)
+    4
+    >>> dl.remove(1)
+    >>> dl += [5]
+    >>> dl + [6]
+    [1, 2, 5, 6]
+    >>> dl + (6,)
+    [1, 2, 5, 6]
+    >>> dl.insert(0, 0)
+    >>> dl
+    [0, 1, 2, 5]
+    >>> dl == [0, 1, 2, 5]
+    True
+    >>> dl == (0, 1, 2, 5)
+    True
+    >>> len(recwarn)
+    1
+    """
+
+    __slots__ = ()
+
+    _warn = functools.partial(
+        warnings.warn,
+        "EntryPoints list interface is deprecated. Cast to list if needed.",
+        DeprecationWarning,
+        stacklevel=pypy_partial(2),
+    )
+
+    def _wrap_deprecated_method(method_name: str):  # type: ignore
+        def wrapped(self, *args, **kwargs):
+            self._warn()
+            return getattr(super(), method_name)(*args, **kwargs)
+
+        return method_name, wrapped
+
+    locals().update(
+        map(
+            _wrap_deprecated_method,
+            '__setitem__ __delitem__ append reverse extend pop remove '
+            '__iadd__ insert sort'.split(),
+        )
+    )
+
+    def __add__(self, other):
+        if not isinstance(other, tuple):
+            self._warn()
+            other = tuple(other)
+        return self.__class__(tuple(self) + other)
+
+    def __eq__(self, other):
+        if not isinstance(other, tuple):
+            self._warn()
+            other = tuple(other)
+
+        return tuple(self).__eq__(other)
+
+
+class EntryPoints(DeprecatedList):
+    """
+    An immutable collection of selectable EntryPoint objects.
+    """
+
+    __slots__ = ()
+
+    def __getitem__(self, name):  # -> EntryPoint:
+        """
+        Get the EntryPoint in self matching name.
+        """
+        if isinstance(name, int):
+            warnings.warn(
+                "Accessing entry points by index is deprecated. "
+                "Cast to tuple if needed.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            return super().__getitem__(name)
+        try:
+            return next(iter(self.select(name=name)))
+        except StopIteration:
+            raise KeyError(name)
+
+    def select(self, **params):
+        """
+        Select entry points from self that match the
+        given parameters (typically group and/or name).
+        """
+        return EntryPoints(ep for ep in self if ep.matches(**params))
+
+    @property
+    def names(self):
+        """
+        Return the set of all names of all entry points.
+        """
+        return {ep.name for ep in self}
+
+    @property
+    def groups(self):
+        """
+        Return the set of all groups of all entry points.
+
+        For coverage while SelectableGroups is present.
+        >>> EntryPoints().groups
+        set()
+        """
+        return {ep.group for ep in self}
+
+    @classmethod
+    def _from_text_for(cls, text, dist):
+        return cls(ep._for(dist) for ep in cls._from_text(text))
+
+    @staticmethod
+    def _from_text(text):
+        return (
+            EntryPoint(name=item.value.name, value=item.value.value, group=item.name)
+            for item in Sectioned.section_pairs(text or '')
+        )
+
+
+class Deprecated:
+    """
+    Compatibility add-in for mapping to indicate that
+    mapping behavior is deprecated.
+
+    >>> recwarn = getfixture('recwarn')
+    >>> class DeprecatedDict(Deprecated, dict): pass
+    >>> dd = DeprecatedDict(foo='bar')
+    >>> dd.get('baz', None)
+    >>> dd['foo']
+    'bar'
+    >>> list(dd)
+    ['foo']
+    >>> list(dd.keys())
+    ['foo']
+    >>> 'foo' in dd
+    True
+    >>> list(dd.values())
+    ['bar']
+    >>> len(recwarn)
+    1
+    """
+
+    _warn = functools.partial(
+        warnings.warn,
+        "SelectableGroups dict interface is deprecated. Use select.",
+        DeprecationWarning,
+        stacklevel=pypy_partial(2),
+    )
+
+    def __getitem__(self, name):
+        self._warn()
+        return super().__getitem__(name)
+
+    def get(self, name, default=None):
+        self._warn()
+        return super().get(name, default)
+
+    def __iter__(self):
+        self._warn()
+        return super().__iter__()
+
+    def __contains__(self, *args):
+        self._warn()
+        return super().__contains__(*args)
+
+    def keys(self):
+        self._warn()
+        return super().keys()
+
+    def values(self):
+        self._warn()
+        return super().values()
+
+
+class SelectableGroups(Deprecated, dict):
+    """
+    A backward- and forward-compatible result from
+    entry_points that fully implements the dict interface.
+    """
+
+    @classmethod
+    def load(cls, eps):
+        by_group = operator.attrgetter('group')
+        ordered = sorted(eps, key=by_group)
+        grouped = itertools.groupby(ordered, by_group)
+        return cls((group, EntryPoints(eps)) for group, eps in grouped)
+
+    @property
+    def _all(self):
+        """
+        Reconstruct a list of all entrypoints from the groups.
+        """
+        groups = super(Deprecated, self).values()
+        return EntryPoints(itertools.chain.from_iterable(groups))
+
+    @property
+    def groups(self):
+        return self._all.groups
+
+    @property
+    def names(self):
+        """
+        for coverage:
+        >>> SelectableGroups().names
+        set()
+        """
+        return self._all.names
+
+    def select(self, **params):
+        if not params:
+            return self
+        return self._all.select(**params)
+
+
+class PackagePath(pathlib.PurePosixPath):
+    """A reference to a path in a package"""
+
+    def read_text(self, encoding='utf-8'):
+        with self.locate().open(encoding=encoding) as stream:
+            return stream.read()
+
+    def read_binary(self):
+        with self.locate().open('rb') as stream:
+            return stream.read()
+
+    def locate(self):
+        """Return a path-like object for this path"""
+        return self.dist.locate_file(self)
+
+
+class FileHash:
+    def __init__(self, spec):
+        self.mode, _, self.value = spec.partition('=')
+
+    def __repr__(self):
+        return f'<FileHash mode: {self.mode} value: {self.value}>'
+
+
+class Distribution:
+    """A Python distribution package."""
+
+    @abc.abstractmethod
+    def read_text(self, filename):
+        """Attempt to load metadata file given by the name.
+
+        :param filename: The name of the file in the distribution info.
+        :return: The text if found, otherwise None.
+        """
+
+    @abc.abstractmethod
+    def locate_file(self, path):
+        """
+        Given a path to a file in this distribution, return a path
+        to it.
+        """
+
+    @classmethod
+    def from_name(cls, name):
+        """Return the Distribution for the given package name.
+
+        :param name: The name of the distribution package to search for.
+        :return: The Distribution instance (or subclass thereof) for the named
+            package, if found.
+        :raises PackageNotFoundError: When the named package's distribution
+            metadata cannot be found.
+        """
+        for resolver in cls._discover_resolvers():
+            dists = resolver(DistributionFinder.Context(name=name))
+            dist = next(iter(dists), None)
+            if dist is not None:
+                return dist
+        else:
+            raise PackageNotFoundError(name)
+
+    @classmethod
+    def discover(cls, **kwargs):
+        """Return an iterable of Distribution objects for all packages.
+
+        Pass a ``context`` or pass keyword arguments for constructing
+        a context.
+
+        :context: A ``DistributionFinder.Context`` object.
+        :return: Iterable of Distribution objects for all packages.
+        """
+        context = kwargs.pop('context', None)
+        if context and kwargs:
+            raise ValueError("cannot accept context and kwargs")
+        context = context or DistributionFinder.Context(**kwargs)
+        return itertools.chain.from_iterable(
+            resolver(context) for resolver in cls._discover_resolvers()
+        )
+
+    @staticmethod
+    def at(path):
+        """Return a Distribution for the indicated metadata path
+
+        :param path: a string or path-like object
+        :return: a concrete Distribution instance for the path
+        """
+        return PathDistribution(pathlib.Path(path))
+
+    @staticmethod
+    def _discover_resolvers():
+        """Search the meta_path for resolvers."""
+        declared = (
+            getattr(finder, 'find_distributions', None) for finder in sys.meta_path
+        )
+        return filter(None, declared)
+
+    @property
+    def metadata(self) -> _meta.PackageMetadata:
+        """Return the parsed metadata for this Distribution.
+
+        The returned object will have keys that name the various bits of
+        metadata.  See PEP 566 for details.
+        """
+        text = (
+            self.read_text('METADATA')
+            or self.read_text('PKG-INFO')
+            # This last clause is here to support old egg-info files.  Its
+            # effect is to just end up using the PathDistribution's self._path
+            # (which points to the egg-info file) attribute unchanged.
+            or self.read_text('')
+        )
+        return _adapters.Message(email.message_from_string(text))
+
+    @property
+    def name(self):
+        """Return the 'Name' metadata for the distribution package."""
+        return self.metadata['Name']
+
+    @property
+    def _normalized_name(self):
+        """Return a normalized version of the name."""
+        return Prepared.normalize(self.name)
+
+    @property
+    def version(self):
+        """Return the 'Version' metadata for the distribution package."""
+        return self.metadata['Version']
+
+    @property
+    def entry_points(self):
+        return EntryPoints._from_text_for(self.read_text('entry_points.txt'), self)
+
+    @property
+    def files(self):
+        """Files in this distribution.
+
+        :return: List of PackagePath for this distribution or None
+
+        Result is `None` if the metadata file that enumerates files
+        (i.e. RECORD for dist-info or SOURCES.txt for egg-info) is
+        missing.
+        Result may be empty if the metadata exists but is empty.
+        """
+
+        def make_file(name, hash=None, size_str=None):
+            result = PackagePath(name)
+            result.hash = FileHash(hash) if hash else None
+            result.size = int(size_str) if size_str else None
+            result.dist = self
+            return result
+
+        @pass_none
+        def make_files(lines):
+            return list(starmap(make_file, csv.reader(lines)))
+
+        return make_files(self._read_files_distinfo() or self._read_files_egginfo())
+
+    def _read_files_distinfo(self):
+        """
+        Read the lines of RECORD
+        """
+        text = self.read_text('RECORD')
+        return text and text.splitlines()
+
+    def _read_files_egginfo(self):
+        """
+        SOURCES.txt might contain literal commas, so wrap each line
+        in quotes.
+        """
+        text = self.read_text('SOURCES.txt')
+        return text and map('"{}"'.format, text.splitlines())
+
+    @property
+    def requires(self):
+        """Generated requirements specified for this Distribution"""
+        reqs = self._read_dist_info_reqs() or self._read_egg_info_reqs()
+        return reqs and list(reqs)
+
+    def _read_dist_info_reqs(self):
+        return self.metadata.get_all('Requires-Dist')
+
+    def _read_egg_info_reqs(self):
+        source = self.read_text('requires.txt')
+        return pass_none(self._deps_from_requires_text)(source)
+
+    @classmethod
+    def _deps_from_requires_text(cls, source):
+        return cls._convert_egg_info_reqs_to_simple_reqs(Sectioned.read(source))
+
+    @staticmethod
+    def _convert_egg_info_reqs_to_simple_reqs(sections):
+        """
+        Historically, setuptools would solicit and store 'extra'
+        requirements, including those with environment markers,
+        in separate sections. More modern tools expect each
+        dependency to be defined separately, with any relevant
+        extras and environment markers attached directly to that
+        requirement. This method converts the former to the
+        latter. See _test_deps_from_requires_text for an example.
+        """
+
+        def make_condition(name):
+            return name and f'extra == "{name}"'
+
+        def quoted_marker(section):
+            section = section or ''
+            extra, sep, markers = section.partition(':')
+            if extra and markers:
+                markers = f'({markers})'
+            conditions = list(filter(None, [markers, make_condition(extra)]))
+            return '; ' + ' and '.join(conditions) if conditions else ''
+
+        def url_req_space(req):
+            """
+            PEP 508 requires a space between the url_spec and the quoted_marker.
+            Ref python/importlib_metadata#357.
+            """
+            # '@' is uniquely indicative of a url_req.
+            return ' ' * ('@' in req)
+
+        for section in sections:
+            space = url_req_space(section.value)
+            yield section.value + space + quoted_marker(section.name)
+
+
+class DistributionFinder(MetaPathFinder):
+    """
+    A MetaPathFinder capable of discovering installed distributions.
+    """
+
+    class Context:
+        """
+        Keyword arguments presented by the caller to
+        ``distributions()`` or ``Distribution.discover()``
+        to narrow the scope of a search for distributions
+        in all DistributionFinders.
+
+        Each DistributionFinder may expect any parameters
+        and should attempt to honor the canonical
+        parameters defined below when appropriate.
+        """
+
+        name = None
+        """
+        Specific name for which a distribution finder should match.
+        A name of ``None`` matches all distributions.
+        """
+
+        def __init__(self, **kwargs):
+            vars(self).update(kwargs)
+
+        @property
+        def path(self):
+            """
+            The sequence of directory path that a distribution finder
+            should search.
+
+            Typically refers to Python installed package paths such as
+            "site-packages" directories and defaults to ``sys.path``.
+            """
+            return vars(self).get('path', sys.path)
+
+    @abc.abstractmethod
+    def find_distributions(self, context=Context()):
+        """
+        Find distributions.
+
+        Return an iterable of all Distribution instances capable of
+        loading the metadata for packages matching the ``context``,
+        a DistributionFinder.Context instance.
+        """
+
+
+class FastPath:
+    """
+    Micro-optimized class for searching a path for
+    children.
+
+    >>> FastPath('').children()
+    ['...']
+    """
+
+    @functools.lru_cache()  # type: ignore
+    def __new__(cls, root):
+        return super().__new__(cls)
+
+    def __init__(self, root):
+        self.root = root
+
+    def joinpath(self, child):
+        return pathlib.Path(self.root, child)
+
+    def children(self):
+        with suppress(Exception):
+            return os.listdir(self.root or '.')
+        with suppress(Exception):
+            return self.zip_children()
+        return []
+
+    def zip_children(self):
+        zip_path = zipp.Path(self.root)
+        names = zip_path.root.namelist()
+        self.joinpath = zip_path.joinpath
+
+        return dict.fromkeys(child.split(posixpath.sep, 1)[0] for child in names)
+
+    def search(self, name):
+        return self.lookup(self.mtime).search(name)
+
+    @property
+    def mtime(self):
+        with suppress(OSError):
+            return os.stat(self.root).st_mtime
+        self.lookup.cache_clear()
+
+    @method_cache
+    def lookup(self, mtime):
+        return Lookup(self)
+
+
+class Lookup:
+    def __init__(self, path: FastPath):
+        base = os.path.basename(path.root).lower()
+        base_is_egg = base.endswith(".egg")
+        self.infos = FreezableDefaultDict(list)
+        self.eggs = FreezableDefaultDict(list)
+
+        for child in path.children():
+            low = child.lower()
+            if low.endswith((".dist-info", ".egg-info")):
+                # rpartition is faster than splitext and suitable for this purpose.
+                name = low.rpartition(".")[0].partition("-")[0]
+                normalized = Prepared.normalize(name)
+                self.infos[normalized].append(path.joinpath(child))
+            elif base_is_egg and low == "egg-info":
+                name = base.rpartition(".")[0].partition("-")[0]
+                legacy_normalized = Prepared.legacy_normalize(name)
+                self.eggs[legacy_normalized].append(path.joinpath(child))
+
+        self.infos.freeze()
+        self.eggs.freeze()
+
+    def search(self, prepared):
+        infos = (
+            self.infos[prepared.normalized]
+            if prepared
+            else itertools.chain.from_iterable(self.infos.values())
+        )
+        eggs = (
+            self.eggs[prepared.legacy_normalized]
+            if prepared
+            else itertools.chain.from_iterable(self.eggs.values())
+        )
+        return itertools.chain(infos, eggs)
+
+
+class Prepared:
+    """
+    A prepared search for metadata on a possibly-named package.
+    """
+
+    normalized = None
+    legacy_normalized = None
+
+    def __init__(self, name):
+        self.name = name
+        if name is None:
+            return
+        self.normalized = self.normalize(name)
+        self.legacy_normalized = self.legacy_normalize(name)
+
+    @staticmethod
+    def normalize(name):
+        """
+        PEP 503 normalization plus dashes as underscores.
+        """
+        return re.sub(r"[-_.]+", "-", name).lower().replace('-', '_')
+
+    @staticmethod
+    def legacy_normalize(name):
+        """
+        Normalize the package name as found in the convention in
+        older packaging tools versions and specs.
+        """
+        return name.lower().replace('-', '_')
+
+    def __bool__(self):
+        return bool(self.name)
+
+
+@install
+class MetadataPathFinder(NullFinder, DistributionFinder):
+    """A degenerate finder for distribution packages on the file system.
+
+    This finder supplies only a find_distributions() method for versions
+    of Python that do not have a PathFinder find_distributions().
+    """
+
+    def find_distributions(self, context=DistributionFinder.Context()):
+        """
+        Find distributions.
+
+        Return an iterable of all Distribution instances capable of
+        loading the metadata for packages matching ``context.name``
+        (or all names if ``None`` indicated) along the paths in the list
+        of directories ``context.path``.
+        """
+        found = self._search_paths(context.name, context.path)
+        return map(PathDistribution, found)
+
+    @classmethod
+    def _search_paths(cls, name, paths):
+        """Find metadata directories in paths heuristically."""
+        prepared = Prepared(name)
+        return itertools.chain.from_iterable(
+            path.search(prepared) for path in map(FastPath, paths)
+        )
+
+    def invalidate_caches(cls):
+        FastPath.__new__.cache_clear()
+
+
+class PathDistribution(Distribution):
+    def __init__(self, path: SimplePath):
+        """Construct a distribution.
+
+        :param path: SimplePath indicating the metadata directory.
+        """
+        self._path = path
+
+    def read_text(self, filename):
+        with suppress(
+            FileNotFoundError,
+            IsADirectoryError,
+            KeyError,
+            NotADirectoryError,
+            PermissionError,
+        ):
+            return self._path.joinpath(filename).read_text(encoding='utf-8')
+
+    read_text.__doc__ = Distribution.read_text.__doc__
+
+    def locate_file(self, path):
+        return self._path.parent / path
+
+    @property
+    def _normalized_name(self):
+        """
+        Performance optimization: where possible, resolve the
+        normalized name from the file system path.
+        """
+        stem = os.path.basename(str(self._path))
+        return self._name_from_stem(stem) or super()._normalized_name
+
+    def _name_from_stem(self, stem):
+        name, ext = os.path.splitext(stem)
+        if ext not in ('.dist-info', '.egg-info'):
+            return
+        name, sep, rest = stem.partition('-')
+        return name
+
+
+def distribution(distribution_name):
+    """Get the ``Distribution`` instance for the named package.
+
+    :param distribution_name: The name of the distribution package as a string.
+    :return: A ``Distribution`` instance (or subclass thereof).
+    """
+    return Distribution.from_name(distribution_name)
+
+
+def distributions(**kwargs):
+    """Get all ``Distribution`` instances in the current environment.
+
+    :return: An iterable of ``Distribution`` instances.
+    """
+    return Distribution.discover(**kwargs)
+
+
+def metadata(distribution_name) -> _meta.PackageMetadata:
+    """Get the metadata for the named package.
+
+    :param distribution_name: The name of the distribution package to query.
+    :return: A PackageMetadata containing the parsed metadata.
+    """
+    return Distribution.from_name(distribution_name).metadata
+
+
+def version(distribution_name):
+    """Get the version string for the named package.
+
+    :param distribution_name: The name of the distribution package to query.
+    :return: The version string for the package as defined in the package's
+        "Version" metadata key.
+    """
+    return distribution(distribution_name).version
+
+
+def entry_points(**params) -> Union[EntryPoints, SelectableGroups]:
+    """Return EntryPoint objects for all installed packages.
+
+    Pass selection parameters (group or name) to filter the
+    result to entry points matching those properties (see
+    EntryPoints.select()).
+
+    For compatibility, returns ``SelectableGroups`` object unless
+    selection parameters are supplied. In the future, this function
+    will return ``EntryPoints`` instead of ``SelectableGroups``
+    even when no selection parameters are supplied.
+
+    For maximum future compatibility, pass selection parameters
+    or invoke ``.select`` with parameters on the result.
+
+    :return: EntryPoints or SelectableGroups for all installed packages.
+    """
+    norm_name = operator.attrgetter('_normalized_name')
+    unique = functools.partial(unique_everseen, key=norm_name)
+    eps = itertools.chain.from_iterable(
+        dist.entry_points for dist in unique(distributions())
+    )
+    return SelectableGroups.load(eps).select(**params)
+
+
+def files(distribution_name):
+    """Return a list of files for the named package.
+
+    :param distribution_name: The name of the distribution package to query.
+    :return: List of files composing the distribution.
+    """
+    return distribution(distribution_name).files
+
+
+def requires(distribution_name):
+    """
+    Return a list of requirements for the named package.
+
+    :return: An iterator of requirements, suitable for
+        packaging.requirement.Requirement.
+    """
+    return distribution(distribution_name).requires
+
+
+def packages_distributions() -> Mapping[str, List[str]]:
+    """
+    Return a mapping of top-level packages to their
+    distributions.
+
+    >>> import collections.abc
+    >>> pkgs = packages_distributions()
+    >>> all(isinstance(dist, collections.abc.Sequence) for dist in pkgs.values())
+    True
+    """
+    pkg_to_dist = collections.defaultdict(list)
+    for dist in distributions():
+        for pkg in _top_level_declared(dist) or _top_level_inferred(dist):
+            pkg_to_dist[pkg].append(dist.metadata['Name'])
+    return dict(pkg_to_dist)
+
+
+def _top_level_declared(dist):
+    return (dist.read_text('top_level.txt') or '').split()
+
+
+def _top_level_inferred(dist):
+    return {
+        f.parts[0] if len(f.parts) > 1 else f.with_suffix('').name
+        for f in always_iterable(dist.files)
+        if f.suffix == ".py"
+    }
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_adapters.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_adapters.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import re
-import textwrap
-import email.message
-
-from ._text import FoldedCase
-
-
-class Message(email.message.Message):
-    multiple_use_keys = set(
-        map(
-            FoldedCase,
-            [
-                'Classifier',
-                'Obsoletes-Dist',
-                'Platform',
-                'Project-URL',
-                'Provides-Dist',
-                'Provides-Extra',
-                'Requires-Dist',
-                'Requires-External',
-                'Supported-Platform',
-                'Dynamic',
-            ],
-        )
-    )
-    """
-    Keys that may be indicated multiple times per PEP 566.
-    """
-
-    def __new__(cls, orig: email.message.Message):
-        res = super().__new__(cls)
-        vars(res).update(vars(orig))
-        return res
-
-    def __init__(self, *args, **kwargs):
-        self._headers = self._repair_headers()
-
-    # suppress spurious error from mypy
-    def __iter__(self):
-        return super().__iter__()
-
-    def _repair_headers(self):
-        def redent(value):
-            "Correct for RFC822 indentation"
-            if not value or '\n' not in value:
-                return value
-            return textwrap.dedent(' ' * 8 + value)
-
-        headers = [(key, redent(value)) for key, value in vars(self)['_headers']]
-        if self._payload:
-            headers.append(('Description', self.get_payload()))
-        return headers
-
-    @property
-    def json(self):
-        """
-        Convert PackageMetadata to a JSON-compatible format
-        per PEP 0566.
-        """
-
-        def transform(key):
-            value = self.get_all(key) if key in self.multiple_use_keys else self[key]
-            if key == 'Keywords':
-                value = re.split(r'\s+', value)
-            tk = key.lower().replace('-', '_')
-            return tk, value
-
-        return dict(map(transform, map(FoldedCase, self)))
+import re
+import textwrap
+import email.message
+
+from ._text import FoldedCase
+
+
+class Message(email.message.Message):
+    multiple_use_keys = set(
+        map(
+            FoldedCase,
+            [
+                'Classifier',
+                'Obsoletes-Dist',
+                'Platform',
+                'Project-URL',
+                'Provides-Dist',
+                'Provides-Extra',
+                'Requires-Dist',
+                'Requires-External',
+                'Supported-Platform',
+                'Dynamic',
+            ],
+        )
+    )
+    """
+    Keys that may be indicated multiple times per PEP 566.
+    """
+
+    def __new__(cls, orig: email.message.Message):
+        res = super().__new__(cls)
+        vars(res).update(vars(orig))
+        return res
+
+    def __init__(self, *args, **kwargs):
+        self._headers = self._repair_headers()
+
+    # suppress spurious error from mypy
+    def __iter__(self):
+        return super().__iter__()
+
+    def _repair_headers(self):
+        def redent(value):
+            "Correct for RFC822 indentation"
+            if not value or '\n' not in value:
+                return value
+            return textwrap.dedent(' ' * 8 + value)
+
+        headers = [(key, redent(value)) for key, value in vars(self)['_headers']]
+        if self._payload:
+            headers.append(('Description', self.get_payload()))
+        return headers
+
+    @property
+    def json(self):
+        """
+        Convert PackageMetadata to a JSON-compatible format
+        per PEP 0566.
+        """
+
+        def transform(key):
+            value = self.get_all(key) if key in self.multiple_use_keys else self[key]
+            if key == 'Keywords':
+                value = re.split(r'\s+', value)
+            tk = key.lower().replace('-', '_')
+            return tk, value
+
+        return dict(map(transform, map(FoldedCase, self)))
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_collections.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_collections.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import collections
-
-
-# from jaraco.collections 3.3
-class FreezableDefaultDict(collections.defaultdict):
-    """
-    Often it is desirable to prevent the mutation of
-    a default dict after its initial construction, such
-    as to prevent mutation during iteration.
-
-    >>> dd = FreezableDefaultDict(list)
-    >>> dd[0].append('1')
-    >>> dd.freeze()
-    >>> dd[1]
-    []
-    >>> len(dd)
-    1
-    """
-
-    def __missing__(self, key):
-        return getattr(self, '_frozen', super().__missing__)(key)
-
-    def freeze(self):
-        self._frozen = lambda key: self.default_factory()
-
-
-class Pair(collections.namedtuple('Pair', 'name value')):
-    @classmethod
-    def parse(cls, text):
-        return cls(*map(str.strip, text.split("=", 1)))
+import collections
+
+
+# from jaraco.collections 3.3
+class FreezableDefaultDict(collections.defaultdict):
+    """
+    Often it is desirable to prevent the mutation of
+    a default dict after its initial construction, such
+    as to prevent mutation during iteration.
+
+    >>> dd = FreezableDefaultDict(list)
+    >>> dd[0].append('1')
+    >>> dd.freeze()
+    >>> dd[1]
+    []
+    >>> len(dd)
+    1
+    """
+
+    def __missing__(self, key):
+        return getattr(self, '_frozen', super().__missing__)(key)
+
+    def freeze(self):
+        self._frozen = lambda key: self.default_factory()
+
+
+class Pair(collections.namedtuple('Pair', 'name value')):
+    @classmethod
+    def parse(cls, text):
+        return cls(*map(str.strip, text.split("=", 1)))
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_functools.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_functools.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import types
-import functools
-
-
-# from jaraco.functools 3.3
-def method_cache(method, cache_wrapper=None):
-    """
-    Wrap lru_cache to support storing the cache data in the object instances.
-
-    Abstracts the common paradigm where the method explicitly saves an
-    underscore-prefixed protected property on first call and returns that
-    subsequently.
-
-    >>> class MyClass:
-    ...     calls = 0
-    ...
-    ...     @method_cache
-    ...     def method(self, value):
-    ...         self.calls += 1
-    ...         return value
-
-    >>> a = MyClass()
-    >>> a.method(3)
-    3
-    >>> for x in range(75):
-    ...     res = a.method(x)
-    >>> a.calls
-    75
-
-    Note that the apparent behavior will be exactly like that of lru_cache
-    except that the cache is stored on each instance, so values in one
-    instance will not flush values from another, and when an instance is
-    deleted, so are the cached values for that instance.
-
-    >>> b = MyClass()
-    >>> for x in range(35):
-    ...     res = b.method(x)
-    >>> b.calls
-    35
-    >>> a.method(0)
-    0
-    >>> a.calls
-    75
-
-    Note that if method had been decorated with ``functools.lru_cache()``,
-    a.calls would have been 76 (due to the cached value of 0 having been
-    flushed by the 'b' instance).
-
-    Clear the cache with ``.cache_clear()``
-
-    >>> a.method.cache_clear()
-
-    Same for a method that hasn't yet been called.
-
-    >>> c = MyClass()
-    >>> c.method.cache_clear()
-
-    Another cache wrapper may be supplied:
-
-    >>> cache = functools.lru_cache(maxsize=2)
-    >>> MyClass.method2 = method_cache(lambda self: 3, cache_wrapper=cache)
-    >>> a = MyClass()
-    >>> a.method2()
-    3
-
-    Caution - do not subsequently wrap the method with another decorator, such
-    as ``@property``, which changes the semantics of the function.
-
-    See also
-    http://code.activestate.com/recipes/577452-a-memoize-decorator-for-instance-methods/
-    for another implementation and additional justification.
-    """
-    cache_wrapper = cache_wrapper or functools.lru_cache()
-
-    def wrapper(self, *args, **kwargs):
-        # it's the first call, replace the method with a cached, bound method
-        bound_method = types.MethodType(method, self)
-        cached_method = cache_wrapper(bound_method)
-        setattr(self, method.__name__, cached_method)
-        return cached_method(*args, **kwargs)
-
-    # Support cache clear even before cache has been created.
-    wrapper.cache_clear = lambda: None
-
-    return wrapper
-
-
-# From jaraco.functools 3.3
-def pass_none(func):
-    """
-    Wrap func so it's not called if its first param is None
-
-    >>> print_text = pass_none(print)
-    >>> print_text('text')
-    text
-    >>> print_text(None)
-    """
-
-    @functools.wraps(func)
-    def wrapper(param, *args, **kwargs):
-        if param is not None:
-            return func(param, *args, **kwargs)
-
-    return wrapper
+import types
+import functools
+
+
+# from jaraco.functools 3.3
+def method_cache(method, cache_wrapper=None):
+    """
+    Wrap lru_cache to support storing the cache data in the object instances.
+
+    Abstracts the common paradigm where the method explicitly saves an
+    underscore-prefixed protected property on first call and returns that
+    subsequently.
+
+    >>> class MyClass:
+    ...     calls = 0
+    ...
+    ...     @method_cache
+    ...     def method(self, value):
+    ...         self.calls += 1
+    ...         return value
+
+    >>> a = MyClass()
+    >>> a.method(3)
+    3
+    >>> for x in range(75):
+    ...     res = a.method(x)
+    >>> a.calls
+    75
+
+    Note that the apparent behavior will be exactly like that of lru_cache
+    except that the cache is stored on each instance, so values in one
+    instance will not flush values from another, and when an instance is
+    deleted, so are the cached values for that instance.
+
+    >>> b = MyClass()
+    >>> for x in range(35):
+    ...     res = b.method(x)
+    >>> b.calls
+    35
+    >>> a.method(0)
+    0
+    >>> a.calls
+    75
+
+    Note that if method had been decorated with ``functools.lru_cache()``,
+    a.calls would have been 76 (due to the cached value of 0 having been
+    flushed by the 'b' instance).
+
+    Clear the cache with ``.cache_clear()``
+
+    >>> a.method.cache_clear()
+
+    Same for a method that hasn't yet been called.
+
+    >>> c = MyClass()
+    >>> c.method.cache_clear()
+
+    Another cache wrapper may be supplied:
+
+    >>> cache = functools.lru_cache(maxsize=2)
+    >>> MyClass.method2 = method_cache(lambda self: 3, cache_wrapper=cache)
+    >>> a = MyClass()
+    >>> a.method2()
+    3
+
+    Caution - do not subsequently wrap the method with another decorator, such
+    as ``@property``, which changes the semantics of the function.
+
+    See also
+    http://code.activestate.com/recipes/577452-a-memoize-decorator-for-instance-methods/
+    for another implementation and additional justification.
+    """
+    cache_wrapper = cache_wrapper or functools.lru_cache()
+
+    def wrapper(self, *args, **kwargs):
+        # it's the first call, replace the method with a cached, bound method
+        bound_method = types.MethodType(method, self)
+        cached_method = cache_wrapper(bound_method)
+        setattr(self, method.__name__, cached_method)
+        return cached_method(*args, **kwargs)
+
+    # Support cache clear even before cache has been created.
+    wrapper.cache_clear = lambda: None
+
+    return wrapper
+
+
+# From jaraco.functools 3.3
+def pass_none(func):
+    """
+    Wrap func so it's not called if its first param is None
+
+    >>> print_text = pass_none(print)
+    >>> print_text('text')
+    text
+    >>> print_text(None)
+    """
+
+    @functools.wraps(func)
+    def wrapper(param, *args, **kwargs):
+        if param is not None:
+            return func(param, *args, **kwargs)
+
+    return wrapper
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_itertools.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_itertools.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from itertools import filterfalse
-
-
-def unique_everseen(iterable, key=None):
-    "List unique elements, preserving order. Remember all elements ever seen."
-    # unique_everseen('AAAABBBCCDAABBB') --> A B C D
-    # unique_everseen('ABBCcAD', str.lower) --> A B C D
-    seen = set()
-    seen_add = seen.add
-    if key is None:
-        for element in filterfalse(seen.__contains__, iterable):
-            seen_add(element)
-            yield element
-    else:
-        for element in iterable:
-            k = key(element)
-            if k not in seen:
-                seen_add(k)
-                yield element
-
-
-# copied from more_itertools 8.8
-def always_iterable(obj, base_type=(str, bytes)):
-    """If *obj* is iterable, return an iterator over its items::
-
-        >>> obj = (1, 2, 3)
-        >>> list(always_iterable(obj))
-        [1, 2, 3]
-
-    If *obj* is not iterable, return a one-item iterable containing *obj*::
-
-        >>> obj = 1
-        >>> list(always_iterable(obj))
-        [1]
-
-    If *obj* is ``None``, return an empty iterable:
-
-        >>> obj = None
-        >>> list(always_iterable(None))
-        []
-
-    By default, binary and text strings are not considered iterable::
-
-        >>> obj = 'foo'
-        >>> list(always_iterable(obj))
-        ['foo']
-
-    If *base_type* is set, objects for which ``isinstance(obj, base_type)``
-    returns ``True`` won't be considered iterable.
-
-        >>> obj = {'a': 1}
-        >>> list(always_iterable(obj))  # Iterate over the dict's keys
-        ['a']
-        >>> list(always_iterable(obj, base_type=dict))  # Treat dicts as a unit
-        [{'a': 1}]
-
-    Set *base_type* to ``None`` to avoid any special handling and treat objects
-    Python considers iterable as iterable:
-
-        >>> obj = 'foo'
-        >>> list(always_iterable(obj, base_type=None))
-        ['f', 'o', 'o']
-    """
-    if obj is None:
-        return iter(())
-
-    if (base_type is not None) and isinstance(obj, base_type):
-        return iter((obj,))
-
-    try:
-        return iter(obj)
-    except TypeError:
-        return iter((obj,))
+from itertools import filterfalse
+
+
+def unique_everseen(iterable, key=None):
+    "List unique elements, preserving order. Remember all elements ever seen."
+    # unique_everseen('AAAABBBCCDAABBB') --> A B C D
+    # unique_everseen('ABBCcAD', str.lower) --> A B C D
+    seen = set()
+    seen_add = seen.add
+    if key is None:
+        for element in filterfalse(seen.__contains__, iterable):
+            seen_add(element)
+            yield element
+    else:
+        for element in iterable:
+            k = key(element)
+            if k not in seen:
+                seen_add(k)
+                yield element
+
+
+# copied from more_itertools 8.8
+def always_iterable(obj, base_type=(str, bytes)):
+    """If *obj* is iterable, return an iterator over its items::
+
+        >>> obj = (1, 2, 3)
+        >>> list(always_iterable(obj))
+        [1, 2, 3]
+
+    If *obj* is not iterable, return a one-item iterable containing *obj*::
+
+        >>> obj = 1
+        >>> list(always_iterable(obj))
+        [1]
+
+    If *obj* is ``None``, return an empty iterable:
+
+        >>> obj = None
+        >>> list(always_iterable(None))
+        []
+
+    By default, binary and text strings are not considered iterable::
+
+        >>> obj = 'foo'
+        >>> list(always_iterable(obj))
+        ['foo']
+
+    If *base_type* is set, objects for which ``isinstance(obj, base_type)``
+    returns ``True`` won't be considered iterable.
+
+        >>> obj = {'a': 1}
+        >>> list(always_iterable(obj))  # Iterate over the dict's keys
+        ['a']
+        >>> list(always_iterable(obj, base_type=dict))  # Treat dicts as a unit
+        [{'a': 1}]
+
+    Set *base_type* to ``None`` to avoid any special handling and treat objects
+    Python considers iterable as iterable:
+
+        >>> obj = 'foo'
+        >>> list(always_iterable(obj, base_type=None))
+        ['f', 'o', 'o']
+    """
+    if obj is None:
+        return iter(())
+
+    if (base_type is not None) and isinstance(obj, base_type):
+        return iter((obj,))
+
+    try:
+        return iter(obj)
+    except TypeError:
+        return iter((obj,))
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/_text.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/_text.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import re
-
-from ._functools import method_cache
-
-
-# from jaraco.text 3.5
-class FoldedCase(str):
-    """
-    A case insensitive string class; behaves just like str
-    except compares equal when the only variation is case.
-
-    >>> s = FoldedCase('hello world')
-
-    >>> s == 'Hello World'
-    True
-
-    >>> 'Hello World' == s
-    True
-
-    >>> s != 'Hello World'
-    False
-
-    >>> s.index('O')
-    4
-
-    >>> s.split('O')
-    ['hell', ' w', 'rld']
-
-    >>> sorted(map(FoldedCase, ['GAMMA', 'alpha', 'Beta']))
-    ['alpha', 'Beta', 'GAMMA']
-
-    Sequence membership is straightforward.
-
-    >>> "Hello World" in [s]
-    True
-    >>> s in ["Hello World"]
-    True
-
-    You may test for set inclusion, but candidate and elements
-    must both be folded.
-
-    >>> FoldedCase("Hello World") in {s}
-    True
-    >>> s in {FoldedCase("Hello World")}
-    True
-
-    String inclusion works as long as the FoldedCase object
-    is on the right.
-
-    >>> "hello" in FoldedCase("Hello World")
-    True
-
-    But not if the FoldedCase object is on the left:
-
-    >>> FoldedCase('hello') in 'Hello World'
-    False
-
-    In that case, use in_:
-
-    >>> FoldedCase('hello').in_('Hello World')
-    True
-
-    >>> FoldedCase('hello') > FoldedCase('Hello')
-    False
-    """
-
-    def __lt__(self, other):
-        return self.lower() < other.lower()
-
-    def __gt__(self, other):
-        return self.lower() > other.lower()
-
-    def __eq__(self, other):
-        return self.lower() == other.lower()
-
-    def __ne__(self, other):
-        return self.lower() != other.lower()
-
-    def __hash__(self):
-        return hash(self.lower())
-
-    def __contains__(self, other):
-        return super().lower().__contains__(other.lower())
-
-    def in_(self, other):
-        "Does self appear in other?"
-        return self in FoldedCase(other)
-
-    # cache lower since it's likely to be called frequently.
-    @method_cache
-    def lower(self):
-        return super().lower()
-
-    def index(self, sub):
-        return self.lower().index(sub.lower())
-
-    def split(self, splitter=' ', maxsplit=0):
-        pattern = re.compile(re.escape(splitter), re.I)
-        return pattern.split(self, maxsplit)
+import re
+
+from ._functools import method_cache
+
+
+# from jaraco.text 3.5
+class FoldedCase(str):
+    """
+    A case insensitive string class; behaves just like str
+    except compares equal when the only variation is case.
+
+    >>> s = FoldedCase('hello world')
+
+    >>> s == 'Hello World'
+    True
+
+    >>> 'Hello World' == s
+    True
+
+    >>> s != 'Hello World'
+    False
+
+    >>> s.index('O')
+    4
+
+    >>> s.split('O')
+    ['hell', ' w', 'rld']
+
+    >>> sorted(map(FoldedCase, ['GAMMA', 'alpha', 'Beta']))
+    ['alpha', 'Beta', 'GAMMA']
+
+    Sequence membership is straightforward.
+
+    >>> "Hello World" in [s]
+    True
+    >>> s in ["Hello World"]
+    True
+
+    You may test for set inclusion, but candidate and elements
+    must both be folded.
+
+    >>> FoldedCase("Hello World") in {s}
+    True
+    >>> s in {FoldedCase("Hello World")}
+    True
+
+    String inclusion works as long as the FoldedCase object
+    is on the right.
+
+    >>> "hello" in FoldedCase("Hello World")
+    True
+
+    But not if the FoldedCase object is on the left:
+
+    >>> FoldedCase('hello') in 'Hello World'
+    False
+
+    In that case, use in_:
+
+    >>> FoldedCase('hello').in_('Hello World')
+    True
+
+    >>> FoldedCase('hello') > FoldedCase('Hello')
+    False
+    """
+
+    def __lt__(self, other):
+        return self.lower() < other.lower()
+
+    def __gt__(self, other):
+        return self.lower() > other.lower()
+
+    def __eq__(self, other):
+        return self.lower() == other.lower()
+
+    def __ne__(self, other):
+        return self.lower() != other.lower()
+
+    def __hash__(self):
+        return hash(self.lower())
+
+    def __contains__(self, other):
+        return super().lower().__contains__(other.lower())
+
+    def in_(self, other):
+        "Does self appear in other?"
+        return self in FoldedCase(other)
+
+    # cache lower since it's likely to be called frequently.
+    @method_cache
+    def lower(self):
+        return super().lower()
+
+    def index(self, sub):
+        return self.lower().index(sub.lower())
+
+    def split(self, splitter=' ', maxsplit=0):
+        pattern = re.compile(re.escape(splitter), re.I)
+        return pattern.split(self, maxsplit)
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/importlib_metadata/LICENSE` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/importlib_metadata/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright 2017-2019 Jason R. Coombs, Barry Warsaw
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+Copyright 2017-2019 Jason R. Coombs, Barry Warsaw
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/zipp.LICENSE` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/zipp.LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright Jason R. Coombs
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+Copyright Jason R. Coombs
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `sitecustomize_entrypoints-1.0.0/src/sitecustomize/_vendor/zipp.py` & `sitecustomize-entrypoints-1.1.0/src/sitecustomize/_vendor/zipp.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,312 +1,312 @@
-import io
-import posixpath
-import zipfile
-import itertools
-import contextlib
-import pathlib
-
-
-__all__ = ['Path']
-
-
-def _parents(path):
-    """
-    Given a path with elements separated by
-    posixpath.sep, generate all parents of that path.
-
-    >>> list(_parents('b/d'))
-    ['b']
-    >>> list(_parents('/b/d/'))
-    ['/b']
-    >>> list(_parents('b/d/f/'))
-    ['b/d', 'b']
-    >>> list(_parents('b'))
-    []
-    >>> list(_parents(''))
-    []
-    """
-    return itertools.islice(_ancestry(path), 1, None)
-
-
-def _ancestry(path):
-    """
-    Given a path with elements separated by
-    posixpath.sep, generate all elements of that path
-
-    >>> list(_ancestry('b/d'))
-    ['b/d', 'b']
-    >>> list(_ancestry('/b/d/'))
-    ['/b/d', '/b']
-    >>> list(_ancestry('b/d/f/'))
-    ['b/d/f', 'b/d', 'b']
-    >>> list(_ancestry('b'))
-    ['b']
-    >>> list(_ancestry(''))
-    []
-    """
-    path = path.rstrip(posixpath.sep)
-    while path and path != posixpath.sep:
-        yield path
-        path, tail = posixpath.split(path)
-
-
-_dedupe = dict.fromkeys
-"""Deduplicate an iterable in original order"""
-
-
-def _difference(minuend, subtrahend):
-    """
-    Return items in minuend not in subtrahend, retaining order
-    with O(1) lookup.
-    """
-    return itertools.filterfalse(set(subtrahend).__contains__, minuend)
-
-
-class CompleteDirs(zipfile.ZipFile):
-    """
-    A ZipFile subclass that ensures that implied directories
-    are always included in the namelist.
-    """
-
-    @staticmethod
-    def _implied_dirs(names):
-        parents = itertools.chain.from_iterable(map(_parents, names))
-        as_dirs = (p + posixpath.sep for p in parents)
-        return _dedupe(_difference(as_dirs, names))
-
-    def namelist(self):
-        names = super(CompleteDirs, self).namelist()
-        return names + list(self._implied_dirs(names))
-
-    def _name_set(self):
-        return set(self.namelist())
-
-    def resolve_dir(self, name):
-        """
-        If the name represents a directory, return that name
-        as a directory (with the trailing slash).
-        """
-        names = self._name_set()
-        dirname = name + '/'
-        dir_match = name not in names and dirname in names
-        return dirname if dir_match else name
-
-    @classmethod
-    def make(cls, source):
-        """
-        Given a source (filename or zipfile), return an
-        appropriate CompleteDirs subclass.
-        """
-        if isinstance(source, CompleteDirs):
-            return source
-
-        if not isinstance(source, zipfile.ZipFile):
-            return cls(source)
-
-        # Only allow for FastLookup when supplied zipfile is read-only
-        if 'r' not in source.mode:
-            cls = CompleteDirs
-
-        source.__class__ = cls
-        return source
-
-
-class FastLookup(CompleteDirs):
-    """
-    ZipFile subclass to ensure implicit
-    dirs exist and are resolved rapidly.
-    """
-
-    def namelist(self):
-        with contextlib.suppress(AttributeError):
-            return self.__names
-        self.__names = super(FastLookup, self).namelist()
-        return self.__names
-
-    def _name_set(self):
-        with contextlib.suppress(AttributeError):
-            return self.__lookup
-        self.__lookup = super(FastLookup, self)._name_set()
-        return self.__lookup
-
-
-class Path:
-    """
-    A pathlib-compatible interface for zip files.
-
-    Consider a zip file with this structure::
-
-        .
-        ├── a.txt
-        └── b
-            ├── c.txt
-            └── d
-                └── e.txt
-
-    >>> data = io.BytesIO()
-    >>> zf = zipfile.ZipFile(data, 'w')
-    >>> zf.writestr('a.txt', 'content of a')
-    >>> zf.writestr('b/c.txt', 'content of c')
-    >>> zf.writestr('b/d/e.txt', 'content of e')
-    >>> zf.filename = 'mem/abcde.zip'
-
-    Path accepts the zipfile object itself or a filename
-
-    >>> root = Path(zf)
-
-    From there, several path operations are available.
-
-    Directory iteration (including the zip file itself):
-
-    >>> a, b = root.iterdir()
-    >>> a
-    Path('mem/abcde.zip', 'a.txt')
-    >>> b
-    Path('mem/abcde.zip', 'b/')
-
-    name property:
-
-    >>> b.name
-    'b'
-
-    join with divide operator:
-
-    >>> c = b / 'c.txt'
-    >>> c
-    Path('mem/abcde.zip', 'b/c.txt')
-    >>> c.name
-    'c.txt'
-
-    Read text:
-
-    >>> c.read_text()
-    'content of c'
-
-    existence:
-
-    >>> c.exists()
-    True
-    >>> (b / 'missing.txt').exists()
-    False
-
-    Coercion to string:
-
-    >>> import os
-    >>> str(c).replace(os.sep, posixpath.sep)
-    'mem/abcde.zip/b/c.txt'
-
-    At the root, ``name``, ``filename``, and ``parent``
-    resolve to the zipfile. Note these attributes are not
-    valid and will raise a ``ValueError`` if the zipfile
-    has no filename.
-
-    >>> root.name
-    'abcde.zip'
-    >>> str(root.filename).replace(os.sep, posixpath.sep)
-    'mem/abcde.zip'
-    >>> str(root.parent)
-    'mem'
-    """
-
-    __repr = "{self.__class__.__name__}({self.root.filename!r}, {self.at!r})"
-
-    def __init__(self, root, at=""):
-        """
-        Construct a Path from a ZipFile or filename.
-
-        Note: When the source is an existing ZipFile object,
-        its type (__class__) will be mutated to a
-        specialized type. If the caller wishes to retain the
-        original type, the caller should either create a
-        separate ZipFile object or pass a filename.
-        """
-        self.root = FastLookup.make(root)
-        self.at = at
-
-    def open(self, mode='r', *args, pwd=None, **kwargs):
-        """
-        Open this entry as text or binary following the semantics
-        of ``pathlib.Path.open()`` by passing arguments through
-        to io.TextIOWrapper().
-        """
-        if self.is_dir():
-            raise IsADirectoryError(self)
-        zip_mode = mode[0]
-        if not self.exists() and zip_mode == 'r':
-            raise FileNotFoundError(self)
-        stream = self.root.open(self.at, zip_mode, pwd=pwd)
-        if 'b' in mode:
-            if args or kwargs:
-                raise ValueError("encoding args invalid for binary operation")
-            return stream
-        return io.TextIOWrapper(stream, *args, **kwargs)
-
-    @property
-    def name(self):
-        return pathlib.Path(self.at).name or self.filename.name
-
-    @property
-    def suffix(self):
-        return pathlib.Path(self.at).suffix or self.filename.suffix
-
-    @property
-    def suffixes(self):
-        return pathlib.Path(self.at).suffixes or self.filename.suffixes
-
-    @property
-    def stem(self):
-        return pathlib.Path(self.at).stem or self.filename.stem
-
-    @property
-    def filename(self):
-        return pathlib.Path(self.root.filename).joinpath(self.at)
-
-    def read_text(self, *args, **kwargs):
-        with self.open('r', *args, **kwargs) as strm:
-            return strm.read()
-
-    def read_bytes(self):
-        with self.open('rb') as strm:
-            return strm.read()
-
-    def _is_child(self, path):
-        return posixpath.dirname(path.at.rstrip("/")) == self.at.rstrip("/")
-
-    def _next(self, at):
-        return self.__class__(self.root, at)
-
-    def is_dir(self):
-        return not self.at or self.at.endswith("/")
-
-    def is_file(self):
-        return self.exists() and not self.is_dir()
-
-    def exists(self):
-        return self.at in self.root._name_set()
-
-    def iterdir(self):
-        if not self.is_dir():
-            raise ValueError("Can't listdir a file")
-        subs = map(self._next, self.root.namelist())
-        return filter(self._is_child, subs)
-
-    def __str__(self):
-        return posixpath.join(self.root.filename, self.at)
-
-    def __repr__(self):
-        return self.__repr.format(self=self)
-
-    def joinpath(self, *other):
-        next = posixpath.join(self.at, *other)
-        return self._next(self.root.resolve_dir(next))
-
-    __truediv__ = joinpath
-
-    @property
-    def parent(self):
-        if not self.at:
-            return self.filename.parent
-        parent_at = posixpath.dirname(self.at.rstrip('/'))
-        if parent_at:
-            parent_at += '/'
-        return self._next(parent_at)
+import io
+import posixpath
+import zipfile
+import itertools
+import contextlib
+import pathlib
+
+
+__all__ = ['Path']
+
+
+def _parents(path):
+    """
+    Given a path with elements separated by
+    posixpath.sep, generate all parents of that path.
+
+    >>> list(_parents('b/d'))
+    ['b']
+    >>> list(_parents('/b/d/'))
+    ['/b']
+    >>> list(_parents('b/d/f/'))
+    ['b/d', 'b']
+    >>> list(_parents('b'))
+    []
+    >>> list(_parents(''))
+    []
+    """
+    return itertools.islice(_ancestry(path), 1, None)
+
+
+def _ancestry(path):
+    """
+    Given a path with elements separated by
+    posixpath.sep, generate all elements of that path
+
+    >>> list(_ancestry('b/d'))
+    ['b/d', 'b']
+    >>> list(_ancestry('/b/d/'))
+    ['/b/d', '/b']
+    >>> list(_ancestry('b/d/f/'))
+    ['b/d/f', 'b/d', 'b']
+    >>> list(_ancestry('b'))
+    ['b']
+    >>> list(_ancestry(''))
+    []
+    """
+    path = path.rstrip(posixpath.sep)
+    while path and path != posixpath.sep:
+        yield path
+        path, tail = posixpath.split(path)
+
+
+_dedupe = dict.fromkeys
+"""Deduplicate an iterable in original order"""
+
+
+def _difference(minuend, subtrahend):
+    """
+    Return items in minuend not in subtrahend, retaining order
+    with O(1) lookup.
+    """
+    return itertools.filterfalse(set(subtrahend).__contains__, minuend)
+
+
+class CompleteDirs(zipfile.ZipFile):
+    """
+    A ZipFile subclass that ensures that implied directories
+    are always included in the namelist.
+    """
+
+    @staticmethod
+    def _implied_dirs(names):
+        parents = itertools.chain.from_iterable(map(_parents, names))
+        as_dirs = (p + posixpath.sep for p in parents)
+        return _dedupe(_difference(as_dirs, names))
+
+    def namelist(self):
+        names = super(CompleteDirs, self).namelist()
+        return names + list(self._implied_dirs(names))
+
+    def _name_set(self):
+        return set(self.namelist())
+
+    def resolve_dir(self, name):
+        """
+        If the name represents a directory, return that name
+        as a directory (with the trailing slash).
+        """
+        names = self._name_set()
+        dirname = name + '/'
+        dir_match = name not in names and dirname in names
+        return dirname if dir_match else name
+
+    @classmethod
+    def make(cls, source):
+        """
+        Given a source (filename or zipfile), return an
+        appropriate CompleteDirs subclass.
+        """
+        if isinstance(source, CompleteDirs):
+            return source
+
+        if not isinstance(source, zipfile.ZipFile):
+            return cls(source)
+
+        # Only allow for FastLookup when supplied zipfile is read-only
+        if 'r' not in source.mode:
+            cls = CompleteDirs
+
+        source.__class__ = cls
+        return source
+
+
+class FastLookup(CompleteDirs):
+    """
+    ZipFile subclass to ensure implicit
+    dirs exist and are resolved rapidly.
+    """
+
+    def namelist(self):
+        with contextlib.suppress(AttributeError):
+            return self.__names
+        self.__names = super(FastLookup, self).namelist()
+        return self.__names
+
+    def _name_set(self):
+        with contextlib.suppress(AttributeError):
+            return self.__lookup
+        self.__lookup = super(FastLookup, self)._name_set()
+        return self.__lookup
+
+
+class Path:
+    """
+    A pathlib-compatible interface for zip files.
+
+    Consider a zip file with this structure::
+
+        .
+        ├── a.txt
+        └── b
+            ├── c.txt
+            └── d
+                └── e.txt
+
+    >>> data = io.BytesIO()
+    >>> zf = zipfile.ZipFile(data, 'w')
+    >>> zf.writestr('a.txt', 'content of a')
+    >>> zf.writestr('b/c.txt', 'content of c')
+    >>> zf.writestr('b/d/e.txt', 'content of e')
+    >>> zf.filename = 'mem/abcde.zip'
+
+    Path accepts the zipfile object itself or a filename
+
+    >>> root = Path(zf)
+
+    From there, several path operations are available.
+
+    Directory iteration (including the zip file itself):
+
+    >>> a, b = root.iterdir()
+    >>> a
+    Path('mem/abcde.zip', 'a.txt')
+    >>> b
+    Path('mem/abcde.zip', 'b/')
+
+    name property:
+
+    >>> b.name
+    'b'
+
+    join with divide operator:
+
+    >>> c = b / 'c.txt'
+    >>> c
+    Path('mem/abcde.zip', 'b/c.txt')
+    >>> c.name
+    'c.txt'
+
+    Read text:
+
+    >>> c.read_text()
+    'content of c'
+
+    existence:
+
+    >>> c.exists()
+    True
+    >>> (b / 'missing.txt').exists()
+    False
+
+    Coercion to string:
+
+    >>> import os
+    >>> str(c).replace(os.sep, posixpath.sep)
+    'mem/abcde.zip/b/c.txt'
+
+    At the root, ``name``, ``filename``, and ``parent``
+    resolve to the zipfile. Note these attributes are not
+    valid and will raise a ``ValueError`` if the zipfile
+    has no filename.
+
+    >>> root.name
+    'abcde.zip'
+    >>> str(root.filename).replace(os.sep, posixpath.sep)
+    'mem/abcde.zip'
+    >>> str(root.parent)
+    'mem'
+    """
+
+    __repr = "{self.__class__.__name__}({self.root.filename!r}, {self.at!r})"
+
+    def __init__(self, root, at=""):
+        """
+        Construct a Path from a ZipFile or filename.
+
+        Note: When the source is an existing ZipFile object,
+        its type (__class__) will be mutated to a
+        specialized type. If the caller wishes to retain the
+        original type, the caller should either create a
+        separate ZipFile object or pass a filename.
+        """
+        self.root = FastLookup.make(root)
+        self.at = at
+
+    def open(self, mode='r', *args, pwd=None, **kwargs):
+        """
+        Open this entry as text or binary following the semantics
+        of ``pathlib.Path.open()`` by passing arguments through
+        to io.TextIOWrapper().
+        """
+        if self.is_dir():
+            raise IsADirectoryError(self)
+        zip_mode = mode[0]
+        if not self.exists() and zip_mode == 'r':
+            raise FileNotFoundError(self)
+        stream = self.root.open(self.at, zip_mode, pwd=pwd)
+        if 'b' in mode:
+            if args or kwargs:
+                raise ValueError("encoding args invalid for binary operation")
+            return stream
+        return io.TextIOWrapper(stream, *args, **kwargs)
+
+    @property
+    def name(self):
+        return pathlib.Path(self.at).name or self.filename.name
+
+    @property
+    def suffix(self):
+        return pathlib.Path(self.at).suffix or self.filename.suffix
+
+    @property
+    def suffixes(self):
+        return pathlib.Path(self.at).suffixes or self.filename.suffixes
+
+    @property
+    def stem(self):
+        return pathlib.Path(self.at).stem or self.filename.stem
+
+    @property
+    def filename(self):
+        return pathlib.Path(self.root.filename).joinpath(self.at)
+
+    def read_text(self, *args, **kwargs):
+        with self.open('r', *args, **kwargs) as strm:
+            return strm.read()
+
+    def read_bytes(self):
+        with self.open('rb') as strm:
+            return strm.read()
+
+    def _is_child(self, path):
+        return posixpath.dirname(path.at.rstrip("/")) == self.at.rstrip("/")
+
+    def _next(self, at):
+        return self.__class__(self.root, at)
+
+    def is_dir(self):
+        return not self.at or self.at.endswith("/")
+
+    def is_file(self):
+        return self.exists() and not self.is_dir()
+
+    def exists(self):
+        return self.at in self.root._name_set()
+
+    def iterdir(self):
+        if not self.is_dir():
+            raise ValueError("Can't listdir a file")
+        subs = map(self._next, self.root.namelist())
+        return filter(self._is_child, subs)
+
+    def __str__(self):
+        return posixpath.join(self.root.filename, self.at)
+
+    def __repr__(self):
+        return self.__repr.format(self=self)
+
+    def joinpath(self, *other):
+        next = posixpath.join(self.at, *other)
+        return self._next(self.root.resolve_dir(next))
+
+    __truediv__ = joinpath
+
+    @property
+    def parent(self):
+        if not self.at:
+            return self.filename.parent
+        parent_at = posixpath.dirname(self.at.rstrip('/'))
+        if parent_at:
+            parent_at += '/'
+        return self._next(parent_at)
```

