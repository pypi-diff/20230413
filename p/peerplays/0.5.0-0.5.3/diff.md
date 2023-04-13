# Comparing `tmp/peerplays-0.5.0.tar.gz` & `tmp/peerplays-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peerplays-0.5.0.tar", last modified: Wed Feb  8 19:29:46 2023, max compression
+gzip compressed data, was "peerplays-0.5.3.tar", last modified: Thu Apr 13 13:17:52 2023, max compression
```

## Comparing `peerplays-0.5.0.tar` & `peerplays-0.5.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.070923 peerplays-0.5.0/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1186 2023-01-19 17:12:23.000000 peerplays-0.5.0/LICENSE.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-01-19 17:12:23.000000 peerplays-0.5.0/MANIFEST.in
--rw-rw-r--   0 pi        (1000) pi        (1000)     1463 2023-02-08 19:29:46.070923 peerplays-0.5.0/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)     1628 2023-01-20 19:05:15.000000 peerplays-0.5.0/README.md
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.018924 peerplays-0.5.0/peerplays/
--rw-rw-r--   0 pi        (1000) pi        (1000)      483 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2264 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/account.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2189 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/amount.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1328 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/asset.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      536 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/bet.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1833 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/bettingmarket.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2537 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/bettingmarketgroup.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1132 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/block.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      863 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/blockchain.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      410 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/blockchainobject.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.038923 peerplays-0.5.0/peerplays/cli/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5651 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/account.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1013 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/asset.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4473 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/bookie.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1213 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/bos.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2593 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/cli.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      793 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/committee.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5321 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4080 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/info.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1607 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1153 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/message.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2443 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/proposal.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      877 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/rpc.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2364 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/ui.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6625 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/wallet.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      781 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/cli/witness.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      566 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/committee.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1803 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/event.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1606 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/eventgroup.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2484 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/exceptions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1179 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/genesisbalance.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1507 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/instance.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    26634 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/market.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1806 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/memo.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      595 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/message.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3142 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/notify.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    74662 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/peerplays.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5335 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/peerplays2.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    14479 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/price.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      937 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/proposal.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1550 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/rule.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6388 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/son.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1305 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/sport.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      710 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/storage.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1880 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/transactionbuilder.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1182 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/utils.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      820 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/wallet.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1149 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplays/witness.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.022924 peerplays-0.5.0/peerplays.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1463 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)     2245 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       53 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)      118 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       37 2023-02-08 19:29:45.000000 peerplays-0.5.0/peerplays.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.042923 peerplays-0.5.0/peerplaysapi/
--rw-rw-r--   0 pi        (1000) pi        (1000)       60 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysapi/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      868 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysapi/exceptions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2278 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysapi/node.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      162 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysapi/wallet.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    12677 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysapi/websocket.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.050923 peerplays-0.5.0/peerplaysbase/
--rw-rw-r--   0 pi        (1000) pi        (1000)      173 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3275 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/account.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      741 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/asset_permissions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2194 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/chains.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      112 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/memo.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    17525 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/objects.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      682 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/objecttypes.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2838 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/operationids.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    66532 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/operations.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      671 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/signedtransactions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1324 2023-01-19 17:12:23.000000 peerplays-0.5.0/peerplaysbase/types.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      269 2023-01-19 17:12:23.000000 peerplays-0.5.0/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)      351 2023-02-08 19:29:46.074922 peerplays-0.5.0/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1682 2023-02-06 11:44:02.000000 peerplays-0.5.0/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-02-08 19:29:46.070923 peerplays-0.5.0/tests/
--rw-rw-r--   0 pi        (1000) pi        (1000)     3071 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_account.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6877 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_amount.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1271 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_asset.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      821 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_base_objects.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6165 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_betting.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     9804 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_bookie.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1169 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_cachedlist.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      813 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_fee.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5109 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_hrp.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5344 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_market.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3321 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_market_place.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      422 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_message.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3059 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_nft.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3571 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_object_creation_parents.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     7375 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_peerplays.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3941 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_proposals.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1220 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_rbac_small.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    36545 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_transactions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3836 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_txbuffers.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-01-19 17:12:23.000000 peerplays-0.5.0/tests/test_witness.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.459962 peerplays-0.5.3/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1186 2023-01-19 17:12:23.000000 peerplays-0.5.3/LICENSE.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-01-19 17:12:23.000000 peerplays-0.5.3/MANIFEST.in
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1463 2023-04-13 13:17:52.459962 peerplays-0.5.3/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1628 2023-03-20 12:45:42.000000 peerplays-0.5.3/README.md
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.355963 peerplays-0.5.3/peerplays/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      483 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2264 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/account.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2189 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/amount.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1328 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/asset.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      536 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/bet.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1833 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/bettingmarket.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2537 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/bettingmarketgroup.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1132 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/block.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      863 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/blockchain.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      410 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/blockchainobject.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.387963 peerplays-0.5.3/peerplays/cli/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-04-13 13:12:37.000000 peerplays-0.5.3/peerplays/cli/account.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1013 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/asset.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4473 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/bookie.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1213 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/bos.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2593 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/cli.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      793 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/committee.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5321 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4080 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/info.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1607 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1153 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/message.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2443 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/proposal.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      877 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/rpc.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5957 2023-04-13 13:12:37.000000 peerplays-0.5.3/peerplays/cli/ui.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6625 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/wallet.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      781 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/cli/witness.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      566 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/committee.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1803 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/event.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1606 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/eventgroup.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2484 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/exceptions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1179 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/genesisbalance.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1507 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/instance.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    26634 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/market.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1806 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/memo.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      595 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/message.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3142 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/notify.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    74662 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/peerplays.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5335 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/peerplays2.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    14479 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/price.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      937 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/proposal.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1550 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/rule.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6388 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/son.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1305 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/sport.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      710 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/storage.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1880 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/transactionbuilder.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1182 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/utils.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      820 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/wallet.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1149 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplays/witness.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.363963 peerplays-0.5.3/peerplays.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1463 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2245 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       53 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)      118 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       37 2023-04-13 13:17:52.000000 peerplays-0.5.3/peerplays.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.395963 peerplays-0.5.3/peerplaysapi/
+-rw-rw-r--   0 pi        (1000) pi        (1000)       60 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysapi/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      868 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysapi/exceptions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2021 2023-04-13 01:45:17.000000 peerplays-0.5.3/peerplaysapi/node.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      162 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysapi/wallet.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    12677 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysapi/websocket.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.419963 peerplays-0.5.3/peerplaysbase/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      173 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3275 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/account.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      741 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/asset_permissions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      670 2023-04-10 17:37:44.000000 peerplays-0.5.3/peerplaysbase/chains.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      112 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/memo.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    17525 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/objects.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      682 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/objecttypes.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2838 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/operationids.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    66532 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/operations.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      671 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/signedtransactions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1324 2023-01-19 17:12:23.000000 peerplays-0.5.3/peerplaysbase/types.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      269 2023-01-19 17:12:23.000000 peerplays-0.5.3/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)      351 2023-04-13 13:17:52.459962 peerplays-0.5.3/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1682 2023-04-13 13:12:37.000000 peerplays-0.5.3/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-04-13 13:17:52.455962 peerplays-0.5.3/tests/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3071 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_account.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6877 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_amount.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1271 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_asset.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      821 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_base_objects.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6165 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_betting.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     9804 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_bookie.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1169 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_cachedlist.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      813 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_fee.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5109 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_hrp.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5344 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_market.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3321 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_market_place.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      422 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_message.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3059 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_nft.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3571 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_object_creation_parents.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     7375 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_peerplays.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3941 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_proposals.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1220 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_rbac_small.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    36545 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_transactions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3836 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_txbuffers.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-01-19 17:12:23.000000 peerplays-0.5.3/tests/test_witness.py
```

### Comparing `peerplays-0.5.0/LICENSE.txt` & `peerplays-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/PKG-INFO` & `peerplays-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peerplays
-Version: 0.5.0
+Version: 0.5.3
 Summary: Python library for PEERPLAYS
 Home-page: https://gitlab.com/PBSA/tools-libs/python-peerplays
 Author: PBSA and contributors. Original by Fabian Schuh.
 Author-email: info@pbsa.info
 Maintainer: PBSA
 Maintainer-email: info@pbsa.info
 Keywords: peerplays,library,api,rpc
```

### Comparing `peerplays-0.5.0/README.md` & `peerplays-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/account.py` & `peerplays-0.5.3/peerplays/account.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/amount.py` & `peerplays-0.5.3/peerplays/amount.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/asset.py` & `peerplays-0.5.3/peerplays/asset.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/bet.py` & `peerplays-0.5.3/peerplays/bet.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/bettingmarket.py` & `peerplays-0.5.3/peerplays/bettingmarket.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/bettingmarketgroup.py` & `peerplays-0.5.3/peerplays/bettingmarketgroup.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/block.py` & `peerplays-0.5.3/peerplays/block.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/blockchain.py` & `peerplays-0.5.3/peerplays/blockchain.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/account.py` & `peerplays-0.5.3/peerplays/cli/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import json
 import click
 from pprint import pprint
 from prettytable import PrettyTable
+from peerplays.block import BlockHeader
 from peerplays.account import Account
 from .decorators import onlineChain, unlockWallet
 from .ui import print_permissions, pprintOperation
 from .main import main
 
 
 @main.command()
@@ -69,16 +70,21 @@
 @click.argument("account", nargs=-1)
 @click.option("--csv/--table", help="Show output as csv or table", default=False)
 @click.option(
     "--type", type=str, help="Only show operations of this type", multiple=True
 )
 @click.option("--exclude", type=str, help="Exclude certain types", multiple=True)
 @click.option("--limit", type=int, help="Limit number of elements", default=15)
-@click.option("--raw/--no-raw", default=False)
-def history(ctx, account, limit, type, csv, exclude, raw):
+@click.option("--raw/--no-raw", default=False,
+              help="Show raw operation JSON"
+)
+@click.option("--results/--no-results", default=False,
+              help="Show operation results"
+)
+def history(ctx, account, limit, type, csv, exclude, raw, results):
     """ Show history of an account
     """
     from peerplaysbase.operations import getOperationNameForId
 
     header = ["#", "time (block)", "operation", "details"]
     if csv:
         import csv
@@ -89,19 +95,24 @@
         t = PrettyTable(header)
         t.align = "r"
         t.align["details"] = "l"
 
     for a in account:
         account = Account(a, peerplays_instance=ctx.peerplays)
         for b in account.history(limit=limit, only_ops=type, exclude_ops=exclude):
+            block = BlockHeader(b["block_num"])
             row = [
-                b["id"].split(".")[2],
-                "%s" % (b["block_num"]),
+                b["id"],
+                "%s (%s)" % (block.time(), b["block_num"]),
                 "{} ({})".format(getOperationNameForId(b["op"][0]), b["op"][0]),
-                pprintOperation(b) if not raw else json.dumps(b, indent=4),
+                (
+                    pprintOperation(b) if not raw else json.dumps(b, indent=4)
+                ) + (
+                    "" if not results else "\n\nresults: %s\n"%b["result"]
+                ),
             ]
             if csv:
                 t.writerow(row)
             else:
                 t.add_row(row)
     if not csv:
         click.echo(t)
```

### Comparing `peerplays-0.5.0/peerplays/cli/asset.py` & `peerplays-0.5.3/peerplays/cli/asset.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/bookie.py` & `peerplays-0.5.3/peerplays/cli/bookie.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/bos.py` & `peerplays-0.5.3/peerplays/cli/bos.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/cli.py` & `peerplays-0.5.3/peerplays/cli/cli.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/committee.py` & `peerplays-0.5.3/peerplays/cli/committee.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/decorators.py` & `peerplays-0.5.3/peerplays/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/info.py` & `peerplays-0.5.3/peerplays/cli/info.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/main.py` & `peerplays-0.5.3/peerplays/cli/main.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/message.py` & `peerplays-0.5.3/peerplays/cli/message.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/proposal.py` & `peerplays-0.5.3/peerplays/cli/proposal.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/rpc.py` & `peerplays-0.5.3/peerplays/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/wallet.py` & `peerplays-0.5.3/peerplays/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/cli/witness.py` & `peerplays-0.5.3/peerplays/cli/witness.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/committee.py` & `peerplays-0.5.3/peerplays/committee.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/event.py` & `peerplays-0.5.3/peerplays/event.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/eventgroup.py` & `peerplays-0.5.3/peerplays/eventgroup.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/exceptions.py` & `peerplays-0.5.3/peerplays/exceptions.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/genesisbalance.py` & `peerplays-0.5.3/peerplays/genesisbalance.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/instance.py` & `peerplays-0.5.3/peerplays/instance.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/market.py` & `peerplays-0.5.3/peerplays/market.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/memo.py` & `peerplays-0.5.3/peerplays/memo.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/message.py` & `peerplays-0.5.3/peerplays/message.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/notify.py` & `peerplays-0.5.3/peerplays/notify.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/peerplays.py` & `peerplays-0.5.3/peerplays/peerplays.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/peerplays2.py` & `peerplays-0.5.3/peerplays/peerplays2.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/price.py` & `peerplays-0.5.3/peerplays/price.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/proposal.py` & `peerplays-0.5.3/peerplays/proposal.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/rule.py` & `peerplays-0.5.3/peerplays/rule.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/son.py` & `peerplays-0.5.3/peerplays/son.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/sport.py` & `peerplays-0.5.3/peerplays/sport.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/storage.py` & `peerplays-0.5.3/peerplays/storage.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/transactionbuilder.py` & `peerplays-0.5.3/peerplays/transactionbuilder.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/utils.py` & `peerplays-0.5.3/peerplays/utils.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/wallet.py` & `peerplays-0.5.3/peerplays/wallet.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays/witness.py` & `peerplays-0.5.3/peerplays/witness.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplays.egg-info/PKG-INFO` & `peerplays-0.5.3/peerplays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peerplays
-Version: 0.5.0
+Version: 0.5.3
 Summary: Python library for PEERPLAYS
 Home-page: https://gitlab.com/PBSA/tools-libs/python-peerplays
 Author: PBSA and contributors. Original by Fabian Schuh.
 Author-email: info@pbsa.info
 Maintainer: PBSA
 Maintainer-email: info@pbsa.info
 Keywords: peerplays,library,api,rpc
```

### Comparing `peerplays-0.5.0/peerplays.egg-info/SOURCES.txt` & `peerplays-0.5.3/peerplays.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysapi/exceptions.py` & `peerplays-0.5.3/peerplaysapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysapi/node.py` & `peerplays-0.5.3/peerplaysapi/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,14 @@
             raise exceptions.UnhandledRPCError(msg)
         else:
             raise e
 
 
 class PeerPlaysNodeRPC(Api):
 
-    def register_apis(self):
-        self.login("", "", api_id=1)
-        self.api_id["database"] = self.database(api_id=1)
-        self.api_id["history"] = self.history(api_id=1)
-        self.api_id["network_broadcast"] = self.network_broadcast(api_id=1)
-
     def get_account(self, name, **kwargs):
         """ Get full account details from account name or id
 
             :param str name: Account name or account id
         """
         if len(name.split(".")) == 3:
             return self.get_objects([name])[0]
```

### Comparing `peerplays-0.5.0/peerplaysapi/websocket.py` & `peerplays-0.5.3/peerplaysapi/websocket.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/account.py` & `peerplays-0.5.3/peerplaysbase/account.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/asset_permissions.py` & `peerplays-0.5.3/peerplaysbase/asset_permissions.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/objects.py` & `peerplays-0.5.3/peerplaysbase/objects.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/objecttypes.py` & `peerplays-0.5.3/peerplaysbase/objecttypes.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/operationids.py` & `peerplays-0.5.3/peerplaysbase/operationids.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/operations.py` & `peerplays-0.5.3/peerplaysbase/operations.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/signedtransactions.py` & `peerplays-0.5.3/peerplaysbase/signedtransactions.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/peerplaysbase/types.py` & `peerplays-0.5.3/peerplaysbase/types.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/setup.py` & `peerplays-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 try:
     codecs.lookup("mbcs")
 except LookupError:
     ascii = codecs.lookup("ascii")
     codecs.register(lambda name, enc=ascii: {True: enc}.get(name == "mbcs"))
 
-VERSION = "0.5.0"
+VERSION = "0.5.3"
 
 # Strip some stuff from README for PyPI description:
 long_desc = open("README.md").read()
 long_desc = re.sub(
     '<!-- EXCLUDE_FROM_PYPI -->?(.*?)<!-- END_EXCLUDE_FROM_PYPI -->',
     '',
     long_desc,
```

### Comparing `peerplays-0.5.0/tests/test_account.py` & `peerplays-0.5.3/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_amount.py` & `peerplays-0.5.3/tests/test_amount.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_asset.py` & `peerplays-0.5.3/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_base_objects.py` & `peerplays-0.5.3/tests/test_base_objects.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_betting.py` & `peerplays-0.5.3/tests/test_betting.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_bookie.py` & `peerplays-0.5.3/tests/test_bookie.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_cachedlist.py` & `peerplays-0.5.3/tests/test_cachedlist.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_fee.py` & `peerplays-0.5.3/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_hrp.py` & `peerplays-0.5.3/tests/test_hrp.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_market.py` & `peerplays-0.5.3/tests/test_market.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_market_place.py` & `peerplays-0.5.3/tests/test_market_place.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_nft.py` & `peerplays-0.5.3/tests/test_nft.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_object_creation_parents.py` & `peerplays-0.5.3/tests/test_object_creation_parents.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_peerplays.py` & `peerplays-0.5.3/tests/test_peerplays.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_proposals.py` & `peerplays-0.5.3/tests/test_proposals.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_rbac_small.py` & `peerplays-0.5.3/tests/test_rbac_small.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_transactions.py` & `peerplays-0.5.3/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `peerplays-0.5.0/tests/test_txbuffers.py` & `peerplays-0.5.3/tests/test_txbuffers.py`

 * *Files identical despite different names*

