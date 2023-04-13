# Comparing `tmp/bittrade_binance_websocket-0.1.7.tar.gz` & `tmp/bittrade_binance_websocket-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_binance_websocket-0.1.7.tar", max compression
+gzip compressed data, was "bittrade_binance_websocket-0.1.8.tar", max compression
```

## Comparing `bittrade_binance_websocket-0.1.7.tar` & `bittrade_binance_websocket-0.1.8.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.1.7/README.md
--rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/__init__.py
--rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/__init__.py
--rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/book_ticker.py
--rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/depth.py
--rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/message.py
--rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/subscribe.py
--rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/__init__.py
--rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0     3531 2023-03-26 22:59:27.837091 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/generic.py
--rw-r--r--   0        0        0     2622 2023-03-26 22:59:27.837264 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/http.py
--rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/private.py
--rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/private_user_stream.py
--rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/public_stream.py
--rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/reconnect.py
--rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/__init__.py
--rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/add_order.py
--rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/cancel_order.py
--rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/ping.py
--rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/request_response.py
--rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/time.py
--rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/framework/__init__.py
--rw-r--r--   0        0        0     8307 2023-04-12 10:32:29.216475 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/framework/framework.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/json.py
--rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/listen.py
--rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/__init__.py
--rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/accounts.py
--rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/contingency_type.py
--rw-r--r--   0        0        0      789 2023-04-12 10:13:14.706632 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/endpoints.py
--rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0     3790 2023-04-12 10:32:29.217898 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/framework.py
--rw-r--r--   0        0        0      465 2023-04-12 10:13:14.708202 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/loan.py
--rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/message.py
--rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/oco_list_status.py
--rw-r--r--   0        0        0     5878 2023-04-08 09:51:07.675078 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/order.py
--rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/order_status.py
--rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/permission.py
--rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/private.py
--rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/request.py
--rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/response_message.py
--rw-r--r--   0        0        0       15 2023-03-07 05:38:31.457289 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/get_time.py
--rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/listen_key.py
--rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/margin_account.py
--rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/symbol_status.py
--rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/operators/__init__.py
--rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/operators/orderbook/__init__.py
--rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/operators/stream/response_messages.py
--rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/__init__.py
--rw-r--r--   0        0        0      642 2023-04-01 04:56:33.596498 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/cancel_order.py
--rw-r--r--   0        0        0      639 2023-04-01 04:56:55.000215 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/create_order.py
--rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/current_open_orders.py
--rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/get_time.py
--rw-r--r--   0        0        0     1167 2023-03-24 09:56:30.849712 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/http_factory_decorator.py
--rw-r--r--   0        0        0     2485 2023-03-26 22:59:27.840684 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/listen_key.py
--rw-r--r--   0        0        0      830 2023-04-12 10:13:14.708641 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/margin_loan.py
--rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/query_margin_account.py
--rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/query_margin_fee_data.py
--rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/symbol_orders_cancel.py
--rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0     3824 2023-03-30 09:47:19.704651 bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/sign.py
--rw-r--r--   0        0        0     1764 2023-04-12 10:33:54.691147 bittrade_binance_websocket-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.7/setup.py
--rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.1.8/README.md
+-rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/__init__.py
+-rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/__init__.py
+-rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/book_ticker.py
+-rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/depth.py
+-rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/message.py
+-rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/__init__.py
+-rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0     3531 2023-03-26 22:59:27.837091 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2622 2023-03-26 22:59:27.837264 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/http.py
+-rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/private.py
+-rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/private_user_stream.py
+-rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/public_stream.py
+-rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/__init__.py
+-rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/add_order.py
+-rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/cancel_order.py
+-rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/ping.py
+-rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/request_response.py
+-rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/time.py
+-rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/framework/__init__.py
+-rw-r--r--   0        0        0     8470 2023-04-13 03:19:03.949497 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/framework/framework.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/json.py
+-rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/listen.py
+-rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/accounts.py
+-rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/contingency_type.py
+-rw-r--r--   0        0        0      881 2023-04-13 02:30:51.437278 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/endpoints.py
+-rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0     3990 2023-04-13 03:17:38.397874 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/framework.py
+-rw-r--r--   0        0        0      465 2023-04-12 10:13:14.708202 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/loan.py
+-rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/message.py
+-rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/oco_list_status.py
+-rw-r--r--   0        0        0     5577 2023-04-12 10:36:31.478459 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/order.py
+-rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/order_status.py
+-rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/permission.py
+-rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/private.py
+-rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/request.py
+-rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/response_message.py
+-rw-r--r--   0        0        0       15 2023-03-07 05:38:31.457289 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/get_time.py
+-rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/listen_key.py
+-rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/margin_account.py
+-rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/symbol_status.py
+-rw-r--r--   0        0        0     1112 2023-04-13 04:00:27.126562 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/trade.py
+-rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/operators/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/operators/orderbook/__init__.py
+-rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/operators/stream/response_messages.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-01 04:56:33.596498 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/cancel_order.py
+-rw-r--r--   0        0        0      639 2023-04-01 04:56:55.000215 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/create_order.py
+-rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/current_open_orders.py
+-rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/get_time.py
+-rw-r--r--   0        0        0     1167 2023-03-24 09:56:30.849712 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/http_factory_decorator.py
+-rw-r--r--   0        0        0     2485 2023-03-26 22:59:27.840684 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/listen_key.py
+-rw-r--r--   0        0        0      830 2023-04-12 10:13:14.708641 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/margin_loan.py
+-rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/query_margin_account.py
+-rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/query_margin_fee_data.py
+-rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/symbol_orders_cancel.py
+-rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0     2271 2023-04-13 07:43:16.471911 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/trade_list.py
+-rw-r--r--   0        0        0     3824 2023-03-30 09:47:19.704651 bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/sign.py
+-rw-r--r--   0        0        0     1765 2023-04-13 20:42:28.975673 bittrade_binance_websocket-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.8/setup.py
+-rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.1.8/PKG-INFO
```

### Comparing `bittrade_binance_websocket-0.1.7/README.md` & `bittrade_binance_websocket-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/book_ticker.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/depth.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/depth.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/channels/subscribe.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/channels/subscribe.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/connection_operators.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/generic.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/http.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/private.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/private_user_stream.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/private_user_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/public_stream.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/public_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/connection/reconnect.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/add_order.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/add_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/cancel_order.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/ping.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/ping.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/request_response.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/events/time.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/events/time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/framework/framework.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/framework/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     cancel_order_factory,
     cancel_symbol_orders_factory,
 )
 from bittrade_binance_websocket.rest.cancel_order import cancel_order_http_factory
 from bittrade_binance_websocket.rest.query_margin_account import (
     query_margin_account_details_http_factory,
 )
+from bittrade_binance_websocket.rest.trade_list import account_trade_list_http_factory
 from bittrade_binance_websocket.rest.query_margin_fee_data import (
     query_margin_fee_data_http_factory,
 )
 from bittrade_binance_websocket.rest.symbol_orders_cancel import (
     delete_symbol_order_http_factory,
 )
 from bittrade_binance_websocket.rest.create_order import (
@@ -171,14 +172,15 @@
         spot_trade_sockets=spot_trade_sockets,
         spot_trade_guaranteed_sockets=spot_trade_guaranteed_sockets,
         spot_order_create=spot_order_create,
         spot_order_cancel=spot_order_cancel,
         spot_symbol_orders_cancel=spot_symbol_orders_cancel,
         order_create_http=create_order_http_factory(trade_signer_http),
         order_cancel_http=cancel_order_http_factory(trade_signer_http),
+        trade_list_http=account_trade_list_http_factory(trade_signer_http),
         symbol_orders_cancel_http=symbol_orders_cancel_http,
         current_open_orders_http=open_orders_http,
         user_data_stream_messages=user_data_stream_messages,
         user_data_stream_sockets=user_data_stream_socket,
         user_data_stream_socket_bundles=user_data_stream_socket_bundles,
         public_stream_bundles=public_stream_bundles,
         public_stream_sockets=public_stream_sockets,
```

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/filters/kind.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/filters/kind.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/json.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/messages/listen.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/messages/listen.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/endpoints.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/endpoints.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,12 +7,14 @@
     ISOLATED_MARGIN_LISTEN_KEY = "/sapi/v1/userDataStream/isolated"
     LISTEN_KEY = "/api/v3/userDataStream"
     MARGIN_OPEN_ORDERS = "/sapi/v1/margin/openOrders"
     MARGIN_ORDER = "/sapi/v1/margin/order"
     MARGIN_LOAN = "/sapi/v1/margin/loan"
     MARGIN_REPAY = "/sapi/v1/margin/repay"
     SPOT_ORDER = "/api/v3/order"
+    SPOT_TRADE_LIST = "/api/v3/myTrades"
+    MARGIN_TRADE_LIST = "/sapi/v1/margin/myTrades"
     QUERY_CROSS_MARGIN_ACCOUNT_DETAILS = "/sapi/v1/margin/account"
     QUERY_ISOLATED_MARGIN_ACCOUNT_DETAILS = "/sapi/v1/margin/isolated/account"
     QUERY_ISOLATED_MARGIN_FEE_DATA = "/sapi/v1/margin/isolatedMarginData"
     QUERY_CROSS_MARGIN_FEE_DATA = "/sapi/v1/margin/crossMarginData"
     SYMBOL_PRICE_TICKER = "/api/v3/ticker/price"
```

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/enhanced_websocket.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/framework.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from elm_framework_helpers.websockets import models
 from bittrade_binance_websocket.models import UserFeedMessage
 from bittrade_binance_websocket.models.loan import AccountBorrowRequest
 from bittrade_binance_websocket.models.response_message import SpotResponseMessage
 from bittrade_binance_websocket.models.rest import margin_account
 from bittrade_binance_websocket.models.rest.listen_key import CreateListenKeyResponse
 from bittrade_binance_websocket.models.rest.symbol_price_ticker import SymbolPriceTicker
+from bittrade_binance_websocket.models.trade import TradeDataRequest, TradeDict
 from bittrade_binance_websocket.models.order import (
     OrderCancelRequest,
     SymbolOrdersCancelRequest,
     PlaceOrderRequest,
     PlaceOrderResponse,
-    MarginSymbolOrdersRequest,
     SymbolOrderResponseItem,
 )
 
 
 class BookConfig(NamedTuple):
     pair: str
     depth: int
@@ -46,14 +46,16 @@
     spot_trade_socket_messages: Observable[dict]
     spot_trade_sockets: Observable[models.EnhancedWebsocket]
     spot_trade_guaranteed_sockets: models.EnhancedWebsocketBehaviorSubject
     spot_order_create: Callable[[PlaceOrderRequest], Observable[PlaceOrderResponse]]
     spot_order_cancel: Callable[[OrderCancelRequest], Observable[dict]]
     order_create_http: Callable[[PlaceOrderRequest], Observable[PlaceOrderResponse]]
     order_cancel_http: Callable[[OrderCancelRequest], Observable[dict]]
+    order_cancel_http: Callable[[OrderCancelRequest], Observable[dict]]
+    trade_list_http: Callable[[TradeDataRequest], Observable[list[TradeDict]]]
     margin_account_borrow_http: Callable[[AccountBorrowRequest], Observable[dict]]
     margin_account_repay_http: Callable[[AccountBorrowRequest], Observable[dict]]
     spot_symbol_orders_cancel: Callable[
         [SymbolOrdersCancelRequest], Observable[SpotResponseMessage]
     ]
     symbol_orders_cancel_http: Callable[
         [SymbolOrdersCancelRequest], Observable[SpotResponseMessage]
```

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/order.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,26 +149,14 @@
         if self.is_margin:
             as_dict["isIsolated"] = "TRUE" if self.isIsolated else "FALSE"
         else:
             del as_dict["isIsolated"]
         return as_dict
 
 
-@dataclasses.dataclass
-class MarginSymbolOrdersRequest:
-    symbol: str
-    isIsolated: bool = False
-    recvWindow: Optional[int] = None
-
-    def to_dict(self):
-        as_dict = dataclasses.asdict(self)
-        as_dict["isIsolated"] = "TRUE" if self.isIsolated else "FALSE"
-        return as_dict
-
-
 class UserDataStreamOrder(TypedDict):
     E: int  # Event time
     s: str  # Symbol
     c: str  # Client order ID
     S: str  # Side
     o: str  # Order type
     f: str  # Time in force
```

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/order_status.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/order_status.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/models/rest/margin_account.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/models/rest/margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/operators/orderbook/__init__.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/operators/orderbook/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/operators/stream/response_messages.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/operators/stream/response_messages.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/cancel_order.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/create_order.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/current_open_orders.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/current_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/get_time.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/get_time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/http_factory_decorator.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/http_factory_decorator.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/listen_key.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/listen_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/margin_loan.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/margin_loan.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/query_margin_account.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/query_margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/query_margin_fee_data.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/query_margin_fee_data.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/symbol_orders_cancel.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/symbol_orders_cancel.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/rest/symbol_price_ticker.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/rest/symbol_price_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/bittrade_binance_websocket/sign.py` & `bittrade_binance_websocket-0.1.8/bittrade_binance_websocket/sign.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.1.7/pyproject.toml` & `bittrade_binance_websocket-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-binance-websocket"
-version = "0.1.7"
+version = "0.1.8"
 description = "Reactive Websocket for Binance"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 license = "MIT"
 classifiers = [
@@ -50,14 +50,15 @@
 
 
 
 
 
 
 
+
 
 
 
 
 
 [tool.poetry.group.rich.dependencies]
 fire = "^0.5.0"
```

### Comparing `bittrade_binance_websocket-0.1.7/setup.py` & `bittrade_binance_websocket-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.4.2,<2.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'bittrade-binance-websocket',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Reactive Websocket for Binance',
     'long_description': '# Binance Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff \n- Respond to ping\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_huobi_websocket\').addHandler(logging.StreamHandler())\n```\n\nIn addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`\n\nTo view a full, timestamped history of the socket exchanges use\n\n```\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nThis means that you\'ll need to implement the signature token yourself. The library never has access to your API secret.\n\nSee `examples/sign.py` for an example of implementation but it is generally as simple as:\n\n```python\nauthenticated_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n# Development guidelines\n\n## `*_http` methods\n\nREST functions over http should be suffixed with `_http` e.g. `get_book_http`.\nThey should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.\n\nWhere possible models should be defined to describe the *raw* result and *parsed result* if available/useful.\n\nReactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.\n\nAny operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-binance-websocket',
```

### Comparing `bittrade_binance_websocket-0.1.7/PKG-INFO` & `bittrade_binance_websocket-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-binance-websocket
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reactive Websocket for Binance
 Home-page: https://github.com/TechSpaceAsia/bittrade-binance-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

