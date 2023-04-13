# Comparing `tmp/bovine-0.0.9.tar.gz` & `tmp/bovine-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.0.9.tar", max compression
+gzip compressed data, was "bovine-0.1.0.tar", max compression
```

## Comparing `bovine-0.0.9.tar` & `bovine-0.1.0.tar`

### file list

```diff
@@ -1,73 +1,104 @@
--rw-r--r--   0        0        0     9040 2023-03-25 10:32:01.307672 bovine-0.0.9/README.md
--rw-r--r--   0        0        0     1611 2023-03-25 10:38:12.803581 bovine-0.0.9/bovine/__init__.py
--rw-r--r--   0        0        0      135 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      433 2023-03-25 10:43:18.023969 bovine-0.0.9/bovine/activitypub/activity_factory.py
--rw-r--r--   0        0        0     5213 2023-03-25 10:37:33.475555 bovine-0.0.9/bovine/activitypub/actor.py
--rw-r--r--   0        0        0     2258 2023-03-24 15:50:13.824440 bovine-0.0.9/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      429 2023-03-20 10:43:54.377726 bovine-0.0.9/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0      582 2023-03-25 10:39:52.167675 bovine-0.0.9/bovine/activitypub/object_factory.py
--rw-r--r--   0        0        0     3159 2023-03-25 10:43:18.083969 bovine-0.0.9/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      500 2023-02-04 17:51:50.746650 bovine-0.0.9/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0      778 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/__init__.py
--rw-r--r--   0        0        0      597 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/accept_builder.py
--rw-r--r--   0        0        0     1456 2023-02-01 09:02:28.507153 bovine-0.0.9/bovine/activitystreams/activities/create_builder.py
--rw-r--r--   0        0        0      735 2023-03-10 14:37:48.405572 bovine-0.0.9/bovine/activitystreams/activities/delete_builder.py
--rw-r--r--   0        0        0      509 2023-02-01 10:42:10.659202 bovine-0.0.9/bovine/activitystreams/activities/follow_builder.py
--rw-r--r--   0        0        0     1040 2023-03-10 14:37:54.201636 bovine-0.0.9/bovine/activitystreams/activities/like_builder.py
--rw-r--r--   0        0        0      387 2023-01-17 14:01:43.244742 bovine-0.0.9/bovine/activitystreams/activities/test_accept_builder.py
--rw-r--r--   0        0        0      917 2023-03-10 14:36:42.507038 bovine-0.0.9/bovine/activitystreams/activities/test_create_builder.py
--rw-r--r--   0        0        0      259 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/activities/test_delete_builder.py
--rw-r--r--   0        0        0      379 2023-01-31 08:41:47.244847 bovine-0.0.9/bovine/activitystreams/activities/test_follow_builder.py
--rw-r--r--   0        0        0      409 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/test_like_builder.py
--rw-r--r--   0        0        0      299 2023-03-09 14:15:03.990325 bovine-0.0.9/bovine/activitystreams/activities/undo_builder.py
--rw-r--r--   0        0        0     3329 2023-03-10 14:36:37.496150 bovine-0.0.9/bovine/activitystreams/actor_builder.py
--rw-r--r--   0        0        0      155 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/__init__.py
--rw-r--r--   0        0        0      944 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/context_builder.py
--rw-r--r--   0        0        0     1357 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/common/test_context_builder.py
--rw-r--r--   0        0        0      307 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/activitystreams/objects/__init__.py
--rw-r--r--   0        0        0      235 2023-03-19 16:16:18.865574 bovine-0.0.9/bovine/activitystreams/objects/note_builder.py
--rw-r--r--   0        0        0     3794 2023-03-23 18:13:46.605395 bovine-0.0.9/bovine/activitystreams/objects/object_builder.py
--rw-r--r--   0        0        0     2157 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/activitystreams/objects/test_note_builder.py
--rw-r--r--   0        0        0      163 2023-01-31 08:42:22.041274 bovine-0.0.9/bovine/activitystreams/objects/test_tombstone_builder.py
--rw-r--r--   0        0        0      344 2023-03-10 14:37:20.402249 bovine-0.0.9/bovine/activitystreams/objects/tombstone_builder.py
--rw-r--r--   0        0        0     1021 2023-02-05 10:08:43.390300 bovine-0.0.9/bovine/activitystreams/ordered_collection_builder.py
--rw-r--r--   0        0        0      971 2023-02-04 15:54:46.460872 bovine-0.0.9/bovine/activitystreams/ordered_collection_page_builder.py
--rw-r--r--   0        0        0     1615 2023-03-10 14:36:40.235525 bovine-0.0.9/bovine/activitystreams/test_actor_builder.py
--rw-r--r--   0        0        0     1165 2023-02-04 15:45:55.208330 bovine-0.0.9/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      907 2023-02-04 15:55:05.840941 bovine-0.0.9/bovine/activitystreams/test_ordered_collection_page_builder.py
--rw-r--r--   0        0        0     1177 2023-03-21 16:59:50.049501 bovine-0.0.9/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0      787 2023-03-20 09:55:30.800090 bovine-0.0.9/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     1593 2023-03-19 16:16:18.805573 bovine-0.0.9/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0        0 2023-02-01 11:25:23.677425 bovine-0.0.9/bovine/clients/__init__.py
--rw-r--r--   0        0        0       83 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/clients/consts.py
--rw-r--r--   0        0        0     1034 2023-03-10 14:34:42.596286 bovine-0.0.9/bovine/clients/event_source.py
--rw-r--r--   0        0        0     1493 2023-03-24 15:30:34.358765 bovine-0.0.9/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3159 2023-03-24 17:31:32.720575 bovine-0.0.9/bovine/clients/moo_auth_client.py
--rw-r--r--   0        0        0     1399 2023-03-10 11:13:25.612108 bovine-0.0.9/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     3261 2023-03-10 14:34:56.587254 bovine-0.0.9/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     1074 2023-03-24 14:58:19.852389 bovine-0.0.9/bovine/clients/signed_http_client.py
--rw-r--r--   0        0        0      638 2023-03-25 10:43:18.023969 bovine-0.0.9/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      304 2023-03-10 15:13:34.129037 bovine-0.0.9/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1159 2023-03-10 14:35:33.299257 bovine-0.0.9/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      576 2023-03-24 14:59:03.816692 bovine-0.0.9/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0      282 2023-03-09 14:15:03.994325 bovine-0.0.9/bovine/test_types.py
--rw-r--r--   0        0        0     1832 2023-03-09 14:15:03.994325 bovine-0.0.9/bovine/types.py
--rw-r--r--   0        0        0     1045 2023-02-01 11:31:34.017446 bovine-0.0.9/bovine/utils/__init__.py
--rw-r--r--   0        0        0     1966 2023-03-25 10:43:18.055969 bovine-0.0.9/bovine/utils/crypto/__init__.py
--rw-r--r--   0        0        0     2175 2023-03-24 15:33:41.584599 bovine-0.0.9/bovine/utils/crypto/did_key.py
--rw-r--r--   0        0        0     1028 2023-03-25 10:43:18.035969 bovine-0.0.9/bovine/utils/crypto/test_crypto.py
--rw-r--r--   0        0        0     1339 2023-03-25 10:43:18.043969 bovine-0.0.9/bovine/utils/crypto/test_did_key.py
--rw-r--r--   0        0        0      519 2023-01-24 19:32:45.881784 bovine-0.0.9/bovine/utils/date.py
--rw-r--r--   0        0        0     1955 2023-03-24 14:26:06.295997 bovine-0.0.9/bovine/utils/http_signature.py
--rw-r--r--   0        0        0      186 2023-03-10 11:19:46.071642 bovine-0.0.9/bovine/utils/parse.py
--rw-r--r--   0        0        0     2715 2023-03-19 16:16:18.853573 bovine-0.0.9/bovine/utils/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-02-10 10:31:09.425518 bovine-0.0.9/bovine/utils/signature_parser.py
--rw-r--r--   0        0        0      181 2023-02-01 10:42:08.771183 bovine-0.0.9/bovine/utils/test.py
--rw-r--r--   0        0        0      737 2023-02-01 11:30:58.697070 bovine-0.0.9/bovine/utils/test_date.py
--rw-r--r--   0        0        0     2979 2023-03-19 16:16:18.825573 bovine-0.0.9/bovine/utils/test_http_signature.py
--rw-r--r--   0        0        0      457 2023-03-10 11:08:29.021486 bovine-0.0.9/bovine/utils/test_parse.py
--rw-r--r--   0        0        0     1207 2023-02-10 10:31:31.613742 bovine-0.0.9/bovine/utils/test_signature_parser.py
--rw-r--r--   0        0        0       22 2023-03-25 10:40:50.823746 bovine-0.0.9/bovine/version.py
--rw-r--r--   0        0        0      932 2023-03-25 10:40:37.763729 bovine-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 bovine-0.0.9/setup.py
--rw-r--r--   0        0        0     9872 1970-01-01 00:00:00.000000 bovine-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-13 15:55:57.830393 bovine-0.1.0/README.md
+-rw-r--r--   0        0        0     8584 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:55:57.986394 bovine-0.1.0/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-13 15:56:35.630722 bovine-0.1.0/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3091 2023-04-13 15:56:35.630722 bovine-0.1.0/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2476 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      905 2023-04-13 15:56:36.202727 bovine-0.1.0/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3664 2023-04-13 15:56:36.210727 bovine-0.1.0/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2736 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2219 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      429 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2909 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0     3664 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     3386 2023-04-13 15:56:36.194727 bovine-0.1.0/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3838 2023-04-13 15:56:36.194727 bovine-0.1.0/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4085 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     1493 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/ordered_collection_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1443 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/__pycache__/ordered_collection_page_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4559 2023-04-13 15:56:36.242727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3304 2023-04-13 15:56:36.266727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3167 2023-04-13 15:56:36.270727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2095 2023-04-13 15:56:36.274727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1431 2023-04-13 15:56:36.278727 bovine-0.1.0/bovine/activitystreams/__pycache__/test_ordered_collection_page_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3726 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4240 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0      949 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/ordered_collection_builder.py
+-rw-r--r--   0        0        0      899 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/ordered_collection_page_builder.py
+-rw-r--r--   0        0        0     2163 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1418 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1381 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1165 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      907 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/test_ordered_collection_page_builder.py
+-rw-r--r--   0        0        0     2354 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2835 2023-04-13 15:56:36.198727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2023-04-13 15:56:36.202727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4762 2023-04-13 15:56:36.290727 bovine-0.1.0/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      787 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     1326 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     1480 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      267 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1471 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1013 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2507 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1549 2023-04-13 15:56:36.302728 bovine-0.1.0/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     2470 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     1470 2023-04-13 15:56:36.070726 bovine-0.1.0/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1351 2023-04-13 15:56:36.294728 bovine-0.1.0/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1575 2023-04-13 15:56:36.298728 bovine-0.1.0/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1224 2023-04-13 15:56:36.298728 bovine-0.1.0/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2093 2023-04-13 15:56:36.306728 bovine-0.1.0/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      820 2023-04-13 15:56:36.306728 bovine-0.1.0/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0       91 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1106 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      787 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3176 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/moo_auth_client.py
+-rw-r--r--   0        0        0     1399 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     3278 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     1074 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/signed_http_client.py
+-rw-r--r--   0        0        0      609 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0      624 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      327 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1145 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      529 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     3999 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3633 2023-04-13 15:56:35.874724 bovine-0.1.0/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2921 2023-04-13 15:56:36.014725 bovine-0.1.0/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2908 2023-04-13 15:56:36.014725 bovine-0.1.0/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2256 2023-04-13 15:56:36.018725 bovine-0.1.0/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1783 2023-04-13 15:56:36.066726 bovine-0.1.0/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2362 2023-04-13 15:56:36.230727 bovine-0.1.0/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-04-13 15:56:36.314728 bovine-0.1.0/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2741 2023-04-13 15:56:36.318728 bovine-0.1.0/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     7453 2023-04-13 15:56:36.334728 bovine-0.1.0/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2673 2023-04-13 15:56:36.346728 bovine-0.1.0/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2764 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4989 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      178 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0      282 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/test_types.py
+-rw-r--r--   0        0        0     1837 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/types.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:55:57.986394 bovine-0.1.0/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      876 2023-04-13 15:56:36.018725 bovine-0.1.0/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0      365 2023-04-13 15:56:35.870724 bovine-0.1.0/bovine/utils/__pycache__/parse.cpython-310.pyc
+-rw-r--r--   0        0        0     3442 2023-04-13 15:56:36.366728 bovine-0.1.0/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1666 2023-04-13 15:56:36.370728 bovine-0.1.0/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      981 2023-04-13 15:56:36.374728 bovine-0.1.0/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      456 2023-04-13 15:56:36.374728 bovine-0.1.0/bovine/utils/__pycache__/webfinger.cpython-310.pyc
+-rw-r--r--   0        0        0      519 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/date.py
+-rw-r--r--   0        0        0      186 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/parse.py
+-rw-r--r--   0        0        0      181 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test.py
+-rw-r--r--   0        0        0      737 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      457 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      200 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0      332 2023-04-13 15:55:57.830393 bovine-0.1.0/bovine/utils/webfinger.py
+-rw-r--r--   0        0        0     1184 2023-04-13 15:55:57.834393 bovine-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10012 1970-01-01 00:00:00.000000 bovine-0.1.0/PKG-INFO
```

### Comparing `bovine-0.0.9/README.md` & `bovine-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 to write ActivityPub Clients. Furthermore, this package contains
 the cryptographic routines to verify HTTP signatures.
 
 Furthermore, the folder `examples` contains a few examples on
 how `BovineActor` can be used. The cryptographic routines
 are used in `bovine_fedi` to verify signatures.
 
+Documentation is available at [ReadTheDocs](https://bovine.readthedocs.io/en/latest/)
+
 ## Example: Make a post aka Faking at being a Server
 
 While [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.
 
 Without having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.
 
 The stub server is given by the following snippet. One should note that it just answers with predefined json from a config file, that hasn't been generated yet. One could easily replace it with serving static files. See also [the Mastodon Blog](https://blog.joinmastodon.org/2018/06/how-to-implement-a-basic-activitypub-server/) for a similar implementation.
@@ -90,15 +92,14 @@
 ```python
 import asyncio
 
 from uuid import uuid4
 from bovine import BovineActor
 
 target_account = "https://mas.to/users/themilkman"
-target_inbox = "https://mas.to/users/themilkman/inbox"
 
 
 async def run():
     async with BovineActor.from_file("bovine.toml") as actor:
         activity_factory, object_factory = actor.factories
         note = (
             object_factory.note("Hello")
@@ -106,35 +107,36 @@
             .with_mention(target_account)
             .build()
         )
         note["id"] = actor.actor_id + "/" + str(uuid4())
         create = activity_factory.create(note).build()
         create["id"] = actor.actor_id + "/" + str(uuid4())
 
+        remote_actor = await actor.get(target_account)
+        target_inbox = remote_actor["inbox"]
         await actor.post(target_inbox, create)
 
 
 asyncio.run(run())
 ```
 
 A few comments are in order:
 
 - The id needs to be set on the Note and Create in order to be compatible with Mastodon. When using proper Client To Server as below, it is superfluous
 - The form of adding the `target_account` to both to and mention causes it to be a direct message.
-- Normally, you would look up the inbox from the target account.
 
-## Using BovineActor
+## Using BovineClient
 
-One can import it via `from bovine import BovineActor`. Then one can either use it via:
+One can import it via `from bovine import BovineClient`. Then one can either use it via:
 
 ```python
-async with BovineActor(config) as actor:
+async with BovineClient(config) as actor:
     ...
 # or
-actor = BovineActor(config)
+actor = BovineClient(config)
 await actor.init()
 ```
 
 Here the config object can be present in two variants. First it can contain the keys `host` and `private_key`, where `host` is the domain the ActivityPub Actor is on and `private_key` is a mutlicodec encoded Ed25519 key, whose corresponding did-key has been added to the Actor. In this case [Moo-Auth-1](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation) will be used. The second variant is to use [HTTP Signatures](https://docs.joinmastodon.org/spec/security/#http), where the keys `account_url`, `public_key_url`, and `private_key` need to be present. Alternatively, to passing a config object, one can use `BovineActor.from_file(path_to_toml_file)`.
 
 ### Making a post
```

### Comparing `bovine-0.0.9/bovine/activitypub/collection_helper.py` & `bovine-0.1.0/bovine/activitypub/collection_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 
         self.element_cache = {}
 
     async def refresh(self):
         if self.basic_information is None:
             self.basic_information = await self.actor.get(self.collection_id)
 
-        print(self.basic_information)
-
         response = await self.actor.get(self.basic_information["first"])
 
         self.items = response["orderedItems"]
         self.next_items = response["next"]
         self.item_index = 0
 
     async def summary(self):
```

### Comparing `bovine-0.0.9/bovine/activitypub/test_actor.py` & `bovine-0.1.0/bovine/activitypub/test_actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 import json
 from unittest.mock import AsyncMock, MagicMock
 
 import aiohttp
 
+from bovine import BovineActor
 from bovine.activitystreams import (
     build_ordered_collection,
     build_ordered_collection_page,
 )
-from bovine.utils.test import get_user_keys
-
-from .actor import ActivityPubActor
-
-
-def test_actor_host():
-    actor = ActivityPubActor().with_actor_id("https://domain.tld/users/someone")
-
-    assert actor.host == "domain.tld"
+from bovine.crypto.test import private_key
 
 
 async def test_activity_pub_client_get_collection_no_pages():
     session = AsyncMock(aiohttp.ClientSession)
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
-    public_key, private_key = get_user_keys()
     session = AsyncMock(aiohttp.ClientSession)
     session.get = AsyncMock()
 
     actor = (
-        ActivityPubActor()
+        BovineActor({})
         .with_actor_id("actor_id")
         .with_http_signature(public_key_url, private_key, session=session)
     )
 
     text_mock = AsyncMock()
     session.get.return_value = MagicMock(aiohttp.ClientResponse)
     session.get.return_value.text = text_mock
@@ -49,20 +41,19 @@
     assert result["items"] == items
 
 
 async def test_activity_pub_client_get_collection_pages():
     session = AsyncMock(aiohttp.ClientSession)
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
-    public_key, private_key = get_user_keys()
     session = AsyncMock(aiohttp.ClientSession)
     session.get = AsyncMock()
 
     actor = (
-        ActivityPubActor()
+        BovineActor({})
         .with_actor_id("actor_id")
         .with_http_signature(public_key_url, private_key, session=session)
     )
     text_mock = AsyncMock()
     session.get.return_value = MagicMock(aiohttp.ClientResponse)
     session.get.return_value.text = text_mock
```

### Comparing `bovine-0.0.9/bovine/activitystreams/activities/like_builder.py` & `bovine-0.1.0/bovine/activitystreams/ordered_collection_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-import uuid
+class OrderedCollectionBuilder:
+    def __init__(self, url: str):
+        self.url = url
+        self.items: list | None = None
+        self.count = 0
+        self.first = None
+        self.last = None
 
-from bovine.activitystreams.common import build_context
-
-
-class LikeBuilder:
-    def __init__(self, account: str, obj: dict):
-        self.account = account
-        self.obj = obj
-        self.content = None
-        self.to = set()
-        self.cc = set()
-
-    def add_to(self, recipient):
-        self.to.add(recipient)
+    def with_items(self, items: list):
+        self.items = items
         return self
 
-    def add_cc(self, recipient):
-        self.cc.add(recipient)
+    def with_count(self, count: int):
+        self.count = count
         return self
 
-    def with_content(self, content):
-        self.content = content
+    def with_first_and_last(self, first, last):
+        self.first = first
+        self.last = last
         return self
 
     def build(self) -> dict:
-        context = build_context().build()
-
         result = {
-            "@context": context,
-            "id": self.account + "#likes+" + str(uuid.uuid4()),
-            "type": "Like",
-            "actor": self.account,
-            "object": self.obj,
+            "@context": "https://www.w3.org/ns/activitystreams",
+            "id": self.url,
+            "totalItems": self.count,
+            "type": "OrderedCollection",
         }
 
-        if self.to:
-            result["to"] = list(self.to)
+        if self.items:
+            result["orderedItems"] = self.items
 
-        if self.cc:
-            result["cc"] = list(self.cc)
+        if self.first:
+            result["first"] = self.first
 
-        if self.content:
-            result["content"] = self.content
+        if self.last:
+            result["last"] = self.last
 
         return result
```

### Comparing `bovine-0.0.9/bovine/activitystreams/ordered_collection_page_builder.py` & `bovine-0.1.0/bovine/activitystreams/ordered_collection_page_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from .common import build_context
-
-
 class OrderedCollectionPageBuilder:
     def __init__(self, url: str, part_of: str):
-        self.context_builder = build_context()
         self.url = url
         self.items: list = []
         self.part_of = part_of
         self.next: str | None = None
         self.prev: str | None = None
 
     def with_items(self, items: list):
@@ -20,15 +16,15 @@
 
     def with_prev(self, url):
         self.prev = url
         return self
 
     def build(self) -> dict:
         result = {
-            "@context": self.context_builder.build(),
+            "@context": "https://www.w3.org/ns/activitystreams",
             "id": self.url,
             "partOf": self.part_of,
             "orderedItems": self.items,
             "type": "OrderedCollectionPage",
         }
 
         if self.next:
```

### Comparing `bovine-0.0.9/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.1.0/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/activitystreams/test_ordered_collection_page_builder.py` & `bovine-0.1.0/bovine/activitystreams/test_ordered_collection_page_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/activitystreams/utils/print.py` & `bovine-0.1.0/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/clients/event_source.py` & `bovine-0.1.0/bovine/clients/event_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import aiohttp
 
 from bovine.types import ServerSentEvent
 
 
 class EventSource:
-    def __init__(self, session, url, headers={}):
+    def __init__(self, session: aiohttp.ClientSession, url: str, headers: dict = {}):
         self.session = session
         self.url = url
         self.headers = headers
         self.response = None
 
     async def create_response(self):
         timeout = aiohttp.ClientTimeout(total=None)
@@ -23,16 +23,18 @@
         return self
 
     async def __anext__(self):
         if self.response is None:
             await self.create_response()
 
         to_parse = ""
+
         async for line_in_bytes in self.response.content:
             line = line_in_bytes.decode("utf-8")
             if line[0] == ":":
                 continue
             if line == "\n":
                 event = ServerSentEvent.parse_utf8(to_parse)
-                return event
+                if event.data:
+                    return event
             else:
                 to_parse = f"{to_parse}{line}"
```

### Comparing `bovine-0.0.9/bovine/clients/lookup_account.py` & `bovine-0.1.0/bovine/clients/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,39 @@
-import json
-import logging
-
 import aiohttp
 
 from bovine.utils.parse import parse_fediverse_handle
 
-from .consts import BOVINE_CLIENT_NAME
-
-logger = logging.getLogger(__name__)
-
-
-async def lookup_with_webfinger(
-    session: aiohttp.ClientSession, webfinger_url: str, params: dict
-):
-    async with session.get(
-        webfinger_url, params=params, headers={"user-agent": BOVINE_CLIENT_NAME}
-    ) as response:
-        if response.status != 200:
-            logger.warn(f"{params['resource']} not found using webfinger")
-            return None
-        text = await response.text()
-        data = json.loads(text)
-
-        if "links" not in data:
-            return None
-
-        links = data["links"]
-        for entry in links:
-            if "rel" in entry and entry["rel"] == "self":
-                return entry["href"]
-
-    return None
+from .lookup_account import lookup_with_webfinger  # noqa F401
 
 
 async def lookup_account_with_webfinger(
     session: aiohttp.ClientSession, fediverse_handle: str
 ) -> str | None:
+    """Looks up the actor url associated with a FediVerse handle,
+    i.e. an identifier of the form username@domain, using
+    the webfinger endpoint
+
+    :param session: the aiohttp.ClientSession to use
+    :param fediverse_handle: the FediVerse handle as a string
+    """
     username, domain = parse_fediverse_handle(fediverse_handle)
 
     webfinger_url = f"https://{domain}/.well-known/webfinger"
     params = {"resource": f"acct:{username}@{domain}"}
 
     return await lookup_with_webfinger(session, webfinger_url, params)
 
 
 async def lookup_did_with_webfinger(
     session: aiohttp.ClientSession, domain: str, did: str
 ) -> str | None:
+    """Looks up the actor url associated with a did and domain
+    using the webfinger endpoint
+
+    :param session: the aiohttp.ClientSession to use
+    :param domain: the domain to perform the lookup from
+    :param did: the did key to perform lookup with
+    """
     webfinger_url = f"https://{domain}/.well-known/webfinger"
     params = {"resource": did}
 
     return await lookup_with_webfinger(session, webfinger_url, params)
```

### Comparing `bovine-0.0.9/bovine/clients/moo_auth_client.py` & `bovine-0.1.0/bovine/clients/moo_auth_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from urllib.parse import urlparse
 
-from bovine.utils import build_signature
-from bovine.utils.crypto import content_digest_sha256
+from bovine.crypto.helper import content_digest_sha256
+from bovine.crypto.http_signature import build_signature
 from bovine.utils.date import get_gmt_now
 
 from .consts import BOVINE_CLIENT_NAME
 from .event_source import EventSource
 
 # from bovine.utils.crypto.did_key import private_key_to_ed25519
```

### Comparing `bovine-0.0.9/bovine/clients/nodeinfo.py` & `bovine-0.1.0/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/clients/signed_http.py` & `bovine-0.1.0/bovine/clients/signed_http.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from urllib.parse import urlparse
 
 import aiohttp
 
-from bovine.utils import build_signature
-from bovine.utils.crypto import content_digest_sha256
+from bovine.crypto.helper import content_digest_sha256
+from bovine.crypto.http_signature import build_signature
 from bovine.utils.date import get_gmt_now
 
 from .consts import BOVINE_CLIENT_NAME
 from .event_source import EventSource
 
 logger = logging.getLogger(__name__)
```

### Comparing `bovine-0.0.9/bovine/clients/signed_http_client.py` & `bovine-0.1.0/bovine/clients/signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/clients/test_lookup_account.py` & `bovine-0.1.0/bovine/clients/test_lookup_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiohttp
 
-from .lookup_account import lookup_account_with_webfinger, lookup_did_with_webfinger
+from . import lookup_account_with_webfinger, lookup_did_with_webfinger
 
 
 async def test_lookup_account():
     async with aiohttp.ClientSession() as session:
         result = await lookup_account_with_webfinger(session, "helge@mymath.rocks")
 
     assert result.startswith("https://mymath.rocks/")
```

### Comparing `bovine-0.0.9/bovine/clients/test_signed_http.py` & `bovine-0.1.0/bovine/clients/test_signed_http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from unittest.mock import AsyncMock, MagicMock
 
 import aiohttp
 
-from bovine.utils.signature_checker import SignatureChecker
-from bovine.utils.test import get_user_keys
+from bovine.crypto.signature_checker import SignatureChecker
+from bovine.crypto.test import private_key, public_key
 
 from .signed_http import signed_get
 
 
 async def test_signed_get():
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
-    public_key, private_key = get_user_keys()
     session = AsyncMock(aiohttp.ClientSession)
     session.get = AsyncMock()
     session.get.return_value = "value"
 
     key_retriever = AsyncMock()
-    key_retriever.return_value = public_key
+    key_retriever.return_value = public_key, "owner"
     signature_checker = SignatureChecker(key_retriever)
 
     response = await signed_get(session, public_key_url, private_key, url)
 
     session.get.assert_awaited_once()
 
     assert response == "value"
@@ -33,11 +32,11 @@
     headers = args[1]["headers"]
 
     request = MagicMock()
     request.headers = headers
     request.method = "get"
     request.url = url
 
-    assert await signature_checker.validate_signature(request)
+    assert await signature_checker.validate_signature(request) == "owner"
 
     key_retriever.assert_awaited_once()
     assert key_retriever.await_args[0] == (public_key_url,)
```

### Comparing `bovine-0.0.9/bovine/clients/test_signed_http_client.py` & `bovine-0.1.0/bovine/clients/test_signed_http_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from unittest.mock import AsyncMock
 
 import aiohttp
 
-from bovine.utils.test import get_user_keys
+from bovine.crypto.test import private_key
 
 from .signed_http_client import SignedHttpClient
 
 
 async def test_activity_pub_client_get():
     session = AsyncMock(aiohttp.ClientSession)
     url = "https://test_domain/test_path"
     public_key_url = "public_key_url"
-    public_key, private_key = get_user_keys()
     session = AsyncMock(aiohttp.ClientSession)
     session.get = AsyncMock()
 
     client = SignedHttpClient(session, public_key_url, private_key)
 
     await client.get(url)
```

### Comparing `bovine-0.0.9/bovine/types.py` & `bovine-0.1.0/bovine/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return message.encode("utf-8")
 
     @staticmethod
     def parse(raw):
         return ServerSentEvent.parse_utf8(raw.decode("utf-8"))
 
     @staticmethod
-    def parse_utf8(raw):
+    def parse_utf8(raw: str):
         data = None
         event = None
         event_id = None
         retry = None
         for line in raw.splitlines():
             m = sse_line_pattern.match(line)
             if m is None:
```

### Comparing `bovine-0.0.9/bovine/utils/crypto/__init__.py` & `bovine-0.1.0/bovine/crypto/helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,91 @@
 import base64
 import hashlib
 import logging
 
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding, rsa
+from cryptography.hazmat.primitives.asymmetric import ed25519, padding, rsa
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key,
 )
+from multiformats import multibase, multicodec
 
 logger = logging.getLogger(__name__)
 
 
-def generate_public_private_key():
-    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048)
-    private_key_pem = private_key.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.PKCS8,
-        encryption_algorithm=serialization.NoEncryption(),
-    )
-
-    public_key = private_key.public_key()
-    public_key_pem = public_key.public_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PublicFormat.SubjectPublicKeyInfo,
-    )
+def content_digest_sha256(content: str | bytes) -> str:
+    """Computes the SHA256 digest of given content"""
+    if isinstance(content, str):
+        content = content.encode("utf-8")
 
-    return public_key_pem.decode("utf-8"), private_key_pem.decode("utf-8")
+    digest = base64.standard_b64encode(hashlib.sha256(content).digest()).decode("utf-8")
+    return "sha-256=" + digest
 
 
 def sign_message(private_key, message):
-    key = load_pem_private_key(private_key.encode("utf-8"), password=None)
+    private_key = private_key.replace("\\n", "\n")
+    try:
+        key = load_pem_private_key(private_key.encode("utf-8"), password=None)
+        assert isinstance(key, rsa.RSAPrivateKey)
+    except Exception as e:
+        logger.error(e)
+        logger.error(private_key)
+        raise (e)
 
     return base64.standard_b64encode(
         key.sign(
             message.encode("utf-8"),
             padding.PKCS1v15(),
             hashes.SHA256(),
         )
     ).decode("utf-8")
 
 
 def verify_signature(public_key, message, signature):
+    public_key = public_key.replace("\\n", "\n")
     public_key_loaded = load_pem_public_key(public_key.encode("utf-8"))
 
+    assert isinstance(public_key_loaded, rsa.RSAPublicKey)
+
     try:
         public_key_loaded.verify(
             base64.standard_b64decode(signature),
             message.encode("utf-8"),
             padding.PKCS1v15(),
             hashes.SHA256(),
         )
     except InvalidSignature:
         logger.warning("invalid signature")
         return False
 
     return True
 
 
-def content_digest_sha256(content):
-    if isinstance(content, str):
-        content = content.encode("utf-8")
+def public_key_to_did_key(public_key: ed25519.Ed25519PublicKey) -> str:
+    public_bytes = public_key.public_bytes(
+        encoding=serialization.Encoding.Raw,
+        format=serialization.PublicFormat.Raw,
+    )
 
-    digest = base64.standard_b64encode(hashlib.sha256(content).digest()).decode("utf-8")
-    return "sha-256=" + digest
+    wrapped = multicodec.wrap("ed25519-pub", public_bytes)
+    encoded = multibase.encode(wrapped, "base58btc")
+
+    return "did:key:" + encoded
+
+
+def did_key_to_public_key(did: str) -> ed25519.Ed25519PublicKey:
+    assert did.startswith("did:key:")
+    decoded = multibase.decode(did[8:])
+    codec, key_bytes = multicodec.unwrap(decoded)
+    assert codec.name == "ed25519-pub"
+
+    return ed25519.Ed25519PublicKey.from_public_bytes(key_bytes)
+
+
+def private_key_to_ed25519(private_key_str: str) -> ed25519.Ed25519PrivateKey:
+    decoded = multibase.decode(private_key_str)
+    codec, key_bytes = multicodec.unwrap(decoded)
+    assert codec.name == "ed25519-priv"
+
+    return ed25519.Ed25519PrivateKey.from_private_bytes(key_bytes)
```

### Comparing `bovine-0.0.9/bovine/utils/crypto/test_crypto.py` & `bovine-0.1.0/bovine/crypto/test_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-from bovine.utils.test import get_user_keys
+from cryptography.hazmat.primitives.asymmetric import ed25519
 
-from . import (
+from .helper import (
     content_digest_sha256,
-    generate_public_private_key,
+    did_key_to_public_key,
     sign_message,
     verify_signature,
 )
+from .test import private_key, public_key
 
 
-def test_crypto_sign_verify():
-    message = "secret"
-
-    public_key, private_key = get_user_keys()
-
-    signature = sign_message(private_key, message)
+def test_content_digest_sha256():
+    digest = content_digest_sha256("content")
 
-    assert verify_signature(public_key, message, signature)
+    assert digest == "sha-256=7XACtDnprIRfIjV9giusFERzD722AW0+yUMil7nsn3M="
 
 
-def test_crypto_sign_verify_failure():
-    message = "secret"
+def test_did_to_public_key():
+    did_example = "did:key:z6MkiTBz1ymuepAQ4HEHYSF1H8quG5GLVVQR3djdX3mDooWp"
 
-    public_key, private_key = get_user_keys()
+    public_key = did_key_to_public_key(did_example)
 
-    assert not verify_signature(public_key, message, "")
+    assert isinstance(public_key, ed25519.Ed25519PublicKey)
 
 
-def test_content_digest_sha256():
-    digest = content_digest_sha256("content")
+def test_crypto_sign_verify():
+    message = "secret"
 
-    assert digest.startswith("sha-256=")
+    signature = sign_message(private_key, message)
 
+    assert verify_signature(public_key, message, signature)
 
-def test_generate_public_private_key():
-    public_key, private_key = generate_public_private_key()
 
-    assert public_key.startswith("-----BEGIN PUBLIC KEY-----")
-    assert public_key.endswith("-----END PUBLIC KEY-----\n")
+def test_crypto_sign_verify_failure():
+    message = "secret"
 
-    assert private_key.startswith("-----BEGIN PRIVATE KEY-----")
-    assert private_key.endswith("-----END PRIVATE KEY-----\n")
+    assert not verify_signature(public_key, message, "")
```

### Comparing `bovine-0.0.9/bovine/utils/date.py` & `bovine-0.1.0/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/utils/http_signature.py` & `bovine-0.1.0/bovine/crypto/http_signature.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import logging
 
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives.asymmetric import ed25519
 from multiformats import multibase, multicodec
 
-from .crypto import sign_message, verify_signature
-from .crypto.did_key import did_key_to_public_key
+from .helper import did_key_to_public_key, sign_message, verify_signature
 
 logger = logging.getLogger(__name__)
 
 
+def build_signature(host, method, target):
+    return (
+        HttpSignature()
+        .with_field("(request-target)", f"{method} {target}")
+        .with_field("host", host)
+    )
+
+
 class HttpSignature:
     def __init__(self):
         self.fields = []
 
     def build_signature(self, key_id, private_key):
         message = self.build_message()
```

### Comparing `bovine-0.0.9/bovine/utils/signature_checker.py` & `bovine-0.1.0/bovine/crypto/signature_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import logging
 import traceback
 from urllib.parse import urlparse
 
-from .date import check_max_offset_now, parse_gmt
+import bovine.utils.date
+from bovine.utils.date import parse_gmt
+
+from .helper import content_digest_sha256
 from .http_signature import HttpSignature
 from .signature_parser import parse_signature_header
 
 logger = logging.getLogger(__name__)
 
 
 class SignatureChecker:
     def __init__(self, key_retriever):
         self.key_retriever = key_retriever
 
-    async def validate_signature(self, request, digest=None):
+    async def validate_signature(self, request):
         if "signature" not in request.headers:
-            logger.warning("Signature not present")
+            logger.debug("Signature not present")
             return None
 
+        if request.method.lower() == "post":
+            data = await request.get_data()
+            digest = content_digest_sha256(data)
+        else:
+            digest = None
+
         if digest is not None:
             request_digest = request.headers["digest"]
             request_digest = request_digest[:4].lower() + request_digest[4:]
             if request_digest != digest:
                 logger.warning("Different digest")
                 return None
 
@@ -38,37 +47,37 @@
                 return None
 
             if digest is not None and "digest" not in signature_fields:
                 logger.warning("Digest not present, but computable")
                 return None
 
             http_date = parse_gmt(request.headers["date"])
-            if not check_max_offset_now(http_date):
+            if not bovine.utils.date.check_max_offset_now(http_date):
                 logger.warning(
                     f"Encountered invalid http date {request.headers['date']}"
                 )
                 return None
 
             for field in signature_fields:
                 if field == "(request-target)":
                     method = request.method.lower()
                     parsed_url = urlparse(request.url)
                     path = parsed_url.path
                     http_signature.with_field(field, f"{method} {path}")
                 else:
                     http_signature.with_field(field, request.headers[field])
 
-            public_key = await self.key_retriever(parsed_signature.key_id)
+            public_key, owner = await self.key_retriever(parsed_signature.key_id)
 
             if public_key is None:
-                logger.warning(f"Could not retrieve key from {parsed_signature.key_id}")
+                logger.debug(f"Could not retrieve key from {parsed_signature.key_id}")
                 return None
 
             if http_signature.verify(public_key, parsed_signature.signature):
-                return parsed_signature.key_id
+                return owner
 
         except Exception as e:
             logger.error(str(e))
             logger.error(request.headers)
             for log_line in traceback.format_exc().splitlines():
                 logger.error(log_line)
             return None
```

### Comparing `bovine-0.0.9/bovine/utils/signature_parser.py` & `bovine-0.1.0/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/utils/test_date.py` & `bovine-0.1.0/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/bovine/utils/test_signature_parser.py` & `bovine-0.1.0/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.0.9/setup.py` & `bovine-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,260 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bovine
+Version: 0.1.0
+Summary: Core functionality of bovine needed to build client to server applications
+Home-page: https://codeberg.org/helge/bovine
+License: MIT
+Author: Helge
+Author-email: helge.krueger@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: bleach (>=6.0.0,<7.0.0)
+Requires-Dist: cryptography (>=39.0.0,<40.0.0)
+Requires-Dist: multiformats (>=0.2.1,<0.3.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Project-URL: Documentation, https://bovine.readthedocs.io/en/latest/
+Project-URL: Repository, https://codeberg.org/helge/bovine
+Description-Content-Type: text/markdown
 
-packages = \
-['bovine',
- 'bovine.activitypub',
- 'bovine.activitystreams',
- 'bovine.activitystreams.activities',
- 'bovine.activitystreams.common',
- 'bovine.activitystreams.objects',
- 'bovine.activitystreams.utils',
- 'bovine.clients',
- 'bovine.utils',
- 'bovine.utils.crypto']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.3,<4.0.0',
- 'bleach>=6.0.0,<7.0.0',
- 'cryptography>=39.0.0,<40.0.0',
- 'multiformats>=0.2.1,<0.3.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'tomli>=2.0.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'bovine',
-    'version': '0.0.9',
-    'description': 'Core functionality of bovine needed to build client to server applications',
-    'long_description': '# Bovine\n\nThis package contains two essential parts of bovine. First\nit defines `BovineActor`, which contains all the necessities\nto write ActivityPub Clients. Furthermore, this package contains\nthe cryptographic routines to verify HTTP signatures.\n\nFurthermore, the folder `examples` contains a few examples on\nhow `BovineActor` can be used. The cryptographic routines\nare used in `bovine_fedi` to verify signatures.\n\n## Example: Make a post aka Faking at being a Server\n\nWhile [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.\n\nWithout having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.\n\nThe stub server is given by the following snippet. One should note that it just answers with predefined json from a config file, that hasn\'t been generated yet. One could easily replace it with serving static files. See also [the Mastodon Blog](https://blog.joinmastodon.org/2018/06/how-to-implement-a-basic-activitypub-server/) for a similar implementation.\n\n```python\nimport tomli\nimport json\nfrom quart import Quart\n\napp = Quart(__name__)\n\nwith open("server.toml", "rb") as fp:\n    config = tomli.load(fp)\n\n@app.get("/.well-known/webfinger")\nasync def webfinger():\n    return json.loads(config["webfinger"])\n\n\n@app.get("/actor")\nasync def actor():\n    return json.loads(config["actor"])\n\nif __name__ == "__main__":\n    app.run()\n```\n\nThe following script generates the config files. You will have to adapt the `hostname` variable and be able to serve the entire thing through https.\n\n```python\nimport bovine\nimport tomli_w\nimport json\n\nhostname = "bovine-demo.mymath.rocks"\n\npublic_key, private_key = bovine.utils.crypto.generate_public_private_key()\nactor_url = f"https://{hostname}/actor"\nactor = (\n    bovine.activitystreams.build_actor("actor")\n    .with_account_url(actor_url)\n    .with_public_key(public_key)\n)\n\nwebfinger = {\n    "subject": f"acct:actor@{hostname}",\n    "links": [\n        {\n            "href": actor_url,\n            "rel": "self",\n            "type": "application/activity+json",\n        }\n    ],\n}\n\nserver_config = {"actor": json.dumps(actor.build()), "webfinger": json.dumps(webfinger)}\n\nactor_config = {\n    "account_url": actor_url,\n    "public_key_url": f"{actor_url}#main-key",\n    "private_key": private_key,\n}\n\nwith open("server.toml", "wb") as fp:\n    tomli_w.dump(server_config, fp)\n\nwith open("bovine.toml", "wb") as fp:\n    tomli_w.dump(actor_config, fp)\n```\n\nYou can now access the urls, which are in my case [https://bovine-demo.mymath.rocks/actor](https://bovine-demo.mymath.rocks/actor) and [https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks](https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks). Using this, we can now lookup the fediverse handle `actor@bovine-demo.mymath.rocks` on most FediVerse applications.\n\nYou can now send a post via the following code snippet:\n\n```python\nimport asyncio\n\nfrom uuid import uuid4\nfrom bovine import BovineActor\n\ntarget_account = "https://mas.to/users/themilkman"\ntarget_inbox = "https://mas.to/users/themilkman/inbox"\n\n\nasync def run():\n    async with BovineActor.from_file("bovine.toml") as actor:\n        activity_factory, object_factory = actor.factories\n        note = (\n            object_factory.note("Hello")\n            .add_to(target_account)\n            .with_mention(target_account)\n            .build()\n        )\n        note["id"] = actor.actor_id + "/" + str(uuid4())\n        create = activity_factory.create(note).build()\n        create["id"] = actor.actor_id + "/" + str(uuid4())\n\n        await actor.post(target_inbox, create)\n\n\nasyncio.run(run())\n```\n\nA few comments are in order:\n\n- The id needs to be set on the Note and Create in order to be compatible with Mastodon. When using proper Client To Server as below, it is superfluous\n- The form of adding the `target_account` to both to and mention causes it to be a direct message.\n- Normally, you would look up the inbox from the target account.\n\n## Using BovineActor\n\nOne can import it via `from bovine import BovineActor`. Then one can either use it via:\n\n```python\nasync with BovineActor(config) as actor:\n    ...\n# or\nactor = BovineActor(config)\nawait actor.init()\n```\n\nHere the config object can be present in two variants. First it can contain the keys `host` and `private_key`, where `host` is the domain the ActivityPub Actor is on and `private_key` is a mutlicodec encoded Ed25519 key, whose corresponding did-key has been added to the Actor. In this case [Moo-Auth-1](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation) will be used. The second variant is to use [HTTP Signatures](https://docs.joinmastodon.org/spec/security/#http), where the keys `account_url`, `public_key_url`, and `private_key` need to be present. Alternatively, to passing a config object, one can use `BovineActor.from_file(path_to_toml_file)`.\n\n### Making a post\n\nBovineActor contains two factories to create [ActivityStreams Objects](https://www.w3.org/TR/activitystreams-vocabulary/#object-types) and [ActivityStreams Activities](https://www.w3.org/TR/activitystreams-vocabulary/#activity-types). One can obtain them by running\n\n```python\nactivity_factory, object_factory = actor.factories\n```\n\nThe simplest usage example is a create wrapping a note, that looks like:\n\n```python\nactivity_factory, object_factory = actor.factories\nnote = object_factory.note("Hello").as_public().build()\ncreate = activity_factory.create(note).build()\n```\n\nThe result should be the something equivalent to the json\n\n```json\n{\n  "@context": "https://www.w3.org/ns/activitystreams",\n  "type": "Create",\n  "actor": "https://domain/actor",\n  "object": {\n    "attributedTo": "https://domain/actor",\n    "type": "Note",\n    "content": "Hello",\n    "published": "2023-03-25T08:12:32Z",\n    "to": "as:Public",\n    "cc": "https://domain/followers_collection"\n  },\n  "published": "2023-03-25T08:12:32Z",\n  "to": "as:Public",\n  "cc": "https://domain/followers_collection"\n}\n```\n\nThe details depend on the used actor and will likely contain superfluous elements until the creation process is improved. We can now send this activity to our outbox using\n\n```python\nawait actor.send_to_outbox(create)\n```\n\n__Note__: This is different from what we did in the first example, where we used `await actor.post(inbox, create)`. The difference is that in the first example, we faked being a server, now we are actually using Client To Server.\n\n### The inbox and outbox\n\nBy running\n\n```python\ninbox = await actor.inbox()\noutbox = await actor.outbox()\n```\n\none can obtain `CollectionHelper` objects. These are meant to make it easier to interact with collection objects. In the simplest use case, one can use\n\n```python\nawait inbox.next_item()\n```\n\nto get the items from the inbox one after the other. It is also possible to print a summary of all elements that have been fetched from the inbox using `await inbox.summary()`. Finally, it is possible to iterate over the inbox via\n\n```python\nasync for item in inbox.iterate(max_number=3):\n    do_something(item)\n```\n\n### Proxying elements\n\nWe have already seen the difference between using `post` directly to an inbox and posting to the actor\'s outbox using `send_to_outbox`. A similar pattern applies to fetching objects. Both of these commands often have a similar result\n\n```python\nawait actor.get(object_id)\nawait actor.proxy_element(object_id)\n```\n\nHowever, they do different things:\n\n- The first `actor.get` sends a webrequest to the server `object_id` is on and retrieves it\n- The second `actor.proxy_element` sends a request to the actor\'s server for the object. This request is then either answered from the server\'s object store or by the server fetching the object. The cache behavior is up to the server. Depending of the evolution of `proxyUrl` of an Actor, more options might be added here.\n\nAs most servers don\'t support Moo-Auth-1, using `proxy_element` is the only way to obtain foreign objects, when using it.\n\n### Event Source\n\nThe event source is demonstrated in `examples/sse.py`. First, the event source will be specified in a [FEP](https://codeberg.org/fediverse/fep) to come. It provides a way to receive updates from the server, whenever a new element is added to the inbox or outbox. The basic usage is\n\n```python\nevent_source = await actor.event_source()\nasync for event in event_source:\n    if event and event.data:\n        data = json.loads(event.data)\n        do_something(data)\n```\n\nIf you plan on writing long running applications, the event source does not automatically reconnect, so you will need to implement this. [mechanical_bull](https://codeberg.org/helge/mechanical_bull) uses the event source in this way.\n',
-    'author': 'Helge',
-    'author_email': 'helge.krueger@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://codeberg.org/helge/bovine',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+# Bovine
+
+This package contains two essential parts of bovine. First
+it defines `BovineActor`, which contains all the necessities
+to write ActivityPub Clients. Furthermore, this package contains
+the cryptographic routines to verify HTTP signatures.
+
+Furthermore, the folder `examples` contains a few examples on
+how `BovineActor` can be used. The cryptographic routines
+are used in `bovine_fedi` to verify signatures.
+
+Documentation is available at [ReadTheDocs](https://bovine.readthedocs.io/en/latest/)
+
+## Example: Make a post aka Faking at being a Server
+
+While [ActivityPub](https://www.w3.org/TR/activitypub/) specifies Server to Server and Client to Server, they really are just two sides of the same coin. In this example, we will work through how to use `BovineActor` to post a message.
+
+Without having an ActivityPub Server supporting Client to Server, this will require a bit of setup. This setup will build a stub server that just allows other ActivityPub servers to associate us with a domain.
+
+The stub server is given by the following snippet. One should note that it just answers with predefined json from a config file, that hasn't been generated yet. One could easily replace it with serving static files. See also [the Mastodon Blog](https://blog.joinmastodon.org/2018/06/how-to-implement-a-basic-activitypub-server/) for a similar implementation.
+
+```python
+import tomli
+import json
+from quart import Quart
+
+app = Quart(__name__)
+
+with open("server.toml", "rb") as fp:
+    config = tomli.load(fp)
+
+@app.get("/.well-known/webfinger")
+async def webfinger():
+    return json.loads(config["webfinger"])
+
+
+@app.get("/actor")
+async def actor():
+    return json.loads(config["actor"])
+
+if __name__ == "__main__":
+    app.run()
+```
+
+The following script generates the config files. You will have to adapt the `hostname` variable and be able to serve the entire thing through https.
+
+```python
+import bovine
+import tomli_w
+import json
+
+hostname = "bovine-demo.mymath.rocks"
+
+public_key, private_key = bovine.utils.crypto.generate_public_private_key()
+actor_url = f"https://{hostname}/actor"
+actor = (
+    bovine.activitystreams.build_actor("actor")
+    .with_account_url(actor_url)
+    .with_public_key(public_key)
+)
+
+webfinger = {
+    "subject": f"acct:actor@{hostname}",
+    "links": [
+        {
+            "href": actor_url,
+            "rel": "self",
+            "type": "application/activity+json",
+        }
+    ],
+}
+
+server_config = {"actor": json.dumps(actor.build()), "webfinger": json.dumps(webfinger)}
+
+actor_config = {
+    "account_url": actor_url,
+    "public_key_url": f"{actor_url}#main-key",
+    "private_key": private_key,
 }
 
+with open("server.toml", "wb") as fp:
+    tomli_w.dump(server_config, fp)
+
+with open("bovine.toml", "wb") as fp:
+    tomli_w.dump(actor_config, fp)
+```
+
+You can now access the urls, which are in my case [https://bovine-demo.mymath.rocks/actor](https://bovine-demo.mymath.rocks/actor) and [https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks](https://bovine-demo.mymath.rocks/.well-known/webfinger?resource=acct:actor@bovine-demo.mymath.rocks). Using this, we can now lookup the fediverse handle `actor@bovine-demo.mymath.rocks` on most FediVerse applications.
+
+You can now send a post via the following code snippet:
+
+```python
+import asyncio
+
+from uuid import uuid4
+from bovine import BovineActor
+
+target_account = "https://mas.to/users/themilkman"
+
+
+async def run():
+    async with BovineActor.from_file("bovine.toml") as actor:
+        activity_factory, object_factory = actor.factories
+        note = (
+            object_factory.note("Hello")
+            .add_to(target_account)
+            .with_mention(target_account)
+            .build()
+        )
+        note["id"] = actor.actor_id + "/" + str(uuid4())
+        create = activity_factory.create(note).build()
+        create["id"] = actor.actor_id + "/" + str(uuid4())
+
+        remote_actor = await actor.get(target_account)
+        target_inbox = remote_actor["inbox"]
+        await actor.post(target_inbox, create)
+
+
+asyncio.run(run())
+```
+
+A few comments are in order:
+
+- The id needs to be set on the Note and Create in order to be compatible with Mastodon. When using proper Client To Server as below, it is superfluous
+- The form of adding the `target_account` to both to and mention causes it to be a direct message.
+
+## Using BovineClient
+
+One can import it via `from bovine import BovineClient`. Then one can either use it via:
+
+```python
+async with BovineClient(config) as actor:
+    ...
+# or
+actor = BovineClient(config)
+await actor.init()
+```
+
+Here the config object can be present in two variants. First it can contain the keys `host` and `private_key`, where `host` is the domain the ActivityPub Actor is on and `private_key` is a mutlicodec encoded Ed25519 key, whose corresponding did-key has been added to the Actor. In this case [Moo-Auth-1](https://blog.mymath.rocks/2023-03-15/BIN1_Moo_Authentication_and_Authoriation) will be used. The second variant is to use [HTTP Signatures](https://docs.joinmastodon.org/spec/security/#http), where the keys `account_url`, `public_key_url`, and `private_key` need to be present. Alternatively, to passing a config object, one can use `BovineActor.from_file(path_to_toml_file)`.
+
+### Making a post
+
+BovineActor contains two factories to create [ActivityStreams Objects](https://www.w3.org/TR/activitystreams-vocabulary/#object-types) and [ActivityStreams Activities](https://www.w3.org/TR/activitystreams-vocabulary/#activity-types). One can obtain them by running
+
+```python
+activity_factory, object_factory = actor.factories
+```
+
+The simplest usage example is a create wrapping a note, that looks like:
+
+```python
+activity_factory, object_factory = actor.factories
+note = object_factory.note("Hello").as_public().build()
+create = activity_factory.create(note).build()
+```
+
+The result should be the something equivalent to the json
+
+```json
+{
+  "@context": "https://www.w3.org/ns/activitystreams",
+  "type": "Create",
+  "actor": "https://domain/actor",
+  "object": {
+    "attributedTo": "https://domain/actor",
+    "type": "Note",
+    "content": "Hello",
+    "published": "2023-03-25T08:12:32Z",
+    "to": "as:Public",
+    "cc": "https://domain/followers_collection"
+  },
+  "published": "2023-03-25T08:12:32Z",
+  "to": "as:Public",
+  "cc": "https://domain/followers_collection"
+}
+```
+
+The details depend on the used actor and will likely contain superfluous elements until the creation process is improved. We can now send this activity to our outbox using
+
+```python
+await actor.send_to_outbox(create)
+```
+
+__Note__: This is different from what we did in the first example, where we used `await actor.post(inbox, create)`. The difference is that in the first example, we faked being a server, now we are actually using Client To Server.
+
+### The inbox and outbox
+
+By running
+
+```python
+inbox = await actor.inbox()
+outbox = await actor.outbox()
+```
+
+one can obtain `CollectionHelper` objects. These are meant to make it easier to interact with collection objects. In the simplest use case, one can use
+
+```python
+await inbox.next_item()
+```
+
+to get the items from the inbox one after the other. It is also possible to print a summary of all elements that have been fetched from the inbox using `await inbox.summary()`. Finally, it is possible to iterate over the inbox via
+
+```python
+async for item in inbox.iterate(max_number=3):
+    do_something(item)
+```
+
+### Proxying elements
+
+We have already seen the difference between using `post` directly to an inbox and posting to the actor's outbox using `send_to_outbox`. A similar pattern applies to fetching objects. Both of these commands often have a similar result
+
+```python
+await actor.get(object_id)
+await actor.proxy_element(object_id)
+```
+
+However, they do different things:
+
+- The first `actor.get` sends a webrequest to the server `object_id` is on and retrieves it
+- The second `actor.proxy_element` sends a request to the actor's server for the object. This request is then either answered from the server's object store or by the server fetching the object. The cache behavior is up to the server. Depending of the evolution of `proxyUrl` of an Actor, more options might be added here.
+
+As most servers don't support Moo-Auth-1, using `proxy_element` is the only way to obtain foreign objects, when using it.
+
+### Event Source
+
+The event source is demonstrated in `examples/sse.py`. First, the event source will be specified in a [FEP](https://codeberg.org/fediverse/fep) to come. It provides a way to receive updates from the server, whenever a new element is added to the inbox or outbox. The basic usage is
+
+```python
+event_source = await actor.event_source()
+async for event in event_source:
+    if event and event.data:
+        data = json.loads(event.data)
+        do_something(data)
+```
+
+If you plan on writing long running applications, the event source does not automatically reconnect, so you will need to implement this. [mechanical_bull](https://codeberg.org/helge/mechanical_bull) uses the event source in this way.
 
-setup(**setup_kwargs)
```

