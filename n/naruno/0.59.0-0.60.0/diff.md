# Comparing `tmp/naruno-0.59.0.tar.gz` & `tmp/naruno-0.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.59.0.tar", last modified: Thu Jun 29 00:20:02 2023, max compression
+gzip compressed data, was "naruno-0.60.0.tar", last modified: Fri Jul 28 22:57:29 2023, max compression
```

## Comparing `naruno-0.59.0.tar` & `naruno-0.60.0.tar`

### file list

```diff
@@ -1,302 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.394561 naruno-0.59.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-29 00:19:51.000000 naruno-0.59.0/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 00:19:51.000000 naruno-0.59.0/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 00:19:51.000000 naruno-0.59.0/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 00:19:51.000000 naruno-0.59.0/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 00:19:51.000000 naruno-0.59.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-29 00:20:02.394561 naruno-0.59.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-06-29 00:19:51.000000 naruno-0.59.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/apps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.378560 naruno-0.59.0/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.382560 naruno-0.59.0/naruno/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/gui/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.386560 naruno-0.59.0/naruno/gui/lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.386560 naruno-0.59.0/naruno/gui/lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.370559 naruno-0.59.0/naruno/gui/lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.386560 naruno-0.59.0/naruno/gui/lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.386560 naruno-0.59.0/naruno/gui/lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/lib/libs/kv/welcome_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    29480 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.390560 naruno-0.59.0/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.394561 naruno-0.59.0/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.394561 naruno-0.59.0/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.394561 naruno-0.59.0/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.394561 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 00:19:51.000000 naruno-0.59.0/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:20:02.374559 naruno-0.59.0/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-29 00:20:02.000000 naruno-0.59.0/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-29 00:20:02.000000 naruno-0.59.0/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:20:02.000000 naruno-0.59.0/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 00:20:02.000000 naruno-0.59.0/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 00:20:02.000000 naruno-0.59.0/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 00:20:02.394561 naruno-0.59.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-29 00:19:51.000000 naruno-0.59.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.859548 naruno-0.60.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-28 22:57:19.000000 naruno-0.60.0/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 22:57:19.000000 naruno-0.60.0/LICENCE-naruno-lib-kot__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 22:57:19.000000 naruno-0.60.0/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 22:57:19.000000 naruno-0.60.0/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-28 22:57:19.000000 naruno-0.60.0/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 22:57:19.000000 naruno-0.60.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-28 22:57:29.859548 naruno-0.60.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-28 22:57:19.000000 naruno-0.60.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.835547 naruno-0.60.0/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.835547 naruno-0.60.0/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25532 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/apps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.831547 naruno-0.60.0/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.831547 naruno-0.60.0/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.831547 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.839547 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.831547 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.843547 naruno-0.60.0/naruno/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.835547 naruno-0.60.0/naruno/gui/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.851547 naruno-0.60.0/naruno/gui/lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.851547 naruno-0.60.0/naruno/gui/lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.835547 naruno-0.60.0/naruno/gui/lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.851547 naruno-0.60.0/naruno/gui/lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.851547 naruno-0.60.0/naruno/gui/lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/lib/libs/kv/welcome_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/kot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.855548 naruno-0.60.0/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.859548 naruno-0.60.0/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.859548 naruno-0.60.0/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.859548 naruno-0.60.0/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.859548 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-28 22:57:19.000000 naruno-0.60.0/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:57:29.835547 naruno-0.60.0/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-28 22:57:29.000000 naruno-0.60.0/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-07-28 22:57:29.000000 naruno-0.60.0/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:57:29.000000 naruno-0.60.0/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-28 22:57:29.000000 naruno-0.60.0/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 22:57:29.000000 naruno-0.60.0/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:57:29.859548 naruno-0.60.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-28 22:57:19.000000 naruno-0.60.0/setup.py
```

### Comparing `naruno-0.59.0/LICENCE-naruno-gui_lib__.md` & `naruno-0.60.0/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/LICENCE-naruno-lib-mix__.md` & `naruno-0.60.0/LICENCE-naruno-lib-kot__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.60.0/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/LICENSE-others__.md` & `naruno-0.60.0/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/PKG-INFO` & `naruno-0.60.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.59.0
+Version: 0.60.0
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.59.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.0 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.59.0/README.md` & `naruno-0.60.0/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/accounts/account.py` & `naruno-0.60.0/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/accounts/commanders/delete_commander.py` & `naruno-0.60.0/naruno/accounts/commanders/save_commander.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import os
 
 from naruno.config import COMMANDERS_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 
+commanders_db = KOT("commanders", folder=get_config()["main_folder"] + "/db")
 
-def DeleteCommander(tx):
-    os.chdir(get_config()["main_folder"])
-    for entry in os.scandir(COMMANDERS_PATH):
-        if tx in entry.name:
-            os.remove(entry.path)
+
+def SaveCommander(commander):
+    commanders_db.set(commander, True)
```

### Comparing `naruno-0.59.0/naruno/accounts/commanders/save_commander.py` & `naruno-0.60.0/naruno/accounts/commanders/delete_commander.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import os
 
 from naruno.config import COMMANDERS_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 
+commanders_db = KOT("commanders", folder=get_config()["main_folder"] + "/db")
 
-def SaveCommander(commander):
-    the_path = COMMANDERS_PATH + commander
-    os.chdir(get_config()["main_folder"])
-    with open(the_path, "w") as my_transaction_file:
-        my_transaction_file.write("1")
+
+def DeleteCommander(tx):
+    if commanders_db.get(tx) == True:
+        commanders_db.delete(tx)
```

### Comparing `naruno-0.59.0/naruno/accounts/get_accounts.py` & `naruno-0.60.0/naruno/accounts/get_accounts.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import os
 import sqlite3
 
+import naruno
+from naruno.accounts.save_accounts import get_ram_accounts
 from naruno.config import TEMP_ACCOUNTS_PATH
 from naruno.lib.config_system import get_config
 
 
-def GetAccounts(custom_TEMP_ACCOUNTS_PATH=None):
+def GetAccounts(custom_TEMP_ACCOUNTS_PATH=None, reset: bool = False):
     """
     Returns the accounts from TEMP_ACCOUNTS_PATH.
     """
+    os.chdir(get_config()["main_folder"])
 
     the_TEMP_ACCOUNTS_PATH = (TEMP_ACCOUNTS_PATH if custom_TEMP_ACCOUNTS_PATH
                               is None else custom_TEMP_ACCOUNTS_PATH)
-
-    os.chdir(get_config()["main_folder"])
-    conn = sqlite3.connect(the_TEMP_ACCOUNTS_PATH, check_same_thread=False)
-    c = conn.cursor()
-    c.execute(
-        """CREATE TABLE IF NOT EXISTS account_list (address text, sequence_number integer, balance integer)"""
-    )
-
-    return c
+    the_TEMP_ACCOUNTS_PATH = os.path.join(get_config()["main_folder"],
+                                          the_TEMP_ACCOUNTS_PATH)
+    return naruno.accounts.save_accounts.accounts_ram_db[get_ram_accounts(
+        the_TEMP_ACCOUNTS_PATH, reset=reset)]
```

### Comparing `naruno-0.59.0/naruno/accounts/get_balance.py` & `naruno-0.60.0/naruno/accounts/get_balance.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from naruno.wallet.wallet_import import Address
 
 
 def GetBalance(user,
                account_list=None,
                dont_convert=False,
                block=None,
-               custom_TEMP_BLOCK_PATH=None):
+               custom_TEMP_BLOCK_PATH=None,
+               tx_signature=None,
+               custom_pending=None):
     """
     Returns the users balance.
     """
     address = Address(user) if not dont_convert else user
 
     balance = GetMinimumTransferAmount(
         block=block, custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
@@ -33,26 +35,28 @@
             urlopen(
                 f"http://test_net.1.naruno.org:8000/balance/get/?address={address}"
             ).read().decode("utf-8").replace("\n", ""))
     else:
         if block is None:
             try:
                 block = GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-            except FileNotFoundError:
+            except TypeError:
                 return None
 
         balance = -block.minumum_transfer_amount
 
         the_account_list = GetAccounts(
         ) if account_list is None else account_list
-        the_account_list.execute(
-            f"SELECT * FROM account_list WHERE address = ?", (address,))
-        for row in the_account_list.fetchall():
-            balance += row[2]
-            break
+        balance += the_account_list[address][
+            1] if address in the_account_list else 0
+
         if not block.just_one_tx:
-            for tx in block.validating_list + GetPending():
-                if Address(tx.fromUser) == user:
+            the_pending = custom_pending if custom_pending is not None else GetPending()
+            for tx in block.validating_list + the_pending:
+                sub_control = True
+                if tx_signature is not None:
+                    if tx.signature == tx_signature:
+                        sub_control = False
+                if Address(tx.fromUser) == user and sub_control:
                     balance -= float(tx.amount) + float(tx.transaction_fee)
-                elif tx.toUser == user:
-                    balance += float(tx.amount)
+
     return balance
```

### Comparing `naruno-0.59.0/naruno/accounts/get_sequence_number.py` & `naruno-0.60.0/naruno/accounts/get_sequence_number.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from naruno.accounts.get_accounts import GetAccounts
 from naruno.transactions.pending.get_pending import GetPending
 from naruno.wallet.wallet_import import Address
 
 
-def GetSequanceNumber(user, account_list=None, dont_convert=False, block=None):
+def GetSequanceNumber(user, account_list=None, dont_convert=False, block=None,custom_pending=None):
     user = Address(user) if not dont_convert else user
     sequence_number = 0
+
     the_account_list = GetAccounts() if account_list is None else account_list
-    the_account_list.execute(
-        f"SELECT * FROM account_list WHERE address = ?", (user,))
-    for Accounts in the_account_list.fetchall():
-        sequence_number = Accounts[1]
-        break
+
+    sequence_number = the_account_list[user][
+        0] if user in the_account_list else 0
+
     if block is not None:
+        the_pending = custom_pending if custom_pending is not None else GetPending()
         if not block.just_one_tx:
-            for tx in block.validating_list + GetPending():
+            for tx in block.validating_list + the_pending:
                 if Address(tx.fromUser) == user:
                     sequence_number += 1
     return sequence_number
```

### Comparing `naruno-0.59.0/naruno/api/buildozer/main.py` & `naruno-0.60.0/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/api/main.py` & `naruno-0.60.0/naruno/api/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import argparse
 import contextlib
 import os
 import sys
+import threading
+import traceback
 
 from flask import Flask
 from flask import jsonify
 from flask import request
 from waitress import serve
 from waitress.server import create_server
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 
 from flask_cors import CORS
-
+from naruno.blockchain.block.block_main import Block
 from naruno.accounts.get_balance import GetBalance
 from naruno.accounts.get_sequence_number import GetSequanceNumber
 from naruno.blockchain.block.create_block import CreateBlock
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.just_one_tx import GetJustOneTX
 from naruno.blockchain.block.max_data_size import GetMaxDataSize
 from naruno.blockchain.block.max_tx_number import GetMaxTXNumber
@@ -141,14 +143,15 @@
     return jsonify(print_wallets())
 
 
 @app.route("/send/", methods=["POST"])
 def send_coin_data_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
+    result = "false"
     try:
         if the_settings()["publisher_mode"]:
             return jsonify(
                 {"error": "You can't send a transaction in publisher mode."})
         address = str(
             request.form["to_user"]) if "to_user" in request.form else None
         amount = float(
@@ -170,50 +173,51 @@
             block=block,
             custom_current_time=custom_current_time,
             custom_sequence_number=custom_sequence_number,
             custom_balance=custom_balance,
             custom_account_list=custom_account_list,
             custom_set_sequence_number=sequence_number,
         )
+        if send_tx != False:
+            SavetoMyTransaction(send_tx, sended=True)
+            if not the_settings()["baklava"]:
+                server.send_transaction(
+                    send_tx,
+                    custom_current_time=custom_current_time,
+                    custom_sequence_number=custom_sequence_number,
+                    custom_balance=custom_balance,
+                    custom_server=custom_server,
+                )
+                SaveBlock(
+                    block,
+                    custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
+                    custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
+                    custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
+                    custom_TEMP_BLOCKSHASH_PART_PATH=
+                    custom_TEMP_BLOCKSHASH_PART_PATH,
+                )
+            result = send_tx.dump_json()
+  
     except:
-        result = "false"
-    if send_tx != False:
-        SavetoMyTransaction(send_tx, sended=True)
-        if not the_settings()["baklava"]:
-            server.send_transaction(
-                send_tx,
-                custom_current_time=custom_current_time,
-                custom_sequence_number=custom_sequence_number,
-                custom_balance=custom_balance,
-                custom_server=custom_server,
-            )
-            SaveBlock(
-                block,
-                custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
-                custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
-                custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
-                custom_TEMP_BLOCKSHASH_PART_PATH=
-                custom_TEMP_BLOCKSHASH_PART_PATH,
-            )
-    result = send_tx.dump_json() if send_tx != False else False
+        traceback.print_exc()
+
 
     return jsonify(result)
 
 
 @app.route("/wallet/balance", methods=["GET"])
 def balance_wallets_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     if the_settings()["publisher_mode"]:
         return jsonify(
             {"error": "You can't get the balance in publisher mode."})
     the_wallet = wallet_import(-1,
                                0) if custom_wallet is None else custom_wallet
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
     return jsonify(
         GetBalance(the_wallet, account_list=account_list, block=the_block))
 
 
 @app.route("/node/start/<ip>/<port>", methods=["GET"])
 def node_start_page(ip, port):
     logger.debug(
@@ -348,37 +352,41 @@
         return jsonify(
             {"error": "You can't turn off the debug mode in publisher mode."})
     app.config["DEBUG"] = False
     ft_mode_settings(False)
     return jsonify("OK")
 
 
-@app.route("/block/get", methods=["GET"])
-def block_get_page():
-    logger.debug(
-        f"{request.remote_addr} {request.method} {request.url} {request.data}")
-    if the_settings()["publisher_mode"]:
-        return jsonify({"error": "You can't get the block in publisher mode."})
-    the_server = server.Server if custom_server is None else custom_server
-    if the_settings()["test_mode"]:
+def block_get_page_proccess(the_server):
         the_block = CreateBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
         SaveBlock(
             the_block,
             custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
             custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
             custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
             custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
         )
         the_server.send_block_to_other_nodes()
         the_consensus_trigger = (consensus_trigger if custom_consensus_trigger
                                  is None else custom_consensus_trigger)
         trigger = perpetualTimer(the_block.consensus_timer,
-                                 the_consensus_trigger)
+                                 the_consensus_trigger, the_consensus=True)
         global custom_consensus_trigger_result
         custom_consensus_trigger_result = trigger
+
+
+@app.route("/block/get", methods=["GET"])
+def block_get_page():
+    logger.debug(
+        f"{request.remote_addr} {request.method} {request.url} {request.data}")
+    if the_settings()["publisher_mode"]:
+        return jsonify({"error": "You can't get the block in publisher mode."})
+    the_server = server.Server if custom_server is None else custom_server
+    if the_settings()["test_mode"]:
+        block_get_page_proccess(the_server,)
     else:
         the_server.send_me_full_block()
     return jsonify("OK")
 
 
 @app.route("/export/transactions/csv", methods=["GET"])
 def export_transaction_csv_page():
@@ -529,16 +537,15 @@
 def balance_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
     address = str(request.args.get("address"))
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(
         GetBalance(
             address,
             block=the_block,
             account_list=custom_account_list,
             dont_convert=True,
@@ -550,16 +557,15 @@
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
     address = str(request.args.get("address"))
 
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(
         GetSequanceNumber(
             address,
             account_list=custom_account_list,
             dont_convert=True,
             block=the_block,
@@ -616,63 +622,58 @@
 @app.route("/blocktransactionfee/get/", methods=["GET"])
 def blocktransactionfee_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(the_block.transaction_fee)
 
 
 @app.route("/blockmaxtxnumber/get/", methods=["GET"])
 def blockmaxtxnumber_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(GetMaxTXNumber(block=the_block))
 
 
 @app.route("/blockjustonetx/get/", methods=["GET"])
 def blockjustonetx_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(GetJustOneTX(block=the_block))
 
 
 @app.route("/blockmaxdatasize/get/", methods=["GET"])
 def blockmaxdatasize_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
 
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(GetMaxDataSize(block=the_block))
 
 
 @app.route("/blockminumumtransferamount/get/", methods=["GET"])
 def blockminumumtransferamount_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
-    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                 if custom_block is None else custom_block)
+    the_block = Block("API")
 
     return jsonify(the_block.minumum_transfer_amount)
 
 
 @app.errorhandler(500)
 def handle_exception(e):
     logger.exception(f"500: {e}")
```

### Comparing `naruno-0.59.0/naruno/apps/checker.py` & `naruno-0.60.0/naruno/apps/checker.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/apps/remote_app.py` & `naruno-0.60.0/naruno/apps/remote_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 import os
 import random
 import string
 import sys
 import threading
 import time
 from hashlib import sha256
+import traceback
 
 import requests
 
 from naruno.accounts.commanders.delete_commander import DeleteCommander
 from naruno.accounts.commanders.get_comnder import GetCommander
 from naruno.accounts.commanders.save_commander import SaveCommander
 from naruno.api.main import start
 from naruno.apps.checker import checker
 from naruno.blockchain.block.block_main import Block
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 from naruno.lib.log import get_logger
 from naruno.lib.perpetualtimer import perpetualTimer
 from naruno.lib.settings_system import the_settings
 from naruno.transactions.my_transactions.save_to_my_transaction import \
     SavetoMyTransaction
 from naruno.transactions.my_transactions.sended_transaction import \
     SendedTransaction
@@ -72,14 +74,19 @@
         :param host: The host of the node
         :param port: The port of the node
         :param password: The password of the wallet
         """
         self.app_name = app_name
         self.cache_name = sha256(
             self.app_name.encode()).hexdigest() + wallet_import(-1, 3)
+
+        self.integrationcache_db = KOT(
+            "integrationcache" + self.cache_name,
+            folder=get_config()["main_folder"] + "/db",
+        )
         self.host = host
         self.port = port
 
         self.first_host = copy.copy(host)
         self.first_port = copy.copy(port)
 
         self.api = None
@@ -116,15 +123,15 @@
 
         self.check_thread = None
 
         backup_host = copy.copy(self.host)
         backup_port = copy.copy(self.port)
         self.change_by_network()
         success = False
-        with contextlib.suppress(Exception):
+        try:
             self.max_tx_number = int(
                 self.prepare_request(
                     "/blockmaxtxnumber/get/",
                     type="get",
                 ).text)
             self.max_data_size = int(
                 self.prepare_request(
@@ -136,39 +143,40 @@
 
             if total_check is None:
                 self.total_check = self.prepare_request(
                     "/blockjustonetx/get/",
                     type="get",
                 ).text
 
-
                 self.total_check = False if "true" in self.total_check else True
 
-
             self.original_wait_amoount = copy.copy(self.wait_amount)
 
-            
-            self.check_thread = perpetualTimer(self.original_wait_amoount, checker, (self, )) if self.total_check else self.check_thread
+            self.check_thread = (perpetualTimer(
+                self.original_wait_amoount, checker,
+                (self, )) if self.total_check else self.check_thread)
             self.wait_amount = 0 if self.total_check else self.wait_amount
             success = True
-       
+        except:
+            traceback.print_exc()
+
         logger.error("Network is not active") if not success else None
         self.close() if not success else None
         sys.exit() if not success else None
 
         self.host = backup_host
         self.port = backup_port
 
         logger.info(f"Integration of {self.app_name} is started")
 
     def change_by_network(self):
-        self.host = "test_net.1.naruno.org" if the_settings()["baklava"] else self.host
+        self.host = "test_net.1.naruno.org" if the_settings(
+        )["baklava"] else self.host
         self.port = 8000 if the_settings()["baklava"] else self.port
 
-
     def init_api(self):
         try:
             self.prepare_request("/", "get")
         except Exception as e:
             self.start_api()
 
     def start_api(self):
@@ -182,15 +190,14 @@
         sys.argv = backup
 
     def wait_until_complated(self, custom_list=None):
         while len(self.sended_txs) > 0:
             time.sleep(self.sending_wait_time)
             self.sended_txs = (custom_list
                                if custom_list is not None else self.sended_txs)
-        
 
     def close(self):
         DeleteCommander(self.commander) if not self.commander is None else None
         self.wait_until_complated() if self.check_thread is not None else None
         self.check_thread.cancel() if self.check_thread is not None else None
         if self.api is not None:
             self.api.close()
@@ -200,54 +207,53 @@
         self.cache = []
 
     def get_cache(self):
         if self.cache_true == False:
             self.cache = []
             return
 
-        os.chdir(get_config()["main_folder"])
+        record = self.integrationcache_db.get("cache")
 
-        if not os.path.exists(f"db/remote_app_cache/{self.cache_name}.cache"):
+        if record is None:
             self.cache = []
             self.save_cache()
-        with open(f"db/remote_app_cache/{self.cache_name}.cache",
-                  "r") as cache:
-            self.cache = json.load(cache)
-
-        self.backward_support_cache()
-        self.save_cache()
+        else:
+            self.cache = record
+            self.backward_support_cache()
+            self.save_cache()
 
     def backward_support_cache(self):
         for each_cache in self.cache:
             if len(self.cache[self.cache.index(each_cache)]) != 96:
                 # remoe the cache
                 self.cache.remove(each_cache)
 
     def save_cache(self):
         if self.cache_true == False:
             self.get_cache()
             return
+
+
         self.backward_support_cache()
-        os.chdir(get_config()["main_folder"])
-        with open(f"db/remote_app_cache/{self.cache_name}.cache",
-                  "w") as cache:
-            json.dump(self.cache, cache)
+
+        self.integrationcache_db.set("cache", self.cache)
+
 
     def delete_cache(self):
-        os.chdir(get_config()["main_folder"])
-        os.remove(f"db/remote_app_cache/{self.cache_name}.cache")
+        self.integrationcache_db.delete("cache")
 
     def prepare_request(self, end_point, type, data=None) -> requests.Response:
         """
         :param end_point: The end point of the request
         :param type: The type of the request (get, post)
         :param data: The data of the request
         :return: The response of the request
         """
         api = f"http://{self.host}:{self.port}"
+
         response = None
         if type == "post":
             response = requests.post(api + end_point, data=data)
         elif type == "get":
             response = requests.get(api + end_point)
 
         return response
@@ -736,15 +742,17 @@
     ):
         self.host = copy.copy(self.first_host)
         self.port = copy.copy(self.first_port)
 
         backup_host = copy.copy(self.host)
         backup_port = copy.copy(self.port)
 
-        self.wait_until_complated() if ((self.sended or force_sended) and self.check_thread is not None and not from_thread) else None
+        self.wait_until_complated() if ((self.sended or force_sended)
+                                        and self.check_thread is not None
+                                        and not from_thread) else None
 
         self.change_by_network()
 
         baklava_datas = None
 
         with contextlib.suppress(Exception):
             baklava_datas = self.get_(
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/blocks_hash.py` & `naruno-0.60.0/naruno/blockchain/block/blocks_hash.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,106 +7,103 @@
 import json
 import os
 import sqlite3
 
 from naruno.config import TEMP_BLOCKSHASH_PART_PATH
 from naruno.config import TEMP_BLOCKSHASH_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 from naruno.lib.log import get_logger
 
+blockshash_db = KOT("blockshash", folder=get_config()["main_folder"] + "/db")
+
 logger = get_logger("BLOCKCHAIN")
 
 
 def SaveBlockshash(the_blockshash, custom_TEMP_BLOCKSHASH_PATH=None):
     """
     Saves the blockshash to the TEMP_BLOCKSHASH_PATH.
     """
-
     os.chdir(get_config()["main_folder"])
+
     the_TEMP_BLOCKSHASH_PATH = (TEMP_BLOCKSHASH_PATH
                                 if custom_TEMP_BLOCKSHASH_PATH is None else
                                 custom_TEMP_BLOCKSHASH_PATH)
 
-    conn = sqlite3.connect(the_TEMP_BLOCKSHASH_PATH)
-    c = conn.cursor()
-    c.execute("""CREATE TABLE IF NOT EXISTS blockshash_list (hash text)""")
-    if type(the_blockshash) == list:
-        for i in the_blockshash:
-            c.execute("""INSERT INTO blockshash_list VALUES (?)""", (i, ))
-    else:
-        c.execute(
-            """INSERT INTO blockshash_list VALUES (?)""",
-            (the_blockshash, ),
-        )
-    conn.commit()
-    conn.close()
+    the_TEMP_BLOCKSHASH_PATH = os.path.join(get_config()["main_folder"],
+                                            the_TEMP_BLOCKSHASH_PATH)
+
+    if type(the_blockshash) != list:
+        the_blockshash = [the_blockshash]
+
+    the_blockshash = (GetBlockshash(
+        custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH) +
+                      the_blockshash)
+
+    blockshash_db.set("blockshash",
+                      the_blockshash,
+                      custom_key_location=the_TEMP_BLOCKSHASH_PATH)
 
 
 def SaveBlockshash_part(the_blockshash, custom_TEMP_BLOCKSHASH_PART_PATH=None):
     """
     Saves the blockshash part to the TEMP_BLOCKSHASH_PART_PATH.
     """
-
     os.chdir(get_config()["main_folder"])
+
     the_TEMP_BLOCKSHASH_PART_PATH = (TEMP_BLOCKSHASH_PART_PATH if
                                      custom_TEMP_BLOCKSHASH_PART_PATH is None
                                      else custom_TEMP_BLOCKSHASH_PART_PATH)
-    conn = sqlite3.connect(the_TEMP_BLOCKSHASH_PART_PATH)
-    c = conn.cursor()
-    c.execute(
-        """CREATE TABLE IF NOT EXISTS blockshash_part_list (hash text)""")
-    if type(the_blockshash) == list:
-        for i in the_blockshash:
-            c.execute("""INSERT INTO blockshash_part_list VALUES (?)""", (i, ))
-    else:
-        c.execute(
-            """INSERT INTO blockshash_part_list VALUES (?)""",
-            (the_blockshash, ),
-        )
-    conn.commit()
-    conn.close()
+
+    the_TEMP_BLOCKSHASH_PART_PATH = os.path.join(
+        get_config()["main_folder"], the_TEMP_BLOCKSHASH_PART_PATH)
+
+    if type(the_blockshash) != list:
+        the_blockshash = [the_blockshash]
+
+    the_blockshash = (GetBlockshash_part(
+        custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH) +
+                      the_blockshash)
+
+    blockshash_db.set(
+        "blockshash_part",
+        the_blockshash,
+        custom_key_location=the_TEMP_BLOCKSHASH_PART_PATH,
+    )
 
 
 def GetBlockshash(custom_TEMP_BLOCKSHASH_PATH=None):
     """
     Returns the blockshash.
     """
+    os.chdir(get_config()["main_folder"])
+
     the_TEMP_BLOCKSHASH_PATH = (TEMP_BLOCKSHASH_PATH
                                 if custom_TEMP_BLOCKSHASH_PATH is None else
                                 custom_TEMP_BLOCKSHASH_PATH)
 
-    os.chdir(get_config()["main_folder"])
-
-    conn = sqlite3.connect(the_TEMP_BLOCKSHASH_PATH, check_same_thread=False)
-    c = conn.cursor()
-    c.execute("""CREATE TABLE IF NOT EXISTS blockshash_list (hash text)""")
-    c.execute("""SELECT * FROM blockshash_list""")
-    result = c.fetchall()
+    the_TEMP_BLOCKSHASH_PATH = os.path.join(get_config()["main_folder"],
+                                            the_TEMP_BLOCKSHASH_PATH)
 
-    result = [i[0] for i in result]
-    conn.close()
+    record = blockshash_db.get("blockshash",
+                               custom_key_location=the_TEMP_BLOCKSHASH_PATH)
 
-    return result
+    return record if record is not None else []
 
 
 def GetBlockshash_part(custom_TEMP_BLOCKSHASH_PART_PATH=None):
     """
     Returns the blockshash part.
     """
+    os.chdir(get_config()["main_folder"])
+
     the_TEMP_BLOCKSHASH_PART_PATH = (TEMP_BLOCKSHASH_PART_PATH if
                                      custom_TEMP_BLOCKSHASH_PART_PATH is None
                                      else custom_TEMP_BLOCKSHASH_PART_PATH)
 
-    os.chdir(get_config()["main_folder"])
-
-    conn = sqlite3.connect(the_TEMP_BLOCKSHASH_PART_PATH,
-                           check_same_thread=False)
-    c = conn.cursor()
-    c.execute(
-        """CREATE TABLE IF NOT EXISTS blockshash_part_list (hash text)""")
-    c.execute("""SELECT * FROM blockshash_part_list""")
-    result = c.fetchall()
+    the_TEMP_BLOCKSHASH_PART_PATH = os.path.join(
+        get_config()["main_folder"], the_TEMP_BLOCKSHASH_PART_PATH)
 
-    result = [i[0] for i in result]
-    conn.close()
+    record = blockshash_db.get(
+        "blockshash_part", custom_key_location=the_TEMP_BLOCKSHASH_PART_PATH)
 
-    return result
+    return record if record is not None else []
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.60.0/naruno/blockchain/block/change_transaction_fee.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from naruno.lib.log import get_logger
 from naruno.transactions.pending.get_pending import GetPendingLen
+from decimal import Decimal
+
 
 logger = get_logger("BLOCKCHAIN")
 
 
 def ChangeTransactionFee(
     block,
     custom_pending_transaction_len=None,
@@ -34,14 +36,15 @@
         f"block.default_optimum_transaction_number {block.default_optimum_transaction_number}"
     )
     logger.debug(
         f"block.default_increase_of_fee {block.default_increase_of_fee}")
     if (total_len // block.default_optimum_transaction_number) != 0:
         increase = (total_len // block.default_optimum_transaction_number
                     ) * block.default_increase_of_fee
-        block.transaction_fee += increase
+        decimal_amount = Decimal(str(block.transaction_fee)) + Decimal(str(increase))
+        block.transaction_fee = float(decimal_amount)
         logger.info("Transaction fee will be increased")
 
     else:
         logger.info("Transaction fee is not changed")
         block.transaction_fee = block.default_transaction_fee
     logger.info(f"New transaction fee is : {block.transaction_fee} ")
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/create_block.py` & `naruno-0.60.0/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/get_block.py` & `naruno-0.60.0/naruno/blockchain/block/get_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,79 +10,93 @@
 
 from naruno.blockchain.block.block_main import Block
 from naruno.config import TEMP_BLOCK_PATH
 from naruno.consensus.rounds.round_1.process.transactions.checks.duplicated import \
     Remove_Duplicates
 from naruno.lib.config_system import get_config
 from naruno.lib.log import get_logger
-
+import naruno
 logger = get_logger("BLOCKCHAIN")
 
+the_ram_block = {}
 
 def GetBlock(custom_TEMP_BLOCK_PATH=None,
              get_normal_block=False,
-             dont_clean=False):
+             dont_clean=False, reset=False):
     """
     Returns the block.
     """
-    logger.debug("Getting block from disk")
-
     the_TEMP_BLOCK_PATH = (TEMP_BLOCK_PATH if custom_TEMP_BLOCK_PATH is None
                            else custom_TEMP_BLOCK_PATH)
 
+    if naruno.blockchain.block.get_block.the_ram_block is not None and not reset:
+        if the_TEMP_BLOCK_PATH in naruno.blockchain.block.get_block.the_ram_block:
+            return naruno.blockchain.block.get_block.the_ram_block[the_TEMP_BLOCK_PATH]
+
+    from naruno.blockchain.block.save_block import block_db
+
+    logger.debug("Getting block from disk")
+
+
+
     os.chdir(get_config()["main_folder"])
 
     highest_the_TEMP_BLOCK_PATH = the_TEMP_BLOCK_PATH
     highest_number = 0
 
     highest_second_number = 0
     highest_other_high_number = 0
     for file in os.listdir("db/"):
         if ("db/" + file).startswith(the_TEMP_BLOCK_PATH) and not (
                 "db/" + file) == the_TEMP_BLOCK_PATH:
-            number = int((("db/" + file).replace(the_TEMP_BLOCK_PATH,
-                                                 "")).split("-")[1])  # seq
-            high_number = int(
-                (("db/" + file).replace(the_TEMP_BLOCK_PATH,
-                                        "")).split("-")[3])  # val
-            other_high_number = int(
-                (("db/" + file).replace(the_TEMP_BLOCK_PATH,
-                                        "")).split("-")[2])  # val
-
-            # Write a code for getting the blocks with high number
-            if number > highest_number:
-                highest_number = number
-                highest_the_TEMP_BLOCK_PATH = "db/" + file
-                highest_second_number = high_number
-                highest_other_high_number = other_high_number
-            elif number == highest_number:
-                if high_number > highest_second_number:
+            with contextlib.suppress(IndexError):
+                number = int((("db/" + file).replace(the_TEMP_BLOCK_PATH,
+                                                    "")).split("-")[1])  # seq
+                high_number = int(
+                    (("db/" + file).replace(the_TEMP_BLOCK_PATH,
+                                            "")).split("-")[3])  # val
+                other_high_number = int(
+                    (("db/" + file).replace(the_TEMP_BLOCK_PATH,
+                                            "")).split("-")[2])  # val
+
+                # Write a code for getting the blocks with high number
+                if number > highest_number:
                     highest_number = number
                     highest_the_TEMP_BLOCK_PATH = "db/" + file
                     highest_second_number = high_number
                     highest_other_high_number = other_high_number
-                elif high_number == highest_second_number:
-                    if other_high_number > highest_other_high_number:
+                elif number == highest_number:
+                    if high_number > highest_second_number:
                         highest_number = number
                         highest_the_TEMP_BLOCK_PATH = "db/" + file
                         highest_second_number = high_number
                         highest_other_high_number = other_high_number
+                    elif high_number == highest_second_number:
+                        if other_high_number > highest_other_high_number:
+                            highest_number = number
+                            highest_the_TEMP_BLOCK_PATH = "db/" + file
+                            highest_second_number = high_number
+                            highest_other_high_number = other_high_number
 
     logger.debug("Highest block: " + highest_the_TEMP_BLOCK_PATH)
 
     result_normal = Block("non")
+    block_db_path_first = os.path.join(get_config()["main_folder"],
+                                       the_TEMP_BLOCK_PATH)
+    record_of_normal = Block.load_json(block_db.get(the_TEMP_BLOCK_PATH,
+                                    custom_key_location=block_db_path_first))
+    if record_of_normal is not None:
+        result_normal = record_of_normal
+
+    block_db_path_second = os.path.join(get_config()["main_folder"],
+                                        highest_the_TEMP_BLOCK_PATH)
+    logger.debug("Highest block path: " + block_db_path_second)
+    result_highest = Block.load_json(block_db.get(highest_the_TEMP_BLOCK_PATH,
+                                  custom_key_location=block_db_path_second))
 
-    with contextlib.suppress(json.decoder.JSONDecodeError):
-        with open(the_TEMP_BLOCK_PATH, "r") as block_file:
-            the_block_json = json.load(block_file)
-            result_normal = Block.load_json(the_block_json)
-
-    with open(highest_the_TEMP_BLOCK_PATH, "r") as block_file:
-        the_block_json = json.load(block_file)
-        result_highest = Block.load_json(the_block_json)
 
     result_normal = Remove_Duplicates(result_normal)
     result_highest = Remove_Duplicates(result_highest)
 
     result_normal.validating_list = sorted(result_normal.validating_list,
                                            key=lambda x: x.fromUser)
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.60.0/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,27 @@
     custom_TEMP_BLOCKSHASH_PART_PATH=None,
     dont_clean=False,
 ):
     """
     Gets the block from the blockchain database
     """
     try:
-
         the_BLOCKS_PATH = (BLOCKS_PATH if custom_BLOCKS_PATH is None else
                            custom_BLOCKS_PATH)
 
         the_block = GetBlock(
-            (the_BLOCKS_PATH + str(sequence_number) + ".block.json"), dont_clean=dont_clean)
+            (the_BLOCKS_PATH + str(sequence_number) + ".block.json"),
+            dont_clean=dont_clean, reset=True,
+        )
         the_accounts = GetAccounts(
             (the_BLOCKS_PATH + str(sequence_number) + ".accounts.db"))
         the_blockshash = GetBlockshash(the_BLOCKS_PATH + str(sequence_number) +
                                        ".blockshash.json")
         the_blockshashpart = GetBlockshash_part(the_BLOCKS_PATH +
                                                 str(sequence_number) +
                                                 ".blockshashpart.json")
         result = [the_block, the_accounts, the_blockshash, the_blockshashpart]
 
         return result
 
-    except FileNotFoundError:
+    except TypeError:
         return False
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.60.0/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,12 @@
             urlopen(
                 "http://test_net.1.naruno.org:8000/blockminumumtransferamount/get/"
             ).read().decode("utf-8"))
     else:
         if block is None:
             try:
                 block = GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-            except FileNotFoundError:
+            except TypeError:
                 return None
         minimum_transfer_amount = block.minumum_transfer_amount
 
     return minimum_transfer_amount
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.60.0/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.60.0/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.60.0/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/just_one_tx.py` & `naruno-0.60.0/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/max_data_size.py` & `naruno-0.60.0/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/max_tx_number.py` & `naruno-0.60.0/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.60.0/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         if l and not l.startswith("-----")
     ])
     my_address = wallet_import(-1, 3)
     our_tx = any((validated_transaction.fromUser == my_public_key) or (
         validated_transaction.toUser == my_address)
                  for validated_transaction in block.validating_list)
     if our_tx or force:
+        logger.debug("Saving block to blockchain database...")
         the_BLOCKS_PATH = (BLOCKS_PATH if custom_BLOCKS_PATH is None else
                            custom_BLOCKS_PATH)
         SaveBlock(
             block,
             (the_BLOCKS_PATH + str(block.sequence_number) + ".block.json"),
             dont_clean=dont_clean,
         )
@@ -73,8 +74,9 @@
             custom_TEMP_BLOCKSHASH_PART_PATH,
             (the_BLOCKS_PATH + str(block.sequence_number) +
              ".blockshashpart.json"),
         )
 
         return True
     else:
+        logger.debug("Not saving block to blockchain database...")
         return False
```

### Comparing `naruno-0.59.0/naruno/blockchain/block/shares.py` & `naruno-0.60.0/naruno/blockchain/block/shares.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 
 from naruno.blockchain.block.block_main import Block
 from naruno.consensus.rounds.round_1.process.transactions.checks.duplicated import \
     Remove_Duplicates
 from naruno.lib.log import get_logger
 from naruno.transactions.transaction import Transaction
+from decimal import Decimal
 
 logger = get_logger("BLOCKCHAIN")
 
 
 def shares(block: Block,
            custom_shares=None,
            custom_fee_address=None,
@@ -55,22 +56,23 @@
                             share[0],
                             "NP",
                             share[1],
                             0,
                             the_time,
                         ))
 
-    fee = 0
+    fee = Decimal("0")
     if not dont_clean:
         block = Remove_Duplicates(block)
     block.validating_list = sorted(block.validating_list,
                                    key=lambda x: x.fromUser)
     for tx in block.validating_list:
         if not "NARUNO" in tx.signature:
-            fee += tx.transaction_fee
+            fee += Decimal(str(tx.transaction_fee))
+    fee = float(fee)
     if fee > 0:
         tx_list.append(
             Transaction(
                 0,
                 "NARUNO",
                 "NARUNOA",
                 the_fee_address,
```

### Comparing `naruno-0.59.0/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.60.0/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,18 @@
 
 
         for block in self.candidate_blocks:
             temp_tx = [
                 Transaction.load_json(element)
                 for element in block["transaction"] if type(element) is dict
             ]
-            block["transaction"] = temp_tx
+            block["transaction"] = temp_tx
+
+
+        last_list = []
+        for block in self.candidate_blocks:
+            if int(block["total_length"]) == len(block["transaction"]):
+                last_list.append(block)
+
+        self.candidate_blocks = last_list
+
+
```

### Comparing `naruno-0.59.0/naruno/cli/main.py` & `naruno-0.60.0/naruno/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import argparse
 import os
 import sys
+import threading
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 import time
 from getpass import getpass
 
 from naruno.accounts.get_balance import GetBalance
 from naruno.blockchain.block.create_block import CreateBlock
@@ -103,14 +104,21 @@
         menu_space() + menu_maker(menu_number="publishermodeon",
                                   menu_text="Publisher Mode On") +
         menu_maker(menu_number="publishermodeoff",
                    menu_text="Publisher Mode Off") + menu_space())
 
     print(quit_menu_maker(mode="main"))
 
+def get_block_process():
+                the_block = CreateBlock()
+                SaveBlock(the_block)
+                server.Server.send_block_to_other_nodes()
+                logger.info("Consensus timer is started")
+                perpetualTimer(the_block.consensus_timer, consensus_trigger, the_consensus=True)    
+
 
 def menu():
     """
     The main structure of the cli mode, this function prints the menu,
     listens to the entries, makes the directions.
     """
 
@@ -213,19 +221,15 @@
                 print("You have not a transaction")
 
         if choices_input == "returntrs":
             PrintTransactions()
 
         if choices_input == "getblock":
             if the_settings()["test_mode"]:
-                the_block = CreateBlock()
-                SaveBlock(the_block)
-                server.Server.send_block_to_other_nodes()
-                logger.info("Consensus timer is started")
-                perpetualTimer(the_block.consensus_timer, consensus_trigger)
+                get_block_process()
             else:
                 server.Server.send_me_full_block()
 
         if choices_input == "status":
             print(Status())
 
         if choices_input == "getproof":
```

### Comparing `naruno-0.59.0/naruno/config.py` & `naruno-0.60.0/naruno/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 LOADING_BLOCK_PATH = "db/loading_block.naruno.json"
 LOADING_ACCOUNTS_PATH = "db/loading_block_accounts.naruno.db"
 LOADING_BLOCKSHASH_PATH = "db/loading_block_blockshash.naruno.json"
 LOADING_BLOCKSHASH_PART_PATH = "db/loading_block_blockshash_part.naruno.json"
 
 BLOCKS_PATH = "db/blocks/"
-PENDING_TRANSACTIONS_PATH = "db/pending_transactions/"
+PENDING_TRANSACTIONS_PATH = None
 
 WALLETS_PATH = "db/wallet_list.json"
 
 MY_TRANSACTION_PATH = "db/my_transactions/"
 
 # Export
 MY_TRANSACTION_EXPORT_PATH = "db/my_transaction.csv"
```

### Comparing `naruno-0.59.0/naruno/consensus/consensus_main.py` & `naruno-0.60.0/naruno/consensus/consensus_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import threading
-
+import traceback
+import contextlib
 from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.candidate_block.candidate_block_main import \
     candidate_block
 from naruno.consensus.finished.finished_main import finished_main
 from naruno.consensus.ongoing.ongoing_main import ongoing_main
 from naruno.consensus.sync.sync import sync
 from naruno.lib.log import get_logger
 from naruno.node.client.client import client
 from naruno.node.server.server import server
 from naruno.transactions.pending.get_pending import GetPending
+import naruno
 
 logger = get_logger("CONSENSUS")
 
 
 def consensus_trigger(
     custom_block: Block = None,
     custom_candidate_class: candidate_block = None,
@@ -37,58 +39,67 @@
     dont_clean=False,
 ) -> Block:
     """
     Consensus process consists of 2 stages. This function makes
     the necessary redirects according to the situation and works
     to shorten the block time.
     """
+    with contextlib.suppress(Exception):
+        naruno.lib.perpetualtimer.the_consensus_thread = True
 
-    block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-             if custom_block is None else custom_block)
-    pending_list_txs = GetPending()
-
-    logger.info(
-        f"BLOCK#{block.sequence_number}:{block.empty_block_number} Consensus process started"
-    )
-
-    logger.info("Consensus Sync process started")
-    threading.Thread(
-        target=sync,
-        args=(
-            block,
-            pending_list_txs,
-            custom_server,
-        ),
-    ).start()
+    try:
+
+        block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+                if custom_block is None else custom_block)
+        pending_list_txs = GetPending()
 
-    if block.validated:
-        logger.info(
-            "BLOCK is an validated block, consensus process is finished")
-        finished_main(
-            block,
-            custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
-            custom_BLOCKS_PATH=custom_BLOCKS_PATH,
-            custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
-            custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
-            custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
-            pass_sync=pass_sync,
-            dont_clean=dont_clean,
-        )
-    else:
         logger.info(
-            "BLOCK is an unvalidated block, consensus process is ongoing")
-        ongoing_main(
-            block,
-            custom_candidate_class=custom_candidate_class,
-            custom_unl_nodes=custom_unl_nodes,
-            custom_UNL_NODES_PATH=custom_UNL_NODES_PATH,
-            custom_server=custom_server,
-            custom_unl=custom_unl,
-            custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
-            custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
-            custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
-            custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
-            pass_sync=pass_sync,
+            f"BLOCK#{block.sequence_number}:{block.empty_block_number} Consensus process started"
         )
 
+        logger.info("Consensus Sync process started")
+        threading.Thread(
+            target=sync,
+            args=(
+                block,
+                pending_list_txs,
+                custom_server,
+            ),
+        ).start()
+
+        if block.validated:
+            logger.info(
+                "BLOCK is an validated block, consensus process is finished")
+            finished_main(
+                block,
+                custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
+                custom_BLOCKS_PATH=custom_BLOCKS_PATH,
+                custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
+                custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
+                custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
+                pass_sync=pass_sync,
+                dont_clean=dont_clean,
+            )
+        else:
+            logger.info(
+                "BLOCK is an unvalidated block, consensus process is ongoing")
+            ongoing_main(
+                block,
+                custom_candidate_class=custom_candidate_class,
+                custom_unl_nodes=custom_unl_nodes,
+                custom_UNL_NODES_PATH=custom_UNL_NODES_PATH,
+                custom_server=custom_server,
+                custom_unl=custom_unl,
+                custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
+                custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
+                custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
+                custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
+                pass_sync=pass_sync,
+            )
+    except:
+        traceback.print_exc()
+
     logger.info("Consensus process is done")
+    with contextlib.suppress(Exception):
+        naruno.lib.perpetualtimer.the_consensus_thread = False    
+
     return block
```

### Comparing `naruno-0.59.0/naruno/consensus/finished/finished_main.py` & `naruno-0.60.0/naruno/consensus/finished/finished_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
+import contextlib
 import os
 import shutil
 import time
 
 from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.blocks_hash import GetBlockshash
 from naruno.blockchain.block.blocks_hash import GetBlockshash_part
@@ -26,28 +27,37 @@
 from naruno.consensus.finished.true_time.true_time_main import true_time
 from naruno.lib.log import get_logger
 from naruno.lib.mix.merkle_root import MerkleTree
 from naruno.lib.settings_system import save_settings
 from naruno.lib.settings_system import the_settings
 from naruno.node.server.server import server
 from naruno.transactions.pending_to_validating import PendingtoValidating
+from naruno.transactions.cleaner import Cleaner
+from naruno.transactions.pending.get_pending import GetPending
+import naruno
 
 logger = get_logger("CONSENSUS")
-
-
+def make_sync(the_server):
+    logger.info("Syncing the block to other nodes is triggered")
+    with contextlib.suppress(Exception):
+        [
+            the_server.send_block_to_other_nodes(sync_client, sync=True)
+            for sync_client in the_server.sync_clients
+        ]
 def finished_main(
     block: Block,
     custom_TEMP_BLOCK_PATH: str = None,
     custom_BLOCKS_PATH: str = None,
     custom_TEMP_ACCOUNTS_PATH: str = None,
     custom_TEMP_BLOCKSHASH_PATH: str = None,
     custom_TEMP_BLOCKSHASH_PART_PATH: str = None,
     custom_server: server = None,
     pass_sync: bool = False,
     dont_clean=False,
+    force_sync: bool = False,
 ) -> None:
     the_server = None
     if custom_server is None:
         the_server = server.Server
     else:
         the_server = custom_server
 
@@ -60,68 +70,77 @@
     the_TEMP_BLOCKSHASH_PART_PATH = (TEMP_BLOCKSHASH_PART_PATH if
                                      custom_TEMP_BLOCKSHASH_PART_PATH is None
                                      else custom_TEMP_BLOCKSHASH_PART_PATH)
 
     the_TEMP_BLOCK_PATH = (TEMP_BLOCK_PATH if custom_TEMP_BLOCK_PATH is None
                            else custom_TEMP_BLOCK_PATH)
     block.sync_empty_blocks() if pass_sync is False else None
+    make_sync(the_server) if force_sync is True else None
     if true_time(block):
-        logger.debug(
+        logger.info(
             "Consensus proccess is complated, the block will be reset")
 
         reset_block = block.reset_the_block()
+        logger.debug("Block reseted")
 
         settings = the_settings()
         if reset_block != False:
+            
             block2 = reset_block[0]
 
             new_tx_from_us = False
             new_transactions_list = transactions_main(block2)
-            if new_transactions_list is not None:
+            if new_transactions_list:
+                logger.debug("New transactions list is not None")
                 SaveBlockstoBlockchainDB(
                     block2,
                     custom_BLOCKS_PATH=the_BLOCKS_PATH,
                     custom_TEMP_ACCOUNTS_PATH=the_TEMP_ACCOUNTS_PATH,
                     custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH,
                     custom_TEMP_BLOCKSHASH_PART_PATH=
                     the_TEMP_BLOCKSHASH_PART_PATH,
                     dont_clean=dont_clean,
                 )
                 new_tx_from_us = True
                 settings["save_blockshash"] = True
                 save_settings(settings)
             if block2.sequence_number == 0:
+                logger.debug("Block sequence number is 0")
                 SaveBlockstoBlockchainDB(
                     block2,
                     custom_BLOCKS_PATH=the_BLOCKS_PATH,
                     custom_TEMP_ACCOUNTS_PATH=the_TEMP_ACCOUNTS_PATH,
                     custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH,
                     custom_TEMP_BLOCKSHASH_PART_PATH=
                     the_TEMP_BLOCKSHASH_PART_PATH,
                     force=True,
                     dont_clean=dont_clean,
                 )
 
+
             SaveBlockshash(
                 reset_block[1].previous_hash,
                 custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH,
             )
+            logger.debug("Blockshash saved")
 
             the_blocks_hash = GetBlockshash(
                 custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH)
 
             if len(the_blocks_hash) == block.part_amount:
-                block.empty_block_number += block.gap_block_number
+                logger.debug("Blockshash length is equal to part amount")
+                block.empty_block_number += block.gap_block_number + block.hard_block_number
 
                 block.sync = True
                 SaveBlockshash_part(
                     MerkleTree(the_blocks_hash).getRootHash(),
                     custom_TEMP_BLOCKSHASH_PART_PATH=
                     the_TEMP_BLOCKSHASH_PART_PATH,
                 )
+                logger.debug("Blockshash part saved")
                 the_blockshas_part = GetBlockshash_part(
                     custom_TEMP_BLOCKSHASH_PART_PATH=
                     the_TEMP_BLOCKSHASH_PART_PATH)
                 block.part_amount_cache = MerkleTree(
                     the_blockshas_part).getRootHash()
                 if settings["save_blockshash"] == True:
                     shutil.copyfile(
@@ -139,37 +158,34 @@
                          ".blockshash_full.json"),
                     )
                 os.remove(the_TEMP_BLOCKSHASH_PATH)
 
                 difference = (block.start_time +
                               (block.hard_block_number *
                                block.block_time)) - int(time.time())
-                time.sleep(difference)
+                if difference > 0:
+                    time.sleep(difference)    
+                block.sync = False         
+                make_sync(the_server)
+
+
 
+
+        Cleaner(block, pending_list_txs=GetPending(), disable_already_in_2=False)
         PendingtoValidating(block)
+        logger.debug("Pending to validating is complated")
         SaveBlock(
             block,
             custom_TEMP_BLOCK_PATH=the_TEMP_BLOCK_PATH,
             custom_TEMP_ACCOUNTS_PATH=the_TEMP_ACCOUNTS_PATH,
             custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH,
             custom_TEMP_BLOCKSHASH_PART_PATH=the_TEMP_BLOCKSHASH_PART_PATH,
         )
+        with contextlib.suppress(Exception):
+            naruno.consensus.sync.sync.sync_round_1 = True
+            naruno.consensus.sync.sync.sended_txs = []
+            naruno.node.server.server.tx_signature_list = {}
         return True
     else:
-        if block.sync == True:
-            block.sync = False
-            SaveBlock(
-                block,
-                custom_TEMP_BLOCK_PATH=the_TEMP_BLOCK_PATH,
-                custom_TEMP_ACCOUNTS_PATH=the_TEMP_ACCOUNTS_PATH,
-                custom_TEMP_BLOCKSHASH_PATH=the_TEMP_BLOCKSHASH_PATH,
-                custom_TEMP_BLOCKSHASH_PART_PATH=the_TEMP_BLOCKSHASH_PART_PATH,
-            )
-            [
-                the_server.send_block_to_other_nodes(sync_client, sync=True)
-                for sync_client in the_server.sync_clients
-            ]
-            the_server.sync_clients = []
-
-        logger.debug(
+        logger.info(
             "Consensus proccess is complated, waiting for the true time")
         return False
```

### Comparing `naruno-0.59.0/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.60.0/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.60.0/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from naruno.blockchain.candidate_block.candidate_block_main import \
     candidate_block
+from naruno.blockchain.block.block_main import Block
 from naruno.lib.log import get_logger
 
-logger = get_logger("CONSENSUS_FIRST_ROUND")
+logger = get_logger("CONSENSUS_SECOND_ROUND")
 
 
-def candidate_blocks_check(candidate_class: candidate_block,
-                           unl_nodes: dict) -> bool:
-    logger.info("Candidate block control started for round 2")
+def candidate_blocks_hashes_check(candidate_class: candidate_block,
+                                  unl_nodes: dict, block=None) -> bool:
+    logger.info("Candidate block hash control started for round 2")
     logger.debug(
-        f"len(candidate_class.candidate_blocks): {len(candidate_class.candidate_blocks)}"
+        f"len(candidate_class.candidate_block_hashes): {len(candidate_class.candidate_block_hashes)}"
     )
     logger.debug(f"len(unl_nodes): {len(unl_nodes)}")
-    if len(candidate_class.candidate_blocks) > ((
-        (len(unl_nodes) + 1) * 50) / 100):
-        logger.info("Candidate block number is True")
+
+    the_block = Block(creator="Naruno") if block is None else block
+    if len(candidate_class.candidate_block_hashes) > ((
+        (len(unl_nodes) + 1) * the_block.candidate_blocks_hashes_check) / 100):
+        logger.info("Candidate block hash number is True")
         return True
     else:
-        logger.info("Candidate block number is not True")
+        logger.info("Candidate block hash number is not True")
         return False
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         block=block,
         custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
         custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
         custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
         custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,           
         ):
         return False    
-    if not candidate_blocks_check(candidate_class, unl_nodes):
+    if not candidate_blocks_check(candidate_class, unl_nodes, block=block):
         return False
     logger.info("Round 1 checking is True")
     return True
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     logger.debug(f"current_time: {current_time}")
     logger.debug(f"the_time: {the_time}")
     if current_time >= the_time:
         logger.info("Time is true")
         return True
     else:
         if not current_time >= the_time - (block.round_1_time / 2):
-            PendingtoValidating(block)
+            #PendingtoValidating(block)
             SaveBlock(
                 block,
                 custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
                 custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
                 custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
                 custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
             )
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,21 +40,23 @@
                       clean=clean)
 
     block.round_1 = True
     block.round_2_starting_time = block.start_time + block.round_1_time
 
     account_list = GetAccounts(
         custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH)
-    block = ProccesstheTransaction(
+    resukt_of_proccesstransaction = ProccesstheTransaction(
         block,
         account_list,
         custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
         custom_shares=custom_shares,
         custom_fee_address=custom_fee_address,
     )
+    block = resukt_of_proccesstransaction[0]
+    account_list = resukt_of_proccesstransaction[1]
 
     part_of_blocks_hash = GetBlockshash_part(
         custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH)
     the_blocks_hash = GetBlockshash(
         custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH)
     logger.debug(f"part_of_blocks_hash: {part_of_blocks_hash}")
     logger.debug(f"the_blocks_hash: {the_blocks_hash}")
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                             if other_block_tx.signature == other_block_txs.signature:
                                 tx_valid += 1
             else:
                 tx_valid += 1
 
             logger.debug(
                 f"Tx valid of {other_block_tx.signature} : {tx_valid}")
-            if tx_valid > ((len(unl_nodes) + 1) / 2):
+            if tx_valid > (((len(unl_nodes) + 1) * block.find_validated) / 100):
                 already_in_ok = False
                 for alrady_tx in temp_validating_list[:]:
                     if other_block_tx.signature == alrady_tx.signature:
                         logger.debug("The transaction is already in the list")
                         already_in_ok = True
                 if not already_in_ok:
                     logger.debug(
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     candidate_block
 from naruno.consensus.rounds.round_1.checks.checks_main import round_check
 from naruno.consensus.rounds.round_1.process.process_main import round_process
 from naruno.lib.log import get_logger
 from naruno.node.get_candidate_blocks import GetCandidateBlocks
 from naruno.node.server.server import server
 from naruno.node.unl import Unl
-
+import naruno
 logger = get_logger("CONSENSUS_FIRST_ROUND")
 
 
 def consensus_round_1(
     block: Block,
     custom_candidate_class: candidate_block = None,
     custom_unl_nodes: dict = None,
@@ -45,15 +45,15 @@
         f"BLOCK#{block.sequence_number}:{block.empty_block_number} First round is starting"
     )
 
     unl_nodes = (Unl.get_unl_nodes(custom_UNL_NODES_PATH=custom_UNL_NODES_PATH)
                  if custom_unl_nodes is None else custom_unl_nodes)
     logger.debug(f"unl_nodes: {unl_nodes}")
     candidate_class = (GetCandidateBlocks(
-        custom_nodes_list=Unl.get_as_node_type(unl_nodes), block=block)
+        custom_nodes_list=Unl.get_as_node_type(unl_nodes)+Unl.get_as_node_type(unl_nodes, c_type=3), block=block)
                        if custom_candidate_class is None else
                        custom_candidate_class)
     logger.debug(f"candidate_class: {candidate_class.__dict__}")
 
     if round_check(
             block,
             candidate_class,
@@ -71,12 +71,13 @@
             custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
             custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
             custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
             custom_shares=custom_shares,
             custom_fee_address=custom_fee_address,
             clean=clean,
         )
+        naruno.consensus.sync.sync.sync_round_2 = True
         logger.info("Round 1 check is True")
         return True
     else:
         logger.warning("Round 1 check is False")
         return False
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from naruno.blockchain.candidate_block.candidate_block_main import \
     candidate_block
 from naruno.lib.log import get_logger
+from naruno.blockchain.block.block_main import Block
+logger = get_logger("CONSENSUS_FIRST_ROUND")
 
-logger = get_logger("CONSENSUS_SECOND_ROUND")
 
-
-def candidate_blocks_hashes_check(candidate_class: candidate_block,
-                                  unl_nodes: dict) -> bool:
-    logger.info("Candidate block hash control started for round 2")
+def candidate_blocks_check(candidate_class: candidate_block,
+                           unl_nodes: dict, block=None) -> bool:
+    logger.info("Candidate block control started for round 2")
     logger.debug(
-        f"len(candidate_class.candidate_block_hashes): {len(candidate_class.candidate_block_hashes)}"
+        f"len(candidate_class.candidate_blocks): {len(candidate_class.candidate_blocks)}"
     )
+
+    the_block = Block(creator="Naruno") if block is None else block
+
     logger.debug(f"len(unl_nodes): {len(unl_nodes)}")
-    if len(candidate_class.candidate_block_hashes) > ((
-        (len(unl_nodes) + 1) * 50) / 100):
-        logger.info("Candidate block hash number is True")
+    if len(candidate_class.candidate_blocks) > ((
+        (len(unl_nodes) + 1) * the_block.candidate_blocks_check) / 100):
+        logger.info("Candidate block number is True")
         return True
     else:
-        logger.info("Candidate block hash number is not True")
+        logger.info("Candidate block number is not True")
         return False
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 
 logger = get_logger("CONSENSUS_SECOND_ROUND")
 
 
 def round_check(block: Block, candidate_class: candidate_block,
                 unl_nodes: dict) -> bool:
     logger.info("Round 2 checking is started")
-    if not candidate_blocks_hashes_check(candidate_class, unl_nodes):
+    if not candidate_blocks_hashes_check(candidate_class, unl_nodes, block=block):
         return False
     if not time_difference_check(block=block):
         return False
     logger.info("Round 2 checking is True")
     return True
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,30 +34,30 @@
         for other_block in candidate_class.candidate_block_hashes[:]:
             if (candidate_block_hash != other_block
                     and candidate_block_hash["hash"] == other_block["hash"]):
                 tx_valid += 1
 
         logger.debug(f"Hash valid of  {candidate_block_hash} : {tx_valid}")
 
-        if tx_valid > (((len(unl_nodes)+1) * 50) / 100):
+        if tx_valid > (((len(unl_nodes)+1) * block.process_candidate_blocks_hashes) / 100):
             logger.info(
                 f"candidate_block_hash: {candidate_block_hash} is validated.")
             current_hash = candidate_block_hash
 
     for candidate_block_hash in candidate_class.candidate_block_hashes[:]:
         logger.debug(f"Candidate block hash previous_hash {candidate_block_hash}")
 
         tx_valid = 1
 
         for other_block in candidate_class.candidate_block_hashes[:]:
             if (candidate_block_hash != other_block
                     and candidate_block_hash["previous_hash"] == other_block["previous_hash"]):
                 tx_valid += 1
         logger.debug(f"Hash valid of previous_hash  {candidate_block_hash} : {tx_valid}")
-        if tx_valid > (((len(unl_nodes)+1) * 50) / 100):
+        if tx_valid > (((len(unl_nodes)+1) * block.process_candidate_blocks_hashes) / 100):
             logger.info(
                 f"candidate_block_hash previous_hash: {candidate_block_hash} is validated.")
             previous_hash = candidate_block_hash
 
 
 
     if current_hash != {"signature": "A", "hash": False, "previous_hash": False} or previous_hash != {"signature": "A", "hash": False, "previous_hash": False}:
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     logger.info("Rescue operation is started")
     logger.debug(f"First block: {block}")
     sender = candidate_block_hash["hash"]["sender"]
     logger.debug(
         f"Our block is not valid, the system will try to get true block from naruno.node {sender}"
     )
     block.dowload_true_block = sender
-    unl_list = Unl.get_as_node_type([sender])
+    unl_list = Unl.get_as_node_type([sender], c_type=2)
     the_server = server.Server if custom_server is None else custom_server
     the_unl_node = random.choice(
         unl_list) if custom_unl is None else custom_unl
     logger.info(f"True block requested from {the_unl_node}")
     the_server.send_client(the_unl_node, {"action": "sendmefullblock"})
     logger.debug(f"End block: {block}")
     return block
```

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.60.0/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/sync/send_block.py` & `naruno-0.60.0/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/consensus/sync/send_block_hash.py` & `naruno-0.60.0/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/POPPINS_LICENCE` & `naruno-0.60.0/naruno/gui/lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Black.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Bold.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Italic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Light.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Medium.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Regular.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-Thin.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.60.0/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/images/logo.ico` & `naruno-0.60.0/naruno/gui/lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/images/logo.png` & `naruno-0.60.0/naruno/gui/lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/images/logo_sm_orb_fw.png` & `naruno-0.60.0/naruno/gui/lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/images/logo_w_bc.png` & `naruno-0.60.0/naruno/gui/lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/images/logo_win.ico` & `naruno-0.60.0/naruno/gui/lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/node_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/node_screen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 import os
+import threading
 
 from kivy.core.clipboard import Clipboard
 from kivymd.toast import toast
 from kivymd.uix.button import MDFlatButton
 from kivymd.uix.gridlayout import MDGridLayout
 from kivymd.uix.screen import MDScreen
 from kivymd_extensions.sweetalert import SweetAlert
@@ -17,14 +18,20 @@
 from naruno.lib.perpetualtimer import perpetualTimer
 from naruno.lib.qr import qr
 from naruno.lib.settings_system import the_settings
 from naruno.lib.status import Status
 from naruno.node.server.server import server
 
 
+def get_block_process():
+            the_block = CreateBlock()
+            SaveBlock(the_block)
+            server.Server.send_block_to_other_nodes()
+            perpetualTimer(the_block.consensus_timer, consensus_trigger, the_consensus=True)
+
 class NodeScreen(MDScreen):
     pass
 
 
 class NodeBox(MDGridLayout):
     cols = 2
 
@@ -91,18 +98,15 @@
             ],
         )
 
     def get_block(self):
         if not self.check_node_server():
             return False
         if the_settings()["test_mode"]:
-            the_block = CreateBlock()
-            SaveBlock(the_block)
-            server.Server.send_block_to_other_nodes()
-            perpetualTimer(the_block.consensus_timer, consensus_trigger)
+            get_block_process()
         else:
             server.Server.send_me_full_block()
 
     def nd_id(self):
         Clipboard.copy(server.id)
         popup(title="The ID has been copied to your clipboard.",
               type="success")
```

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/operations_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/operations_screen.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from kivymd.uix.bottomsheet import MDListBottomSheet
 from kivymd.uix.button import MDFlatButton
 from kivymd.uix.gridlayout import MDGridLayout
 from kivymd.uix.screen import MDScreen
 from kivymd_extensions.sweetalert import SweetAlert
 
 import naruno.gui.the_naruno_gui_app
+from naruno.accounts.get_balance import GetBalance
+from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.save_block import SaveBlock
 from naruno.config import MY_TRANSACTION_EXPORT_PATH
 from naruno.gui.popup import popup
 from naruno.lib.export import export_the_transactions
 from naruno.lib.settings_system import the_settings
 from naruno.lib.sign import sign
@@ -33,47 +35,59 @@
     pass
 
 
 class OperationBox(MDGridLayout):
     cols = 2
 
     def sent_the_coins(self):
-        the_block = GetBlock()
+        if not the_settings()["baklava"]:
+            the_block = GetBlock()
+        else:
+            the_block = Block("baklava")
+
+        the_balance = GetBalance(
+            self.send_coin_dialog.input_results["Receiver"],
+            dont_convert=True,
+            block=the_block,
+        )
 
         if (float(self.send_coin_dialog.input_results["Amount"])
-                >= the_block.minumum_transfer_amount):
+                >= the_block.minumum_transfer_amount) or the_balance >= 0:
             if (wallet_import(int(the_settings()["wallet"]), 2) == sha256(
                     self.send_coin_dialog.input_results["Password"].encode(
                         "utf-8")).hexdigest()):
                 block = the_block
                 send_tx = send(
                     self.send_coin_dialog.input_results["Password"],
                     self.send_coin_dialog.input_results["Receiver"],
                     amount=float(
                         self.send_coin_dialog.input_results["Amount"]),
                     data=str(self.send_coin_dialog.input_results["Data"]),
                     block=block,
                 )
                 if send_tx != False:
-                    from naruno.node.server.server import server
+                    SavetoMyTransaction(send_tx, sended=True)
+                    if not the_settings()["baklava"]:
+                        from naruno.node.server.server import server
 
-                    if server.Server is None:
-                        popup(title="Please start the node server",
-                              type="failure")
-                        return False
+                        if server.Server is None:
+                            popup(title="Please start the node server",
+                                  type="failure")
+                            return False
+                        server.send_transaction(send_tx)
+                        SaveBlock(block)
 
-                    SavetoMyTransaction(send_tx, sended=True)
-                    server.send_transaction(send_tx)
-                    SaveBlock(block)
             else:
                 popup(title="Password is not correct", type="failure")
+        else:
+            popup(title="Amount is not enough", type="failure")
 
     def show_send_coin_dialog(self):
         self.send_coin_dialog = popup(
-            title="Send Coin",
+            title="Send Coin&Data",
             target=self.sent_the_coins,
             inputs=[
                 ["Receiver", False],
                 ["Amount", False],
                 ["Data", False],
                 ["Password", True],
             ],
@@ -132,17 +146,18 @@
             target=self.verify_the_data,
             inputs=[["Path", False]],
         )
 
     def send_coin(self):
         try:
             GetBlock()
-        except FileNotFoundError:
-            popup(title="Please connect to an network.", type="failure")
-            return False
+        except TypeError:
+            if not the_settings()["baklava"]:
+                popup(title="Please connect to an network.", type="failure")
+                return False
         self.show_send_coin_dialog()
 
     def sign(self):
         self.show_sign_dialog()
 
     def verify(self):
         self.show_verify_dialog()
@@ -156,15 +171,15 @@
                 type="success",
             )
 
         else:
             popup(title="You have not a transaction", type="warning")
 
     def callback_for_transaction_history_items(self, *args):
-        the_signature_of_tx = args[0][:96]
+        the_signature_of_tx = args[0].signature
         Clipboard.copy(the_signature_of_tx)
         popup(
             title=
             "The signature of transaction has been copied to your clipboard.",
             text=f"The signature is : {the_signature_of_tx}",
             type="success",
         )
```

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/root_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/settings_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/settings_screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 from naruno.lib.backup.naruno_export import naruno_export
 from naruno.lib.backup.naruno_import import naruno_import
 from naruno.lib.settings_system import d_mode_settings
 from naruno.lib.settings_system import dark_mode_settings
 from naruno.lib.settings_system import mt_settings
 from naruno.lib.settings_system import t_mode_settings
 from naruno.lib.settings_system import the_settings
+from naruno.lib.settings_system import baklava_settings
 
 
 class SettingsScreen(MDScreen):
     pass
 
 
 class SettingsBox(MDGridLayout):
     cols = 2
 
     d_first_status = the_settings()["debug_mode"]
     t_first_status = the_settings()["test_mode"]
     mt_first_status = the_settings()["mute_notifications"]
     dark_mode_first_status = the_settings()["dark_mode"]
+    baklava_first_status = the_settings()["baklava"]
 
     def D_Status_Changing(self, instance, value):
         d_mode_settings(value)
 
     def T_Status_Changing(self, instance, value):
         t_mode_settings(value)
 
@@ -72,14 +74,18 @@
         else:
             self.alert.dismiss()
 
     def DARK_MODE_Status_Changing(self, instance, value):
         dark_mode_settings(value)
         self.show_dialog()
 
+    def BAKLAVA_Status_Changing(self, instance, value):
+        baklava_settings(value)
+
+
     def export_bt(self):
         export_location = naruno_export()
         Clipboard.copy(export_location)
         if platform == "android":
             from android.storage import primary_external_storage_path
 
             dir = primary_external_storage_path()
@@ -98,14 +104,15 @@
 
     def import_the_db(self):
         naruno_import(self.import_backup_dialog.input_results["Path"])
         SettingsBox.dark_mode_first_status = the_settings()["dark_mode"]
         SettingsBox.d_first_status = the_settings()["debug_mode"]
         SettingsBox.t_first_status = the_settings()["test_mode"]
         SettingsBox.mt_first_status = the_settings()["mute_notifications"]
+        SettingsBox.baklava_first_status = the_settings()["baklava"]
         naruno.gui.the_naruno_gui_app.the_naruno_gui.restart()
 
     def import_bt(self):
         self.import_backup_dialog = popup(
             title="Import your export (App Will Restart)",
             target=self.import_the_db,
             inputs=[["Path", False]],
```

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/tabnavigation.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/wallet_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/baseclass/welcome_screen.py` & `naruno-0.60.0/naruno/gui/lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/node_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/operations_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/operations_screen.kv`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         AnchorLayout:
             size_hint_y: None
             height: but1.height
             MDRoundFlatIconButton:
                 id: but1
                 icon: "send-circle-outline"
                 on_press: root.send_coin()
-                text: "Send Coin"
+                text: "Send Coin&Data"
                 halign: "right"
                 font_style: "Button"
 
 
         AnchorLayout:
             size_hint_y: None
             height: but2.height
```

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/root_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/settings_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/settings_screen.kv`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,27 @@
         AnchorLayout:
             anchor_x: 'center'
             anchor_y: 'center'
             MDSwitch:
                 active: root.dark_mode_first_status
                 on_active: root.DARK_MODE_Status_Changing(self, self.active)
 
+
+
+        NarunoLabel:
+            text: "BAKLAVA"
+            halign: "center"
+            font_style: "Button"
+        AnchorLayout:
+            anchor_x: 'center'
+            anchor_y: 'center'
+            MDSwitch:
+                active: root.baklava_first_status
+                on_active: root.BAKLAVA_Status_Changing(self, self.active)
+
         AnchorLayout:
             size_hint_y: None
             height: but1.height
             MDRoundFlatIconButton:
                 id: but1
                 icon: "export"
                 on_press: root.export_bt()
```

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/tabnavigation.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/wallet_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/lib/libs/kv/welcome_screen.kv` & `naruno-0.60.0/naruno/gui/lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/main.py` & `naruno-0.60.0/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/gui/popup.py` & `naruno-0.60.0/naruno/gui/popup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import os
 
 from kivymd.uix.button import MDFlatButton
+from kivymd.uix.gridlayout import MDGridLayout
 from kivymd.uix.textfield import MDTextField
 from kivymd_extensions.sweetalert import SweetAlert
 
 import naruno.gui.the_naruno_gui_app
 
 
 class popup:
@@ -50,15 +51,14 @@
     def show(self):
         self.dialog.open()
 
     def dismiss(self, widget=None):
         self.dialog.dismiss()
 
     def clean(self):
-
         for obj in self.dialog.content_cls.children:
             if isinstance(obj, MDTextField):
                 obj.text = ""
 
     def director(self, widget):
         print("director")
 
@@ -77,42 +77,47 @@
         print("director")
         self.target()
         self.dismiss()
 
     def create(self):
         if self.dialog is None:
             if self.type == "custom":
+                custom_content_cls = MDGridLayout(
+                    adaptive_height=True,
+                    padding=("24dp", "68dp", "24dp", "24dp"),
+                    spacing="24dp",
+                    cols=2,
+                )
                 self.dialog = SweetAlert(
                     title=self.title,
                     type=self.type,
                     auto_dismiss=False,
                     buttons=[
                         MDFlatButton(
                             text="CANCEL",
                             font_size="18sp",
                             on_press=self.dismiss,
                             font_name=os.path.join(
-                                naruno.gui.
-                                the_naruno_gui_app.
-                                the_naruno_gui.FONT_PATH,
+                                naruno.gui.the_naruno_gui_app.the_naruno_gui.
+                                FONT_PATH,
                                 "Poppins-Bold",
                             ),
                         ),
                         MDFlatButton(
                             text="OK",
                             font_size="18sp",
                             font_name=os.path.join(
-                                naruno.gui.
-                                the_naruno_gui_app.
-                                the_naruno_gui.FONT_PATH,
+                                naruno.gui.the_naruno_gui_app.the_naruno_gui.
+                                FONT_PATH,
                                 "Poppins-Bold",
                             ),
                             on_press=self.director,
                         ),
                     ],
+                    content_cls=custom_content_cls,
                 )
 
                 for i in self.inputs:
                     content = i[0]
                     is_pass = i[1]
                     self.dialog.content_cls.add_widget(
                         MDTextField(hint_text=content,
@@ -137,26 +142,24 @@
                     type=self.type,
                     buttons=[
                         MDFlatButton(
                             text="NO",
                             font_size="18sp",
                             on_press=self.dismiss,
                             font_name=os.path.join(
-                                naruno.gui.
-                                the_naruno_gui_app.
-                                the_naruno_gui.FONT_PATH,
+                                naruno.gui.the_naruno_gui_app.the_naruno_gui.
+                                FONT_PATH,
                                 "Poppins-Bold",
                             ),
                         ),
                         MDFlatButton(
                             text="YES",
                             font_size="18sp",
                             font_name=os.path.join(
-                                naruno.gui.
-                                the_naruno_gui_app.
-                                the_naruno_gui.FONT_PATH,
+                                naruno.gui.the_naruno_gui_app.the_naruno_gui.
+                                FONT_PATH,
                                 "Poppins-Bold",
                             ),
                             on_press=self.director_without_input,
                         ),
                     ],
                 )
```

### Comparing `naruno-0.59.0/naruno/lib/backup/naruno_export.py` & `naruno-0.60.0/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/backup/naruno_import.py` & `naruno-0.60.0/naruno/lib/backup/naruno_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import copy
 import os
 import shutil
 import sys
+import json
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", "..", ".."))
 from naruno.lib.config_system import get_config, save_config
 from naruno.lib.log import get_logger
 from naruno.lib.settings_system import save_settings, temp_json, the_settings
+from naruno.config import WALLETS_PATH
+from naruno.wallet.save_wallet_list import save_wallet_list
 
 logger = get_logger("LIB")
 
 
 def naruno_import(export_location: str) -> None:
     """
     Extract a ZIP archive to the `db` folder in the main directory of the application.
@@ -37,8 +40,17 @@
     after_backup_settings = the_settings()
     for element in temp_json:
         if element not in after_backup_settings:
             after_backup_settings[element] = temp_json[element]
 
     save_settings(after_backup_settings)
 
+
+    #Wallets before KOT
+    old_wallet = os.path.join(main_folder, WALLETS_PATH)
+    if os.path.exists(old_wallet):
+        with open(old_wallet, "r") as wallet_list_file:
+            wallets = json.load(wallet_list_file)
+            save_wallet_list(wallets)
+
+
     logger.info("Import completed")
```

### Comparing `naruno-0.59.0/naruno/lib/clean_up.py` & `naruno-0.60.0/naruno/lib/clean_up.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import contextlib
 import os
 import shutil
 import sys
+import copy
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 
+import naruno
 from naruno.lib.config_system import get_config
 
+from naruno.lib.kot import KOT
 
 def CleanUp_tests():
+
+    with contextlib.suppress(AttributeError):
+        naruno.accounts.save_accounts.accounts_ram_db = {}
+
+
+    
+
     os.chdir(get_config()["main_folder"])
     for the_file in os.listdir("db/"):
         if the_file.startswith("test_"):
             if os.path.isfile(f"db/{the_file}"):
                 with contextlib.suppress(PermissionError):
                     os.remove(f"db/{the_file}")
```

### Comparing `naruno-0.59.0/naruno/lib/config_system.py` & `naruno-0.60.0/naruno/lib/config_system.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import json
 import os
 
 from naruno.config import CONFIG_PATH
+from naruno.lib.kot import KOT
+
+config_db = KOT("config",
+                folder=os.path.join(os.path.dirname(__file__), "..") + "/db")
 
 
 def save_config(config):
     """
     Saves the settings.
     """
 
-    temp_folder = os.path.dirname(os.path.realpath(__file__))
-    os.chdir(temp_folder)
-    os.chdir("..")
-    with open(CONFIG_PATH, "w") as config_file:
-        json.dump(config, config_file, indent=4)
+    config_db.set("config", config)
 
 
 def create_and_save_the_configs():
     """
     Creates and saves configs.
     """
 
@@ -34,11 +34,11 @@
 
 def get_config():
     """
     Returns the configs. If it doesn't exist, it creates,
     saves and returns.
     """
 
-    if not os.path.exists(CONFIG_PATH):
+    record = config_db.get("config")
+    if record is None:
         return create_and_save_the_configs()
-    with open(CONFIG_PATH, "r") as config_file:
-        return json.load(config_file)
+    return record
```

### Comparing `naruno-0.59.0/naruno/lib/encryption.py` & `naruno-0.60.0/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/export.py` & `naruno-0.60.0/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/log.py` & `naruno-0.60.0/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/mix/merkle_root.py` & `naruno-0.60.0/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/mix/mixlib.py` & `naruno-0.60.0/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/notification.py` & `naruno-0.60.0/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/accounts.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", "..", ".."))
 
 from naruno.accounts.account import Account
 from naruno.accounts.get_accounts import GetAccounts
 from naruno.accounts.save_accounts import SaveAccounts
 from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.hash.accounts_hash import AccountsHash
+from naruno.lib.config_system import get_config
 
 
 class Accounts_IO_Performance_Analyzer:
     """
     This class is used to analyze the performance of GetBlock
     """
 
@@ -47,19 +48,26 @@
         """
         This function is used to analyze the performance of GetBlock
         """
 
         result = (
             calculate(self.save_operation)[0],
             calculate(self.get_operation)[0],
-            os.path.getsize("db/Accounts_Performance_Analyzer_accounts.pf") /
-            1000000,
+            os.path.getsize(
+                os.path.join(
+                    get_config()["main_folder"],
+                    "db/Accounts_Performance_Analyzer_accounts.pf",
+                )) / 1000000,
         )
 
-        os.remove("db/Accounts_Performance_Analyzer_accounts.pf")
+        os.remove(
+            os.path.join(
+                get_config()["main_folder"],
+                "db/Accounts_Performance_Analyzer_accounts.pf",
+            ))
 
         return result
 
     def save_operation(self):
         """
         This function is used to analyze the performance of GetBlock
         """
```

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/block.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.60.0/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/perpetualtimer.py` & `naruno-0.60.0/naruno/lib/perpetualtimer.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,33 +3,47 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import contextlib
 import json
 from threading import Event, Thread, Timer
-
+import naruno
+import time
+the_consensus_thread = False
 
 class perpetualTimer(Timer):
     """
     It trig the functions at time intervals, independent of the main process.
 
     perpetualTimer class consists of 3 elements:
       * t: The time interval of perpetualTimer.
       * hFunction: The function to be triggered.
     """
 
-    def __init__(self, interval, function, args=None, kwargs=None):
+    def __init__(self, interval, function, args=None, kwargs=None, the_consensus = False):
         Thread.__init__(self)
         self.interval = interval
         self.function = function
         self.args = args if args is not None else []
         self.kwargs = kwargs if kwargs is not None else {}
+        self.consensus = the_consensus
         self.finished = Event()
 
         if self.interval != 0:
             self.start()
 
+    def execute_the_f(self):
+        with contextlib.suppress(json.decoder.JSONDecodeError):
+            self.function(*self.args, **self.kwargs)
+
+
+
     def run(self):
         while not self.finished.wait(self.interval):
-            with contextlib.suppress(json.decoder.JSONDecodeError):
-                self.function(*self.args, **self.kwargs)
+            if self.consensus:
+                if naruno.lib.perpetualtimer.the_consensus_thread:
+                    time.sleep(0.5)
+                else:
+                    self.execute_the_f()
+            else:
+                self.execute_the_f()
```

### Comparing `naruno-0.59.0/naruno/lib/qr.py` & `naruno-0.60.0/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/safety.py` & `naruno-0.60.0/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/settings_system.py` & `naruno-0.60.0/naruno/lib/settings_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import json
 import os
 
 from naruno.config import SETTING_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
+
+settings_db = KOT("settings", folder=get_config()["main_folder"] + "/db")
 
 temp_json = {
     "test_mode": False,
     "funtionaltest_mode": False,
     "debug_mode": False,
     "wallet": 0,
     "save_blockshash": True,
@@ -29,18 +32,15 @@
 }
 
 
 def save_settings(new_settings):
     """
     Saves the settings.
     """
-
-    os.chdir(get_config()["main_folder"])
-    with open(SETTING_PATH, "w") as settings_file:
-        json.dump(new_settings, settings_file, indent=4)
+    settings_db.set("settings", new_settings)
 
 
 def create_and_save_the_settings(test_mode_settings=False,
                                  debug_mode_settings=True):
     """
     Creates and saves settings.
     """
@@ -161,20 +161,18 @@
 
 def the_settings():
     """
     Returns the settings. If it doesn't exist, it creates,
     saves and returns.
     """
 
-    os.chdir(get_config()["main_folder"])
-
-    if not os.path.exists(SETTING_PATH):
-        return create_and_save_the_settings()
-    with open(SETTING_PATH, "r") as settings_file:
-        the_setting = json.load(settings_file)
+    the_setting = settings_db.get("settings")
+    if the_setting is None:
+        create_and_save_the_settings()
+        the_setting = settings_db.get("settings")
 
     missing = False
     for element in temp_json:
         if element not in the_setting:
             missing = True
             the_setting[element] = temp_json[element]
     if missing:
```

### Comparing `naruno-0.59.0/naruno/lib/sign.py` & `naruno-0.60.0/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/lib/status.py` & `naruno-0.60.0/naruno/lib/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import time
-
+import copy
 from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.lib.settings_system import save_settings
 from naruno.lib.settings_system import the_settings
 from naruno.node.unl import Unl
 from naruno.transactions.my_transactions.get_my_transaction import \
     GetMyTransaction
@@ -20,34 +20,36 @@
     custom_UNL_NODES_PATH: str = None,
     custom_first_block: Block = None,
     custom_new_block: Block = None,
     custom_connections: list = None,
     custom_transactions: list = None,
     no_cache: bool = False,
     cache_time: int = 300,
-    wait_time=50,
+    wait_time=None,
 ) -> dict:
     """
     Returns the status of the network.
     """
     a_settings = the_settings()
     currently_time = time.time()
+    the_wait_time = wait_time if wait_time is not None else Block("status").block_time*3
 
     if (no_cache or a_settings["status_cache_time"] + cache_time <=
             currently_time) and (not a_settings["status_working"]
                                  or a_settings["status_cache_time"] +
-                                 wait_time + 2 <= currently_time):
+                                 the_wait_time + 2 <= currently_time):
         a_settings["status_working"] = True
         if not no_cache:
             a_settings["status_cache_time"] = time.time()
         save_settings(a_settings)
-        first_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-                       if custom_first_block is None else custom_first_block)
+        first_block = copy.copy((GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+                       if custom_first_block is None else custom_first_block))
 
-        time.sleep(wait_time)
+        
+        time.sleep(the_wait_time)
         new_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
                      if custom_new_block is None else custom_new_block)
 
         connections = (Unl.get_as_node_type(
             Unl.get_unl_nodes(custom_UNL_NODES_PATH=custom_UNL_NODES_PATH))
                        if custom_connections is None else custom_connections)
         connected_nodes = [
```

### Comparing `naruno-0.59.0/naruno/lib/verify.py` & `naruno-0.60.0/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/node/server/server.py` & `naruno-0.60.0/naruno/node/server/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,44 +10,55 @@
 import os
 import random
 import socket
 import time
 from hashlib import sha256
 from shutil import move
 from threading import Thread
+import traceback
 
+from naruno.accounts.save_accounts import accounts_db
 from naruno.blockchain.block.block_main import Block
+from naruno.blockchain.block.blocks_hash import blockshash_db
 from naruno.blockchain.block.change_transaction_fee import ChangeTransactionFee
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.save_block import SaveBlock
 from naruno.config import CONNECTED_NODES_PATH
 from naruno.config import LOADING_ACCOUNTS_PATH
 from naruno.config import LOADING_BLOCK_PATH
 from naruno.config import LOADING_BLOCKSHASH_PART_PATH
 from naruno.config import LOADING_BLOCKSHASH_PATH
 from naruno.config import PENDING_TRANSACTIONS_PATH
 from naruno.config import TEMP_ACCOUNTS_PATH
 from naruno.config import TEMP_BLOCK_PATH
 from naruno.config import TEMP_BLOCKSHASH_PART_PATH
 from naruno.config import TEMP_BLOCKSHASH_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 from naruno.lib.log import get_logger
 from naruno.node.client.client import client
 from naruno.node.unl import Unl
 from naruno.transactions.get_transaction import GetTransaction
 from naruno.transactions.transaction import Transaction
 from naruno.wallet.ellipticcurve.ecdsa import Ecdsa
 from naruno.wallet.ellipticcurve.privateKey import PrivateKey
 from naruno.wallet.ellipticcurve.publicKey import PublicKey
 from naruno.wallet.ellipticcurve.signature import Signature
 from naruno.wallet.wallet_import import wallet_import
 
-a_block = Block("onur")
-buffer_size = 6525 + int(
-    (a_block.max_data_size // a_block.max_tx_number) * 1.5)
+from naruno.node.get_candidate_blocks import self_candidates
+import naruno
+
+connectednodes_db = KOT("connectednodes",
+                        folder=get_config()["main_folder"] + "/db")
+ 
+
+
+tx_signature_list = {}
+
 
 
 class server(Thread):
     Server = None
     id = wallet_import(0, 0)
 
     def __init__(
@@ -107,17 +118,16 @@
         self.LOADING_BLOCKSHASH_PATH = (LOADING_BLOCKSHASH_PATH if
                                         custom_LOADING_BLOCKSHASH_PATH is None
                                         else custom_LOADING_BLOCKSHASH_PATH)
         self.LOADING_BLOCKSHASH_PART_PATH = (
             LOADING_BLOCKSHASH_PART_PATH if custom_LOADING_BLOCKSHASH_PART_PATH
             is None else custom_LOADING_BLOCKSHASH_PART_PATH)
 
-        self.CONNECTED_NODES_PATH = (CONNECTED_NODES_PATH
-                                     if custom_CONNECTED_NODES_PATH is None
-                                     else custom_CONNECTED_NODES_PATH)
+        self.CONNECTED_NODES_PATH = (None if custom_CONNECTED_NODES_PATH
+                                     is None else custom_CONNECTED_NODES_PATH)
 
         self.PENDING_TRANSACTIONS_PATH = (
             PENDING_TRANSACTIONS_PATH if custom_PENDING_TRANSACTIONS_PATH
             is None else custom_PENDING_TRANSACTIONS_PATH)
 
         self.custom_variables = custom_variables
 
@@ -131,14 +141,31 @@
         self.logger = get_logger(f"NODE_{self.host}_{self.port}")
 
         self.logger.info(f"Server started as {server.id}")
 
         self.logger.debug("Save messages: " + str(save_messages))
         self.logger.debug("Test mode: " + str(test))
 
+
+        self.send_busy = []
+
+
+        a_block = Block("onur")
+        self.logger.debug(f"Block max_data_size: {a_block.max_data_size}")
+        self.logger.debug(f"Block max_tx_number: {a_block.max_tx_number}")
+        self.buffer_size = 6525 + int(
+            (a_block.max_data_size // a_block.max_tx_number) * 1.5)
+        self.buffer_size_2 = 6525 + int(
+            (a_block.max_data_size // a_block.max_tx_number) * 1.5)
+        self.buffer_size_3 = 6525 + int(
+            (a_block.max_data_size // a_block.max_tx_number) * 5)    
+        self.buffer_size_4 = 6525 + int(
+            (a_block.max_data_size // a_block.max_tx_number) * 0.5)   
+
+      
         if not test:
             self.__class__.Server = self
             self.start()
 
     def check_connected(self, host, port):
         for a_client in self.clients:
             if a_client.host == host and a_client.port == port:
@@ -146,24 +173,27 @@
 
         return False
 
     def run(self):
         self.logger.info("Server ear started")
         self.sock.settimeout(10.0)
         while self.running:
-            with contextlib.suppress(socket.timeout):
+            with contextlib.suppress(Exception):
                 conn, addr = self.sock.accept()
                 self.logger.debug(f"New connection request: {addr}")
                 data = conn.recv(1024)
-                conn.send(self.id.encode("utf-8"))
-                client_id = data.decode("utf-8")
+                
+                raw_id = data.decode("utf-8")
+                client_id = raw_id.split("-")[0]
+                client_type = int(raw_id.split("-")[1])
+                conn.send((self.id+"-"+str(client_type)).encode("utf-8"))
                 self.logger.debug(f"New connection id: {client_id}")
                 if Unl.node_is_unl(client_id):
                     self.logger.info(f"Confirmed")
-                    self.clients.append(client(conn, addr, client_id, self))
+                    self.clients.append(client(conn, addr, client_id, self, c_type=client_type))
                     self.save_connected_node(addr[0], addr[1], client_id)
                 else:
                     self.logger.warning(f"Rejected")
             time.sleep(0.01)
 
     def stop(self):
         self.running = False
@@ -183,39 +213,69 @@
             str(data),
             PrivateKey.fromPem(wallet_import(0, 1)),
         ).toBase64()
 
         data["signature"] = sign
         return data
 
-    def send(self, data, except_client=None):
+    def send(self, data, except_client=None, c_type=0):
         data = self.prepare_message(data)
 
         for a_client in self.clients:
             if a_client != except_client:
-                self.send_client(a_client, data, ready_to_send=True)
+                if a_client.c_type == c_type:
+                    self.send_client(a_client, data, ready_to_send=True, c_type=c_type)
         try:
             del data["buffer"]
         except KeyError:
             pass
         return data
 
-    def send_client(self, node, data, ready_to_send=False):
+    def send_client(self, node, data, ready_to_send=False, c_type=0):
         self.logger.debug(
             f"Sending message: {data} to {node.host}:{node.port}={node.id}")
         if not ready_to_send:
             data = self.prepare_message(data)
-        if len(json.dumps(data).encode("utf-8")) < buffer_size:
-            data["buffer"] = "0" * (
-                (buffer_size - len(json.dumps(data).encode("utf-8"))) - 14)
-        with contextlib.suppress(socket.timeout):
-            node.socket.sendall(json.dumps(data).encode("utf-8"))
+
+
+
+        if c_type == 0:
+            the_buffer = self.buffer_size
+        elif c_type == 1:
+            the_buffer = self.buffer_size_2
+        elif c_type == 2:
+            the_buffer = self.buffer_size_3
+        elif c_type == 3:
+            the_buffer = self.buffer_size_4
+
+        before_buffer_size = len(json.dumps(data).encode("utf-8"))
+        self.logger.debug(
+            f"Before buffer size: {before_buffer_size}")
+
+        if before_buffer_size < the_buffer:
+            self.logger.debug("Buffer is not full")
+            self.logger.debug(f"the_buffer: {the_buffer}")
+            self.logger.debug(f"before_buffer_size: {before_buffer_size}")
+            result = ((the_buffer - before_buffer_size) - 14)
+            self.logger.debug(f"result: {result}")
+            data["buffer"] = "0" * result
+            self.logger.debug(
+                f"After buffer size: {len(json.dumps(data).encode('utf-8'))}")
+        while node.id+str(c_type) in self.send_busy:
+            time.sleep(0.01)
+        self.send_busy.append(node.id+str(c_type))
+        try:
+            with contextlib.suppress(socket.timeout):
+                node.socket.sendall(json.dumps(data).encode("utf-8"))
+                time.sleep(0.02)
+        except:
+            traceback.print_exc()
+        self.send_busy.remove(node.id+str(c_type))
         with contextlib.suppress(KeyError):
             del data["buffer"]
-        time.sleep(0.02)
         if self.save_messages:
             self.our_messages.append(data)
         return data
 
     def get_message(self, client, data, hash_of_data=""):
         self.logger.info(
             f"Starting to proccess the message ({hash_of_data}) of {client.id}:{client.host}:{client.port}"
@@ -256,59 +316,71 @@
 
         if not signature_verify:
             self.logger.error("Signature not valid")
             return False
 
         return True
 
-    def connect(self, host, port):
-        self.logger.info(f"Asking for new node on {host}:{port}")
-        connected = self.check_connected(host=host, port=port)
-        if not connected:
+
+    def _connect(self, host, port, c_type=0):
             self.logger.info(
                 "New connection request confirmed trying to connect")
             conn = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             conn.settimeout(10.0)
             addr = (host, port)
-            conn.connect(addr)
-            conn.send(server.id.encode("utf-8"))
             try:
-                client_id = conn.recv(1024).decode("utf-8")
+                conn.connect(addr)
+                conn.send((self.id+"-"+str(c_type)).encode("utf-8"))                
+                raw_id = conn.recv(1024).decode("utf-8")
+                client_id = raw_id.split("-")[0]
+                client_type = int(raw_id.split("-")[1])                
                 if Unl.node_is_unl(client_id):
                     self.logger.info(
                         f"Succesfully connected to {client_id} on {host}:{port}"
                     )
-                    self.clients.append(client(conn, addr, client_id, self))
+                    self.clients.append(client(conn, addr, client_id, self, c_type=client_type))
                     self.save_connected_node(addr[0], addr[1], client_id)
                     return True
             except socket.timeout:
                 self.logger.warning(f"Connection timeout")
                 conn.close()
+            except ConnectionRefusedError:
+                self.logger.warning(f"Connection refused")
+                conn.close()    
+
+    def connect(self, host, port):
+        self.logger.info(f"Asking for new node on {host}:{port}")
+        connected = self.check_connected(host=host, port=port)
+        if not connected:
+            self._connect(host, port)
+            time.sleep(1)
+            self._connect(host, port, c_type=1)
+            time.sleep(1)
+            self._connect(host, port, c_type=2)
+            time.sleep(1)
+            self._connect(host, port, c_type=3)
         else:
             self.logger.warning("Already connected")
 
     @staticmethod
     def get_connected_nodes(custom_CONNECTED_NODES_PATH=None):
         """
         Returns the connected nodes.
         """
 
-        the_CONNECTED_NODES_PATH = (CONNECTED_NODES_PATH
-                                    if custom_CONNECTED_NODES_PATH is None else
-                                    custom_CONNECTED_NODES_PATH)
-
         the_pending_list = {}
-        os.chdir(get_config()["main_folder"])
-        for entry in os.scandir(the_CONNECTED_NODES_PATH):
-            if entry.name != "README.md":
-                with open(entry.path, "r") as my_transaction_file:
-                    loaded_json = json.load(my_transaction_file)
-                    the_pending_list[loaded_json["host"] +
-                                     str(loaded_json["port"]) +
-                                     loaded_json["id"]] = loaded_json
+        all_records = (connectednodes_db.get_all()
+                       if custom_CONNECTED_NODES_PATH is None else KOT(
+                           "connectednodes" + custom_CONNECTED_NODES_PATH,
+                           folder=get_config()["main_folder"] + "/db",
+                       ).get_all())
+        for entry in all_records:
+            loaded_json = all_records[entry]
+            the_pending_list[loaded_json["host"] + str(loaded_json["port"]) +
+                             loaded_json["id"]] = loaded_json
 
         return the_pending_list
 
     def save_connected_node(self, host, port, node_id):
         """
         Saves the connected nodes.
         """
@@ -316,18 +388,20 @@
         node_list = {}
         node_list["id"] = node_id
         node_list["host"] = host
         node_list["port"] = port
 
         node_id = sha256(
             (node_id + host + str(port)).encode("utf-8")).hexdigest()
-        file_name = self.CONNECTED_NODES_PATH + f"{node_id}.json"
-        os.chdir(get_config()["main_folder"])
-        with open(file_name, "w") as connected_node_file:
-            json.dump(node_list, connected_node_file, indent=4)
+
+        connectednodes_db.set(
+            node_id, node_list) if self.CONNECTED_NODES_PATH is None else KOT(
+                "connectednodes" + self.CONNECTED_NODES_PATH,
+                folder=get_config()["main_folder"] + "/db",
+            ).set(node_id, node_list)
 
     @staticmethod
     def connectionfrommixdb(custom_server=None,
                             custom_CONNECTED_NODES_PATH=None):
         """
         Connects to the mixdb.
         """
@@ -344,20 +418,22 @@
                     node_list[element]["port"],
                 )
 
     def connected_node_delete(self, node):
         """
         Deletes a connected node.
         """
-        os.chdir(get_config()["main_folder"])
+
         node_id = sha256((node["id"] + node["host"] +
                           str(node["port"])).encode("utf-8")).hexdigest()
-        for entry in os.scandir(self.CONNECTED_NODES_PATH):
-            if entry.name == f"{node_id}.json":
-                os.remove(entry.path)
+        connectednodes_db.delete(
+            node_id) if self.CONNECTED_NODES_PATH is None else KOT(
+                "connectednodes" + self.CONNECTED_NODES_PATH,
+                folder=get_config()["main_folder"] + "/db",
+            ).delete(node_id)
 
     def direct_message(self, node, data, hash_of_data):
         if "sendmefullblock" == data["action"]:
             self.send_block_to_other_nodes(node, hash_of_data=hash_of_data)
 
         if "fullblock" == data["action"]:
             self.get_full_chain(data, node, hash_of_data=hash_of_data)
@@ -381,23 +457,32 @@
 
         if "myblockhash" == data["action"]:
             self.get_candidate_block_hash(data,
                                           node,
                                           hash_of_data=hash_of_data)
 
     def send_me_full_block(self, node=None):
-        the_node = node if node is not None else random.choice(self.clients)
+        the_node = node
+        choices = []
+        if the_node is None:
+            for i in self.clients:
+                if i.c_type == 2:
+                    choices.append(i)
+            the_node = random.choice(choices)
+
         self.logger.info(
             f"Sending sendmefullblock to {the_node.id}:{the_node.host}:{the_node.port}"
         )
-        self.send_client(the_node, {"action": "sendmefullblock"})
+        self.send_client(the_node, {"action": "sendmefullblock"}, c_type=2)
 
     def send_my_block(self, block: Block):
         self.logger.info(f"Sending my block to all nodes")
-        system = block
+        system = self_candidates(block)[0]
+
+        
 
         new_list = []
 
         signature_list = []
 
         for element in system.validating_list:
             tx_json = element.dump_json()
@@ -407,70 +492,78 @@
         first_element = [new_list[0]] if len(new_list) > 0 else []
 
         data = {
             "action": "myblock",
             "transaction": first_element,
             "total_length": len(new_list),
             "sequence_number":
-            system.sequence_number + system.empty_block_number,
+            system.sequence_number+system.empty_block_number,
             "adding": False,
         }
 
         self.send(data)
+        time.sleep(2)
 
         if len(new_list) > 1:
             for element in new_list[1:]:
                 data = {
                     "action": "myblock",
                     "transaction": [element],
                     "total_length": len(new_list),
                     "sequence_number":
-                    system.sequence_number + system.empty_block_number,
+                    system.sequence_number+system.empty_block_number,
                     "adding": True,
                 }
 
                 self.send(data)
 
+
     def send_my_block_hash(self, block):
         self.logger.info(f"Sending my block hash to all nodes")
-        system = block
+         
+        system = self_candidates(block)[1]
 
         data = {
             "action": "myblockhash",
             "hash": system.hash,
             "previous_hash": system.previous_hash,
             "sequence_number":
-            system.sequence_number + system.empty_block_number,
+            system.sequence_number+system.empty_block_number,
         }
 
-        self.send(data)
+        self.send(data, c_type=3)
 
     def get_candidate_block(self, data, node: client, hash_of_data=""):
         self.logger.info(f"Getting candidate block with {hash_of_data}")
         self.logger.debug(
             f"Getting candidate block from {node.id}:{node.host}:{node.port}")
         if node.candidate_block is None:
             node.candidate_block = data
             return
         if data["sequence_number"] > node.candidate_block["sequence_number"]:
+            self.logger.debug("Candidate block is updated directly")
             if len(node.candidate_block_history) >= 5:
                 node.candidate_block_history.pop(0)
 
             node.candidate_block_history.append(copy.copy(
                 node.candidate_block))
             node.candidate_block = data
         else:
+            self.logger.debug("Candidate block is not updated directly")
             if node.candidate_block["total_length"] <= data["total_length"]:
                 if node.candidate_block["total_length"] == data[
                         "total_length"]:
                     if data["adding"]:
-                        node.candidate_block["transaction"].append(
-                            data["transaction"][0])
-                    else:
-                        node.candidate_block = data
+                        control = True
+                        for i in node.candidate_block["transaction"]:
+                            if i["signature"] == data["transaction"][0]["signature"]:
+                                control = False
+                        if control:
+                            node.candidate_block["transaction"].append(data["transaction"][0])
+
                 else:
                     node.candidate_block = data
 
     def get_candidate_block_hash(self, data, node: client, hash_of_data=""):
         self.logger.info(f"Getting candidate block hash with {hash_of_data}")
         if node.candidate_block_hash is None:
             node.candidate_block_hash = data
@@ -483,211 +576,224 @@
             if len(node.candidate_block_hash_history) >= 5:
                 node.candidate_block_hash_history.pop(0)
 
             node.candidate_block_hash_history.append(
                 copy.copy(node.candidate_block_hash))
             node.candidate_block_hash = data
         else:
-            if len(node.candidate_block_hash["hash"]) <= len(data["hash"]):
-                node.candidate_block_hash = data
+            #if len(node.candidate_block_hash["hash"]) <= len(data["hash"]):
+            node.candidate_block_hash = data
 
     def send_full_chain(self, node=None):
         log_text = ("Sending full chain" if node is None else
                     f"Sending full chain to {node.id}:{node.host}:{node.port}")
         self.logger.info(log_text)
         file = open(self.TEMP_BLOCK_PATH, "rb")
         SendData = file.read(1024)
         while SendData:
             data = {
                 "action": "fullblock",
                 "byte": (SendData.decode(encoding="iso-8859-1")),
             }
             if node is None:
-                self.send(data)
+                self.send(data, c_type=2)
             else:
-                self.send_client(node, data)
+                self.send_client(node, data, c_type=2)
 
             SendData = file.read(1024)
 
             if not SendData:
                 data = {
                     "action": "fullblock",
                     "byte": "end",
                 }
                 if node is None:
-                    self.send(data)
+                    self.send(data, c_type=2)
                 else:
-                    self.send_client(node, data)
+                    self.send_client(node, data, c_type=2)
 
     def send_full_accounts(self, node=None):
         the_TEMP_ACCOUNTS_PATH = self.TEMP_ACCOUNTS_PATH
         file = open(the_TEMP_ACCOUNTS_PATH, "rb")
         SendData = file.read(1024)
         while SendData:
             data = {
                 "action": "fullaccounts",
                 "byte": (SendData.decode(encoding="iso-8859-1")),
             }
 
             if node is None:
-                self.send(data)
+                self.send(data, c_type=2)
             else:
-                self.send_client(node, data)
+                self.send_client(node, data, c_type=2)
 
             SendData = file.read(1024)
             if not SendData:
                 data = {"action": "fullaccounts", "byte": "end"}
                 if node is None:
-                    self.send(data)
+                    self.send(data, c_type=2)
                 else:
-                    self.send_client(node, data)
+                    self.send_client(node, data, c_type=2)
 
     def send_full_blockshash(self, node=None):
         the_TEMP_BLOCKSHASH_PATH = self.TEMP_BLOCKSHASH_PATH
         file = open(the_TEMP_BLOCKSHASH_PATH, "rb")
         SendData = file.read(1024)
         while SendData:
             data = {
                 "action": "fullblockshash",
                 "byte": (SendData.decode(encoding="iso-8859-1")),
             }
             if node is None:
-                self.send(data)
+                self.send(data, c_type=2)
             else:
-                self.send_client(node, data)
+                self.send_client(node, data, c_type=2)
 
             SendData = file.read(1024)
 
             if not SendData:
                 data = {"action": "fullblockshash", "byte": "end"}
                 if node is None:
-                    self.send(data)
+                    self.send(data, c_type=2)
                 else:
-                    self.send_client(node, data)
+                    self.send_client(node, data, c_type=2)
 
     def send_full_blockshash_part(self, node=None):
         the_TEMP_BLOCKSHASH_PART_PATH = self.TEMP_BLOCKSHASH_PART_PATH
         file = open(the_TEMP_BLOCKSHASH_PART_PATH, "rb")
         SendData = file.read(1024)
         while SendData:
             data = {
                 "action": "fullblockshash_part",
                 "byte": (SendData.decode(encoding="iso-8859-1")),
             }
             if node is None:
-                self.send(data)
+                self.send(data, c_type=2)
             else:
-                self.send_client(node, data)
+                self.send_client(node, data, c_type=2)
 
             SendData = file.read(1024)
 
             if not SendData:
                 data = {"action": "fullblockshash_part", "byte": "end"}
                 if node is None:
-                    self.send(data)
+                    self.send(data, c_type=2)
                 else:
-                    self.send_client(node, data)
+                    self.send_client(node, data, c_type=2)
 
     def get_full_chain(self, data, node, hash_of_data=""):
         self.logger.info(f"Getting full chain with {hash_of_data}")
         get_ok = False
 
         if not os.path.exists(self.TEMP_BLOCK_PATH):
             get_ok = True
         else:
-            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH)
+            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH, reset=self.custom_variables)
             if node.id == system.dowload_true_block:
                 get_ok = True
 
         if get_ok:
             if str(data["byte"]) == "end":
                 move(self.LOADING_BLOCK_PATH, self.TEMP_BLOCK_PATH)
 
                 from naruno.consensus.consensus_main import consensus_trigger
                 from naruno.lib.perpetualtimer import perpetualTimer
 
                 system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH,
-                                  get_normal_block=True)
+                                  get_normal_block=True, reset=self.custom_variables)
 
                 ChangeTransactionFee(system)
 
-                perpetualTimer(system.consensus_timer, consensus_trigger)
+                perpetualTimer(system.consensus_timer, consensus_trigger, the_consensus=True)
                 SaveBlock(
                     system,
                     custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH,
                     custom_TEMP_ACCOUNTS_PATH=self.TEMP_ACCOUNTS_PATH,
                     custom_TEMP_BLOCKSHASH_PATH=self.TEMP_BLOCKSHASH_PATH,
                     custom_TEMP_BLOCKSHASH_PART_PATH=self.
                     TEMP_BLOCKSHASH_PART_PATH,
                 )
 
             else:
+                os.chdir(get_config()["main_folder"])
                 file = open(self.LOADING_BLOCK_PATH, "ab")
 
                 file.write((data["byte"].encode(encoding="iso-8859-1")))
                 file.close()
 
     def get_full_blockshash(self, data, node, hash_of_data=""):
         self.logger.info(f"Getting full blockshash with {hash_of_data}")
         the_TEMP_BLOCKSHASH_PATH = self.TEMP_BLOCKSHASH_PATH
         get_ok = False
 
         if not os.path.exists(the_TEMP_BLOCKSHASH_PATH):
             get_ok = True
         else:
-            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH)
+            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH, reset=self.custom_variables)
             if node.id == system.dowload_true_block:
                 get_ok = True
 
         if get_ok:
             if str(data["byte"]) == "end":
+                blockshash_db.set("blockshash", None)
+                with contextlib.suppress(FileNotFoundError):
+                    os.remove(the_TEMP_BLOCKSHASH_PATH)
                 move(self.LOADING_BLOCKSHASH_PATH, the_TEMP_BLOCKSHASH_PATH)
             else:
+                os.chdir(get_config()["main_folder"])
                 file = open(self.LOADING_BLOCKSHASH_PATH, "ab")
                 file.write((data["byte"].encode(encoding="iso-8859-1")))
                 file.close()
 
     def get_full_blockshash_part(self, data, node, hash_of_data=""):
         self.logger.info(f"Getting full blockshash part with {hash_of_data}")
         the_TEMP_BLOCKSHASH_PART_PATH = self.TEMP_BLOCKSHASH_PART_PATH
         get_ok = False
 
         if not os.path.exists(the_TEMP_BLOCKSHASH_PART_PATH):
             get_ok = True
         else:
-            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH)
+            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH, reset=self.custom_variables)
             if node.id == system.dowload_true_block:
                 get_ok = True
 
         if get_ok:
             if str(data["byte"]) == "end":
+                blockshash_db.set("blockshash_part", None)
+                with contextlib.suppress(FileNotFoundError):
+                    os.remove(the_TEMP_BLOCKSHASH_PART_PATH)
                 move(self.LOADING_BLOCKSHASH_PART_PATH,
                      the_TEMP_BLOCKSHASH_PART_PATH)
             else:
+                os.chdir(get_config()["main_folder"])
                 file = open(self.LOADING_BLOCKSHASH_PART_PATH, "ab")
                 file.write((data["byte"].encode(encoding="iso-8859-1")))
                 file.close()
 
     def get_full_accounts(self, data, node, hash_of_data=""):
         self.logger.info(f"Getting full accounts with {hash_of_data}")
         the_TEMP_ACCOUNTS_PATH = self.TEMP_ACCOUNTS_PATH
         the_LOADING_ACCOUNTS_PATH = self.LOADING_ACCOUNTS_PATH
         get_ok = False
 
         if not os.path.exists(the_TEMP_ACCOUNTS_PATH):
             get_ok = True
         else:
-            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH)
+            system = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH, reset=self.custom_variables)
             if node.id == system.dowload_true_block:
                 get_ok = True
 
         if get_ok:
             if str(data["byte"]) == "end":
+                accounts_db.set("accounts", None)
+                with contextlib.suppress(FileNotFoundError):
+                    os.remove(the_TEMP_ACCOUNTS_PATH)
                 move(the_LOADING_ACCOUNTS_PATH, the_TEMP_ACCOUNTS_PATH)
             else:
+                os.chdir(get_config()["main_folder"])
                 file = open(the_LOADING_ACCOUNTS_PATH, "ab")
                 file.write((data["byte"].encode(encoding="iso-8859-1")))
                 file.close()
 
     @staticmethod
     def send_transaction(
         tx,
@@ -712,72 +818,73 @@
                 "transaction_fee": tx.transaction_fee,
                 "transaction_time": tx.transaction_time,
                 "custom_current_time": custom_current_time,
                 "custom_sequence_number": custom_sequence_number,
                 "custom_balance": custom_balance,
             }
             the_server = server.Server if custom_server is None else custom_server
-            the_server.send(data, except_client=except_client)
+            the_server.send(data, except_client=except_client, c_type=1)
 
     def get_transaction(self, data, node, hash_of_data=""):
         self.logger.info(f"Getting transaction with {hash_of_data}")
-        block = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH)
+        if self not in naruno.node.server.server.tx_signature_list:
+            naruno.node.server.server.tx_signature_list[self] = []
+
+        if data["txsignature"] in naruno.node.server.server.tx_signature_list[self]:
+            self.logger.debug("Transaction is already getted")
+            return
+
+        naruno.node.server.server.tx_signature_list[self].append(data["txsignature"])
+        
         the_transaction = Transaction(
             data["sequence_number"],
             data["txsignature"],
             data["fromUser"],
             data["to_user"],
             data["data"],
             data["amount"],
             data["transaction_fee"],
             data["transaction_time"],
         )
+        block = GetBlock(custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH, reset=self.custom_variables)
         custom_current_time = None
         custom_sequence_number = None
         custom_balance = None
         if self.custom_variables:
             custom_current_time = data["custom_current_time"]
             custom_sequence_number = data["custom_sequence_number"]
             custom_balance = data["custom_balance"]
 
-        if GetTransaction(
+        GetTransaction(
                 block,
                 the_transaction,
                 custom_current_time=custom_current_time,
                 custom_sequence_number=custom_sequence_number,
                 custom_balance=custom_balance,
                 custom_PENDING_TRANSACTIONS_PATH=self.
                 PENDING_TRANSACTIONS_PATH,
-        ):
-            server.send_transaction(the_transaction,
-                                    except_client=node,
-                                    custom_server=self)
-            SaveBlock(
-                block,
-                custom_TEMP_BLOCK_PATH=self.TEMP_BLOCK_PATH,
-                custom_TEMP_ACCOUNTS_PATH=self.TEMP_ACCOUNTS_PATH,
-                custom_TEMP_BLOCKSHASH_PATH=self.TEMP_BLOCKSHASH_PATH,
-                custom_TEMP_BLOCKSHASH_PART_PATH=self.
-                TEMP_BLOCKSHASH_PART_PATH,
-            )
-
+                except_client=node,
+                custom_server=self)
+        
     def send_block_to_other_nodes(self,
                                   node=None,
                                   sync=False,
                                   hash_of_data=""):
         """
         Sends the block to the other nodes.
         """
         self.logger.info(f"Sending block to other nodes with {hash_of_data}")
         if node is None or sync:
+            self.logger.info("Sync process started")
             self.send_full_accounts(node=node)
             self.send_full_blockshash(node=node)
             self.send_full_blockshash_part(node=node)
             self.send_full_chain(node=node)
         else:
+            self.logger.info("Node appended to sync_clients")
             self.sync_clients.append(node)
 
     def get_ip(self):
         """
         Returns the IP address of the socket in this class.
         """
         ip = self.sock.getsockname()[0]
```

### Comparing `naruno-0.59.0/naruno/node/unl.py` & `naruno-0.60.0/naruno/node/unl.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import itertools
 import json
 import os
 import time
 
 from naruno.config import UNL_NODES_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
+
+unl_db = KOT("unl", folder=get_config()["main_folder"] + "/db")
 
 
 class Unl:
 
     @staticmethod
     def save_new_unl_node(node_id):
         """
@@ -24,43 +27,40 @@
         nodes_list = Unl.get_unl_nodes()
 
         already_in_list = any(element == node_id for element in nodes_list)
         if not already_in_list:
             nodes_list[node_id] = {}
             nodes_list[node_id]["date"] = time.time()
 
-            os.chdir(get_config()["main_folder"])
-            with open(UNL_NODES_PATH, "w") as unl_nodes_file:
-                json.dump(nodes_list, unl_nodes_file, indent=4)
+            unl_db.set("unl", nodes_list)
 
     @staticmethod
     def get_unl_nodes(custom_UNL_NODES_PATH=None):
         """
         Returns the UNL nodes list from UNL_NODES_PATH.
         """
 
-        the_UNL_NODES_PATH = (UNL_NODES_PATH if custom_UNL_NODES_PATH is None
-                              else custom_UNL_NODES_PATH)
-
-        if not os.path.exists(the_UNL_NODES_PATH):
-            return {}
-
-        os.chdir(get_config()["main_folder"])
-        with open(the_UNL_NODES_PATH, "r") as unl_nodes_file:
-            return json.load(unl_nodes_file)
+        record = (unl_db.get("unl") if custom_UNL_NODES_PATH is None else KOT(
+            "unl" + custom_UNL_NODES_PATH,
+            folder=get_config()["main_folder"] + "/db",
+        ).get("unl"))
+        return record if record is not None else {}
 
     @staticmethod
-    def get_as_node_type(id_list):
+    def get_as_node_type(id_list, c_type=0):
         """
         Converts the UNL node list to Node class.
         """
 
         from naruno.node.server.server import server
-
-        nodes = [] if server.Server is None else server.Server.clients
+        nodes = []
+        if server.Server is not None:
+         for i in server.Server.clients:
+            if i.c_type == c_type:
+                nodes.append(i)
         return nodes
 
     @staticmethod
     def node_is_unl(node_id):
         """
         Returns the this node is unl or not.
         """
@@ -77,10 +77,8 @@
         Deletes the UNL node
         """
 
         saved_nodes = Unl.get_unl_nodes()
         if node_id in saved_nodes:
             del saved_nodes[node_id]
 
-            os.chdir(get_config()["main_folder"])
-            with open(UNL_NODES_PATH, "w") as connected_node_file:
-                json.dump(saved_nodes, connected_node_file, indent=4)
+            unl_db.set("unl", saved_nodes)
```

### Comparing `naruno-0.59.0/naruno/transactions/check/check_transaction.py` & `naruno-0.60.0/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/check/datas/check_datas.py` & `naruno-0.60.0/naruno/transactions/check/datas/check_datas.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,45 +19,52 @@
     transaction,
     custom_current_time=None,
     custom_balance=None,
     custom_sequence_number=None,
     custom_PENDING_TRANSACTIONS_PATH=None,
     custom_account_list=None,
     disable_already_in=False,
+    disable_already_in_2=False,
 ):
     """
     Check if the transaction datas are valid
     """
 
     if not disable_already_in:
-        pending_transactions = GetPending(
-            custom_PENDING_TRANSACTIONS_PATH=custom_PENDING_TRANSACTIONS_PATH)
+        pending_transactions = GetPending(custom_PENDING_TRANSACTIONS_PATH=custom_PENDING_TRANSACTIONS_PATH)
+
+    if not disable_already_in and not disable_already_in_2:
+        
         for already_tx in pending_transactions + block.validating_list:
-            if already_tx.signature == transaction.signature:
+            if already_tx.signature == transaction.signature :
                 logger.error("Transaction is already in the pending list")
                 return False
 
         for tx in pending_transactions + block.validating_list:
             if (tx.fromUser == transaction.fromUser) and block.just_one_tx:
                 if tx.signature != transaction.signature:
                     if transaction.transaction_time < tx.transaction_time:
                         pass
                     elif transaction.transaction_time == tx.transaction_time:
                         if transaction.sequence_number < tx.sequence_number:
                             pass
                         else:
+
+                                logger.info("Multiple transaction in one account")
+                                return False
+                    else:
+
                             logger.info("Multiple transaction in one account")
                             return False
-                    else:
-                        logger.info("Multiple transaction in one account")
-                        return False
     if not disable_already_in:
         balance = (GetBalance(
             transaction.fromUser,
             block=block,
+            tx_signature=transaction.signature,
+            custom_pending=pending_transactions
         ) if custom_balance is None else custom_balance)
         if balance >= (float(transaction.amount) +
                     float(transaction.transaction_fee)):
             pass
         else:
             logger.error("Balance is not valid")
             return False
@@ -66,41 +73,42 @@
             pass
         else:
             if (GetBalance(
                     transaction.toUser,
                     account_list=custom_account_list,
                     dont_convert=True,
                     block=block,
+                    custom_pending=pending_transactions,
             ) >= 0):
                 pass
             else:
                 logger.error("Minimum transfer amount is not reached")
                 return False
 
     if transaction.transaction_fee >= block.transaction_fee:
         pass
     else:
         logger.error(
             f"Transaction fee is not reached {transaction.transaction_fee}-{block.transaction_fee}"
         )
         return False
 
-    if not disable_already_in:
+    if not disable_already_in and not disable_already_in_2:
         get_sequence_number = (GetSequanceNumber(transaction.fromUser, block=block)
                             if custom_sequence_number is None else
                             custom_sequence_number)
         if transaction.sequence_number == (get_sequence_number + 1):
             pass
         else:
             logger.error("Sequance number is not valid")
             return False
 
-    current_time = (int(time.time())
-                    if custom_current_time is None else custom_current_time)
-    if (current_time -
-            transaction.transaction_time) <= block.transaction_delay_time:
-        pass
-    else:
-        logger.error("Transaction time is not valid")
-        return False
+        current_time = (int(time.time())
+                        if custom_current_time is None else custom_current_time)
+        if (current_time -
+                transaction.transaction_time) <= block.transaction_delay_time:
+            pass
+        else:
+            logger.error("Transaction time is not valid")
+            return False
 
     return True
```

### Comparing `naruno-0.59.0/naruno/transactions/check/len/check_len.py` & `naruno-0.60.0/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/check/sign/check_sign.py` & `naruno-0.60.0/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/check/type/check_type.py` & `naruno-0.60.0/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/cleaner.py` & `naruno-0.60.0/naruno/transactions/cleaner.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 def Cleaner(
     block: Block,
     pending_list_txs: list,
     custom_current_time=None,
     custom_sequence_number=None,
     custom_balance=None,
+    disable_already_in=True,
+    disable_already_in_2=True,
 ):
     system_txs = []
 
     for transaction in block.validating_list:
         if transaction.signature == "NARUNO":
             block.validating_list.remove(transaction)
             system_txs.append(transaction)
@@ -33,30 +35,31 @@
             the_sequance_number = transaction.sequence_number - 1
         if not Check_Datas(
                 block,
                 transaction,
                 custom_current_time=custom_current_time,
                 custom_balance=custom_balance,
                 custom_sequence_number=the_sequance_number,
-                disable_already_in=True,
+                disable_already_in=disable_already_in,
+                disable_already_in_2=disable_already_in_2,
         ):
             DeletePending(transaction)
             pending_list_txs.remove(transaction)
 
     for transaction in block.validating_list:
         the_sequance_number = None
         if custom_sequence_number == -1:
             the_sequance_number = transaction.sequence_number - 1
         if not Check_Datas(
                 block,
                 transaction,
                 custom_current_time=custom_current_time,
                 custom_balance=custom_balance,
                 custom_sequence_number=the_sequance_number,
-                disable_already_in=True,
+                disable_already_in=disable_already_in,
         ):
             block.validating_list.remove(transaction)
 
     def clean(list_of_transactions: list) -> list:
         list_of_transactions = list(dict.fromkeys(list_of_transactions))
 
         list_of_transactions = sorted(list_of_transactions,
@@ -114,8 +117,8 @@
     for transaction in difference:
         DeletePending(transaction)
     pending_list_txs = cleaned_pending_list_txs
 
     for transaction in system_txs:
         block.validating_list.append(transaction)
 
-    return (cleaned_validating_list, cleaned_pending_list_txs)
+    return (cleaned_validating_list, cleaned_pending_list_txs)
```

### Comparing `naruno-0.59.0/naruno/transactions/get_transaction.py` & `naruno-0.60.0/naruno/transactions/get_transaction.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import threading
+import traceback
+
 from naruno.transactions.check.check_transaction import \
     CheckTransaction
 from naruno.transactions.pending.save_pending import SavePending
 
 
+
 def GetTransaction(
     block,
     the_transaction,
     custom_current_time=None,
     custom_sequence_number=None,
     custom_balance=None,
     custom_PENDING_TRANSACTIONS_PATH=None,
     custom_account_list=None,
+    except_client=None,
+    custom_server=None,
 ):
     if CheckTransaction(
             block,
             the_transaction,
             custom_current_time,
             custom_sequence_number,
             custom_balance,
```

### Comparing `naruno-0.59.0/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.60.0/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.60.0/naruno/transactions/my_transactions/get_proof.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import os
 from hashlib import sha256
 from zipfile import ZipFile
 
 from naruno.blockchain.block.get_block_from_blockchain_db import \
     GetBlockstoBlockchainDB
+from naruno.blockchain.block.save_block import block_db
 from naruno.config import BLOCKS_PATH
 from naruno.config import PROOF_PATH
 from naruno.lib.config_system import get_config
 
 
 def GetProof(
     signature: str,
@@ -29,16 +30,19 @@
     the_BLOCKS_PATH = BLOCKS_PATH if custom_BLOCKS_PATH is None else custom_BLOCKS_PATH
 
     os.chdir(get_config()["main_folder"])
     sequence_number = None
 
     for file in os.listdir(the_BLOCKS_PATH):
         if file.endswith(".block.json"):
-            with open(the_BLOCKS_PATH + file, "r") as block_file:
-                the_block_json = json.load(block_file)
+            path_of_first = os.path.join(get_config()["main_folder"],
+                                         the_BLOCKS_PATH + file)
+            the_block_json = block_db.get(
+                the_BLOCKS_PATH + file,
+                custom_key_location=path_of_first)
             for transaction in the_block_json["validating_list"]:
                 if transaction["signature"] == signature:
                     sequence_number = file.split(".")[0]
 
     if sequence_number is None:
         return None
```

### Comparing `naruno-0.59.0/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.60.0/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         custom_currently_list: The list for custom situations.
     Returns:
         The list of the my transactions.
     """
 
     currently_list = (GetMyTransaction() if custom_currently_list is None else
                       custom_currently_list)
+    save_list = []
     if not tx.signature == "NARUNO":
         new = True
 
         for tx_list in currently_list:
             if tx_list[0].signature == tx.signature:
                 new = False
 
@@ -48,17 +49,19 @@
                              f"{tx.data}:{tx.amount} to {tx.toUser}")
             elif sended and validated:
                 notification("Validated TX",
                              f"{tx.data}:{tx.amount} to {tx.toUser}")
 
             tx_list = [tx, validated, sended]
             currently_list.append(tx_list)
+            save_list.append(tx_list)
 
         else:
             for tx_list in currently_list:
                 if tx_list[0].signature == tx.signature:
                     tx_list[1] = validated
                     tx_list[2] = sended
+                    save_list.append(tx_list)
 
-    SaveMyTransaction(currently_list)
+    SaveMyTransaction(save_list)
 
     return currently_list
```

### Comparing `naruno-0.59.0/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.60.0/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         tx: The transaction that is going to be validated.
     Returns:
         The list of the my transactions.
     """
 
     custom_currently_list = (GetMyTransaction() if custom_currently_list
                              is None else custom_currently_list)
+    save_list = []
     for i in custom_currently_list:
         if i[0].signature == tx.signature:
             if not i[2]:
                 notification("Sended TX",
                              f"{tx.data}:{tx.amount} to {tx.toUser}")
             i[2] = True
-    SaveMyTransaction(custom_currently_list)
+            save_list.append(i)
+    SaveMyTransaction(save_list)
     return custom_currently_list
```

### Comparing `naruno-0.59.0/naruno/transactions/pending/delete_pending.py` & `naruno-0.60.0/naruno/transactions/pending/save_pending.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
+import json
 import os
 from hashlib import sha256
 
 from naruno.config import PENDING_TRANSACTIONS_PATH
 from naruno.lib.config_system import get_config
+from naruno.lib.kot import KOT
 
+pendingtransactions_db = KOT("pendingtransactions",
+                             folder=get_config()["main_folder"] + "/db")
 
-def DeletePending(tx, custom_PENDING_TRANSACTIONS_PATH=None):
-    the_PENDING_TRANSACTIONS_PATH = (PENDING_TRANSACTIONS_PATH if
-                                     custom_PENDING_TRANSACTIONS_PATH is None
-                                     else custom_PENDING_TRANSACTIONS_PATH)
-    os.chdir(get_config()["main_folder"])
+
+def SavePending(tx, custom_PENDING_TRANSACTIONS_PATH=None):
+    if custom_PENDING_TRANSACTIONS_PATH == PENDING_TRANSACTIONS_PATH:
+        custom_PENDING_TRANSACTIONS_PATH = None    
     file_name = sha256((tx.signature).encode("utf-8")).hexdigest()
-    for entry in os.scandir(the_PENDING_TRANSACTIONS_PATH):
-        if entry.name == f"{file_name}.json":
-            os.remove(entry.path)
+
+    pendingtransactions_db.set(file_name, tx.dump_json()) if custom_PENDING_TRANSACTIONS_PATH is None else KOT("pendingtransactions"+custom_PENDING_TRANSACTIONS_PATH, folder=get_config()["main_folder"] + "/db").set(file_name, tx.dump_json())
```

### Comparing `naruno-0.59.0/naruno/transactions/pending/get_pending.py` & `naruno-0.60.0/naruno/transactions/pending/get_pending.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,35 +5,27 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import json
 import os
 
 from naruno.config import PENDING_TRANSACTIONS_PATH
 from naruno.lib.config_system import get_config
+
 from naruno.transactions.transaction import Transaction
 
+from naruno.transactions.pending.save_pending import pendingtransactions_db
+from naruno.lib.kot import KOT
 
 def GetPending(custom_PENDING_TRANSACTIONS_PATH=None):
-    the_PENDING_TRANSACTIONS_PATH = (PENDING_TRANSACTIONS_PATH if
-                                     custom_PENDING_TRANSACTIONS_PATH is None
-                                     else custom_PENDING_TRANSACTIONS_PATH)
+    if custom_PENDING_TRANSACTIONS_PATH == PENDING_TRANSACTIONS_PATH:
+        custom_PENDING_TRANSACTIONS_PATH = None
     the_pending_list = []
-    os.chdir(get_config()["main_folder"])
-    for entry in os.scandir(the_PENDING_TRANSACTIONS_PATH):
-        if entry.name != "README.md":
-            with open(entry.path, "r") as my_transaction_file:
-                the_pending_list.append(
-                    Transaction.load_json(json.load(my_transaction_file)))
+    all_records = pendingtransactions_db.get_all() if custom_PENDING_TRANSACTIONS_PATH is None else KOT("pendingtransactions"+custom_PENDING_TRANSACTIONS_PATH, folder=get_config()["main_folder"] + "/db").get_all()
+    for entry in all_records:
+        the_pending_list.append(Transaction.load_json(all_records[entry]))
     return sorted(the_pending_list, key=lambda x: x.signature)
 
 
 def GetPendingLen(custom_PENDING_TRANSACTIONS_PATH=None):
-    the_PENDING_TRANSACTIONS_PATH = (PENDING_TRANSACTIONS_PATH if
-                                     custom_PENDING_TRANSACTIONS_PATH is None
-                                     else custom_PENDING_TRANSACTIONS_PATH)
-    the_pending_list = []
-    os.chdir(get_config()["main_folder"])
-    for entry in os.scandir(the_PENDING_TRANSACTIONS_PATH):
-        if entry.name != "README.md":
-            the_pending_list.append(1)
 
-    return len(the_pending_list)
+
+    return pendingtransactions_db.get_count() if custom_PENDING_TRANSACTIONS_PATH is None else KOT("pendingtransactions"+custom_PENDING_TRANSACTIONS_PATH, folder=get_config()["main_folder"] + "/db").get_count()
```

### Comparing `naruno-0.59.0/naruno/transactions/pending/save_pending.py` & `naruno-0.60.0/naruno/transactions/pending/delete_pending.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
-import json
 import os
 from hashlib import sha256
 
 from naruno.config import PENDING_TRANSACTIONS_PATH
 from naruno.lib.config_system import get_config
+from naruno.transactions.pending.save_pending import pendingtransactions_db
+from naruno.lib.kot import KOT
 
-
-def SavePending(tx, custom_PENDING_TRANSACTIONS_PATH=None):
-    the_PENDING_TRANSACTIONS_PATH = (PENDING_TRANSACTIONS_PATH if
-                                     custom_PENDING_TRANSACTIONS_PATH is None
-                                     else custom_PENDING_TRANSACTIONS_PATH)
+def DeletePending(tx, custom_PENDING_TRANSACTIONS_PATH=None):
+    if custom_PENDING_TRANSACTIONS_PATH == PENDING_TRANSACTIONS_PATH:
+        custom_PENDING_TRANSACTIONS_PATH = None    
     file_name = sha256((tx.signature).encode("utf-8")).hexdigest()
-    the_path = the_PENDING_TRANSACTIONS_PATH + f"{file_name}.json"
-    os.chdir(get_config()["main_folder"])
-    with open(the_path, "w") as my_transaction_file:
-        json.dump(tx.dump_json(), my_transaction_file)
+    pendingtransactions_db.delete(file_name)  if custom_PENDING_TRANSACTIONS_PATH is None else KOT("pendingtransactions"+custom_PENDING_TRANSACTIONS_PATH, folder=get_config()["main_folder"] + "/db").delete(file_name)
```

### Comparing `naruno-0.59.0/naruno/transactions/pending_to_validating.py` & `naruno-0.60.0/naruno/transactions/pending_to_validating.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,81 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import contextlib
+import copy
+import threading
+
 
 from naruno.blockchain.block.block_main import Block
 from naruno.lib.log import get_logger
 from naruno.node.server.server import server
 from naruno.transactions.pending.delete_pending import DeletePending
 from naruno.transactions.pending.get_pending import GetPending
+from naruno.transactions.pending.save_pending import SavePending
 
 logger = get_logger("TRANSACTIONS")
 
 
+
+
 def PendingtoValidating(block: Block):
     """
     Adds transactions to the verification list
     if there are suitable conditions.
     """
     logger.info("Pending to validating transfer process is started")
     first_validating_list_len = len(block.validating_list)
     first_max_tx_number = block.max_tx_number
     logger.debug(f"Currently tx amount: {first_validating_list_len}")
     logger.debug(f"Validating list capacity: {first_max_tx_number}")
 
     pending_list_txs = GetPending()
+    logger.debug(f"Pending list is got: {pending_list_txs}")
+
 
-    with contextlib.suppress(Exception):
-        [
-            server.send_transaction(i)
-            for i in pending_list_txs + block.validating_list
-        ]
 
+
+    first_situation = copy.copy(block.validating_list)
+    the_list_of_tx = pending_list_txs + first_situation
+    
+    block.validating_list = []
+
+    logger.debug(f"Pending list is sent to server")
     if len(block.validating_list) < block.max_tx_number:
-        for tx in OrderbyFee(pending_list_txs):
+        logger.debug("List is not full")
+        for tx in OrderbyFee(the_list_of_tx):
+            logger.debug(f"TX {tx.signature} is checking")
             if len(block.validating_list) < block.max_tx_number:
                 logger.info(f"tx {tx.signature} is moved to validating list")
 
                 block.validating_list.append(tx)
+                the_list_of_tx.remove(tx)
+                if not tx in first_situation:
+                    DeletePending(tx)
 
-                DeletePending(tx)
             else:
                 logger.info(
                     f"TX {tx.signature} is can not moved to validating list")
     else:
         logger.info("List is full")
+    
+    for i in the_list_of_tx:
+        if i in first_situation:
+            SavePending(i)
+        
+
+    
 
 
 def OrderbyFee(transactions: list):
     """
     Sorts transactions by fee.
     """
 
-    transactions.sort(key=lambda x: x.transaction_fee, reverse=True)
-    return transactions
+    the_transactions = copy.copy(transactions)
+    the_transactions.sort(key=lambda x: x.signature, reverse=True)
+    the_transactions.sort(key=lambda x: x.transaction_fee, reverse=True)
+    return the_transactions
```

### Comparing `naruno-0.59.0/naruno/transactions/print_transactions.py` & `naruno-0.60.0/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/process_the_transaction.py` & `naruno-0.60.0/naruno/transactions/process_the_transaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import sqlite3
-
+from decimal import Decimal
 from naruno.accounts.account import Account
 from naruno.accounts.save_accounts import SaveAccounts
 from naruno.blockchain.block.shares import shares
 from naruno.config import TEMP_ACCOUNTS_PATH
 from naruno.consensus.rounds.round_1.process.transactions.checks.duplicated import \
     Remove_Duplicates
 from naruno.lib.log import get_logger
@@ -34,17 +34,16 @@
     """
 
     logger.info("Transaction processing started.")
 
     if not dont_clean:
         block = Remove_Duplicates(block)
 
-    the_TEMP_ACCOUNTS_PATH = (TEMP_ACCOUNTS_PATH
-                              if custom_TEMP_ACCOUNTS_PATH is None else
-                              custom_TEMP_ACCOUNTS_PATH)
+    the_TEMP_ACCOUNTS_PATH = (TEMP_ACCOUNTS_PATH if custom_TEMP_ACCOUNTS_PATH
+                              is None else custom_TEMP_ACCOUNTS_PATH)
 
     edited_accounts = []
 
     clean_list = []
     for unclear in block.validating_list:
         if not "NARUNO" in unclear.signature:
             clean_list.append(unclear)
@@ -72,23 +71,28 @@
         logger.info(f"Transaction: {trans.__dict__}")
 
         touser_inlist = True
         to_user_in_new_list = False
 
         address_of_fromUser = Address(trans.fromUser)
         logger.debug(f"FromUser address: {address_of_fromUser}")
-        the_account_list.execute(
-            "SELECT * FROM account_list WHERE address = ?", (address_of_fromUser,)
-        )
-        first_list = the_account_list.fetchall()
-        the_account_list.execute(
-            "SELECT * FROM account_list WHERE address = ?", (trans.toUser,))
-        second_list = the_account_list.fetchall()
+        the_record_account_list = []
+
+        the_record_account_list.append([
+            address_of_fromUser,
+            the_account_list[address_of_fromUser][0],
+            the_account_list[address_of_fromUser][1],
+        ]) if address_of_fromUser in the_account_list else None
+        the_record_account_list.append([
+            trans.toUser,
+            the_account_list[trans.toUser][0],
+            the_account_list[trans.toUser][1],
+        ]) if trans.toUser in the_account_list else None
 
-        for the_pulled_account in first_list + second_list:
+        for the_pulled_account in the_record_account_list:
             account_list.append(
                 Account(the_pulled_account[0], the_pulled_account[2],
                         the_pulled_account[1]))
 
         for Accounts in account_list:
             touser_inlist = False
 
@@ -113,37 +117,41 @@
                 i.balance += float(trans.amount)
                 to_user_in_new_list = True
 
         # If not included in the account_list, add.
         if not touser_inlist and not to_user_in_new_list:
             new_added_accounts_list.append(
                 Account(trans.toUser, float(trans.amount)))
-
+    logger.info(f"Actions: {actions}")
     for action in actions:
         for account in account_list:
             if action[0] == account.Address:
+                alread_in = True if account in edited_accounts else False
+                the_account = edited_accounts[edited_accounts.index(account)] if account in edited_accounts else account                
+                if the_account.Address == block.fee_address:
+                    logger.info(f"Fee Address Input: {the_account.dump_json()}")
                 if action[1] == "balance":
-                    account.balance += action[2]
+                    balance_decimal = Decimal(str(the_account.balance)) + Decimal(str(action[2]))
+                    the_account.balance = float(balance_decimal)
                 elif action[1] == "sequence_number":
-                    account.sequence_number += action[2]
-                edited_accounts.append(account)
+                    the_account.sequence_number += action[2]
+
+                if the_account.Address == block.fee_address:
+                    logger.info(f"Fee Address Output: {the_account.dump_json()}")
+                if not alread_in:
+                    edited_accounts.append(the_account)
 
     # Syncs new sorted list to block.validating_list
 
     block.validating_list = sorted(temp_validating_list,
                                    key=lambda x: x.signature)
 
     new_added_accounts_list = sorted(new_added_accounts_list,
                                      key=lambda x: x.Address)
 
-    conn = sqlite3.connect(the_TEMP_ACCOUNTS_PATH)
-    c = conn.cursor()
-    for changed_account in edited_accounts:
-        c.execute(
-            "UPDATE account_list SET balance = ?, sequence_number = ? WHERE address = ?"
-        ,(changed_account.balance,changed_account.sequence_number,changed_account.Address))
-        conn.commit()
-    conn.close()
 
-    SaveAccounts(new_added_accounts_list, the_TEMP_ACCOUNTS_PATH)
+    logger.debug(f"SaveAccounts list: {new_added_accounts_list + edited_accounts}")
+    logger.debug(f"SaveAccounts path: {the_TEMP_ACCOUNTS_PATH}")
+    the_account_list_result = SaveAccounts(new_added_accounts_list + edited_accounts,
+                 the_TEMP_ACCOUNTS_PATH, sequence=block.sequence_number+block.empty_block_number)
 
-    return block
+    return [block, the_account_list_result]
```

### Comparing `naruno-0.59.0/naruno/transactions/send.py` & `naruno-0.60.0/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/transactions/transaction.py` & `naruno-0.60.0/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/delete_current_wallet.py` & `naruno-0.60.0/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/math.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.60.0/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/get_saved_wallet.py` & `naruno-0.60.0/naruno/wallet/get_saved_wallet.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import json
 import os
 
 from naruno.config import WALLETS_PATH
 from naruno.lib.config_system import get_config
-
+from naruno.lib.kot import KOT
+wallet_db = KOT("wallet",
+                        folder=get_config()["main_folder"] + "/db")
 
 def get_saved_wallet():
-    os.chdir(get_config()["main_folder"])
+    record = wallet_db.get("wallet")
 
-    if not os.path.exists(WALLETS_PATH):
-        return {}
 
-    with open(WALLETS_PATH, "r") as wallet_list_file:
-        return json.load(wallet_list_file)
+    return record if record is not None else {}
```

### Comparing `naruno-0.59.0/naruno/wallet/print_wallets.py` & `naruno-0.60.0/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/save_wallet_list.py` & `naruno-0.60.0/naruno/wallet/save_wallet_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 import json
 import os
 from hashlib import sha256
 
 from naruno.config import WALLETS_PATH
 from naruno.lib.config_system import get_config
 from naruno.wallet.get_saved_wallet import get_saved_wallet
-
+from naruno.lib.kot import KOT
+wallet_db = KOT("wallet",
+                        folder=get_config()["main_folder"] + "/db")
 
 def save_to_wallet_list(publicKey, privateKey, password):
     wallet_list = get_saved_wallet()
 
     wallet_list[publicKey] = {}
 
     wallet_list[publicKey]["publickey"] = publicKey.replace("\n", "")
@@ -24,10 +26,8 @@
     wallet_list[publicKey]["password_sha256"] = sha256(
         password.encode("utf-8")).hexdigest()
 
     save_wallet_list(wallet_list)
 
 
 def save_wallet_list(wallet_list):
-    os.chdir(get_config()["main_folder"])
-    with open(WALLETS_PATH, "w") as wallet_list_file:
-        json.dump(wallet_list, wallet_list_file, indent=4)
+    wallet_db.set("wallet", wallet_list)
```

### Comparing `naruno-0.59.0/naruno/wallet/wallet_create.py` & `naruno-0.60.0/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/wallet_delete.py` & `naruno-0.60.0/naruno/wallet/wallet_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 import json
 import os
 
 from naruno.config import WALLETS_PATH
 from naruno.lib.config_system import get_config
 from naruno.lib.log import get_logger
 from naruno.wallet.get_saved_wallet import get_saved_wallet
+from naruno.wallet.save_wallet_list import save_wallet_list
 
 logger = get_logger("WALLET")
 
-
 def wallet_delete(account):
     saved_wallet = get_saved_wallet()
     if account in saved_wallet:
         del saved_wallet[account]
 
-        os.chdir(get_config()["main_folder"])
-        with open(WALLETS_PATH, "w") as wallet_list_file:
-            json.dump(saved_wallet, wallet_list_file, indent=4)
+        save_wallet_list(saved_wallet)
         logger.info(f"Wallet {account} deleted")
         return True
     else:
         logger.error(f"Wallet {account} not found")
         return False
```

### Comparing `naruno-0.59.0/naruno/wallet/wallet_import.py` & `naruno-0.60.0/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno/wallet/wallet_selector.py` & `naruno-0.60.0/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.59.0/naruno.egg-info/PKG-INFO` & `naruno-0.60.0/naruno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.59.0
+Version: 0.60.0
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.59.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.0 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.59.0/naruno.egg-info/SOURCES.txt` & `naruno-0.60.0/naruno.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENCE-naruno-gui_lib__.md
+LICENCE-naruno-lib-kot__.md
 LICENCE-naruno-lib-mix__.md
 LICENCE-naruno-wallet-elipticcurve__.md
 LICENSE-others__.md
 MANIFEST.in
 README.md
 setup.py
 naruno/__init__.py
@@ -135,14 +136,15 @@
 naruno/gui/lib/libs/kv/tabnavigation.kv
 naruno/gui/lib/libs/kv/wallet_screen.kv
 naruno/gui/lib/libs/kv/welcome_screen.kv
 naruno/lib/clean_up.py
 naruno/lib/config_system.py
 naruno/lib/encryption.py
 naruno/lib/export.py
+naruno/lib/kot.py
 naruno/lib/log.py
 naruno/lib/notification.py
 naruno/lib/perpetualtimer.py
 naruno/lib/qr.py
 naruno/lib/safety.py
 naruno/lib/settings_system.py
 naruno/lib/sign.py
```

### Comparing `naruno-0.59.0/setup.py` & `naruno-0.60.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.59.0",
+    version="0.60.0",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

