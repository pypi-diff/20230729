# Comparing `tmp/deebot-client-2.1.0.tar.gz` & `tmp/deebot-client-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-2.1.0.tar", last modified: Tue Jul 18 20:37:57 2023, max compression
+gzip compressed data, was "deebot-client-3.0.0b0.tar", last modified: Sat Jul 29 09:55:57 2023, max compression
```

## Comparing `deebot-client-2.1.0.tar` & `deebot-client-3.0.0b0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-18 20:37:50.000000 deebot-client-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-18 20:37:57.565588 deebot-client-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-18 20:37:50.000000 deebot-client-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.557587 deebot-client-2.1.0/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.557587 deebot-client-2.1.0/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 20:37:50.000000 deebot-client-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 20:37:57.569588 deebot-client-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-18 20:37:50.000000 deebot-client-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.553587 deebot-client-2.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.347691 deebot-client-3.0.0b0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 09:55:57.000000 deebot-client-3.0.0b0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.343691 deebot-client-3.0.0b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.351691 deebot-client-3.0.0b0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.351691 deebot-client-3.0.0b0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:57.355691 deebot-client-3.0.0b0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-29 09:55:53.000000 deebot-client-3.0.0b0/tests/messages/test_stats.py
```

### Comparing `deebot-client-2.1.0/LICENSE.txt` & `deebot-client-3.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/PKG-INFO` & `deebot-client-3.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.1.0
+Version: 3.0.0b0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-2.1.0/README.md` & `deebot-client-3.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/api_client.py` & `deebot-client-3.0.0b0/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/authentication.py` & `deebot-client-3.0.0b0/deebot_client/authentication.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/command.py` & `deebot-client-3.0.0b0/deebot_client/command.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/__init__.py` & `deebot-client-3.0.0b0/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/charge.py` & `deebot-client-3.0.0b0/deebot_client/commands/charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/charge_state.py` & `deebot-client-3.0.0b0/deebot_client/commands/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/clean.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/clean_count.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/clean_logs.py` & `deebot-client-3.0.0b0/deebot_client/commands/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/common.py` & `deebot-client-3.0.0b0/deebot_client/commands/common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/custom.py` & `deebot-client-3.0.0b0/deebot_client/commands/custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/error.py` & `deebot-client-3.0.0b0/deebot_client/commands/error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/fan_speed.py` & `deebot-client-3.0.0b0/deebot_client/commands/fan_speed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 """(fan) speed commands."""
 from collections.abc import Mapping
 from typing import Any
 
-from ..events import FanSpeedEvent
+from ..events import FanSpeedEvent, FanSpeedLevel
 from ..message import HandlingResult, MessageBodyDataDict
-from ..util import DisplayNameIntEnum
 from .common import EventBus, NoArgsCommand, SetCommand
 
 
-class FanSpeedLevel(DisplayNameIntEnum):
-    """Enum class for all possible fan speed levels."""
-
-    # Values should be sort from low to high on their meanings
-    QUIET = 1000
-    NORMAL = 0
-    MAX = 1
-    MAX_PLUS = 2, "max+"
-
-
 class GetFanSpeed(NoArgsCommand, MessageBodyDataDict):
     """Get fan speed command."""
 
     name = "getSpeed"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
-        event_bus.notify(FanSpeedEvent(FanSpeedLevel(int(data["speed"])).display_name))
+        event_bus.notify(FanSpeedEvent(FanSpeedLevel(int(data["speed"]))))
         return HandlingResult.success()
 
 
 class SetFanSpeed(SetCommand):
     """Set fan speed command."""
 
     name = "setSpeed"
```

### Comparing `deebot-client-2.1.0/deebot_client/commands/life_span.py` & `deebot-client-3.0.0b0/deebot_client/commands/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/map.py` & `deebot-client-3.0.0b0/deebot_client/commands/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/pos.py` & `deebot-client-3.0.0b0/deebot_client/commands/pos.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/stats.py` & `deebot-client-3.0.0b0/deebot_client/commands/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/volume.py` & `deebot-client-3.0.0b0/deebot_client/commands/volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/commands/water_info.py` & `deebot-client-3.0.0b0/deebot_client/commands/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/events/__init__.py` & `deebot-client-3.0.0b0/deebot_client/events/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 from typing import Any, Optional
 
 from ..events.base import Event
 from ..models import Room, VacuumState
 from ..util import DisplayNameIntEnum
+from .fan_speed import FanSpeedEvent, FanSpeedLevel
 from .map import (
     MajorMapEvent,
     MapSetEvent,
     MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
@@ -77,21 +78,14 @@
 class ErrorEvent(Event):
     """Error event representation."""
 
     code: int
     description: str | None
 
 
-@dataclass(frozen=True)
-class FanSpeedEvent(Event):
-    """Fan speed event representation."""
-
-    speed: str
-
-
 @unique
 class LifeSpan(str, Enum):
     """Enum class for all possible life span components."""
 
     SIDE_BRUSH = "sideBrush"
     BRUSH = "brush"
     FILTER = "heap"
```

### Comparing `deebot-client-2.1.0/deebot_client/events/const.py` & `deebot-client-3.0.0b0/deebot_client/events/const.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/events/event_bus.py` & `deebot-client-3.0.0b0/deebot_client/events/event_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Event emitter module."""
 import asyncio
 import threading
 from collections.abc import Callable, Coroutine
+from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar
 
 from ..logging_filter import get_logger
 from ..models import VacuumState
 from ..util import cancel, create_task
 from . import AvailabilityEvent, Event, StateEvent
 
@@ -24,14 +25,16 @@
         super().__init__()
 
         self.subscriber_callbacks: Final[
             list[Callable[[T], Coroutine[Any, Any, None]]]
         ] = []
         self.semaphore: Final = asyncio.Semaphore(1)
         self.last_event: T | None = None
+        self.last_event_time: datetime = datetime(1, 1, 1, 1, 1, 1, tzinfo=timezone.utc)
+        self.notify_handle: asyncio.TimerHandle | None = None
 
 
 class EventBus:
     """A very simple event bus system."""
 
     def __init__(
         self,
@@ -69,60 +72,80 @@
             create_task(self._tasks, callback(event_processing_data.last_event))
         elif len(event_processing_data.subscriber_callbacks) == 1:
             # first subscriber therefore do refresh
             self.request_refresh(event_type)
 
         return unsubscribe
 
-    def notify(self, event: T) -> bool:
+    def notify(self, event: T, *, debounce_time: float = 0) -> None:
         """Notify subscriber with given event representation."""
         event_processing_data = self._get_or_create_event_processing_data(type(event))
 
         if (
-            isinstance(event, StateEvent)
-            and event.state == VacuumState.IDLE
-            and event_processing_data.last_event
-            and event_processing_data.last_event.state == VacuumState.DOCKED  # type: ignore[attr-defined]
-        ):
-            # todo distinguish better between docked and idle and outside event bus. # pylint: disable=fixme
-            # Problem getCleanInfo will return state=idle, when bot is charging
-            event = StateEvent(VacuumState.DOCKED)  # type: ignore[assignment]
-        elif (
-            isinstance(event, AvailabilityEvent)
-            and event.available
-            and event_processing_data.last_event
-            and not event_processing_data.last_event.available  # type: ignore[attr-defined]
-        ):
-            # unavailable -> available: refresh everything
-            for event_type, _ in self._event_processing_dict.items():
-                if event_type != AvailabilityEvent:
-                    self.request_refresh(event_type)
-
-        if event == event_processing_data.last_event:
-            _LOGGER.debug("Event is the same! Skipping (%s)", event)
-            return False
-
-        event_processing_data.last_event = event
-        if event_processing_data.subscriber_callbacks:
-            _LOGGER.debug("Notify subscribers with %s", event)
-            for callback in event_processing_data.subscriber_callbacks:
-                create_task(self._tasks, callback(event))
-            return True
-
-        _LOGGER.debug("No subscribers... Discharging %s", event)
-        return False
+            handle := event_processing_data.notify_handle
+        ) is not None and not handle.cancelled():
+            handle.cancel()
+
+        def _notify(event: T) -> None:
+            event_processing_data.last_event_time = datetime.now(timezone.utc)
+            event_processing_data.notify_handle = None
+
+            if (
+                isinstance(event, StateEvent)
+                and event.state == VacuumState.IDLE
+                and event_processing_data.last_event
+                and event_processing_data.last_event.state == VacuumState.DOCKED  # type: ignore[attr-defined]
+            ):
+                # todo distinguish better between docked and idle and outside event bus. # pylint: disable=fixme
+                # Problem getCleanInfo will return state=idle, when bot is charging
+                event = StateEvent(VacuumState.DOCKED)  # type: ignore[assignment]
+            elif (
+                isinstance(event, AvailabilityEvent)
+                and event.available
+                and event_processing_data.last_event
+                and not event_processing_data.last_event.available  # type: ignore[attr-defined]
+            ):
+                # unavailable -> available: refresh everything
+                for event_type, _ in self._event_processing_dict.items():
+                    if event_type != AvailabilityEvent:
+                        self.request_refresh(event_type)
+
+            if event == event_processing_data.last_event:
+                _LOGGER.debug("Event is the same! Skipping (%s)", event)
+                return
+
+            event_processing_data.last_event = event
+            if event_processing_data.subscriber_callbacks:
+                _LOGGER.debug("Notify subscribers with %s", event)
+                for callback in event_processing_data.subscriber_callbacks:
+                    create_task(self._tasks, callback(event))
+            else:
+                _LOGGER.debug("No subscribers... Discharging %s", event)
+
+        now = datetime.now(timezone.utc)
+        if debounce_time <= 0 or (
+            now - event_processing_data.last_event_time
+        ) > timedelta(seconds=debounce_time):
+            _notify(event)
+        else:
+            event_processing_data.notify_handle = asyncio.get_running_loop().call_later(
+                debounce_time, _notify, event
+            )
 
     def request_refresh(self, event_class: type[T]) -> None:
         """Request manual refresh."""
         if self.has_subscribers(event_class):
             create_task(self._tasks, self._call_refresh_function(event_class))
 
     async def teardown(self) -> None:
         """Teardown eventbus."""
         await cancel(self._tasks)
+        for data in self._event_processing_dict.values():
+            if handle := data.notify_handle:
+                handle.cancel()
 
     async def _call_refresh_function(self, event_class: type[T]) -> None:
         semaphore = self._event_processing_dict[event_class].semaphore
         if semaphore.locked():
             _LOGGER.debug("Already refresh function running. Skipping...")
             return
```

### Comparing `deebot-client-2.1.0/deebot_client/events/map.py` & `deebot-client-3.0.0b0/deebot_client/events/map.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,8 +98,8 @@
     active: bool
 
 
 @dataclass(frozen=True)
 class MapChangedEvent(Event):
     """Map changed event."""
 
-    when: datetime = datetime.utcnow()
+    when: datetime
```

### Comparing `deebot-client-2.1.0/deebot_client/logging_filter.py` & `deebot-client-3.0.0b0/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/map.py` & `deebot-client-3.0.0b0/deebot_client/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import base64
 import dataclasses
 import lzma
 import math
 import struct
 import zlib
 from collections.abc import Callable, Coroutine
-from datetime import datetime, timedelta
+from datetime import datetime, timezone
 from io import BytesIO
 from typing import Any, Final
 
 from numpy import ndarray, reshape, zeros
 from PIL import Image, ImageDraw, ImageOps
 
 from deebot_client.events.map import MapChangedEvent
@@ -535,19 +535,17 @@
     """Map data."""
 
     def __init__(self, event_bus: EventBus) -> None:
         self._changed: bool = False
 
         def on_change() -> None:
             self._changed = True
-            now = datetime.utcnow()
-            last_event = event_bus.get_last_event(MapChangedEvent)
-            if last_event is None or (now - last_event.when) > timedelta(seconds=1):
-                # throttle notify to ones a second
-                event_bus.notify(MapChangedEvent(now))
+            event_bus.notify(
+                MapChangedEvent(datetime.now(timezone.utc)), debounce_time=1
+            )
 
         self._on_change = on_change
         self._map_pieces: OnChangedList[MapPiece] = OnChangedList(
             on_change, [MapPiece(on_change, i) for i in range(64)]
         )
         self._map_subsets: OnChangedDict[int, MapSubsetEvent] = OnChangedDict(on_change)
         self._positions: OnChangedList[Position] = OnChangedList(on_change)
```

### Comparing `deebot-client-2.1.0/deebot_client/message.py` & `deebot-client-3.0.0b0/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/messages/__init__.py` & `deebot-client-3.0.0b0/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/messages/battery.py` & `deebot-client-3.0.0b0/deebot_client/messages/battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/messages/stats.py` & `deebot-client-3.0.0b0/deebot_client/messages/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/models.py` & `deebot-client-3.0.0b0/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/mqtt_client.py` & `deebot-client-3.0.0b0/deebot_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/util.py` & `deebot-client-3.0.0b0/deebot_client/util.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client/vacuum_bot.py` & `deebot-client-3.0.0b0/deebot_client/vacuum_bot.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/deebot_client.egg-info/PKG-INFO` & `deebot-client-3.0.0b0/deebot_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.1.0
+Version: 3.0.0b0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-2.1.0/deebot_client.egg-info/SOURCES.txt` & `deebot-client-3.0.0b0/deebot_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 deebot_client/commands/true_detect.py
 deebot_client/commands/volume.py
 deebot_client/commands/water_info.py
 deebot_client/events/__init__.py
 deebot_client/events/base.py
 deebot_client/events/const.py
 deebot_client/events/event_bus.py
+deebot_client/events/fan_speed.py
 deebot_client/events/map.py
 deebot_client/events/water_info.py
 deebot_client/messages/__init__.py
 deebot_client/messages/battery.py
 deebot_client/messages/stats.py
 tests/commands/__init__.py
 tests/commands/test_advanced_mode.py
```

### Comparing `deebot-client-2.1.0/setup.py` & `deebot-client-3.0.0b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="2.1.0",
+    version="3.0.0b0",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
```

### Comparing `deebot-client-2.1.0/tests/commands/__init__.py` & `deebot-client-3.0.0b0/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_advanced_mode.py` & `deebot-client-3.0.0b0/tests/commands/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_carpet.py` & `deebot-client-3.0.0b0/tests/commands/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_charge.py` & `deebot-client-3.0.0b0/tests/commands/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_clean.py` & `deebot-client-3.0.0b0/tests/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_clean_count.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_clean_log.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_clean_preference.py` & `deebot-client-3.0.0b0/tests/commands/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_common.py` & `deebot-client-3.0.0b0/tests/commands/test_common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_continuous_cleaning.py` & `deebot-client-3.0.0b0/tests/commands/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_custom.py` & `deebot-client-3.0.0b0/tests/commands/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_fan_speed.py` & `deebot-client-3.0.0b0/tests/commands/test_fan_speed.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 def test_FanSpeedLevel_unique() -> None:
     verify_DisplayNameEnum_unique(FanSpeedLevel)
 
 
 async def test_GetFanSpeed() -> None:
     json = get_request_json({"speed": 2})
-    await assert_command(GetFanSpeed(), json, FanSpeedEvent("max+"))
+    await assert_command(GetFanSpeed(), json, FanSpeedEvent(FanSpeedLevel.MAX_PLUS))
 
 
 @pytest.mark.parametrize(
-    "value, expected", [("quiet", 1000), ("max+", 2), (0, 0), (FanSpeedLevel.MAX, 1)]
+    "value, expected",
+    [("quiet", 1000), ("max_plus", 2), (0, 0), (FanSpeedLevel.MAX, 1)],
 )
 def test_SetFanSpeed(value: str | int | FanSpeedLevel, expected: int) -> None:
     command = SetFanSpeed(value)
     assert command.name == "setSpeed"
     assert command._args == {"speed": expected}
```

### Comparing `deebot-client-2.1.0/tests/commands/test_life_span.py` & `deebot-client-3.0.0b0/tests/commands/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_map.py` & `deebot-client-3.0.0b0/tests/commands/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_mulitmap_state.py` & `deebot-client-3.0.0b0/tests/commands/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_true_detect.py` & `deebot-client-3.0.0b0/tests/commands/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/commands/test_water_info.py` & `deebot-client-3.0.0b0/tests/commands/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/messages/test_battery.py` & `deebot-client-3.0.0b0/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/messages/test_get_messages.py` & `deebot-client-3.0.0b0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.1.0/tests/messages/test_stats.py` & `deebot-client-3.0.0b0/tests/messages/test_stats.py`

 * *Files identical despite different names*

