# Comparing `tmp/trongrid_extractor-1.0.0.tar.gz` & `tmp/trongrid_extractor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-1.0.0.tar", max compression
+gzip compressed data, was "trongrid_extractor-1.1.0.tar", max compression
```

## Comparing `trongrid_extractor-1.0.0.tar` & `trongrid_extractor-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2082 2023-07-21 04:07:56.103083 trongrid_extractor-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-1.0.0/LICENSE
--rw-r--r--   0        0        0     4285 2023-07-20 21:33:51.204396 trongrid_extractor-1.0.0/README.md
--rw-r--r--   0        0        0      710 2023-07-21 04:09:20.260330 trongrid_extractor-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      664 2023-07-07 20:10:24.551800 trongrid_extractor-1.0.0/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-21 03:53:28.444528 trongrid_extractor-1.0.0/trongrid_extractor/api.py
--rw-r--r--   0        0        0      256 2023-07-02 01:07:20.257342 trongrid_extractor-1.0.0/trongrid_extractor/config.py
--rw-r--r--   0        0        0     2556 2023-07-07 17:52:23.460205 trongrid_extractor-1.0.0/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     3281 2023-07-07 20:10:24.552907 trongrid_extractor-1.0.0/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2282 2023-07-21 03:57:18.162746 trongrid_extractor-1.0.0/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-1.0.0/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      328 2023-07-02 00:33:07.504060 trongrid_extractor-1.0.0/trongrid_extractor/helpers/rich_helpers.py
--rw-r--r--   0        0        0      452 2023-07-07 20:02:09.527800 trongrid_extractor-1.0.0/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1726 2023-07-02 01:02:30.797593 trongrid_extractor-1.0.0/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     4747 2023-07-20 22:04:21.872581 trongrid_extractor-1.0.0/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     1781 2023-07-01 22:52:26.788565 trongrid_extractor-1.0.0/trongrid_extractor/request_params.py
--rw-r--r--   0        0        0     5248 2023-07-21 03:55:50.173322 trongrid_extractor-1.0.0/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4687 2023-07-07 18:41:19.685481 trongrid_extractor-1.0.0/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 trongrid_extractor-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2194 2023-07-28 22:19:01.255021 trongrid_extractor-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-07-28 20:52:50.935725 trongrid_extractor-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4142 2023-07-28 20:56:58.771383 trongrid_extractor-1.1.0/README.md
+-rw-r--r--   0        0        0      712 2023-07-28 22:19:01.263890 trongrid_extractor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2023-07-28 20:56:58.788236 trongrid_extractor-1.1.0/trongrid_extractoor/__init__.py
+-rw-r--r--   0        0        0     6315 2023-07-28 20:56:58.785597 trongrid_extractor-1.1.0/trongrid_extractoor/api.py
+-rw-r--r--   0        0        0      257 2023-07-28 20:56:58.785694 trongrid_extractor-1.1.0/trongrid_extractoor/config.py
+-rw-r--r--   0        0        0     2661 2023-07-28 21:06:25.963567 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     3285 2023-07-28 20:56:58.785735 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2892 2023-07-28 20:56:58.839083 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-07-28 20:52:51.688337 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      328 2023-07-28 20:52:51.688174 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/rich_helpers.py
+-rw-r--r--   0        0        0      453 2023-07-28 20:56:58.785753 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1727 2023-07-28 20:56:58.843479 trongrid_extractor-1.1.0/trongrid_extractoor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     4751 2023-07-28 20:56:58.785673 trongrid_extractor-1.1.0/trongrid_extractoor/progress_tracker.py
+-rw-r--r--   0        0        0     1784 2023-07-28 20:56:58.785644 trongrid_extractor-1.1.0/trongrid_extractoor/request_params.py
+-rw-r--r--   0        0        0     5253 2023-07-28 20:56:58.785565 trongrid_extractor-1.1.0/trongrid_extractoor/response.py
+-rw-r--r--   0        0        0     4692 2023-07-28 20:56:58.785489 trongrid_extractor-1.1.0/trongrid_extractoor/trc20_txn.py
+-rw-r--r--   0        0        0     4784 1970-01-01 00:00:00.000000 trongrid_extractor-1.1.0/PKG-INFO
```

### Comparing `trongrid_extractor-1.0.0/CHANGELOG.md` & `trongrid_extractor-1.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# NEXT RELEASE
+
+# 1.1.0
+* Add `parse_written_at_from_filename()` method
+* `TCNH` and `wstUSDT` token shorthand
+
 # 1.0.0
 * As of mid July 2023 TronGrid seems to have repaired their API so it no longer just gives up after returning 5 pages of responses. This dramatically simplifies the code in this package.
 * Guarantee there is always a CSV with a header row at the end even if there's no rows returned by query.
 * enable `jUSDC` and `stUSDT` token shorthand symbols
 
 # 0.4.0
 * `--resume` option automatically determines the token address from the CSV
```

### Comparing `trongrid_extractor-1.0.0/README.md` & `trongrid_extractor-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,44 +10,36 @@
 Set `LOG_LEVEL=DEBUG` to get debug logging.
 
 #### Compiling Multiple CSVs To One File
 There is a script that will collect all CSVs with a given symbol/address prefix and uniquify the rows into a single CSV. Run `scripts/compile_csvs.py --help` to see the usage options.
 
 ## As Package
 ```python
-from trongrid_extractor.api import Api
+from trongrid_extractoor.api import Api
 
 Api().events_for_token('Tf2939nbd23kmdo')
 ```
 
 `events_for_token()` hits the `contracts/[CONTRACT_ADDRESS]/events` endpoint and can pull all transfers for a given contract by filtering for `event_name=Transfer`. Other endpoints like `contracts/[CONTRACT_ADDRESS]/transactions` don't seem to really work.
 
+
 # Trongrid Documentation, Quirks, Etc.
+**UPDATE: cirac July 2023 Trongrid appears to have fixed this issue and the `next` URL will actually give you more than 5 pages.**
+
 When you make an API request to TronGrid they return you a page of results. If there are more than the page size (200 here) then the response includes a `next` key that has a URL you can hit to get the next page. Sounds convenient, right? Except it doesn't work. After 5 pages TronGrid will tell you your timespan is too big and please try again. This package is written to go around this "quirk" by backing up the `max_timestamp` parameter when it can't page any more.
 
 * [Trongrid API documentation](https://developers.tron.network/v4.0/reference/note)
 
-### Paging Completion
-It seems like (not 100% confident) when a given query is finished paging it returns JSON with a `page_size` value of `0` like this:
-```json
-{
-    'data': [],
-    'success': True,
-    'meta': {
-        'at': 1687935779799,
-        'page_size': 0
-    }
-}
-```
 
 # Contributing
 This project was developed with `poetry` and as such is probably easier to work with using `poetry` to manage dependencies in the dev environment. Install with:
 ```
 poetry install --with=dev
 ```
+
 ## Running Tests
 ```
 pytest
 ```
 
 ## Publishing to PyPi
 ### Configuration
@@ -81,8 +73,8 @@
    ```
     INFO       Returning 1000 transactions from _rescue_extraction(), modified params in place.                                    api.py:191
     INFO     Writing 1000 rows to 'events_USDD_written_2023-06-28T04.22.00.csv'...                                           csv_helper.py:17
     [06/28/23 10:22:34] INFO       Removed 200 duplicate transactions...                                                                   progress_tracker.py:47
     WARNING  0 txns found. We seem to be stuck at 2023-01-26T03:18:54+00:00.                                                       api.py:103
     WARNING    Last request params: {'only_confirmed': 'true', 'limit': 200, 'min_timestamp': 1483228800000.0, 'max_timestamp':    api.py:104
             1674703134000.0, 'event_name': 'Transfer'}
-   ```
+    ```
```

### Comparing `trongrid_extractor-1.0.0/pyproject.toml` & `trongrid_extractor-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "1.0.0"
+version = "1.1.0"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
-packages = [{include = "trongrid_extractor"}]
+packages = [{include = "trongrid_extractoor"}]
 homepage = "https://chainargos.com"
 
 include = [
     "CHANGELOG.md",
     "LICENSE",
 ]
 
@@ -27,8 +27,8 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
-extract_tron_transactions = 'trongrid_extractor:extract_tron_transactions'
+extract_tron_transactions = 'trongrid_extractoor:extract_tron_transactions'
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/__init__.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from os import environ
 
 from rich.logging import RichHandler
 
-from trongrid_extractor.api import Api
-from trongrid_extractor.helpers.argument_parser import parse_args
-from trongrid_extractor.helpers.string_constants import PACKAGE_NAME
-from trongrid_extractor.helpers.time_helpers import MAX_TIME, TRON_LAUNCH_TIME, str_to_timestamp
+from trongrid_extractoor.api import Api
+from trongrid_extractoor.helpers.argument_parser import parse_args
+from trongrid_extractoor.helpers.string_constants import PACKAGE_NAME
+from trongrid_extractoor.helpers.time_helpers import MAX_TIME, TRON_LAUNCH_TIME, str_to_timestamp
 
 
 def extract_tron_transactions():
     """When called by the installed script use the Rich logger."""
     args = parse_args()
 
     Api().events_for_token(
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/api.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import tempfile
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pendulum
 from pendulum import DateTime
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.address_helpers import is_contract_address
-from trongrid_extractor.helpers.csv_helper import *
-from trongrid_extractor.helpers.string_constants import *
-from trongrid_extractor.helpers.time_helpers import *
-from trongrid_extractor.progress_tracker import ProgressTracker
-from trongrid_extractor.request_params import MAX_TRADES_PER_CALL, RequestParams
-from trongrid_extractor.response import Response
-from trongrid_extractor.trc20_txn import Trc20Txn
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.address_helpers import is_contract_address
+from trongrid_extractoor.helpers.csv_helper import *
+from trongrid_extractoor.helpers.string_constants import *
+from trongrid_extractoor.helpers.time_helpers import *
+from trongrid_extractoor.progress_tracker import ProgressTracker
+from trongrid_extractoor.request_params import MAX_TRADES_PER_CALL, RequestParams
+from trongrid_extractoor.response import Response
+from trongrid_extractoor.trc20_txn import Trc20Txn
 
 RESCUE_DURATION_WALKBACK_SECONDS = [
     20,
     200,
     1000,
 ]
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/helpers/address_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 import logging
 from typing import Optional
 
 import base58
 from rich.console import Console
 from rich.text import Text
 
-from trongrid_extractor.helpers.dict_helper import get_dict_key_by_value
-from trongrid_extractor.helpers.rich_helpers import console
+from trongrid_extractoor.helpers.dict_helper import get_dict_key_by_value
+from trongrid_extractoor.helpers.rich_helpers import console
 
 TOKEN_ADDRESSES = {
     'TFczxzPhnThNSqr5by8tvxsdCFRRz6cPNq': 'APENFT',
     'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',   # BTC on Tron (?!)
     'TAFjULxiVgT4qWk6UZwjqwZXTSaGaqnVp4': 'BTT',
     'TMz2SWatiAtZVVcH2ebpsbVtYwUPT9EdjH': 'BUSD',
     'THbVQp8kMjStKNnf2iCY6NEzThKMK5aBHg': 'DOGET',  # DOGEcoin on Tron (?!)
     'TDyvndWuvX5xTBwHPYJi7J3Yq8pq8yh62h': 'HT',     # Huobi Token
     'TNSBA6KvSvMoTqQcEgpVK7VhHT3z7wifxy': 'jUSDC',
     'TCFLL5dx5ZJdKnWuesXxi1VPwjLVmWZZy9': 'JST',
     'TVh1PF9xr4zC5uAqRcCbxF1By6ucp95G4i': 'stUSDT',
     'TSSMHYeV2uE9qYH95DqyoCuNCzEL1NvU3S': 'SUN',
+    'TBqsNXUtqaLptVK8AYvdPPctpqd8oBYWUC': 'TCNH',
     'TUpMhErZL2fhh4sVNULAbNKLokS4GjC1F4': 'TUSD',
     'TEkxiTehnzSmSe2XqrBj4w32RUN966rdz8': 'USDC',
     'TPYmHEhy5n8TCEfYGqW2rPxsghSfzghPDn': 'USDD',
     'TMwFHYXLJaRUPeW6421aqXL4ZEzPRFGkGT': 'USDJ',
     'TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t': 'USDT',
     'TLa2f6VPqDgRE67v1736s7bJ8Ray5wYjU7': 'WIN',
+    'TGkxzkDKyMeq2T7edKnyjZoFypyzjkkssq': 'wstUSDT',
     'TNUC9Qb1rRpS5CbWLmNMxXBjyFoydXjWFR': 'WTRX',
 }
 
 
 def symbol_for_address(address: str) -> Optional[str]:
     return TOKEN_ADDRESSES.get(address)
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/helpers/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from argparse import ArgumentParser, Namespace
 from os import environ
 from pathlib import Path
 from sys import exit
 
 from rich.logging import RichHandler
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.address_helpers import is_contract_address, address_of_symbol, print_symbol_addresses
-from trongrid_extractor.helpers.string_constants import PACKAGE_NAME
-from trongrid_extractor.helpers.time_helpers import str_to_timestamp
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.address_helpers import is_contract_address, address_of_symbol, print_symbol_addresses
+from trongrid_extractoor.helpers.string_constants import PACKAGE_NAME
+from trongrid_extractoor.helpers.time_helpers import str_to_timestamp
 
 
 parser = ArgumentParser(
     description='Pull transactions for a given token. Either --token or --resume-csv must be provided. ',
     epilog='For a limited number of known symbols (USDT, USDD, etc.) you can use the symbol string instead ' \
            'of the on chain address.'
 )
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/helpers/csv_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import csv
+import re
 from dataclasses import dataclass, field, asdict, fields
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.address_helpers import *
-from trongrid_extractor.trc20_txn import Trc20Txn
+import pendulum
+
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.address_helpers import *
+from trongrid_extractoor.trc20_txn import Trc20Txn
+
+WRITTEN = 'written'
+WRITTEN_AT_REGEX = re.compile(WRITTEN + "_(\\d{4}-\\d{2}-\\d{2}T\\d{2}[.:]\\d{2}[.:]\\d{2})\\.csv")
 
 
 def write_rows(file_path: Union[str, Path], rows: List[Trc20Txn], _klass = Trc20Txn) -> None:
     log.info(f"Writing {len(rows)} rows...")
     _fields = [fld.name for fld in fields(_klass)]
 
     if Path(file_path).exists():
@@ -72,8 +78,19 @@
         filename += f"{symbol}_"
 
     filename += f"{address}_"
     return filename
 
 
 def csv_suffix() -> str:
-    return f"written_{datetime.now().strftime('%Y-%m-%dT%H.%M.%S')}.csv"
+    """String showing the time the file was created."""
+    return f"{WRITTEN}_{datetime.now().strftime('%Y-%m-%dT%H.%M.%S')}.csv"
+
+
+def parse_written_at_from_filename(csv_path: Union[str, Path]) -> pendulum.DateTime:
+    """Extract the written timestmap (output of csv_suffix()) to a timestamp."""
+    match = WRITTEN_AT_REGEX.search(str(csv_path))
+
+    if match is None:
+        raise ValueError(f"'{csv_path}' does not seem to have an embedded written_at timestamp!")
+
+    return pendulum.parse(match.group(1).replace('.', ':'))
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/helpers/time_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import Union
 
 import pendulum
 from pendulum import DateTime
 
-from trongrid_extractor.config import log
+from trongrid_extractoor.config import log
 
 # 2017-01-01, though Tron was really prolly launched in 2018
 TRON_LAUNCH_TIME = pendulum.datetime(2017, 1, 1, tz='UTC')
 TRON_LAUNCH_TIME_IN_EPOCH_MS = TRON_LAUNCH_TIME.timestamp() * 1000
 MAX_TIME = DateTime.now().add(years=2)
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/progress_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from sys import exit
 
 from pendulum import DateTime
 from rich.text import Text
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.rich_helpers import print_error_and_exit
-from trongrid_extractor.trc20_txn import Trc20Txn
-from trongrid_extractor.helpers.time_helpers import ms_to_datetime
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.rich_helpers import print_error_and_exit
+from trongrid_extractoor.trc20_txn import Trc20Txn
+from trongrid_extractoor.helpers.time_helpers import ms_to_datetime
 
 
 class ProgressTracker:
     def __init__(
             self,
             output_csv_path: Path,
             resume_from_csv: bool = False,
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/request_params.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/request_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 import pendulum
 from pendulum import DateTime
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.string_constants import EVENT_NAME, MIN_TIMESTAMP, MAX_TIMESTAMP, TRANSFER
-from trongrid_extractor.helpers.time_helpers import TRON_LAUNCH_TIME, datetime_to_ms, ms_to_datetime
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.string_constants import EVENT_NAME, MIN_TIMESTAMP, MAX_TIMESTAMP, TRANSFER
+from trongrid_extractoor.helpers.time_helpers import TRON_LAUNCH_TIME, datetime_to_ms, ms_to_datetime
 
 MAX_TRADES_PER_CALL = 200
 DEFAULT_MAX_TIMESTAMP = pendulum.now('UTC').add(months=2)
 
 
 @dataclass
 class RequestParams:
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/response.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Any, Dict, Union
 
 import requests
 from requests_toolbelt.utils import dump
 from rich.pretty import pprint
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
-from trongrid_extractor.config import log
-from trongrid_extractor.request_params import RequestParams
-from trongrid_extractor.helpers.csv_helper import *
-from trongrid_extractor.helpers.string_constants import *
-from trongrid_extractor.helpers.time_helpers import *
+from trongrid_extractoor.config import log
+from trongrid_extractoor.request_params import RequestParams
+from trongrid_extractoor.helpers.csv_helper import *
+from trongrid_extractoor.helpers.string_constants import *
+from trongrid_extractoor.helpers.time_helpers import *
 
 # If the distance between min and max_timestamp is less than this don't consider a 0 row
 # result a failure.
 OK_DURATION_FOR_ZERO_TXNS_MS = 10000
 JSON_HEADERS = {'Accept': 'application/json'}
 
 TRONGRID_RETRY_KWARGS = {
```

### Comparing `trongrid_extractor-1.0.0/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-1.1.0/trongrid_extractoor/trc20_txn.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 import pendulum
 
-from trongrid_extractor.config import log
-from trongrid_extractor.helpers.address_helpers import hex_to_tron
-from trongrid_extractor.helpers.rich_helpers import console
-from trongrid_extractor.helpers.string_constants import DATA, RESULT
-from trongrid_extractor.helpers.time_helpers import ms_to_datetime
+from trongrid_extractoor.config import log
+from trongrid_extractoor.helpers.address_helpers import hex_to_tron
+from trongrid_extractoor.helpers.rich_helpers import console
+from trongrid_extractoor.helpers.string_constants import DATA, RESULT
+from trongrid_extractoor.helpers.time_helpers import ms_to_datetime
 
 # Some tokens use src/dst/wad instead of from/to/value
 FROM_TO_AMOUNT = ('from', 'to', 'amount')
 FROM_TO_VALUE = ('from', 'to', 'value')
 SRC_DST_WAD = ('src', 'dst', 'wad')
```

### Comparing `trongrid_extractor-1.0.0/PKG-INFO` & `trongrid_extractor-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,44 +28,36 @@
 Set `LOG_LEVEL=DEBUG` to get debug logging.
 
 #### Compiling Multiple CSVs To One File
 There is a script that will collect all CSVs with a given symbol/address prefix and uniquify the rows into a single CSV. Run `scripts/compile_csvs.py --help` to see the usage options.
 
 ## As Package
 ```python
-from trongrid_extractor.api import Api
+from trongrid_extractoor.api import Api
 
 Api().events_for_token('Tf2939nbd23kmdo')
 ```
 
 `events_for_token()` hits the `contracts/[CONTRACT_ADDRESS]/events` endpoint and can pull all transfers for a given contract by filtering for `event_name=Transfer`. Other endpoints like `contracts/[CONTRACT_ADDRESS]/transactions` don't seem to really work.
 
+
 # Trongrid Documentation, Quirks, Etc.
+**UPDATE: cirac July 2023 Trongrid appears to have fixed this issue and the `next` URL will actually give you more than 5 pages.**
+
 When you make an API request to TronGrid they return you a page of results. If there are more than the page size (200 here) then the response includes a `next` key that has a URL you can hit to get the next page. Sounds convenient, right? Except it doesn't work. After 5 pages TronGrid will tell you your timespan is too big and please try again. This package is written to go around this "quirk" by backing up the `max_timestamp` parameter when it can't page any more.
 
 * [Trongrid API documentation](https://developers.tron.network/v4.0/reference/note)
 
-### Paging Completion
-It seems like (not 100% confident) when a given query is finished paging it returns JSON with a `page_size` value of `0` like this:
-```json
-{
-    'data': [],
-    'success': True,
-    'meta': {
-        'at': 1687935779799,
-        'page_size': 0
-    }
-}
-```
 
 # Contributing
 This project was developed with `poetry` and as such is probably easier to work with using `poetry` to manage dependencies in the dev environment. Install with:
 ```
 poetry install --with=dev
 ```
+
 ## Running Tests
 ```
 pytest
 ```
 
 ## Publishing to PyPi
 ### Configuration
@@ -99,9 +91,9 @@
    ```
     INFO       Returning 1000 transactions from _rescue_extraction(), modified params in place.                                    api.py:191
     INFO     Writing 1000 rows to 'events_USDD_written_2023-06-28T04.22.00.csv'...                                           csv_helper.py:17
     [06/28/23 10:22:34] INFO       Removed 200 duplicate transactions...                                                                   progress_tracker.py:47
     WARNING  0 txns found. We seem to be stuck at 2023-01-26T03:18:54+00:00.                                                       api.py:103
     WARNING    Last request params: {'only_confirmed': 'true', 'limit': 200, 'min_timestamp': 1483228800000.0, 'max_timestamp':    api.py:104
             1674703134000.0, 'event_name': 'Transfer'}
-   ```
+    ```
```

