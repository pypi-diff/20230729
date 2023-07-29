# Comparing `tmp/portablemc-3.3.1.tar.gz` & `tmp/portablemc-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portablemc-3.3.1.tar", max compression
+gzip compressed data, was "portablemc-4.0.0rc1.tar", max compression
```

## Comparing `portablemc-3.3.1.tar` & `portablemc-4.0.0rc1.tar`

### file list

```diff
@@ -1,7 +1,18 @@
--rw-r--r--   0        0        0    82267 2023-04-01 13:48:53.477205 portablemc-3.3.1/portablemc/__init__.py
--rw-r--r--   0        0        0      800 2023-02-03 21:20:02.472494 portablemc-3.3.1/portablemc/__main__.py
--rw-r--r--   0        0        0    56450 2023-04-01 10:22:23.807431 portablemc-3.3.1/portablemc/cli.py
--rw-r--r--   0        0        0      895 2023-04-01 13:48:45.858097 portablemc-3.3.1/pyproject.toml
--rw-r--r--   0        0        0      104 2022-06-12 20:34:32.676104 portablemc-3.3.1/README.md
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 portablemc-3.3.1/setup.py
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 portablemc-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 20:55:06.871777 portablemc-4.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    14683 2023-07-29 19:17:52.174139 portablemc-4.0.0rc1/README.md
+-rw-r--r--   0        0        0      306 2023-07-22 19:03:05.137436 portablemc-4.0.0rc1/portablemc/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-14 20:55:06.888443 portablemc-4.0.0rc1/portablemc/__main__.py
+-rw-r--r--   0        0        0    16930 2023-07-29 18:39:34.554294 portablemc-4.0.0rc1/portablemc/auth.py
+-rw-r--r--   0        0        0    28227 2023-07-29 19:42:29.366986 portablemc-4.0.0rc1/portablemc/cli/__init__.py
+-rw-r--r--   0        0        0    13780 2023-07-29 19:58:42.262680 portablemc-4.0.0rc1/portablemc/cli/lang.py
+-rw-r--r--   0        0        0     9442 2023-07-29 20:10:30.949309 portablemc-4.0.0rc1/portablemc/cli/output.py
+-rw-r--r--   0        0        0     7297 2023-07-29 19:06:02.641566 portablemc-4.0.0rc1/portablemc/cli/parse.py
+-rw-r--r--   0        0        0     3034 2023-07-28 21:45:28.559579 portablemc-4.0.0rc1/portablemc/cli/util.py
+-rw-r--r--   0        0        0    12222 2023-07-29 20:26:00.437021 portablemc-4.0.0rc1/portablemc/download.py
+-rw-r--r--   0        0        0     5322 2023-07-29 16:13:33.741775 portablemc-4.0.0rc1/portablemc/fabric.py
+-rw-r--r--   0        0        0    18738 2023-07-29 16:13:49.891610 portablemc-4.0.0rc1/portablemc/forge.py
+-rw-r--r--   0        0        0     2373 2023-07-15 10:13:00.771725 portablemc-4.0.0rc1/portablemc/http.py
+-rw-r--r--   0        0        0    75003 2023-07-29 19:33:08.560588 portablemc-4.0.0rc1/portablemc/standard.py
+-rw-r--r--   0        0        0     5040 2023-07-23 13:48:34.873644 portablemc-4.0.0rc1/portablemc/util.py
+-rw-r--r--   0        0        0      950 2023-07-22 19:08:50.757737 portablemc-4.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    15730 1970-01-01 00:00:00.000000 portablemc-4.0.0rc1/PKG-INFO
```

### Comparing `portablemc-3.3.1/portablemc/__init__.py` & `portablemc-4.0.0rc1/portablemc/standard.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,1958 +1,1820 @@
-# encoding: utf-8
-
-# Copyright (C) 2021-2023  Théo Rozier
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-"""
-Core module of PortableMC, it provides a flexible API to download and start Minecraft.
+"""Definition of standard version supporting the standard metadata format used by Mojang. 
+This module also provide Mojang's version manifest which can be used as default version
+repository, allowing resolution of what we call "vanilla" versions.
 """
 
-from typing import cast, Generator, Callable, Optional, Tuple, Dict, Type, List
-from http.client import HTTPConnection, HTTPSConnection, HTTPResponse, HTTPException
-from urllib import parse as url_parse, request as url_request
-from urllib.request import Request as UrlRequest
-from uuid import uuid4, uuid5, UUID
-from urllib.error import HTTPError
+from subprocess import Popen, TimeoutExpired, PIPE, STDOUT
+import xml.etree.ElementTree as ET
 from json import JSONDecodeError
-from datetime import datetime
-from zipfile import ZipFile
-from os import path
+from pathlib import Path
+from uuid import uuid4
 import platform
-import hashlib
 import shutil
-import base64
 import json
-import ssl
-import os
 import re
+import os
 
+from .download import DownloadList, DownloadEntry, DownloadResultProgress, DownloadResultError
+from .util import jvm_bin_filename, merge_dict, calc_input_sha1, LibrarySpecifier
+from .auth import AuthSession, OfflineAuthSession
+from .http import http_request, HttpError
+from . import LAUNCHER_NAME, LAUNCHER_VERSION
 
-__all__ = [
-    "LAUNCHER_NAME", "LAUNCHER_VERSION", "LAUNCHER_AUTHORS", "LAUNCHER_COPYRIGHT", "LAUNCHER_URL",
-    "Context", "Version", "StartOptions", "Start", "VersionManifest",
-    "AuthSession", "OfflineAuthSession", "YggdrasilAuthSession", "MicrosoftAuthSession", "AuthDatabase",
-    "DownloadEntry", "DownloadList", "DownloadProgress", "DownloadEntryProgress", "DownloadReport",
-    "BaseError", "JsonRequestError", "AuthError", "VersionManifestError", "VersionError", "JvmLoadingError",
-        "BinaryNotFound",
-    "LibrarySpecifier",
-    "http_request", "json_request", "json_simple_request",
-    "merge_dict",
-    "interpret_rule_os", "interpret_rule", "interpret_args",
-    "replace_vars", "replace_list_vars",
-    "get_minecraft_dir", "get_minecraft_os", "get_minecraft_arch", "get_minecraft_archbits", "get_minecraft_jvm_os",
-    "get_jvm_bin_filename",
-    "can_extract_native",
-    "from_iso_date",
-    # "calc_input_sha1",  TODO: To add in the future when stabilized
-    "LEGACY_JVM_ARGUMENTS"
-]
-
-
-LAUNCHER_NAME = "portablemc"
-LAUNCHER_VERSION = "3.3.1"
-LAUNCHER_AUTHORS = ["Théo Rozier <contact@theorozier.fr>", "Github contributors"]
-LAUNCHER_COPYRIGHT = "PortableMC  Copyright (C) 2021-2023  Théo Rozier"
-LAUNCHER_URL = "https://github.com/mindstorm38/portablemc"
+from typing import Optional, Iterator, Dict, List, Tuple, Any, Callable, Set
 
 
 RESOURCES_URL = "https://resources.download.minecraft.net/"
 LIBRARIES_URL = "https://libraries.minecraft.net/"
-VERSION_MANIFEST_URL = "https://piston-meta.mojang.com/mc/game/version_manifest_v2.json"
 JVM_META_URL = "https://piston-meta.mojang.com/v1/products/java-runtime/2ec0cc96c44e5a76b9c8b7c39df7210883d12871/all.json"
+VERSION_MANIFEST_URL = "https://piston-meta.mojang.com/mc/game/version_manifest_v2.json"
 
 
 class Context:
-
-    """
-    This class is used to manage an installation context for Minecraft. This context can be reused multiple
-    times to install multiple versions. A context stores multiple important paths but all these paths can be
-    changed after the construction and before preparing versions.
+    """Context of the game's installation and runtime. This defines various directories
+    where versions, assets, libraries or JVM are stored, as well as a bin directory for
+    temporary runtime files, and also a working directory from where the game will run.
     """
 
-    def __init__(self, main_dir: Optional[str] = None, work_dir: Optional[str] = None):
-
-        """
-        Construct a Minecraft context. The main directory `main_dir` is used to construct versions, assets, libraries
-        and JVM directories, but it is not stored afterward. The working directory `work_dir` (also named "game
-        directory"), however it is stored as-is.\n
-        By default `main_dir` is set to the default .minecraft (https://minecraft.fandom.com/fr/wiki/.minecraft) and
-        `work_dir` is set by default to the value of `main_dir`.
+    def __init__(self, 
+        main_dir: Optional[Path] = None, 
+        work_dir: Optional[Path] = None
+    ) -> None:
+        """Construct a Minecraft installation context. This context is used by most of the
+        installer's tasks to know where to install files and from where to launch the game.
+
+        :param main_dir: The main directory where versions, assets, libraries and 
+        optionally JVM are installed. If not specified this path will be set the usual 
+        `.minecraft` (see https://minecraft.fandom.com/fr/wiki/.minecraft).
+        :param work_dir: The working directory from where the game is run, the game stores
+        thing like saves, resource packs, options and mods if relevant. This defaults to
+        `main_dir` if not specified.
+        """
+
+        main_dir = get_minecraft_dir() if main_dir is None else main_dir
+        self.work_dir = main_dir if work_dir is None else work_dir
+        self.versions_dir = main_dir / "versions"
+        self.assets_dir = main_dir / "assets"
+        self.libraries_dir = main_dir / "libraries"
+        self.jvm_dir = main_dir / "jvm"
+        self.bin_dir = self.work_dir / "bin"
+
+    def get_version(self, version: str) -> "VersionHandle":
+        """Get a version's handle.
+        """
+        return VersionHandle(version, self.versions_dir / version)
+
+    def list_versions(self) -> "Iterator[VersionHandle]":
+        """List installed versions given their handles.
+        """
+        if self.versions_dir.is_dir():
+            for version_dir in self.versions_dir.iterdir():
+                if version_dir.is_dir():
+                    version = VersionHandle(version_dir.name, version_dir)
+                    if version.metadata_exists():
+                        yield version
+    
+    def gen_bin_dir(self) -> Path:
+        """Generate a random named binary directory, may be used for any kind of temporary
+        files and data. Usually for shared libraries used by the game. Note that this 
+        directory isn't created by this method, only its path is returned.
         """
+        return self.bin_dir / str(uuid4())
 
-        main_dir = get_minecraft_dir() if main_dir is None else path.realpath(main_dir)
-        self.work_dir = main_dir if work_dir is None else path.realpath(work_dir)
-        self.versions_dir = path.join(main_dir, "versions")
-        self.assets_dir = path.join(main_dir, "assets")
-        self.libraries_dir = path.join(main_dir, "libraries")
-        self.jvm_dir = path.join(main_dir, "jvm")
-        self.bin_dir = path.join(self.work_dir, "bin")
 
-    def has_version_metadata(self, version: str) -> bool:
-        """ Return True if the given version has a metadata file. """
-        return path.isfile(path.join(self.versions_dir, version, f"{version}.json"))
-
-    def get_version_dir(self, version_id: str) -> str:
-        return path.join(self.versions_dir, version_id)
-
-    def list_versions(self) -> Generator[Tuple[str, int], None, None]:
-        """ A generator method that yields all versions (version, mtime) that have a version metadata file. """
-        if path.isdir(self.versions_dir):
-            for version in os.listdir(self.versions_dir):
-                try:
-                    yield version, path.getmtime(path.join(self.versions_dir, version, f"{version}.json"))
-                except OSError:
-                    pass
+class Watcher:
+    """Base class for a watcher of the install process.
+    """
+    
+    def handle(self, event: Any) -> None:
+        """Called when the watcher can handle the given event. Default implementation
+        does nothing.
+        """
 
 
-class Version:
+class VersionHandle:
+    """This class holds a version handle that allows modifying its metadata, reading and
+    writing it. The parents of this version can also be linked and then merged together
+    to get a full metadata.
 
-    """
-    This class is used to manage the installation of a version and then run it.\n
-    All public function in this class can be executed multiple times, however they might add duplicate URLs to
-    the download list. The game still requires some parts to be prepared before starting.
+    This class cannot really be used as a complete version to prepare tasks on, this is
+    rather a handle that defines its hierarchical chain of versions.
     """
 
-    def __init__(self, context: Context, version_id: str):
+    __slots__ = "id", "dir", "metadata", "parent"
 
-        """ Construct a new version, using a specific context and the exact version ID you want to start. """
+    def __init__(self, id: str, dir: Path) -> None:
+        self.id = id
+        self.dir = dir
+        self.metadata = {}
+        self.parent: Optional[VersionHandle] = None
+    
+    def metadata_exists(self) -> bool:
+        """This function returns true if the version's metadata file exists.
+        """
+        return self.metadata_file().is_file()
+    
+    def metadata_file(self) -> Path:
+        """This function returns the computed path of the metadata file.
+        """
+        return self.dir / f"{self.id}.json"
 
-        self.context = context
-        self.id = version_id
+    def jar_file(self) -> Path:
+        """This function returns the computed path of the JAR file of the game.
+        """
+        return self.dir / f"{self.id}.jar"
 
-        self.manifest: Optional[VersionManifest] = None
-        self.dl = DownloadList()
+    def write_metadata_file(self) -> None:
+        """This function write the metadata file of the version with the internal data.
+        """
+        self.dir.mkdir(parents=True, exist_ok=True)
+        with self.metadata_file().open("wt") as fp:
+            json.dump(self.metadata, fp)
 
-        self.version_meta: Optional[dict] = None
-        self.version_dir: Optional[str] = None
-        self.version_jar_file: Optional[str] = None
+    def read_metadata_file(self) -> bool:
+        """This function reads the metadata file and updates the internal data if found.
 
-        self.assets_index_version: Optional[str] = None
-        self.assets_virtual_dir: Optional[str] = None
-        self.assets_count: Optional[int] = None
+        :return: True if the data was actually updated from the file.
+        """
+        try:
+            with self.metadata_file().open("rt") as fp:
+                self.metadata = json.load(fp)
+            return True
+        except (OSError, JSONDecodeError):
+            return False
+    
+    def recurse(self) -> "Iterator[VersionHandle]":
+        """Walk through every version metadata in the hierarchy of the current one.
+        """
+        version_meta = self
+        while version_meta is not None:
+            yield version_meta
+            version_meta = version_meta.parent
+    
+    def merge(self) -> dict:
+        """Merge this version metadata and all of its parents into a `FullMetadata`.
+        """
+        result = {}
+        for version_meta in self.recurse():
+            merge_dict(result, version_meta.metadata)
+        return result
+
+
+class Environment:
+    """Describe the game's environment needed to run it. Such instance is produced by
+    installing a version and may be used to run the game.
+
+    Note that native libs can contain both JAR files with dynamic libraries inside them 
+    and paths to dynamic libraries. The latter being symlinked in the bin directory, or
+    copied if not possible (lacking permission on Windows).
+    """
 
-        self.logging_file: Optional[str] = None
-        self.logging_argument: Optional[str] = None
+    def __init__(self, context: Context, main_class: str) -> None:
+        self.context = context
+        self.jvm_args: List[str] = []
+        self.game_args: List[str] = []
+        self.main_class = main_class
+        self.args_replacements: Dict[str, str] = {}
+        self.native_libs: List[Path] = []
+        self.fixes: Dict[str, Any] = {}
+    
+    def run(self, runner: "Optional[Runner]" = None) -> None:
+        """Run this game's environment, with an optional custom runner.
+        """
+        (runner or StandardRunner()).run(self)
 
-        self.classpath_libs: List[str] = []
-        self.native_libs: List[str] = []
+class Runner:
+    """Base class handling game running, this default implementation just create a
+    process and forwards to its outputs to the outputs of the current process.
+    """
 
-        self.jvm_version: Optional[str] = None
-        self.jvm_exec: Optional[str] = None
+    def run(self, env: Environment) -> None:
+        raise NotImplementedError
 
-    def _ensure_version_manifest(self) -> 'VersionManifest':
-        if self.manifest is None:
-            self.manifest = VersionManifest()
-        return self.manifest
 
-    def _check_version_meta(self):
-        if self.version_meta is None:
-            raise ValueError("You should install metadata first.")
+class Version:
+    """Base class for basic version resolving, it handles metadata parsing and resources
+    resolution. This class provides support for standard versions as provided by the
+    Mojang's version manifest.
+    """
+    
+    FIX_LEGACY_PROXY = "legacy_proxy"
+    FIX_LEGACY_MERGE_SORT = "legacy_merge_sort"
+    FIX_LEGACY_RESOLUTION = "legacy_resolution"
+    FIX_LEGACY_QUICK_PLAY = "legacy_quick_play"
+    FIX_AUTH_LIB_2_1_28 = "auth_lib_2_1_28"
+    FIX_LWJGL = "lwjgl"
+
+    def __init__(self, version: str = "release", *, 
+        context: Optional[Context] = None,
+    ) -> None:
+        """Construct a standard version installer and runner.
+
+        :param context: The installation context of the game, used to know where to find
+        its metadata and where to install resources. If the context is not given, the 
+        default one is constructed (see Context documentation).
+        :param version: The root version to resolve at first, all of its parents will
+        be loaded and then all the metadata will be merged together. This merged metadata
+        will be used by this class to install its resources such as libraries and assets.
+        """
 
-    def prepare_meta(self, *, recursion_limit: int = 50):
+        # Entry attributes
+        self.version = version
+        self.context = context or Context()
+        self.manifest = VersionManifest()
+        
+        # General options
+        self.demo: bool = False
+        self.auth_session: Optional[AuthSession] = None
+        self.resolution: Optional[Tuple[int, int]] = None
+        self.disable_multiplayer: bool = False
+        self.disable_chat: bool = False
+        self.quick_play: Optional[QuickPlay] = None
+        self.jvm_path: Optional[Path] = None
+        self.libraries_filters: List[Callable[[Dict[LibrarySpecifier, _Library]], None]] = []
+        self.fixes: Dict[str, Any] = { 
+            self.FIX_LEGACY_PROXY: True, 
+            self.FIX_LEGACY_MERGE_SORT: True,
+            self.FIX_LEGACY_RESOLUTION: True,
+            self.FIX_LEGACY_QUICK_PLAY: True,
+            self.FIX_AUTH_LIB_2_1_28: True,
+            self.FIX_LWJGL: None
+        }
 
+        # Resolved version metadata, root version and its hierarchy, and merged metadata
+        self._hierarchy: List[VersionHandle] = []
+        self._metadata: dict = {}
+
+        # Features used for rule resolution across the metadata
+        self._features: Dict[str, bool] = {}
+
+        # Path to the JAR file to run the game
+        self._jar_path: Optional[Path] = None
+
+        # Assets dictionary and index version, with optional legacy directories
+        self._assets_index_version: Optional[str] = None
+        self._assets: Dict[str, Path] = {}
+        self._assets_virtual_dir: Optional[Path] = None
+        self._assets_resources_dir: Optional[Path] = None
+
+        # Native and class libraries (using dict so we keep order)
+        self._libs: Dict[LibrarySpecifier, _Library] = {}
+        self._native_libs: List[Path] = []
+        self._class_libs: List[Path] = []
+
+        # Logger config parsed from metadata
+        self._logger_path: Optional[Path] = None
+        self._logger_arg: Optional[str] = None
+        
+        # JVM to use for launching the game
+        self._jvm_path: Optional[Path] = None
+        self._jvm_version: Optional[str] = None
+
+        self._dl = DownloadList()
+        self._applied_fixes: Dict[str, Any] = {}
+
+    def set_auth_offline(self, username: Optional[str], uuid: Optional[str]) -> None:
+        """Shortcut for setting an offline session with the given username/uuid pair.
         """
-        Prepare all metadata files for this version, this take `inheritsFrom` key into account and all parents metadata
-        files are downloaded. You can change the limit of parents metadata to download with the `recursion_limit`
-        argument, if the number of parents exceed this argument, a `VersionError` is raised with
-        `VersionError.TO_MUCH_PARENTS` and the version ID as argument. Each metadata file is downloaded (if not already
-        cached) in their own directory named after the version ID, the directory is placed in the `versions_dir` of the
-        context.\n
-        This method will load the official Mojang version manifest, however you can set the `manifest` attribute of this
-        object before with a custom manifest if you want to support more versions.\n
-        If any version in the `inheritsFrom` tree is not found, a `VersionError` is raised with `VersionError.NOT_FOUND`
-        and the version ID as argument.\n
-        Note that this method is authorized to change the version identifier through its internal method `_prepare_id`.\n
-        This method can raise `JsonRequestError` for any error for requests to JSON file.
-        """
-
-        self._prepare_id()
+        self.auth_session = OfflineAuthSession(username, uuid)
 
-        version_meta, version_dir = self._prepare_meta_internal(self.id)
-        while "inheritsFrom" in version_meta:
-            if recursion_limit <= 0:
-                raise VersionError(VersionError.TO_MUCH_PARENTS, self.id)
-            recursion_limit -= 1
-            parent_meta, _ = self._prepare_meta_internal(version_meta["inheritsFrom"])
-            del version_meta["inheritsFrom"]
-            merge_dict(version_meta, parent_meta)
+    def set_quick_play_singleplayer(self, level_name: str) -> None:
+        """Configure quick play for entering a singleplayer level after game's launch.
+        """
+        self.quick_play = QuickPlaySingleplayer(level_name)
+    
+    def set_quick_play_multiplayer(self, host: str, port: int = 25565) -> None:
+        """Configure quick play for connecting to a server after game's launch.
+        """
+        self.quick_play = QuickPlayMultiplayer(host, port)
+    
+    def set_quick_play_realms(self, realm: str) -> None:
+        """Configure quick play for connection to a realm after game's launch.
+        """
+        self.quick_play = QuickPlayRealms(realm)
 
-        self.version_meta, self.version_dir = version_meta, version_dir
+    def install(self, *, watcher: Optional[Watcher] = None) -> Environment:
+        """This function ensures that this version is properly installed given 
+        configuration of this class' attributes. This function can be called multiple
+        time and will not recompute what have already been done, if errors happen, the
+        install can be resumed and the failed steps will be retried.
+        """
+
+        watcher = watcher or Watcher()
+
+        self._dl.clear()
+        self._applied_fixes.clear()
+
+        self._resolve_version(watcher)
+        self._resolve_metadata(watcher)
+        self._resolve_features(watcher)
+        self._resolve_jvm(watcher)  # JVM added here on purpose to ease implementation of ForgeVersion
+        self._resolve_jar(watcher)
+        self._resolve_assets(watcher)
+        self._resolve_libraries(watcher)
+        self._resolve_logger(watcher)
+        self._download(watcher)
+        self._finalize_assets(watcher)
 
-    def _prepare_id(self):
+        return self._resolve_env(watcher)
+    
+    def _resolve_version(self, watcher: Watcher) -> None:
+        """This step is executed just before resolving version metadata and its parents,
+        it should process the version and ensure that the version is relevant for the
+        metadata resolving.
 
+        The default implementation resolve aliases (release, snapshot) if needed.
         """
-        Internal method to modify the version's identifier (`id` attribute), this is called before
-        fetching version metadata. This method doesn't change the identifier by default.
+        self.version = self.manifest.filter_latest(self.version)[0]
+
+    def _resolve_metadata(self, watcher: Watcher) -> None:
+        """This step resolves metadata of the root version and all of its parents.
         """
 
-    def _prepare_meta_internal(self, version_id: str) -> Tuple[dict, str]:
+        hierarchy = self._hierarchy
+        version: Optional[str] = self.version
+        hierarchy.clear()
 
-        """
-        An internal method to ensure an up-to-date version metadata together with its directory.
-        """
+        while version is not None:
 
-        version_dir = self.context.get_version_dir(version_id)
-        version_meta_file = path.join(version_dir, f"{version_id}.json")
+            if len(hierarchy) > 10:
+                raise TooMuchParentsError(hierarchy)
+            
+            watcher.handle(VersionLoadingEvent(version))
 
-        try:
-            with open(version_meta_file, "rt") as version_meta_fp:
-                version_meta = json.load(version_meta_fp)
-        except (OSError, JSONDecodeError):
-            version_meta = None
+            # Get version instance and load/fetch is needed.
+            handle = self.context.get_version(version)
+            if not self._load_version(handle, watcher):
+                watcher.handle(VersionFetchingEvent(version))
+                self._fetch_version(handle, watcher)
+            
+            watcher.handle(VersionLoadedEvent(version))
 
-        if version_meta is not None:
-            if self._validate_version_meta(version_id, version_dir, version_meta_file, version_meta):
-                return version_meta, version_dir
-            else:
-                version_meta = None
+            # Set the parent of the last version to the version being resolved.
+            if len(hierarchy):
+                hierarchy[-1].parent = handle
+            
+            hierarchy.append(handle)
+            version = handle.metadata.pop("inheritsFrom", None)
+            
+            if version is not None and not isinstance(version, str):
+                raise ValueError("metadata: /inheritsFrom must be a string")
 
-        if version_meta is None:
-            try:
-                version_meta = self._fetch_version_meta(version_id, version_dir, version_meta_file)
-                if "_pmc_no_dump" not in version_meta:
-                    os.makedirs(version_dir, exist_ok=True)
-                    with open(version_meta_file, "wt") as version_meta_fp:
-                        json.dump(version_meta, version_meta_fp, indent=2)
-            except NotADirectoryError:
-                raise VersionError(VersionError.INVALID_ID, version_id)
+        self._metadata = hierarchy[0].merge()
 
-        return version_meta, version_dir
+    def _load_version(self, version: VersionHandle, watcher: Watcher) -> bool:
+        """This function is responsible for loading a version's metadata. Note that 
+        implementations are free to load other things beside metadata.
 
-    def _validate_version_meta(self, version_id: str, version_dir: str, version_meta_file: str, version_meta: dict) -> bool:
+        This function returns true if loading was successful, if this function returns
+        false, the `fetch_version` function is then called to fetch the version. This can
+        be used to check integrity of a version.
 
-        """
-        An internal method to check if a version's metadata is up-to-date, returns `True` if it is.
-        If `False`, the version metadata is re-fetched, this is the default when version metadata
-        doesn't exist.
+        De default implementation of this function just read metadata file and return 
+        true if successful.
 
-        The default implementation check official versions againt the expected SHA1 hash of the metadata
-        file.
+        :param version: The version metadata to validate or not.
+        :param state: Sequence state when the MetadataTask execute.
+        :return: True if the given version is valid and its metadata was properly loaded.
         """
 
-        version_super_meta = self._ensure_version_manifest().get_version(version_id)
+        if not version.read_metadata_file():
+            return False
+
+        try:
+            version_super_meta = self.manifest.get_version(version.id)
+        except HttpError:
+            # Silently ignoring HTTP errors, we want to be able to launch offline.
+            return True
+        
         if version_super_meta is None:
             return True
         else:
             expected_sha1 = version_super_meta.get("sha1")
             if expected_sha1 is not None:
                 try:
-                    with open(version_meta_file, "rb") as version_meta_fp:
+                    with version.metadata_file().open("rb") as version_meta_fp:
                         current_sha1 = calc_input_sha1(version_meta_fp)
                         return expected_sha1 == current_sha1
                 except OSError:
                     return False
             return True
 
-    def _fetch_version_meta(self, version_id: str, version_dir: str, version_meta_file: str) -> dict:
+    def _fetch_version(self, version: VersionHandle, watcher: Watcher) -> None:
+        """Fetch the data of the given version.
 
-        """
-        An internal method to fetch a version metadata. The returned dict can contain an optional
-        key '_pmc_no_dump' that prevent dumping the dictionary as JSON to the metadata file.
+        The default implementation try to fetch version from Mojang's version manifest.
 
-        The default implementation fetch from official versions, and directly write the read data
-        to the meta file in order to keep the exact same SHA1 hash of the metadata. The default
-        implementation also set the `_pmc_no_dump` flag to the returned data in order to avoid
-        overwriting the file.
+        :param version: The version meta to fetch data into.
+        :param state: Sequence state when the MetadataTask execute.
+        :raises VersionNotFoundError: In case of error finding the version.
         """
 
-        version_super_meta = self._ensure_version_manifest().get_version(version_id)
+        version_super_meta = self.manifest.get_version(version.id)
         if version_super_meta is None:
-            raise VersionError(VersionError.NOT_FOUND, version_id)
-        code, raw_data = http_request(version_super_meta["url"], "GET")
-        if code != 200:
-            raise VersionError(VersionError.NOT_FOUND, version_id)
-        os.makedirs(version_dir, exist_ok=True)
-        with open(version_meta_file, "wb") as fp:
-            fp.write(raw_data)
-        try:
-            data = json.loads(raw_data)
-            data["_pmc_no_dump"] = True
-            return data
-        except JSONDecodeError:
-            raise VersionError(VersionError.NOT_FOUND, version_id)
-
-    def prepare_jar(self):
-
-        """
-        Must be called once metadata file are prepared, using `prepare_meta`, if not, `ValueError` is raised.\n
-        If the metadata provides a client download URL, and the version JAR file doesn't exists or have not the expected
-        size, it's added to the download list to be downloaded to the same directory as the metadata file.\n
-        If no download URL is provided by metadata and the JAR file does not exists, a VersionError is raised with
-        `VersionError.JAR_NOT_FOUND` and the version ID as argument.
-        """
-
-        # FIXME: The official launcher seems to use the JAR of inherited versions instead of re-downloading
-        #  the same JAR for this specific version. It's not critical but it could be changed.
-
-        self._check_version_meta()
-        self.version_jar_file = path.join(self.version_dir, f"{self.id}.jar")
-        client_download = self.version_meta.get("downloads", {}).get("client")
-        if client_download is not None:
-            entry = DownloadEntry.from_meta(client_download, self.version_jar_file, name=f"{self.id}.jar")
-            if not path.isfile(entry.dst) or path.getsize(entry.dst) != entry.size:
-                self.dl.append(entry)
-        elif not path.isfile(self.version_jar_file):
-            raise VersionError(VersionError.JAR_NOT_FOUND, self.id)
+            raise VersionNotFoundError(version.id)
 
-    def prepare_assets(self):
-
-        """
-        Must be called once metadata file are prepared, using `prepare_meta`, if not, `ValueError` is raised.\n
-        This method download the asset index file (if not already cached) named after the asset version into the
-        directory `indexes` placed into the directory `assets_dir` of the context. Once ready, the asset index file
-        is analyzed and each object is checked, if it does not exist or not have the expected size, it is downloaded
-        to the `objects` directory placed into the directory `assets_dir` of the context.\n
-        If the metadata doesn't provide an `assetIndex`, the process is skipped.\n
-        This method also set the `assets_count` attribute with the number of assets for this version.\n
-        This method can raise `JsonRequestError` if it fails to load the asset index file.
-        """
-
-        self._check_version_meta()
-
-        assets_indexes_dir = path.join(self.context.assets_dir, "indexes")
-        asset_index_info = self.version_meta.get("assetIndex")
-        if asset_index_info is None:
+        res = http_request("GET", version_super_meta["url"], accept="application/json")
+        
+        # First decode the data and set it to the version meta. Raising if invalid.
+        version.metadata = res.json()
+        
+        # If successful, write the raw data directly to the file.
+        version.dir.mkdir(parents=True, exist_ok=True)
+        with version.metadata_file().open("wb") as fp:
+            fp.write(res.data)
+
+    def _resolve_features(self, watcher: Watcher) -> None:
+        """Step resolving the version's features, whose are a mapping of string to 
+        boolean, indicating if such feature is enabled or not. This is later used 
+        to compute rules when needed.
+        """
+
+        self._features["is_demo_user"] = self.demo
+        self._features["has_custom_resolution"] = self.resolution is not None
+        if self.quick_play is not None:
+            self._features[self.quick_play.feature] = True
+        
+        watcher.handle(FeaturesEvent([feature for feature, enabled in self._features.items() if enabled]))
+
+    def _resolve_jar(self, watcher: Watcher) -> None:
+        """This step resolves the JAR file to use for launcher the game.
+        """
+
+        self._jar_path = self._hierarchy[0].jar_file()
+
+        # First try to find a /downloads/client download entry.
+        version_dls = self._metadata.get("downloads")
+        if version_dls is not None:
+
+            if not isinstance(version_dls, dict):
+                raise ValueError("metadata: /downloads must be an object")
+            
+            client_dl = version_dls.get("client")
+            if client_dl is not None:
+                self._dl.add(parse_download_entry(client_dl, self._jar_path, "metadata: /downloads/client"), verify=True)
+                watcher.handle(JarFoundEvent())
+                return
+        
+        # If no download entry has been found, but the JAR exists, we use it.
+        if self._jar_path.is_file():
+            watcher.handle(JarFoundEvent())
             return
-
-        assets_index_version = self.version_meta.get("assets", asset_index_info.get("id", None))
+        
+        self._jar_path = None
+        raise JarNotFoundError()
+
+    def _resolve_assets(self, watcher: Watcher) -> None:
+        """This step resolve assets from metadata and add missing entries to the download
+        list for future download.
+        """
+
+        metadata = self._metadata
+        context = self.context
+
+        assets_index_info = metadata.get("assetIndex")
+        if assets_index_info is None:
+            # Asset info may not be present, it's not required because some custom 
+            # versions may want to use there own internal assets.
+            return
+        
+        if not isinstance(assets_index_info, dict):
+            raise ValueError("metadata: /assetIndex must be an object")
+        
+        assets_index_version = metadata.get("assets", assets_index_info.get("id"))
         if assets_index_version is None:
+            # Same as above.
             return
+        
+        if not isinstance(assets_index_version, str):
+            raise ValueError("metadata: /assets or /assetIndex/id must be a string")
+        
+        watcher.handle(AssetsResolveEvent(assets_index_version, None))
 
-        assets_index_file = path.join(assets_indexes_dir, f"{assets_index_version}.json")
+        assets_indexes_dir = context.assets_dir / "indexes"
+        assets_index_file = assets_indexes_dir / f"{assets_index_version}.json"
 
         try:
-            with open(assets_index_file, "rb") as assets_index_fp:
+            with assets_index_file.open("rb") as assets_index_fp:
                 assets_index = json.load(assets_index_fp)
         except (OSError, JSONDecodeError):
-            asset_index_url = asset_index_info["url"]
-            assets_index = json_simple_request(asset_index_url)
-            os.makedirs(assets_indexes_dir, exist_ok=True)
-            with open(assets_index_file, "wt") as assets_index_fp:
+
+            # If for some reason we can't read an assets index, try downloading it.
+            assets_index_url = assets_index_info.get("url")
+            if not isinstance(assets_index_url, str):
+                raise ValueError("metadata: /assetIndex/url must be a string")
+            
+            assets_index = http_request("GET", assets_index_url, accept="application/json").json()
+            assets_indexes_dir.mkdir(parents=True, exist_ok=True)
+            with assets_index_file.open("wt") as assets_index_fp:
                 json.dump(assets_index, assets_index_fp)
 
-        assets_objects_dir = path.join(self.context.assets_dir, "objects")
-        assets_virtual_dir = path.join(self.context.assets_dir, "virtual", assets_index_version)
-        assets_mapped_to_resources = assets_index.get("map_to_resources", False)  # For version <= 13w23b
+        assets_objects_dir = context.assets_dir / "objects"
+        assets_resources = assets_index.get("map_to_resources", False)  # For version <= 13w23b
         assets_virtual = assets_index.get("virtual", False)  # For 13w23b < version <= 13w48b (1.7.2)
 
-        assets = {}
+        if not isinstance(assets_resources, bool):
+            raise ValueError("assets index: /map_to_resources must be a boolean")
+        if not isinstance(assets_virtual, bool):
+            raise ValueError("assets index: /virtual must be a boolean")
+
+        assets_objects = assets_index.get("objects")
+        if not isinstance(assets_objects, dict):
+            raise ValueError("assets index: /objects must be an object")
+
+        for asset_id, asset_obj in assets_objects.items():
+
+            if not isinstance(asset_obj, dict):
+                raise ValueError(f"assets index: /objects/{asset_id} must be an object")
+
+            asset_hash = asset_obj.get("hash")
+            if not isinstance(asset_hash, str):
+                raise ValueError(f"assets index: /objects/{asset_id}/hash must be a string")
+            
+            asset_size = asset_obj.get("size")
+            if not isinstance(asset_size, int):
+                raise ValueError(f"assets index: /objects/{asset_id}/size must be an integer")
 
-        for asset_id, asset_obj in assets_index["objects"].items():
-            asset_hash = asset_obj["hash"]
             asset_hash_prefix = asset_hash[:2]
-            asset_size = asset_obj["size"]
-            asset_file = path.join(assets_objects_dir, asset_hash_prefix, asset_hash)
-            assets[asset_id] = asset_file
-            if not path.isfile(asset_file) or path.getsize(asset_file) != asset_size:
-                asset_url = f"{RESOURCES_URL}{asset_hash_prefix}/{asset_hash}"
-                self.dl.append(DownloadEntry(asset_url, asset_file, size=asset_size, sha1=asset_hash, name=asset_id))
-
-        def finalize():
-            if assets_mapped_to_resources or assets_virtual:
-                for asset_id_to_copy, asset_file_to_copy in assets.items():
-                    if assets_mapped_to_resources:
-                        resources_asset_file = path.join(self.context.work_dir, "resources", asset_id_to_copy)
-                        if not path.isfile(resources_asset_file):
-                            os.makedirs(path.dirname(resources_asset_file), exist_ok=True)
-                            shutil.copyfile(asset_file_to_copy, resources_asset_file)
-                    if assets_virtual:
-                        virtual_asset_file = path.join(assets_virtual_dir, asset_id_to_copy)
-                        if not path.isfile(virtual_asset_file):
-                            os.makedirs(path.dirname(virtual_asset_file), exist_ok=True)
-                            shutil.copyfile(asset_file_to_copy, virtual_asset_file)
-
-        self.dl.add_callback(finalize)
-        self.assets_index_version = assets_index_version
-        self.assets_virtual_dir = assets_virtual_dir
-        self.assets_count = len(assets_index["objects"])
-
-    def prepare_logger(self):
-
-        """
-        Must be called once metadata file are prepared, using `prepare_meta`, if not, `ValueError` is raised.\n
-        This method check the metadata for a client logging configuration, it it doesn't exist the configuration is
-        added to the download list.
-        """
-
-        self._check_version_meta()
-        client_logging = self.version_meta.get("logging", {}).get("client")
-        if client_logging is not None:
-            logging_file_info = client_logging["file"]
-            logging_file = path.join(self.context.assets_dir, "log_configs", logging_file_info["id"])
-            download_entry = DownloadEntry.from_meta(logging_file_info, logging_file, name=logging_file_info["id"])
-            if not path.isfile(logging_file) or path.getsize(logging_file) != download_entry.size:
-                self.dl.append(download_entry)
-            self.logging_file = logging_file
-            self.logging_argument = client_logging["argument"]
-
-    def prepare_libraries(self, *, predicate: "Optional[Callable[[LibrarySpecifier], bool]]" = None):
-
-        """
-        Must be called once metadata file are prepared, using `prepare_meta`, if not, `ValueError` is raised.\n
-        If the version JAR file is not set, a ValueError is raised because it is required to be added in classpath.\n
-        This method check all libraries found in the metadata, each library is downloaded if not already stored. Real
-        Java libraries are added to the classpath list and native libraries are added to the native list.\n
-        Optional predicate can be used to filter libraries to download and include to the classpath.
-        """
-
-        self._check_version_meta()
-
-        if self.version_jar_file is None:
-            raise ValueError("The version JAR file must be prepared before calling this method.")
+            asset_file = assets_objects_dir.joinpath(asset_hash_prefix, asset_hash)
 
-        self.classpath_libs.clear()
-        self.native_libs.clear()
+            asset_url = f"{RESOURCES_URL}{asset_hash_prefix}/{asset_hash}"
+            self._assets[asset_id] = asset_file
+            self._dl.add(DownloadEntry(asset_url, asset_file, size=asset_size, sha1=asset_hash, name=asset_id), verify=True)
+        
+        self._assets_index_version = assets_index_version
+        self._assets_virtual_dir = context.assets_dir.joinpath("virtual", assets_index_version) if assets_virtual else None
+        self._assets_resources_dir = context.work_dir / "resources" if assets_resources else None
+
+        watcher.handle(AssetsResolveEvent(assets_index_version, len(self._assets)))
+
+    def _finalize_assets(self, watcher: Watcher) -> None:
+        """Step called after download to finalize installation of assets when 
+        """
+
+        if self._assets_resources_dir is not None:
+            for asset_id, asset_file in self._assets.items():
+                dst_file = self._assets_resources_dir / asset_id
+                dst_file.parent.mkdir(parents=True, exist_ok=True)
+                shutil.copyfile(str(asset_file), str(dst_file))
+
+        if self._assets_virtual_dir is not None:
+            for asset_id, asset_file in self._assets.items():
+                dst_file = self._assets_virtual_dir / asset_id
+                dst_file.parent.mkdir(parents=True, exist_ok=True)
+                shutil.copyfile(str(asset_file), str(dst_file))
+
+    def _resolve_libraries(self, watcher: Watcher) -> None:
+        """Step resolving libraries from version's metadata. 
+        
+        **Note that this is the most critical step and libraries resolving is really 
+        important for running the game.**
+        
+        *This step has to support both older format where native libraries were given
+        appart from regular class path libraries, all of this should also support 
+        automatic downloading both from an explicit artifact URL, or with a maven repo
+        URL.*
+        """
+
+        watcher.handle(LibrariesResolvingEvent())
+
+        # Recursion order is important for libraries resolving, root libraries should
+        # be placed first.
+        for version in self._hierarchy[0].recurse():
 
-        for lib_obj in self.version_meta["libraries"]:
+            metadata_libraries = version.metadata.get("libraries")
+            if metadata_libraries is None:
+                continue
 
-            if "rules" in lib_obj:
-                if not interpret_rule(lib_obj["rules"]):
-                    continue
+            if not isinstance(metadata_libraries, list):
+                raise ValueError("metadata: /libraries must be a list")
 
-            lib_spec = LibrarySpecifier.from_str(lib_obj["name"])
+            for library_idx, library in enumerate(metadata_libraries):
 
-            # FIXME: Maybe we should test for this after the natives condition.
-            if predicate is not None:
-                if not predicate(lib_spec):
-                    continue
+                if not isinstance(library, dict):
+                    raise ValueError(f"metadata: /libraries/{library_idx} must be an object")
+                
+                name = library.get("name")
+                if not isinstance(name, str):
+                    raise ValueError(f"metadata: /libraries/{library_idx}/name must be a string")
+                
+                spec = LibrarySpecifier.from_str(name)
 
-            # Old metadata files provides a 'natives' mapping from OS to the
-            # classifier specific for this OS.
-            lib_natives: Optional[dict] = lib_obj.get("natives")
-
-            if lib_natives is not None:
-                # If natives object is present, the classifier associated to the
-                # OS overrides the lib_spec classifier.
-                lib_spec.classifier = lib_natives.get(get_minecraft_os())
-                if lib_spec.classifier is None:
-                    continue
-                archbits = get_minecraft_archbits()
-                if len(archbits):
-                    lib_spec.classifier = lib_spec.classifier.replace("${arch}", archbits)
-                lib_libs = self.native_libs
-            else:
-                lib_libs = self.classpath_libs
+                rules = library.get("rules")
+                if rules is not None:
 
-            lib_path: Optional[str] = None
-            lib_dl_entry: Optional[DownloadEntry] = None
-            lib_dl: Optional[dict] = lib_obj.get("downloads")
-
-            if lib_dl is not None:
-
-                if lib_natives is not None:
-                    # Only check classifiers if natives mapping is present.
-                    lib_dl_classifiers = lib_dl.get("classifiers")
-                    lib_dl_meta = None if lib_dl_classifiers is None else lib_dl_classifiers.get(lib_spec.classifier)
-                else:
-                    # If we are not dealing with natives, just take the artifact.
-                    lib_dl_meta = lib_dl.get("artifact")
+                    if not isinstance(rules, list):
+                        raise ValueError(f"metadata: /libraries/{library_idx}/rules must be a list")
+                    
+                    if not interpret_rule(rules, self._features, f"metadata: /libraries/{library_idx}/rules"):
+                        continue
 
-                # If some download metadata was found, we try to create an entry from it.
-                if lib_dl_meta is not None:
+                # Old metadata files provides a 'natives' mapping from OS to the classifier
+                # specific for this OS, this kind of libs are "native libs", we need to
+                # extract their dynamic libs into the "bin" directory before running.
+                natives = library.get("natives")
+                if natives is not None:
 
-                    lib_dl_path = lib_dl_meta.get("path")
+                    if not isinstance(natives, dict):
+                        raise ValueError(f"metadata: /libraries/{library_idx}/natives must be an object")
+                    
+                    # If natives object is present, the classifier associated to the
+                    # OS overrides the lib_spec classifier.
+                    spec.classifier = natives.get(minecraft_os)
+                    if spec.classifier is None:
+                        continue
 
-                    # It sometime happens that no download path is provided.
-                    if lib_dl_path is None:
+                    if minecraft_arch_bits is not None:
+                        spec.classifier = spec.classifier.replace("${arch}", str(minecraft_arch_bits))
 
-                        # In such case, we can guess the path from the URL (error if not present).
-                        lib_dl_url = lib_dl_meta.get("url")
-                        if lib_dl_url is None:
-                            raise ValueError("None of 'url' or 'path' fields are present in the download metadata.", lib_spec)
-                        
-                        # For now, we only guess the path if the url is the official repository.
-                        if lib_dl_url.startswith(LIBRARIES_URL):
-                            lib_dl_path = lib_dl_url[len(LIBRARIES_URL):]
-                        else:
-                            # FIXME: In the future, support urls that are not from official repository.
-                            raise ValueError("The path can only be guess from the official repository.", lib_spec)
-                    
-                    # Here the path should not be none, because of raised errors.
-                    lib_path = path.join(self.context.libraries_dir, lib_dl_path)
-                    lib_dl_entry = DownloadEntry.from_meta(lib_dl_meta, lib_path, name=str(lib_spec))
-
-            # If we don't have a download entry, try to make one of the library specifier (only if version is set).
-            if lib_dl_entry is None:
-                lib_path_raw = lib_spec.jar_file_path()
-                lib_path = path.join(self.context.libraries_dir, lib_path_raw)
-                if not path.isfile(lib_path):
-                    # The official launcher seems to default to their repository, it will also allows us
-                    # to prevent launch if such lib cannot be found.
-                    lib_repo_url: str = lib_obj.get("url", LIBRARIES_URL)
-                    if lib_repo_url[-1] != "/":
-                        lib_repo_url += "/"  # Let's be sure to have a '/' as last character.
-                    lib_dl_entry = DownloadEntry(f"{lib_repo_url}{lib_path_raw}", lib_path, name=str(lib_spec))
-
-            # Even if no download entry has been found, we add the path because it might be already downloaded.
-            lib_libs.append(lib_path)
-
-            if lib_dl_entry is not None:
-                if not path.isfile(lib_path) or (lib_dl_entry.size is not None and path.getsize(lib_path) != lib_dl_entry.size):
-                    self.dl.append(lib_dl_entry)
+                lib_entry: Optional[DownloadEntry] = None
                 
-        self.classpath_libs.append(self.version_jar_file)
+                # Avoids ready downloading if a fix is being used, in such case we'll use
+                # the Mojang's libraries.
+                downloads = library.get("downloads")
+                if downloads is not None:
+
+                    if not isinstance(downloads, dict):
+                        raise ValueError(f"metadata: /libraries/{library_idx}/downloads must be an object")
+
+                    if natives is not None:
+                        # Only check classifiers if natives mapping is present.
+                        lib_dl_classifiers = downloads.get("classifiers")
+                        dl_meta = None if lib_dl_classifiers is None else lib_dl_classifiers.get(spec.classifier)
+                    else:
+                        # If we are not dealing with natives, just take the artifact.
+                        dl_meta = downloads.get("artifact")
+
+                    if dl_meta is not None:
+                        # lib_path = self.context.libraries_dir / spec.file_path()
+                        lib_entry = parse_download_entry(dl_meta, Path(), f"metadata: /libraries/{library_idx}/downloads/artifact")
+
+                # If no download entry can be found, try to find the maven repository url.
+                if lib_entry is None:
+                    repo_url = library.get("url")
+                    if repo_url is not None:
 
-    def prepare_jvm(self):
+                        if not isinstance(repo_url, str):
+                            raise ValueError(f"metadata: /libraries/{library_idx}/url must be a string")
+                        
+                        # Let's be sure to have a '/' as last character.
+                        if repo_url[-1] != "/":
+                            repo_url += "/"
+                        
+                        lib_path_rel = spec.file_path()
+                        # lib_path = self.context.libraries_dir / lib_path_rel
+                        lib_entry = DownloadEntry(f"{repo_url}{lib_path_rel}", Path())
+
+                # Adding parsed library.
+                # Insertion ordering is guaranteed on dictionaries since python 3.6
+                self._libs[spec] = _Library(natives is not None, lib_entry)
+
+        # Fix libraries before computation
+        self._filter_libraries(watcher)
+
+        # Apply custom libs filters after builtin filters.
+        for libs_filter in self.libraries_filters:
+            libs_filter(self._libs)
+
+        # Finally take the final version of libs and add them to download list.
+        self._native_libs.clear()
+        self._class_libs.clear()
+        for spec, parsed_lib in self._libs.items():
+
+            lib_path = self.context.libraries_dir / spec.file_path()
+            lib_entry = parsed_lib.entry
+
+            # If no repository URL is given, no more download method is available,
+            # so if the JAR file isn't installed, the game cannot be launched.
+            # 
+            # Note: In the past, we used to default the url to Mojang's maven 
+            # repository, but this was a bad habit because most libraries could
+            # not be downloaded from their repository, and this was confusing to
+            # get a download error for such libraries.
+            if lib_entry is None or not len(lib_entry.url):
+                if not lib_path.is_file():
+                    raise LibraryNotFoundError(spec)
+            else:
+                lib_entry.dst = lib_path
+                lib_entry.name = str(spec)
+                self._dl.add(lib_entry, verify=True)
+            
+            # Finally, add it to the correct libs list.
+            libs = self._native_libs if parsed_lib.native else self._class_libs
+            libs.append(lib_path)
+
+        watcher.handle(LibrariesResolvedEvent(len(self._class_libs), len(self._native_libs)))
+
+    def _filter_libraries(self, watcher: Watcher) -> None:
+        """This step should fix libraries and customize the `_libs` list before actually
+        registering them for download or check availability. The default implementation is
+        used for fixing authlib on 1.16.4 and 1.16.5 and LWJGL fixing.
+        """
+
+        # Versions 1.16.4 and 1.16.5 uses authlib:2.1.28 which cause multiplayer button
+        # (and probably in-game chat) to be disabled, this can be fixed by switching to
+        # version 2.2.30
+        if self.fixes.get(self.FIX_AUTH_LIB_2_1_28):
+            spec = LibrarySpecifier("com.mojang", "authlib", "2.1.28")
+            lib = self._libs.pop(spec, None)
+            if lib is not None:
+                spec.version = "2.2.30"
+                if lib.entry is not None:
+                    lib.entry.url = f"{LIBRARIES_URL}com/mojang/authlib/2.2.30/authlib-2.2.30.jar"
+                    lib.entry.sha1 = "d6e677199aa6b19c4a9a2e725034149eb3e746f8"
+                    lib.entry.size = 87497
+                self._applied_fixes[self.FIX_AUTH_LIB_2_1_28] = True
+                self._libs[spec] = lib
+        
+        # Fixing LWJGL, this can be useful on ARM devices because Mojang doesn't provide
+        # natives for this architecture.
+        lwjgl_version = self.fixes.get(self.FIX_LWJGL)
+        if lwjgl_version is not None:
+
+            # Check that we support this LWJGL version.
+            if lwjgl_version not in ("3.2.3", "3.3.0", "3.3.1", "3.3.2"):
+                raise ValueError(f"unsupported lwjgl fix version: {lwjgl_version}")
+
+            # Compute natives required for the specific version
+            lwjgl_natives_map: Dict[Optional[str], Dict[Optional[str], str]] = {
+                "windows": {"x86_64": "natives-windows", "x86": "natives-windows-x86"},
+                "linux": {"x86_64": "natives-linux", "x86": "natives-linux", "arm64": "natives-linux-arm64", "arm32": "natives-linux-arm32"},
+                "osx": {"x86_64": "natives-macos"}
+            }
+
+            if lwjgl_version in ("3.3.0", "3.3.1", "3.3.2"):
+                lwjgl_natives_map["windows"]["arm64"] = "natives-windows-arm64"
+                lwjgl_natives_map["osx"]["arm64"] = "natives-macos-arm64"
+
+            # Get natives and error if no natives for current os/arch
+            lwjgl_natives = lwjgl_natives_map.get(minecraft_os, {}).get(minecraft_arch)
+            if lwjgl_natives is None:
+                raise ValueError(f"unsupported lwjgl fix version for your os/arch")
+
+            # Remove all LWJGL libs.
+            for to_remove in list(filter(lambda l: l.group == "org.lwjgl", self._libs.keys())):
+                del self._libs[to_remove]
+            
+            def add_lwjgl_lib(name: str) -> None:
+                for classifier in (None, lwjgl_natives):
+                    spec = LibrarySpecifier("org.lwjgl", name, lwjgl_version, classifier)
+                    entry = DownloadEntry(f"https://repo1.maven.org/maven2/{spec.file_path()}", Path())
+                    lib = _Library(False, entry)
+                    self._libs[spec] = lib
+
+            add_lwjgl_lib("lwjgl")
+            add_lwjgl_lib("lwjgl-jemalloc")
+            add_lwjgl_lib("lwjgl-openal")
+            add_lwjgl_lib("lwjgl-opengl")
+            add_lwjgl_lib("lwjgl-glfw")
+            add_lwjgl_lib("lwjgl-stb")
+            add_lwjgl_lib("lwjgl-tinyfd")
 
-        """
-        Must be called once metadata file are prepared, using `prepare_meta`, if not, `ValueError` is raised.\n
-        This method ensure that the JVM adapted to this version is downloaded to the `jvm_dir` of the context.\n
-        This method can raise `JvmLoadingError` with `JvmLoadingError.UNSUPPORTED_ARCH` if Mojang does not provide
-        a JVM for your current architecture, or `JvmLoadingError.UNSUPPORTED_VERSION` if the required JVM version is
-        not provided by Mojang. It can also raise `JsonRequestError` when failing to get JSON files.\n
-        The error `JvmLoadingError.UNSUPPORTED_LIBC` can also be raised on non-glibc systems, because Mojang only
-        provides JVM linked to glibc.
+            self._applied_fixes[self.FIX_LWJGL] = lwjgl_version
+
+    def _resolve_logger(self, watcher: Watcher) -> None:
+        """This step resolve the logger to use for launcher the game.
         """
 
-        self._check_version_meta()
+        logging = self._metadata.get("logging")
+        if logging is None:
+            return
+        
+        if not isinstance(logging, dict):
+            raise ValueError("metadata: /logging must be an object")
+        
+        client_logging = logging.get("client")
+        if client_logging is None:
+            return
+        
+        if not isinstance(client_logging, dict):
+            raise ValueError("metadata: /logging/client must be an object")
+        
+        argument = client_logging.get("argument")
+        if not isinstance(argument, str):
+            raise ValueError("metadata: /logging/client/argument must be a string")
+
+        file_info = client_logging.get("file")
+        if not isinstance(file_info, dict):
+            raise ValueError("metadata: /logging/client/file must be an object")
+        
+        file_id = file_info.get("id")
+        if not isinstance(file_id, str):
+            raise ValueError("metadata: /logging/client/file/id must be a string")
+
+        self._logger_arg = argument
+        self._logger_path = self.context.assets_dir / "log_configs" / file_id
+        dl_entry = parse_download_entry(file_info, self._logger_path, "metadata: /logging/client/file")
+        self._dl.add(dl_entry, verify=True)
+
+        watcher.handle(LoggerFoundEvent(file_id.replace(".xml", "")))
+
+    def _resolve_jvm(self, watcher: Watcher) -> None:
+        """Step resolving a JVM suitable for running the game.
+        """
+
+        watcher.handle(JvmLoadingEvent())
+
+        # Don't do anything if JVM is already provided.
+        if self.jvm_path is not None:
+            self._jvm_path = self.jvm_path
+            self._jvm_version = None
+            watcher.handle(JvmLoadedEvent(self._jvm_version, JvmLoadedEvent.CUSTOM))
+            return
+        
+        jvm_version_info = self._metadata.get("javaVersion", {})
+        if not isinstance(jvm_version_info, dict):
+            raise ValueError("metadata: /javaVersion must be a string")
+
+        jvm_major_version = jvm_version_info.get("majorVersion")
+        if jvm_major_version is not None and not isinstance(jvm_major_version, int):
+            raise ValueError("metadata: /javaVersion/majorVersion must be an integer")
 
         if platform.system() == "Linux" and platform.libc_ver()[0] != "glibc":
-            raise JvmLoadingError(JvmLoadingError.UNSUPPORTED_LIBC)
+            return self._resolve_builtin_jvm(watcher, JvmNotFoundError.UNSUPPORTED_LIBC, jvm_major_version)
 
-        jvm_version_type = self.version_meta.get("javaVersion", {}).get("component", "jre-legacy")
+        jvm_version_type = jvm_version_info.get("component", "jre-legacy")
+        if not isinstance(jvm_version_type, str):
+            raise ValueError("metadata: /javaVersion/component must be a string")
 
-        jvm_dir = path.join(self.context.jvm_dir, jvm_version_type)
-        jvm_manifest_file = path.join(self.context.jvm_dir, f"{jvm_version_type}.json")
+        jvm_dir = self.context.jvm_dir / jvm_version_type
+        jvm_manifest_file = self.context.jvm_dir / f"{jvm_version_type}.json"
 
         try:
-            with open(jvm_manifest_file, "rt") as jvm_manifest_fp:
+            with jvm_manifest_file.open("rt") as jvm_manifest_fp:
                 jvm_manifest = json.load(jvm_manifest_fp)
         except (OSError, JSONDecodeError):
 
-            all_jvm_meta = json_simple_request(JVM_META_URL)
-            jvm_arch_meta = all_jvm_meta.get(get_minecraft_jvm_os())
-            if jvm_arch_meta is None:
-                raise JvmLoadingError(JvmLoadingError.UNSUPPORTED_ARCH)
+            all_jvm_meta = http_request("GET", JVM_META_URL, accept="application/json").json()
+            if not isinstance(all_jvm_meta, dict):
+                raise ValueError("jvm metadata: / must be an object")
+            
+            jvm_arch_meta = all_jvm_meta.get(minecraft_jvm_os)
+            if not isinstance(jvm_arch_meta, dict):
+                return self._resolve_builtin_jvm(watcher, JvmNotFoundError.UNSUPPORTED_ARCH, jvm_major_version)
 
             jvm_meta = jvm_arch_meta.get(jvm_version_type)
-            if jvm_meta is None:
-                raise JvmLoadingError(JvmLoadingError.UNSUPPORTED_VERSION)
-
-            jvm_manifest = json_simple_request(jvm_meta[0]["manifest"]["url"])
-            jvm_manifest["version"] = jvm_meta[0]["version"]["name"]
+            if not isinstance(jvm_meta, list) or not len(jvm_meta):
+                return self._resolve_builtin_jvm(watcher, JvmNotFoundError.UNSUPPORTED_VERSION, jvm_major_version)
 
-            os.makedirs(self.context.jvm_dir, exist_ok=True)
-            with open(jvm_manifest_file, "wt") as jvm_manifest_fp:
-                json.dump(jvm_manifest, jvm_manifest_fp, indent=2)
-
-        jvm_files = jvm_manifest["files"]
-        self.jvm_exec = path.join(jvm_dir, "bin", get_jvm_bin_filename())
-        self.jvm_version = jvm_manifest.get("version", "unknown")
+            jvm_meta_manifest = jvm_meta[0].get("manifest")
+            if not isinstance(jvm_meta_manifest, dict):
+                raise ValueError(f"jvm metadata: /{minecraft_jvm_os}/{jvm_version_type}/0/manifest must be an object")
+            
+            jvm_meta_manifest_url = jvm_meta_manifest.get("url")
+            if not isinstance(jvm_meta_manifest_url, str):
+                raise ValueError(f"jvm metadata: /{minecraft_jvm_os}/{jvm_version_type}/0/manifest/url must be a string")
+
+            jvm_manifest = http_request("GET", jvm_meta_manifest_url, accept="application/json").json()
+
+            if not isinstance(jvm_manifest, dict):
+                raise ValueError("jvm manifest: / must be an object")
+
+            jvm_manifest["version"] = jvm_meta[0].get("version", {}).get("name")
+
+            jvm_manifest_file.parent.mkdir(parents=True, exist_ok=True)
+            with jvm_manifest_file.open("wt") as jvm_manifest_fp:
+                json.dump(jvm_manifest, jvm_manifest_fp)
+        
+        self._jvm_path = jvm_dir.joinpath("bin", jvm_bin_filename)
+        self._jvm_version = jvm_manifest.get("version")
+
+        jvm_files = jvm_manifest.get("files")
+        if not isinstance(jvm_files, dict):
+            raise ValueError("jvm manifest: /files must be an object")
 
-        jvm_exec_files = []
-        os.makedirs(jvm_dir, exist_ok=True)
         for jvm_file_path_prefix, jvm_file in jvm_files.items():
-            if jvm_file["type"] == "file":
-                jvm_file_path = path.join(jvm_dir, jvm_file_path_prefix)
-                jvm_download_info = jvm_file["downloads"]["raw"]
-                if not path.isfile(jvm_file_path) or path.getsize(jvm_file_path) != jvm_download_info["size"]:
-                    self.dl.append(DownloadEntry.from_meta(jvm_download_info, jvm_file_path, name=jvm_file_path_prefix))
-                if jvm_file.get("executable", False):
-                    jvm_exec_files.append(jvm_file_path)
-
-        if len(jvm_exec_files):
-            def finalize():
-                for exec_file in jvm_exec_files:
-                    os.chmod(exec_file, 0o777)
-            self.dl.add_callback(finalize)
-
-    def download(self, *, progress_callback: 'Optional[Callable[[DownloadProgress], None]]' = None) -> 'DownloadReport':
-        """ Download all missing files computed in `prepare_` methods. """
-        return self.dl.download_files(progress_callback=progress_callback)
+            if jvm_file.get("type") == "file":
 
-
-    def install(self, *, jvm: bool = False) -> 'DownloadReport':
-
-        """
-        Prepare (meta, jar, assets, logger, libs, jvm) and download the version with optional JVM installation.
-        Return True if download is successful.
+                jvm_file_path = jvm_dir / jvm_file_path_prefix
+                jvm_download_raw = jvm_file.get("downloads", {}).get("raw")
+                jvm_download_entry = parse_download_entry(jvm_download_raw, jvm_file_path, f"jvm manifest: /files/{jvm_file_path_prefix}/downloads/raw")
+                jvm_download_entry.executable = jvm_file.get("executable", False)
+
+                self._dl.add(jvm_download_entry, verify=True)
+        
+        watcher.handle(JvmLoadedEvent(self._jvm_version, JvmLoadedEvent.MOJANG))
+
+    def _resolve_builtin_jvm(self, watcher: Watcher, reason: str, major_version: Optional[int]) -> None:
+        """Internal function to find the builtin Java executable, the reason why this is
+        needed is given in parameter. The expected major version is also given, it should
+        not be none because we cannot check builtin version.
+        """
+
+        if major_version is None:
+            raise JvmNotFoundError(reason)
+
+        builtin_path = shutil.which(jvm_bin_filename)
+        if builtin_path is None:
+            raise JvmNotFoundError(reason)
+        
+        try:
+            
+            # Get version of the JVM.
+            process = Popen([builtin_path, "-version"], bufsize=1, stdout=PIPE, stderr=STDOUT, universal_newlines=True)
+            stdout, _stderr = process.communicate(timeout=1)
+
+            version_start = stdout.index(f"1.{major_version}" if major_version <= 8 else str(major_version))
+            version = None
+            
+            # Parse version by getting all character that are numeric or '.'.
+            for i, ch in enumerate(stdout[version_start:]):
+                if not ch.isnumeric() and ch not in (".", "_"):
+                    version = stdout[version_start:i]
+                    break
+            
+            if version is None:
+                raise ValueError()
+
+        except (TimeoutExpired, ValueError):
+            raise JvmNotFoundError(JvmNotFoundError.BUILTIN_INVALID_VERSION)
+
+        self._jvm_path = Path(builtin_path)
+        self._jvm_version = version
+        watcher.handle(JvmLoadedEvent(version, JvmLoadedEvent.BUILTIN))
+
+    def _download(self, watcher: Watcher) -> None:
+        
+        entries_count = len(self._dl.entries)
+        if not entries_count:
+            return
+        
+        # Note: do not create more thread than available entries.
+        threads_count = min(entries_count, (os.cpu_count() or 1) * 4)
+        errors = []
+
+        watcher.handle(DownloadStartEvent(threads_count, entries_count, self._dl.size))
+
+        for result_count, result in self._dl.download(threads_count, partial_progress=True):
+            if isinstance(result, DownloadResultProgress):
+                watcher.handle(DownloadProgressEvent(
+                    result.thread_id,
+                    result_count,
+                    result.entry,
+                    result.size,
+                    result.speed,
+                    result.done
+                ))
+            elif isinstance(result, DownloadResultError):
+                errors.append((result.entry, result.code))
+
+        # If errors are present, raise an error.
+        if len(errors):
+            raise DownloadError(errors)
+        
+        # Clear entries if successful, therefore multiple calls can be chained if
+        # needed, without re-downloading the same files.
+        self._dl.clear()
+        
+        watcher.handle(DownloadCompleteEvent())
+
+    def _resolve_env(self, watcher: Watcher) -> Environment:
+        """Step for computing correct environment to run the game as configured in this 
+        version's instance.²
         """
 
-        self.prepare_meta()
-        self.prepare_jar()
-        self.prepare_assets()
-        self.prepare_logger()
-        self.prepare_libraries()
-        if jvm:
-            self.prepare_jvm()
-
-        return self.download()
-
-    def start(self, opts: 'Optional[StartOptions]' = None):
-        """ Faster method to start the version. This actually use `Start` class, however, you can use it directly. """
-        start = Start(self)
-        start.prepare(opts or StartOptions())
-        start.start()
-
-
-class StartOptions:
-
-    def __init__(self):
-        self.auth_session: Optional[AuthSession] = None
-        self.uuid: Optional[str] = None             # DEPRECATED, use OfflineAuthSession or 'with_offline'
-        self.username: Optional[str] = None         # DEPRECATED, use OfflineAuthSession or 'with_offline'
-        self.demo: bool = False
-        self.resolution: Optional[Tuple[int, int]] = None
-        self.disable_multiplayer: bool = False
-        self.disable_chat: bool = False
-        self.server_address: Optional[str] = None
-        self.server_port: Optional[int] = None
-        self.jvm_exec: Optional[str] = None         # Overrides the version's jvm_exec
-        self.old_fix: bool = True                   # For legacy merge sort and betacraft proxy
-        self.features: Dict[str, bool] = {}         # Additional features
-
-    @classmethod
-    def with_online(cls, auth_session: 'AuthSession') -> 'StartOptions':
-        opts = StartOptions()
-        opts.auth_session = auth_session
-        return opts
-
-    @classmethod
-    def with_offline(cls, username: Optional[str], uuid: Optional[str]) -> 'StartOptions':
-        opts = StartOptions()
-        opts.auth_session = OfflineAuthSession(uuid, username)
-        return opts
-
-
-class Start:
-
-    """
-    Class used to control the starting procedure of Minecraft, it is made in order to allow the user to customize
-    every argument given to the executable.
-    """
-
-    def __init__(self, version: Version):
-
-        self.version = version
-
-        self.args_replacements: Dict[str, str] = {}
-        self.main_class: Optional[str] = None
-        self.jvm_args: List[str] = []
-        self.game_args: List[str] = []
-
-        # Additional binaries files to add to bin dir.
-        # These files will be symlinked on linux and copied on Windows (privilege issue).
-        self.bin_files: List[str] = []
-
-        self.bin_dir_factory: Callable[[str], str] = self.default_bin_dir_factory
-        self.runner: Callable[[List[str], str], None] = self.default_runner
-
-    def _check_version(self):
-        if self.version.version_meta is None:
-            raise ValueError("You should install the version metadata first.")
-
-    def get_username(self) -> str:
-        return self.args_replacements.get("auth_player_name", "n/a")
+        assert self._assets_index_version is not None, "_resolve_assets() missing"
 
-    def get_uuid(self) -> str:
-        return self.args_replacements.get("auth_uuid", "n/a")
+        # Main class
+        main_class = self._metadata.get("mainClass")
+        if not isinstance(main_class, str):
+            raise ValueError("metadata: /mainClass must be a string")
+
+        # Get authentication of create a random offline.
+        auth_session = self.auth_session or OfflineAuthSession(None, None)
+
+        # Class path, without main class (added later depending on arguments present).
+        class_path = list(map(str, self._class_libs))
+
+        # Environment definition.
+        env = Environment(self.context, main_class)
+        env.jvm_args.append(str(self._jvm_path))
+
+        env.native_libs = self._native_libs.copy()
+        env.fixes = self._applied_fixes
+        all_features = set()
+
+        # Check if modern arguments are present (> 1.12.2).
+        modern_args = self._metadata.get("arguments")
+        if modern_args is not None:
+
+            if not isinstance(modern_args, dict):
+                raise ValueError("metadata: /arguments must be an object")
+        
+            # Interpret JVM arguments.
+            modern_jvm_args = modern_args.get("jvm", [])
+            interpret_args(modern_jvm_args, self._features, env.jvm_args, "metadata: /arguments/jvm", all_features=all_features)
+            
+            # Interpret Game arguments.
+            modern_game_args = modern_args.get("game", [])
+            interpret_args(modern_game_args, self._features, env.game_args, "metadata: /arguments/game", all_features=all_features)
+        
+        else:
 
-    def prepare(self, opts: StartOptions):
+            interpret_args(legacy_jvm_args, self._features, env.jvm_args, f"<legacy_jvm_args>", all_features=all_features)
 
-        """
-        This method is used to prepare internal arguments arrays, main class and arguments variables according to the
-        version of this object and the given options. After this method you can call multiple times the `start` method.
-        However, before calling the `start` method you can change `args_replacements`, `main_class`, `jvm_args`,
-        `game_args`.\n
-        This method can raise a `ValueError` if the version metadata has no `mainClass` or if no JVM executable was set
-        in the given options nor downloaded by `Version` instance.
-        """
+            # Append legacy game arguments, if available.
+            legacy_game_args = self._metadata.get("minecraftArguments")
+            if legacy_game_args is not None:
+                if not isinstance(legacy_game_args, str):
+                    raise ValueError("metadata: /minecraftArguments must be a string")
+                env.game_args.extend(legacy_game_args.split(" "))
 
-        self._check_version()
+        # JVM argument for logging config
+        if self._logger_path is not None and self._logger_arg is not None:
+            env.jvm_args.append(self._logger_arg.replace("${path}", str(self._logger_path)))
 
-        # Main class
-        self.main_class = self.version.version_meta.get("mainClass")
-        if self.main_class is None:
-            raise ValueError("The version metadata has no main class to start.")
-
-        # Prepare JVM exec
-        jvm_exec = opts.jvm_exec
-        if jvm_exec is None:
-            jvm_exec = self.version.jvm_exec
-            if jvm_exec is None:
-                raise ValueError("No JVM executable set in options or downloaded by the version.")
-
-        # Features
-        features = {
-            "is_demo_user": opts.demo,
-            "has_custom_resolution": opts.resolution is not None,
-            **opts.features
-        }
+        # JVM argument for launch wrapper JAR path
+        if main_class == "net.minecraft.launchwrapper.Launch":
+            env.jvm_args.append(f"-Dminecraft.client.jar={self._jar_path}")
 
-        # Auth (we fallback to OfflineAuthSession and deprecated 'opts.username' and 'opts.uuid' if not set)
-        auth_session = OfflineAuthSession(opts.username, opts.uuid) if opts.auth_session is None else opts.auth_session
-        uuid = auth_session.uuid
-        username = auth_session.username
+        # If no modern arguments, fix some arguments.
+        if modern_args is None:
+            # Old versions seems to prefer having the main class first in class path.
+            class_path.insert(0, str(self._jar_path))
+        else:
+            # Modern versions seems to prefer having the main class last in class path.
+            class_path.append(str(self._jar_path))
+   
+        # Get the last version in the parent's tree, we use it to apply legacy fixes.
+        ancestor_id = list(self._hierarchy[0].recurse())[-1].id
+
+        # Legacy proxy aims to fix things like skins on old versions.
+        # This is applicable to all alpha/beta and 1.0:1.5
+        if self.fixes.get(self.FIX_LEGACY_PROXY):
+
+            proxy_port = None
+            if ancestor_id.startswith("a1.0."):
+                proxy_port = 80
+            elif ancestor_id.startswith("a1.1."):
+                proxy_port = 11702
+            elif ancestor_id.startswith(("a1.", "b1.")):
+                proxy_port = 11705
+            elif ancestor_id in ("1.0", "1.1", "1.3", "1.4", "1.5") or \
+                ancestor_id.startswith(("1.2.", "1.3.", "1.4.", "1.5.")):
+                proxy_port = 11707
+            
+            if proxy_port is not None:
+                self._applied_fixes[self.FIX_LEGACY_PROXY] = f"betacraft.uk:{proxy_port}"
+                env.jvm_args.append("-Dhttp.proxyHost=betacraft.uk")
+                env.jvm_args.append(f"-Dhttp.proxyPort={proxy_port}")
+        
+        # Legacy merge sort is applicable to alpha and beta versions.
+        if ancestor_id.startswith(("a1.", "b1.")) and self.fixes.get(self.FIX_LEGACY_MERGE_SORT):
+            self._applied_fixes[self.FIX_LEGACY_MERGE_SORT] = True
+            env.jvm_args.append("-Djava.util.Arrays.useLegacyMergeSort=true")
+
+        # The arguments do not support custom resolution, try to fix.
+        if self.resolution is not None and "has_custom_resolution" not in all_features:
+            if self.fixes.get(self.FIX_LEGACY_RESOLUTION):
+                self._applied_fixes[self.FIX_LEGACY_RESOLUTION] = self.resolution
+                env.game_args.extend((
+                    "--width", str(self.resolution[0]),
+                    "--height", str(self.resolution[1]),
+                ))
+        
+        # The arguments do not support quick play.
+        if isinstance(self.quick_play, QuickPlayMultiplayer) and "is_quick_play_multiplayer" not in all_features:
+            if self.fixes.get(self.FIX_LEGACY_QUICK_PLAY):
+                self._applied_fixes[self.FIX_LEGACY_QUICK_PLAY] = f"{self.quick_play.host}:{self.quick_play.port}"
+                env.game_args.extend(("--server", self.quick_play.host))
+                env.game_args.extend(("--port", str(self.quick_play.port)))
+
+        # Global options.        
+        if self.disable_multiplayer:
+            env.game_args.append("--disableMultiplayer")
+        if self.disable_chat:
+            env.game_args.append("--disableChat")
 
         # Arguments replacements
-        self.args_replacements = {
+        env.args_replacements = {
             # Game
-            "auth_player_name": username,
-            "version_name": self.version.id,
-            "library_directory": self.version.context.libraries_dir,
-            "game_directory": self.version.context.work_dir,
-            "assets_root": self.version.context.assets_dir,
-            "assets_index_name": self.version.assets_index_version,
-            "auth_uuid": uuid,
+            "auth_player_name": auth_session.username,
+            "version_name": self._hierarchy[0].id,
+            "library_directory": str(self.context.libraries_dir),
+            "game_directory": str(self.context.work_dir),
+            "assets_root": str(self.context.assets_dir),
+            "assets_index_name": self._assets_index_version,
+            "auth_uuid": auth_session.uuid,
             "auth_access_token": auth_session.format_token_argument(False),
             "auth_xuid": auth_session.get_xuid(),
             "clientid": auth_session.client_id,
             "user_type": auth_session.user_type,
-            "version_type": self.version.version_meta.get("type", ""),
+            "version_type": self._metadata.get("type", ""),
             # Game (legacy)
             "auth_session": auth_session.format_token_argument(True),
-            "game_assets": self.version.assets_virtual_dir,
+            "game_assets": str(self._assets_virtual_dir or ""),
             "user_properties": "{}",
             # JVM
             "natives_directory": "",
             "launcher_name": LAUNCHER_NAME,
             "launcher_version": LAUNCHER_VERSION,
-            "classpath_separator": path.pathsep,
-            "classpath": path.pathsep.join(self.version.classpath_libs)
+            "classpath_separator": os.pathsep,
+            "classpath": os.pathsep.join(class_path)
         }
 
-        if opts.resolution is not None:
-            self.args_replacements["resolution_width"] = str(opts.resolution[0])
-            self.args_replacements["resolution_height"] = str(opts.resolution[1])
-
-        # Arguments
-        modern_args = self.version.version_meta.get("arguments", {})
-        modern_jvm_args = modern_args.get("jvm")
-        modern_game_args = modern_args.get("game")
-
-        self.jvm_args.clear()
-        self.game_args.clear()
-
-        # JVM arguments
-        self.jvm_args.append(jvm_exec)
-        interpret_args(LEGACY_JVM_ARGUMENTS if modern_jvm_args is None else modern_jvm_args, features, self.jvm_args)
+        if self.quick_play is not None and self.quick_play.feature in all_features:
+            self.quick_play.add_args_replacements(env.args_replacements)
 
-        # JVM argument for logging config
-        if self.version.logging_argument is not None and self.version.logging_file is not None:
-            self.jvm_args.append(self.version.logging_argument.replace("${path}", self.version.logging_file))
+        if self.resolution is not None:
+            env.args_replacements["resolution_width"] = str(self.resolution[0])
+            env.args_replacements["resolution_height"] = str(self.resolution[1])
+        
+        return env
 
-        # JVM argument for launch wrapper JAR path
-        if self.main_class == "net.minecraft.launchwrapper.Launch":
-            self.jvm_args.append(f"-Dminecraft.client.jar={self.version.version_jar_file}")
 
-        # Add old fix JVM args
-        if opts.old_fix:
-            version_split = self.version.id.split(".", 2)
-            if version_split[0].endswith("b1") or version_split[0].endswith("a1"):
-                self.jvm_args.append("-Djava.util.Arrays.useLegacyMergeSort=true")
-                self.jvm_args.append("-Dhttp.proxyHost=betacraft.pl")
-            elif len(version_split) >= 2 and len(version_split[1]) == 1 and ord("0") <= ord(version_split[1][0]) <= ord("5"):
-                self.jvm_args.append("-Dhttp.proxyHost=betacraft.pl")
-
-        # Game arguments
-        if modern_game_args is None:
-            # If no modern arguments were found, we try finding legacy game arguments.
-            self.game_args.extend(self.version.version_meta.get("minecraftArguments", "").split(" "))
-            # If the resolution is set but we are using legacy arguments, we
-            # manually add resolution arguments to the game args.
-            if opts.resolution is not None:
-                self.game_args.extend([
-                    "--width", str(opts.resolution[0]),
-                    "--height", str(opts.resolution[1]),
-                ])
-        else:
-            interpret_args(modern_game_args, features, self.game_args)
+class QuickPlay:
+    """Base class for quick play launch methods for the game.
+    Note that these quick play types may not be supported by the game.
+    """
 
-        if opts.disable_multiplayer:
-            self.game_args.append("--disableMultiplayer")
-        if opts.disable_chat:
-            self.game_args.append("--disableChat")
-
-        if opts.server_address is not None:
-            self.game_args.extend(("--server", opts.server_address))
-        if opts.server_port is not None:
-            self.game_args.extend(("--port", str(opts.server_port)))
-
-    def start(self):
-
-        """
-        Start the game using configured attributes `args_replacements`, `main_class`, `jvm_args`, `game_args`.
-        You can easily configure these attributes with the `prepare` method.\n
-        This method actually use the `bin_dir_factory` of this object to produce a path where to extract binaries, by
-        default a random UUID is appended to the common `bin_dir` of the context. The `runner` argument is also used to
-        run the game, by default is uses the `subprocess.run` method. These two attributes can be changed before calling
-        this method.\n
-        This method may raise `BinaryNotFound` when one of the `self.bin_files` can't be resolved.
-        """
-
-        if self.main_class is None:
-            raise ValueError("Main class should be set before starting the game.")
-
-        bin_dir = self.bin_dir_factory(self.version.context.bin_dir)
-        cleaned = False
-
-        def cleanup():
-            nonlocal cleaned
-            if not cleaned:
-                shutil.rmtree(bin_dir, ignore_errors=True)
-                cleaned = True
-
-        import atexit
-        atexit.register(cleanup)
-
-        os.makedirs(bin_dir, exist_ok=True)
-        for native_lib in self.version.native_libs:
-            with ZipFile(native_lib, "r") as native_zip:
-                for native_zip_info in native_zip.infolist():
-                    native_name = native_zip_info.filename
-                    if can_extract_native(native_name):
-                        try:
-                            native_name = native_name[native_name.rindex("/") + 1:]
-                        except ValueError:
-                            native_name = native_name
-                        with native_zip.open(native_zip_info, "r") as native_zip_file:
-                            with open(path.join(bin_dir, native_name), "wb") as native_file:
-                                shutil.copyfileobj(native_zip_file, native_file)
-
-        for bin_file_raw in self.bin_files:
-            # Resolve a potential symlink and check if the binary exists before linking.
-            bin_file = path.realpath(bin_file_raw)
-            if not path.isfile(bin_file):
-                raise BinaryNotFound(bin_file_raw)
-            bin_name = path.basename(bin_file)
-            # Here we try to remove the version numbers of .so files.
-            so_idx = bin_name.rfind(".so")
-            if so_idx >= 0:
-                bin_name = bin_name[:so_idx + len(".so")]
-            # Try to symlink the file in the bin dir, and fallback to simple copy.
-            bin_dst_file = path.join(bin_dir, bin_name)
-            try:
-                os.symlink(bin_file, bin_dst_file)
-            except OSError:
-                shutil.copyfile(bin_file, bin_dst_file)
-
-        self.args_replacements["natives_directory"] = bin_dir
-
-        self.runner([
-            *replace_list_vars(self.jvm_args, self.args_replacements),
-            self.main_class,
-            *replace_list_vars(self.game_args, self.args_replacements)
-        ], self.version.context.work_dir)
-
-        cleanup()
-
-    @staticmethod
-    def default_bin_dir_factory(common_bin_dir: str) -> str:
-        return path.join(common_bin_dir, str(uuid4()))
-
-    @staticmethod
-    def default_runner(args: List[str], cwd: str) -> None:
-        import subprocess
-        subprocess.run(args, cwd=cwd)
+    feature: str
 
+    def add_args_replacements(self, args_replacements: Dict[str, str]) -> None:
+        raise NotImplementedError
 
-class VersionManifest:
+class QuickPlaySingleplayer(QuickPlay):
+    """Quick play mode to launch a singleplayer level given its name.
+    """
 
-    def __init__(self, cache_file: Optional[str] = None, cache_timeout: Optional[float] = None):
-        self.data: Optional[float] = None
-        self.cache_timeout = cache_timeout
-        self.cache_file = cache_file
-        self.sync = False
+    feature = "is_quick_play_singleplayer"
 
-    def _ensure_data(self) -> Optional[dict]:
+    def __init__(self, level_name: str) -> None:
+        self.level_name = level_name
 
-        if self.data is None:
+    def add_args_replacements(self, args_replacements: Dict[str, str]) -> None:
+        args_replacements["quickPlaySingleplayer"] = self.level_name
 
-            headers = {}
-            cache_data = None
+class QuickPlayMultiplayer(QuickPlay):
+    """Quick play mode to automatically connect to a given server when launching game.
+    """
 
-            if self.cache_file is not None:
-                try:
-                    with open(self.cache_file, "rt") as cache_fp:
-                        cache_data = json.load(cache_fp)
-                    if "last_modified" in cache_data:
-                        headers["If-Modified-Since"] = cache_data["last_modified"]
-                except (OSError, JSONDecodeError):
-                    pass
+    feature = "is_quick_play_multiplayer"
 
-            rcv_headers = {}
-            status, data = (404, {})
+    def __init__(self, host: str, port: int = 25565) -> None:
+        self.host = host
+        self.port = port
 
-            if self.cache_timeout is None or self.cache_timeout > 0:
-                try:
-                    status, data = json_request(VERSION_MANIFEST_URL, "GET", headers=headers, ignore_error=True,
-                                                timeout=self.cache_timeout, rcv_headers=rcv_headers)
-                except OSError:
-                    pass  # We silently ignore OSError (all socket errors and URL errors) and use default 404
+    def add_args_replacements(self, args_replacements: Dict[str, str]) -> None:
+        args_replacements["quickPlayMultiplayer"] = f"{self.host}:{self.port}"
 
-            if status == 200:
-                if "Last-Modified" in rcv_headers:
-                    data["last_modified"] = rcv_headers["Last-Modified"]
-                self.data = data
-                self.sync = True
-                if self.cache_file is not None:
-                    os.makedirs(path.dirname(self.cache_file), exist_ok=True)
-                    with open(self.cache_file, "wt") as cache_fp:
-                        json.dump(data, cache_fp, indent=2)
-            else:
-                # If the status is not 200, we fall back to the cached data if it exists, if not, raise error.
-                # This can be 304 status, in this case cache_data is set so there is no problem.
-                if cache_data is None:
-                    raise VersionManifestError(VersionManifestError.NOT_FOUND)
-                self.data = cache_data
+class QuickPlayRealms(QuickPlay):
+    """Quick play mode to automatically connection to a given realm when launching game.
+    """
 
-        return self.data
+    feature = "is_quick_play_realms"
 
-    def filter_latest(self, version: str) -> Tuple[str, bool]:
-        if version in ("release", "snapshot"):
-            latest = self._ensure_data()["latest"].get(version)
-            if latest is not None:
-                return latest, True
-        return version, False
+    def __init__(self, realm: str) -> None:
+        self.realm = realm
+    
+    def add_args_replacements(self, args_replacements: Dict[str, str]) -> None:
+        args_replacements["quickPlayRealms"] = self.realm
 
-    def get_version(self, version: str) -> Optional[dict]:
-        version, _alias = self.filter_latest(version)
-        try:
-            for version_data in self._ensure_data()["versions"]:
-                if version_data["id"] == version:
-                    return version_data
-        except VersionManifestError:
-            pass  # Silently ignore manifest errors because we want to be able to launch offline.
-        return None
 
-    def all_versions(self) -> list:
-        return self._ensure_data()["versions"]
+class WatcherGroup(Watcher):
+    """A group of watcher that is itself a watcher, its functions dispatches events to
+    all tasks.
+    """
 
-    def get_version_type(self, version: str) -> str:
-        obj = self.get_version(version)
-        return "release" if obj is None else obj.get("type", "release")
+    def __init__(self) -> None:
+        self.children: Set[Watcher] = set()
+    
+    def add(self, watcher: Watcher) -> None:
+        """Add a watcher to the installer to this group.
+        """
+        self.children.add(watcher)
+    
+    def remove(self, watcher: Watcher) -> None:
+        """Remove a watcher from the group.
+        """
+        self.children.remove(watcher)
+    
+    def handle(self, event: Any) -> None:
+        for watcher in self.children:
+            watcher.handle(event)
 
+class SimpleWatcher(Watcher):
 
-class AuthSession:
+    def __init__(self, handlers: Dict[type, Callable[[Any], None]]) -> None:
+        self.handlers = handlers
 
-    type = "raw"
-    user_type = ""
-    fields = "access_token", "username", "uuid", "client_id"
+    def handle(self, event: Any) -> None:
+        handler = self.handlers.get(type(event))
+        if handler is not None:
+            handler(event)
 
-    @classmethod
-    def fix_data(cls, data: dict):
-        pass
 
-    def __init__(self):
-        self.access_token = ""
-        self.username = ""
-        self.uuid = ""
-        self.client_id = ""
+class _Library:
+    """Intermediate class representing a parsed game's library. This is subclassed to
+    denote. This class is not yet part of the public API.
+    """
+    __slots__ = "native", "entry"
+    def __init__(self, native: bool, entry: Optional[DownloadEntry]) -> None:
+        self.native = native
+        self.entry = entry
 
-    def format_token_argument(self, legacy: bool) -> str:
-        return f"token:{self.access_token}:{self.uuid}" if legacy else self.access_token
 
-    def get_xuid(self) -> str:
-        """ Getter specific to Microsoft, but common to auth sessions because it's used in `Start.prepare`. """
-        return ""
+class VersionNotFoundError(Exception):
+    """Raised when a version was not found. The version that was not found is given.
+    """
+    def __init__(self, version: str) -> None:
+        self.version = version
 
-    def validate(self) -> bool:
-        return True
+class TooMuchParentsError(Exception):
+    """Raised when a version hierarchy is too deep. The hierarchy of versions is given
+    in property `versions`.
+    """
+    def __init__(self, versions: List[VersionHandle]) -> None:
+        self.versions = versions
 
-    def refresh(self):
-        pass
+class LibraryNotFoundError(Exception):
+    """Critical error raised when a library has no download indication and is not 
+    currently installed in game's libraries.
+    """
+    def __init__(self, lib: LibrarySpecifier) -> None:
+        self.lib = lib
 
-    def invalidate(self):
-        pass
+class JarNotFoundError(Exception):
+    """Raised when no version's JAR file could be found from the metadata.
+    """
 
+class JvmNotFoundError(Exception):
+    """Raised if no JVM can be found, the particular reason is given as code. This error
+    is raised only if no builtin Java can be resolved.
+    """
 
-class OfflineAuthSession(AuthSession):
+    UNSUPPORTED_LIBC = "unsupported_libc"
+    UNSUPPORTED_ARCH = "unsupported_arch"
+    UNSUPPORTED_VERSION = "unsupported_version"
+    BUILTIN_INVALID_VERSION = "builtin_invalid_version"
 
-    type = "offline"
-    user_type = ""
+    def __init__(self, code: str) -> None:
+        self.code = code
 
-    def __init__(self, username: Optional[str], uuid: Optional[str]):
+class DownloadError(Exception):
+    """Raised when the downloader failed to download some entries.
+    """
+    def __init__(self, errors: List[Tuple[DownloadEntry, str]]) -> None:
         super().__init__()
-        if uuid is not None and len(uuid) == 32:
-            # If the UUID is already valid.
-            self.uuid = uuid
-            self.username = uuid[:8] if username is None else username[:16]
-        else:
-            namespace_hash = UUID("8df5a464-38de-11ec-aa66-3fd636ee2ed7")
-            if username is None:
-                self.uuid = uuid5(namespace_hash, platform.node()).hex
-                self.username = self.uuid[:8]
-            else:
-                self.username = username[:16]
-                self.uuid = uuid5(namespace_hash, self.username).hex
+        self.errors = errors
 
-    def format_token_argument(self, legacy: bool) -> str:
-        return ""
 
+class VersionEvent:
+    """Base class for events regarding version.
+    """
+    __slots__ = "version",
+    def __init__(self, version: str) -> None:
+        self.version = version
 
-class YggdrasilAuthSession(AuthSession):
-
-    type = "yggdrasil"
-    user_type = "mojang"
-    fields = "access_token", "username", "uuid", "client_id"
-
-    @classmethod
-    def fix_data(cls, data: dict):
-        if "client_token" in data:
-            data["client_id"] = data.pop("client_token")
-
-    def __init__(self):
-        super().__init__()
-
-    def validate(self) -> bool:
-        return self.request("validate", {
-            "accessToken": self.access_token,
-            "clientToken": self.client_id
-        }, False)[0] == 204
-
-    def refresh(self):
-        _, res = self.request("refresh", {
-            "accessToken": self.access_token,
-            "clientToken": self.client_id
-        })
-        self.access_token = res["accessToken"]
-        self.username = res["selectedProfile"]["name"]  # Refresh username if renamed (does it works? to check.).
-
-    def invalidate(self):
-        self.request("invalidate", {
-            "accessToken": self.access_token,
-            "clientToken": self.client_id
-        }, False)
-
-    @classmethod
-    def authenticate(cls, client_id: str, email: str, password: str) -> 'YggdrasilAuthSession':
-        _, res = cls.request("authenticate", {
-            "agent": {
-                "name": "Minecraft",
-                "version": 1
-            },
-            "username": email,
-            "password": password,
-            "clientToken": client_id
-        })
-        sess = cls()
-        sess.access_token = res["accessToken"]
-        sess.username = res["selectedProfile"]["name"]
-        sess.uuid = res["selectedProfile"]["id"]
-        sess.client_id = res["clientToken"]
-        return sess
-
-    @classmethod
-    def request(cls, req: str, payload: dict, error: bool = True) -> Tuple[int, dict]:
-        code, res = json_request(f"https://authserver.mojang.com/{req}", "POST",
-                                 data=json.dumps(payload).encode("ascii"),
-                                 headers={"Content-Type": "application/json"},
-                                 ignore_error=True)
-        if error and code != 200:
-            raise AuthError(AuthError.YGGDRASIL, res["errorMessage"])
-        return code, res
-
-
-class MicrosoftAuthSession(AuthSession):
-
-    type = "microsoft"
-    user_type = "msa"
-    fields = "access_token", "username", "uuid", "client_id", "refresh_token", "app_id", "redirect_uri", "xuid"
-
-    @classmethod
-    def fix_data(cls, data: dict):
-        if "app_id" not in data and "client_id" in data:
-            data["app_id"] = data.pop("client_id")
-        if "client_id" not in data or not len(data["client_id"]):
-            data["client_id"] = str(uuid4())
-        if "xuid" not in data:
-            data["xuid"] = cls.decode_jwt_payload(data["access_token"])["xuid"]
-
-    def __init__(self):
-        super().__init__()
-        self.refresh_token = ""
-        self.app_id = ""
-        self.redirect_uri = ""
-        self.xuid = ""
-        self._new_username: Optional[str] = None
-
-    def get_xuid(self) -> str:
-        return self.xuid
-
-    def validate(self) -> bool:
-        self._new_username = None
-        code, res = self.mc_request_profile(self.access_token)
-        if code == 200:
-            username = res["name"]
-            if self.username != username:
-                self._new_username = username
-                return False
-            return True
-        return False
+class VersionLoadingEvent(VersionEvent):
+    """Event triggered when a version is being loaded.
+    """
 
-    def refresh(self):
-        if self._new_username is not None:
-            self.username = self._new_username
-            self._new_username = None
-        else:
-            res = self.authenticate_base({
-                "client_id": self.app_id,
-                "redirect_uri": self.redirect_uri,
-                "refresh_token": self.refresh_token,
-                "grant_type": "refresh_token",
-                "scope": "xboxlive.signin"
-            })
-            self.access_token = res["access_token"]
-            self.username = res["username"]
-            self.uuid = res["uuid"]
-
-    @staticmethod
-    def get_authentication_url(app_id: str, redirect_uri: str, email: str, nonce: str):
-        return "https://login.live.com/oauth20_authorize.srf?{}".format(url_parse.urlencode({
-            "client_id": app_id,
-            "redirect_uri": redirect_uri,
-            "response_type": "code id_token",
-            "scope": "xboxlive.signin offline_access openid email",
-            "login_hint": email,
-            "nonce": nonce,
-            "response_mode": "form_post"
-        }))
-
-    @staticmethod
-    def get_logout_url(app_id: str, redirect_uri: str):
-        return "https://login.live.com/oauth20_logout.srf?{}".format(url_parse.urlencode({
-            "client_id": app_id,
-            "redirect_uri": redirect_uri
-        }))
-
-    @classmethod
-    def check_token_id(cls, token_id: str, email: str, nonce: str) -> bool:
-        id_token_payload = cls.decode_jwt_payload(token_id)
-        return id_token_payload["nonce"] == nonce and id_token_payload["email"].casefold() == email.casefold()
-
-    @classmethod
-    def authenticate(cls, client_id: str, app_id: str, code: str, redirect_uri: str) -> 'MicrosoftAuthSession':
-        res = cls.authenticate_base({
-            "client_id": app_id,
-            "redirect_uri": redirect_uri,
-            "code": code,
-            "grant_type": "authorization_code",
-            "scope": "xboxlive.signin"
-        })
-        sess = cls()
-        sess.access_token = res["access_token"]
-        sess.username = res["username"]
-        sess.uuid = res["uuid"]
-        sess.client_id = client_id
-        sess.refresh_token = res["refresh_token"]
-        sess.app_id = app_id
-        sess.redirect_uri = redirect_uri
-        sess.xuid = cls.decode_jwt_payload(res["access_token"])["xuid"]
-        return sess
-
-    @classmethod
-    def authenticate_base(cls, request_token_payload: dict) -> dict:
-
-        # Microsoft OAuth
-        _, res = cls.ms_request("https://login.live.com/oauth20_token.srf", request_token_payload, payload_url_encoded=True)
-
-        if "error" in res:
-            raise AuthError(AuthError.MICROSOFT_OUTDATED_TOKEN)
-
-        ms_refresh_token = res.get("refresh_token")
-
-        # Xbox Live Token
-        _, res = cls.ms_request("https://user.auth.xboxlive.com/user/authenticate", {
-            "Properties": {
-                "AuthMethod": "RPS",
-                "SiteName": "user.auth.xboxlive.com",
-                "RpsTicket": "d={}".format(res["access_token"])
-            },
-            "RelyingParty": "http://auth.xboxlive.com",
-            "TokenType": "JWT"
-        })
-
-        xbl_token = res["Token"]
-        xbl_user_hash = res["DisplayClaims"]["xui"][0]["uhs"]
-
-        # Xbox Live XSTS Token
-        _, res = cls.ms_request("https://xsts.auth.xboxlive.com/xsts/authorize", {
-            "Properties": {
-                "SandboxId": "RETAIL",
-                "UserTokens": [xbl_token]
-            },
-            "RelyingParty": "rp://api.minecraftservices.com/",
-            "TokenType": "JWT"
-        })
-        xsts_token = res["Token"]
-
-        if xbl_user_hash != res["DisplayClaims"]["xui"][0]["uhs"]:
-            raise AuthError(AuthError.MICROSOFT_INCONSISTENT_USER_HASH)
-
-        # MC Services Auth
-        _, res = cls.ms_request("https://api.minecraftservices.com/authentication/login_with_xbox", {
-            "identityToken": f"XBL3.0 x={xbl_user_hash};{xsts_token}"
-        })
-        mc_access_token = res["access_token"]
-
-        # MC Services Profile
-        code, res = cls.mc_request_profile(mc_access_token)
-
-        if code == 404:
-            raise AuthError(AuthError.MICROSOFT_DOES_NOT_OWN_MINECRAFT)
-        elif code == 401:
-            raise AuthError(AuthError.MICROSOFT_OUTDATED_TOKEN)
-        elif "error" in res or code != 200:
-            raise AuthError(AuthError.MICROSOFT, res.get("errorMessage", res.get("error", "Unknown error")))
-
-        return {
-            "refresh_token": ms_refresh_token,
-            "access_token": mc_access_token,
-            "username": res["name"],
-            "uuid": res["id"]
-        }
+class VersionFetchingEvent(VersionEvent):
+    """Event triggered when a version is being fetched.
+    """
 
-    @classmethod
-    def ms_request(cls, url: str, payload: dict, *, payload_url_encoded: bool = False) -> Tuple[int, dict]:
-        data = (url_parse.urlencode(payload) if payload_url_encoded else json.dumps(payload)).encode("ascii")
-        content_type = "application/x-www-form-urlencoded" if payload_url_encoded else "application/json"
-        return json_request(url, "POST", data=data, headers={"Content-Type": content_type})
-
-    @classmethod
-    def mc_request_profile(cls, bearer: str) -> Tuple[int, dict]:
-        url = "https://api.minecraftservices.com/minecraft/profile"
-        return json_request(url, "GET", headers={"Authorization": f"Bearer {bearer}"}, ignore_error=True)
-
-    @classmethod
-    def base64url_decode(cls, s: str) -> bytes:
-        rem = len(s) % 4
-        if rem > 0:
-            s += "=" * (4 - rem)
-        return base64.urlsafe_b64decode(s)
-
-    @classmethod
-    def decode_jwt_payload(cls, jwt: str) -> dict:
-        return json.loads(cls.base64url_decode(jwt.split(".")[1]))
-
-
-class AuthDatabase:
-
-    types = {
-        YggdrasilAuthSession.type: YggdrasilAuthSession,
-        MicrosoftAuthSession.type: MicrosoftAuthSession
-    }
-
-    def __init__(self, filename: str, legacy_filename: Optional[str] = None):
-        self.filename = filename
-        self.legacy_filename = legacy_filename
-        self.sessions: Dict[str, Dict[str, AuthSession]] = {}
-        self.client_id: Optional[str] = None
-
-    def load(self):
-        self.sessions.clear()
-        if not path.isfile(self.filename):
-            self._load_legacy_and_delete()
-        try:
-            with open(self.filename, "rb") as fp:
-                data = json.load(fp)
-                self.client_id = data.get("client_id")
-                for typ, sess_type in self.types.items():
-                    typ_data = data.get(typ)
-                    if typ_data is not None:
-                        sessions = self.sessions[typ] = {}
-                        sessions_data = typ_data["sessions"]
-                        for email, sess_data in sessions_data.items():
-                            # Use class method fix_data to migrate data from older versions of the auth database.
-                            sess_type.fix_data(sess_data)
-                            sess = sess_type()
-                            for field in sess_type.fields:
-                                setattr(sess, field, sess_data.get(field, ""))
-                            sessions[email.casefold()] = sess
-        except (OSError, KeyError, TypeError, JSONDecodeError):
-            pass
+class VersionLoadedEvent(VersionEvent):
+    """Event triggered when a version has been successfully loaded.
+    """
 
-    def _load_legacy_and_delete(self):
-        if self.legacy_filename is not None:
-            try:
-                with open(self.legacy_filename, "rt") as fp:
-                    for line in fp.readlines():
-                        parts = line.split(" ")
-                        if len(parts) == 5:
-                            sess = YggdrasilAuthSession()
-                            sess.access_token = parts[4]
-                            sess.username = parts[2]
-                            sess.uuid = parts[3]
-                            sess.client_id = parts[1]
-                            self.put(parts[0], sess)
-                os.remove(self.legacy_filename)
-            except OSError:
-                pass
-
-    def save(self):
-        if not path.isfile(self.filename):
-            os.makedirs(path.dirname(self.filename), exist_ok=True)
-        with open(self.filename, "wt") as fp:
-            data = {}
-            if self.client_id is not None:
-                data["client_id"] = self.client_id
-            for typ, sessions in self.sessions.items():
-                if typ not in self.types:
-                    continue
-                sess_type = self.types[typ]
-                sessions_data = {}
-                data[typ] = {"sessions": sessions_data}
-                for email, sess in sessions.items():
-                    sess_data = sessions_data[email] = {}
-                    for field in sess_type.fields:
-                        sess_data[field] = getattr(sess, field)
-            json.dump(data, fp, indent=2)
-
-    def get(self, email: str, sess_type: Type[AuthSession]) -> Optional[AuthSession]:
-        sessions = self.sessions.get(sess_type.type)
-        return None if sessions is None else sessions.get(email.casefold())
-
-    def put(self, email: str, sess: AuthSession):
-        sessions = self.sessions.get(sess.type)
-        if sessions is None:
-            if sess.type not in self.types:
-                raise ValueError("Given session's type is not supported.")
-            sessions = self.sessions[sess.type] = {}
-        sessions[email.casefold()] = sess
-
-    def remove(self, email: str, sess_type: Type[AuthSession]) -> Optional[AuthSession]:
-        email = email.casefold()
-        sessions = self.sessions.get(sess_type.type)
-        if sessions is not None:
-            session = sessions.get(email)
-            if session is not None:
-                del sessions[email]
-                return session
-
-    def get_client_id(self) -> str:
-        if self.client_id is None or len(self.client_id) != 36:
-            self.client_id = str(uuid4())
-        return self.client_id
-
-
-class DownloadEntry:
-
-    """
-    An entry to download later in a `DownloadList`.
-    **This object should not be modified after being added to a list.**
-    *Fallbacks and name can however be modified after insertion.*
-    """
-
-    __slots__ = "url", "size", "sha1", "dst", "name", "fallbacks"
-
-    def __init__(self, url: str, dst: str, *, size: Optional[int] = None, sha1: Optional[str] = None, name: Optional[str] = None):
-        self.url = url
-        self.dst = dst
-        self.size = size
-        self.sha1 = sha1
-        self.name = url if name is None else name
-        self.fallbacks: Optional[list] = None
-
-    def add_fallback(self, fallback: 'DownloadEntry'):
-        if self.fallbacks is None:
-            self.fallbacks = [fallback]
-        else:
-            self.fallbacks.append(fallback)
+class FeaturesEvent:
+    """Event triggered when features for the version has been computed. Only enabled 
+    features are given as list of features.
+    """
+    __slots__ = "features",
+    def __init__(self, features: List[str]) -> None:
+        self.features = features
 
-    @classmethod
-    def from_meta(cls, info: dict, dst: str, *, name: Optional[str] = None) -> 'DownloadEntry':
-        if "url" not in info:
-            raise ValueError("Missing required 'url' field in download meta.", info)
-        return DownloadEntry(info["url"], dst, size=info.get("size"), sha1=info.get("sha1"), name=name)
+class JarFoundEvent:
+    """Event triggered when the game's JAR file has been found.
+    """
 
-    def __hash__(self) -> int:
-        # Making size and sha1 in the hash is useful to make them, this means that once added
-        # to a dictionary, these attributes should not be modified.
-        return hash((self.url, self.dst, self.size, self.sha1))
+class AssetsResolveEvent:
+    __slots__ = "index_version", "count"
+    def __init__(self, index_version: str, count: Optional[int]) -> None:
+        self.index_version = index_version
+        self.count = count
 
-    def __eq__(self, other):
-        return (self.url, self.dst, self.size, self.sha1) == (other.url, other.dst, other.size, other.sha1)
+class LibrariesResolvingEvent:
+    """Event triggered when libraries start being resolved.
+    """
 
+class LibrariesResolvedEvent:
+    """Event triggered when all libraries has been successfully resolved.
+    """
+    __slots__ = "class_libs_count", "native_libs_count"
+    def __init__(self, class_libs_count: int, native_libs_count: int) -> None:
+        self.class_libs_count = class_libs_count
+        self.native_libs_count = native_libs_count
+
+class LoggerFoundEvent:
+    __slots__ = "version"
+    def __init__(self, version: str) -> None:
+        self.version = version
 
-class DownloadReport:
+class JvmLoadingEvent:
+    """Event triggered when JVM start being resolved.
+    """
 
-    CONN_ERROR = "conn_error"
-    NOT_FOUND = "not_found"
-    INVALID_SIZE = "invalid_size"
-    INVALID_SHA1 = "invalid_sha1"
-    TOO_MANY_REDIRECTIONS = "too_many_redirections"
+class JvmLoadedEvent:
+    """Event triggered when JVM has been resolved. If count is none then the resolved 
+    version is a builtin JVM.
+    """
 
-    def __init__(self):
-        self.fails: Dict[DownloadEntry, str] = {}
-        self.final_size: int = 0
+    MOJANG = "mojang"    # Mojang provided JVM
+    BUILTIN = "builtin"  # Builtin JVM (java command)
+    CUSTOM = "custom"    # Custom JVM given with jvm_path
 
+    __slots__ = "version", "kind"
+    def __init__(self, version: Optional[str], kind: str) -> None:
+        self.version = version
+        self.kind = kind
 
-class DownloadList:
+class DownloadStartEvent:
+    __slots__ = "threads_count", "entries_count", "size"
+    def __init__(self, threads_count: int, entries_count: int, size: int) -> None:
+        self.threads_count = threads_count
+        self.entries_count = entries_count
+        self.size = size
 
-    __slots__ = "entries", "callbacks", "count", "size"
+class DownloadProgressEvent:
+    __slots__ = "thread_id", "count", "entry", "size", "speed", "done"
+    def __init__(self, thread_id: int, count: int, entry: DownloadEntry, size: int, speed: float, done: bool) -> None:
+        self.thread_id = thread_id
+        self.count = count
+        self.entry = entry
+        self.size = size
+        self.speed = speed
+        self.done = done
 
-    def __init__(self):
-        self.entries: Dict[str, List[DownloadEntry]] = {}
-        self.callbacks: List[Callable[[], None]] = []
-        self.count = 0
-        self.size = 0
+class DownloadCompleteEvent:
+    __slots__ = tuple()
 
-    def append(self, entry: DownloadEntry):
-        url_parsed = url_parse.urlparse(entry.url)
-        if url_parsed.scheme not in ("http", "https"):
-            raise ValueError(f"Illegal URL scheme '{url_parsed.scheme}://' for HTTP connection.")
-        host_key = f"{int(url_parsed.scheme == 'https')}{url_parsed.netloc}"
-        entries = self.entries.get(host_key)
-        if entries is None:
-            self.entries[host_key] = entries = []
-        entries.append(entry)
-        self.count += 1
-        if entry.size is not None:
-            self.size += entry.size
 
-    def reset(self):
-        """ Clear the whole download list (entries, callbacks, total count and size). """
-        self.entries.clear()
-        self.callbacks.clear()
-        self.count = 0
-        self.size = 0
+class VersionManifest:
+    """The Mojang's official version manifest. Providing officially available versions 
+    with optional cache file.
+    """
 
-    def add_callback(self, callback: Callable[[], None]):
-        """ Add a function that will be called anyway at the end of the actual download. """
-        self.callbacks.append(callback)
+    def __init__(self, cache_file: Optional[Path] = None) -> None:
+        self.data: Optional[dict] = None
+        self.cache_file = cache_file
 
-    def download_files(self, *, progress_callback: 'Optional[Callable[[DownloadProgress], None]]' = None) -> DownloadReport:
+    def _ensure_data(self) -> dict:
+        """Internal method that ensure that the manifest data is up-to-date.
 
-        """
-        Downloads the given list of files. Even if some downloads fails, it continues. Use the returned
-        `DownloadReport` to determine if some files has failed.
+        :return: The full data of the manifest.
+        :raises HttpError: Underlying HTTP error if manifest could not be requested.
         """
 
-        report = DownloadReport()
-
-        if len(self.entries):
-
-            buffer_back = bytearray(65536)
-            buffer = memoryview(buffer_back)
-            total_size = 0
-
-            if progress_callback is not None:
-                progress = DownloadProgress(self.size)
-                entry_progress = DownloadEntryProgress()
-                progress.entries.append(entry_progress)
-            else:
-                progress = None
-                entry_progress = None
-
-            # Maximum tries count or a single entry.
-            max_try_count = 3
-
-            # Internal utility to allow iterating over redirections.
-            def download_internal(current_dl: DownloadList, next_dl: DownloadList):
+        if self.data is None:
 
-                nonlocal total_size, buffer, progress_callback, progress, report
-
-                headers = {}
-                for host, entries in current_dl.entries.items():
-
-                    conn_type = HTTPSConnection if (host[0] == "1") else HTTPConnection
-                    conn = conn_type(host[1:])
-
-                    try:
-
-                        max_entry_idx = len(entries) - 1
-                        headers["Connection"] = "keep-alive"
-
-                        for i, entry in enumerate(entries):
-
-                            if i == max_entry_idx:
-                                # For the last entry
-                                headers["Connection"] = "close"
-
-                            # Allow modifying this URL when redirections happen.
-                            size_target = 0 if entry.size is None else entry.size
-                            error = None
-
-                            for _i in range(max_try_count):
-
-                                try:
-                                    conn.request("GET", entry.url, None, headers)
-                                    res = conn.getresponse()
-                                except (ConnectionError, OSError, HTTPException):
-                                    error = DownloadReport.CONN_ERROR
-                                    continue
-
-                                if res.status == 301 or res.status == 302:
-                                    redirect_url = res.headers["location"]
-                                    next_dl.append(DownloadEntry(redirect_url, entry.dst, size=entry.size, sha1=entry.sha1, name=entry.name))
-                                    break
-                                elif res.status != 200:
-                                    while res.readinto(buffer):
-                                        pass  # This loop is used to skip all bytes in the stream, and allow further request.
-                                    error = DownloadReport.NOT_FOUND
-                                    continue
-
-                                sha1 = None if entry.sha1 is None else hashlib.sha1()
-                                size = 0
-
-                                os.makedirs(path.dirname(entry.dst), exist_ok=True)
-                                try:
-                                    with open(entry.dst, "wb") as dst_fp:
-                                        while True:
-                                            read_len = res.readinto(buffer)
-                                            if not read_len:
-                                                break
-                                            buffer_view = buffer[:read_len]
-                                            size += read_len
-                                            total_size += read_len
-                                            if sha1 is not None:
-                                                sha1.update(buffer_view)
-                                            dst_fp.write(buffer_view)
-                                            if progress_callback is not None:
-                                                progress.size = total_size
-                                                entry_progress.name = entry.name
-                                                entry_progress.total = size_target
-                                                entry_progress.size = size
-                                                progress_callback(progress)
-                                except KeyboardInterrupt:
-                                    if path.isfile(entry.dst):
-                                        os.remove(entry.dst)
-                                    raise
-
-                                if entry.size is not None and size != entry.size:
-                                    error = DownloadReport.INVALID_SIZE
-                                elif entry.sha1 is not None and sha1.hexdigest() != entry.sha1:
-                                    error = DownloadReport.INVALID_SHA1
-                                else:
-                                    # When successful, add the downloaded size to the final size in report.
-                                    report.final_size += size
-                                    break  # Break the for loop in order to skip the for-else branch
-
-                                # We are here only when the file download has started but checks have failed,
-                                # then we should remove the file.
-                                if path.isfile(entry.dst):
-                                    os.remove(entry.dst)
-
-                                # If error happened, subtract the size and restart from the latest total_size.
-                                total_size -= size
-
-                            else:
-                                # This for-else branch is only triggered when break is not triggered.
-                                if entry.fallbacks is not None and len(entry.fallbacks):
-                                    # If there are fallbacks, don't set the error and go to them.
-                                    for fallback_entry in entry.fallbacks:
-                                        next_dl.append(fallback_entry)
-                                else:
-                                    # If the break was not triggered, an error should be set.
-                                    report.fails[entry] = error
-
-                    finally:
-                        conn.close()
-
-            # The following block is calling 'download_internal', it's used for taking
-            # redirections into account.
-            current_dl0 = self
-            redirect_depth = 0
-            while current_dl0.count:
-                if redirect_depth == 5:
-                    # When too many redirects, set fail reason for each entry.
-                    for failed_entries in current_dl0.entries.values():
-                        for failed_entry in failed_entries:
-                            report.fails[failed_entry] = DownloadReport.TOO_MANY_REDIRECTIONS
-                    break
-                next_list0 = DownloadList()
-                download_internal(current_dl0, next_list0)
-                current_dl0 = next_list0
-                redirect_depth += 1
+            headers = {}
+            cache_data = None
 
-        for callback in self.callbacks:
-            callback()
+            # If a cache file should be used, try opening it and read the last modified
+            # time that will be used for requesting the manifest, only if needed.
+            if self.cache_file is not None:
+                try:
+                    with self.cache_file.open("rt") as cache_fp:
+                        cache_data = json.load(cache_fp)
+                    if "last_modified" in cache_data:
+                        headers["If-Modified-Since"] = cache_data["last_modified"]
+                except (OSError, json.JSONDecodeError):
+                    pass
+            
+            try:
 
-        return report
+                res = http_request("GET", VERSION_MANIFEST_URL, 
+                    headers=headers, 
+                    accept="application/json")
+                
+                self.data = res.json()
 
+                if "Last-Modified" in res.headers:
+                    self.data["last_modified"] = res.headers["Last-Modified"]
 
-class DownloadEntryProgress:
+                if self.cache_file is not None:
+                    self.cache_file.parent.mkdir(parents=True, exist_ok=True)
+                    with self.cache_file.open("wt") as cache_fp:
+                        json.dump(self.data, cache_fp, indent=2)
+
+            except HttpError as error:
+                res = error.res
+                if res.status == 304 and cache_data is not None:
+                    self.data = cache_data
+                else:
+                    raise
 
-    __slots__ = "name", "size", "total"
+        return self.data
 
-    def __init__(self):
-        self.name = ""
-        self.size = 0
-        self.total = 0
+    def filter_latest(self, version: str) -> Tuple[str, bool]:
+        """Filter a version identifier if 'release' or 'snapshot' alias is used, then it's
+        replaced by the full version identifier, like `1.19.3`.
 
+        :param version: The version id or alias.
+        :return: A tuple containing the full version id and a boolean indicating if the
+        given version identifier is an alias.
+        :raises HttpError: Underlying HTTP error if manifest could not be requested.
+        """
 
-class DownloadProgress:
+        if version in ("release", "snapshot"):
+            latest = self._ensure_data()["latest"].get(version)
+            if latest is not None:
+                return latest, True
+        return version, False
 
-    __slots__ = "entries", "size", "total"
+    def get_version(self, version: str) -> Optional[dict]:
+        """Get a manifest's version metadata. Containing the metadata's URL, its SHA1 and
+        its type.
 
-    def __init__(self, total: int):
-        self.entries: List[DownloadEntryProgress] = []
-        self.size: int = 0  # Size can be greater that total, this happen if any DownloadEntry has an unknown size.
-        self.total = total
+        :param version: The version identifier.
+        :return: If found, the version is returned.
+        :raises HttpError: Underlying HTTP error if manifest could not be requested.
+        """
+        version, _alias = self.filter_latest(version)
+        for version_data in self._ensure_data()["versions"]:
+            if version_data["id"] == version:
+                return version_data
+        return None
 
+    def all_versions(self) -> list:
+        return self._ensure_data()["versions"]
 
-class BaseError(Exception):
 
-    def __init__(self, code: str):
-        super().__init__()
-        self.code = code
+class StandardRunner(Runner):
+    """Base class handling game running, this default implementation just create a
+    process and forwards to its outputs to the outputs of the current process.
+    """
 
+    def run(self, env: Environment) -> None:
 
-class JsonRequestError(BaseError):
+        from zipfile import ZipFile
 
-    INVALID_RESPONSE_NOT_JSON = "invalid_response_not_json"
+        bin_dir = env.context.gen_bin_dir()
+        replacements = env.args_replacements.copy()
+        replacements["natives_directory"] = str(bin_dir)
+        
+        bin_dir.mkdir(parents=True, exist_ok=True)
 
-    def __init__(self, code: str, url: str, method: str, status: int, data: bytes):
-        super().__init__(code)
-        self.url = url
-        self.method = method
-        self.status = status
-        self.data = data
+        try:
 
+            # Here we copy libraries into the bin directory, in case of archives (jar, zip)
+            # we extract all so/dll/dylib files into the directory, if this is a directly
+            # pointing to an archive, we symlink or copy it in-place.
+            if len(env.native_libs):
+                for src_file in env.native_libs:
+
+                    if not src_file.is_file():
+                        raise ValueError(f"source native file not found: {src_file}")
+
+                    native_name = src_file.name
+                    if native_name.endswith((".zip", ".jar")):
+
+                        with ZipFile(src_file, "r") as native_zip:
+                            for native_zip_info in native_zip.infolist():
+                                native_name = native_zip_info.filename
+                                if native_name.endswith((".so", ".dll", ".dylib")):
+
+                                    try:
+                                        native_name = native_name[native_name.rindex("/") + 1:]
+                                    except ValueError:
+                                        native_name = native_name
+                                    
+                                    dst_file = bin_dir / native_name
+
+                                    with native_zip.open(native_zip_info, "r") as src_fp:
+                                        with dst_file.open("wb") as dst_fp:
+                                            shutil.copyfileobj(src_fp, dst_fp)
+                                    
+                    else:
+
+                        # Here we try to remove the version numbers of .so files.
+                        so_idx = native_name.rfind(".so")
+                        if so_idx >= 0:
+                            native_name = native_name[:so_idx + len(".so")]
+                        # Try to symlink the file in the bin dir, and fallback to simple copy.
+                        dst_file = bin_dir / native_name
 
-class AuthError(BaseError):
+                        try:
+                            dst_file.symlink_to(src_file)
+                        except OSError:
+                            shutil.copyfile(src_file, dst_file)
+                        
+            # We create the wrapper process with required arguments.
+            process = self.process_create([
+                *replace_list_vars(env.jvm_args, replacements),
+                env.main_class,
+                *replace_list_vars(env.game_args, replacements)
+            ], env.context.work_dir)
+
+            self.process_wait(process)
+
+        finally:
+            # Any error while setting up the binary directory cause it to be deleted.
+            shutil.rmtree(bin_dir, ignore_errors=True)
+
+    def process_create(self, args: List[str], work_dir: Path) -> Popen:
+        """This function is called when process needs to be created with the given 
+        arguments in the given working directory. The default implementation does nothing
+        special but this can be used to create the process with enabled output piping,
+        to later use in `process_wait`.
+        """
+        return Popen(args, cwd=work_dir)
+
+    def process_wait(self, process: Popen) -> None:
+        """This function is called with the running Minecraft process for waiting the end
+        of the process. Implementors may want to read incoming logging.
+        """
+        process.wait()
+
+class StreamRunner(StandardRunner):
+    """A specialized implementation of `RunTask` which allows streaming the game's output
+    logs. This implementation also provides parsing of log4j XML layouts for logs.
+    """
+    
+    def process_create(self, args: List[str], work_dir: Path) -> Popen:
+        return Popen(args, cwd=work_dir, stdout=PIPE, stderr=STDOUT, bufsize=1, universal_newlines=True)
 
-    YGGDRASIL = "yggdrasil"
-    MICROSOFT = "microsoft"
-    MICROSOFT_INCONSISTENT_USER_HASH = "microsoft.inconsistent_user_hash"
-    MICROSOFT_DOES_NOT_OWN_MINECRAFT = "microsoft.does_not_own_minecraft"
-    MICROSOFT_OUTDATED_TOKEN = "microsoft.outdated_token"
+    def process_wait(self, process: Popen) -> None:
 
-    def __init__(self, code: str, details: Optional[str] = None):
-        super().__init__(code)
-        self.details = details
+        from threading import Thread
 
+        thread = Thread(target=self.process_stream_thread, name="Minecraft Stream Thread", args=(process,))
+        thread.start()
 
-class VersionManifestError(BaseError):
-    NOT_FOUND = "not_found"
+        process.wait()
 
+    def process_stream_thread(self, process: Popen) -> None:
 
-class VersionError(BaseError):
+        stdout = process.stdout
+        assert stdout is not None, "should not be none because it should be piped"
 
-    NOT_FOUND = "not_found"
-    TO_MUCH_PARENTS = "to_much_parents"
-    JAR_NOT_FOUND = "jar_not_found"
-    INVALID_ID = "invalid_id"
+        parser = None
+        for line in iter(stdout.readline, ""):
 
-    def __init__(self, code: str, version: str):
-        super().__init__(code)
-        self.version = version
+            if parser is None:
+                if line.lstrip().startswith("<log4j:"):
+                    parser = XmlStreamParser()
+                else:
+                    parser = StreamParser()
 
+            if not parser.feed(line, self.process_stream_event):
+                parser = StreamParser()
+                parser.feed(line, self.process_stream_event)  # Should not fail
+    
+    def process_stream_event(self, event: Any) -> None:
+        """This function gets called when an event is received from the game's log.
+        """
 
-class JvmLoadingError(BaseError):
-    UNSUPPORTED_ARCH = "unsupported_arch"
-    UNSUPPORTED_VERSION = "unsupported_version"
-    UNSUPPORTED_LIBC = "unsupported_libc"
+class StreamParser:
+    """Base implementation of game's output stream parsing.
+    """
 
+    def feed(self, line: str, callback: Callable[[Any], None]) -> bool:
+        """Feed the parser, if successful the callback can be used to give back the object
+        containing the parsed log, and true should be returned. Returning false mean that
+        parsing has failed, the caller can then switch to a simpler parser.
 
-class BinaryNotFound(Exception):
+        This default implementation just forward incoming lines to the callback.
+        """
+        callback(line)
+        return True
 
-    """
-    This type of error can be raised by `Start.start(...)` to signal the caller that
-    one of the specified additional binaries doesn't exists and therefore can't be 
-    symlinked nor copied inside the runtime's bin directory.
+class XmlStreamParser(StreamParser):
+    """This parser produces `XmlStreamEvent` kind of events by parsing the game's stream
+    as a log4j log stream.
     """
 
-    def __init__(self, bin_file: str):
-        super().__init__()
-        self.bin_file = bin_file
+    def __init__(self) -> None:
+        self.xml = ET.XMLPullParser(["start", "end"])
+        self.xml.feed("<?xml version=\"1.0\"?><root xmlns:log4j=\"log4j\">")
+        self.next_event = None
 
+    def feed(self, line: str, callback: Callable[[Any], None]) -> bool:
+        self.xml.feed(line)
+        try:
+            for event, elem in self.xml.read_events():
+                if elem.tag == "{log4j}Event":
+                    if event == "start":
+                        self.next_event = XmlStreamEvent(int(elem.attrib["timestamp"]) / 1000.0,
+                            elem.attrib["logger"],
+                            elem.attrib["level"],
+                            elem.attrib["thread"])
+                    elif event == "end" and self.next_event is not None:
+                        callback(self.next_event)
+                        self.next_event = None
+                elif event == "end" and self.next_event is not None:
+                    if elem.tag == "{log4j}Message":
+                        self.next_event.message = elem.text
+                    elif elem.tag == "{log4j}Throwable":
+                        self.next_event.throwable = elem.text
+            return True
+        except ET.ParseError:
+            return False
 
-class LibrarySpecifier:
+class XmlStreamEvent:
+    """Class representing an event happening in the game's logs.
+    """
 
-    __slots__ = "group", "artifact", "version", "classifier"
+    __slots__ = "time", "logger", "level", "thread", "message", "throwable"
 
-    def __init__(self, group: str, artifact: str, version: str, classifier: "Optional[str]"):
-        self.group = group
-        self.artifact = artifact
-        self.version = version
-        self.classifier = classifier
+    def __init__(self, time: float, logger: str, level: str, thread: str) -> None:
+        self.time = time
+        self.logger = logger
+        self.level = level
+        self.thread = thread
+        self.message = None
+        self.throwable = None
     
-    @classmethod
-    def from_str(cls, s: str) -> "LibrarySpecifier":
-        """ Parse a library specifier string 'group:artifact:version[:classifier]'. """
-        parts = s.split(":", 3)
-        if len(parts) < 3:
-            raise ValueError("Invalid library specifier.")
-        else:
-            return LibrarySpecifier(parts[0], parts[1], parts[2], parts[3] if len(parts) == 4 else None)
-
-    def __str__(self) -> str:
-        return f"{self.group}:{self.artifact}:{self.version}" + ("" if self.classifier is None else f":{self.classifier}")
-
     def __repr__(self) -> str:
-        return f"<LibrarySpecifier {self}>"
+        return f"<ProcessEvent date: {self.time}, logger: {self.logger}, level: {self.level}, thread: {self.thread}, message: {repr(self.message)}>"
 
-    def jar_file_path(self) -> str:
-        """ 
-        Return the standard path to store the JAR file of this specifier, the path separator
-        will always be forward slashes '/', because it's compatible with linux/mac/windows 
-        and URL paths.\n
-        Specifier `com.foo.bar:artifact:version` gives `com/foo/bar/artifact/version/artifact-version.jar`.
-        """
-        file_name = f"{self.artifact}-{self.version}" + ("" if self.classifier is None else f"-{self.classifier}") + ".jar"
-        return "/".join([*self.group.split("."), self.artifact, self.version, file_name])
-
-
-def http_request(url: str, method: str, *,
-                 data: Optional[bytes] = None,
-                 headers: Optional[dict] = None,
-                 timeout: Optional[float] = None,
-                 rcv_headers: Optional[dict] = None) -> Tuple[int, bytes]:
 
+def parse_download_entry(value: Any, dst: Path, path: str) -> DownloadEntry:
+    """Common function to parse a download entry from a metadata JSON file.
     """
-    Make an HTTP request at a specified URL and retrieve raw data. This is a simpler wrapper
-    to the standard `url.request.urlopen` wrapper, it ignores HTTP error codes.
 
-    :param url: The URL to request.
-    :param method: The HTTP method to use for this request.
-    :param data: Optional data to put in the request's body.
-    :param headers: Optional headers to add to default ones.
-    :param timeout: Optional timeout for the TCP handshake.
-    :param rcv_headers: Optional received headers dictionary, populated after
-    :return: A tuple (HTTP response code, data bytes).
-    """
+    if not isinstance(value, dict):
+        raise ValueError(f"{path} must an object")
 
-    if headers is None:
-        headers = {}
-
-    try:
+    url = value.get("url")
+    if not isinstance(url, str):
+        raise ValueError(f"{path}/url must be a string")
 
-        try:
-            import certifi
-            ctx = ssl.create_default_context(cafile=certifi.where())
-        except ImportError:
-            ctx = None
+    size = value.get("size")
+    if size is not None and not isinstance(size, int):
+        raise ValueError(f"{path}/size must be an integer")
 
-        req = UrlRequest(url, data, headers, method=method)
-        res: HTTPResponse = url_request.urlopen(req, timeout=timeout, context=ctx)
+    sha1 = value.get("sha1")
+    if sha1 is not None and not isinstance(sha1, str):
+        raise ValueError(f"{path}/sha1 must be a string")
 
-    except HTTPError as err:
-        res = cast(HTTPResponse, err)
+    return DownloadEntry(url, dst, size=size, sha1=sha1, name=dst.name)
 
-    if rcv_headers is not None:
-        for header_name, header_value in res.getheaders():
-            rcv_headers[header_name] = header_value
 
-    return res.status, res.read()
+def interpret_rule(rules: Any, features: Dict[str, bool], path: str, *, 
+    all_features: Optional[Set[str]] = None
+) -> bool:
+    """Common function to interpret rules and determine if the condition is met.
+    """
 
+    if not isinstance(rules, list):
+        raise ValueError(f"{path} must be a list")
 
-def json_request(url: str, method: str, *,
-                 data: Optional[bytes] = None,
-                 headers: Optional[dict] = None,
-                 ignore_error: bool = False,
-                 timeout: Optional[float] = None,
-                 rcv_headers: Optional[dict] = None) -> Tuple[int, dict]:
+    allowed = False
+    for i, rule in enumerate(rules):
 
-    """
-    A simple wrapper around ``http_request` function to decode returned data to JSON. If decoding fails and parameter
-    `ignore_error` is false, error `JsonRequestError` is raised with `JsonRequestError.INVALID_RESPONSE_NOT_JSON`.
-    """
+        if not isinstance(rule, dict):
+            raise ValueError(f"{path}/{i} must be an object")
 
-    if headers is None:
-        headers = {}
-    if "Accept" not in headers:
-        headers["Accept"] = "application/json"
+        rule_os = rule.get("os")
+        if rule_os is not None and not interpret_rule_os(rule_os, f"{path}/{i}/os"):
+            continue
 
-    status, data = http_request(url, method, data=data, headers=headers, timeout=timeout, rcv_headers=rcv_headers)
+        rule_features = rule.get("features")
+        if rule_features is not None:
+            
+            if not isinstance(rule_features, dict):
+                raise ValueError(f"{path}/{i}/features must be an object")
 
-    try:
-        return status, json.loads(data)
-    except JSONDecodeError:
-        if ignore_error:
-            return status, {"raw": data}
+            feat_valid = True
+            for feat_name, feat_expected in rule_features.items():
+                if all_features is not None:
+                    all_features.add(feat_name)
+                if features.get(feat_name) != feat_expected:
+                    feat_valid = False
+            
+            if not feat_valid:
+                continue
+        
+        action = rule.get("action")
+        if action == "disallow":
+            return False    # Early return because of disallow.
+        elif action == "allow":
+            allowed = True  # Only other possible value is "allow".
         else:
-            raise JsonRequestError(JsonRequestError.INVALID_RESPONSE_NOT_JSON, url, method, status, data)
-
-
-def json_simple_request(url: str, *, ignore_error: bool = False, timeout: Optional[int] = None) -> dict:
-    """ Make a GET request for a JSON API at specified URL. Might raise `JsonRequestError` if failed. """
-    return json_request(url, "GET", ignore_error=ignore_error, timeout=timeout)[1]
+            raise ValueError(f"{path}/{i}/action must be 'allow' and 'disallow'")
 
+    return allowed
 
-def merge_dict(dst: dict, other: dict):
 
+def interpret_rule_os(rule_os: Any, path: str) -> bool:
+    """Common function to interpret a rule constraint on the running OS.
     """
-    Merge the 'other' dict into the 'dst' dict. For every key/value in 'other', if the key is present in 'dst'
-    it does nothing. Unless values in both dict are also dict, in this case the merge is recursive. If the
-    value in both dict are list, the 'dst' list is extended (.extend()) with the one of 'other'.
-    """
-
-    for k, v in other.items():
-        if k in dst:
-            if isinstance(dst[k], dict) and isinstance(other[k], dict):
-                merge_dict(dst[k], other[k])
-            elif isinstance(dst[k], list) and isinstance(other[k], list):
-                dst[k].extend(other[k])
-        else:
-            dst[k] = other[k]
 
-
-def interpret_rule_os(rule_os: dict) -> bool:
+    if not isinstance(rule_os, dict):
+        raise ValueError(f"{path} must be an object")
+    
     os_name = rule_os.get("name")
-    if os_name is None or os_name == get_minecraft_os():
+    if os_name is None or os_name == minecraft_os:
         os_arch = rule_os.get("arch")
-        if os_arch is None or os_arch == get_minecraft_arch():
+        if os_arch is None or os_arch == minecraft_arch:
             os_version = rule_os.get("version")
             if os_version is None or re.search(os_version, platform.version()) is not None:
                 return True
     return False
 
 
-def interpret_rule(rules: List[dict], features: Optional[dict] = None) -> bool:
-    allowed = False
-    for rule in rules:
-        rule_os = rule.get("os")
-        if rule_os is not None and not interpret_rule_os(rule_os):
-            continue
-        rule_features: Optional[dict] = rule.get("features")
-        if rule_features is not None:
-            feat_valid = True
-            for feat_name, feat_expected in rule_features.items():
-                if features.get(feat_name) != feat_expected:
-                    feat_valid = False
-                    break
-            if not feat_valid:
-                continue
-        allowed = (rule["action"] == "allow")
-    return allowed
+def interpret_args(args: Any, features: Dict[str, bool], dst: List[str], path: str, *, 
+    all_features: Optional[Set[str]] = None
+) -> None:
+    """Common function for interpreting a list of arguments, whose may be conditional
+    under some rules. An optional set of features can be given and will be filled with
+    all features found (even if not used).
+    """
+
+    if not isinstance(args, list):
+        raise ValueError(f"{path} must be a list")
 
+    for i, arg in enumerate(args):
 
-def interpret_args(args: list, features: dict, dst: List[str]):
-    for arg in args:
         if isinstance(arg, str):
             dst.append(arg)
-        else:
+        elif isinstance(arg, dict):
+
             rules = arg.get("rules")
             if rules is not None:
-                if not interpret_rule(rules, features):
+                if not interpret_rule(rules, features, f"{path}/{i}/rules", all_features=all_features):
                     continue
+            
             arg_value = arg["value"]
             if isinstance(arg_value, list):
                 dst.extend(arg_value)
             elif isinstance(arg_value, str):
                 dst.append(arg_value)
+            else:
+                raise ValueError(f"{path}/{i}/value must be a list or a string")
+        else:
+            raise ValueError(f"{path}/{i} must be an object or a string")
 
 
-def replace_vars(txt: str, replacements: Dict[str, str]) -> str:
+def replace_vars(text: str, replacements: Dict[str, str]) -> str:
+    """Replace all variables of the form `${foo}` in a string. If some keys are missing,
+    the unformatted text is returned.
+    """
     try:
-        return txt.replace("${", "{").format_map(replacements)
+        return text.replace("${", "{").format_map(replacements)
     except KeyError:
-        return txt
+        return text
 
 
-def replace_list_vars(lst: List[str], replacements: Dict[str, str]) -> Generator[str, None, None]:
-    return (replace_vars(elt, replacements) for elt in lst)
+def replace_list_vars(text_list: List[str], replacements: Dict[str, str]) -> Iterator[str]:
+    """Call `replace_vars` on multiple texts in a list with the same replacements.
+    """
+    return (replace_vars(elt, replacements) for elt in text_list)
 
 
-def get_minecraft_dir() -> str:
-    home = path.expanduser("~")
+def get_minecraft_dir() -> Path:
+    """Internal function to get the default directory for installing
+    and running Minecraft.
+    """
+    home = Path.home()
     return {
-        "Windows": path.join(home, "AppData", "Roaming", ".minecraft"),
-        "Darwin": path.join(home, "Library", "Application Support", "minecraft"),
-    }.get(platform.system(), path.join(home, ".minecraft"))
-
-
-_minecraft_os: Optional[str] = None
-def get_minecraft_os() -> str:
-    """ Return the current OS identifier used in rules matching, 'linux', 'windows', 'osx' and '' if not found. """
-    global _minecraft_os
-    if _minecraft_os is None:
-        _minecraft_os = {
-            "Linux": "linux", 
-            "Windows": "windows", 
-            "Darwin": "osx",
-            "FreeBSD": "freebsd"
-        }.get(platform.system(), "")
-    return _minecraft_os
-
-
-_minecraft_arch: Optional[str] = None
-def get_minecraft_arch() -> str:
-    """ Return the architecture to use in rules matching, 'x86', 'x86_64' or '' if not found. """
-    global _minecraft_arch
-    if _minecraft_arch is None:
-        machine = platform.machine().lower()
-        _minecraft_arch = {
-            "i386": "x86",
-            "i686": "x86",
-            "x86_64": "x86_64",
-            "amd64": "x86_64",
-            "arm64": "arm64",
-            "aarch64": "arm64",
-            "aarch32": "arm32",  # Don't know if this value is possible
-            "armv7l": "arm32",
-            "armv6l": "arm32",
-        }.get(machine, "")
-    return _minecraft_arch
-
-
-_minecraft_archbits: Optional[str] = None
-def get_minecraft_archbits() -> str:
-    """ Return the address size of the architecture used for rules matching, '64', '32', or '' if not found. """
-    global _minecraft_archbits
-    if _minecraft_archbits is None:
-        raw_bits = platform.architecture()[0]
-        _minecraft_archbits = "64" if raw_bits == "64bit" else "32" if raw_bits == "32bit" else ""
-    return _minecraft_archbits
-
-
-_minecraft_jvm_os: Optional[str] = None
-def get_minecraft_jvm_os() -> str:
-    """ Return the OS identifier used to choose the right JVM to download. """
-    global _minecraft_jvm_os
-    if _minecraft_jvm_os is None:
-        _minecraft_jvm_os = {
-            "osx": {"x86_64": "mac-os", "arm64": "mac-os-arm64"},
-            "linux": {"x86": "linux-i386", "x86_64": "linux"},
-            "windows": {"x86": "windows-x86", "x86_64": "windows-x64"}
-        }.get(get_minecraft_os(), {}).get(get_minecraft_arch())
-    return _minecraft_jvm_os
-
-
-def get_jvm_bin_filename() -> str:
-    """ Return the JVM binary filename for the current platform, 'javaw' on windows and 'java' on others. """
-    return "javaw.exe" if platform.system() == "Windows" else "java"
-
-
-def can_extract_native(filename: str) -> bool:
-    """ Return True if a file should be extracted to binaries directory. """
-    return filename.endswith((".so", ".dll", ".dylib"))
-
-
-def from_iso_date(raw: str) -> datetime:
-    """
-    Replacement for `datetime.fromisoformat()` which is missing from Python 3.6. This function
-    replace it if needed.
-    Currently, only a subset of the ISO format is supported, both hours, minutes and seconds
-    must be defined and the timezone, if present must contain both hours and minutes, no more.
-    """
-    if hasattr(datetime, "fromisoformat"):
-        return datetime.fromisoformat(raw)
-    from datetime import timezone, timedelta
-    tz_idx = raw.find("+")
-    dt = datetime.strptime(raw[:tz_idx], "%Y-%m-%dT%H:%M:%S")
-    if tz_idx != -1:
-        tz_dt = datetime.strptime(raw[tz_idx + 1:], "%H:%M")
-        dt = dt.replace(tzinfo=timezone(timedelta(hours=tz_dt.hour, minutes=tz_dt.minute)))
-    return dt
-
-
-def calc_input_sha1(input_stream, *, buffer_len: int = 8192) -> str:
-    h = hashlib.sha1()
-    b = bytearray(buffer_len)
-    mv = memoryview(b)
-    for n in iter(lambda: input_stream.readinto(mv), 0):
-        h.update(mv[:n])
-    return h.hexdigest()
-
+        "Windows": home.joinpath("AppData", "Roaming", ".minecraft"),
+        "Darwin": home.joinpath("Library", "Application Support", "minecraft"),
+    }.get(platform.system(), home / ".minecraft")
+
+
+# Name of the OS has used by Minecraft.
+minecraft_os = {
+    "Linux": "linux", 
+    "Windows": "windows", 
+    "Darwin": "osx",
+    "FreeBSD": "freebsd"
+}.get(platform.system())
+
+# Name of the processor's architecture has used by Minecraft.
+minecraft_arch = {
+    "i386": "x86",
+    "i686": "x86",
+    "x86_64": "x86_64",
+    "amd64": "x86_64",
+    "arm64": "arm64",
+    "aarch64": "arm64",
+    "armv7l": "arm32",
+    "armv6l": "arm32",
+}.get(platform.machine().lower())
+
+# Stores the bits length of pointers on the current system.
+minecraft_arch_bits = {
+    "64bit": 64,
+    "32bit": 32
+}.get(platform.architecture()[0])
+
+# Name of the OS has used by Mojang for officially distributed JVMs.
+minecraft_jvm_os = None if minecraft_arch is None else {
+    "Darwin": {"x86_64": "mac-os", "arm64": "mac-os-arm64"},
+    "Linux": {"x86": "linux-i386", "x86_64": "linux"},
+    "Windows": {"x86": "windows-x86", "x86_64": "windows-x64"}
+}.get(platform.system(), {}).get(minecraft_arch)
 
-LEGACY_JVM_ARGUMENTS = [
+# JVM arguments used if no arguments are specified.
+legacy_jvm_args = [
     {
         "rules": [{"action": "allow", "os": {"name": "osx"}}],
         "value": ["-XstartOnFirstThread"]
     },
     {
         "rules": [{"action": "allow", "os": {"name": "windows"}}],
         "value": "-XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump"
```

### Comparing `portablemc-3.3.1/portablemc/__main__.py` & `portablemc-4.0.0rc1/portablemc/__main__.py`

 * *Files identical despite different names*

### Comparing `portablemc-3.3.1/pyproject.toml` & `portablemc-4.0.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "portablemc"
-version = "3.3.1"
+version = "4.0.0rc1"
 description = "PortableMC is a module that provides both an API for development of your custom launcher and an executable script to run PortableMC CLI."
 authors = ["Théo Rozier <contact@theorozier.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/mindstorm38/portablemc"
 repository = "https://github.com/mindstorm38/portablemc"
 documentation = "https://github.com/mindstorm38/portablemc"
@@ -16,11 +16,14 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Environment :: Console"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.7"
+
+[tool.poetry.group.test.dependencies]
+pytest = "*"
 
 [tool.poetry.scripts]
 portablemc = "portablemc.cli:main"
```

