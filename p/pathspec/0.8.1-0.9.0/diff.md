# Comparing `tmp/pathspec-0.8.1.tar.gz` & `tmp/pathspec-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pathspec-0.8.1.tar", last modified: Sat Nov  7 19:37:55 2020, max compression
+gzip compressed data, was "dist/pathspec-0.9.0.tar", last modified: Sun Jul 18 00:27:56 2021, max compression
```

## Comparing `pathspec-0.8.1.tar` & `pathspec-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2020-11-07 19:37:55.000000 pathspec-0.8.1/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     5692 2020-11-07 19:31:55.000000 pathspec-0.8.1/CHANGES.rst
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2020-11-07 19:37:55.000000 pathspec-0.8.1/pathspec/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     4405 2020-02-03 03:22:42.000000 pathspec-0.8.1/pathspec/pattern.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     7027 2020-11-07 19:27:35.000000 pathspec-0.8.1/pathspec/pathspec.py
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2020-11-07 19:37:55.000000 pathspec-0.8.1/pathspec/tests/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2020-02-03 03:22:42.000000 pathspec-0.8.1/pathspec/tests/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    12786 2020-02-03 03:22:42.000000 pathspec-0.8.1/pathspec/tests/test_gitwildmatch.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     7906 2020-04-07 02:21:51.000000 pathspec-0.8.1/pathspec/tests/test_util.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     3975 2020-11-07 19:27:35.000000 pathspec-0.8.1/pathspec/tests/test_pathspec.py
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2020-11-07 19:37:55.000000 pathspec-0.8.1/pathspec/patterns/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      184 2020-02-03 03:22:42.000000 pathspec-0.8.1/pathspec/patterns/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     9947 2020-02-03 03:22:42.000000 pathspec-0.8.1/pathspec/patterns/gitwildmatch.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     2213 2020-11-07 19:35:24.000000 pathspec-0.8.1/pathspec/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    17929 2020-04-07 03:43:06.000000 pathspec-0.8.1/pathspec/util.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      777 2020-04-07 03:10:57.000000 pathspec-0.8.1/pathspec/compat.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       30 2020-01-29 02:45:39.000000 pathspec-0.8.1/MANIFEST.in
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       67 2020-11-07 19:37:55.000000 pathspec-0.8.1/setup.cfg
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2020-11-07 19:37:55.000000 pathspec-0.8.1/pathspec.egg-info/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    14258 2020-11-07 19:37:54.000000 pathspec-0.8.1/pathspec.egg-info/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2020-11-07 19:37:54.000000 pathspec-0.8.1/pathspec.egg-info/dependency_links.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      474 2020-11-07 19:37:54.000000 pathspec-0.8.1/pathspec.egg-info/SOURCES.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        9 2020-11-07 19:37:54.000000 pathspec-0.8.1/pathspec.egg-info/top_level.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     4463 2020-01-29 02:45:39.000000 pathspec-0.8.1/README.rst
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    14258 2020-11-07 19:37:55.000000 pathspec-0.8.1/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    16726 2020-01-29 02:44:58.000000 pathspec-0.8.1/LICENSE
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     1559 2020-01-29 02:45:39.000000 pathspec-0.8.1/setup.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2021-07-18 00:27:56.000000 pathspec-0.9.0/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     6397 2021-07-18 00:13:17.000000 pathspec-0.9.0/CHANGES.rst
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4811 2021-06-12 17:34:35.000000 pathspec-0.9.0/pathspec/pattern.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     8048 2021-06-12 18:06:53.000000 pathspec-0.9.0/pathspec/pathspec.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec/tests/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2020-02-03 03:22:42.000000 pathspec-0.9.0/pathspec/tests/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    15160 2021-07-18 00:15:39.000000 pathspec-0.9.0/pathspec/tests/test_gitwildmatch.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     7906 2020-04-07 02:21:51.000000 pathspec-0.9.0/pathspec/tests/test_util.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4845 2021-06-12 16:27:25.000000 pathspec-0.9.0/pathspec/tests/test_pathspec.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec/patterns/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      184 2020-02-03 03:22:42.000000 pathspec-0.9.0/pathspec/patterns/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    11899 2021-07-18 00:05:09.000000 pathspec-0.9.0/pathspec/patterns/gitwildmatch.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1085 2021-06-03 03:48:54.000000 pathspec-0.9.0/pathspec/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1617 2021-07-18 00:13:02.000000 pathspec-0.9.0/pathspec/_meta.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    19889 2021-06-12 17:28:58.000000 pathspec-0.9.0/pathspec/util.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      830 2021-06-12 16:47:43.000000 pathspec-0.9.0/pathspec/compat.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1617 2021-07-18 00:13:02.000000 pathspec-0.9.0/pathspec_meta.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       43 2021-06-03 03:48:54.000000 pathspec-0.9.0/MANIFEST.in
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1329 2021-07-18 00:27:56.000000 pathspec-0.9.0/setup.cfg
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec.egg-info/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    15192 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec.egg-info/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec.egg-info/dependency_links.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      528 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec.egg-info/SOURCES.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        9 2021-07-18 00:27:56.000000 pathspec-0.9.0/pathspec.egg-info/top_level.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4463 2020-01-29 02:45:39.000000 pathspec-0.9.0/README.rst
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    15192 2021-07-18 00:27:56.000000 pathspec-0.9.0/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1137 2021-06-03 03:48:54.000000 pathspec-0.9.0/tox_pip_install.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    16726 2020-01-29 02:44:58.000000 pathspec-0.9.0/LICENSE
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       57 2021-06-03 03:48:54.000000 pathspec-0.9.0/setup.py
```

### Comparing `pathspec-0.8.1/CHANGES.rst` & `pathspec-0.9.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 
 Change History
 ==============
 
+0.9.0 (2021-07-17)
+------------------
+
+- `Issue #44`_/`Issue #50`_: Raise `GitWildMatchPatternError` for invalid git patterns.
+- `Issue #45`_: Fix for duplicate leading double-asterisk, and edge cases.
+- `Issue #46`_: Fix matching absolute paths.
+- API change: `util.normalize_files()` now returns a `Dict[str, List[pathlike]]` instead of a `Dict[str, pathlike]`.
+- Added type hinting.
+
+.. _`Issue #44`: https://github.com/cpburnz/python-path-specification/issues/44
+.. _`Issue #45`: https://github.com/cpburnz/python-path-specification/pull/45
+.. _`Issue #46`: https://github.com/cpburnz/python-path-specification/issues/46
+.. _`Issue #50`: https://github.com/cpburnz/python-path-specification/pull/50
+
+
 0.8.1 (2020-11-07)
 ------------------
 
 - `Issue #43`_: Add support for addition operator.
 
 .. _`Issue #43`: https://github.com/cpburnz/python-path-specification/pull/43
```

### Comparing `pathspec-0.8.1/pathspec/pattern.py` & `pathspec-0.9.0/pathspec/pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # encoding: utf-8
 """
 This module provides the base definition for patterns.
 """
 
 import re
+try:
+	from typing import (
+		AnyStr,
+		Iterable,
+		Iterator,
+		Optional,
+		Pattern as RegexHint,
+		Text,
+		Tuple,
+		Union)
+except ImportError:
+	pass
 
 from .compat import unicode
 
 
 class Pattern(object):
 	"""
 	The :class:`Pattern` class is the abstract definition of a pattern.
 	"""
 
 	# Make the class dict-less.
 	__slots__ = ('include',)
 
 	def __init__(self, include):
+		# type: (Optional[bool]) -> None
 		"""
 		Initializes the :class:`Pattern` instance.
 
 		*include* (:class:`bool` or :data:`None`) is whether the matched
 		files should be included (:data:`True`), excluded (:data:`False`),
 		or is a null-operation (:data:`None`).
 		"""
@@ -29,14 +42,15 @@
 		"""
 		*include* (:class:`bool` or :data:`None`) is whether the matched
 		files should be included (:data:`True`), excluded (:data:`False`),
 		or is a null-operation (:data:`None`).
 		"""
 
 	def match(self, files):
+		# type: (Iterable[Text]) -> Iterator[Text]
 		"""
 		Matches this pattern against the specified files.
 
 		*files* (:class:`~collections.abc.Iterable` of :class:`str`) contains
 		each file relative to the root directory (e.g., ``"relative/path/to/file"``).
 
 		Returns an :class:`~collections.abc.Iterable` yielding each matched
@@ -51,14 +65,15 @@
 	using regular expressions.
 	"""
 
 	# Make the class dict-less.
 	__slots__ = ('regex',)
 
 	def __init__(self, pattern, include=None):
+		# type: (Union[AnyStr, RegexHint], Optional[bool]) -> None
 		"""
 		Initializes the :class:`RegexPattern` instance.
 
 		*pattern* (:class:`unicode`, :class:`bytes`, :class:`re.RegexObject`,
 		or :data:`None`) is the pattern to compile into a regular
 		expression.
 
@@ -99,25 +114,27 @@
 		else:
 			raise TypeError("pattern:{!r} is not a string, RegexObject, or None.".format(pattern))
 
 		super(RegexPattern, self).__init__(include)
 		self.regex = regex
 
 	def __eq__(self, other):
+		# type: (RegexPattern) -> bool
 		"""
 		Tests the equality of this regex pattern with *other* (:class:`RegexPattern`)
 		by comparing their :attr:`~Pattern.include` and :attr:`~RegexPattern.regex`
 		attributes.
 		"""
 		if isinstance(other, RegexPattern):
 			return self.include == other.include and self.regex == other.regex
 		else:
 			return NotImplemented
 
 	def match(self, files):
+		# type: (Iterable[Text]) -> Iterable[Text]
 		"""
 		Matches this pattern against the specified files.
 
 		*files* (:class:`~collections.abc.Iterable` of :class:`str`)
 		contains each file relative to the root directory (e.g., "relative/path/to/file").
 
 		Returns an :class:`~collections.abc.Iterable` yielding each matched
@@ -126,14 +143,15 @@
 		if self.include is not None:
 			for path in files:
 				if self.regex.match(path) is not None:
 					yield path
 
 	@classmethod
 	def pattern_to_regex(cls, pattern):
+		# type: (Text) -> Tuple[Text, bool]
 		"""
 		Convert the pattern into an uncompiled regular expression.
 
 		*pattern* (:class:`str`) is the pattern to convert into a regular
 		expression.
 
 		Returns the uncompiled regular expression (:class:`str` or :data:`None`),
```

### Comparing `pathspec-0.8.1/pathspec/pathspec.py` & `pathspec-0.9.0/pathspec/pathspec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,66 @@
 # encoding: utf-8
 """
 This module provides an object oriented interface for pattern matching
 of files.
 """
 
+try:
+	from typing import (
+		Any,
+		AnyStr,
+		Callable,
+		Iterable,
+		Iterator,
+		Optional,
+		Text,
+		Union)
+except ImportError:
+	pass
+
+try:
+	# Python 3.6+ type hints.
+	from os import PathLike
+	from typing import Collection
+except ImportError:
+	pass
+
 from . import util
-from .compat import Collection, iterkeys, izip_longest, string_types, unicode
+from .compat import (
+	CollectionType,
+	iterkeys,
+	izip_longest,
+	string_types)
+from .pattern import Pattern
+from .util import TreeEntry
 
 
 class PathSpec(object):
 	"""
 	The :class:`PathSpec` class is a wrapper around a list of compiled
 	:class:`.Pattern` instances.
 	"""
 
 	def __init__(self, patterns):
+		# type: (Iterable[Pattern]) -> None
 		"""
 		Initializes the :class:`PathSpec` instance.
 
 		*patterns* (:class:`~collections.abc.Collection` or :class:`~collections.abc.Iterable`)
 		yields each compiled pattern (:class:`.Pattern`).
 		"""
 
-		self.patterns = patterns if isinstance(patterns, Collection) else list(patterns)
+		self.patterns = patterns if isinstance(patterns, CollectionType) else list(patterns)
 		"""
 		*patterns* (:class:`~collections.abc.Collection` of :class:`.Pattern`)
 		contains the compiled patterns.
 		"""
 
 	def __eq__(self, other):
+		# type: (PathSpec) -> bool
 		"""
 		Tests the equality of this path-spec with *other* (:class:`PathSpec`)
 		by comparing their :attr:`~PathSpec.patterns` attributes.
 		"""
 		if isinstance(other, PathSpec):
 			paired_patterns = izip_longest(self.patterns, other.patterns)
 			return all(a == b for a, b in paired_patterns)
@@ -43,36 +71,39 @@
 		"""
 		Returns the number of compiled patterns this path-spec contains
 		(:class:`int`).
 		"""
 		return len(self.patterns)
 
 	def __add__(self, other):
+		# type: (PathSpec) -> PathSpec
 		"""
 		Combines the :attr:`Pathspec.patterns` patterns from two
 		:class:`PathSpec` instances.
 		"""
 		if isinstance(other, PathSpec):
 			return PathSpec(self.patterns + other.patterns)
 		else:
 			return NotImplemented
 
 	def __iadd__(self, other):
+		# type: (PathSpec) -> PathSpec
 		"""
 		Adds the :attr:`Pathspec.patterns` patterns from one :class:`PathSpec`
 		instance to this instance.
 		"""
 		if isinstance(other, PathSpec):
 			self.patterns += other.patterns
 			return self
 		else:
 			return NotImplemented
 
 	@classmethod
 	def from_lines(cls, pattern_factory, lines):
+		# type: (Union[Text, Callable[[AnyStr], Pattern]], Iterable[AnyStr]) -> PathSpec
 		"""
 		Compiles the pattern lines.
 
 		*pattern_factory* can be either the name of a registered pattern
 		factory (:class:`str`), or a :class:`~collections.abc.Callable` used
 		to compile patterns. It must accept an uncompiled pattern (:class:`str`)
 		and return the compiled pattern (:class:`.Pattern`).
@@ -88,18 +119,19 @@
 			pattern_factory = util.lookup_pattern(pattern_factory)
 		if not callable(pattern_factory):
 			raise TypeError("pattern_factory:{!r} is not callable.".format(pattern_factory))
 
 		if not util._is_iterable(lines):
 			raise TypeError("lines:{!r} is not an iterable.".format(lines))
 
-		lines = [pattern_factory(line) for line in lines if line]
-		return cls(lines)
+		patterns = [pattern_factory(line) for line in lines if line]
+		return cls(patterns)
 
 	def match_file(self, file, separators=None):
+		# type: (Union[Text, PathLike], Optional[Collection[Text]]) -> bool
 		"""
 		Matches the file to this path-spec.
 
 		*file* (:class:`str` or :class:`~pathlib.PurePath`) is the file path
 		to be matched against :attr:`self.patterns <PathSpec.patterns>`.
 
 		*separators* (:class:`~collections.abc.Collection` of :class:`str`)
@@ -108,61 +140,65 @@
 
 		Returns :data:`True` if *file* matched; otherwise, :data:`False`.
 		"""
 		norm_file = util.normalize_file(file, separators=separators)
 		return util.match_file(self.patterns, norm_file)
 
 	def match_entries(self, entries, separators=None):
+		# type: (Iterable[TreeEntry], Optional[Collection[Text]]) -> Iterator[TreeEntry]
 		"""
 		Matches the entries to this path-spec.
 
 		*entries* (:class:`~collections.abc.Iterable` of :class:`~util.TreeEntry`)
 		contains the entries to be matched against :attr:`self.patterns <PathSpec.patterns>`.
 
 		*separators* (:class:`~collections.abc.Collection` of :class:`str`;
 		or :data:`None`) optionally contains the path separators to
 		normalize. See :func:`~pathspec.util.normalize_file` for more
 		information.
 
-		Returns the matched entries (:class:`~collections.abc.Iterable` of
+		Returns the matched entries (:class:`~collections.abc.Iterator` of
 		:class:`~util.TreeEntry`).
 		"""
 		if not util._is_iterable(entries):
 			raise TypeError("entries:{!r} is not an iterable.".format(entries))
 
 		entry_map = util._normalize_entries(entries, separators=separators)
 		match_paths = util.match_files(self.patterns, iterkeys(entry_map))
 		for path in match_paths:
 			yield entry_map[path]
 
 	def match_files(self, files, separators=None):
+		# type: (Iterable[Union[Text, PathLike]], Optional[Collection[Text]]) -> Iterator[Union[Text, PathLike]]
 		"""
 		Matches the files to this path-spec.
 
 		*files* (:class:`~collections.abc.Iterable` of :class:`str; or
 		:class:`pathlib.PurePath`) contains the file paths to be matched
 		against :attr:`self.patterns <PathSpec.patterns>`.
 
 		*separators* (:class:`~collections.abc.Collection` of :class:`str`;
 		or :data:`None`) optionally contains the path separators to
 		normalize. See :func:`~pathspec.util.normalize_file` for more
 		information.
 
-		Returns the matched files (:class:`~collections.abc.Iterable` of
-		:class:`str`).
+		Returns the matched files (:class:`~collections.abc.Iterator` of
+		:class:`str` or :class:`pathlib.PurePath`).
 		"""
 		if not util._is_iterable(files):
 			raise TypeError("files:{!r} is not an iterable.".format(files))
 
 		file_map = util.normalize_files(files, separators=separators)
 		matched_files = util.match_files(self.patterns, iterkeys(file_map))
-		for path in matched_files:
-			yield file_map[path]
+		for norm_file in matched_files:
+			for orig_file in file_map[norm_file]:
+				yield orig_file
 
 	def match_tree_entries(self, root, on_error=None, follow_links=None):
+		# type: (Text, Optional[Callable], Optional[bool]) -> Iterator[TreeEntry]
 		"""
 		Walks the specified root path for all files and matches them to this
 		path-spec.
 
 		*root* (:class:`str`; or :class:`pathlib.PurePath`) is the root
 		directory to search.
 
@@ -170,21 +206,22 @@
 		optionally is the error handler for file-system exceptions. See
 		:func:`~pathspec.util.iter_tree_entries` for more information.
 
 		*follow_links* (:class:`bool` or :data:`None`) optionally is whether
 		to walk symbolic links that resolve to directories. See
 		:func:`~pathspec.util.iter_tree_files` for more information.
 
-		Returns the matched files (:class:`~collections.abc.Iterable` of
-		:class:`str`).
+		Returns the matched files (:class:`~collections.abc.Iterator` of
+		:class:`.TreeEntry`).
 		"""
 		entries = util.iter_tree_entries(root, on_error=on_error, follow_links=follow_links)
 		return self.match_entries(entries)
 
 	def match_tree_files(self, root, on_error=None, follow_links=None):
+		# type: (Text, Optional[Callable], Optional[bool]) -> Iterator[Text]
 		"""
 		Walks the specified root path for all files and matches them to this
 		path-spec.
 
 		*root* (:class:`str`; or :class:`pathlib.PurePath`) is the root
 		directory to search for files.
```

### Comparing `pathspec-0.8.1/pathspec/tests/test_gitwildmatch.py` & `pathspec-0.9.0/pathspec/tests/test_gitwildmatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import re
 import sys
 import unittest
 
 import pathspec.patterns.gitwildmatch
 import pathspec.util
-from pathspec.patterns.gitwildmatch import GitWildMatchPattern
+from pathspec.patterns.gitwildmatch import GitWildMatchPattern, GitWildMatchPatternError
 
 if sys.version_info[0] >= 3:
 	unichr = chr
 
 
 class GitWildMatchTest(unittest.TestCase):
 	"""
@@ -180,34 +180,37 @@
 
 	def test_03_inner_double_asterisk(self):
 		"""
 		Tests a path with an inner double-asterisk directory.
 
 		This should match:
 
+			left/right
 			left/bar/right
 			left/foo/bar/right
 			left/bar/right/foo
 
 		This should **not** match (according to git check-ignore (v2.4.1)):
 
 			foo/left/bar/right
 		"""
 		regex, include = GitWildMatchPattern.pattern_to_regex('left/**/right')
 		self.assertTrue(include)
 		self.assertEqual(regex, '^left(?:/.+)?/right(?:/.*)?$')
 
 		pattern = GitWildMatchPattern(re.compile(regex), include)
 		results = set(pattern.match([
+			'left/right',
 			'left/bar/right',
 			'left/foo/bar/right',
 			'left/bar/right/foo',
 			'foo/left/bar/right',
 		]))
 		self.assertEqual(results, {
+			'left/right',
 			'left/bar/right',
 			'left/foo/bar/right',
 			'left/bar/right/foo',
 		})
 
 	def test_03_only_double_asterisk(self):
 		"""
@@ -219,31 +222,84 @@
 
 	def test_03_parent_double_asterisk(self):
 		"""
 		Tests a file name with a double-asterisk parent directory.
 
 		This should match:
 
+			spam
 			foo/spam
 			foo/spam/bar
 		"""
 		regex, include = GitWildMatchPattern.pattern_to_regex('**/spam')
 		self.assertTrue(include)
 		self.assertEqual(regex, '^(?:.+/)?spam(?:/.*)?$')
 
 		pattern = GitWildMatchPattern(re.compile(regex), include)
 		results = set(pattern.match([
+			'spam',
 			'foo/spam',
 			'foo/spam/bar',
 		]))
 		self.assertEqual(results, {
+			'spam',
 			'foo/spam',
 			'foo/spam/bar',
 		})
 
+	def test_03_duplicate_leading_double_asterisk_edge_case(self):
+		"""
+		Regression test for duplicate leading **/ bug.
+		"""
+		regex, include = GitWildMatchPattern.pattern_to_regex('**')
+		self.assertTrue(include)
+		self.assertEqual(regex, '^.+$')
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/**')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/**/**')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
+		regex, include = GitWildMatchPattern.pattern_to_regex('**/api')
+		self.assertTrue(include)
+		self.assertEqual(regex, '^(?:.+/)?api(?:/.*)?$')
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/**/api')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
+		regex, include = GitWildMatchPattern.pattern_to_regex('**/api/')
+		self.assertTrue(include)
+		self.assertEqual(regex, '^(?:.+/)?api/.*$')
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/api/**')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/**/api/**/**')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
+	def test_03_double_asterisk_trailing_slash_edge_case(self):
+		"""
+		Tests the edge-case **/ pattern.
+
+		This should match everything except individual files in the root directory.
+		"""
+		regex, include = GitWildMatchPattern.pattern_to_regex('**/')
+		self.assertTrue(include)
+		self.assertEqual(regex, '^.+/.*$')
+
+		equivalent_regex, include = GitWildMatchPattern.pattern_to_regex('**/**/')
+		self.assertTrue(include)
+		self.assertEqual(equivalent_regex, regex)
+
 	def test_04_infix_wildcard(self):
 		"""
 		Tests a pattern with an infix wildcard.
 
 		This should match:
 
 			foo--bar
@@ -468,7 +524,25 @@
 		"""
 		Test escaping a string with meta-characters
 		"""
 		fname = "file!with*weird#naming_[1].t?t"
 		escaped = r"file\!with\*weird\#naming_\[1\].t\?t"
 		result = GitWildMatchPattern.escape(fname)
 		self.assertEqual(result, escaped)
+
+	def test_09_single_escape_fail(self):
+		"""
+		Test an escape on a line by itself.
+		"""
+		self._check_invalid_pattern("\\")
+
+	def test_09_single_exclamation_mark_fail(self):
+		"""
+		Test an escape on a line by itself.
+		"""
+		self._check_invalid_pattern("!")
+
+	def _check_invalid_pattern(self, git_ignore_pattern):
+		expected_message_pattern = re.escape(repr(git_ignore_pattern))
+		with self.assertRaisesRegexp(GitWildMatchPatternError, expected_message_pattern):
+			GitWildMatchPattern(git_ignore_pattern)
+
```

### Comparing `pathspec-0.8.1/pathspec/tests/test_util.py` & `pathspec-0.9.0/pathspec/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pathspec-0.8.1/pathspec/tests/test_pathspec.py` & `pathspec-0.9.0/pathspec/tests/test_pathspec.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,60 @@
 
 
 class PathSpecTest(unittest.TestCase):
 	"""
 	The ``PathSpecTest`` class tests the ``PathSpec`` class.
 	"""
 
+	def test_01_absolute_dir_paths_1(self):
+		"""
+		Tests that absolute paths will be properly normalized and matched.
+		"""
+		spec = pathspec.PathSpec.from_lines('gitwildmatch', [
+			'foo',
+		])
+		results = set(spec.match_files([
+			'/a.py',
+			'/foo/a.py',
+			'/x/a.py',
+			'/x/foo/a.py',
+			'a.py',
+			'foo/a.py',
+			'x/a.py',
+			'x/foo/a.py',
+		]))
+		self.assertEqual(results, {
+			'/foo/a.py',
+			'/x/foo/a.py',
+			'foo/a.py',
+			'x/foo/a.py',
+		})
+
+	def test_01_absolute_dir_paths_2(self):
+		"""
+		Tests that absolute paths will be properly normalized and matched.
+		"""
+		spec = pathspec.PathSpec.from_lines('gitwildmatch', [
+			'/foo',
+		])
+		results = set(spec.match_files([
+			'/a.py',
+			'/foo/a.py',
+			'/x/a.py',
+			'/x/foo/a.py',
+			'a.py',
+			'foo/a.py',
+			'x/a.py',
+			'x/foo/a.py',
+		]))
+		self.assertEqual(results, {
+			'/foo/a.py',
+			'foo/a.py',
+		})
+
 	def test_01_current_dir_paths(self):
 		"""
 		Tests that paths referencing the current directory will be properly
 		normalized and matched.
 		"""
 		spec = pathspec.PathSpec.from_lines('gitwildmatch', [
 			'*.txt',
```

### Comparing `pathspec-0.8.1/pathspec/patterns/gitwildmatch.py` & `pathspec-0.9.0/pathspec/patterns/gitwildmatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,51 @@
 derived from Rsync's wildmatch. Git uses wildmatch for its ".gitignore"
 files.
 """
 from __future__ import unicode_literals
 
 import re
 import warnings
+try:
+	from typing import (
+		AnyStr,
+		Optional,
+		Text,
+		Tuple)
+except ImportError:
+	pass
 
 from .. import util
 from ..compat import unicode
 from ..pattern import RegexPattern
 
 #: The encoding to use when parsing a byte string pattern.
 _BYTES_ENCODING = 'latin1'
 
 
+class GitWildMatchPatternError(ValueError):
+	"""
+	The :class:`GitWildMatchPatternError` indicates an invalid git wild match
+	pattern.
+	"""
+	pass
+
+
 class GitWildMatchPattern(RegexPattern):
 	"""
 	The :class:`GitWildMatchPattern` class represents a compiled Git
 	wildmatch pattern.
 	"""
 
 	# Keep the dict-less class hierarchy.
 	__slots__ = ()
 
 	@classmethod
 	def pattern_to_regex(cls, pattern):
+		# type: (AnyStr) -> Tuple[Optional[AnyStr], Optional[bool]]
 		"""
 		Convert the pattern into a regular expression.
 
 		*pattern* (:class:`unicode` or :class:`bytes`) is the pattern to
 		convert into a regular expression.
 
 		Returns the uncompiled regular expression (:class:`unicode`, :class:`bytes`,
@@ -43,14 +60,15 @@
 			return_type = unicode
 		elif isinstance(pattern, bytes):
 			return_type = bytes
 			pattern = pattern.decode(_BYTES_ENCODING)
 		else:
 			raise TypeError("pattern:{!r} is not a unicode or byte string.".format(pattern))
 
+		original_pattern = pattern
 		pattern = pattern.strip()
 
 		if pattern.startswith('#'):
 			# A pattern starting with a hash ('#') serves as a comment
 			# (neither includes nor excludes files). Escape the hash with a
 			# back-slash to match a literal hash (i.e., '\#').
 			regex = None
@@ -59,15 +77,14 @@
 		elif pattern == '/':
 			# EDGE CASE: According to `git check-ignore` (v2.4.1), a single
 			# '/' does not match any file.
 			regex = None
 			include = None
 
 		elif pattern:
-
 			if pattern.startswith('!'):
 				# A pattern starting with an exclamation mark ('!') negates the
 				# pattern (exclude instead of include). Escape the exclamation
 				# mark with a back-slash to match a literal exclamation mark
 				# (i.e., '\!').
 				include = False
 				# Remove leading exclamation mark.
@@ -76,19 +93,39 @@
 				include = True
 
 			if pattern.startswith('\\'):
 				# Remove leading back-slash escape for escaped hash ('#') or
 				# exclamation mark ('!').
 				pattern = pattern[1:]
 
+			# Allow a regex override for edge cases that cannot be handled
+			# through normalization.
+			override_regex = None
+
 			# Split pattern into segments.
 			pattern_segs = pattern.split('/')
 
 			# Normalize pattern to make processing easier.
 
+			# EDGE CASE: Deal with duplicate double-asterisk sequences.
+			# Collapse each sequence down to one double-asterisk. Iterate over
+			# the segments in reverse and remove the duplicate double
+			# asterisks as we go.
+			for i in range(len(pattern_segs) - 1, 0, -1):
+				prev = pattern_segs[i-1]
+				seg = pattern_segs[i]
+				if prev == '**' and seg == '**':
+					del pattern_segs[i]
+
+			if len(pattern_segs) == 2 and pattern_segs[0] == '**' and not pattern_segs[1]:
+				# EDGE CASE: The '**/' pattern should match everything except
+				# individual files in the root directory. This case cannot be
+				# adequately handled through normalization. Use the override.
+				override_regex = '^.+/.*$'
+
 			if not pattern_segs[0]:
 				# A pattern beginning with a slash ('/') will only match paths
 				# directly on the root directory instead of any descendant
 				# paths. So, remove empty first segment to make pattern relative
 				# to root.
 				del pattern_segs[0]
 
@@ -105,80 +142,98 @@
 			else:
 				# EDGE CASE: A pattern without a beginning slash ('/') but
 				# contains at least one prepended directory (e.g.
 				# "dir/{pattern}") should not match "**/dir/{pattern}",
 				# according to `git check-ignore` (v2.4.1).
 				pass
 
+			if not pattern_segs:
+				# After resolving the edge cases, we end up with no
+				# pattern at all. This must be because the pattern is
+				# invalid.
+				raise GitWildMatchPatternError("Invalid git pattern: %r" % (original_pattern,))
+
 			if not pattern_segs[-1] and len(pattern_segs) > 1:
-				# A pattern ending with a slash ('/') will match all descendant
-				# paths if it is a directory but not if it is a regular file.
-				# This is equivilent to "{pattern}/**". So, set last segment to
-				# double asterisks to include all descendants.
+				# A pattern ending with a slash ('/') will match all
+				# descendant paths if it is a directory but not if it is a
+				# regular file. This is equivalent to "{pattern}/**". So, set
+				# last segment to a double-asterisk to include all
+				# descendants.
 				pattern_segs[-1] = '**'
 
-			# Build regular expression from pattern.
-			output = ['^']
-			need_slash = False
-			end = len(pattern_segs) - 1
-			for i, seg in enumerate(pattern_segs):
-				if seg == '**':
-					if i == 0 and i == end:
-						# A pattern consisting solely of double-asterisks ('**')
-						# will match every path.
-						output.append('.+')
-					elif i == 0:
-						# A normalized pattern beginning with double-asterisks
-						# ('**') will match any leading path segments.
-						output.append('(?:.+/)?')
-						need_slash = False
-					elif i == end:
-						# A normalized pattern ending with double-asterisks ('**')
-						# will match any trailing path segments.
-						output.append('/.*')
+			if override_regex is None:
+				# Build regular expression from pattern.
+				output = ['^']
+				need_slash = False
+				end = len(pattern_segs) - 1
+				for i, seg in enumerate(pattern_segs):
+					if seg == '**':
+						if i == 0 and i == end:
+							# A pattern consisting solely of double-asterisks ('**')
+							# will match every path.
+							output.append('.+')
+						elif i == 0:
+							# A normalized pattern beginning with double-asterisks
+							# ('**') will match any leading path segments.
+							output.append('(?:.+/)?')
+							need_slash = False
+						elif i == end:
+							# A normalized pattern ending with double-asterisks ('**')
+							# will match any trailing path segments.
+							output.append('/.*')
+						else:
+							# A pattern with inner double-asterisks ('**') will match
+							# multiple (or zero) inner path segments.
+							output.append('(?:/.+)?')
+							need_slash = True
+
+					elif seg == '*':
+						# Match single path segment.
+						if need_slash:
+							output.append('/')
+						output.append('[^/]+')
+						need_slash = True
+
 					else:
-						# A pattern with inner double-asterisks ('**') will match
-						# multiple (or zero) inner path segments.
-						output.append('(?:/.+)?')
+						# Match segment glob pattern.
+						if need_slash:
+							output.append('/')
+
+						output.append(cls._translate_segment_glob(seg))
+						if i == end and include is True:
+							# A pattern ending without a slash ('/') will match a file
+							# or a directory (with paths underneath it). E.g., "foo"
+							# matches "foo", "foo/bar", "foo/bar/baz", etc.
+							# EDGE CASE: However, this does not hold for exclusion cases
+							# according to `git check-ignore` (v2.4.1).
+							output.append('(?:/.*)?')
+
 						need_slash = True
-				elif seg == '*':
-					# Match single path segment.
-					if need_slash:
-						output.append('/')
-					output.append('[^/]+')
-					need_slash = True
-				else:
-					# Match segment glob pattern.
-					if need_slash:
-						output.append('/')
-					output.append(cls._translate_segment_glob(seg))
-					if i == end and include is True:
-						# A pattern ending without a slash ('/') will match a file
-						# or a directory (with paths underneath it). E.g., "foo"
-						# matches "foo", "foo/bar", "foo/bar/baz", etc.
-						# EDGE CASE: However, this does not hold for exclusion cases
-						# according to `git check-ignore` (v2.4.1).
-						output.append('(?:/.*)?')
-					need_slash = True
-			output.append('$')
-			regex = ''.join(output)
+
+				output.append('$')
+				regex = ''.join(output)
+
+			else:
+				# Use regex override.
+				regex = override_regex
 
 		else:
 			# A blank pattern is a null-operation (neither includes nor
 			# excludes files).
 			regex = None
 			include = None
 
 		if regex is not None and return_type is bytes:
 			regex = regex.encode(_BYTES_ENCODING)
 
 		return regex, include
 
 	@staticmethod
 	def _translate_segment_glob(pattern):
+		# type: (Text) -> Text
 		"""
 		Translates the glob pattern to a regular expression. This is used in
 		the constructor to translate a path segment glob pattern to its
 		corresponding regular expression.
 
 		*pattern* (:class:`str`) is the glob pattern.
 
@@ -211,92 +266,107 @@
 
 			elif char == '?':
 				# Single-character wildcard. Match any single character (except
 				# a slash).
 				regex += '[^/]'
 
 			elif char == '[':
-				# Braket expression wildcard. Except for the beginning
-				# exclamation mark, the whole braket expression can be used
+				# Bracket expression wildcard. Except for the beginning
+				# exclamation mark, the whole bracket expression can be used
 				# directly as regex but we have to find where the expression
 				# ends.
-				# - "[][!]" matchs ']', '[' and '!'.
-				# - "[]-]" matchs ']' and '-'.
-				# - "[!]a-]" matchs any character except ']', 'a' and '-'.
+				# - "[][!]" matches ']', '[' and '!'.
+				# - "[]-]" matches ']' and '-'.
+				# - "[!]a-]" matches any character except ']', 'a' and '-'.
 				j = i
 				# Pass brack expression negation.
 				if j < end and pattern[j] == '!':
 					j += 1
-				# Pass first closing braket if it is at the beginning of the
+				# Pass first closing bracket if it is at the beginning of the
 				# expression.
 				if j < end and pattern[j] == ']':
 					j += 1
-				# Find closing braket. Stop once we reach the end or find it.
+				# Find closing bracket. Stop once we reach the end or find it.
 				while j < end and pattern[j] != ']':
 					j += 1
 
 				if j < end:
-					# Found end of braket expression. Increment j to be one past
-					# the closing braket:
+					# Found end of bracket expression. Increment j to be one past
+					# the closing bracket:
 					#
 					#  [...]
 					#   ^   ^
 					#   i   j
 					#
 					j += 1
 					expr = '['
 
 					if pattern[i] == '!':
 						# Braket expression needs to be negated.
 						expr += '^'
 						i += 1
 					elif pattern[i] == '^':
-						# POSIX declares that the regex braket expression negation
+						# POSIX declares that the regex bracket expression negation
 						# "[^...]" is undefined in a glob pattern. Python's
 						# `fnmatch.translate()` escapes the caret ('^') as a
 						# literal. To maintain consistency with undefined behavior,
 						# I am escaping the '^' as well.
 						expr += '\\^'
 						i += 1
 
-					# Build regex braket expression. Escape slashes so they are
+					# Build regex bracket expression. Escape slashes so they are
 					# treated as literal slashes by regex as defined by POSIX.
 					expr += pattern[i:j].replace('\\', '\\\\')
 
-					# Add regex braket expression to regex result.
+					# Add regex bracket expression to regex result.
 					regex += expr
 
-					# Set i to one past the closing braket.
+					# Set i to one past the closing bracket.
 					i = j
 
 				else:
-					# Failed to find closing braket, treat opening braket as a
-					# braket literal instead of as an expression.
+					# Failed to find closing bracket, treat opening bracket as a
+					# bracket literal instead of as an expression.
 					regex += '\\['
 
 			else:
 				# Regular character, escape it for regex.
 				regex += re.escape(char)
 
 		return regex
 
 	@staticmethod
 	def escape(s):
+		# type: (AnyStr) -> AnyStr
 		"""
 		Escape special characters in the given string.
 
 		*s* (:class:`unicode` or :class:`bytes`) a filename or a string
 		that you want to escape, usually before adding it to a `.gitignore`
 
-		Returns the escaped string (:class:`unicode`, :class:`bytes`)
+		Returns the escaped string (:class:`unicode` or :class:`bytes`)
 		"""
+		if isinstance(s, unicode):
+			return_type = unicode
+			string = s
+		elif isinstance(s, bytes):
+			return_type = bytes
+			string = s.decode(_BYTES_ENCODING)
+		else:
+			raise TypeError("s:{!r} is not a unicode or byte string.".format(s))
+
 		# Reference: https://git-scm.com/docs/gitignore#_pattern_format
 		meta_characters = r"[]!*#?"
 
-		return "".join("\\" + x if x in meta_characters else x for x in s)
+		out_string = "".join("\\" + x if x in meta_characters else x for x in string)
+
+		if return_type is bytes:
+			return out_string.encode(_BYTES_ENCODING)
+		else:
+			return out_string
 
 util.register_pattern('gitwildmatch', GitWildMatchPattern)
 
 
 class GitIgnorePattern(GitWildMatchPattern):
 	"""
 	The :class:`GitIgnorePattern` class is deprecated by :class:`GitWildMatchPattern`.
@@ -304,15 +374,15 @@
 	"""
 
 	def __init__(self, *args, **kw):
 		"""
 		Warn about deprecation.
 		"""
 		self._deprecated()
-		return super(GitIgnorePattern, self).__init__(*args, **kw)
+		super(GitIgnorePattern, self).__init__(*args, **kw)
 
 	@staticmethod
 	def _deprecated():
 		"""
 		Warn about deprecation.
 		"""
 		warnings.warn("GitIgnorePattern ('gitignore') is deprecated. Use GitWildMatchPattern ('gitwildmatch') instead.", DeprecationWarning, stacklevel=3)
```

### Comparing `pathspec-0.8.1/pathspec/util.py` & `pathspec-0.9.0/pathspec/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,43 @@
 This module provides utility methods for dealing with path-specs.
 """
 
 import os
 import os.path
 import posixpath
 import stat
-
-from .compat import Collection, Iterable, string_types, unicode
+try:
+	from typing import (
+		Any,
+		AnyStr,
+		Callable,
+		Dict,
+		Iterable,
+		Iterator,
+		List,
+		Optional,
+		Sequence,
+		Set,
+		Text,
+		Union)
+except ImportError:
+	pass
+try:
+	# Python 3.6+ type hints.
+	from os import PathLike
+	from typing import Collection
+except ImportError:
+	pass
+
+from .compat import (
+	CollectionType,
+	IterableType,
+	string_types,
+	unicode)
+from .pattern import Pattern
 
 NORMALIZE_PATH_SEPS = [sep for sep in [os.sep, os.altsep] if sep and sep != posixpath.sep]
 """
 *NORMALIZE_PATH_SEPS* (:class:`list` of :class:`str`) contains the path
 separators that need to be normalized to the POSIX separator for the
 current operating system. The separators are determined by examining
 :data:`os.sep` and :data:`os.altsep`.
@@ -22,14 +49,15 @@
 """
 *_registered_patterns* (:class:`dict`) maps a name (:class:`str`) to the
 registered pattern factory (:class:`~collections.abc.Callable`).
 """
 
 
 def detailed_match_files(patterns, files, all_matches=None):
+	# type: (Iterable[Pattern], Iterable[Text], Optional[bool]) -> Dict[Text, 'MatchDetail']
 	"""
 	Matches the files to the patterns, and returns which patterns matched
 	the files.
 
 	*patterns* (:class:`~collections.abc.Iterable` of :class:`~pathspec.pattern.Pattern`)
 	contains the patterns to use.
 
@@ -39,15 +67,15 @@
 	*all_matches* (:class:`boot` or :data:`None`) is whether to return all
 	matches patterns (:data:`True`), or only the last matched pattern
 	(:data:`False`). Default is :data:`None` for :data:`False`.
 
 	Returns the matched files (:class:`dict`) which maps each matched file
 	(:class:`str`) to the patterns that matched in order (:class:`.MatchDetail`).
 	"""
-	all_files = files if isinstance(files, Collection) else list(files)
+	all_files = files if isinstance(files, CollectionType) else list(files)
 	return_files = {}
 	for pattern in patterns:
 		if pattern.include is not None:
 			result_files = pattern.match(all_files)
 			if pattern.include:
 				# Add files and record pattern.
 				for result_file in result_files:
@@ -64,25 +92,27 @@
 				for file in result_files:
 					del return_files[file]
 
 	return return_files
 
 
 def _is_iterable(value):
+	# type: (Any) -> bool
 	"""
 	Check whether the value is an iterable (excludes strings).
 
 	*value* is the value to check,
 
 	Returns whether *value* is a iterable (:class:`bool`).
 	"""
-	return isinstance(value, Iterable) and not isinstance(value, (unicode, bytes))
+	return isinstance(value, IterableType) and not isinstance(value, (unicode, bytes))
 
 
 def iter_tree_entries(root, on_error=None, follow_links=None):
+	# type: (Text, Optional[Callable], Optional[bool]) -> Iterator['TreeEntry']
 	"""
 	Walks the specified directory for all files and directories.
 
 	*root* (:class:`str`) is the root directory to search.
 
 	*on_error* (:class:`~collections.abc.Callable` or :data:`None`)
 	optionally is the error handler for file-system exceptions. It will be
@@ -92,28 +122,29 @@
 
 	*follow_links* (:class:`bool` or :data:`None`) optionally is whether
 	to walk symbolic links that resolve to directories. Default is
 	:data:`None` for :data:`True`.
 
 	Raises :exc:`RecursionError` if recursion is detected.
 
-	Returns an :class:`~collections.abc.Iterable` yielding each file or
+	Returns an :class:`~collections.abc.Iterator` yielding each file or
 	directory entry (:class:`.TreeEntry`) relative to *root*.
 	"""
 	if on_error is not None and not callable(on_error):
 		raise TypeError("on_error:{!r} is not callable.".format(on_error))
 
 	if follow_links is None:
 		follow_links = True
 
 	for entry in _iter_tree_entries_next(os.path.abspath(root), '', {}, on_error, follow_links):
 		yield entry
 
 
 def iter_tree_files(root, on_error=None, follow_links=None):
+	# type: (Text, Optional[Callable], Optional[bool]) -> Iterator[Text]
 	"""
 	Walks the specified directory for all files.
 
 	*root* (:class:`str`) is the root directory to search for files.
 
 	*on_error* (:class:`~collections.abc.Callable` or :data:`None`)
 	optionally is the error handler for file-system exceptions. It will be
@@ -123,15 +154,15 @@
 
 	*follow_links* (:class:`bool` or :data:`None`) optionally is whether
 	to walk symbolic links that resolve to directories. Default is
 	:data:`None` for :data:`True`.
 
 	Raises :exc:`RecursionError` if recursion is detected.
 
-	Returns an :class:`~collections.abc.Iterable` yielding the path to
+	Returns an :class:`~collections.abc.Iterator` yielding the path to
 	each file (:class:`str`) relative to *root*.
 	"""
 	if on_error is not None and not callable(on_error):
 		raise TypeError("on_error:{!r} is not callable.".format(on_error))
 
 	if follow_links is None:
 		follow_links = True
@@ -142,14 +173,15 @@
 
 
 # Alias `iter_tree_files()` as `iter_tree()`.
 iter_tree = iter_tree_files
 
 
 def _iter_tree_entries_next(root_full, dir_rel, memo, on_error, follow_links):
+	# type: (Text, Text, Dict[Text, Text], Callable, bool) -> Iterator['TreeEntry']
 	"""
 	Scan the directory for all descendant files.
 
 	*root_full* (:class:`str`) the absolute path to the root directory.
 
 	*dir_rel* (:class:`str`) the path to the directory to scan relative to
 	*root_full*.
@@ -219,26 +251,28 @@
 	# same directory to appear multiple times. If this is not done, the
 	# second occurrence of the directory will be incorrectly interpreted
 	# as a recursion. See <https://github.com/cpburnz/python-path-specification/pull/7>.
 	del memo[dir_real]
 
 
 def lookup_pattern(name):
+	# type: (Text) -> Callable[[AnyStr], Pattern]
 	"""
 	Lookups a registered pattern factory by name.
 
 	*name* (:class:`str`) is the name of the pattern factory.
 
 	Returns the registered pattern factory (:class:`~collections.abc.Callable`).
 	If no pattern factory is registered, raises :exc:`KeyError`.
 	"""
 	return _registered_patterns[name]
 
 
 def match_file(patterns, file):
+	# type: (Iterable[Pattern], Text) -> bool
 	"""
 	Matches the file to the patterns.
 
 	*patterns* (:class:`~collections.abc.Iterable` of :class:`~pathspec.pattern.Pattern`)
 	contains the patterns to use.
 
 	*file* (:class:`str`) is the normalized file path to be matched
@@ -251,38 +285,40 @@
 		if pattern.include is not None:
 			if file in pattern.match((file,)):
 				matched = pattern.include
 	return matched
 
 
 def match_files(patterns, files):
+	# type: (Iterable[Pattern], Iterable[Text]) -> Set[Text]
 	"""
 	Matches the files to the patterns.
 
 	*patterns* (:class:`~collections.abc.Iterable` of :class:`~pathspec.pattern.Pattern`)
 	contains the patterns to use.
 
 	*files* (:class:`~collections.abc.Iterable` of :class:`str`) contains
 	the normalized file paths to be matched against *patterns*.
 
 	Returns the matched files (:class:`set` of :class:`str`).
 	"""
-	all_files = files if isinstance(files, Collection) else list(files)
+	all_files = files if isinstance(files, CollectionType) else list(files)
 	return_files = set()
 	for pattern in patterns:
 		if pattern.include is not None:
 			result_files = pattern.match(all_files)
 			if pattern.include:
 				return_files.update(result_files)
 			else:
 				return_files.difference_update(result_files)
 	return return_files
 
 
 def _normalize_entries(entries, separators=None):
+	# type: (Iterable['TreeEntry'], Optional[Collection[Text]]) -> Dict[Text, 'TreeEntry']
 	"""
 	Normalizes the entry paths to use the POSIX path separator.
 
 	*entries* (:class:`~collections.abc.Iterable` of :class:`.TreeEntry`)
 	contains the entries to be normalized.
 
 	*separators* (:class:`~collections.abc.Collection` of :class:`str`; or
@@ -295,16 +331,18 @@
 	norm_files = {}
 	for entry in entries:
 		norm_files[normalize_file(entry.path, separators=separators)] = entry
 	return norm_files
 
 
 def normalize_file(file, separators=None):
+	# type: (Union[Text, PathLike], Optional[Collection[Text]]) -> Text
 	"""
-	Normalizes the file path to use the POSIX path separator (i.e., ``'/'``).
+	Normalizes the file path to use the POSIX path separator (i.e.,
+	``'/'``), and make the paths relative (remove leading ``'/'``).
 
 	*file* (:class:`str` or :class:`pathlib.PurePath`) is the file path.
 
 	*separators* (:class:`~collections.abc.Collection` of :class:`str`; or
 	:data:`None`) optionally contains the path separators to normalize.
 	This does not need to include the POSIX path separator (``'/'``), but
 	including it will not affect the results. Default is :data:`None` for
@@ -319,42 +357,54 @@
 
 	# Convert path object to string.
 	norm_file = str(file)
 
 	for sep in separators:
 		norm_file = norm_file.replace(sep, posixpath.sep)
 
-	# Remove current directory prefix.
-	if norm_file.startswith('./'):
+	if norm_file.startswith('/'):
+		# Make path relative.
+		norm_file = norm_file[1:]
+
+	elif norm_file.startswith('./'):
+		# Remove current directory prefix.
 		norm_file = norm_file[2:]
 
 	return norm_file
 
 
 def normalize_files(files, separators=None):
+	# type: (Iterable[Union[str, PathLike]], Optional[Collection[Text]]) -> Dict[Text, List[Union[str, PathLike]]]
 	"""
 	Normalizes the file paths to use the POSIX path separator.
 
 	*files* (:class:`~collections.abc.Iterable` of :class:`str` or
 	:class:`pathlib.PurePath`) contains the file paths to be normalized.
 
 	*separators* (:class:`~collections.abc.Collection` of :class:`str`; or
 	:data:`None`) optionally contains the path separators to normalize.
 	See :func:`normalize_file` for more information.
 
-	Returns a :class:`dict` mapping the each normalized file path (:class:`str`)
-	to the original file path (:class:`str`)
+	Returns a :class:`dict` mapping the each normalized file path
+	(:class:`str`) to the original file paths (:class:`list` of
+	:class:`str` or :class:`pathlib.PurePath`).
 	"""
 	norm_files = {}
 	for path in files:
-		norm_files[normalize_file(path, separators=separators)] = path
+		norm_file = normalize_file(path, separators=separators)
+		if norm_file in norm_files:
+			norm_files[norm_file].append(path)
+		else:
+			norm_files[norm_file] = [path]
+
 	return norm_files
 
 
 def register_pattern(name, pattern_factory, override=None):
+	# type: (Text, Callable[[AnyStr], Pattern], Optional[bool]) -> None
 	"""
 	Registers the specified pattern factory.
 
 	*name* (:class:`str`) is the name to register the pattern factory
 	under.
 
 	*pattern_factory* (:class:`~collections.abc.Callable`) is used to
@@ -378,57 +428,62 @@
 class AlreadyRegisteredError(Exception):
 	"""
 	The :exc:`AlreadyRegisteredError` exception is raised when a pattern
 	factory is registered under a name already in use.
 	"""
 
 	def __init__(self, name, pattern_factory):
+		# type: (Text, Callable[[AnyStr], Pattern]) -> None
 		"""
 		Initializes the :exc:`AlreadyRegisteredError` instance.
 
 		*name* (:class:`str`) is the name of the registered pattern.
 
 		*pattern_factory* (:class:`~collections.abc.Callable`) is the
 		registered pattern factory.
 		"""
 		super(AlreadyRegisteredError, self).__init__(name, pattern_factory)
 
 	@property
 	def message(self):
+		# type: () -> Text
 		"""
 		*message* (:class:`str`) is the error message.
 		"""
 		return "{name!r} is already registered for pattern factory:{pattern_factory!r}.".format(
 			name=self.name,
 			pattern_factory=self.pattern_factory,
 		)
 
 	@property
 	def name(self):
+		# type: () -> Text
 		"""
 		*name* (:class:`str`) is the name of the registered pattern.
 		"""
 		return self.args[0]
 
 	@property
 	def pattern_factory(self):
+		# type: () -> Callable[[AnyStr], Pattern]
 		"""
 		*pattern_factory* (:class:`~collections.abc.Callable`) is the
 		registered pattern factory.
 		"""
 		return self.args[1]
 
 
 class RecursionError(Exception):
 	"""
 	The :exc:`RecursionError` exception is raised when recursion is
 	detected.
 	"""
 
 	def __init__(self, real_path, first_path, second_path):
+		# type: (Text, Text, Text) -> None
 		"""
 		Initializes the :exc:`RecursionError` instance.
 
 		*real_path* (:class:`str`) is the real path that recursion was
 		encountered on.
 
 		*first_path* (:class:`str`) is the first path encountered for
@@ -437,41 +492,45 @@
 		*second_path* (:class:`str`) is the second path encountered for
 		*real_path*.
 		"""
 		super(RecursionError, self).__init__(real_path, first_path, second_path)
 
 	@property
 	def first_path(self):
+		# type: () -> Text
 		"""
 		*first_path* (:class:`str`) is the first path encountered for
 		:attr:`self.real_path <RecursionError.real_path>`.
 		"""
 		return self.args[1]
 
 	@property
 	def message(self):
+		# type: () -> Text
 		"""
 		*message* (:class:`str`) is the error message.
 		"""
 		return "Real path {real!r} was encountered at {first!r} and then {second!r}.".format(
 			real=self.real_path,
 			first=self.first_path,
 			second=self.second_path,
 		)
 
 	@property
 	def real_path(self):
+		# type: () -> Text
 		"""
 		*real_path* (:class:`str`) is the real path that recursion was
 		encountered on.
 		"""
 		return self.args[0]
 
 	@property
 	def second_path(self):
+		# type: () -> Text
 		"""
 		*second_path* (:class:`str`) is the second path encountered for
 		:attr:`self.real_path <RecursionError.real_path>`.
 		"""
 		return self.args[2]
 
 
@@ -480,14 +539,15 @@
 	The :class:`.MatchDetail` class contains information about
 	"""
 
 	#: Make the class dict-less.
 	__slots__ = ('patterns',)
 
 	def __init__(self, patterns):
+		# type: (Sequence[Pattern]) -> None
 		"""
 		Initialize the :class:`.MatchDetail` instance.
 
 		*patterns* (:class:`~collections.abc.Sequence` of :class:`~pathspec.pattern.Pattern`)
 		contains the patterns that matched the file in the order they were
 		encountered.
 		"""
@@ -506,14 +566,15 @@
 	entry.
 	"""
 
 	#: Make the class dict-less.
 	__slots__ = ('_lstat', 'name', 'path', '_stat')
 
 	def __init__(self, name, path, lstat, stat):
+		# type: (Text, Text, os.stat_result, os.stat_result) -> None
 		"""
 		Initialize the :class:`.TreeEntry` instance.
 
 		*name* (:class:`str`) is the base name of the entry.
 
 		*path* (:class:`str`) is the relative path of the entry.
 
@@ -543,14 +604,15 @@
 		self._stat = stat
 		"""
 		*_stat* (:class:`~os.stat_result`) is the stat result of the linked
 		entry.
 		"""
 
 	def is_dir(self, follow_links=None):
+		# type: (Optional[bool]) -> bool
 		"""
 		Get whether the entry is a directory.
 
 		*follow_links* (:class:`bool` or :data:`None`) is whether to follow
 		symbolic links. If this is :data:`True`, a symlink to a directory
 		will result in :data:`True`. Default is :data:`None` for :data:`True`.
 
@@ -559,14 +621,15 @@
 		if follow_links is None:
 			follow_links = True
 
 		node_stat = self._stat if follow_links else self._lstat
 		return stat.S_ISDIR(node_stat.st_mode)
 
 	def is_file(self, follow_links=None):
+		# type: (Optional[bool]) -> bool
 		"""
 		Get whether the entry is a regular file.
 
 		*follow_links* (:class:`bool` or :data:`None`) is whether to follow
 		symbolic links. If this is :data:`True`, a symlink to a regular file
 		will result in :data:`True`. Default is :data:`None` for :data:`True`.
 
@@ -575,20 +638,22 @@
 		if follow_links is None:
 			follow_links = True
 
 		node_stat = self._stat if follow_links else self._lstat
 		return stat.S_ISREG(node_stat.st_mode)
 
 	def is_symlink(self):
+		# type: () -> bool
 		"""
 		Returns whether the entry is a symbolic link (:class:`bool`).
 		"""
 		return stat.S_ISLNK(self._lstat.st_mode)
 
 	def stat(self, follow_links=None):
+		# type: (Optional[bool]) -> os.stat_result
 		"""
 		Get the cached stat result for the entry.
 
 		*follow_links* (:class:`bool` or :data:`None`) is whether to follow
 		symbolic links. If this is :data:`True`, the stat result of the
 		linked file will be returned. Default is :data:`None` for :data:`True`.
```

### Comparing `pathspec-0.8.1/pathspec/compat.py` & `pathspec-0.9.0/pathspec/compat.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,7 +32,10 @@
 
 try:
 	# Python 3.6+.
 	from collections.abc import Collection
 except ImportError:
 	# Python 2.7 - 3.5.
 	from collections import Container as Collection
+
+CollectionType = Collection
+IterableType = Iterable
```

### Comparing `pathspec-0.8.1/pathspec.egg-info/PKG-INFO` & `pathspec-0.9.0/pathspec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pathspec
-Version: 0.8.1
+Version: 0.9.0
 Summary: Utility library for gitignore style pattern matching of file paths.
 Home-page: https://github.com/cpburnz/python-path-specification
 Author: Caleb P. Burns
 Author-email: cpburnz@gmail.com
 License: MPL 2.0
-Description: *pathspec*: Path Specification
+Description: 
+        *pathspec*: Path Specification
         ==============================
         
         *pathspec* is a utility library for pattern matching of file paths. So
         far this only includes Git's wildmatch pattern matching which itself is
         derived from Rsync's wildmatch. Git uses wildmatch for its `gitignore`_
         files.
         
@@ -155,17 +156,33 @@
         Other Languages
         ---------------
         
         *pathspec* is also available as a `Ruby gem`_.
         
         .. _`Ruby gem`: https://github.com/highb/pathspec-ruby
         
+        
         Change History
         ==============
         
+        0.9.0 (2021-07-17)
+        ------------------
+        
+        - `Issue #44`_/`Issue #50`_: Raise `GitWildMatchPatternError` for invalid git patterns.
+        - `Issue #45`_: Fix for duplicate leading double-asterisk, and edge cases.
+        - `Issue #46`_: Fix matching absolute paths.
+        - API change: `util.normalize_files()` now returns a `Dict[str, List[pathlike]]` instead of a `Dict[str, pathlike]`.
+        - Added type hinting.
+        
+        .. _`Issue #44`: https://github.com/cpburnz/python-path-specification/issues/44
+        .. _`Issue #45`: https://github.com/cpburnz/python-path-specification/pull/45
+        .. _`Issue #46`: https://github.com/cpburnz/python-path-specification/issues/46
+        .. _`Issue #50`: https://github.com/cpburnz/python-path-specification/pull/50
+        
+        
         0.8.1 (2020-11-07)
         ------------------
         
         - `Issue #43`_: Add support for addition operator.
         
         .. _`Issue #43`: https://github.com/cpburnz/python-path-specification/pull/43
         
@@ -365,25 +382,28 @@
         - Fixed relative path gitignore patterns.
         
         
         0.2.0 (2013-12-07)
         ------------------
         
         - Initial release.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7
+Description-Content-Type: text/x-rst
```

### Comparing `pathspec-0.8.1/README.rst` & `pathspec-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pathspec-0.8.1/PKG-INFO` & `pathspec-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pathspec
-Version: 0.8.1
+Version: 0.9.0
 Summary: Utility library for gitignore style pattern matching of file paths.
 Home-page: https://github.com/cpburnz/python-path-specification
 Author: Caleb P. Burns
 Author-email: cpburnz@gmail.com
 License: MPL 2.0
-Description: *pathspec*: Path Specification
+Description: 
+        *pathspec*: Path Specification
         ==============================
         
         *pathspec* is a utility library for pattern matching of file paths. So
         far this only includes Git's wildmatch pattern matching which itself is
         derived from Rsync's wildmatch. Git uses wildmatch for its `gitignore`_
         files.
         
@@ -155,17 +156,33 @@
         Other Languages
         ---------------
         
         *pathspec* is also available as a `Ruby gem`_.
         
         .. _`Ruby gem`: https://github.com/highb/pathspec-ruby
         
+        
         Change History
         ==============
         
+        0.9.0 (2021-07-17)
+        ------------------
+        
+        - `Issue #44`_/`Issue #50`_: Raise `GitWildMatchPatternError` for invalid git patterns.
+        - `Issue #45`_: Fix for duplicate leading double-asterisk, and edge cases.
+        - `Issue #46`_: Fix matching absolute paths.
+        - API change: `util.normalize_files()` now returns a `Dict[str, List[pathlike]]` instead of a `Dict[str, pathlike]`.
+        - Added type hinting.
+        
+        .. _`Issue #44`: https://github.com/cpburnz/python-path-specification/issues/44
+        .. _`Issue #45`: https://github.com/cpburnz/python-path-specification/pull/45
+        .. _`Issue #46`: https://github.com/cpburnz/python-path-specification/issues/46
+        .. _`Issue #50`: https://github.com/cpburnz/python-path-specification/pull/50
+        
+        
         0.8.1 (2020-11-07)
         ------------------
         
         - `Issue #43`_: Add support for addition operator.
         
         .. _`Issue #43`: https://github.com/cpburnz/python-path-specification/pull/43
         
@@ -365,25 +382,28 @@
         - Fixed relative path gitignore patterns.
         
         
         0.2.0 (2013-12-07)
         ------------------
         
         - Initial release.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7
+Description-Content-Type: text/x-rst
```

### Comparing `pathspec-0.8.1/LICENSE` & `pathspec-0.9.0/LICENSE`

 * *Files identical despite different names*

