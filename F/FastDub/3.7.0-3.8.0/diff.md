# Comparing `tmp/FastDub-3.7.0.tar.gz` & `tmp/FastDub-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastDub-3.7.0.tar", last modified: Wed May 24 08:53:30 2023, max compression
+gzip compressed data, was "FastDub-3.8.0.tar", last modified: Sat Jul 29 13:18:03 2023, max compression
```

## Comparing `FastDub-3.7.0.tar` & `FastDub-3.8.0.tar`

### file list

```diff
@@ -1,44 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.862236 FastDub-3.7.0/
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.839062 FastDub-3.7.0/FastDub.egg-info/
--rw-rw-rw-   0        0        0    18202 2023-05-24 08:53:30.000000 FastDub-3.7.0/FastDub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-05-24 08:53:30.000000 FastDub-3.7.0/FastDub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 08:53:30.000000 FastDub-3.7.0/FastDub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2023-05-24 08:53:30.000000 FastDub-3.7.0/FastDub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 08:53:30.000000 FastDub-3.7.0/FastDub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18202 2023-05-24 08:53:30.862236 FastDub-3.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    10519 2023-05-24 08:29:39.000000 FastDub-3.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.839062 FastDub-3.7.0/fastdub/
--rw-rw-rw-   0        0        0      981 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/__init__.py
--rw-rw-rw-   0        0        0    13306 2023-05-24 08:35:24.000000 FastDub-3.7.0/fastdub/__main__.py
--rw-rw-rw-   0        0        0     2779 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/audio.py
--rw-rw-rw-   0        0        0     7132 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/dubber.py
--rw-rw-rw-   0        0        0     4226 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/ffmpeg_wrapper.py
--rw-rw-rw-   0        0        0     3038 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.846583 FastDub-3.7.0/fastdub/translator/
--rw-rw-rw-   0        0        0      605 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/translator/__init__.py
--rw-rw-rw-   0        0        0     2015 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/translator/subs_translate.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.846583 FastDub-3.7.0/fastdub/utils/
--rw-rw-rw-   0        0        0       84 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/utils/__init__.py
--rw-rw-rw-   0        0        0      968 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/utils/json2srt.py
--rw-rw-rw-   0        0        0     2644 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/voicer.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.846583 FastDub-3.7.0/fastdub/youtube/
--rw-rw-rw-   0        0        0      402 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/__init__.py
--rw-rw-rw-   0        0        0     5895 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.846583 FastDub-3.7.0/fastdub/youtube/pafy/
--rw-rw-rw-   0        0        0      371 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/__init__.py
--rw-rw-rw-   0        0        0    16042 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/backend_internal.py
--rw-rw-rw-   0        0        0    23099 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/backend_shared.py
--rw-rw-rw-   0        0        0     7231 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/backend_youtube_dl.py
--rw-rw-rw-   0        0        0     7957 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/channel.py
--rw-rw-rw-   0        0        0     3880 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/g.py
--rw-rw-rw-   0        0        0    10071 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/jsinterp.py
--rw-rw-rw-   0        0        0     6229 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/pafy.py
--rw-rw-rw-   0        0        0    10668 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/playlist.py
--rw-rw-rw-   0        0        0     1404 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/pafy/util.py
--rw-rw-rw-   0        0        0     1953 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:53:30.862236 FastDub-3.7.0/fastdub/youtube/yt_upload/
--rw-rw-rw-   0        0        0      210 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/yt_upload/__init__.py
--rw-rw-rw-   0        0        0     6664 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/yt_upload/upload_video.py
--rw-rw-rw-   0        0        0     1809 2023-05-24 08:29:39.000000 FastDub-3.7.0/fastdub/youtube/yt_upload/uploader.py
--rw-rw-rw-   0        0        0       42 2023-05-24 08:53:30.866528 FastDub-3.7.0/setup.cfg
--rw-rw-rw-   0        0        0     3167 2023-05-24 08:46:21.000000 FastDub-3.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.886432 FastDub-3.8.0/
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.866318 FastDub-3.8.0/FastDub.egg-info/
+-rw-rw-rw-   0        0        0    15519 2023-07-29 13:18:03.000000 FastDub-3.8.0/FastDub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2023-07-29 13:18:03.000000 FastDub-3.8.0/FastDub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 13:18:03.000000 FastDub-3.8.0/FastDub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      318 2023-07-29 13:18:03.000000 FastDub-3.8.0/FastDub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 13:18:03.000000 FastDub-3.8.0/FastDub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15519 2023-07-29 13:18:03.886432 FastDub-3.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9114 2023-07-29 12:15:06.000000 FastDub-3.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.883027 FastDub-3.8.0/fastdub/
+-rw-rw-rw-   0        0        0    10096 2023-07-29 12:21:11.000000 FastDub-3.8.0/fastdub/__init__.py
+-rw-rw-rw-   0        0        0    13306 2023-07-29 11:30:57.000000 FastDub-3.8.0/fastdub/__main__.py
+-rw-rw-rw-   0        0        0     2779 2023-07-29 11:30:57.000000 FastDub-3.8.0/fastdub/audio.py
+-rw-rw-rw-   0        0        0     7113 2023-07-29 12:27:49.000000 FastDub-3.8.0/fastdub/dubber.py
+-rw-rw-rw-   0        0        0     4226 2023-07-29 11:30:57.000000 FastDub-3.8.0/fastdub/ffmpeg_wrapper.py
+-rw-rw-rw-   0        0        0     3038 2023-07-29 11:30:57.000000 FastDub-3.8.0/fastdub/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.885878 FastDub-3.8.0/fastdub/translator/
+-rw-rw-rw-   0        0        0      591 2023-07-29 12:20:37.000000 FastDub-3.8.0/fastdub/translator/__init__.py
+-rw-rw-rw-   0        0        0     2015 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/translator/subs_translate.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.886432 FastDub-3.8.0/fastdub/utils/
+-rw-rw-rw-   0        0        0       84 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/utils/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/utils/json2srt.py
+-rw-rw-rw-   0        0        0     2644 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/voicer.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.886432 FastDub-3.8.0/fastdub/youtube/
+-rw-rw-rw-   0        0        0      388 2023-07-29 12:26:20.000000 FastDub-3.8.0/fastdub/youtube/__init__.py
+-rw-rw-rw-   0        0        0     6006 2023-07-29 12:54:59.000000 FastDub-3.8.0/fastdub/youtube/downloader.py
+-rw-rw-rw-   0        0        0     1948 2023-07-29 12:50:01.000000 FastDub-3.8.0/fastdub/youtube/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:03.886432 FastDub-3.8.0/fastdub/youtube/yt_upload/
+-rw-rw-rw-   0        0        0      210 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/youtube/yt_upload/__init__.py
+-rw-rw-rw-   0        0        0     6664 2023-05-24 08:29:39.000000 FastDub-3.8.0/fastdub/youtube/yt_upload/upload_video.py
+-rw-rw-rw-   0        0        0     1823 2023-07-29 12:50:01.000000 FastDub-3.8.0/fastdub/youtube/yt_upload/uploader.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 13:18:03.897936 FastDub-3.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3167 2023-07-29 12:55:27.000000 FastDub-3.8.0/setup.py
```

### Comparing `FastDub-3.7.0/README.md` & `FastDub-3.8.0/fastdub/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""# FastDub
+
 Package for voice over subtitles:
 
 * with the ability to embed in video,
 * audio ducking,
 * dynamic voice changer for a single track. _Add **--voice-set-anchor** at the beginning of the subtitle line. (Applies
   to
   all
@@ -11,15 +13,15 @@
 
 ---
 
 # Install for Ubuntu
 
 > sudo apt update -y && sudo apt upgrade -y
 >
-> sudo apt install python3 python3-pip ffmpeg [espeak](http://espeak.sourceforge.net/data/) libxml2-dev libxslt1-dev
+> sudo apt install python3 python3-pip ffmpeg [espeak](https://espeak.sourceforge.net/data/) libxml2-dev libxslt1-dev
 >
 > ; libxml for translator functions
 >
 > sudo python3 -m pip install -U pip setuptools wheel
 >
 > sudo python3 -m pip install -U [FastDub](https://pypi.org/project/FastDub/)
 
@@ -80,41 +82,40 @@
 
 # Usage
 
 > python -m fastdub --help
 
 ```
 usage: fastdub [-h] [-rc {0,1,2}] [-ra | --cleanup-audio | -n-ra | --no-cleanup-audio] [-ev | --export-video | -n-ev | --no-export-video]
-               [-l LANGUAGE] [-tc THREADS_COUNT] -i INPUT [-vf VIDEO_FORMAT] [-sf SUBTITLES_FORMAT] [-En EXCLUDE [EXCLUDE ...]]
-               [-Eu EXCLUDE_UNDERSCORE] [-sc | --sidechain | -n-sc | --no-sidechain] [-sc-args SIDECHAIN_FFMPEG_PARAMS]
-               [-sc-lvl SIDECHAIN_LEVEL_SC]
-               [-v {microsoft irina desktop - russian,microsoft zira desktop - english united states),microsoft david desktop - english (united s
-tates,aleksandr-hq,arina,artemiy,evgeniy-eng,evgeniy-rus,lyubov,marianna,mikhail,pavel,tatiana,victoria,vitaliy,volodymyr,vsevolod,yuriy}]       
-               [-a ALIGN] [-v-set-a VOICE_SET_ANCHOR] [-ll {trace,debug,verbose,info,warning,error,fatal,panic,quiet}]
-               [-y | --confirm | -n-y | --no-confirm] [-af AUDIO_FORMAT] [-wm WATERMARK] [-tb | --traceback | -n-tb | --no-traceback] [-yt]      
+               [-l LANGUAGE] [-ll {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}] [-tc THREADS_COUNT] -i INPUT [-vf VIDEO_FORMAT]
+               [-sf SUBTITLES_FORMAT] [-En EXCLUDE [EXCLUDE ...]] [-Eu EXCLUDE_UNDERSCORE] [-sc | --sidechain | -n-sc | --no-sidechain]
+               [-sc-args SIDECHAIN_FFMPEG_PARAMS] [-sc-lvl SIDECHAIN_LEVEL_SC]
+               [-v {...}]
+               [-a ALIGN] [-v-set-a VOICE_SET_ANCHOR] [-fll {trace,debug,verbose,info,warning,error,fatal,panic,quiet}]
+               [-y | --confirm | -n-y | --no-confirm] [-af AUDIO_FORMAT] [-wm WATERMARK] [-tb | --traceback | -n-tb | --no-traceback] [-yt]
                [-ak API_KEYS [API_KEYS ...]] [-yts] [-yts-l YOUTUBE_SEARCH_LIMIT] [-yts-rg YOUTUBE_SEARCH_REGION] [-ytu]
                [-ytu-ps {private,public,unlisted}] [-ytu-t] [-tr] [--rewrite-srt | --no-rewrite-srt]
-               [-ts {alibaba,apertium,argos,baidu,bing,caiyun,cloudYi,deepl,elia,google,iciba,iflytek,iflyrec,itranslate,judic,languageWire,lingv
-anex,niutrans,mglip,modernMt,myMemory,papago,qqFanyi,qqTranSmart,reverso,sogou,sysTran,tilde,translateCom,translateMe,utibet,volcEngine,yandex,ye
-ekit,youdao}]
+               [-ts {...}]
 
 fastdub is a tool for dubbing videos by subtitle files.
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -rc {0,1,2}, --remove-cache {0,1,2}
                         Remove all cache (_cached_texts directory) files
                                 0 - No remove cache
                                 1 - Delete cache before voice acting
                                 2 - Delete cache after voice acting (default)
   -ra, --cleanup-audio, -n-ra, --no-cleanup-audio
                         Remove result audio if video exists (default True) (default: True)
   -ev, --export-video, -n-ev, --no-export-video
   -l LANGUAGE, --language LANGUAGE
                         Subtitles language (ru)
+  -ll {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}, --loglevel {CRITICAL,FATAL,ERROR,WARN,WARNING,INFO,DEBUG,NOTSET}
+                        Program log level
   -tc THREADS_COUNT, --threads-count THREADS_COUNT
                         Process count to download (pass to cpu count, < 2 to disable)
                                 *N = N * cpu count
 
 Input:
   -i INPUT, --input INPUT
                         Input directory/YouTube Playlist/Video URL.
@@ -129,34 +130,31 @@
   -Eu EXCLUDE_UNDERSCORE, --exclude-underscore EXCLUDE_UNDERSCORE
                         Exclude files starts with underscore
 
 Audio Ducking:
   -sc, --sidechain, -n-sc, --no-sidechain
                         Enable audio side chain compress (ducking) (default: True)
   -sc-args SIDECHAIN_FFMPEG_PARAMS, --sidechain-ffmpeg-params SIDECHAIN_FFMPEG_PARAMS
-                        sidechain FFMpeg parameters (default '')
+                        sidechain FFmpeg parameters (default '')
   -sc-lvl SIDECHAIN_LEVEL_SC, --sidechain-level-sc SIDECHAIN_LEVEL_SC
                         Set sidechain gain. Range is between 0.015625 and 64. (default 0.8)
 
 Voicer:
-  -v {microsoft irina desktop - russian,microsoft zira desktop - english (united states),microsoft david desktop - english (united states),aleksa
-ndr-hq,arina,artemiy,evgeniy-eng,evgeniy-rus,lyubov,marianna,mikhail,pavel,tatiana,victoria,vitaliy,volodymyr,vsevolod,yuriy}, --voice {microsoft
- irina desktop - russian,microsoft zira desktop - english (united states),microsoft david desktop - english (united states),aleksandr-hq,arina,ar
-temiy,evgeniy-eng,evgeniy-rus,lyubov,marianna,mikhail,pavel,tatiana,victoria,vitaliy,volodymyr,vsevolod,yuriy}
+  -v {...}, --voice {...}
                         SAPI voice for voice acting.
   -a ALIGN, --align ALIGN
                         Audio fit align (divisor)
                                 1 = right
                                 2 = center (default)
   -v-set-a VOICE_SET_ANCHOR, --voice-set-anchor VOICE_SET_ANCHOR
                         Anchor indicating voice actor change (default "!:")
 
-FFMpeg Output:
-  -ll {trace,debug,verbose,info,warning,error,fatal,panic,quiet}, --loglevel {trace,debug,verbose,info,warning,error,fatal,panic,quiet}
-                        FFMpegWrapper loglevel
+FFmpeg Output:
+  -fll {trace,debug,verbose,info,warning,error,fatal,panic,quiet}, --ffmpeg-loglevel {trace,debug,verbose,info,warning,error,fatal,panic,quiet}
+                        FFmpegWrapper loglevel
   -y, --confirm, -n-y, --no-confirm
                         Don't ask for confirmation (default: True)
   -af AUDIO_FORMAT, --audio-format AUDIO_FORMAT
                         Out audio files format (default wav)
   -wm WATERMARK, --watermark WATERMARK
                         Add watermark to output video
 
@@ -186,19 +184,15 @@
                         Translate title and description on upload. (+ Arguments from translate argument group)
 
 Translate:
   -tr, --translate      Translate input subtitles files
   --rewrite-srt, --no-rewrite-srt
                         Rewrite input subtitles files.
                         If not, add "_" to the beginning of the original subtitle file. (default: False)
-  -ts {alibaba,apertium,argos,baidu,bing,caiyun,cloudYi,deepl,elia,google,iciba,iflytek,iflyrec,itranslate,judic,languageWire,lingvanex,niutrans,
-mglip,modernMt,myMemory,papago,qqFanyi,qqTranSmart,reverso,sogou,sysTran,tilde,translateCom,translateMe,utibet,volcEngine,yandex,yeekit,youdao}, 
---translate-service {alibaba,apertium,argos,baidu,bing,caiyun,cloudYi,deepl,elia,google,iciba,iflytek,iflyrec,itranslate,judic,languageWire,lingv
-anex,niutrans,mglip,modernMt,myMemory,papago,qqFanyi,qqTranSmart,reverso,sogou,sysTran,tilde,translateCom,translateMe,utibet,volcEngine,yandex,ye
-ekit,youdao}
+  -ts {...}, --translate-service {...}
                         Subtitle translation service. (default google)
 ```
 
 **If the voice set after "!:" is not selected during voiceover, clear the cache with the -rc argument**
 
 ## Example
 
@@ -228,10 +222,44 @@
 
 Default service is Google.
 
 ## Other
 
 ### The `fastdub.utils` module stores helper functions.
 
-### python -m pydoc -w fastdub
-
 ### You can write your issues on [GitHub](https://github.com/NIKDISSV-Forever/fastdub/issues) in English or in Russian.
+"""
+from __future__ import annotations
+
+from multiprocessing import cpu_count
+
+__all__ = ('PrettyViewPrefix', 'GlobalSettings')
+__author__ = 'NIKDISSV'
+
+
+class GlobalSettings:
+    __slots__ = ()
+    threads_count = cpu_count()
+    language = 'ru'
+    watermark = ''
+    tqdm_kwargs = {'dynamic_ncols': True}
+
+
+class PrettyViewPrefix:
+    """Class for representing a number as units"""
+    __slots__ = ()
+
+    @staticmethod
+    def from_any(size: float, div: float, base: str, prefixes) -> str:
+        for prefix in prefixes[:-1]:
+            if size < div:
+                return f'{size:,g}{prefix}{base}'
+            size /= div
+        return f'{size:,g}{prefixes[-1]}{base}'
+
+    @classmethod
+    def from_bytes(cls, size: float) -> str:
+        return cls.from_any(size, 1000., 'B', ('', 'k', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y'))
+
+    @classmethod
+    def from_seconds(cls, size: float) -> str:
+        return cls.from_any(size, 60., '', 'smh')
```

### Comparing `FastDub-3.7.0/fastdub/__main__.py` & `FastDub-3.8.0/fastdub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import getcwd
 from time import perf_counter
 
 import rich.traceback
 
 import fastdub.youtube
 from fastdub import GlobalSettings, PrettyViewPrefix, dubber, translator, voicer, youtube
-from fastdub.ffmpeg_wrapper import DefaultFFMpegParams
+from fastdub.ffmpeg_wrapper import DefaultFFmpegParams
 from fastdub.translator.subs_translate import SrtTranslate
 
 __all__ = ('parse_args', 'main')
 THREADS_MAY_NEED = youtube.SUPPORTED or translator.SUPPORTED
 
 if hasattr(logging, '_nameToLevel'):
     def _get_logging_level_names() -> tuple[str]:
@@ -96,34 +96,34 @@
                                      help='Exclude <name> (glob)')
     exclude_input_group.add_argument('-Eu', '--exclude-underscore', default=True,
                                      help='Exclude files starts with underscore')
 
     ducking_group = arg_parser.add_argument_group('Audio Ducking')
     ducking_group.add_argument('-sc', '--sidechain', action=BooleanOptionalAction, default=True,
                                help='Enable audio side chain compress (ducking)')
-    ducking_group.add_argument('-sc-args', '--sidechain-ffmpeg-params', default=DefaultFFMpegParams.sidechain_args,
-                               help=f'sidechain FFMpeg parameters (default {DefaultFFMpegParams.sidechain_args!r})')
+    ducking_group.add_argument('-sc-args', '--sidechain-ffmpeg-params', default=DefaultFFmpegParams.sidechain_args,
+                               help=f'sidechain FFmpeg parameters (default {DefaultFFmpegParams.sidechain_args!r})')
     ducking_group.add_argument('-sc-lvl', '--sidechain-level-sc', type=float, default=.8,
                                help='Set sidechain gain. Range is between 0.015625 and 64. (default 0.8)')
 
     voicer_group = arg_parser.add_argument_group('Voicer')
     voicer_group.add_argument('-v', '--voice', type=str.lower, choices=voicer.VOICES_NAMES.keys(),
                               help='SAPI voice for voice acting.')
     voicer_group.add_argument('-a', '--align', default=2., type=float,
                               help='Audio fit align (divisor)'
                                    '\n\t1 = right'
                                    '\n\t2 = center (default)')
     voicer_group.add_argument('-v-set-a', '--voice-set-anchor', default='!:',
                               help='Anchor indicating voice actor change (default "!:")')
 
-    ffmpeg_group = arg_parser.add_argument_group('FFMpeg Output')
+    ffmpeg_group = arg_parser.add_argument_group('FFmpeg Output')
     ffmpeg_group.add_argument('-fll', '--ffmpeg-loglevel', default='panic',
                               choices=(
                                   'trace', 'debug', 'verbose', 'info', 'warning', 'error', 'fatal', 'panic', 'quiet'),
-                              help='FFMpegWrapper loglevel')
+                              help='FFmpegWrapper loglevel')
     ffmpeg_group.add_argument('-y', '--confirm', action=BooleanOptionalAction, default=True,
                               help="Don't ask for confirmation")
     ffmpeg_group.add_argument('-af', '--audio-format', default='wav',
                               help='Out audio files format (default wav)')
     ffmpeg_group.add_argument('-wm', '--watermark', default='',
                               help='Add watermark to output video')
 
@@ -188,19 +188,19 @@
     logging.getLogger().setLevel(args.loglevel)
 
     remove_cache = args.remove_cache
     if remove_cache == 1:
         dubber.VOICER.cleanup()
 
     GlobalSettings.watermark = args.watermark
-    DefaultFFMpegParams.ffmpeg_log_level = args.ffmpeg_loglevel
+    DefaultFFmpegParams.ffmpeg_log_level = args.ffmpeg_loglevel
 
     total_time = 0
     if args.confirm:
-        DefaultFFMpegParams.args += '-y',
+        DefaultFFmpegParams.args += '-y',
         total_time = perf_counter()
 
     if THREADS_MAY_NEED:
         GlobalSettings.threads_count = args.threads_count
 
     if youtube.SUPPORTED and args.youtube:
         query: str = args.input
```

### Comparing `FastDub-3.7.0/fastdub/audio.py` & `FastDub-3.8.0/fastdub/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 import os.path
 from copy import copy
 from tempfile import TemporaryDirectory
 
 import pydub.silence
 
-from fastdub.ffmpeg_wrapper import FFMpegWrapper
+from fastdub.ffmpeg_wrapper import FFmpegWrapper
 
 __all__ = ('AudioSegment',
            'speed_change', 'calc_speed_change_ffmpeg_arg',
            'fit')
 
 
 class AudioSegment(pydub.AudioSegment):
@@ -37,24 +37,24 @@
                          "This is usually due to errors in subtitle timecodes.")
     if speed_changes == 1:
         return audio if allow_copy else copy(audio)
     with TemporaryDirectory() as tmp:
         inp = os.path.join(tmp, 'inp.wav')
         audio.export(inp)
         out = os.path.join(tmp, 'out.wav')
-        FFMpegWrapper.convert('-i', inp,
+        FFmpegWrapper.convert('-i', inp,
                               '-af', calc_speed_change_ffmpeg_arg(speed_changes),
                               out, loglevel=log_level)
         return AudioSegment.from_file(out)
 
 
 def calc_speed_change_ffmpeg_arg(speed_changes: float) -> str:
     """
     The given function takes in a float value representing the speed change
-    and returns a corresponding FFMpeg argument string for changing the speed of an audio or video file.
+    and returns a corresponding FFmpeg argument string for changing the speed of an audio or video file.
     """
     if .5 <= speed_changes <= 100.:
         return f'atempo={speed_changes}'
     if .25 <= speed_changes <= 10_000.:
         return f'atempo=sqrt({speed_changes}),atempo=sqrt({speed_changes})'
     power = math.ceil(math.log(speed_changes, .5 if speed_changes < .5 else 100.))
     return (f'atempo={speed_changes}^(1/{power}),' * power)[:-1]
```

### Comparing `FastDub-3.7.0/fastdub/dubber.py` & `FastDub-3.8.0/fastdub/dubber.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import logging
 import os.path
 import shutil
 from pathlib import Path
 from typing import Sequence
 
-import rich.align
 from tqdm import tqdm
 
 from fastdub import audio, subtitles, voicer, GlobalSettings
 from fastdub.audio import AudioSegment, calc_speed_change_ffmpeg_arg
-from fastdub.ffmpeg_wrapper import FFMpegWrapper
+from fastdub.ffmpeg_wrapper import FFmpegWrapper
 
 __all__ = ('Dubber', 'VOICER')
 
 from fastdub.subtitles import Line, TimeLabel
 
 VOICER = voicer.Voicer()
 
@@ -78,15 +77,15 @@
         result_dir = Path(target_sub).parent / '_result'
         result_dir.mkdir(exist_ok=True)
         out_audio_base = result_dir / f'{fn}_{self.language}.{self.audio_format}'
 
         subs = subtitles.parse(target_sub)
         default_right_border = 0
         if target_vid and subs:
-            default_right_border = FFMpegWrapper.get_video_duration_ms(target_vid)
+            default_right_border = FFmpegWrapper.get_video_duration_ms(target_vid)
         default_right_border = max(default_right_border, end := subs[-1].ms.end)
         subs += Line(TimeLabel(default_right_border, end, end - default_right_border)),
 
         progress_total = len(subs) - 1
 
         fit_align = self.fit_align
         audio_format = self.audio_format
@@ -129,39 +128,39 @@
             logging.info(f'changing audio speed {change_speed:g}')
             ffmpeg_concat_args += '-af', calc_speed_change_ffmpeg_arg(change_speed)
         else:
             ffmpeg_concat_args += '-c', 'copy'
 
         temp_audio_file = str(out_audio_base.with_stem(f'_{out_audio_base.stem}'))
         logging.info('concatenating parts...')
-        FFMpegWrapper.convert('-f', 'concat', '-safe', '0', '-i', list_file, *ffmpeg_concat_args,
+        FFmpegWrapper.convert('-f', 'concat', '-safe', '0', '-i', list_file, *ffmpeg_concat_args,
                               temp_audio_file)
         cur_audio = audio.AudioSegment.from_file(temp_audio_file)
         shutil.rmtree(working_dir, ignore_errors=True)
 
         if total_duration_ms != max_duration:
             cur_audio = audio.AudioSegment.silent(
                 min(max_duration - total_duration_ms, subs[0].ms.start)
             ) + cur_audio
 
         result_out_audio = str(out_audio_base)
         if target_vid:
             cur_audio.export(temp_audio_file, format='wav')
             if self.ducking:
                 logging.info('sidechain')
-                FFMpegWrapper.sidechain(target_vid,
+                FFmpegWrapper.sidechain(target_vid,
                                         temp_audio_file,
                                         result_out_audio,
                                         self.sidechain_level_sc,
                                         self.sidechain_ffmpeg_params)
             else:
                 logging.info('amix')
-                FFMpegWrapper.amix(target_vid, temp_audio_file, out=result_out_audio)
+                FFmpegWrapper.amix(target_vid, temp_audio_file, out=result_out_audio)
                 # audio.AudioSegment.from_file(target_vid).overlay(cur_audio).export(result_out_audio)
             if export_video:
-                FFMpegWrapper.save_result_data(target_vid, result_out_audio, target_sub,
+                FFmpegWrapper.save_result_data(target_vid, result_out_audio, target_sub,
                                                result_dir / f'{fn}_{self.language}.mkv')
                 if cleanup_audio:
                     os.remove(result_out_audio)
         else:
             cur_audio.export(result_out_audio)
         os.remove(temp_audio_file)
```

### Comparing `FastDub-3.7.0/fastdub/ffmpeg_wrapper.py` & `FastDub-3.8.0/fastdub/ffmpeg_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import re
 import sys
 from pathlib import Path
 from subprocess import check_call, getoutput
 
 from fastdub import GlobalSettings
 
-__all__ = ('FFMpegWrapper', 'DefaultFFMpegParams')
+__all__ = ('FFmpegWrapper', 'DefaultFFmpegParams')
 
 
-class DefaultFFMpegParams:
+class DefaultFFmpegParams:
     __slots__ = ()
     ffmpeg_log_level = 'panic'
     args = ()
     sidechain_args = ''
     executable = 'ffmpeg'
 
 
@@ -36,32 +36,32 @@
             for walkfilename in walkfilenames:
                 walkfilename = Path(walkfilename)
                 if walkfilename.suffix == '.ttf':
                     return f":fontfile='{Path(walkroot, walkfilename)}'"
     return ''
 
 
-class FFMpegWrapper:
+class FFmpegWrapper:
     __slots__ = ()
     DURATION_RE = re.compile(r'Duration: (\d\d):(\d\d):(\d\d\.\d\d)')
 
     @classmethod
     def convert(cls, *args, loglevel=None) -> int:
         if not loglevel:
-            loglevel = DefaultFFMpegParams.ffmpeg_log_level
+            loglevel = DefaultFFmpegParams.ffmpeg_log_level
         return check_call(
-            [str(i) for i in (DefaultFFMpegParams.executable, '-v', loglevel, *DefaultFFMpegParams.args, *args)])
+            [str(i) for i in (DefaultFFmpegParams.executable, '-v', loglevel, *DefaultFFmpegParams.args, *args)])
 
     @classmethod
     def get_video_duration_ms(cls, video_path: str | Path) -> float:
         return cls.get_video_duration_s(video_path) * 1000.
 
     @classmethod
     def get_video_duration_s(cls, video_path: str | Path) -> float:
-        found = cls.DURATION_RE.search(getoutput(f'{DefaultFFMpegParams.executable} -i {video_path}'))
+        found = cls.DURATION_RE.search(getoutput(f'{DefaultFFmpegParams.executable} -i {video_path}'))
         if not found:
             return 0.
         groups = found.groups()
         return float(groups[0]) * 3600. + float(groups[1]) * 60. + float(groups[2])
 
     @classmethod
     def save_result_data(cls, video_path, audio_path, subtitles_path, output_path):
@@ -91,15 +91,15 @@
                 ":fontcolor=white@0.5:box=1:boxcolor=black@0.5"
                 ":x='mod(n,w-text_w)':y='mod(n,h-text_h)'")
 
     @classmethod
     def sidechain(cls, background: str, foreground: str, out: str,
                   level_sc: float = 0.8, params: str = None):
         if params is None:
-            params = DefaultFFMpegParams.sidechain_args
+            params = DefaultFFmpegParams.sidechain_args
         return cls.convert('-i', background, '-i', foreground,
                            '-filter_complex',
                            '[1:a]asplit=2[sc][mix];'
                            f'[0:a][sc]sidechaincompress=level_sc={level_sc}:{params}[compr];'
                            '[compr][mix]amix',
                            out)
```

### Comparing `FastDub-3.7.0/fastdub/subtitles.py` & `FastDub-3.8.0/fastdub/subtitles.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import os.path
 import re
 from typing import NamedTuple
 
 from chardet import detect as detect_encoding
 
-from fastdub.ffmpeg_wrapper import FFMpegWrapper
+from fastdub.ffmpeg_wrapper import FFmpegWrapper
 
 __all__ = ('LINE_REGEX',
            'Line', 'TimeLabel',
            'parse', 'unparse',
            'ms_to_srt_time')
 
 LINE_REGEX = re.compile(r'\n\n^\d+$\n', re.M)
@@ -69,15 +69,15 @@
 
 
 def parse(text_or_file: str, skip_empty: bool = False) -> tuple[Line] | tuple:
     if os.path.isfile(text_or_file):
         fn, ext = os.path.splitext(text_or_file)
         if ext != '.srt':
             converted = f'{fn}.srt'
-            FFMpegWrapper.convert('-i', text_or_file, converted)
+            FFmpegWrapper.convert('-i', text_or_file, converted)
             text_or_file = converted
         text = _read_file(text_or_file)
     else:
         text = text_or_file
     subtitles = ()
     for i in LINE_REGEX.split(f'\n\n{text.lstrip()}')[1:]:
         times_text: list[str, str] = i.split('\n', 1)
```

### Comparing `FastDub-3.7.0/fastdub/translator/__init__.py` & `FastDub-3.8.0/fastdub/translator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import sys
 from typing import Callable
 
-__all__ = ('SUPPORTED',)
+__all__ = ('SUPPORTED', 'get_service_by_name')
 
 try:
     from translators import server
     from fastdub.translator import subs_translate
 
     SERVICES = *server.tss.translators_dict.keys(),
-
-
-    def get_service_by_name(service: str) -> Callable:
-        return server.tss.translators_dict[service]
 except Exception as e:
     SUPPORTED = False
     if not isinstance(e, ImportError):
         sys.stderr.write(str(e))
 else:
     SUPPORTED = True
-    __all__ += ('translators', 'SERVICES', 'get_service_by_name', 'subs_translate')
+    __all__ += ('server', 'SERVICES', 'subs_translate')
+
+
+def get_service_by_name(service: str) -> Callable:
+    return server.tss.translators_dict[service]
```

### Comparing `FastDub-3.7.0/fastdub/translator/subs_translate.py` & `FastDub-3.8.0/fastdub/translator/subs_translate.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.7.0/fastdub/utils/json2srt.py` & `FastDub-3.8.0/fastdub/utils/json2srt.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.7.0/fastdub/voicer.py` & `FastDub-3.8.0/fastdub/voicer.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.7.0/fastdub/youtube/downloader.py` & `FastDub-3.8.0/fastdub/youtube/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
+import logging
 import multiprocessing.pool
 import re
 from pathlib import Path
 from typing import Callable, Optional, TypeVar
 from urllib.parse import urlparse
 
+import pafy
 import rich.live
 import rich.table
+from pafy import g as pafy_g
 from tqdm import tqdm
 from youtubesearchpython import VideosSearch
 
 from fastdub import GlobalSettings, PrettyViewPrefix
 from fastdub.youtube import *
-from fastdub.youtube import pafy
-from fastdub.youtube.pafy import g as pafy_g
 from fastdub.youtube.subtitles import download_srt
 
 __all__ = ('DownloadYTVideo', 'with_api_key')
 
 _API_RET_TYPE = TypeVar('_API_RET_TYPE')
 _PATH_SUPPORTED = re.compile(r'[\\/:?"<>|]+')
 
@@ -76,21 +77,25 @@
         if len(title) <= (97 - len(yt_dl.videoid)):
             title += f' [{yt_dl.videoid}]'
         save_to = self.save_dir / title
 
         _file = Path(save_to)
         srt_file = _file.with_suffix('.srt')
         if not srt_file.is_file():
-            download_srt(yt_dl.videoid, self.language, srt_file)
+            try:
+                download_srt(yt_dl.videoid, self.language, srt_file)
+            except KeyError as e:
+                logging.error(e)
+                return
         mp4_file = _file.with_suffix('.mp4')
         if not mp4_file.is_file():
             try:
                 with_api_key(self.mp4_downloader(yt_dl, mp4_file))
-            except OSError:
-                pass
+            except OSError as e:
+                logging.error(e)
 
     def mp4_downloader(self, yt_dl: YtdlPafy, mp4_file: str | Path):
         mp4_file = str(mp4_file)
         return lambda: yt_dl.getbest('mp4').download(mp4_file,
                                                      quiet=True,
                                                      callback=lambda *args: self.progress_callback(mp4_file, *args))
```

### Comparing `FastDub-3.7.0/fastdub/youtube/subtitles.py` & `FastDub-3.8.0/fastdub/youtube/subtitles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+import logging
 import time
 from math import modf
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Iterable
 
 import download_youtube_subtitle.main as down_yt_subs
@@ -12,16 +13,16 @@
 __all__ = ('download_srt',)
 
 
 def find_caption_num(video_id: str, lang_code: str) -> int | None:
     video_id = down_yt_subs.parseVideoID(video_id)[0]
     try:
         caption_tracks = down_yt_subs.get_tracks_title(video_id)[0]
-    except Exception:
-        down_yt_subs.perr("can't retrive caption")
+    except Exception as e:
+        logging.error(e)
         raise
     for i, caption in enumerate(caption_tracks):
         if caption.get('languageCode') == lang_code:
             return i
 
 
 subs_download = down_yt_subs.main
```

### Comparing `FastDub-3.7.0/fastdub/youtube/yt_upload/upload_video.py` & `FastDub-3.8.0/fastdub/youtube/yt_upload/upload_video.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.7.0/fastdub/youtube/yt_upload/uploader.py` & `FastDub-3.8.0/fastdub/youtube/yt_upload/uploader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
 from pathlib import Path
 from typing import Callable
 
-from fastdub.youtube import pafy
+import pafy
+
 from fastdub.youtube.downloader import with_api_key
 from fastdub.youtube.yt_upload.upload_video import upload
 
 
 class Uploader:
     def __init__(self,
                  privacy_status: str = 'private',
@@ -23,16 +25,16 @@
                 return self.translate(text, lang)
 
             title = f'{name} - {lang}'
             description = category = keywords = None
             ytdl = None
             try:
                 ytdl = with_api_key(lambda: pafy.new(name))
-            except (OSError, ValueError):
-                pass
+            except (OSError, ValueError) as e:
+                logging.error(e)
             if ytdl:
                 title = ytdl.title
                 description = ytdl.description
                 keywords = ytdl.keywords
             command = ('--file', str(fp), '--title', translate(title),
                        '--privacy-status', self.privacy, '--noauth_local_webserver')
             if description:
```

### Comparing `FastDub-3.7.0/setup.py` & `FastDub-3.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 for require in Path('extra_requires').glob('*_*.txt'):
     with open(require, encoding='UTF-8') as f:
         extras_require[require.name.split('.', 1)[0].rsplit('_', 1)[-1].casefold()] = f.read().strip().splitlines()
 extras_require['all'] = sum(extras_require.values(), requires)
 
 setuptools.setup(
     name="FastDub",
-    version="3.7.0",
+    version="3.8.0",
 
     description="A Python CLI package "
                 "for voice over subtitles, with the ability to embed in video, audio ducking, "
                 "and dynamic voice changer for a single track; "
                 "auto translating; "
                 "download and upload to YouTube supports",
```

