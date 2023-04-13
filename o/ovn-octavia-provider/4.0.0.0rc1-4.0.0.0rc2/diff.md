# Comparing `tmp/ovn-octavia-provider-4.0.0.0rc1.tar.gz` & `tmp/ovn-octavia-provider-4.0.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovn-octavia-provider-4.0.0.0rc1.tar", last modified: Thu Mar  2 11:49:41 2023, max compression
+gzip compressed data, was "ovn-octavia-provider-4.0.0.0rc2.tar", last modified: Fri Mar 17 15:42:18 2023, max compression
```

## Comparing `ovn-octavia-provider-4.0.0.0rc1.tar` & `ovn-octavia-provider-4.0.0.0rc2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.325296 ovn-octavia-provider-4.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3092 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7696 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-02 11:49:41.325296 ovn-octavia-provider-4.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.309296 ovn-octavia-provider-4.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4164 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/devstack/local.conf.sample
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.309296 ovn-octavia-provider-4.0.0.0rc1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12963 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/admin/driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/configuration/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/contributor/loadbalancer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/doc/source/pdf-index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.305296 ovn-octavia-provider-4.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/etc/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/etc/octavia/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/etc/octavia/conf.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/etc/octavia/conf.d/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/etc/oslo-config-generator/ovn.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6277 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26047 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/event.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6906 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   135949 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9761 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/ovsdb/impl_idl_ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/ovsdb/ovsdb_monitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45439 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10201 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19381 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7050 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_integration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9964 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11807 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/hacking/test_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6410 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.317296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/schemas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26568 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51697 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   216550 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.313296 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-03-02 11:49:41.000000 ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/playbooks/configure_functional_job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/playbooks/post_functional_job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/playbooks/run_functional_job.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.309296 ovn-octavia-provider-4.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/add-hm-support-2c6729d8816125a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/add-sctp-support-bedfed905e1f5a58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-e890961ed94c146e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/new-repository-for-ovn-octavia-provider-driver-dd81c4414c529c4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/ovn-octavia-provider-driver-multiple-protocols-4a93e184b8f374c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/notes/support-member-create-without-subnetid-0b4e3aa6ac453f28.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8629 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.309296 ovn-octavia-provider-4.0.0.0rc1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.321296 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/roles/setup_logdir/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-03-02 11:49:41.325296 ovn-octavia-provider-4.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.325296 ovn-octavia-provider-4.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1737 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/tools/check_unit_test_structure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1587 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      792 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/tools/generate_config_file_samples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      658 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/tools/pip_install_src_modules.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5584 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:49:41.325296 ovn-octavia-provider-4.0.0.0rc1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6677 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2023-03-02 11:49:02.000000 ovn-octavia-provider-4.0.0.0rc1/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3092 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7990 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4164 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/local.conf.sample
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12963 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/loadbalancer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/pdf-index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/conf.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/conf.d/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/oslo-config-generator/ovn.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6277 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4219 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26138 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/event.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6906 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   136426 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9761 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/impl_idl_ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/ovsdb_monitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51550 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10201 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21679 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7050 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_integration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9964 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11807 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/test_checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6410 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26568 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52034 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   218326 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/configure_functional_job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/post_functional_job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/run_functional_job.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/add-hm-support-2c6729d8816125a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/add-sctp-support-bedfed905e1f5a58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/drop-python-3-6-and-3-7-e890961ed94c146e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/new-repository-for-ovn-octavia-provider-driver-dd81c4414c529c4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/ovn-octavia-provider-driver-multiple-protocols-4a93e184b8f374c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/support-member-create-without-subnetid-0b4e3aa6ac453f28.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8629 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1737 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/check_unit_test_structure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1587 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      792 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/generate_config_file_samples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      658 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/pip_install_src_modules.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5584 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6677 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/zuul.d/project.yaml
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/.pylintrc` & `ovn-octavia-provider-4.0.0.0rc2/.pylintrc`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/AUTHORS` & `ovn-octavia-provider-4.0.0.0rc2/AUTHORS`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/CONTRIBUTING.rst` & `ovn-octavia-provider-4.0.0.0rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ChangeLog` & `ovn-octavia-provider-4.0.0.0rc2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+4.0.0.0rc2
+----------
+
+* Add new FTs for health monitoring basic operations
+* Remove HM uuiid from LB external\_ids when the HM's pool is deleted
+* Fix broken pep8 jobs due to bandit 1.7.5 updated version
+* Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
+* Update .gitreview for stable/2023.1
+
 4.0.0.0rc1
 ----------
 
 * Reset member provisioning status to NO\_MONITOR when a HM is deleted
 * Ensure HM also apply to FIPs associated to LB VIPs
 * Avoid use of ovn metadata port IP for HM checks
 * Remove LB from LS belonging to provider networks
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/HACKING.rst` & `ovn-octavia-provider-4.0.0.0rc2/HACKING.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/LICENSE` & `ovn-octavia-provider-4.0.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/PKG-INFO` & `ovn-octavia-provider-4.0.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-octavia-provider
-Version: 4.0.0.0rc1
+Version: 4.0.0.0rc2
 Summary: OpenStack Octavia integration with OVN
 Home-page: https://docs.openstack.org/ovn-octavia-provider/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================================
         ovn-octavia-provider - OVN Provider driver for Octavia LoadBalancer
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/README.rst` & `ovn-octavia-provider-4.0.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/devstack/local.conf.sample` & `ovn-octavia-provider-4.0.0.0rc2/devstack/local.conf.sample`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/devstack/plugin.sh` & `ovn-octavia-provider-4.0.0.0rc2/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/doc/source/admin/driver.rst` & `ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/driver.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/doc/source/conf.py` & `ovn-octavia-provider-4.0.0.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/doc/source/contributor/loadbalancer.rst` & `ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/loadbalancer.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/doc/source/index.rst` & `ovn-octavia-provider-4.0.0.0rc2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/doc/source/pdf-index.rst` & `ovn-octavia-provider-4.0.0.0rc2/doc/source/pdf-index.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/agent.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/clients.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/clients.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/config.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/config.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/constants.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,7 +105,10 @@
     constants.LB_ALGORITHM_SOURCE_IP: ["ip_src", "ip_dst"],
     None: ["ip_src", "ip_dst", "tp_src", "tp_dst"],
 }
 
 # HM events status
 HM_EVENT_MEMBER_PORT_ONLINE = ['online']
 HM_EVENT_MEMBER_PORT_OFFLINE = ['offline']
+
+# max timeout for request
+MAX_TIMEOUT_REQUEST = 5
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/exceptions.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/common/utils.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/utils.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/driver.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,17 @@
                    'info': request_info}
         self._ovn_helper.add_request(request)
         if pool.healthmonitor is not None and not isinstance(
                 pool.healthmonitor, o_datamodels.UnsetType):
             self.health_monitor_create(pool.healthmonitor)
 
     def pool_delete(self, pool):
+        if pool.healthmonitor:
+            self.health_monitor_delete(pool.healthmonitor)
+
         for member in pool.members:
             self.member_delete(member)
 
         request_info = {'id': pool.pool_id,
                         'protocol': pool.protocol,
                         'loadbalancer_id': pool.loadbalancer_id}
         request = {'type': ovn_const.REQ_TYPE_POOL_DELETE,
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/event.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/event.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/hacking/checks.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/helper.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,16 @@
         if cert_file:
             Stream.ssl_set_certificate_file(cert_file)
 
         if ca_cert_file:
             Stream.ssl_set_ca_cert_file(ca_cert_file)
 
     def shutdown(self):
-        self.requests.put({'type': ovn_const.REQ_TYPE_EXIT})
+        self.requests.put({'type': ovn_const.REQ_TYPE_EXIT},
+                          timeout=ovn_const.MAX_TIMEOUT_REQUEST)
         self.helper_thread.join()
         self.ovn_nbdb.stop()
         del self.ovn_nbdb_api
 
     @staticmethod
     def _map_val(row, col, key):
         # If the row doesnt exist, RowNotFound is raised by the _map_val
@@ -385,15 +386,20 @@
 
     def _find_lb_in_table(self, lb, table):
         return self.ovn_nbdb_api.find_lb_in_table(
             lb, table).execute(check_error=True)
 
     def request_handler(self):
         while True:
-            request = self.requests.get()
+            try:
+                request = self.requests.get(
+                    timeout=ovn_const.MAX_TIMEOUT_REQUEST)
+            except queue.Empty:
+                continue
+
             request_type = request['type']
             if request_type == ovn_const.REQ_TYPE_EXIT:
                 break
 
             request_handler = self._lb_request_func_maps.get(request_type)
             try:
                 if request_handler:
@@ -410,15 +416,15 @@
                 # should be cleaned-up
             except Exception:
                 # If any unexpected exception happens we don't want the
                 # notify_loop to exit.
                 LOG.exception('Unexpected exception in request_handler')
 
     def add_request(self, req):
-        self.requests.put(req)
+        self.requests.put(req, timeout=ovn_const.MAX_TIMEOUT_REQUEST)
 
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(
             driver_exceptions.UpdateStatusError),
         wait=tenacity.wait_exponential(max=75),
         stop=tenacity.stop_after_attempt(15),
         reraise=True)
@@ -2767,23 +2773,30 @@
         commands.append(
             self.ovn_nbdb_api.db_clear('Load_Balancer', ovn_lb.uuid,
                                        'ip_port_mappings'))
         for lbhc in lbhcs:
             commands.append(
                 self.ovn_nbdb_api.db_remove('Load_Balancer', ovn_lb.uuid,
                                             'health_check', lbhc.uuid))
-        commands.append(
-            self.ovn_nbdb_api.db_set(
-                'Load_Balancer', ovn_lb.uuid,
-                ('external_ids', {ovn_const.LB_EXT_IDS_HMS_KEY:
-                                  jsonutils.dumps(hms_key)})))
-        for lbhc in lbhcs:
             commands.append(
                 self.ovn_nbdb_api.db_destroy('Load_Balancer_Health_Check',
                                              lbhc.uuid))
+
+        if hms_key:
+            commands.append(
+                self.ovn_nbdb_api.db_set(
+                    'Load_Balancer', ovn_lb.uuid,
+                    ('external_ids', {
+                        ovn_const.LB_EXT_IDS_HMS_KEY:
+                            jsonutils.dumps(hms_key)})))
+        else:
+            commands.append(
+                self.ovn_nbdb_api.db_remove(
+                    'Load_Balancer', ovn_lb.uuid,
+                    'external_ids', (ovn_const.LB_EXT_IDS_HMS_KEY)))
         self._execute_commands(commands)
 
         # Delete the hm port if not in use by other health monitors
         for subnet in member_subnets:
             self._clean_up_hm_port(subnet)
 
         status = {
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/i18n.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/i18n.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/ovsdb/impl_idl_ovn.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/impl_idl_ovn.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/ovsdb/ovsdb_monitor.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/ovsdb_monitor.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/base.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -155,14 +155,22 @@
         m_member.pool_id = pool_id
         if subnet_id:
             m_member.subnet_id = subnet_id
         m_member.address = address
         m_member.admin_state_up = admin_state_up
         return m_member
 
+    def _create_hm_model(self, pool_id, name, delay, timeout, max_retries,
+                         hm_type, max_retries_down=3, admin_state_up=True):
+        return octavia_data_model.HealthMonitor(
+            admin_state_up=admin_state_up, delay=delay,
+            max_retries=max_retries, max_retries_down=max_retries_down,
+            healthmonitor_id=uuidutils.generate_uuid(),
+            name=name, pool_id=pool_id, type=hm_type, timeout=timeout)
+
     def _create_listener_model(self, loadbalancer_id, pool_id=None,
                                protocol_port=80, protocol=None,
                                admin_state_up=True):
         m_listener = octavia_data_model.Listener()
         if protocol:
             m_listener.protocol = protocol
         else:
@@ -612,15 +620,20 @@
                             if fixed_ip['subnet_id'] == m.subnet_id:
                                 ex = external_ids[
                                     ovn_const.LB_EXT_IDS_LS_REFS_KEY]
                                 act = ex.get(
                                     'neutron-%s' % port['network_id'], 0)
                                 ex['neutron-%s' % port['network_id']] = act + 1
                                 break
-                member_status[m.member_id] = o_constants.NO_MONITOR
+                if p.healthmonitor:
+                    member_status[m.member_id] = o_constants.ONLINE
+                    external_ids[ovn_const.LB_EXT_IDS_HMS_KEY] = \
+                        jsonutils.dumps([p.healthmonitor.healthmonitor_id])
+                else:
+                    member_status[m.member_id] = o_constants.NO_MONITOR
             pool_key = 'pool_' + p.pool_id
             if not p.admin_state_up:
                 pool_key += ':D'
             external_ids[pool_key] = p_members
             pool_info[p.pool_id] = p_members
             if member_status:
                 external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = member_status
@@ -727,25 +740,44 @@
     def _delete_pool_and_validate(self, lb_data, pool_name,
                                   listener_id=None):
         self._o_driver_lib.update_loadbalancer_status.reset_mock()
         p = self._get_pool_from_lb_data(lb_data, pool_name=pool_name)
         self.ovn_driver.pool_delete(p)
         lb_data['pools'].remove(p)
         expected_status = []
-        # When a pool is deleted and if it has any members, there are
-        # expected to be deleted.
+
+        # When a pool is deleted and if it has a health_monitor associated or
+        # any members, there are expected to be deleted.
+        if p.healthmonitor:
+            member_statuses = [{"id": m.member_id,
+                                "provisioning_status": o_constants.ACTIVE,
+                                "operating_status": o_constants.NO_MONITOR}
+                               for m in p.members]
+            expected_status.append(
+                {'healthmonitors': [{
+                    "id": p.healthmonitor.healthmonitor_id,
+                    "provisioning_status": o_constants.DELETED,
+                    "operating_status": o_constants.NO_MONITOR}],
+                 'members': member_statuses,
+                 'loadbalancers': [{
+                     "id": p.loadbalancer_id,
+                     "provisioning_status": o_constants.ACTIVE}],
+                 'pools': [{"id": p.pool_id,
+                            "provisioning_status": o_constants.ACTIVE}],
+                 'listeners': []})
         for m in p.members:
             expected_status.append(
                 {'pools': [{"id": p.pool_id,
                             "provisioning_status": o_constants.ACTIVE,
                             "operating_status": o_constants.ONLINE}],
                  'members': [{"id": m.member_id,
-                              "provisioning_status": "DELETED"}],
-                 'loadbalancers': [{"id": p.loadbalancer_id,
-                                    "provisioning_status": "ACTIVE"}],
+                              "provisioning_status": o_constants.DELETED}],
+                 'loadbalancers': [{
+                     "id": p.loadbalancer_id,
+                     "provisioning_status": o_constants.ACTIVE}],
                  'listeners': []})
             self._update_ls_refs(
                 lb_data, self._local_net_cache[m.subnet_id], add_ref=False)
         if p.members:
             # If Pool has members, delete all members of the pool. When the
             # last member is processed set Operating status of Pool as Offline
             expected_status[-1]['pools'][0][
@@ -922,14 +954,112 @@
             'loadbalancers': [{"id": pool.loadbalancer_id,
                                "provisioning_status": "ACTIVE"}],
             'listeners': []}
 
         self._update_ls_refs(lb_data, network_id, add_ref=False)
         self._wait_for_status_and_validate(lb_data, [expected_status])
 
+    def _create_hm_and_validate(self, lb_data, pool_id, name, delay, timeout,
+                                max_retries, hm_type):
+        self._o_driver_lib.update_loadbalancer_status.reset_mock()
+        pool = self._get_pool_from_lb_data(lb_data, pool_id=pool_id)
+        pool_status = {'id': pool.pool_id,
+                       'provisioning_status': o_constants.ACTIVE,
+                       'operating_status': o_constants.ONLINE}
+
+        m_hm = self._create_hm_model(pool.pool_id, name, delay, timeout,
+                                     max_retries, hm_type)
+        pool.healthmonitor = m_hm
+
+        self.ovn_driver.health_monitor_create(m_hm)
+        pool_listeners = self._get_pool_listeners(lb_data, pool_id)
+        expected_listener_status = [
+            {'id': listener.listener_id,
+             'provisioning_status': o_constants.ACTIVE}
+            for listener in pool_listeners]
+
+        expected_member_status = [
+            {'id': m.member_id, 'provisioning_status': o_constants.ACTIVE,
+             'operating_status': o_constants.ONLINE}
+            for m in pool.members]
+
+        expected_hm_status = {'id': m_hm.healthmonitor_id,
+                              'provisioning_status': o_constants.ACTIVE,
+                              'operating_status': o_constants.ONLINE}
+        expected_status = {
+            'pools': [pool_status],
+            'members': expected_member_status,
+            'loadbalancers': [{'id': pool.loadbalancer_id,
+                               'provisioning_status': o_constants.ACTIVE}],
+            'listeners': expected_listener_status,
+            'healthmonitors': [expected_hm_status]
+        }
+        self._wait_for_status_and_validate(lb_data, [expected_status])
+
+    def _update_hm_and_validate(self, lb_data, pool_id, admin_state_up=None):
+        self._o_driver_lib.update_loadbalancer_status.reset_mock()
+        pool = self._get_pool_from_lb_data(lb_data, pool_id=pool_id)
+        hm = pool.healthmonitor
+        old_hm = copy.deepcopy(hm)
+
+        operating_status = o_constants.ONLINE
+        if admin_state_up is not None:
+            hm.admin_state_up = admin_state_up
+            if not admin_state_up:
+                operating_status = o_constants.OFFLINE
+
+        pool_status = {"id": pool.pool_id,
+                       "provisioning_status": o_constants.ACTIVE}
+
+        self.ovn_driver.health_monitor_update(old_hm, hm)
+
+        expected_hm_status = {'id': hm.healthmonitor_id,
+                              'provisioning_status': o_constants.ACTIVE,
+                              'operating_status': operating_status}
+
+        expected_status = {
+            'pools': [pool_status],
+            'loadbalancers': [{'id': pool.loadbalancer_id,
+                               'provisioning_status': o_constants.ACTIVE}],
+            'healthmonitors': [expected_hm_status]}
+
+        self._wait_for_status_and_validate(lb_data, [expected_status])
+
+    def _delete_hm_and_validate(self, lb_data, pool_id):
+        self._o_driver_lib.update_loadbalancer_status.reset_mock()
+        pool = self._get_pool_from_lb_data(lb_data, pool_id=pool_id)
+        hm = pool.healthmonitor
+        pool.healthmonitor = None
+        pool_status = {'id': pool.pool_id,
+                       'provisioning_status': o_constants.ACTIVE}
+        pool_listeners = self._get_pool_listeners(lb_data, pool_id)
+        expected_listener_status = [
+            {'id': listener.listener_id,
+             'provisioning_status': o_constants.ACTIVE}
+            for listener in pool_listeners]
+
+        self.ovn_driver.health_monitor_delete(hm)
+
+        expected_hm_status = {'id': hm.healthmonitor_id,
+                              'provisioning_status': o_constants.DELETED,
+                              'operating_status': o_constants.NO_MONITOR}
+        expected_member_status = [
+            {'id': m.member_id, 'provisioning_status': o_constants.ACTIVE,
+             'operating_status': o_constants.NO_MONITOR}
+            for m in pool.members]
+        expected_status = {
+            'pools': [pool_status],
+            'loadbalancers': [{"id": pool.loadbalancer_id,
+                               "provisioning_status": o_constants.ACTIVE}],
+            'members': expected_member_status,
+            'listeners': expected_listener_status,
+            'healthmonitors': [expected_hm_status]}
+
+        self._wait_for_status_and_validate(lb_data, [expected_status])
+
     def _create_listener_and_validate(self, lb_data, pool_id=None,
                                       protocol_port=80,
                                       admin_state_up=True, protocol='TCP'):
         if pool_id:
             pool = self._get_pool_from_lb_data(lb_data, pool_id=pool_id)
             loadbalancer_id = pool.loadbalancer_id
             pool_id = pool.pool_id
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_agent.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_driver.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,47 @@
 
         # Deleting the pool should also delete the members.
         self._delete_pool_and_validate(lb_data, "p_TCP")
 
         # Delete the whole LB.
         self._delete_load_balancer_and_validate(lb_data)
 
+    def test_hm(self):
+        lb_data = self._create_load_balancer_and_validate(
+            {'vip_network': 'vip_network',
+             'cidr': '10.0.0.0/24'})
+
+        # TCP Pool
+        self._create_pool_and_validate(lb_data, "p_TCP",
+                                       protocol=o_constants.PROTOCOL_TCP)
+
+        pool_TCP_id = lb_data['pools'][0].pool_id
+
+        # Members for TCP Pool
+        self._create_member_and_validate(
+            lb_data, pool_TCP_id, lb_data['vip_net_info'][1],
+            lb_data['vip_net_info'][0], '10.0.0.10')
+        self._create_member_and_validate(
+            lb_data, pool_TCP_id, lb_data['vip_net_info'][1],
+            lb_data['vip_net_info'][0], '10.0.0.11')
+
+        # CRUD health monitor.
+        self._create_hm_and_validate(lb_data, pool_TCP_id, 'hm_TCP', 10, 30, 3,
+                                     o_constants.HEALTH_MONITOR_TCP)
+        self._update_hm_and_validate(lb_data, pool_TCP_id,
+                                     admin_state_up=False)
+        self._update_hm_and_validate(lb_data, pool_TCP_id, admin_state_up=True)
+        self._delete_hm_and_validate(lb_data, pool_TCP_id)
+
+        # Create to test delete over pool
+        self._create_hm_and_validate(lb_data, pool_TCP_id, 'hm_TCP', 10, 30, 3,
+                                     o_constants.HEALTH_MONITOR_TCP)
+        # Deleting the pool should also delete the health monitor.
+        self._delete_pool_and_validate(lb_data, "p_TCP")
+
     def test_listener(self):
         lb_data = self._create_load_balancer_and_validate(
             {'vip_network': 'vip_network',
              'cidr': '10.0.0.0/24'})
         self._create_pool_and_validate(lb_data, "p_TCP", protocol='TCP')
         self._create_pool_and_validate(lb_data, "p_UDP", protocol='UDP')
         self._create_pool_and_validate(lb_data, "p_SCTP", protocol='SCTP')
@@ -344,14 +377,31 @@
 
     def test_lb_pool_cascade(self):
         self._test_cascade_delete(member=False, listener=False)
 
     def test_cascade_delete(self):
         self._test_cascade_delete()
 
+    def test_hm_unsupported_protocol(self):
+        lb_data = self._create_load_balancer_and_validate(
+            {'vip_network': 'vip_network',
+             'cidr': '10.0.0.0/24'})
+
+        self._create_pool_and_validate(lb_data, "p_SCTP",
+                                       protocol=o_constants.PROTOCOL_SCTP)
+        pool_SCTP_id = lb_data['pools'][0].pool_id
+        self._create_member_and_validate(
+            lb_data, pool_SCTP_id, lb_data['vip_net_info'][1],
+            lb_data['vip_net_info'][0], '10.0.0.10')
+        self.assertRaises(o_exceptions.UnsupportedOptionError,
+                          self._create_hm_and_validate, lb_data, pool_SCTP_id,
+                          'hm_SCTP', 10, 30, 3,
+                          o_constants.HEALTH_MONITOR_SCTP)
+        self._delete_load_balancer_and_validate(lb_data)
+
     def test_for_unsupported_options(self):
         lb_data = self._create_load_balancer_and_validate(
             {'vip_network': 'vip_network',
              'cidr': '10.0.0.0/24'})
 
         m_pool = self._create_pool_model(lb_data['model'].loadbalancer_id,
                                          'lb1')
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/functional/test_integration.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_integration.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/base.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/test_clients.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_clients.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/common/test_utils.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/fakes.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/hacking/test_checks.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/test_checks.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_agent.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_driver.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,32 +894,39 @@
                 'protocol': self.ref_pool.protocol,
                 'loadbalancer_id': self.ref_pool.loadbalancer_id}
         expected = {'type': ovn_const.REQ_TYPE_POOL_DELETE,
                     'info': info}
         self.driver.pool_delete(self.ref_pool)
         self.mock_add_request.assert_called_once_with(expected)
 
-    def test_pool_delete_with_members(self):
+    def test_pool_delete_with_members_and_hm(self):
+        self.ref_pool.healthmonitor = self.ref_health_monitor
         info = {'id': self.ref_pool.pool_id,
                 'protocol': self.ref_pool.protocol,
                 'loadbalancer_id': self.ref_pool.loadbalancer_id}
         expected = {'type': ovn_const.REQ_TYPE_POOL_DELETE,
                     'info': info}
+        info_hm = {'id': self.ref_pool.healthmonitor.healthmonitor_id,
+                   'pool_id': self.ref_pool.pool_id}
         info_member = {'id': self.ref_member.member_id,
                        'pool_id': self.ref_member.pool_id,
                        'subnet_id': self.ref_member.subnet_id,
                        'protocol_port': self.ref_member.protocol_port,
                        'address': self.ref_member.address}
+        expected_hm = {
+            'type': ovn_const.REQ_TYPE_HM_DELETE,
+            'info': info_hm}
         expected_members = {
             'type': ovn_const.REQ_TYPE_MEMBER_DELETE,
             'info': info_member}
         expected_members_dvr = {
             'type': ovn_const.REQ_TYPE_HANDLE_MEMBER_DVR,
             'info': mock.ANY}
-        calls = [mock.call(expected_members),
+        calls = [mock.call(expected_hm),
+                 mock.call(expected_members),
                  mock.call(expected_members_dvr),
                  mock.call(expected)]
         self.driver.pool_delete(self.ref_pool)
         self.mock_add_request.assert_has_calls(calls)
 
     def test_pool_update(self):
         info = {'id': self.ref_update_pool.pool_id,
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_hacking.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider/tests/unit/test_helper.py` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3914,15 +3914,17 @@
         self.assertEqual(status['listeners'][0]['provisioning_status'],
                          constants.ACTIVE)
         expected_clear_calls = [
             mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
                       'ip_port_mappings')]
         expected_remove_calls = [
             mock.call('Load_Balancer', self.ovn_hm_lb.uuid, 'health_check',
-                      self.ovn_hm.uuid)]
+                      self.ovn_hm.uuid),
+            mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
+                      'external_ids', ovn_const.LB_EXT_IDS_HMS_KEY)]
         expected_destroy_calls = [
             mock.call('Load_Balancer_Health_Check', self.ovn_hm.uuid)]
         del_hm_port.assert_called_once_with(self.member_subnet_id)
         self.helper.ovn_nbdb_api.db_clear.assert_has_calls(
             expected_clear_calls)
         self.helper.ovn_nbdb_api.db_remove.assert_has_calls(
             expected_remove_calls)
@@ -3984,14 +3986,43 @@
         status = self.helper.hm_delete(self.health_monitor)
         self.assertEqual(status['healthmonitors'][0]['provisioning_status'],
                          constants.DELETED)
         self.assertEqual(status['healthmonitors'][0]['operating_status'],
                          constants.NO_MONITOR)
         self.helper.ovn_nbdb_api.db_clear.assert_not_called()
 
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_ovn_lb_from_hm_id')
+    def test_hm_delete_hm_not_found_in_external_ids(self, folbfhi):
+        folbfhi.return_value = (self.ovn_hm, self.ovn_hm_lb)
+        self.ovn_hm_lb.external_ids[ovn_const.LB_EXT_IDS_HMS_KEY] = []
+        status = self.helper.hm_delete(self.health_monitor)
+        self.assertEqual(status['healthmonitors'][0]['provisioning_status'],
+                         constants.DELETED)
+        self.assertEqual(status['healthmonitors'][0]['operating_status'],
+                         constants.NO_MONITOR)
+
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_ovn_lb_from_hm_id')
+    def test_hm_delete_hm_not_match_in_external_ids(self, folbfhi):
+        folbfhi.return_value = (self.ovn_hm, self.ovn_hm_lb)
+        self.ovn_hm_lb.external_ids[ovn_const.LB_EXT_IDS_HMS_KEY] = \
+            '["%s"]' % (uuidutils.generate_uuid())
+        status = self.helper.hm_delete(self.health_monitor)
+        self.assertEqual(status['healthmonitors'][0]['provisioning_status'],
+                         constants.DELETED)
+        self.assertEqual(status['healthmonitors'][0]['operating_status'],
+                         constants.NO_MONITOR)
+        expected_set_external_ids_calls = [
+            mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
+                      ('external_ids', {
+                          ovn_const.LB_EXT_IDS_HMS_KEY:
+                              self.ovn_hm_lb.external_ids[
+                                  ovn_const.LB_EXT_IDS_HMS_KEY]}))]
+        self.helper.ovn_nbdb_api.db_set.assert_has_calls(
+            expected_set_external_ids_calls)
+
     def test_hm_update_event_offline(self):
         self.helper.ovn_nbdb_api.db_find_rows.return_value.\
             execute.return_value = [self.ovn_hm_lb]
         self.hm_update_event = ovn_event.ServiceMonitorUpdateEvent(
             self.helper)
         src_ip = '10.22.33.4'
         row = fakes.FakeOvsdbRow.create_one_ovsdb_row(
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/PKG-INFO` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-octavia-provider
-Version: 4.0.0.0rc1
+Version: 4.0.0.0rc2
 Summary: OpenStack Octavia integration with OVN
 Home-page: https://docs.openstack.org/ovn-octavia-provider/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================================
         ovn-octavia-provider - OVN Provider driver for Octavia LoadBalancer
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/ovn_octavia_provider.egg-info/SOURCES.txt` & `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/README.rst` & `ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/releasenotes/source/conf.py` & `ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/requirements.txt` & `ovn-octavia-provider-4.0.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/roles/configure_functional_tests/tasks/main.yaml` & `ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/roles/fetch_journal_log/tasks/main.yaml` & `ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/setup.cfg` & `ovn-octavia-provider-4.0.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/setup.py` & `ovn-octavia-provider-4.0.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/test-requirements.txt` & `ovn-octavia-provider-4.0.0.0rc2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/tools/check_unit_test_structure.sh` & `ovn-octavia-provider-4.0.0.0rc2/tools/check_unit_test_structure.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/tools/coding-checks.sh` & `ovn-octavia-provider-4.0.0.0rc2/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/tools/generate_config_file_samples.sh` & `ovn-octavia-provider-4.0.0.0rc2/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/tools/pip_install_src_modules.sh` & `ovn-octavia-provider-4.0.0.0rc2/tools/pip_install_src_modules.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/tox.ini` & `ovn-octavia-provider-4.0.0.0rc2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 basepython = python3
 usedevelop = True
 setenv = VIRTUAL_ENV={envdir}
          OS_LOG_CAPTURE={env:OS_LOG_CAPTURE:true}
          OS_STDOUT_CAPTURE={env:OS_STDOUT_CAPTURE:true}
          OS_STDERR_CAPTURE={env:OS_STDERR_CAPTURE:true}
          PYTHONWARNINGS=default::DeprecationWarning,ignore::DeprecationWarning:distutils,ignore::DeprecationWarning:site
-deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 allowlist_externals = bash
                       {toxinidir}/tools/pip_install_src_modules.sh
 passenv = http_proxy
           HTTP_PROXY
           https_proxy
@@ -75,15 +75,15 @@
   coverage report --fail-under=92 --skip-covered
   coverage html -d cover
   coverage xml -o cover/coverage.xml
 
 [testenv:docs]
 envdir = {toxworkdir}/docs
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
   -r{toxinidir}/doc/requirements.txt
   -r{toxinidir}/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
 envdir = {toxworkdir}/docs
 deps = {[testenv:docs]deps}
```

### Comparing `ovn-octavia-provider-4.0.0.0rc1/zuul.d/base.yaml` & `ovn-octavia-provider-4.0.0.0rc2/zuul.d/base.yaml`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc1/zuul.d/project.yaml` & `ovn-octavia-provider-4.0.0.0rc2/zuul.d/project.yaml`

 * *Files identical despite different names*

