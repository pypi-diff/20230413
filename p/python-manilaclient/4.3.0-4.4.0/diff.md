# Comparing `tmp/python-manilaclient-4.3.0.tar.gz` & `tmp/python-manilaclient-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-manilaclient-4.3.0.tar", last modified: Fri Feb 17 12:50:02 2023, max compression
+gzip compressed data, was "python-manilaclient-4.4.0.tar", last modified: Thu Apr 13 10:17:23 2023, max compression
```

## Comparing `python-manilaclient-4.3.0.tar` & `python-manilaclient-4.4.0.tar`

### file list

```diff
@@ -1,442 +1,444 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7070 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32302 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/HACKING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/.gitkeep
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/cli/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/osc/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/functional-tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/doc/source/user/shell.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/etc/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/etc/manilaclient/README.manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/etc/oslo-config-generator/manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.000640 python-manilaclient-4.3.0/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18067 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.004640 python-manilaclient-4.3.0/manilaclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.008640 python-manilaclient-4.3.0/manilaclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53048 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27489 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29068 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/osc/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31317 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.008640 python-manilaclient-4.3.0/manilaclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    87123 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_listing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshots_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.012640 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.016639 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46247 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19607 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67674 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9753 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43220 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_functional_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.016639 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.020639 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fake_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46114 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7487 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   156971 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v1/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v1/shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.024639 python-manilaclient-4.3.0/manilaclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12841 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/manilaclient/v2/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30069 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   216521 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/manilaclient/v2/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/playbooks/python-manilaclient-functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/python_manilaclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20135 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10116 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-17 12:50:01.000000 python-manilaclient-4.3.0/python_manilaclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.028639 python-manilaclient-4.3.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/rally-jobs/rally-manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/rally-jobs/rally-manila.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:01.996641 python-manilaclient-4.3.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11142 2023-02-17 12:50:02.044638 python-manilaclient-4.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/tools/manila.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 12:50:02.040638 python-manilaclient-4.3.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-02-17 12:49:02.000000 python-manilaclient-4.3.0/zuul.d/python-manilaclient-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7111 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32493 2023-04-13 10:17:22.000000 python-manilaclient-4.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/HACKING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/.gitkeep
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/cli/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/osc/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/functional-tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/user/shell.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/etc/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/etc/manilaclient/README.manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/etc/oslo-config-generator/manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18067 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.383991 python-manilaclient-4.4.0/manilaclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53048 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27394 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29068 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31317 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.383991 python-manilaclient-4.4.0/manilaclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.391991 python-manilaclient-4.4.0/manilaclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    87123 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_listing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshots_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.403992 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46247 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19607 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67674 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9753 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43220 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_functional_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.403992 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.411992 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fake_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46114 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7487 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   156971 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.415992 python-manilaclient-4.4.0/manilaclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.415992 python-manilaclient-4.4.0/manilaclient/v1/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/manilaclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12841 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/manilaclient/v2/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30069 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   216521 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.427993 python-manilaclient-4.4.0/python_manilaclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20305 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10116 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.427993 python-manilaclient-4.4.0/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/rally-jobs/rally-manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/rally-jobs/rally-manila.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11142 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/tools/manila.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/zuul.d/python-manilaclient-jobs.yaml
```

### Comparing `python-manilaclient-4.3.0/AUTHORS` & `python-manilaclient-4.4.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 devin <genghang888@gmail.com>
 dineshbhor <dinesh.bhor@nttdata.com>
 drngsl <drngsl@qq.com>
 e <liuyamin@fiberhome.com>
 gugug <gu.jin@99cloud.net>
 haixin <653186640@qq.com>
 haixin <haixin@inspur.com>
+hassanasghar <hassanasghar666@gmail.com>
 houming-wang <houming.wang@easystack.cn>
 howardlee <lihongweibj@inspur.com>
 iswarya_vakati <v.iswarya@nectechnologies.in>
 jacky06 <zhang.min@99cloud.net>
 ji-xuepeng <ji.xuepeng@zte.com.cn>
 junboli <junbo85.li@gmail.com>
 kafilat-adeleke <adelekekafilatadenike@gmail.com>
```

### Comparing `python-manilaclient-4.3.0/CONTRIBUTING.rst` & `python-manilaclient-4.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/ChangeLog` & `python-manilaclient-4.4.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+4.4.0
+-----
+
+* Fix share network create command with the AZ option
+* Use suitable api version for OSC
+* Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
+* Update .gitreview for stable/2023.1
+
 4.3.0
 -----
 
 * Add quiesce\_wait\_time for replica promote
 * Metadata for Share Snapshots
 * Drop duplicate tox config
 * Fix tox4 errors
```

### Comparing `python-manilaclient-4.3.0/HACKING` & `python-manilaclient-4.4.0/HACKING`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/LICENSE` & `python-manilaclient-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/PKG-INFO` & `python-manilaclient-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.3.0
+Version: 4.4.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.3.0/README.rst` & `python-manilaclient-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/Makefile` & `python-manilaclient-4.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/cli/osc/v2/index.rst` & `python-manilaclient-4.4.0/doc/source/cli/osc/v2/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/cli/osc_plugin_cli.rst` & `python-manilaclient-4.4.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/conf.py` & `python-manilaclient-4.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/contributor/contributing.rst` & `python-manilaclient-4.4.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/contributor/functional-tests.rst` & `python-manilaclient-4.4.0/doc/source/contributor/functional-tests.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/index.rst` & `python-manilaclient-4.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/user/api.rst` & `python-manilaclient-4.4.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/doc/source/user/shell.rst` & `python-manilaclient-4.4.0/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/__init__.py` & `python-manilaclient-4.4.0/manilaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/api_versions.py` & `python-manilaclient-4.4.0/manilaclient/api_versions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/base.py` & `python-manilaclient-4.4.0/manilaclient/base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/client.py` & `python-manilaclient-4.4.0/manilaclient/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/_i18n.py` & `python-manilaclient-4.4.0/manilaclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/apiclient/exceptions.py` & `python-manilaclient-4.4.0/manilaclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/apiclient/utils.py` & `python-manilaclient-4.4.0/manilaclient/common/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/cliutils.py` & `python-manilaclient-4.4.0/manilaclient/common/cliutils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/constants.py` & `python-manilaclient-4.4.0/manilaclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/common/httpclient.py` & `python-manilaclient-4.4.0/manilaclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/config.py` & `python-manilaclient-4.4.0/manilaclient/config.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/exceptions.py` & `python-manilaclient-4.4.0/manilaclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/extension.py` & `python-manilaclient-4.4.0/manilaclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/plugin.py` & `python-manilaclient-4.4.0/manilaclient/osc/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """OpenStackClient plugin for the Shared File System Service."""
 
 import logging
 
 from osc_lib import utils
 
 from manilaclient import api_versions
+from manilaclient import client
 from manilaclient.common import constants
 from manilaclient import exceptions
 
 LOG = logging.getLogger(__name__)
 
 API_NAME = 'share'
 API_VERSION_OPTION = 'os_share_api_version'
@@ -56,43 +57,50 @@
     return service_type, url
 
 
 def make_client(instance):
     """Returns a shared file system service client."""
     requested_api_version = instance._api_version[API_NAME]
 
-    shared_file_system_client = utils.get_client_class(
-        API_NAME, requested_api_version, API_VERSIONS)
+    service_type, manila_endpoint_url = _get_manila_url_from_service_catalog(
+        instance)
+    instance.setup_auth()
+    debugging_enabled = instance._cli_options.debug
+
+    client_args = dict(session=instance.session,
+                       service_catalog_url=manila_endpoint_url,
+                       endpoint_type=instance.interface,
+                       region_name=instance.region_name,
+                       service_type=service_type,
+                       auth=instance.auth,
+                       http_log_debug=debugging_enabled,
+                       cacert=instance.cacert,
+                       cert=instance.cert,
+                       insecure=not instance.verify)
 
     # Cast the API version into an object for further processing
     requested_api_version = api_versions.APIVersion(
         version_str=requested_api_version)
 
+    max_version = api_versions.APIVersion(api_versions.MAX_VERSION)
+    client_args.update(dict(api_version=max_version))
+    temp_client = client.Client(max_version, **client_args)
+    discovered_version = api_versions.discover_version(temp_client,
+                                                       requested_api_version)
+
+    shared_file_system_client = utils.get_client_class(
+        API_NAME, discovered_version.get_string(), API_VERSIONS)
+
     LOG.debug('Instantiating Shared File System (share) client: %s',
               shared_file_system_client)
     LOG.debug('Shared File System API version: %s',
-              requested_api_version)
+              discovered_version)
 
-    service_type, manila_endpoint_url = _get_manila_url_from_service_catalog(
-        instance)
-
-    instance.setup_auth()
-    debugging_enabled = instance._cli_options.debug
-    client = shared_file_system_client(session=instance.session,
-                                       service_catalog_url=manila_endpoint_url,
-                                       endpoint_type=instance.interface,
-                                       region_name=instance.region_name,
-                                       service_type=service_type,
-                                       auth=instance.auth,
-                                       http_log_debug=debugging_enabled,
-                                       api_version=requested_api_version,
-                                       cacert=instance.cacert,
-                                       cert=instance.cert,
-                                       insecure=not instance.verify)
-    return client
+    client_args.update(dict(api_version=discovered_version))
+    return shared_file_system_client(**client_args)
 
 
 def build_option_parser(parser):
     """Hook to add global options."""
     default_api_version = utils.env('OS_SHARE_API_VERSION') or LATEST_VERSION
     parser.add_argument(
         '--os-share-api-version',
```

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/utils.py` & `python-manilaclient-4.4.0/manilaclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/messages.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/quotas.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/security_services.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/services.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_access_rules.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_type_access.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_group_types.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_groups.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_instances.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_limits.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_networks.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,17 +291,15 @@
         availability_zone = None
         if (parsed_args.availability_zone and
                 share_client.api_version < api_versions.APIVersion("2.51")):
             raise exceptions.CommandError(
                 "Availability zone can be specified only with manila API "
                 "version >= 2.51")
         elif parsed_args.availability_zone:
-            availability_zone = oscutils.find_resource(
-                share_client.availability_zones,
-                parsed_args.availability_zone).name
+            availability_zone = parsed_args.availability_zone
 
         share_network = share_client.share_networks.create(
             name=parsed_args.name,
             description=parsed_args.description,
             neutron_net_id=parsed_args.neutron_net_id,
             neutron_subnet_id=parsed_args.neutron_subnet_id,
             availability_zone=availability_zone,
```

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_pools.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_servers.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshot_instances.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_type_access.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/osc/v2/share_types.py` & `python-manilaclient-4.4.0/manilaclient/osc/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/shell.py` & `python-manilaclient-4.4.0/manilaclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/base.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/client.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/exceptions.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/base.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_messages.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_access_rules.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_group_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_limits.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_networks.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_pools.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_share_types.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/osc/test_shares_group_type.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_common.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_common.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_limits.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_messages.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_quotas.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_scheduler_stats.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_security_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_networks.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_servers.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_share_types.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_listing.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_listing.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_shares_metadata.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_metadata.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/test_snapshots_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshots_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/functional/utils.py` & `python-manilaclient-4.4.0/manilaclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/common/test_httpclient.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/fakes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_fakes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/osc_utils.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/fakes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_messages.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_quotas.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_security_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_groups.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_instances.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_limits.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_networks.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_pools.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_servers.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/test_api_versions.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/test_base.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/test_client.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/test_functional_utils.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/test_functional_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/test_shell.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/utils.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_limits.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quota_classes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_quotas.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_scheduler_stats.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_security_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_networks.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_servers.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_share_types.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v1/test_shares.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fake_clients.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fake_clients.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/fakes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_client.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_limits.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_messages.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quota_classes.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_quotas.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_scheduler_stats.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_security_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_services.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_group_types.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_groups.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_instances.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_networks.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_servers.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shares.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_shell.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_type_access.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/tests/unit/v2/test_types.py` & `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/utils.py` & `python-manilaclient-4.4.0/manilaclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/__init__.py` & `python-manilaclient-4.4.0/manilaclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/client.py` & `python-manilaclient-4.4.0/manilaclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/contrib/list_extensions.py` & `python-manilaclient-4.4.0/manilaclient/v1/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/limits.py` & `python-manilaclient-4.4.0/manilaclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/quota_classes.py` & `python-manilaclient-4.4.0/manilaclient/v1/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/quotas.py` & `python-manilaclient-4.4.0/manilaclient/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/scheduler_stats.py` & `python-manilaclient-4.4.0/manilaclient/v1/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/security_services.py` & `python-manilaclient-4.4.0/manilaclient/v1/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/services.py` & `python-manilaclient-4.4.0/manilaclient/v1/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/share_networks.py` & `python-manilaclient-4.4.0/manilaclient/v1/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/share_servers.py` & `python-manilaclient-4.4.0/manilaclient/v1/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/v1/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/share_type_access.py` & `python-manilaclient-4.4.0/manilaclient/v1/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/share_types.py` & `python-manilaclient-4.4.0/manilaclient/v1/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v1/shares.py` & `python-manilaclient-4.4.0/manilaclient/v1/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/__init__.py` & `python-manilaclient-4.4.0/manilaclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/availability_zones.py` & `python-manilaclient-4.4.0/manilaclient/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/client.py` & `python-manilaclient-4.4.0/manilaclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/contrib/list_extensions.py` & `python-manilaclient-4.4.0/manilaclient/v2/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/limits.py` & `python-manilaclient-4.4.0/manilaclient/v2/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/messages.py` & `python-manilaclient-4.4.0/manilaclient/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/quota_classes.py` & `python-manilaclient-4.4.0/manilaclient/v2/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/quotas.py` & `python-manilaclient-4.4.0/manilaclient/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/scheduler_stats.py` & `python-manilaclient-4.4.0/manilaclient/v2/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/security_services.py` & `python-manilaclient-4.4.0/manilaclient/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/services.py` & `python-manilaclient-4.4.0/manilaclient/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_access_rules.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_group_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_group_type_access.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_group_types.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_groups.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_instances.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_network_subnets.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_networks.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_replica_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_replicas.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_servers.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_snapshot_instances.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_snapshots.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_type_access.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/share_types.py` & `python-manilaclient-4.4.0/manilaclient/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/shares.py` & `python-manilaclient-4.4.0/manilaclient/v2/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/manilaclient/v2/shell.py` & `python-manilaclient-4.4.0/manilaclient/v2/shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/python_manilaclient.egg-info/PKG-INFO` & `python-manilaclient-4.4.0/python_manilaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.3.0
+Version: 4.4.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.3.0/python_manilaclient.egg-info/SOURCES.txt` & `python-manilaclient-4.4.0/python_manilaclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,16 @@
 releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
 releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
 releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
 releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
 releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
 releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
 releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
+releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
+releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
 releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
 releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
 releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
 releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
 releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
 releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
 releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
```

### Comparing `python-manilaclient-4.3.0/python_manilaclient.egg-info/entry_points.txt` & `python-manilaclient-4.4.0/python_manilaclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/rally-jobs/rally-manila-no-ss.yaml` & `python-manilaclient-4.4.0/rally-jobs/rally-manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/rally-jobs/rally-manila.yaml` & `python-manilaclient-4.4.0/rally-jobs/rally-manila.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml` & `python-manilaclient-4.4.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/releasenotes/source/conf.py` & `python-manilaclient-4.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/requirements.txt` & `python-manilaclient-4.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/roles/populate-manilaclient-config/README.rst` & `python-manilaclient-4.4.0/roles/populate-manilaclient-config/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/roles/populate-manilaclient-config/tasks/main.yaml` & `python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/run_tests.sh` & `python-manilaclient-4.4.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/setup.cfg` & `python-manilaclient-4.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/setup.py` & `python-manilaclient-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.3.0/tox.ini` & `python-manilaclient-4.4.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 basepython = python3
 usedevelop = true
 setenv = VIRTUAL_ENV={envdir}
          OS_STDOUT_CAPTURE=1
          OS_STDERR_CAPTURE=1
          PYTHONDONTWRITEBYTECODE=1
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/test-requirements.txt
 commands =
   stestr run {posargs}
   stestr slowest
 
 [testenv:debug]
 commands = oslo_debug_helper -t manilaclient/tests {posargs}
@@ -29,15 +29,15 @@
   flake8
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
   rm -rf doc/build
   sphinx-build -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
@@ -46,15 +46,15 @@
   make
 commands =
   sphinx-build  -W -b latex doc/source doc/build/pdf
   make -C doc/build/pdf
 
 [testenv:releasenotes]
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
     rm -rf releasenotes/build
     sphinx-build -a -E -W -d releasenotes/build/doctrees \
          -b html releasenotes/source releasenotes/build/html
```

### Comparing `python-manilaclient-4.3.0/zuul.d/python-manilaclient-jobs.yaml` & `python-manilaclient-4.4.0/zuul.d/python-manilaclient-jobs.yaml`

 * *Files identical despite different names*

