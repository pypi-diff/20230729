# Comparing `tmp/log_rate_limit-1.2.2.tar.gz` & `tmp/log_rate_limit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_rate_limit-1.2.2.tar", max compression
+gzip compressed data, was "log_rate_limit-1.3.0.tar", max compression
```

## Comparing `log_rate_limit-1.2.2.tar` & `log_rate_limit-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11358 2022-11-12 10:49:11.141791 log_rate_limit-1.2.2/LICENSE
--rw-r--r--   0        0        0      121 2022-11-12 10:50:41.588539 log_rate_limit-1.2.2/NOTICE
--rwxr-xr-x   0        0        0     7090 2022-12-07 19:24:56.781654 log_rate_limit-1.2.2/README.md
--rw-r--r--   0        0        0      248 2022-11-27 15:06:56.230395 log_rate_limit-1.2.2/log_rate_limit/__init__.py
--rwxr-xr-x   0        0        0    12960 2022-12-22 08:52:14.431097 log_rate_limit-1.2.2/log_rate_limit/log_rate_limit.py
--rw-r--r--   0        0        0     1121 2022-12-22 08:49:53.645959 log_rate_limit-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 log_rate_limit-1.2.2/setup.py
--rw-r--r--   0        0        0     8109 1970-01-01 00:00:00.000000 log_rate_limit-1.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2022-11-12 10:49:11.000000 log_rate_limit-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0      126 2023-07-25 19:31:01.960281 log_rate_limit-1.3.0/NOTICE
+-rwxr-xr-x   0        0        0     7092 2023-07-29 19:49:56.401368 log_rate_limit-1.3.0/README.md
+-rwxr-xr-x   0        0        0      248 2022-11-27 15:06:56.000000 log_rate_limit-1.3.0/log_rate_limit/__init__.py
+-rwxr-xr-x   0        0        0    19377 2023-07-29 15:12:14.883411 log_rate_limit-1.3.0/log_rate_limit/log_rate_limit.py
+-rwxr-xr-x   0        0        0     1228 2023-07-29 13:53:11.670014 log_rate_limit-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8111 1970-01-01 00:00:00.000000 log_rate_limit-1.3.0/PKG-INFO
```

### Comparing `log_rate_limit-1.2.2/LICENSE` & `log_rate_limit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `log_rate_limit-1.2.2/README.md` & `log_rate_limit-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
 Import the filter:
 
 ```python
 from log_rate_limit import StreamRateLimitFilter, RateLimit
 ```
 
-Use the filter with your `logger`. With default parameters it will rate limit all repetitive log message:
+Use the filter with your `logger` - with default parameters it will rate-limit all repetitive log messages:
 
 ```python
 logger.addFilter(StreamRateLimitFilter(period_sec=30))
 ```
 
-All logs on `logger` will now be rate limited, but this can be disabled per-log by setting the `stream_id` to `None`:
+All logs on `logger` will now be rate-limited, but this can be disabled per-log by setting the `stream_id` to `None`:
 
 ```python
 logger.warning("Something went wrong!", extra=RateLimit(stream_id=None))
 ```
 
 ## Usage examples
 
@@ -105,15 +105,15 @@
 WARNING:__main__:Issue!
 ```
 
 ### Dynamically override configuration options
 
 Some options set during creation of the initial filter can be overridden for individual log calls. This is done by adding the `extra` parameter to any specific log call, e.g.:
 ```python
-# Override the rate limit period for this specific log call
+# Override the rate-limit period for this specific log call
 logger.warning("Test1", extra=RateLimit(stream_id="stream1", period_sec=30))
 # Override the allow_next_n value for a set of logs in the same stream so that this group of logs don't restrict one
 # another from occuring consecutively
 logger.warning("Test", extra=RateLimit(stream_id="stream2", allow_next_n=2))
 logger.info("Extra", extra=RateLimit(stream_id="stream2"))
 logger.debug("Info", extra=RateLimit(stream_id="stream2"))
 ```
```

### Comparing `log_rate_limit-1.2.2/log_rate_limit/log_rate_limit.py` & `log_rate_limit-1.3.0/log_rate_limit/log_rate_limit.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,14 +22,29 @@
     NONE: DefaultStreamID = None
     # Default stream ID to the log's file and line number location.
     FILE_LINE_NO: DefaultStreamID = "file_line_no"
     # Default stream ID to the log message.
     LOG_MESSAGE: DefaultStreamID = "log_message"
 
 
+class StreamInfo:
+    """All information kept per-stream."""
+
+    def __init__(self) -> None:
+        """Construct object with default values."""
+        super().__init__()
+        # Next time at which rate-limiting no longer applies to each stream. Initial default of 0 will always fire
+        # since it specifies the Unix epoch timestamp.
+        self.next_valid_time: float = 0.0
+        # Count of the number of logs suppressed/skipped in each stream.
+        self.skipped_log_count: int = 0
+        # Count of extra logs left that can ignore rate-limit based on allow_next_n.
+        self.count_logs_left: int = 0
+
+
 class StreamRateLimitFilter(logging.Filter):
     """Filter out each "stream" of logs so they don't happen too fast within a given period of time.
 
     Logs can be separated into "streams" so that the rate-limit only applies to logs in the same stream. Also, the
     trigger times for each stream can be accessed and controlled (read or written) in case there are other non-logging
     events that you want to rate-limit in a similar fasion (or possibly even in the same stream as some other logs).
     """
@@ -39,14 +54,20 @@
         period_sec: float,
         allow_next_n: int = 0,
         default_stream_id: DefaultStreamID = DefaultSID.LOG_MESSAGE,
         filter_undefined: bool = False,
         summary: bool = True,
         summary_msg: str = " + skipped {numskip} logs due to rate-limiting",
         name: str = "",
+        expire_check_sec: int = 60,
+        expire_offset_sec: int = 900,
+        expire_msg: str = " [Previous logs] {numskip} logs were skipped"
+        ' (and expired after {expire_time_sec}s) for stream: "{stream_id}"',
+        stream_id_max_len: Optional[int] = None,
+        print_config: bool = False,
     ):
         """Construct a logging filter that will limit rate of logs.
 
         Parameters
         ----------
         period_sec
             The minimum time period (in seconds) allowed between log messages of the same stream.
@@ -74,30 +95,57 @@
             suppressed/skipped.
         summary_msg
             The summary message used to summarise logs that were suppressed/skipped.
         name
             Filter names form a logger hierarchical where they apply only to current or lower levels, e.g. with name
             "A.B" it will apply to "A.B" and also "A.B.C", "A.B.C.D", etc. but not to "A". See Python docs:
             https://docs.python.org/3/library/logging.html#filter-objects
+        expire_check_sec
+            We expire log stream information after some time to decrease memory usage. This value determines how
+            regularly we check for expired data (which might rarely have some performance impact). Default is set to
+            once per minute.
+        expire_offset_sec
+            This offset is the number of seconds after the log rate limit has been reached for a specific stream
+            before any info we store about the stream will expire. Default is set to 15 minutes.
+        expire_msg
+            The message used to summarise logs that were expired.
+        stream_id_max_len
+            If set, this defines a maximum length for the stream names (stream_id strings). If set to None (the
+            default) then there is no limit. Be aware that while setting this would help limit memory usage, it will
+            also make it very easy for similar log messages to get assigned to the same stream and get confused with
+            each other.
+        print_config
+            At initialisation, print the configuration options provided to this class.
         """
         super().__init__(name)
+        assert period_sec >= 0
+        assert allow_next_n >= 0
+        assert expire_check_sec >= 0
+        assert stream_id_max_len is None or stream_id_max_len > 0
         # These values are all defaults that can be temporarily overriden on-the-fly.
         self._period_sec = period_sec
         self._allow_next_n = allow_next_n
         self._filter_undefined = filter_undefined
         self._default_stream_id = default_stream_id
         self._summary = summary
         self._summary_msg = summary_msg
-        # Next time at which rate-limiting no longer applies to each stream. Initial default of 0 will always fire
-        # since it specifies the Unix epoch timestamp.
-        self._next_valid_time: Dict[StreamID, float] = defaultdict(float)
-        # Count of the number of logs suppressed/skipped in each stream.
-        self._skipped_log_count: Dict[StreamID, int] = defaultdict(int)
-        # Count of extra logs left that can ignore rate-limit based on allow_next_n.
-        self._count_logs_left: Dict[StreamID, int] = defaultdict(int)
+        self._expire_check_sec = expire_check_sec
+        self._expire_offset_sec = expire_offset_sec
+        self._expire_msg = expire_msg
+        self._stream_id_max_len = stream_id_max_len
+
+        # Global coutner of when next to check expired streams.
+        self._next_expire_check_time: Optional[float] = None
+        # All data kept in memory for each stream.
+        self._streams: Dict[StreamID, StreamInfo] = defaultdict(StreamInfo)
+        if print_config:
+            self._print_config()
+
+    def _print_config(self) -> None:
+        print(self.__dict__)
 
     def _get(self, record: logging.LogRecord, attribute: str, default_val: Any = None) -> Any:
         if hasattr(record, attribute):
             return getattr(record, attribute)
         return default_val
 
     def trigger(
@@ -138,15 +186,15 @@
         ------
         True if enough time has passed that this stream is able to trigger.
         """
         if current_time is None:
             current_time = time.time()
         # Allow if enough time has passed since the last log message for this stream (or if this is the first message
         # for this stream - in which case next_valid_time should get the default value of 0).
-        next_valid_time = self._next_valid_time[stream_id]
+        next_valid_time = self._streams[stream_id].next_valid_time
         return current_time >= next_valid_time
 
     def reset_trigger(
         self,
         stream_id: StreamID,
         override_period_sec: Optional[float] = None,
         current_time: Optional[float] = None,
@@ -163,85 +211,168 @@
         current_time
             Optional parameter that can be used to call this function for different points in time.
         """
         if override_period_sec is None:
             override_period_sec = self._period_sec
         if current_time is None:
             current_time = time.time()
-        self._next_valid_time[stream_id] = current_time + override_period_sec
+        self._streams[stream_id].next_valid_time = current_time + override_period_sec
+
+    def _get_default_stream_id(self, record: logging.LogRecord) -> StreamID:
+        default_stream_id = None
+        if self._default_stream_id == DefaultSID.FILE_LINE_NO:
+            # Assign unique default stream_ids.
+            default_stream_id = f"{record.filename}:{record.lineno}"
+        if self._default_stream_id == DefaultSID.LOG_MESSAGE:
+            default_stream_id = record.getMessage()
+        return default_stream_id
+
+    def _check_expiry(self, expire_offset_sec: float, expire_msg: str) -> str:
+        current_time = time.time()
+        # Global check - not specifically related to the current stream being processed, and could affect other
+        # streams.
+        srl_expire_note = ""
+        if self._next_expire_check_time is None or current_time > self._next_expire_check_time:
+            # Check and clear from memory any stream data that has expired.
+            srl_expire_note = self.clear_old_streams(expire_offset_sec, expire_msg=expire_msg)
+            self._next_expire_check_time = current_time + self._expire_check_sec
+        return srl_expire_note
 
     def filter(self, record: logging.LogRecord) -> bool:
         """Filter function that determines if given log message will be displayed.
 
         Returns
         -------
         True if log should be shown or else False if log should be skipped/hidden/filtered out.
         """
         global TEST_MODE
         if TEST_MODE:
             _test_default_overrides(record)
 
-        default_stream_id = None
-        if self._default_stream_id == DefaultSID.FILE_LINE_NO:
-            # Assign unique default stream_ids.
-            default_stream_id = f"{record.filename}:{record.lineno}"
-        if self._default_stream_id == DefaultSID.LOG_MESSAGE:
-            default_stream_id = record.getMessage()
+        default_stream_id = self._get_default_stream_id(record)
         # Get variables that can be dynamically overridden, or else use init-defaults.
         stream_id = self._get(record, "stream_id", default_stream_id)
         period_sec = self._get(record, "period_sec", self._period_sec)
         allow_next_n = self._get(record, "allow_next_n", self._allow_next_n)
         summary = self._get(record, "summary", self._summary)
         summary_msg = self._get(record, "summary_msg", self._summary_msg)
+        expire_offset_sec = self._get(record, "expire_offset_sec", self._expire_offset_sec)
+        expire_msg = self._get(record, "expire_msg", self._expire_msg)
 
-        skip_count = self._skipped_log_count[stream_id]
-        count_left = self._count_logs_left[stream_id]
-
-        # Add any extra attributes we might add to record.
+        # If configured, limit the length of stream_id.
+        if stream_id is not None:
+            # string[0:None] will just select the whole string.
+            stream_id = stream_id[0 : self._stream_id_max_len]
+
+        # Run expiry checks before accessing any fields from the current stream.
+        srl_expire_note = self._check_expiry(expire_offset_sec, expire_msg)
+
+        # Add any extra attributes we might add to record as this allows user's own log formatting to use it (if
+        # they're only sometimes present, then string formatting will fail when attributes aren't found). All
+        # attributes added by this filter will be prepended with "srl_" (for Stream Rate Limit).
         record.srl_summary_note = ""
+        record.srl_expire_note = srl_expire_note
+        # Log any expired messages after the current message.
+        record.msg = f"{record.msg}{srl_expire_note}"
 
         if stream_id is None and not self._filter_undefined:
             return True
 
+        # Fetch stream that we'll use for this log message.
+        stream = self._streams[stream_id]
+
         # Inner function to prevent code duplication.
-        def prep_to_allow_msg(reset_all: bool = True) -> None:
+        def prep_to_allow_msg() -> None:
+            skip_count = stream.skipped_log_count
             # This value might be reset momentarily.
-            self._count_logs_left[stream_id] -= 1
+            stream.count_logs_left -= 1
             # See if we should generate a summary note.
             if skip_count > 0:
                 # Change message to indicate a summary of skipped logs.
-                # NOTE: period_sec might be incorrect if it is, or has been, overridden (either currently or recently).
+                # NOTE: period_sec might be incorrect if it is, or has been, overridden (either currently or
+                # recently).
                 added_msg = summary_msg.format(numskip=skip_count, stream_id=stream_id, period_sec=period_sec)
                 summary_note = f"\n{added_msg}"
                 # Always add summary_note attribute.
                 record.srl_summary_note = summary_note
                 # Only append summary to log message if summary option is set.
                 if summary:
                     record.msg = f"{record.msg}{summary_note}"
-            # Reset counters and timers.
-            if reset_all:
-                self._skipped_log_count[stream_id] = 0
-                self._count_logs_left[stream_id] = allow_next_n
-                self.reset_trigger(stream_id, period_sec)
 
         # Allow if enough time has passed since the last log message for this stream was triggered.
         if self.should_trigger(stream_id):
             prep_to_allow_msg()
+            # Reset all counters and timers.
+            stream.skipped_log_count = 0
+            stream.count_logs_left = allow_next_n
+            self.reset_trigger(stream_id, period_sec)
             return True
 
         # Allow if the "allow next N" option applies and this message is within a count of N of the last allowed
         # message (and previous criteria were not met).
+        count_left = stream.count_logs_left
         if count_left > 0:
-            prep_to_allow_msg(reset_all=False)
+            prep_to_allow_msg()
+            return True
+
+        # Once we've reached here, we'll definitely skip the current log message.
+        stream.skipped_log_count += 1
+
+        # We introduce our own log message if current message was skipped, but other messages were expired during
+        # this processing.
+        if srl_expire_note != "":
+            record.msg = srl_expire_note
             return True
 
-        # Once we've reached here, we'll definitely skip this log message.
-        self._skipped_log_count[stream_id] += 1
         return False
 
+    def clear_old_streams(
+        self, expire_time_sec: float = 7200, current_time: Optional[float] = None, expire_msg: str = ""
+    ) -> str:
+        """Clear old stream IDs to free up memory (in case of many large stream ID strings).
+
+        Parameters
+        ----------
+        expire_time_sec
+            Only clear out streams that haven't been reset in this period of time (in seconds). This is an amount of
+            time added after rate-limiting no longer applies anyway. Highly recommended to be a positive number.
+        current_time
+            Optional parameter that can be used to call this function for different points in time.
+        expire_msg
+            Message format of logs used to report expired streams.
+        """
+        if current_time is None:
+            current_time = time.time()
+
+        # We build a string of keys to remove first since the alternative of looping through the dictionary and
+        # removing keys will require that we iterate through a copy of the dictionary's keys which is exactly
+        # the part which might be using excessive memory.
+        keys_to_remove = []
+        for stream_id in self._streams.keys():
+            next_valid_time = self._streams[stream_id].next_valid_time
+            # Daylight savings or other time changes might break or trigger this check during the transition period?
+            if (next_valid_time + expire_time_sec) < current_time:
+                keys_to_remove.append(stream_id)
+
+        expire_note = ""
+        for stream_id in keys_to_remove:
+            skip_count = self._streams[stream_id].skipped_log_count
+            # If any logs were skipped, then we log it before clearing the cache.
+            if skip_count > 0:
+                added_msg = expire_msg.format(numskip=skip_count, stream_id=stream_id, expire_time_sec=expire_time_sec)
+                expire_note += f"\n{added_msg}"
+            # Remove keys
+            del self._streams[stream_id]
+
+        return expire_note
+
+    def _key_size(self) -> int:
+        """Get an estimate of the number of keys stored in memory."""
+        return len(self._streams)
+
 
 class RateLimit(TypedDict, total=False):
     """Easily construct a logging "extra" dict with rate-limiting parameters."""
 
     # Manually define a stream_id for this logging record. A value of `None` is valid and has specific meaning based on
     # the filter's configuration options.
     stream_id: StreamID
```

### Comparing `log_rate_limit-1.2.2/pyproject.toml` & `log_rate_limit-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "log-rate-limit"
-version = "1.2.2"
+version = "1.3.0"
 description = "Limit excessive log output with Python's standard logging framework."
 authors = ["Simon Muller <samullers@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/samuller/log-rate-limit"
 repository = "https://github.com/samuller/log-rate-limit"
 keywords = ["logging", "log", "limit", "rate"]
 classifiers = [
@@ -32,7 +32,11 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 # Change black's default line length from 88 to 120 characters.
 line-length = 120
+
+[tool.coverage.html]
+# See https://pytest-cov.readthedocs.io/en/latest/contexts.html
+show_contexts = true
```

### Comparing `log_rate_limit-1.2.2/setup.py` & `log_rate_limit-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: log-rate-limit
+Version: 1.3.0
+Summary: Limit excessive log output with Python's standard logging framework.
+Home-page: https://github.com/samuller/log-rate-limit
+Keywords: logging,log,limit,rate
+Author: Simon Muller
+Author-email: samullers@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Logging
+Project-URL: Repository, https://github.com/samuller/log-rate-limit
+Description-Content-Type: text/markdown
 
-packages = \
-['log_rate_limit']
+# log-rate-limit - limit excessive log output
 
-package_data = \
-{'': ['*']}
+[![PyPI Version](https://img.shields.io/pypi/v/log-rate-limit)](https://pypi.org/project/log-rate-limit/)
+[![Build Status](https://github.com/samuller/log-rate-limit/actions/workflows/tests.yml/badge.svg)](https://github.com/samuller/log-rate-limit/actions/workflows/tests.yml)
+[![Code Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)](https://github.com/samuller/pgmerge/actions)
+[![Checked with mypy](https://img.shields.io/badge/mypy-strict-blue)](http://mypy-lang.org/)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-black)](https://black.readthedocs.io/en/stable/)
 
-setup_kwargs = {
-    'name': 'log-rate-limit',
-    'version': '1.2.2',
-    'description': "Limit excessive log output with Python's standard logging framework.",
-    'long_description': '# log-rate-limit - limit excessive log output\n\n[![PyPI Version](https://img.shields.io/pypi/v/log-rate-limit)](https://pypi.org/project/log-rate-limit/)\n[![Build Status](https://github.com/samuller/log-rate-limit/actions/workflows/tests.yml/badge.svg)](https://github.com/samuller/log-rate-limit/actions/workflows/tests.yml)\n[![Code Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)](https://github.com/samuller/pgmerge/actions)\n[![Checked with mypy](https://img.shields.io/badge/mypy-strict-blue)](http://mypy-lang.org/)\n[![Formatted with black](https://img.shields.io/badge/code%20style-black-black)](https://black.readthedocs.io/en/stable/)\n\nA [logging filter](https://docs.python.org/3/library/logging.html#filter-objects) using Python\'s standard logging mechanisms to rate-limit logs - i.e. suppress logs when they are being output too fast.\n\nLog commands are grouped into separate **streams** that will each have their own rate limitation applied without affecting the logs in other streams. By default every log message is assigned a unique stream so that only repeated log messages will be suppressed.\n\nHowever, logs can also be assigned streams manually to achieve various outcomes:\n- A log can be assigned to an undefined/`None` stream so that rate-limiting doesn\'t apply to it.\n- Logs in different parts of the code can be grouped into the same stream so that they share a rate-limit, e.g. when they all trigger due to the same issue and only some are needed to indicate it.\n\nThe default can also be changed so that rate-limiting is disabled by default and only applies to logs for which a `stream_id` has been manually set.\n\n## Quick usage\n\nImport the filter:\n\n```python\nfrom log_rate_limit import StreamRateLimitFilter, RateLimit\n```\n\nUse the filter with your `logger`. With default parameters it will rate limit all repetitive log message:\n\n```python\nlogger.addFilter(StreamRateLimitFilter(period_sec=30))\n```\n\nAll logs on `logger` will now be rate limited, but this can be disabled per-log by setting the `stream_id` to `None`:\n\n```python\nlogger.warning("Something went wrong!", extra=RateLimit(stream_id=None))\n```\n\n## Usage examples\n\n### Rate-limiting by default\n\nExample of rate-limiting with default options where each log message is assigned to its own stream:\n```python\nimport time\nimport logging\nfrom log_rate_limit import StreamRateLimitFilter, RateLimit\n# Setup logging\nlogging.basicConfig()\nlogger = logging.getLogger(__name__)\n\n# Add our filter\nlogger.addFilter(StreamRateLimitFilter(period_sec=1))\n# Log many warnings\nfor _ in range(100):\n    logger.warning("Wolf!")\nfor i in range(100):\n    logger.warning("No really, a wolf!")\n    if i == 98:\n        time.sleep(1)\n# Prevent rate-limited by setting/overriding the stream to be undefined (None)\nfor _ in range(3):\n    logger.warning("Sheep!", extra=RateLimit(stream_id=None))\n``` \nWhich only outputs the following:\n```log\nWARNING:__main__:Wolf!\nWARNING:__main__:No really, a wolf!\nWARNING:__main__:No really, a wolf!\n+ skipped 98 logs due to rate-limiting\nWARNING:__main__:Sheep!\nWARNING:__main__:Sheep!\nWARNING:__main__:Sheep!\n```\nNote that (unless overridden) logs were only repeated after the `sleep()` call, and the repeated log also included an extra summary message added afterwards.\n\nWhen we override rate-limiting above, you\'ll see our filter reads dynamic configs from logging\'s `extra` parameter.\n\n> Be very careful not to forget the `extra=` name part of the argument, as then the logging framework will assume you\'re passing arguments meant for formatting in the logging message and your options will silently be ignored!\n\n### Rate-limit only when specified\n\nIf you want most of your logs to be unaffected and you only have some you want to specifically rate-limit, then you can do the following:\n```python\nimport logging\nfrom log_rate_limit import StreamRateLimitFilter, RateLimit\n# Setup logging\nlogging.basicConfig(level=logging.INFO)\nlogger = logging.getLogger(__name__)\n\n# Add our filter, but don\'t assign unique streams to logs by default\nlogger.addFilter(StreamRateLimitFilter(period_sec=1, default_stream_id=None))\n# Normal logs are now not rate-limited\nfor i in range(3):\n    logger.info(f"Status update: {i}")\n# Only those we manually assign a stream will be rate-limited\nfor _ in range(3):\n    logger.warning("Issue!", extra=RateLimit(stream_id="issue"))\n```\nWhich only outputs the following:\n```log\nINFO:__main__:Status update: 0\nINFO:__main__:Status update: 1\nINFO:__main__:Status update: 2\nWARNING:__main__:Issue!\n```\n\n### Dynamically override configuration options\n\nSome options set during creation of the initial filter can be overridden for individual log calls. This is done by adding the `extra` parameter to any specific log call, e.g.:\n```python\n# Override the rate limit period for this specific log call\nlogger.warning("Test1", extra=RateLimit(stream_id="stream1", period_sec=30))\n# Override the allow_next_n value for a set of logs in the same stream so that this group of logs don\'t restrict one\n# another from occuring consecutively\nlogger.warning("Test", extra=RateLimit(stream_id="stream2", allow_next_n=2))\nlogger.info("Extra", extra=RateLimit(stream_id="stream2"))\nlogger.debug("Info", extra=RateLimit(stream_id="stream2"))\n```\n\nIf you want to set custom options for a large group of log calls without repeatedly adding the `extra` parameter, it\'s possible to use a [LoggerAdapter](https://docs.python.org/3/library/logging.html#loggeradapter-objects):\n```python\nimport logging\nfrom log_rate_limit import StreamRateLimitFilter, RateLimit\n\nlogging.basicConfig(level=logging.INFO)\nlogger = logging.getLogger(__name__)\n# Add our filter\nlogger.addFilter(StreamRateLimitFilter(period_sec=1))\n\n# Use LoggerAdapter to assign additional "extra" parameters to all calls using this logger\nglobal_extra = RateLimit(stream_id="custom_stream", period_sec=20)\nlogger = logging.LoggerAdapter(logger, global_extra)\n# Log many warnings\nfor _ in range(100):\n    logger.warning("Wolf!")\nfor i in range(100):\n    logger.warning("No really, a wolf!")\n```\nWhich merely outputs:\n```log\nWARNING:__main__:Wolf!\n```\nSince both log calls are in the same stream.\n\nAlternatively (to a LoggerAdapter), custom options can also be added by writing your own [logging.Filter](https://docs.python.org/3.8/howto/logging-cookbook.html#using-filters-to-impart-contextual-information).\n\n### Dynamic stream ID\n\nDynamic stream IDs can be assigned based on any criteria you want, e.g.:\n\n```python\nlogger.warning(f"Error occured on device {device_id}!", extra=RateLimit(stream_id=f"error_on_{device_id}"))\n```\n\n## Installation\n\n### Install from PyPI\n\nWith `Python 3` installed on your system, you can run:\n\n    pip install log-rate-limit\n\nTo test that installation worked, you can run:\n\n    python -c "import log_rate_limit"\n\nand you can uninstall at any time with:\n\n    pip uninstall log-rate-limit\n\nTo install with poetry:\n\n    poetry add log-rate-limit\n\n### Install from Github\n\nTo install the newest code directly from Github:\n\n    pip install git+https://github.com/samuller/log-rate-limit\n',
-    'author': 'Simon Muller',
-    'author_email': 'samullers@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/samuller/log-rate-limit',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+A [logging filter](https://docs.python.org/3/library/logging.html#filter-objects) using Python's standard logging mechanisms to rate-limit logs - i.e. suppress logs when they are being output too fast.
 
+Log commands are grouped into separate **streams** that will each have their own rate limitation applied without affecting the logs in other streams. By default every log message is assigned a unique stream so that only repeated log messages will be suppressed.
+
+However, logs can also be assigned streams manually to achieve various outcomes:
+- A log can be assigned to an undefined/`None` stream so that rate-limiting doesn't apply to it.
+- Logs in different parts of the code can be grouped into the same stream so that they share a rate-limit, e.g. when they all trigger due to the same issue and only some are needed to indicate it.
+
+The default can also be changed so that rate-limiting is disabled by default and only applies to logs for which a `stream_id` has been manually set.
+
+## Quick usage
+
+Import the filter:
+
+```python
+from log_rate_limit import StreamRateLimitFilter, RateLimit
+```
+
+Use the filter with your `logger` - with default parameters it will rate-limit all repetitive log messages:
+
+```python
+logger.addFilter(StreamRateLimitFilter(period_sec=30))
+```
+
+All logs on `logger` will now be rate-limited, but this can be disabled per-log by setting the `stream_id` to `None`:
+
+```python
+logger.warning("Something went wrong!", extra=RateLimit(stream_id=None))
+```
+
+## Usage examples
+
+### Rate-limiting by default
+
+Example of rate-limiting with default options where each log message is assigned to its own stream:
+```python
+import time
+import logging
+from log_rate_limit import StreamRateLimitFilter, RateLimit
+# Setup logging
+logging.basicConfig()
+logger = logging.getLogger(__name__)
+
+# Add our filter
+logger.addFilter(StreamRateLimitFilter(period_sec=1))
+# Log many warnings
+for _ in range(100):
+    logger.warning("Wolf!")
+for i in range(100):
+    logger.warning("No really, a wolf!")
+    if i == 98:
+        time.sleep(1)
+# Prevent rate-limited by setting/overriding the stream to be undefined (None)
+for _ in range(3):
+    logger.warning("Sheep!", extra=RateLimit(stream_id=None))
+``` 
+Which only outputs the following:
+```log
+WARNING:__main__:Wolf!
+WARNING:__main__:No really, a wolf!
+WARNING:__main__:No really, a wolf!
++ skipped 98 logs due to rate-limiting
+WARNING:__main__:Sheep!
+WARNING:__main__:Sheep!
+WARNING:__main__:Sheep!
+```
+Note that (unless overridden) logs were only repeated after the `sleep()` call, and the repeated log also included an extra summary message added afterwards.
+
+When we override rate-limiting above, you'll see our filter reads dynamic configs from logging's `extra` parameter.
+
+> Be very careful not to forget the `extra=` name part of the argument, as then the logging framework will assume you're passing arguments meant for formatting in the logging message and your options will silently be ignored!
+
+### Rate-limit only when specified
+
+If you want most of your logs to be unaffected and you only have some you want to specifically rate-limit, then you can do the following:
+```python
+import logging
+from log_rate_limit import StreamRateLimitFilter, RateLimit
+# Setup logging
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
+# Add our filter, but don't assign unique streams to logs by default
+logger.addFilter(StreamRateLimitFilter(period_sec=1, default_stream_id=None))
+# Normal logs are now not rate-limited
+for i in range(3):
+    logger.info(f"Status update: {i}")
+# Only those we manually assign a stream will be rate-limited
+for _ in range(3):
+    logger.warning("Issue!", extra=RateLimit(stream_id="issue"))
+```
+Which only outputs the following:
+```log
+INFO:__main__:Status update: 0
+INFO:__main__:Status update: 1
+INFO:__main__:Status update: 2
+WARNING:__main__:Issue!
+```
+
+### Dynamically override configuration options
+
+Some options set during creation of the initial filter can be overridden for individual log calls. This is done by adding the `extra` parameter to any specific log call, e.g.:
+```python
+# Override the rate-limit period for this specific log call
+logger.warning("Test1", extra=RateLimit(stream_id="stream1", period_sec=30))
+# Override the allow_next_n value for a set of logs in the same stream so that this group of logs don't restrict one
+# another from occuring consecutively
+logger.warning("Test", extra=RateLimit(stream_id="stream2", allow_next_n=2))
+logger.info("Extra", extra=RateLimit(stream_id="stream2"))
+logger.debug("Info", extra=RateLimit(stream_id="stream2"))
+```
+
+If you want to set custom options for a large group of log calls without repeatedly adding the `extra` parameter, it's possible to use a [LoggerAdapter](https://docs.python.org/3/library/logging.html#loggeradapter-objects):
+```python
+import logging
+from log_rate_limit import StreamRateLimitFilter, RateLimit
+
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+# Add our filter
+logger.addFilter(StreamRateLimitFilter(period_sec=1))
+
+# Use LoggerAdapter to assign additional "extra" parameters to all calls using this logger
+global_extra = RateLimit(stream_id="custom_stream", period_sec=20)
+logger = logging.LoggerAdapter(logger, global_extra)
+# Log many warnings
+for _ in range(100):
+    logger.warning("Wolf!")
+for i in range(100):
+    logger.warning("No really, a wolf!")
+```
+Which merely outputs:
+```log
+WARNING:__main__:Wolf!
+```
+Since both log calls are in the same stream.
+
+Alternatively (to a LoggerAdapter), custom options can also be added by writing your own [logging.Filter](https://docs.python.org/3.8/howto/logging-cookbook.html#using-filters-to-impart-contextual-information).
+
+### Dynamic stream ID
+
+Dynamic stream IDs can be assigned based on any criteria you want, e.g.:
+
+```python
+logger.warning(f"Error occured on device {device_id}!", extra=RateLimit(stream_id=f"error_on_{device_id}"))
+```
+
+## Installation
+
+### Install from PyPI
+
+With `Python 3` installed on your system, you can run:
+
+    pip install log-rate-limit
+
+To test that installation worked, you can run:
+
+    python -c "import log_rate_limit"
+
+and you can uninstall at any time with:
+
+    pip uninstall log-rate-limit
+
+To install with poetry:
+
+    poetry add log-rate-limit
+
+### Install from Github
+
+To install the newest code directly from Github:
+
+    pip install git+https://github.com/samuller/log-rate-limit
 
-setup(**setup_kwargs)
```

