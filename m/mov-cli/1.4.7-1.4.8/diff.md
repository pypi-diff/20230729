# Comparing `tmp/mov_cli-1.4.7.tar.gz` & `tmp/mov_cli-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.7.tar", max compression
+gzip compressed data, was "mov_cli-1.4.8.tar", max compression
```

## Comparing `mov_cli-1.4.7.tar` & `mov_cli-1.4.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2023-07-25 17:14:27.983137 mov_cli-1.4.7/LICENSE
--rw-r--r--   0        0        0     6540 2023-07-25 17:14:27.983137 mov_cli-1.4.7/README.md
--rw-r--r--   0        0        0      687 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/__init__.py
--rw-r--r--   0        0        0      810 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      906 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0      341 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/extractors/tukipasti.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     3128 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     2772 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0      356 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ar.json
--rw-r--r--   0        0        0      356 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/de.json
--rw-r--r--   0        0        0      309 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/en.json
--rw-r--r--   0        0        0      348 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/fr.json
--rw-r--r--   0        0        0      338 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ko.json
--rw-r--r--   0        0        0      194 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/langs
--rw-r--r--   0        0        0      308 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/pl.json
--rw-r--r--   0        0        0      289 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/pt.json
--rw-r--r--   0        0        0      418 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ru.json
--rw-r--r--   0        0        0      660 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang/ta.json
--rw-r--r--   0        0        0     1273 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1563 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/player.py
--rw-r--r--   0        0        0     1278 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/props.py
--rw-r--r--   0        0        0     7472 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0     4900 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/utils/select.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/anime/__init__.py
--rw-r--r--   0        0        0     3274 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/anime/gogoanime.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/viewasian.py
--rw-r--r--   0        0        0     3382 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/asian/watchasian.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/cartoons/__init__.py
--rw-r--r--   0        0        0     3544 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/cartoons/kisscartoon.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/__init__.py
--rw-r--r--   0        0        0     6931 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/actvid.py
--rw-r--r--   0        0        0     3274 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/dopebox.py
--rw-r--r--   0        0        0     4242 2023-07-25 17:14:27.983137 mov_cli-1.4.7/mov_cli/websites/english/remotestream.py
--rw-r--r--   0        0        0     3273 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/english/sflix.py
--rw-r--r--   0        0        0     1055 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/english/solar.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/__init__.py
--rw-r--r--   0        0        0     1943 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/einthusan.py
--rw-r--r--   0        0        0     2165 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/indian/tamilyogi.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/international/__init__.py
--rw-r--r--   0        0        0     3950 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/international/wlext.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/livetv/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/livetv/eja.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/sports/__init__.py
--rw-r--r--   0        0        0     4474 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/sports/scdn.py
--rw-r--r--   0        0        0        0 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/__init__.py
--rw-r--r--   0        0        0     2318 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/turkish123.py
--rw-r--r--   0        0        0     2909 2023-07-25 17:14:27.987137 mov_cli-1.4.7/mov_cli/websites/turkish/yoturkish.py
--rw-r--r--   0        0        0      736 2023-07-25 17:14:27.987137 mov_cli-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     7529 1970-01-01 00:00:00.000000 mov_cli-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-29 02:30:28.709043 mov_cli-1.4.8/LICENSE
+-rw-r--r--   0        0        0     6568 2023-07-29 02:30:28.709043 mov_cli-1.4.8/README.md
+-rw-r--r--   0        0        0      657 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0      341 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/extractors/tukipasti.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2772 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0      356 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ar.json
+-rw-r--r--   0        0        0      356 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/de.json
+-rw-r--r--   0        0        0      309 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/en.json
+-rw-r--r--   0        0        0      348 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/fr.json
+-rw-r--r--   0        0        0      338 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ko.json
+-rw-r--r--   0        0        0      194 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/langs
+-rw-r--r--   0        0        0      308 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/pl.json
+-rw-r--r--   0        0        0      289 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/pt.json
+-rw-r--r--   0        0        0      418 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ru.json
+-rw-r--r--   0        0        0      660 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang/ta.json
+-rw-r--r--   0        0        0     1258 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1570 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1505 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/props.py
+-rw-r--r--   0        0        0     7437 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0     5071 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/utils/select.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/anime/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/anime/gogoanime.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/viewasian.py
+-rw-r--r--   0        0        0     3382 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/asian/watchasian.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/cartoons/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/cartoons/kisscartoon.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/__init__.py
+-rw-r--r--   0        0        0     7680 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/actvid.py
+-rw-r--r--   0        0        0     3843 2023-07-29 02:30:28.709043 mov_cli-1.4.8/mov_cli/websites/english/dopebox.py
+-rw-r--r--   0        0        0     4242 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/remotestream.py
+-rw-r--r--   0        0        0     3847 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/sflix.py
+-rw-r--r--   0        0        0     1626 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/english/solar.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/__init__.py
+-rw-r--r--   0        0        0     1943 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/einthusan.py
+-rw-r--r--   0        0        0     2165 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/indian/tamilyogi.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/international/__init__.py
+-rw-r--r--   0        0        0     3950 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/international/wlext.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/livetv/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/livetv/eja.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/sports/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/sports/scdn.py
+-rw-r--r--   0        0        0        0 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/__init__.py
+-rw-r--r--   0        0        0     2318 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/turkish123.py
+-rw-r--r--   0        0        0     2909 2023-07-29 02:30:28.713043 mov_cli-1.4.8/mov_cli/websites/turkish/yoturkish.py
+-rw-r--r--   0        0        0      736 2023-07-29 02:30:28.713043 mov_cli-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 mov_cli-1.4.8/PKG-INFO
```

### Comparing `mov_cli-1.4.7/LICENSE` & `mov_cli-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/README.md` & `mov_cli-1.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
   - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243) are installed.
 
   - Run following commands (Note: this may take a while)
     ```
     apk update && apk upgrade
     apk add python3 fzf
     python3 -m ensurepip
-    mkdir /home/root
+    mkdir /home/root && mkdir /home/root/.config
     pip3 install mov-cli
     ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -32,15 +32,15 @@
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
   id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243)
   are installed. - Run following commands (Note: this may take a while) ``` apk
 update && apk upgrade apk add python3 fzf python3 -m ensurepip mkdir /home/root
-                                                       pip3 install mov-cli ```
+                           && mkdir /home/root/.config pip3 install mov-cli ```
                                                                   (back_to_top)
  ## Usage Type: ```mov-cli``` into your Commandline.
                                                                   (back_to_top)
  ## Disclaimer This project is to be used at the userâs own risk, based on
 their government and laws. This project has no control on the content it is
 serving, using copyrighted content from the providers is not going to be
 accounted for by the developer. It is the userâs own risk. [More on That]
```

### Comparing `mov_cli-1.4.7/mov_cli/__init__.py` & `mov_cli-1.4.8/mov_cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-from .utils.props import home
 
 args_parser = argparse.ArgumentParser()
 args_parser.add_argument("--flatpak-mpv", action="store_true")
 args_parser.add_argument("--vlc", action="store_true")
 args_parser.add_argument("--pupdate", action="store_true")
 args_parser.add_argument("--debug", action="store_true", required=False)
 args_parser.add_argument("-p", required=False, help="Select Provider from Terminal")
```

### Comparing `mov_cli-1.4.7/mov_cli/__main__.py` & `mov_cli-1.4.8/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.8/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.8/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/players/player.py` & `mov_cli-1.4.8/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/utils/httpclient.py` & `mov_cli-1.4.8/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/utils/lang/ta.json` & `mov_cli-1.4.8/mov_cli/utils/lang/ta.json`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/utils/lang.py` & `mov_cli-1.4.8/mov_cli/utils/lang.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fzf import fzf_prompt
 from .props import home
 import mov_cli.__main__ as mc
 from json import loads
-from .props import RestartNeeded, LanguageNotAOption
+from .props import LanguageNotAOption
 from pkgutil import get_data
 
 langsfile = get_data(__name__, "lang/langs")
 
 langsfile = loads(langsfile)
 
 def existing(language: str, g: bool = False):
```

### Comparing `mov_cli-1.4.7/mov_cli/utils/player.py` & `mov_cli-1.4.8/mov_cli/utils/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 # Base Class
 # --------------
 class Player:
     """A base class for players in mov-cli."""
 
-    def __init__(self, display_name: str) -> None:
+    def __init__(self, display_name: str = None) -> None:
         self.__display_name = display_name
 
         self.__os = platform.system()
 
         self.__platform = platform.platform()
 
     @property
```

### Comparing `mov_cli-1.4.7/mov_cli/utils/props.py` & `mov_cli-1.4.8/mov_cli/utils/props.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from platform import system as pf
 from os import environ, mkdir, path
 from getpass import getuser
+from .player import Player
 
 
 def home():
-    plt = pf()
+    plt = Player().os
     if plt == "Windows":
         username = environ["username"]
         return f"C:/Users/{username}/AppData/Roaming/mov-cli"
-    elif (plt == "Linux") or (plt == "Darwin"):
+    elif plt == "Linux":
         return f"/home/{getuser()}/.config/mov-cli"
+    elif plt == "Android":
+        return "/storage/emulated/0/mov-cli"
+    elif plt == "iOS":
+        return "/root/mov-cli_config"
+    elif plt == "Darwin":
+        return f"/Users/{getuser()}/Library/Application Support/mov-cli"
 
 def firstStart():
+    print(home())
     if not path.exists(home()):
         mkdir(home())
 
 class RestartNeeded(Exception):
     """Raise when mov-cli is needed to restart."""
 
     def __init__(self) -> None:
```

### Comparing `mov_cli-1.4.7/mov_cli/utils/scraper.py` & `mov_cli-1.4.8/mov_cli/utils/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from platform import system as pf
 import re
 import subprocess
 
 import mov_cli.__main__ as movcli
 from fzf import fzf_prompt
 
 from .httpclient import HttpClient
```

### Comparing `mov_cli-1.4.7/mov_cli/utils/select.py` & `mov_cli-1.4.8/mov_cli/utils/select.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,20 +87,23 @@
     return import_module(module)
 
 
 def p():
     firstStart()
     try:
         js = open(f"{home()}/provider.mov-cli")
+        calls = json.load(js)
     except FileNotFoundError:
         with open(f"{home()}/provider.mov-cli", "w") as f:
             f.write(json.dumps(base))
-            js = f.read()
-    calls = json.load(js)
-
+        raise RestartNeeded
+    except json.decoder.JSONDecodeError:
+        with open(f"{home()}/provider.mov-cli", "w") as f:
+            f.write(json.dumps(base))
+        raise RestartNeeded
     try:
         from porn_cli.__main__ import websites
 
         if ph != []:
             return dict(calls)
         for main, sub in websites.items():
             calls[main] = sub
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/anime/gogoanime.py` & `mov_cli-1.4.8/mov_cli/websites/anime/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/asian/viewasian.py` & `mov_cli-1.4.8/mov_cli/websites/asian/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/asian/watchasian.py` & `mov_cli-1.4.8/mov_cli/websites/asian/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/cartoons/kisscartoon.py` & `mov_cli-1.4.8/mov_cli/websites/cartoons/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/english/actvid.py` & `mov_cli-1.4.8/mov_cli/websites/english/actvid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import sys
 import base64
 import hashlib
 
 # import chardet
 from Crypto.Cipher import AES
+from Crypto.Util.Padding import unpad
 from urllib import parse as p
 from ...utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
 import json
 
 sys.path.append("..")
 
@@ -76,46 +77,74 @@
         ).json()["link"]
         print(req)
         return req, self.rabbit_id(req)
 
     def rabbit_id(self, url: str) -> tuple:
         parts = p.urlparse(url, allow_fragments=True, scheme="/").path.split("/")
         return (
-            re.findall(r"(https:\/\/.*\/embed-4)", url)[0].replace(
-                "embed-4", "ajax/embed-4/"
+            re.findall(r"(https:\/\/.*\/embed-1)", url)[0].replace(
+                "embed-1", "embed-1/ajax/e-1/"
             ),
             parts[-1],
         )
 
+    ## Decrypting the sources
+
+    def repair_base64(self, s):
+        missing_padding = len(s) % 4
+        if missing_padding != 0:
+            s += '=' * (4 - missing_padding)
+        return s
+
     def gh_key(self):
-        u = self.client.get(
-            "https://raw.githubusercontent.com/enimax-anime/key/e4/key.txt"
-        ).text
-        return bytes(u, "utf-8")
+        response_key = self.client.get('https://github.com/enimax-anime/key/blob/e6/key.txt').json()
+        key = response_key["payload"]["blob"]["rawLines"][0]
+        key = eval(key)
+        return key
 
     def md5(self, data):
         return hashlib.md5(data).digest()
 
     def get_key(self, salt, key):
         x = self.md5(key + salt)
         currentkey = x
         while len(currentkey) < 48:
             x = self.md5(x + key + salt)
             currentkey += x
         return currentkey
+    
+    def decrypt_aes(self, encrypted_data, key):
+        dec_key = key[:32]
+        iv = key[32:]
+        print(iv, dec_key)
+        cipher = AES.new(dec_key, AES.MODE_CBC, iv=iv)
+        decrypted_data = unpad(cipher.decrypt(encrypted_data[16:]), AES.block_size)
+        return decrypted_data.decode('utf-8')
+
+    def decrypt(self, data, key): # dokicloud = pain :'(
+        data = self.repair_base64(data)
+        sources_array = list(data)
+        extracted_key = ""
+
+        for index in key:
+            for i in range(index[0], index[1]):
+                extracted_key += data[i]
+                sources_array[i] = ""
+        
+        extracted_key = self.get_key(base64.b64decode(data)[8:16], bytes(extracted_key, "utf-8"))
+            
+        data_source = "".join(sources_array)
+
+        key = extracted_key
+
+        decrypted = self.decrypt_aes(base64.b64decode(data_source), key)
+        
+        return decrypted
 
-    def unpad(self, s):
-        return s[: -ord(s[len(s) - 1 :])]
-
-    def decrypt(self, data, key):
-        k = self.get_key(base64.b64decode(data)[8:16], key)
-        dec_key = k[:32]
-        iv = k[32:]
-        p = AES.new(dec_key, AES.MODE_CBC, iv=iv).decrypt(base64.b64decode(data)[16:])
-        return self.unpad(p).decode()
+    ## End of decrypting the sources
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
         season_ids = [
             i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
         ]
         season = self.askseason(len(season_ids))
@@ -172,14 +201,8 @@
         sid = self.server_id(m[self.aid])
         iframe_url, tv_id = self.get_link(sid)
         iframe_link, iframe_id = self.rabbit_id(iframe_url)
         url = self.cdn_url(iframe_link, iframe_id)
         if state == "d":
             self.dl(url, name)
             return
-        self.play(url, name)
-
-    def SandR(self, q: str = None):
-        return self.results(self.search(q))
-
-    def redo(self, query: str = None, result: int = None):
-        return self.display(query)
+        self.play(url, name)
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/english/dopebox.py` & `mov_cli-1.4.8/mov_cli/websites/english/dopebox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
-
+from urllib import parse as p
+import re
 
 class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
         self.dseasonp = True
         self.dshowp = True
@@ -19,14 +20,28 @@
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         ep = self.askepisode(len(episodes))
         episode = episodes[int(ep) - 1]
         return episode, season, ep
 
+    def rabbit_id(self, url: str) -> tuple:
+        parts = p.urlparse(url, allow_fragments=True, scheme="/").path.split("/")
+        return (
+            re.findall(r"(https:\/\/.*\/embed-4)", url)[0].replace(
+                "embed-4", "ajax/embed-4/"
+            ),
+            parts[-1],
+        )
+
+    def gh_key(self):
+        response_key = self.client.get('https://github.com/enimax-anime/key/blob/e4/key.txt').json()
+        key = response_key["payload"]["blob"]["rawLines"][0]
+        key = eval(key)
+        return key
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def get_link(self, thing_id: str) -> tuple:
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/english/remotestream.py` & `mov_cli-1.4.8/mov_cli/websites/english/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/english/sflix.py` & `mov_cli-1.4.8/mov_cli/websites/english/sflix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
-
+from urllib import parse as p
+import re
 
 class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
         self.dseasonp = True
         self.dshowp = True
@@ -23,14 +24,29 @@
         episode = episodes[int(ep) - 1]
         return episode, season, ep
 
     def get_link(self, thing_id: str) -> tuple:
         req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()["link"]
         print(req)
         return req, self.rabbit_id(req)
+    
+    def rabbit_id(self, url: str) -> tuple:
+        parts = p.urlparse(url, allow_fragments=True, scheme="/").path.split("/")
+        return (
+            re.findall(r"(https:\/\/.*\/embed-4)", url)[0].replace(
+                "embed-4", "ajax/embed-4/"
+            ),
+            parts[-1],
+        )
+
+    def gh_key(self):
+        response_key = self.client.get('https://github.com/enimax-anime/key/blob/e4/key.txt').json()
+        key = response_key["payload"]["blob"]["rawLines"][0]
+        key = eval(key)
+        return key
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ep_server_id(self, ep_id):
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/english/solar.py` & `mov_cli-1.4.8/mov_cli/websites/indian/tamilyogi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
+from ...utils.scraper import WebScraper
+import re
 
 
-class Provider(pv):
-    def __init__(self, base_url) -> None:
+class Provider(WebScraper):
+    def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
-        self.dseasonp = True
-        self.dshowp = True
 
-    def ask(self, series_id):
-        r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [
-            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
-        ]
-        season = self.askseason(len(season_ids))
-        rf = self.client.get(
-            f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
-        )
-        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".eps-item")]
-        ep = self.askepisode(len(episodes))
-        episode = episodes[int(ep) - 1]
-        return episode, season, ep
-
-    def get_link(self, thing_id: str) -> tuple:
-        req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()["link"]
-        print(req)
-        return req, self.rabbit_id(req)
+    def search(self, q: str):
+        q = input(f"[!] {self.translated[self.task]}") if q is None else q
+        return q
+
+    def results(self, data: str) -> list:
+        req = self.client.get(f"{self.base_url}/?s={data}").text
+        soup = BS(req, self.scraper)
+        items = soup.findAll("div", {"class": "cover"})
+        urls = [items[i].find("a")["href"] for i in range(len(items))]
+        title = [items[i].find("a")["title"] for i in range(len(items))]
+        ids = [i for i in range(len(items))]
+        mov_or_tv = ["MOVIE" for i in range(len(items))]
+        return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
+
+    def cdn_url(self, url):
+        req = self.client.get(url).text
+        soup = BS(req, self.scraper)
+        iframe = soup.find("iframe")["src"]
+        q = self.client.get(iframe).text
+        url = re.findall('file:"(.*?)"', q)[0]
+        return url
+
+    def MOV_PandDP(self, m: list, state: str = "d" or "p"):
+        name = m[self.title]
+        url = self.cdn_url(m[self.url])
+        if state == "d":
+            self.dl(url, name)
+            return
+        self.play(url, name)
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/indian/einthusan.py` & `mov_cli-1.4.8/mov_cli/websites/indian/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/indian/streamblasters.py` & `mov_cli-1.4.8/mov_cli/websites/indian/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/indian/tamilyogi.py` & `mov_cli-1.4.8/mov_cli/websites/turkish/turkish123.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,65 @@
-from bs4 import BeautifulSoup as BS
 from ...utils.scraper import WebScraper
+from bs4 import BeautifulSoup as BS
 import re
 
 
 class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
-    def search(self, q: str):
+    def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
-        return q
+        return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
         soup = BS(req, self.scraper)
-        items = soup.findAll("div", {"class": "cover"})
+        mlitem = soup.findAll("div", {"class": "ml-item"})
+        items = []
+        for i in range(len(mlitem)):
+            if str(mlitem[i]).__contains__("episode"):
+                pass
+            else:
+                items.append(mlitem[i])
         urls = [items[i].find("a")["href"] for i in range(len(items))]
-        title = [items[i].find("a")["title"] for i in range(len(items))]
-        ids = [i for i in range(len(items))]
-        mov_or_tv = ["MOVIE" for i in range(len(items))]
+        title = [items[i].find("a")["oldtitle"] for i in range(len(items))]
+        ids = [items[i]["class"] for i in range(len(items))]
+        mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
-    def cdn_url(self, url):
+    def ask(self, url):
         req = self.client.get(url).text
         soup = BS(req, self.scraper)
-        iframe = soup.find("iframe")["src"]
-        q = self.client.get(iframe).text
-        url = re.findall('file:"(.*?)"', q)[0]
-        return url
-
-    def MOV_PandDP(self, m: list, state: str = "d" or "p"):
-        name = m[self.title]
-        url = self.cdn_url(m[self.url])
+        episodes = soup.findAll("a", {"class": "episodi"})
+        episode = int(self.askepisode(len(episodes)))
+        req = self.client.get(episodes[episode - 1]["href"]).text
+        url, tukibase = self.tuki(req)
+        return url, episode, tukibase
+
+    def download(self, t):
+        req = self.client.get(t[self.url]).text
+        soup = BS(req, self.scraper)
+        episodes = soup.findAll("a", {"class": "episodi"})
+        for e in range(len(episodes)):
+            req = self.client.get(episodes[e]["href"]).text
+            url, tukibase = self.tuki(req)
+            print(url)
+            self.dl(
+                url,
+                t[self.title],
+                season="",
+                episode=e + 1,
+                referrer=tukibase,
+            )
+
+    def TV_PandDP(self, t: list, state: str):
+        if state == "sd":
+            self.download(t)
+            return
+        name = t[self.title]
+        url, episode, ref = self.ask(t[self.url])
         if state == "d":
-            self.dl(url, name)
+            self.dl(url, name, episode=episode)
             return
-        self.play(url, name)
+        self.play(url, name, referrer=ref)
```

### Comparing `mov_cli-1.4.7/mov_cli/websites/international/wlext.py` & `mov_cli-1.4.8/mov_cli/websites/international/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/livetv/eja.py` & `mov_cli-1.4.8/mov_cli/websites/livetv/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/sports/scdn.py` & `mov_cli-1.4.8/mov_cli/websites/sports/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.7/mov_cli/websites/turkish/turkish123.py` & `mov_cli-1.4.8/mov_cli/websites/turkish/yoturkish.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,60 +4,71 @@
 
 
 class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
-    def search(self, q: str = None) -> str:
+    def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
         soup = BS(req, self.scraper)
-        mlitem = soup.findAll("div", {"class": "ml-item"})
         items = []
+        mlitem = soup.findAll("div", {"class": "item"})
         for i in range(len(mlitem)):
             if str(mlitem[i]).__contains__("episode"):
                 pass
             else:
                 items.append(mlitem[i])
+        if soup.find_all("ul", {"class": "pagination"}):
+            pagination = soup.find("ul", {"class": "pagination"}).findAll("li")[1:]
+            for page in pagination:
+                req = self.client.get(page.find("a")["href"]).text
+                soup = BS(req, self.scraper)
+                pageitem = soup.findAll("div", {"class": "item"})
+                for i in range(len(pageitem)):
+                    if str(pageitem[i]).__contains__("episode"):
+                        pass
+                    else:
+                        items.append(pageitem[i])
         urls = [items[i].find("a")["href"] for i in range(len(items))]
-        title = [items[i].find("a")["oldtitle"] for i in range(len(items))]
+        title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [items[i]["class"] for i in range(len(items))]
         mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        req = self.client.get(url).text
+        req = self.client.get(url, True).text
         soup = BS(req, self.scraper)
-        episodes = soup.findAll("a", {"class": "episodi"})
+        episodes = soup.findAll("a", {"class": "episod"})
         episode = int(self.askepisode(len(episodes)))
-        req = self.client.get(episodes[episode - 1]["href"]).text
+        req = self.client.get(episodes[episode - 1]["href"], True).text
         url, tukibase = self.tuki(req)
         return url, episode, tukibase
 
     def download(self, t):
         req = self.client.get(t[self.url]).text
         soup = BS(req, self.scraper)
-        episodes = soup.findAll("a", {"class": "episodi"})
+        episodes = soup.findAll("a", {"class": "episod"})
         for e in range(len(episodes)):
             req = self.client.get(episodes[e]["href"]).text
             url, tukibase = self.tuki(req)
             print(url)
             self.dl(
                 url,
                 t[self.title],
                 season="",
                 episode=e + 1,
                 referrer=tukibase,
             )
 
-    def TV_PandDP(self, t: list, state: str):
+    def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd" or "ds"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
         url, episode, ref = self.ask(t[self.url])
         if state == "d":
             self.dl(url, name, episode=episode)
```

### Comparing `mov_cli-1.4.7/pyproject.toml` & `mov_cli-1.4.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.7"
+version = "1.4.8"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@r3tr0ananas.lol>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.7/PKG-INFO` & `mov_cli-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.7
+Version: 1.4.8
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@r3tr0ananas.lol
@@ -153,15 +153,15 @@
   - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243) are installed.
 
   - Run following commands (Note: this may take a while)
     ```
     apk update && apk upgrade
     apk add python3 fzf
     python3 -m ensurepip
-    mkdir /home/root
+    mkdir /home/root && mkdir /home/root/.config
     pip3 install mov-cli
     ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.7 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.8 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@r3tr0ananas.lol Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
@@ -45,15 +45,15 @@
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
   id1449923287) and [iSH](https://apps.apple.com/us/app/ish-shell/id1436902243)
   are installed. - Run following commands (Note: this may take a while) ``` apk
 update && apk upgrade apk add python3 fzf python3 -m ensurepip mkdir /home/root
-                                                       pip3 install mov-cli ```
+                           && mkdir /home/root/.config pip3 install mov-cli ```
                                                                   (back_to_top)
  ## Usage Type: ```mov-cli``` into your Commandline.
                                                                   (back_to_top)
  ## Disclaimer This project is to be used at the userâs own risk, based on
 their government and laws. This project has no control on the content it is
 serving, using copyrighted content from the providers is not going to be
 accounted for by the developer. It is the userâs own risk. [More on That]
```

