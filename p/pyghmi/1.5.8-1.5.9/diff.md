# Comparing `tmp/pyghmi-1.5.8.tar.gz` & `tmp/pyghmi-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyghmi-1.5.8.tar", last modified: Wed Feb 26 21:59:14 2020, max compression
+gzip compressed data, was "dist/pyghmi-1.5.9.tar", last modified: Fri Feb 28 19:54:05 2020, max compression
```

## Comparing `pyghmi-1.5.8.tar` & `pyghmi-1.5.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      660 2020-02-26 21:58:29.000000 pyghmi-1.5.8/builddeb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2020-02-26 21:58:29.000000 pyghmi-1.5.8/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-02-26 21:58:29.000000 pyghmi-1.5.8/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-02-26 21:58:29.000000 pyghmi-1.5.8/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-02-26 21:58:29.000000 pyghmi-1.5.8/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/util/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/util/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/util/parse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12066 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/util/webclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/media.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/ipmi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31273 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/sdr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22132 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81575 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/ipmi/private/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3737 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/util.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24203 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/spd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4838 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/localsession.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58702 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/simplesession.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66918 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78503 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15082 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/private/serversession.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    43497 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/handler.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2119 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22288 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/config.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4777 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/inventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24628 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/nextscale.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1949 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/pci.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5925 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/EfiDecompressor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88345 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/imm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/firmware.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1493 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/cpu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2335 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/raid_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/energy.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3098 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/psu.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1761 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/dimm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/raid_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13639 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/generic.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1160 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/oem/lookup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14137 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/fru.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23191 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/console.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7014 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/ipmi/bmc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/cmd/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2541 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/cmd/pyghmicons.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/cmd/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2939 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/cmd/pyghmiutil.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2816 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/cmd/fakebmc.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5148 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/cmd/virshbmc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/redfish/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70301 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/redfish/oem/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26565 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/tsma.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35445 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/xcc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5388 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/generic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/redfish/oem/lookup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi/tests/unit/ipmi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/tests/unit/ipmi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/tests/unit/ipmi/test_sdr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-02-26 21:58:29.000000 pyghmi-1.5.8/pyghmi/tests/unit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-02-26 21:59:14.000000 pyghmi-1.5.8/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-02-26 21:58:29.000000 pyghmi-1.5.8/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3854 2020-02-26 21:58:29.000000 pyghmi-1.5.8/python-pyghmi.spec
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2020-02-26 21:58:29.000000 pyghmi-1.5.8/setup.py.tmpl
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      370 2020-02-26 21:58:29.000000 pyghmi-1.5.8/buildrpm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33110 2020-02-26 21:59:13.000000 pyghmi-1.5.8/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2020-02-26 21:59:14.000000 pyghmi-1.5.8/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2020-02-26 21:59:14.000000 pyghmi-1.5.8/pyghmi.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-02-26 21:59:13.000000 pyghmi-1.5.8/pyghmi.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-02-26 21:58:29.000000 pyghmi-1.5.8/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-02-26 21:58:29.000000 pyghmi-1.5.8/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-02-26 21:58:29.000000 pyghmi-1.5.8/README
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      852 2020-02-26 21:58:29.000000 pyghmi-1.5.8/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2020-02-26 21:58:29.000000 pyghmi-1.5.8/CONTRIBUTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-02-26 21:58:29.000000 pyghmi-1.5.8/zuul.d/project.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      292 2020-02-26 21:58:29.000000 pyghmi-1.5.8/makesetup
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2020-02-26 21:58:29.000000 pyghmi-1.5.8/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-02-26 21:58:29.000000 pyghmi-1.5.8/python-pyghmi.spec.tmpl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2020-02-26 21:58:29.000000 pyghmi-1.5.8/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-02-26 21:58:29.000000 pyghmi-1.5.8/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3183 2020-02-26 21:58:29.000000 pyghmi-1.5.8/wheezy.patch
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2020-02-26 21:58:29.000000 pyghmi-1.5.8/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2020-02-26 21:58:29.000000 pyghmi-1.5.8/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-02-26 21:58:29.000000 pyghmi-1.5.8/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7354 2020-02-26 21:58:29.000000 pyghmi-1.5.8/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-26 21:59:14.000000 pyghmi-1.5.8/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-02-26 21:58:29.000000 pyghmi-1.5.8/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-02-26 21:58:29.000000 pyghmi-1.5.8/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2020-02-26 21:59:13.000000 pyghmi-1.5.8/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-02-28 19:53:19.000000 pyghmi-1.5.9/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-02-28 19:53:19.000000 pyghmi-1.5.9/README
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      852 2020-02-28 19:53:19.000000 pyghmi-1.5.9/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-02-28 19:53:19.000000 pyghmi-1.5.9/zuul.d/project.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      660 2020-02-28 19:53:19.000000 pyghmi-1.5.9/builddeb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-02-28 19:53:19.000000 pyghmi-1.5.9/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3183 2020-02-28 19:53:19.000000 pyghmi-1.5.9/wheezy.patch
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2020-02-28 19:53:19.000000 pyghmi-1.5.9/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3854 2020-02-28 19:53:19.000000 pyghmi-1.5.9/python-pyghmi.spec
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2020-02-28 19:53:19.000000 pyghmi-1.5.9/setup.py.tmpl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2020-02-28 19:53:19.000000 pyghmi-1.5.9/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-02-28 19:53:19.000000 pyghmi-1.5.9/MANIFEST.in
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/cmd/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2816 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/cmd/fakebmc.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2939 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/cmd/pyghmiutil.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/cmd/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2541 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/cmd/pyghmicons.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5148 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/cmd/virshbmc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/util/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/util/parse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12066 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/util/webclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/util/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/tests/unit/ipmi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/tests/unit/ipmi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/tests/unit/ipmi/test_sdr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/ipmi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22132 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/events.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24628 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/nextscale.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3098 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/psu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5925 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/EfiDecompressor.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    43497 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/handler.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1493 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/cpu.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4777 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/inventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2335 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/raid_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/raid_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/energy.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2119 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22288 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/config.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88345 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/imm.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1949 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/pci.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/firmware.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1761 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/dimm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13639 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1160 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/oem/lookup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81575 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7014 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/bmc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31273 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/sdr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/ipmi/private/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    66918 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58702 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/simplesession.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3737 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/util.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24203 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/spd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78544 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15082 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/serversession.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4838 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/private/localsession.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23191 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/console.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14137 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/ipmi/fru.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/redfish/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/redfish/oem/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35445 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/xcc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26565 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/tsma.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5388 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/oem/lookup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70301 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:53:19.000000 pyghmi-1.5.9/pyghmi/redfish/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-02-28 19:53:19.000000 pyghmi-1.5.9/python-pyghmi.spec.tmpl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33176 2020-02-28 19:54:05.000000 pyghmi-1.5.9/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-02-28 19:53:19.000000 pyghmi-1.5.9/LICENSE
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      292 2020-02-28 19:53:19.000000 pyghmi-1.5.9/makesetup
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2020-02-28 19:54:05.000000 pyghmi-1.5.9/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-02-28 19:53:19.000000 pyghmi-1.5.9/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2020-02-28 19:54:05.000000 pyghmi-1.5.9/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2020-02-28 19:53:19.000000 pyghmi-1.5.9/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-02-28 19:53:19.000000 pyghmi-1.5.9/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2020-02-28 19:53:19.000000 pyghmi-1.5.9/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-02-28 19:53:19.000000 pyghmi-1.5.9/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-02-28 19:53:19.000000 pyghmi-1.5.9/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-02-28 19:54:05.000000 pyghmi-1.5.9/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-02-28 19:53:19.000000 pyghmi-1.5.9/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7354 2020-02-28 19:53:19.000000 pyghmi-1.5.9/doc/source/conf.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      370 2020-02-28 19:53:19.000000 pyghmi-1.5.9/buildrpm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2020-02-28 19:53:19.000000 pyghmi-1.5.9/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-02-28 19:54:05.000000 pyghmi-1.5.9/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-02-28 19:53:19.000000 pyghmi-1.5.9/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2020-02-28 19:53:19.000000 pyghmi-1.5.9/README.md
```

### Comparing `pyghmi-1.5.8/builddeb` & `pyghmi-1.5.9/builddeb`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/run.yaml` & `pyghmi-1.5.9/playbooks/legacy/tempest-devstack-ironic-pxe_ipmitool-pyghmi-src/run.yaml`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/util/parse.py` & `pyghmi-1.5.9/pyghmi/util/parse.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/util/webclient.py` & `pyghmi-1.5.9/pyghmi/util/webclient.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/media.py` & `pyghmi-1.5.9/pyghmi/media.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/version.py` & `pyghmi-1.5.9/pyghmi/version.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/exceptions.py` & `pyghmi-1.5.9/pyghmi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/sdr.py` & `pyghmi-1.5.9/pyghmi/ipmi/sdr.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/events.py` & `pyghmi-1.5.9/pyghmi/ipmi/events.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/command.py` & `pyghmi-1.5.9/pyghmi/ipmi/command.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/util.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/util.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/spd.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/spd.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/localsession.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/localsession.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/simplesession.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/simplesession.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/constants.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/constants.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/session.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
                 # AF_INET6, but no '::1', try the AF_INET6 version of 127
                 myself = '::ffff:127.0.0.1'
         if iothread is None:
             initevt = threading.Event()
             iothreadwaiters.append(initevt)
             _IOWorker = define_worker()
             iothread = _IOWorker()
+            iothread.daemon = True
             iothread.start()
             initevt.wait()
         elif not iothreadready:
             initevt = threading.Event()
             iothreadwaiters.append(initevt)
             initevt.wait()
         return tmpsocket
@@ -688,15 +689,14 @@
             rsaddr = constants.IPMI_BMC_ADDRESS
         if self.servermode:
             rsaddr = self.clientaddr
         # figure 13-4, first two bytes are rsaddr and
         # netfn, for non-bridge request, rsaddr is always 0x20 since we are
         # addressing BMC while rsaddr is specified forbridge request
         header = bytearray((rsaddr, (netfn << 2) | lun))
-
         reqbody = bytearray((rqaddr, self.seqlun, command)) + data
         headsum = bytearray((_checksum(*header),))
         bodysum = bytearray((_checksum(*reqbody),))
         payload = header + headsum + reqbody + bodysum
         if bridge_request:
             payload = bridge_msg + payload
             # NOTE(fengqian): For bridge request, another check sum is needed.
@@ -1621,15 +1621,15 @@
         if self.servermode:
             self.seqlun = payload[4]
             self.clientaddr = payload[3]
             self.clientnetfn = (payload[1] >> 2) + 1
             self.clientcommand = payload[5]
             self._parse_payload(payload)
             return
-        entry = (payload[1] >> 2, payload[4], payload[5])
+        entry = (payload[1] >> 2, payload[4] & 0xfc, payload[5])
         if self._lookup_request_entry(entry):
             self._remove_request_entry(entry)
 
             # NOTE(fengqian): for bridge request, we need to handle the
             # response twice. First response shows if message send correctly,
             # second response is the real response.
             # If the message is send crrectly, we will discard the first
```

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/private/serversession.py` & `pyghmi-1.5.9/pyghmi/ipmi/private/serversession.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/handler.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/handler.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/drive.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/drive.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/config.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/config.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/inventory.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/inventory.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/nextscale.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/nextscale.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/pci.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/pci.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/EfiDecompressor.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/EfiDecompressor.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/imm.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/imm.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/firmware.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/firmware.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/cpu.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/cpu.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/raid_controller.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/raid_controller.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/energy.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/energy.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/psu.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/psu.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/dimm.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/dimm.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lenovo/raid_drive.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lenovo/raid_drive.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/generic.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/generic.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/oem/lookup.py` & `pyghmi-1.5.9/pyghmi/ipmi/oem/lookup.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/fru.py` & `pyghmi-1.5.9/pyghmi/ipmi/fru.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/console.py` & `pyghmi-1.5.9/pyghmi/ipmi/console.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/ipmi/bmc.py` & `pyghmi-1.5.9/pyghmi/ipmi/bmc.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/cmd/pyghmicons.py` & `pyghmi-1.5.9/pyghmi/cmd/pyghmicons.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/cmd/pyghmiutil.py` & `pyghmi-1.5.9/pyghmi/cmd/pyghmiutil.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/cmd/fakebmc.py` & `pyghmi-1.5.9/pyghmi/cmd/fakebmc.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/cmd/virshbmc.py` & `pyghmi-1.5.9/pyghmi/cmd/virshbmc.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/command.py` & `pyghmi-1.5.9/pyghmi/redfish/command.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/tsma.py` & `pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/tsma.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/main.py` & `pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/main.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/oem/lenovo/xcc.py` & `pyghmi-1.5.9/pyghmi/redfish/oem/lenovo/xcc.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/oem/generic.py` & `pyghmi-1.5.9/pyghmi/redfish/oem/generic.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/redfish/oem/lookup.py` & `pyghmi-1.5.9/pyghmi/redfish/oem/lookup.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/constants.py` & `pyghmi-1.5.9/pyghmi/constants.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/storage.py` & `pyghmi-1.5.9/pyghmi/storage.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/tests/unit/ipmi/test_sdr.py` & `pyghmi-1.5.9/pyghmi/tests/unit/ipmi/test_sdr.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi/tests/unit/base.py` & `pyghmi-1.5.9/pyghmi/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/PKG-INFO` & `pyghmi-1.5.9/pyghmi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyghmi
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python General Hardware Management Initiative (IPMI and others)
 Home-page: http://github.com/openstack/pyghmi/
 Author: Jarrod Johnson
 Author-email: jjohnson2@lenovo.com
 License: Apache License, Version 2.0
 Description: This is a pure python implementation of IPMI protocol.
```

### Comparing `pyghmi-1.5.8/LICENSE` & `pyghmi-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/python-pyghmi.spec` & `pyghmi-1.5.9/python-pyghmi.spec`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/setup.py.tmpl` & `pyghmi-1.5.9/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/ChangeLog` & `pyghmi-1.5.9/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.5.9
+-----
+
+* Discard rsLun in reply
+* Set daemon for IO thread
+
 1.5.8
 -----
 
 * Add a simplesession option
 * Support non-zero LUN
 * fix(kcs): Fix the command class to use bytearray instead of lists for raw data
 * Fix IMM/XCC over network
```

### Comparing `pyghmi-1.5.8/setup.cfg` & `pyghmi-1.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/pyghmi.egg-info/PKG-INFO` & `pyghmi-1.5.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyghmi
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python General Hardware Management Initiative (IPMI and others)
 Home-page: http://github.com/openstack/pyghmi/
 Author: Jarrod Johnson
 Author-email: jjohnson2@lenovo.com
 License: Apache License, Version 2.0
 Description: This is a pure python implementation of IPMI protocol.
```

### Comparing `pyghmi-1.5.8/pyghmi.egg-info/SOURCES.txt` & `pyghmi-1.5.9/pyghmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/setup.py` & `pyghmi-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/CONTRIBUTING.rst` & `pyghmi-1.5.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/tox.ini` & `pyghmi-1.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/python-pyghmi.spec.tmpl` & `pyghmi-1.5.9/python-pyghmi.spec.tmpl`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/wheezy.patch` & `pyghmi-1.5.9/wheezy.patch`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/README.md` & `pyghmi-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/doc/source/conf.py` & `pyghmi-1.5.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyghmi-1.5.8/AUTHORS` & `pyghmi-1.5.9/AUTHORS`

 * *Files identical despite different names*

