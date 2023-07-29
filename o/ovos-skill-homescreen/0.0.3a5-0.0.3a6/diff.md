# Comparing `tmp/ovos-skill-homescreen-0.0.3a5.tar.gz` & `tmp/ovos-skill-homescreen-0.0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-skill-homescreen-0.0.3a5.tar", last modified: Fri Jun 30 22:02:28 2023, max compression
+gzip compressed data, was "ovos-skill-homescreen-0.0.3a6.tar", last modified: Sat Jul 29 17:08:46 2023, max compression
```

## Comparing `ovos-skill-homescreen-0.0.3a5.tar` & `ovos-skill-homescreen-0.0.3a6.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.995375 ovos-skill-homescreen-0.0.3a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 22:02:27.995375 ovos-skill-homescreen-0.0.3a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    26225 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/initialcards.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.971373 ovos-skill-homescreen-0.0.3a5/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.971373 ovos-skill-homescreen-0.0.3a5/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/de-de/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/de-de/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.971373 ovos-skill-homescreen-0.0.3a5/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/en-us/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/en-us/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/es-es/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/es-es/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/fr-fr/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/fr-fr/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/it-it/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/it-it/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/nl-nl/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/nl-nl/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/locale/pt-pt/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/pt-pt/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/locale/pt-pt/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.971373 ovos-skill-homescreen-0.0.3a5/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/res/desktop/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:02:27.995375 ovos-skill-homescreen-0.0.3a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.975374 ovos-skill-homescreen-0.0.3a5/skill/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/skill/cardGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/skill/dashboardHandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.979374 ovos-skill-homescreen-0.0.3a5/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/AddCardOverlay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/AppEntry.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/AppsBar.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/BottomWidgetsArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/BoxesPage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/DayMonthDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/ExamplesDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/GridBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/HorizontalDisplayLayout.qml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/HorizontalTopArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/MainPage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/MediaWidgetButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/MediaWidgetDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/NightTimePage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/NotificationDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/TimeDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/VerticalDisplayLayout.qml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/VerticalTopArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/WeatherArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/WidgetsArea.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.979374 ovos-skill-homescreen-0.0.3a5/ui/boxes/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/boxes/PlayRelaxingMusic.qml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/boxes/PlayTheNews.qml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/boxes/SetAlarmBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/boxes/TakeNoteBox.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.979374 ovos-skill-homescreen-0.0.3a5/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/code/dashmodel.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.979374 ovos-skill-homescreen-0.0.3a5/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/delegates/BoxAbstractDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/delegates/BoxSimpleDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.979374 ovos-skill-homescreen-0.0.3a5/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/alarmicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/cam.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/clouds.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/dialog-close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/fog.svg
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/high_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/humidity.svg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/low_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/mic-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/mic-start.svg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/mic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/moon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/no-internet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/notification-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/notificationicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/offline_layer_one.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/offline_layer_two.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds_day.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds_night.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/rain.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/snow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/storm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/sun.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/sunrise.svg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/sunset.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/timericon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/icons/wind.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/idle.qml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.983374 ovos-skill-homescreen-0.0.3a5/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/sounds/clicked.wav
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/sounds/start-listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.983374 ovos-skill-homescreen-0.0.3a5/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/templates/CardTemplate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.983374 ovos-skill-homescreen-0.0.3a5/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/ExamplesDisplay_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/idle_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:27.995375 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (123)   756810 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-01.png
--rw-r--r--   0 runner    (1001) docker     (123)  2011692 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-02.png
--rw-r--r--   0 runner    (1001) docker     (123)  1137893 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-03.png
--rw-r--r--   0 runner    (1001) docker     (123)  2125851 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-04.png
--rw-r--r--   0 runner    (1001) docker     (123)  1595246 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-05.png
--rw-r--r--   0 runner    (1001) docker     (123)  1711853 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/ui/wallpapers/default.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 22:02:27.000000 ovos-skill-homescreen-0.0.3a5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.110589 ovos-skill-homescreen-0.0.3a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 17:08:46.106589 ovos-skill-homescreen-0.0.3a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/initialcards.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.078588 ovos-skill-homescreen-0.0.3a6/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/de-de/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/de-de/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/en-us/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/en-us/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/es-es/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/es-es/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/fr-fr/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/fr-fr/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/it-it/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/it-it/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/nl-nl/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/nl-nl/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/locale/pt-pt/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/pt-pt/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/locale/pt-pt/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 17:08:46.000000 ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.082588 ovos-skill-homescreen-0.0.3a6/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/res/desktop/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:08:46.110589 ovos-skill-homescreen-0.0.3a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/skill/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/skill/cardGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/skill/dashboardHandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/AddCardOverlay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/AppEntry.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/AppsBar.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/BottomWidgetsArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/BoxesPage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/DayMonthDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/ExamplesDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/GridBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/HorizontalDisplayLayout.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/HorizontalTopArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/MainPage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/MediaWidgetButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/MediaWidgetDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/NightTimePage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/NotificationDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/TimeDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/VerticalDisplayLayout.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/VerticalTopArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/WeatherArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/WidgetsArea.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/ui/boxes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/boxes/PlayRelaxingMusic.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/boxes/PlayTheNews.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/boxes/SetAlarmBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/boxes/TakeNoteBox.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.086588 ovos-skill-homescreen-0.0.3a6/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/code/dashmodel.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.090589 ovos-skill-homescreen-0.0.3a6/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/delegates/BoxAbstractDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/delegates/BoxSimpleDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.094589 ovos-skill-homescreen-0.0.3a6/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/alarmicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/cam.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/dialog-close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/fog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/high_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/humidity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/low_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/mic-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/mic-start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/mic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/moon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/no-internet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/notification-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/notificationicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/offline_layer_one.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/offline_layer_two.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds_day.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds_night.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/rain.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/snow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/storm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/sun.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/sunrise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/sunset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/timericon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/icons/wind.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/idle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.094589 ovos-skill-homescreen-0.0.3a6/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/sounds/clicked.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/sounds/start-listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.094589 ovos-skill-homescreen-0.0.3a6/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/templates/CardTemplate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.098589 ovos-skill-homescreen-0.0.3a6/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/ExamplesDisplay_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/idle_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:08:46.106589 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (123)   756810 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-01.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2011692 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-02.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1137893 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-03.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2125851 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-04.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1595246 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-05.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1711853 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/ui/wallpapers/default.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-29 17:08:42.000000 ovos-skill-homescreen-0.0.3a6/version.py
```

### Comparing `ovos-skill-homescreen-0.0.3a5/LICENSE` & `ovos-skill-homescreen-0.0.3a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/__init__.py` & `ovos-skill-homescreen-0.0.3a6/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         self.bus.on("enclosure.notify.no_internet", self.on_no_internet)
 
         # Handle Screenshot Response
         self.bus.on("ovos.display.screenshot.get.response",
                     self.screenshot_taken)
 
         self.collect_wallpapers()
+        SkillApi.connect_bus(self.bus)
         self._load_skill_apis()
 
         self.schedule_repeating_event(self.update_weather, callback_time, 900)
         self.schedule_repeating_event(self.update_examples, callback_time, 900)
 
         self.bus.on("ovos.wallpaper.manager.loaded",
                     self.register_homescreen_wallpaper_provider)
@@ -220,37 +221,56 @@
                 self.gui['skill_examples'] = {"examples": skill_examples}
             except ImportError:
                 self.settings["examples_enabled"] = False
 
         self.gui['skill_info_enabled'] = self.examples_enabled
         self.gui['skill_info_prefix'] = self.settings.get("examples_prefix", False)
 
+    def _update_datetime_from_api(self):
+        """
+        Update the GUI with date/time from the configured Skill API
+        """
+        time_string = self.datetime_api.get_display_current_time()
+        date_string = self.datetime_api.get_display_date()
+        weekday_string = self.datetime_api.get_weekday()
+        # The datetime skill decides what order day and month are returned
+        day_string, month_string = \
+            self.datetime_api.get_month_date().split(maxsplit=1)
+        year_string = self.datetime_api.get_year()
+        self.gui["time_string"] = time_string
+        self.gui["date_string"] = date_string
+        self.gui["weekday_string"] = weekday_string
+        self.gui['day_string'] = day_string
+        self.gui["month_string"] = month_string
+        self.gui["year_string"] = year_string
+
     def update_dt(self):
         """
         Loads or updates date/time via the datetime_api.
         """
         if not self.datetime_api and self.datetime_skill_id:
             LOG.debug("Requested update before datetime API loaded")
             self._load_skill_apis()
         if self.datetime_api:
-            time_string = self.datetime_api.get_display_current_time()
-            date_string = self.datetime_api.get_display_date()
-            weekday_string = self.datetime_api.get_weekday()
-            day_string, month_string = self._split_month_string(self.datetime_api.get_month_date())
-            year_string = self.datetime_api.get_year()
-        else:
-            date_string_object = get_date_strings(date_format=self.config_core.get("date_format", "MDY"), 
-                                                  time_format=self.config_core.get("time_format", "full"),
-                                                  lang=self.lang)
-            time_string = date_string_object.get("time_string")
-            date_string = date_string_object.get("date_string")
-            weekday_string = date_string_object.get("weekday_string")
-            day_string = date_string_object.get("day_string")
-            month_string = date_string_object.get("month_string")
-            year_string = date_string_object.get("year_string")
+            try:
+                self._update_datetime_from_api()
+                return
+            except Exception as e:
+                LOG.exception(f"Skill API error: {e}")
+
+        date_string_object = get_date_strings(
+            date_format=self.config_core.get("date_format", "MDY"),
+            time_format=self.config_core.get("time_format", "full"),
+            lang=self.lang)
+        time_string = date_string_object.get("time_string")
+        date_string = date_string_object.get("date_string")
+        weekday_string = date_string_object.get("weekday_string")
+        day_string = date_string_object.get("day_string")
+        month_string = date_string_object.get("month_string")
+        year_string = date_string_object.get("year_string")
 
         self.gui["time_string"] = time_string
         self.gui["date_string"] = date_string
         self.gui["weekday_string"] = weekday_string
         self.gui['day_string'] = day_string
         self.gui["month_string"] = month_string
         self.gui["year_string"] = year_string
@@ -381,39 +401,36 @@
         """
         Loads weather, date/time, and examples skill APIs
         """
         # Import Date Time Skill As Date Time Provider if configured (default LF)
         try:
             if not self.datetime_api and self.datetime_skill_id:
                 self.datetime_api = SkillApi.get(self.datetime_skill_id)
+                assert self.datetime_api.get_display_current_time is not None
+                assert self.datetime_api.get_display_date is not None
+                assert self.datetime_api.get_weekday is not None
+                assert self.datetime_api.get_year is not None
+        except AssertionError as e:
+            LOG.error(f"missing API method: {e}")
+            self.datetime_api = None
         except Exception as e:
             LOG.error(f"Failed to import DateTime Skill: {e}")
+            self.datetime_api = None
 
         # Import Skill Info Skill if configured (default OSM)
         if not self.skill_info_api and self.examples_skill_id:
             try:
                 self.skill_info_api = SkillApi.get(self.examples_skill_id)
+                assert self.skill_info_api.skill_info_examples is not None
+            except AssertionError as e:
+                LOG.error(f"missing API method: {e}")
+                self.skill_info_api = None
             except Exception as e:
                 LOG.error(f"Failed to import Info Skill: {e}")
-
-    def _split_month_string(self, month_date: str) -> list:
-        """
-        Splits a month+date string into month and date (i.e. "August 06" -> ["August", "06"])
-        :param month_date: formatted month and day of month ("August 06" or "06 August")
-        :return: [day, month]
-        """
-        month_string = month_date.split(" ")
-        if self.config_core.get('date_format') == 'MDY':
-            day_string = month_string[1]
-            month_string = month_string[0]
-        else:
-            day_string = month_string[0]
-            month_string = month_string[1]
-
-        return [day_string, month_string]
+                self.skill_info_api = None
 
     #####################################################################
     # Build Voice Applications Model
 
     def find_icon_full_path(self, icon_name):
         localuser = environ.get('USER')
         folder_search_paths = ["/usr/share/icons/", "/usr/local/share/icons/",
```

### Comparing `ovos-skill-homescreen-0.0.3a5/initialcards.json` & `ovos-skill-homescreen-0.0.3a6/initialcards.json`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ovos_skill_homescreen.egg-info/SOURCES.txt` & `ovos-skill-homescreen-0.0.3a6/ovos_skill_homescreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/res/desktop/skill.json` & `ovos-skill-homescreen-0.0.3a6/res/desktop/skill.json`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/setup.py` & `ovos-skill-homescreen-0.0.3a6/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/skill/__init__.py` & `ovos-skill-homescreen-0.0.3a6/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/skill/cardGenerator.py` & `ovos-skill-homescreen-0.0.3a6/skill/cardGenerator.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/skill/dashboardHandler.py` & `ovos-skill-homescreen-0.0.3a6/skill/dashboardHandler.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/AddCardOverlay.qml` & `ovos-skill-homescreen-0.0.3a6/ui/AddCardOverlay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/AppEntry.qml` & `ovos-skill-homescreen-0.0.3a6/ui/AppEntry.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/AppsBar.qml` & `ovos-skill-homescreen-0.0.3a6/ui/AppsBar.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/BottomWidgetsArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/BottomWidgetsArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/BoxesPage.qml` & `ovos-skill-homescreen-0.0.3a6/ui/BoxesPage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/DayMonthDisplay.qml` & `ovos-skill-homescreen-0.0.3a6/ui/DayMonthDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/ExamplesDisplay.qml` & `ovos-skill-homescreen-0.0.3a6/ui/ExamplesDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/GridBox.qml` & `ovos-skill-homescreen-0.0.3a6/ui/GridBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/HorizontalDisplayLayout.qml` & `ovos-skill-homescreen-0.0.3a6/ui/HorizontalDisplayLayout.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/HorizontalTopArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/HorizontalTopArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/MainPage.qml` & `ovos-skill-homescreen-0.0.3a6/ui/MainPage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/MediaWidgetButton.qml` & `ovos-skill-homescreen-0.0.3a6/ui/MediaWidgetButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/MediaWidgetDisplay.qml` & `ovos-skill-homescreen-0.0.3a6/ui/MediaWidgetDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/NightTimePage.qml` & `ovos-skill-homescreen-0.0.3a6/ui/NightTimePage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/NotificationDelegate.qml` & `ovos-skill-homescreen-0.0.3a6/ui/NotificationDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/SwipeArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/TimeDisplay.qml` & `ovos-skill-homescreen-0.0.3a6/ui/TimeDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/VerticalDisplayLayout.qml` & `ovos-skill-homescreen-0.0.3a6/ui/VerticalDisplayLayout.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/VerticalTopArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/VerticalTopArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/WeatherArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/WeatherArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/WidgetsArea.qml` & `ovos-skill-homescreen-0.0.3a6/ui/WidgetsArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/boxes/PlayRelaxingMusic.qml` & `ovos-skill-homescreen-0.0.3a6/ui/boxes/PlayRelaxingMusic.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/code/dashmodel.js` & `ovos-skill-homescreen-0.0.3a6/ui/code/dashmodel.js`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/delegates/BoxAbstractDelegate.qml` & `ovos-skill-homescreen-0.0.3a6/ui/delegates/BoxAbstractDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/delegates/BoxSimpleDelegate.qml` & `ovos-skill-homescreen-0.0.3a6/ui/delegates/BoxSimpleDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/alarmicon.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/alarmicon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/clear.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/clear.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/close.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/clouds.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/clouds.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/delete.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/dialog-close.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/fog.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/fog.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/high_temperature.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/high_temperature.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/humidity.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/humidity.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/low_temperature.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/low_temperature.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/mic-min.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/mic-min.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/mic-start.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/mic-start.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/mic.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/mic.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/no-internet.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/no-internet.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/notificationicon.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/notificationicon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/offline_layer_one.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/offline_layer_one.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/offline_layer_two.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/offline_layer_two.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds_day.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds_day.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/partial_clouds_night.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/partial_clouds_night.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/rain.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/rain.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/snow.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/snow.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/storm.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/storm.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/sun.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/sunrise.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/sunset.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/timericon.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/timericon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/icons/wind.svg` & `ovos-skill-homescreen-0.0.3a6/ui/icons/wind.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/idle.qml` & `ovos-skill-homescreen-0.0.3a6/ui/idle.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/qmldir` & `ovos-skill-homescreen-0.0.3a6/ui/qmldir`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/sounds/clicked.wav` & `ovos-skill-homescreen-0.0.3a6/ui/sounds/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/sounds/start-listening.wav` & `ovos-skill-homescreen-0.0.3a6/ui/sounds/start-listening.wav`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/templates/CardTemplate.qml` & `ovos-skill-homescreen-0.0.3a6/ui/templates/CardTemplate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_de.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_es.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_fr.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_it.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_nl.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/AddCardOverlay_pt.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/AddCardOverlay_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_de.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_es.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_fr.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_it.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_nl.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/BoxesPage_pt.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/BoxesPage_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_de.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_es.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_fr.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_it.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_nl.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/GridBox_pt.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/GridBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/idle_de.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/idle_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/idle_es.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/idle_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/idle_it.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/idle_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/idle_nl.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/idle_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/idle_pt.ts` & `ovos-skill-homescreen-0.0.3a6/ui/translations/idle_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm` & `ovos-skill-homescreen-0.0.3a6/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-01.png` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-01.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-02.png` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-02.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-03.png` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-03.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-04.png` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-04.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/background-05.png` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/background-05.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a5/ui/wallpapers/default.jpg` & `ovos-skill-homescreen-0.0.3a6/ui/wallpapers/default.jpg`

 * *Files identical despite different names*

