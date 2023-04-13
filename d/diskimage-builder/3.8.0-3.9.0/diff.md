# Comparing `tmp/diskimage-builder-3.8.0.tar.gz` & `tmp/diskimage-builder-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/diskimage-builder-3.8.0.tar", last modified: Wed Mar 31 08:34:36 2021, max compression
+gzip compressed data, was "dist/diskimage-builder-3.9.0.tar", last modified: Thu Apr  8 07:21:01 2021, max compression
```

## Comparing `diskimage-builder-3.8.0.tar` & `diskimage-builder-3.9.0.tar`

### file list

```diff
@@ -1,1518 +1,1518 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/.testr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.838846 diskimage-builder-3.8.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10124 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/.zuul.d/jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/.zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   100886 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1934 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.838846 diskimage-builder-3.8.0/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9860 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/bin/dib-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.838846 diskimage-builder-3.8.0/contrib/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2562 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/contrib/setup-gate-mirrors.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.838846 diskimage-builder-3.8.0/diskimage_builder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.846847 diskimage-builder-3.8.0/diskimage_builder/block_device/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17835 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/blockdevice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9444 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.846847 diskimage-builder-3.8.0/diskimage_builder/block_device/level0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level0/localloop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.846847 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13461 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15444 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/mbr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/partition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level1/partitioning.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.846847 diskimage-builder-3.8.0/diskimage_builder/block_device/level2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5420 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level2/mkfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.846847 diskimage-builder-3.8.0/diskimage_builder/block_device/level3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6752 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level3/mount.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.850847 diskimage-builder-3.8.0/diskimage_builder/block_device/level4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level4/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/level4/fstab.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6604 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.850847 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.858847 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/bad_edge_graph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/bad_plugin.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/cmd_create.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/deep_graph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/deep_tree.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/duplicate_fs_labels.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/duplicate_name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/gpt_efi.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_graph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_partitions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv_vg.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_partition_ordering.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_spanned_vg.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/multi_key_node.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/multiple_partitions_graph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/multiple_partitions_tree.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/rollback.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/simple_graph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/simple_tree.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/too_long_fs_label.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.858847 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/test_a.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/test_b.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6119 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3574 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_gpt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24482 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mbr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mkfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7778 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mount_order.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5527 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/block_device/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/disk_image_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12071 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/element_dependencies.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.858847 diskimage-builder-3.8.0/diskimage_builder/elements/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.858847 diskimage-builder-3.8.0/diskimage_builder/elements/apt-conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-conf/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.858847 diskimage-builder-3.8.0/diskimage_builder/elements/apt-conf/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      592 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-conf/extra-data.d/99-override-default-apt-conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1635 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/extra-data.d/99-set-apt-package-pins
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      765 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/extra-data.d/99-override-default-apt-sources
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.774842 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/environment.d/00-set-apt-sources
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      128 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/extra-data.d/00-write-apt-sources
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      256 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/pre-install.d/00-test-apt-sources
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1200 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/cleanup.d/99-extract-kernel-and-ramdisk
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.862848 diskimage-builder-3.8.0/diskimage_builder/elements/base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/base/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/environment.d/10-base-defaults
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/base/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      202 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/install.d/00-baseline-environment
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      256 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/install.d/00-up-to-date
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      368 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/install.d/10-cloud-init
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/base/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      453 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/base/pre-install.d/03-baseline-tools
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/block-device-default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/environment.d/15-block-device.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.866848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/block-device-default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/block-device-ppc64el.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/environment.d/15-block-device.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/block-device-default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/block-device-ppc64el.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/environment.d/15-block-device.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1477 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/cleanup.d/51-bootloader
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/environment.d/10-bootloader-default-cmdline
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.870848 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9961 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/finalise.d/50-bootloader
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1244 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.874849 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.874849 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3717 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/bin/cache-url
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.874849 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/tests/test_cache_url.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.874849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/environment.d/10-centos-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/environment.d/11-yum-dnf.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2287 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/pre-install.d/00-02-set-centos-mirror
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      775 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/pre-install.d/02-set-machine-id
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2242 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/root.d/10-centos-cloud-image
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.778842 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.886849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.886849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.886849 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.874849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/environment.d/10-centos-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/environment.d/11-yum-dnf.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.778842 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/environment.d/09-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.878849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/environment.d/09-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.778842 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/7/yum.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/appstream.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/base.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.882849 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/appstream.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/base.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.886849 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.886849 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/environment.d/00-centos7-element-deprecation.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/environment.d/09-centos7-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/environment.d/10-centos7-distro-name.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.778842 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cleanup-kernel-initrd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cleanup-kernel-initrd/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1560 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/99-cleanup-kernel-initrd
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      307 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/post-install.d/20-enable-cloud-init
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      786 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/post-install.d/21-cloud-init-allow-password-auth
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1018 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/install.d/05-set-cloud-init-sources
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-disable-resizefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-disable-resizefs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/50-cloud-init-disable-resizefs
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/51-cloud-init-disable-growpart
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.890850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/environment.d/10-cloud-init-nocloud.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      323 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-nocloud/install.d/05-inject-local-source-data
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/debian/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debian/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1438 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/install.d/10-cloud-opinions
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.782842 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian/test-elements/build-succeeds/environment.d/09-debian-stable
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/environment.d/10-debian-minimal.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2432 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/root.d/75-debian-minimal-baseinstall
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.782842 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.894850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-systemd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-systemd/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-systemd/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-systemd/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      182 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-systemd/root.d/05-debian-systemd
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.898850 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      177 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/root.d/05-debian-upstart
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      712 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/root.d/20-debian-fix-upstart-jobs
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      809 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/cleanup.d/99-clean-up-cache
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.902850 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/environment.d/10-debootstrap-default-locale
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/environment.d/20-network-interface-names
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1657 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/10-debian-networking
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1135 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/12-debian-locale-gen
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      754 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/15-cleanup-debootstrap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3199 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/root.d/08-debootstrap
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/binary-deps.d/deploy
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/init.d/80-deploy
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/binary-deps.d/deploy-kexec
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.906851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/init.d/81-deploy-kexec
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-kexec/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/binary-deps.d/deploy-targetcli
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/dracut-drivers.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/dracut-drivers.d/targetcli-drivers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      257 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/50-add-targetcli-module
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      741 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/iscsi-func
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      770 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/module-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      911 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/targetcli-wrapper
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/binary-deps.d/deploy-tgtadm
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      251 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/50-inject-tgtadm-iscsi-func
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/iscsi-func
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.910851 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.914851 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/environment.d/50-devuser
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.914851 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/extra-data.d/50-devuser
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.914851 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      998 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/install.d/50-devuser
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/devuser/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.914851 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.914851 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3707 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/50-dhcp-all-interfaces
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      849 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/60-remove-cloud-image-interfaces
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/NetworkManager-conf.d-00-main.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces-udev.rules
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      700 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.init
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8438 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-interface@.service
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/environment.d/99-dib-init-system
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      781 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/install.d/20-install-init-scripts
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      674 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/post-install.d/10-enable-init-scripts
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      418 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/pre-install.d/04-dib-init-system
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      267 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/cleanup.d/50-dib-python
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/environment.d/50-dib-python-version
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      767 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/pre-install.d/01-dib-python
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/dib-run-parts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-run-parts/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dib-run-parts/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/dracut.conf.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/dracut.conf.d/disable-nouveau.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/modprobe.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-nouveau/modprobe.d/disable-nouveau.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.918852 diskimage-builder-3.8.0/diskimage_builder/elements/disable-selinux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-selinux/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/disable-selinux/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      195 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/disable-selinux/post-install.d/15-disable-selinux
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      832 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dkms/post-install.d/97-dkms
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/docker/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/docker/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/docker/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1203 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/docker/extra-data.d/01-docker-minimal
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/docker/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1095 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/docker/root.d/08-docker
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2120 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/bin/install-packages
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      364 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/cleanup.d/40-unblock-daemons
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      202 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/cleanup.d/50-remove-img-build-proxy
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      224 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/cleanup.d/60-untrim-dpkg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.922852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/environment.d/10-dpkg.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      216 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/finalise.d/99-clean-up-cache
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1368 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/finalise.d/99-write-dpkg-manifest
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      264 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/pre-install.d/00-disable-apt-recommends
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      170 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/pre-install.d/99-apt-get-update
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      871 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/09-apt-keyring
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      486 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-block-apt-translations
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-block-daemons
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      308 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-build-with-http-cache
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      376 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-shared-apt-cache
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      403 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-trim-dpkg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-network/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/binary-deps.d/dracut-ramdisk
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.926852 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/dracut-drivers.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/dracut-drivers.d/base-drivers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/environment.d/10-dracut-version.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      543 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/deploy-cmdline.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      305 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/module-setup.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/init.d/00-override-troubleshoot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      669 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/install.d/20-install-dracut-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      625 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/01-ensure-drivers
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3006 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/99-build-dracut-ramdisk
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/source-repository-dracut
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/environment.d/10-dracut-regenerate
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      561 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/50-dracut-conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3604 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/finalise.d/50-dracut-regenerate
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.930853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/systemd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/systemd/dynamic-login.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      584 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/dynamic-login.init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/upstart/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/upstart/dynamic-login.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      267 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/install.d/70-enable-dynamic-login-services
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/usr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/usr/local/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1165 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/dynamic-login
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/element-manifest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/element-manifest/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/element-manifest/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/element-manifest/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      363 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/element-manifest/extra-data.d/75-inject-element-manifest
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/cleanup.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/cleanup.d/99-fix-grub
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.934853 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1038 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/install.d/20-stty
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/install.d/serial-console-udev.rules
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/install.d/ttySx.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/ensure-venv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ensure-venv/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ensure-venv/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ensure-venv/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ensure-venv/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/epel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/epel/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/epel/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/epel/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/epel/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/epel/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1601 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/epel/pre-install.d/05-rpm-epel-release
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/environment.d/10-fedora-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/environment.d/11-yum-dnf.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      878 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/pre-install.d/00-02-set-fedora-mirror
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      616 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/pre-install.d/02-set-machine-id
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1896 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/root.d/10-fedora-cloud-image
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.938853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/environment.d/10-fedora-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/environment.d/11-yum-dnf.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.790843 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/yum.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1407 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/fix_shm
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3999 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/install-packages
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      948 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/unfix_shm
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.942853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1739 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/cleanup.d/05-unmount
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/environment.d/00-gentoo-envars.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/extra-data.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52263 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/extra-data.d/gentoo-releng.gpg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1414 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/finalise.d/99-cleanup
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      647 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-finalise.d/01-gentoo-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      475 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-00-set-profile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      198 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-01-migrate-pax
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1640 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-02-flags
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-03-enable-overlays
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1447 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-04-install-desired-python
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5546 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/root.d/10-gentoo-image
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      771 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/root.d/50-gentoo-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.794843 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.946853 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.794843 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/openrc/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      105 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/openrc/growroot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/systemd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/systemd/growroot.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/upstart/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/init-scripts/upstart/growroot.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      439 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/post-install.d/80-growroot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.794843 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.794843 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/usr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.794843 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/usr/local/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/usr/local/sbin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      869 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/usr/local/sbin/growroot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/grub2/post-install.d/01-delete-grubenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      468 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/post-install.d/95-hpdsa
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      197 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/post-install.d/98-hpdsa-post-dkms
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.950854 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      358 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/pre-install.d/06-hpdsa
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      381 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/root.d/10-hpdsa-check-distro
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/binary-deps.d/hwburnin
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwburnin/init.d/70-hwburnin
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/binary-deps.d/hwdiscovery
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/init.d/60-hwdiscovery
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.798843 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/systemd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/systemd/init-ibft-interfaces.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      633 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/init-ibft-interfaces.init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.954854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/upstart/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/upstart/init-ibft-interfaces.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      394 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/post-install.d/70-init-ibft-interfaces
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.798843 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.798843 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/etc/modules-load.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/etc/modules-load.d/ibft.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.798843 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/usr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.798843 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/sbin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      501 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/sbin/init-ibft-interfaces.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      713 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/extra-data.d/50-ilo-firmware
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/init.d/50-ilo-firmware
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/ramdisk-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      165 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ilo/ramdisk-install.d/50-ilo-firmware
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-bin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-bin/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-bin/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      163 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-bin/pre-install.d/01-install-bin
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      422 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/install.d/10-install-static-files
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-static/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-types/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.958854 diskimage-builder-3.8.0/diskimage_builder/elements/install-types/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2387 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/install-types/extra-data.d/99-enable-install-types
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/environment.d/open-iscsi-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      347 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/extra-data.d/50-check-dracut-regenerate
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      364 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/finalise.d/51-open-iscsi-config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      243 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/post-install.d/open-iscsi-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iso/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2000 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iso/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6553 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/cleanup.d/100-build-iso
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/iso/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1968 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/iso/post-install.d/01-copy-bootloaders
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/journal-to-console/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/journal-to-console/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/journal-to-console/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      809 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/journal-to-console/post-install.d/30-journal-to-console
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/environment.d/62-ssh-key
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      355 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/extra-data.d/62-ssh-key
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      592 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/install.d/62-ssh-key
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.962855 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2075 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/local-config/pre-install.d/02-proxy-settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2369 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/finalise.d/60-bootloader
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      408 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/lvm/root.d/10-lvm-check-distro
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1688 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/cleanup.d/01-copy-manifests-dir
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/environment.d/14-manifests
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      754 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/manifests/extra-data.d/20-manifest-dir
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/init.d/01-mellanox
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.966855 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      542 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/install.d/65-mellanox
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/install.d/mellanox-rules.udev
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/udev.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/udev.d/81-mellanox-drivers.rules
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      944 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/extra-data.d/50-modprobe-blacklist
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      241 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/install.d/80-modprobe-blacklist
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe-blacklist/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe-blacklist/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe-blacklist/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      275 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/modprobe-blacklist/install.d/80-modprobe-blacklist
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/no-final-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/no-final-image/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/yum.repos.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/yum.repos.d/fedora-oat.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      629 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/post-install.d/80-enable-sshd-service
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1364 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/post-install.d/99-harden-sshd-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/11-dib-distribution-mirror.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      372 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/extra-data.d/75-copy-mirror-info
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.970855 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1105 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/10-apt-disable-gpg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/environment.d/10-opensuse-distro-name.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      284 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/extra-data.d/01-inject-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2258 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/root.d/10-opensuse-cloud-image
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.806844 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/environment.d/10-opensuse-distro-name.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.806844 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.974856 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4469 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1548 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7597 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs-squash
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4917 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs-v2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1417 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-uninstalls
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      254 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/extra-data.d/99-squash-package-install
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      192 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/install.d/01-package-installs
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      206 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/install.d/99-package-uninstalls
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      197 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/post-install.d/00-package-installs
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      211 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/post-install.d/95-package-uninstalls
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/pre-install.d/10-package-installs
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      210 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/pre-install.d/99-package-uninstalls
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.978856 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7323 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/tests/test_package_squash.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4166 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/51-pip-and-virutalenv-default.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.806844 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/install.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10820 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/04-install-pip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      272 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/post-install.d/89-clean-up-pip-cache
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/source-repository-pip-and-virtualenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.806844 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/environment.d/10-source-installtype-pip-and-virtualenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/environment.d/10-source-installtype-pip-and-virtualenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.982856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/environment.d/10-source-installtype-pip-and-virtualenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/environment.d/10-pip-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      248 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/root.d/11-pip-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6850 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/bin/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/extra-data.d/10-create-pkg-map-dir
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/posix/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/posix/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/posix/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/posix/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7865 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/posix/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1809 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/install.d/65-proliant-tools-install
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      361 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/extra-data.d/00-mount-pypi-mirror
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      192 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/post-install.d/00-unconfigure-pypi-mirror
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.986856 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2818 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/pypi/pre-install.d/04-configure-pypi-mirror
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      997 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/post-install.d/55-brick-client-install
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1127 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/install.d/70-python-build
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      324 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/post-install.d/70-python-build
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/source-repository-pyenv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.810844 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/environment.d/70-test-python-stow.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/69-test-python-stow
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      723 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/71-test-python-stow
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/binary-deps.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/binary-deps.d/ramdisk
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/init.d/10-start-base-system
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/init.d/30-start-network
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      176 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/install.d/20-install-dhcp-client
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      120 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/install.d/52-ramdisk-install-busybox
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1875 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/post-install.d/99-build-ramdisk
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      300 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/cleanup.d/99-extract-ramdisk-files
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      391 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/01-inject-ramdisk-build-files
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.990857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7628 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/init-func
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      952 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init-end
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/init.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/init.d/20-init-variables
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/init.d/40-check-network-ready
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1082 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/post-install.d/01-ensure-binaries
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/udev.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5654 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/udev.d/60-persistent-storage.rules
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.994857 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1127 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/install.d/05-xen-tools
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3253 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/install.d/10-nova-agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/source-repository-nova-agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/source-repository-xen-tools
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/bin/extract-image
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3952 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/bin/map-packages
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/environment.d/50-redhat-common
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      565 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/finalise.d/01-clean-old-kernels
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/environment.d/10-rhel-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/environment.d/11-yum-dnf.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      775 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/pre-install.d/02-set-machine-id
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1388 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel/root.d/10-rhel-cloud-image
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11494 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      910 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/finalise.d/60-unregister
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      288 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/install.d/10-openstack-selinux-rhel
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.814844 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/os-refresh-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5645 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/06-rhel-registration
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.998857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4220 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhel-registration
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2338 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhsm
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      525 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/01-module-configuration
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      288 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/10-rhel-blacklist
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/environment.d/00-rhel7-element-deprecation.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/environment.d/10-rhel7-distro-name.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4646 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/cleanup.d/99-selinux-fixfiles-restore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      359 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/post-install.d/06-network-config-nonzeroconf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      476 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/pre-install.d/00-fix-requiretty
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      179 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/pre-install.d/00-usr-local-bin-secure-path
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1007 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/pre-install.d/01-override-yum-arch
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      320 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/cleanup.d/90-remove-ssh-host-keys
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.814844 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/systemd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/systemd/ssh-keygen.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/upstart/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/upstart/ssh-keygen.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.002857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      801 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/80-ssh-keygen
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.818845 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.818845 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.818845 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1043 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/runtime-ssh-host-keys.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/select-boot-kernel-initrd
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/cleanup.d/99-remove-dib-img-functions
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/extra-data.d/99-copy-dib-img-functions
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/selinux-permissive/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/selinux-permissive/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/selinux-permissive/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      193 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/selinux-permissive/pre-install.d/11-selinux-permissive
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2717 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/environment.d/15-simple-init-networkmanager
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/environment.d/50-disable-cloud-init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      898 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/50-simple-init
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      984 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/60-simple-init-remove-interfaces
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      968 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/40-glean
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      959 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/40-glean
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.006857 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1307 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/post-install.d/80-simple-init
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/source-repository-simple-init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5879 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12420 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/extra-data.d/98-source-repositories
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/install.d/02-stable-interface-names
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/stable-interface-names/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3036 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1519 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/bin/svc-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2829 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/extra-data.d/10-merge-svc-map-files
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      203 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/extra-data.d/11-copy-svc-map-file
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6156 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/tests/test_data_merge.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1208 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/bin/sysctl-set-value
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      995 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/bin/sysctl-write-value
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/sysprep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/sysprep/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/sysprep/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      226 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/sysprep/finalise.d/01-clear-machine-id
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.010858 diskimage-builder-3.8.0/diskimage_builder/elements/uboot/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/uboot/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/uboot/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      916 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/uboot/cleanup.d/98-uboot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/environment.d/99-cloud-init-datasources.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      115 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/post-install.d/99-autoremove
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      269 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/pre-install.d/00-remove-apt-xapian-index
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      393 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/pre-install.d/00-remove-grub
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/pre-install.d/01-set-ubuntu-mirror
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2816 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/root.d/10-cache-ubuntu-tarball
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.826845 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/environment.d/10-ubuntu-distro-name.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/environment.d/11-ubuntu-init-system.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1401 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/install.d/80-disable-rfc3041
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/environment.d/11-ubuntu-kernel.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/environment.d/12-ubuntu-repo-dists.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2089 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/root.d/75-ubuntu-minimal-baseinstall
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.822845 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.014858 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.018859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1138 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/post-install.d/90-get-signed-kernel
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1871 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/75-ubuntu-minimal-baseinstall
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.822845 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.022859 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/test-output-formats
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/vm/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/vm/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/vm/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      242 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/vm/finalise.d/50-remove-bogus-udev-links
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.026859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4551 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/bin/install-packages
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      400 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/cleanup.d/99-remove-yum-repo-conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/extra-data.d/99-yum-repo-conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      325 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/post-install.d/99-reset-yum-conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      425 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/pre-install.d/00-01-yum-keepcache
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      261 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/pre-install.d/00-dnf-update
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      871 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/pre-install.d/01-00-centos-python3
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      271 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum/root.d/50-yum-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/cleanup.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1052 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/cleanup.d/95-remove-yum-mirror
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1447 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/install.d/10-base-networking
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      888 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/install.d/11-ensure-dbus-daemon
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/pkg-map
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3063 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/pre-install.d/03-yum-cleanup
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14662 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/root.d/08-yum-chroot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.030859 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/environment.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/environment.d/10-zipl-default-cmdline
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/finalise.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2002 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/finalise.d/50-zipl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      921 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zipl/pre-install.d/kernel_config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2107 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/bin/install-packages
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/install.d/01-login-defs
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      718 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/post-install.d/10-mkinitrd
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      150 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/post-install.d/98-zypper-clean-cache
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      189 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/post-install.d/99-zypper-no-keep-packages
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      180 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/pre-install.d/01-zypper-keep-packages
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      297 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper/root.d/50-zypper-cache
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/element-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      285 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/post-install.d/01-locale-cleanup
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      416 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/pre-install.d/00-disable-zypper-recommends
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.034860 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5982 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/root.d/08-zypper-chroot
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/diskimage_builder/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/common-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17655 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/common-functions
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/dib-block-device.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4614 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/dib-run-parts
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/die
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24545 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/disk-image-create
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/element-info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/img-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9332 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/img-functions
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3007 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/outfilter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7843 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-functions
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24545 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-image-create
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/logging_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/paths.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/diskimage_builder/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2071 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/diskimage_builder/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9983 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/test_elementdeps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/test_loggingconfig.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/tests/test_no_dup_filenames.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/diskimage_builder/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.842846 diskimage-builder-3.8.0/diskimage_builder.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62653 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2021-03-31 08:34:35.000000 diskimage-builder-3.8.0/diskimage_builder.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/doc/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/lib/element_deps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.038860 diskimage-builder-3.8.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/ci.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7856 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/doc/source/developer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/caches.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/components.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3429 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18143 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/developing_elements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1748 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/dib_lint.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/invocation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/stable_interfaces.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9552 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/developer/vhd_creation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/elements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/doc/source/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/specs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.830846 diskimage-builder-3.8.0/doc/source/specs/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/doc/source/specs/v1/approved/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7081 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/specs/v1/approved/block-device-lvl1-partitioning.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/specs/v1/approved/block-device-overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/specs/v1/approved/v1-template.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/doc/source/user_guide/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23873 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/user_guide/building_an_image.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/user_guide/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/user_guide/install_types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/user_guide/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/doc/source/user_guide/supported_distros.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.830846 diskimage-builder-3.8.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/playbooks/dib-functests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/playbooks/dib-functests/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/playbooks/dib-functests/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.042860 diskimage-builder-3.8.0/playbooks/dib-nodepool/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/playbooks/dib-nodepool/debootstrap.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/pylint.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.830846 diskimage-builder-3.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/1.16.0-updates-bad91fc0b36c1755.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/1.17.0-ef744f36d277dba4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/1.18.0-4433d3076627f10d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/1.18.1-ceeb514708dcb731.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/Add-DIB-UBUNTU-KERNEL-5f75a809f3ce9bab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-6b94d90caea2895e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-aarch64-support-for-rhel-c62a0e02b1ad9033.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-centos-8-support-4fd28eb04e11ba43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-efi-packages-70a19464d31ab8d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-modprobe-element-8e3b0287ebb11920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/add-version-less-rhel-element-82fac7f2609e16d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/apt-transport-https-e4856cb9e2f8422c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/block-device-handling-279cddba8a859718.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/block-device-lvm-c3b8a214952b4db5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/block-device-mkfs-mount-fstab-42d7efe28fc2df04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/block-device-partitioning-237249e7ed2bad26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/block-device-update-partition-table-eb4ff077f90dfb19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/bootloader-commandline-d2db7524f1f9ad28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/bootloader-gpt-d1047f81f3a0631b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/centos-minimal-8-aca6314862741177.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/centos-minimal-8-stream-97021a2c92463dde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/centos-retired-f17ae9f6f03e57e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/cloud-init-resizefs-growpart-e820b8c7f3adb78b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/create-945440b17d500bf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dash-p-after-install-58a87549c1c906c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/debian-minimal-confilicts-c139ab0c98e5762f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/debian-security-7279855cf464f88b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/debian-security-b4f677a148fdf9c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/deprecate-ironic-agent-element.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dhcp-all-interfaces-networkmanager-b34f2fc8fb1a678f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dhcp-vlan-interfaces-b34ab224b9431e3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-distribution-mirror-8c241c0d3d4a539a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-init-system-5647bad17a01c602.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-init-system_fix_for_debian_jessie-c6f7261ee84dad27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-python-deprecate-8401c35a87559076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-run-parts-6f67d038aa5a4156.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dib-run-parts-e18cc3a6c2d66c24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4181 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dibv2-omnibus-b30e0c7ecd76db8d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/doc-auto-element-dependency-cb7488c5bb7301a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dpkg-copy-keys-578e16f7fedd823b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/dracut-network-adaabf90da9f6866.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/efi-bios-images-052283eabba98b90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/efi-bootloader-disk-size-4c1a9f18967104fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/element-info-entry-point-448bf622be6061a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/element-override-ccda78c24ab4a4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/element-vars-c6bf2e6795002f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/ensure-venv-d7c16a2a04fd3b8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/fedora26-690b9fd9ac3c3d4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/fedora32-9dfa4d9d4dcce1ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/fix-dnf-clean-old-kernels-use-rpm-to-erase-in-case-running-kernel-0401f78d63daca77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/fix_rdisc6_loop-32a308a97de99f0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/gpt-esp-partition-size-200568cb6fcc8788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/grub-timeout-1cdd14a2b1467d89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/gzip-env-variable-94e61e0c043f4f1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/harden-sshd-config-3f84556136014f95.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/image-size-padding-24f88d1c4a215221.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/image-size-padding-mb-574104d40fdd2345.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/incorrect-grub-label-5d2000215c0cc73e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/init-ibft-interfaces-9458d97dfcecc3ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/journal-console-752b46542ec5595e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/logfile-quiet-b18f2de4059eecfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/move_tidy_logs_to_main-a8c03427fe1a445c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/no-ironic-agent-689e58268e1bf44f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/openssh-server-0f6d065748a2fc18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/opensuse-150-default-c047033b850d41ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/opensuse-151-default-67ccfffbc134704d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/opensuse-423-default-3bc73fff69374cd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/opensuse-minimal-45267f5be1112c22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/package-install-arch-38bb5a6e61794fa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/package-installs-when-list-cfc00032271bae75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/package-outside-debootstrap-ac93e9ce991819f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/pip-and-virtualenv-args-5d3f2512edd7f3a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/pip-and-virtualenv-platform-removal-52e0d6a22829a3b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/post-root-stage-51da051bcdfbc55f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/pre-finalise-stage-574ae7886274bcba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/python-venv-d5b04fcf57e460bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/remove-dib-utils-37f70dfad54900a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/remove-solicit-delay-57a035b91922522a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/rhel-module-selection-e9f6f06ece1fb829.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/rhel-registration-4d4fe741321e9345.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/rhel7-element-deprecation-b0c1b57be8cd06ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/root-journal-size-618e064d6681699a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/runtime-ssh-host-keys-7a2fc873cc90d33e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/selinux-permissive-pre-install-ce19461ef17ec972.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/simple-init-nm-5d19e249c0a4560b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/simple-init-nm-delay-f579e05467785219.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/simple-init-nm-f0896124dee92a03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/skip-packages-env-c97e7b4820f9bfda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/squashfs-output-91c1f0dc37474d3c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/start-using-reno-446b3d52a467a273.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/sysprep-f3fd036bc1d2c405.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/sysprep-fixes-8890b968a8fa7ac1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/timestamp-43015aa5434e8ddb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/trusty-testing-removal-51160ee59c5477d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/ubuntu-arbitrary-images-c796f5c6dbd40679.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/ubuntu-focal-0f54ed4543247b7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/upgrade-pip-before-c-d2443847f9d58c7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/virtualenv-activation-6de5738c9db8241d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/yum-cache-removal-148c33012515e56e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/notes/yum-minimal-firmware-194846961a6a1cb9.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7596 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.834846 diskimage-builder-3.8.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/roles/dib-functests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-functests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/roles/dib-functests/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-functests/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/roles/dib-functests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-functests/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.062862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.834846 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.834846 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/base.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/extras.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/updates.repo.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/appstream.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/base.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/extras.repo.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.834846 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/fedora-updates.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/fedora.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2021-03-31 08:34:36.070862 diskimage-builder-3.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:35.834846 diskimage-builder-3.8.0/tests/elements/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/tests/elements/fake-os/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/elements/fake-os/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/elements/fake-os/element-provides
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-31 08:34:36.066862 diskimage-builder-3.8.0/tests/elements/fake-os/root.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      346 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/elements/fake-os/root.d/10-fake-os
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      534 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/install_test_deps.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1405 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/run_dib_library_tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13110 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/run_functests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2072 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tests/run_output_format_test.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2021-03-31 08:33:08.000000 diskimage-builder-3.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/.testr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.431034 diskimage-builder-3.9.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10124 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/.zuul.d/jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/.zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12436 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101041 2021-04-08 07:21:00.000000 diskimage-builder-3.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1934 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.431034 diskimage-builder-3.9.0/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9860 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/bin/dib-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.431034 diskimage-builder-3.9.0/contrib/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2562 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/contrib/setup-gate-mirrors.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.431034 diskimage-builder-3.9.0/diskimage_builder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder/block_device/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17835 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/blockdevice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9444 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder/block_device/level0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level0/localloop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13461 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15444 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/mbr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/partition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level1/partitioning.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder/block_device/level2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5420 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level2/mkfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder/block_device/level3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6752 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level3/mount.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.439034 diskimage-builder-3.9.0/diskimage_builder/block_device/level4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level4/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/level4/fstab.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6604 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.439034 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/bad_edge_graph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/bad_plugin.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/cmd_create.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/deep_graph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/deep_tree.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/duplicate_fs_labels.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/duplicate_name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/gpt_efi.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_graph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_partitions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1770 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv_vg.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_partition_ordering.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_spanned_vg.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/multi_key_node.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/multiple_partitions_graph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/multiple_partitions_tree.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/rollback.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/simple_graph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/simple_tree.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/too_long_fs_label.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/test_a.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/test_b.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6119 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3574 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_gpt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24482 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mbr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mkfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7778 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mount_order.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5527 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/block_device/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/disk_image_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12071 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/element_dependencies.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-conf/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-conf/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      592 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-conf/extra-data.d/99-override-default-apt-conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1635 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/extra-data.d/99-set-apt-package-pins
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.443034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      765 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/extra-data.d/99-override-default-apt-sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.375035 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/environment.d/00-set-apt-sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      128 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/extra-data.d/00-write-apt-sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      256 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/test-elements/test-sources/pre-install.d/00-test-apt-sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1200 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/cleanup.d/99-extract-kernel-and-ramdisk
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/base/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/environment.d/10-base-defaults
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/base/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      202 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/install.d/00-baseline-environment
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      256 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/install.d/00-up-to-date
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      368 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/install.d/10-cloud-init
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/base/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      453 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/base/pre-install.d/03-baseline-tools
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/block-device-default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/environment.d/15-block-device.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.447034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/block-device-default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/block-device-ppc64el.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/environment.d/15-block-device.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/block-device-default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/block-device-ppc64el.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/environment.d/15-block-device.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1477 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/cleanup.d/51-bootloader
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/environment.d/10-bootloader-default-cmdline
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10819 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/finalise.d/50-bootloader
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1244 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3717 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/bin/cache-url
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/tests/test_cache_url.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.451034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/environment.d/10-centos-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/environment.d/11-yum-dnf.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2287 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/pre-install.d/00-02-set-centos-mirror
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      775 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/pre-install.d/02-set-machine-id
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2242 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/root.d/10-centos-cloud-image
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.379035 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos/test-elements/8-stream-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/environment.d/10-centos-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/environment.d/11-yum-dnf.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.379035 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/7-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-aarch64-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-build-succeeds/environment.d/09-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/test-elements/8-stream-build-succeeds/environment.d/09-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.379035 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/7/yum.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.455034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/appstream.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8/base.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/appstream.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/yum.repos.d/8-stream/base.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/environment.d/00-centos7-element-deprecation.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/environment.d/09-centos7-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/environment.d/10-centos7-distro-name.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.379035 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/centos7/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.459034 diskimage-builder-3.9.0/diskimage_builder/elements/cleanup-kernel-initrd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cleanup-kernel-initrd/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1560 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/99-cleanup-kernel-initrd
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      307 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/post-install.d/20-enable-cloud-init
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      786 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/post-install.d/21-cloud-init-allow-password-auth
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1018 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/install.d/05-set-cloud-init-sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-disable-resizefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-disable-resizefs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/50-cloud-init-disable-resizefs
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-disable-resizefs/post-install.d/51-cloud-init-disable-growpart
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/environment.d/10-cloud-init-nocloud.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      323 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-nocloud/install.d/05-inject-local-source-data
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.463034 diskimage-builder-3.9.0/diskimage_builder/elements/debian/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1438 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/install.d/10-cloud-opinions
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.383035 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian/test-elements/build-succeeds/environment.d/09-debian-stable
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/environment.d/10-debian-minimal.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2432 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/root.d/75-debian-minimal-baseinstall
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.383035 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/stable-vm/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/test-elements/testing-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-systemd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-systemd/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-systemd/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-systemd/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      182 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-systemd/root.d/05-debian-systemd
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.467033 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      177 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/root.d/05-debian-upstart
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      712 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/root.d/20-debian-fix-upstart-jobs
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      809 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/cleanup.d/99-clean-up-cache
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/environment.d/10-debootstrap-default-locale
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/environment.d/20-network-interface-names
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1657 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/10-debian-networking
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1135 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/12-debian-locale-gen
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      754 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/15-cleanup-debootstrap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3199 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/root.d/08-debootstrap
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/binary-deps.d/deploy
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/init.d/80-deploy
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/binary-deps.d/deploy-kexec
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.471033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/init.d/81-deploy-kexec
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-kexec/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/binary-deps.d/deploy-targetcli
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/dracut-drivers.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/dracut-drivers.d/targetcli-drivers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      257 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/50-add-targetcli-module
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      741 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/iscsi-func
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      770 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/module-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      911 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/targetcli-wrapper
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/binary-deps.d/deploy-tgtadm
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      251 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/50-inject-tgtadm-iscsi-func
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/iscsi-func
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/environment.d/50-devuser
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/extra-data.d/50-devuser
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.475033 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      998 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/install.d/50-devuser
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/devuser/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3707 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/50-dhcp-all-interfaces
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      849 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/60-remove-cloud-image-interfaces
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/NetworkManager-conf.d-00-main.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces-udev.rules
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      700 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.init
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8438 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-interface@.service
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/environment.d/99-dib-init-system
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      781 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/install.d/20-install-init-scripts
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      674 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/post-install.d/10-enable-init-scripts
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      418 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/pre-install.d/04-dib-init-system
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      267 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/cleanup.d/50-dib-python
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/environment.d/50-dib-python-version
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      767 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/pre-install.d/01-dib-python
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.479033 diskimage-builder-3.9.0/diskimage_builder/elements/dib-run-parts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-run-parts/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dib-run-parts/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/dracut.conf.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/dracut.conf.d/disable-nouveau.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/modprobe.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-nouveau/modprobe.d/disable-nouveau.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/disable-selinux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-selinux/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/disable-selinux/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      195 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/disable-selinux/post-install.d/15-disable-selinux
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      832 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dkms/post-install.d/97-dkms
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/docker/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/docker/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/docker/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1203 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/docker/extra-data.d/01-docker-minimal
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/docker/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1095 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/docker/root.d/08-docker
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2120 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/bin/install-packages
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      364 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/cleanup.d/40-unblock-daemons
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      202 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/cleanup.d/50-remove-img-build-proxy
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      224 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/cleanup.d/60-untrim-dpkg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.483033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/environment.d/10-dpkg.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      216 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/finalise.d/99-clean-up-cache
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1368 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/finalise.d/99-write-dpkg-manifest
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      264 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/pre-install.d/00-disable-apt-recommends
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      170 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/pre-install.d/99-apt-get-update
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      871 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/09-apt-keyring
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      486 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-block-apt-translations
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-block-daemons
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      308 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-build-with-http-cache
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      376 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-shared-apt-cache
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      403 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-trim-dpkg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-network/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/binary-deps.d/dracut-ramdisk
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/dracut-drivers.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/dracut-drivers.d/base-drivers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/environment.d/10-dracut-version.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.387035 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.387035 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      543 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/deploy-cmdline.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      305 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/module-setup.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/init.d/00-override-troubleshoot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.487033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      669 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/install.d/20-install-dracut-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      625 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/01-ensure-drivers
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3006 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/99-build-dracut-ramdisk
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/source-repository-dracut
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/environment.d/10-dracut-regenerate
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      561 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/50-dracut-conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3604 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/finalise.d/50-dracut-regenerate
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/systemd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/systemd/dynamic-login.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      584 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/dynamic-login.init
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/upstart/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/upstart/dynamic-login.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      267 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/install.d/70-enable-dynamic-login-services
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/usr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/usr/local/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1165 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/dynamic-login
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/element-manifest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/element-manifest/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/element-manifest/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/element-manifest/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      363 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/element-manifest/extra-data.d/75-inject-element-manifest
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.491033 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/cleanup.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/cleanup.d/99-fix-grub
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1038 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/install.d/20-stty
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/install.d/serial-console-udev.rules
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/install.d/ttySx.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/ensure-venv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ensure-venv/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ensure-venv/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ensure-venv/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ensure-venv/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/epel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/epel/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/epel/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/epel/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/epel/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/epel/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1601 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/epel/pre-install.d/05-rpm-epel-release
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/environment.d/10-fedora-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/environment.d/11-yum-dnf.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      878 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/pre-install.d/00-02-set-fedora-mirror
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      616 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/pre-install.d/02-set-machine-id
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1896 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/root.d/10-fedora-cloud-image
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.495033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/environment.d/10-fedora-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/environment.d/11-yum-dnf.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.391035 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/yum.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1407 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/fix_shm
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3999 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/install-packages
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      948 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/unfix_shm
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1739 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/cleanup.d/05-unmount
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/environment.d/00-gentoo-envars.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/extra-data.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52263 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/extra-data.d/gentoo-releng.gpg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1414 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/finalise.d/99-cleanup
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.499033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      647 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-finalise.d/01-gentoo-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      475 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-00-set-profile
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      198 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-01-migrate-pax
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1640 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-02-flags
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      983 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-03-enable-overlays
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1447 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-04-install-desired-python
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5546 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/root.d/10-gentoo-image
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      771 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/root.d/50-gentoo-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/openrc/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      105 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/openrc/growroot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/systemd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/systemd/growroot.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/upstart/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/init-scripts/upstart/growroot.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      439 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/post-install.d/80-growroot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/usr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/usr/local/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/usr/local/sbin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      869 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/usr/local/sbin/growroot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.503033 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/grub2/post-install.d/01-delete-grubenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      468 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/post-install.d/95-hpdsa
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      197 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/post-install.d/98-hpdsa-post-dkms
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      358 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/pre-install.d/06-hpdsa
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      381 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/root.d/10-hpdsa-check-distro
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/binary-deps.d/hwburnin
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwburnin/init.d/70-hwburnin
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/binary-deps.d/hwdiscovery
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/init.d/60-hwdiscovery
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/systemd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/systemd/init-ibft-interfaces.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      633 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/init-ibft-interfaces.init
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/upstart/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/upstart/init-ibft-interfaces.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      394 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/post-install.d/70-init-ibft-interfaces
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.395035 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.507033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/etc/modules-load.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/etc/modules-load.d/ibft.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.399035 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/usr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.399035 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/sbin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      501 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/static/usr/local/sbin/init-ibft-interfaces.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      713 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/extra-data.d/50-ilo-firmware
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/init.d/50-ilo-firmware
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/ramdisk-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      165 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ilo/ramdisk-install.d/50-ilo-firmware
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-bin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-bin/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-bin/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      163 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-bin/pre-install.d/01-install-bin
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      422 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/install.d/10-install-static-files
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-static/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-types/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/install-types/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2387 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/install-types/extra-data.d/99-enable-install-types
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/environment.d/open-iscsi-config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      347 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/extra-data.d/50-check-dracut-regenerate
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      364 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/finalise.d/51-open-iscsi-config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.511033 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      243 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/post-install.d/open-iscsi-config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/iso/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2000 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/iso/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6553 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/cleanup.d/100-build-iso
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/iso/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1968 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/iso/post-install.d/01-copy-bootloaders
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/journal-to-console/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/journal-to-console/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/journal-to-console/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      809 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/journal-to-console/post-install.d/30-journal-to-console
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/environment.d/62-ssh-key
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      355 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/extra-data.d/62-ssh-key
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      592 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/install.d/62-ssh-key
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2075 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/local-config/pre-install.d/02-proxy-settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2369 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/finalise.d/60-bootloader
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      408 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/lvm/root.d/10-lvm-check-distro
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1688 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/cleanup.d/01-copy-manifests-dir
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/environment.d/14-manifests
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.515033 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      754 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/manifests/extra-data.d/20-manifest-dir
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/init.d/01-mellanox
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      542 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/install.d/65-mellanox
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/install.d/mellanox-rules.udev
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/udev.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/udev.d/81-mellanox-drivers.rules
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      944 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/extra-data.d/50-modprobe-blacklist
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      241 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/install.d/80-modprobe-blacklist
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe-blacklist/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe-blacklist/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe-blacklist/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      275 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/modprobe-blacklist/install.d/80-modprobe-blacklist
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/no-final-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/no-final-image/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/yum.repos.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/yum.repos.d/fedora-oat.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.519033 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      629 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/post-install.d/80-enable-sshd-service
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1364 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/post-install.d/99-harden-sshd-config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/11-dib-distribution-mirror.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      372 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/extra-data.d/75-copy-mirror-info
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1105 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/10-apt-disable-gpg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/environment.d/10-opensuse-distro-name.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      284 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/extra-data.d/01-inject-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2258 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/root.d/10-opensuse-cloud-image
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.403035 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/test-elements/opensuse15-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/environment.d/10-opensuse-distro-name.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.403035 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.523033 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/opensuse-minimal/test-elements/opensuse15-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4469 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1548 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7597 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs-squash
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4917 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs-v2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1417 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-uninstalls
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      254 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/extra-data.d/99-squash-package-install
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      192 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/install.d/01-package-installs
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      206 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/install.d/99-package-uninstalls
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      197 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/post-install.d/00-package-installs
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      211 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/post-install.d/95-package-uninstalls
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/pre-install.d/10-package-installs
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      210 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/pre-install.d/99-package-uninstalls
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.527032 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7323 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/tests/test_package_squash.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4166 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/51-pip-and-virutalenv-default.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.407035 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/install.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10820 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/04-install-pip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      272 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/post-install.d/89-clean-up-pip-cache
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/source-repository-pip-and-virtualenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.407035 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-fedora/environment.d/10-source-installtype-pip-and-virtualenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-opensuse/environment.d/10-source-installtype-pip-and-virtualenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/test-elements/source-install-ubuntu/environment.d/10-source-installtype-pip-and-virtualenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/environment.d/10-pip-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      248 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/root.d/11-pip-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6850 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/bin/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.531032 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/extra-data.d/10-create-pkg-map-dir
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/posix/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/posix/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/posix/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/posix/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7865 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/posix/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1809 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/install.d/65-proliant-tools-install
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      361 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/extra-data.d/00-mount-pypi-mirror
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      192 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/post-install.d/00-unconfigure-pypi-mirror
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2818 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/pypi/pre-install.d/04-configure-pypi-mirror
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      997 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/post-install.d/55-brick-client-install
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.535032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1127 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/install.d/70-python-build
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      324 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/post-install.d/70-python-build
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/source-repository-pyenv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.407035 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/environment.d/70-test-python-stow.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/69-test-python-stow
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      723 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/71-test-python-stow
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/binary-deps.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/binary-deps.d/ramdisk
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/init.d/10-start-base-system
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/init.d/30-start-network
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      176 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/install.d/20-install-dhcp-client
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      120 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/install.d/52-ramdisk-install-busybox
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1875 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/post-install.d/99-build-ramdisk
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      300 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/cleanup.d/99-extract-ramdisk-files
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      391 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/01-inject-ramdisk-build-files
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7628 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/init-func
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      952 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init-end
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/init.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/init.d/20-init-variables
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/init.d/40-check-network-ready
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1082 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/post-install.d/01-ensure-binaries
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.539032 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/udev.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5654 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/udev.d/60-persistent-storage.rules
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1127 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/install.d/05-xen-tools
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3253 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/install.d/10-nova-agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/source-repository-nova-agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/source-repository-xen-tools
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/bin/extract-image
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3952 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/bin/map-packages
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/environment.d/50-redhat-common
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      565 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/finalise.d/01-clean-old-kernels
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.543032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/environment.d/10-rhel-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/environment.d/11-yum-dnf.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      775 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/pre-install.d/02-set-machine-id
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1388 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel/root.d/10-rhel-cloud-image
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10571 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      910 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/finalise.d/60-unregister
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      288 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/install.d/10-openstack-selinux-rhel
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.411034 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/os-refresh-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5645 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/06-rhel-registration
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4220 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhel-registration
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2338 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhsm
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      288 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/10-rhel-blacklist
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/environment.d/00-rhel7-element-deprecation.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/environment.d/10-rhel7-distro-name.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4646 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/cleanup.d/99-selinux-fixfiles-restore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      359 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/post-install.d/06-network-config-nonzeroconf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.547032 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      476 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/pre-install.d/00-fix-requiretty
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      179 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/pre-install.d/00-usr-local-bin-secure-path
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1007 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/pre-install.d/01-override-yum-arch
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      320 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/cleanup.d/90-remove-ssh-host-keys
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.411034 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/systemd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/systemd/ssh-keygen.service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/upstart/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/init-scripts/upstart/ssh-keygen.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      801 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/80-ssh-keygen
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.411034 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.415034 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.415034 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1043 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/runtime-ssh-host-keys.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/select-boot-kernel-initrd
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/cleanup.d/99-remove-dib-img-functions
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/extra-data.d/99-copy-dib-img-functions
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/selinux-permissive/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/selinux-permissive/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/selinux-permissive/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      193 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/selinux-permissive/pre-install.d/11-selinux-permissive
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2717 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.551032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/environment.d/15-simple-init-networkmanager
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/environment.d/50-disable-cloud-init
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      898 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/50-simple-init
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      984 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/60-simple-init-remove-interfaces
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      968 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/40-glean
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      959 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/40-glean
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1307 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/post-install.d/80-simple-init
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/source-repository-simple-init
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5879 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12420 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/extra-data.d/98-source-repositories
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/install.d/02-stable-interface-names
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/stable-interface-names/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3036 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.555032 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1519 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/bin/svc-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2829 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/extra-data.d/10-merge-svc-map-files
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      203 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/extra-data.d/11-copy-svc-map-file
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6156 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/tests/test_data_merge.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1208 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/bin/sysctl-set-value
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      995 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/bin/sysctl-write-value
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/sysprep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/sysprep/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/sysprep/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      226 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/sysprep/finalise.d/01-clear-machine-id
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/uboot/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/uboot/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/uboot/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      916 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/uboot/cleanup.d/98-uboot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/environment.d/99-cloud-init-datasources.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      115 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/post-install.d/99-autoremove
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      269 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/pre-install.d/00-remove-apt-xapian-index
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      393 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/pre-install.d/00-remove-grub
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/pre-install.d/01-set-ubuntu-mirror
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2816 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/root.d/10-cache-ubuntu-tarball
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.419034 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/bionic-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/test-elements/xenial-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/environment.d/10-ubuntu-distro-name.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/environment.d/11-ubuntu-init-system.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.559032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1401 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/install.d/80-disable-rfc3041
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/environment.d/11-ubuntu-kernel.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/environment.d/12-ubuntu-repo-dists.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2089 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/root.d/75-ubuntu-minimal-baseinstall
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.419034 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-arm64-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/bionic-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-arm64-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.563032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/focal-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/test-elements/xenial-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1138 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/post-install.d/90-get-signed-kernel
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1871 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/75-ubuntu-minimal-baseinstall
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.419034 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/bionic-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.567032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/trusty-build-succeeds/environment.d/10-set-distro.bash
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.571032 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/environment.d/10-set-distro.bash
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/test-elements/xenial-build-succeeds/test-output-formats
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/vm/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/vm/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/vm/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      242 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/vm/finalise.d/50-remove-bogus-udev-links
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4551 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/bin/install-packages
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      400 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/cleanup.d/99-remove-yum-repo-conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/extra-data.d/99-yum-repo-conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      325 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/post-install.d/99-reset-yum-conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      425 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/00-01-yum-keepcache
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      261 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/00-dnf-update
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      871 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/01-00-centos-python3
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      525 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/01-module-configuration
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      271 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum/root.d/50-yum-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/cleanup.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1052 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/cleanup.d/95-remove-yum-mirror
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1447 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/install.d/10-base-networking
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      888 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/install.d/11-ensure-dbus-daemon
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/pkg-map
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3063 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/pre-install.d/03-yum-cleanup
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.575032 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14662 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/root.d/08-yum-chroot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/environment.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/environment.d/10-zipl-default-cmdline
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/finalise.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2002 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/finalise.d/50-zipl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      921 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zipl/pre-install.d/kernel_config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2107 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/bin/install-packages
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/install.d/01-login-defs
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      718 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/post-install.d/10-mkinitrd
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      150 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/post-install.d/98-zypper-clean-cache
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      189 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/post-install.d/99-zypper-no-keep-packages
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      180 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/pre-install.d/01-zypper-keep-packages
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      297 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper/root.d/50-zypper-cache
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/element-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      285 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/post-install.d/01-locale-cleanup
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      416 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/pre-install.d/00-disable-zypper-recommends
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.579032 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5982 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/root.d/08-zypper-chroot
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.583032 diskimage-builder-3.9.0/diskimage_builder/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/common-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17655 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/common-functions
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/dib-block-device.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4614 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/dib-run-parts
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/die
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24545 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/disk-image-create
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/element-info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/img-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9495 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/img-functions
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3007 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/outfilter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7843 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-functions
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24545 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-image-create
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/logging_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/paths.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.583032 diskimage-builder-3.9.0/diskimage_builder/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2071 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.583032 diskimage-builder-3.9.0/diskimage_builder/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9983 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/test_elementdeps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/test_loggingconfig.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/tests/test_no_dup_filenames.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/diskimage_builder/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.435034 diskimage-builder-3.9.0/diskimage_builder.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62645 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2021-04-08 07:21:01.000000 diskimage-builder-3.9.0/diskimage_builder.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.583032 diskimage-builder-3.9.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.583032 diskimage-builder-3.9.0/doc/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/lib/element_deps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.587031 diskimage-builder-3.9.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/ci.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7856 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.587031 diskimage-builder-3.9.0/doc/source/developer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/caches.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/components.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3429 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18143 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/developing_elements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1748 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/dib_lint.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/invocation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/stable_interfaces.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9552 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/developer/vhd_creation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/elements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.587031 diskimage-builder-3.9.0/doc/source/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/specs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.423034 diskimage-builder-3.9.0/doc/source/specs/v1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.587031 diskimage-builder-3.9.0/doc/source/specs/v1/approved/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7081 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/specs/v1/approved/block-device-lvl1-partitioning.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/specs/v1/approved/block-device-overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/specs/v1/approved/v1-template.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.587031 diskimage-builder-3.9.0/doc/source/user_guide/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23873 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/user_guide/building_an_image.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/user_guide/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/user_guide/install_types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/user_guide/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/doc/source/user_guide/supported_distros.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.423034 diskimage-builder-3.9.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.591031 diskimage-builder-3.9.0/playbooks/dib-functests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/playbooks/dib-functests/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/playbooks/dib-functests/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.591031 diskimage-builder-3.9.0/playbooks/dib-nodepool/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/playbooks/dib-nodepool/debootstrap.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/pylint.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/1.16.0-updates-bad91fc0b36c1755.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/1.17.0-ef744f36d277dba4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/1.18.0-4433d3076627f10d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/1.18.1-ceeb514708dcb731.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/Add-DIB-UBUNTU-KERNEL-5f75a809f3ce9bab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-6b94d90caea2895e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-aarch64-support-for-rhel-c62a0e02b1ad9033.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-centos-8-support-4fd28eb04e11ba43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-efi-packages-70a19464d31ab8d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-modprobe-element-8e3b0287ebb11920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/add-version-less-rhel-element-82fac7f2609e16d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/apt-transport-https-e4856cb9e2f8422c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/block-device-handling-279cddba8a859718.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/block-device-lvm-c3b8a214952b4db5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/block-device-mkfs-mount-fstab-42d7efe28fc2df04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/block-device-partitioning-237249e7ed2bad26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/block-device-update-partition-table-eb4ff077f90dfb19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/bootloader-commandline-d2db7524f1f9ad28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/bootloader-gpt-d1047f81f3a0631b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/centos-minimal-8-aca6314862741177.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/centos-minimal-8-stream-97021a2c92463dde.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/centos-retired-f17ae9f6f03e57e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/cloud-init-resizefs-growpart-e820b8c7f3adb78b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/create-945440b17d500bf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dash-p-after-install-58a87549c1c906c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/debian-minimal-confilicts-c139ab0c98e5762f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/debian-security-7279855cf464f88b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/debian-security-b4f677a148fdf9c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/deprecate-ironic-agent-element.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dhcp-all-interfaces-networkmanager-b34f2fc8fb1a678f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dhcp-vlan-interfaces-b34ab224b9431e3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-distribution-mirror-8c241c0d3d4a539a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-init-system-5647bad17a01c602.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-init-system_fix_for_debian_jessie-c6f7261ee84dad27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-python-deprecate-8401c35a87559076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-run-parts-6f67d038aa5a4156.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dib-run-parts-e18cc3a6c2d66c24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4181 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dibv2-omnibus-b30e0c7ecd76db8d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/doc-auto-element-dependency-cb7488c5bb7301a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dpkg-copy-keys-578e16f7fedd823b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/dracut-network-adaabf90da9f6866.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/efi-bios-images-052283eabba98b90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/efi-bootloader-disk-size-4c1a9f18967104fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/element-info-entry-point-448bf622be6061a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/element-override-ccda78c24ab4a4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/element-vars-c6bf2e6795002f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/ensure-venv-d7c16a2a04fd3b8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/fedora26-690b9fd9ac3c3d4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/fedora32-9dfa4d9d4dcce1ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/fix-dnf-clean-old-kernels-use-rpm-to-erase-in-case-running-kernel-0401f78d63daca77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/fix_rdisc6_loop-32a308a97de99f0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/gpt-esp-partition-size-200568cb6fcc8788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/grub-timeout-1cdd14a2b1467d89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/gzip-env-variable-94e61e0c043f4f1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/harden-sshd-config-3f84556136014f95.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/image-size-padding-24f88d1c4a215221.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/image-size-padding-mb-574104d40fdd2345.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/incorrect-grub-label-5d2000215c0cc73e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/init-ibft-interfaces-9458d97dfcecc3ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/journal-console-752b46542ec5595e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/logfile-quiet-b18f2de4059eecfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/move_tidy_logs_to_main-a8c03427fe1a445c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/no-ironic-agent-689e58268e1bf44f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/openssh-server-0f6d065748a2fc18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/opensuse-150-default-c047033b850d41ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/opensuse-151-default-67ccfffbc134704d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/opensuse-423-default-3bc73fff69374cd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/opensuse-minimal-45267f5be1112c22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/package-install-arch-38bb5a6e61794fa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/package-installs-when-list-cfc00032271bae75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/package-outside-debootstrap-ac93e9ce991819f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/pip-and-virtualenv-args-5d3f2512edd7f3a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/pip-and-virtualenv-platform-removal-52e0d6a22829a3b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/post-root-stage-51da051bcdfbc55f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/pre-finalise-stage-574ae7886274bcba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/python-venv-d5b04fcf57e460bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/remove-dib-utils-37f70dfad54900a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/remove-solicit-delay-57a035b91922522a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/rhel-module-selection-e9f6f06ece1fb829.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/rhel-registration-4d4fe741321e9345.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/rhel7-element-deprecation-b0c1b57be8cd06ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/root-journal-size-618e064d6681699a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/runtime-ssh-host-keys-7a2fc873cc90d33e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/selinux-permissive-pre-install-ce19461ef17ec972.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/simple-init-nm-5d19e249c0a4560b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/simple-init-nm-delay-f579e05467785219.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/simple-init-nm-f0896124dee92a03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/skip-packages-env-c97e7b4820f9bfda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/squashfs-output-91c1f0dc37474d3c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/start-using-reno-446b3d52a467a273.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/sysprep-f3fd036bc1d2c405.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/sysprep-fixes-8890b968a8fa7ac1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/timestamp-43015aa5434e8ddb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/trusty-testing-removal-51160ee59c5477d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/ubuntu-arbitrary-images-c796f5c6dbd40679.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/ubuntu-focal-0f54ed4543247b7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/upgrade-pip-before-c-d2443847f9d58c7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/virtualenv-activation-6de5738c9db8241d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/yum-cache-removal-148c33012515e56e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/notes/yum-minimal-firmware-194846961a6a1cb9.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7596 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/roles/dib-functests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-functests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/roles/dib-functests/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-functests/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/roles/dib-functests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-functests/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.607031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/base.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/extras.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/7/updates.repo.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/appstream.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/base.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/centos-minimal/8/extras.repo.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/fedora-updates.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/templates/fedora-minimal/default/fedora.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2021-04-08 07:21:01.615031 diskimage-builder-3.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.427034 diskimage-builder-3.9.0/tests/elements/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/tests/elements/fake-os/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/elements/fake-os/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/elements/fake-os/element-provides
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-08 07:21:01.611031 diskimage-builder-3.9.0/tests/elements/fake-os/root.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      346 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/elements/fake-os/root.d/10-fake-os
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      534 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/install_test_deps.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1405 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/run_dib_library_tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13110 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/run_functests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2072 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tests/run_output_format_test.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2021-04-08 07:20:27.000000 diskimage-builder-3.9.0/tox.ini
```

### Comparing `diskimage-builder-3.8.0/.zuul.d/jobs.yaml` & `diskimage-builder-3.9.0/.zuul.d/jobs.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/.zuul.d/project.yaml` & `diskimage-builder-3.9.0/.zuul.d/project.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/AUTHORS` & `diskimage-builder-3.9.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
 loki <lokesh.s@hp.com>
 melissaml <ma.lei@99cloud.net>
 nishagbkar <nisha.ee.iitb@gmail.com>
 nizam <abdul.nizamuddin@nectechnologies.in>
 pengyuesheng <pengyuesheng@gohighsec.com>
 sayalilunkad <sayali.lunkad@suse.com>
 sjing <sjing@cn.ibm.com>
+smoshiur1237 <moshiur.rahman@est.tech>
 stephane <stephane@alum.mit.edu>
 tanlin <lin.tan@intel.com>
 vmud213 <vinay50muddu@yahoo.com>
 wangqi <wang.qi@99cloud.net>
 weiyj <weiyuanjun@inspur.com>
 xhzhf <guoyongxhzhf@163.com>
 yatin <ykarel@redhat.com>
```

### Comparing `diskimage-builder-3.8.0/ChangeLog` & `diskimage-builder-3.9.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+3.9.0
+-----
+
+* Properly set grub2 root device when using efi
+* Make DIB\_DNF\_MODULE\_STREAMS part of yum element
+* Fix: IPA image buidling with OpenSuse
+
 3.8.0
 -----
 
 * update gentoo keywords to support gcc-10
 * replace the link which is in the 06-hpdsa file
 * Only add rhel base repos when REG\_REPOS is not set
 * Support secure-boot bootloader where possible
```

### Comparing `diskimage-builder-3.8.0/LICENSE` & `diskimage-builder-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/PKG-INFO` & `diskimage-builder-3.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: diskimage-builder
-Version: 3.8.0
+Version: 3.9.0
 Summary: Golden Disk Image builder.
 Home-page: https://docs.openstack.org/diskimage-builder/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License (2.0)
 Description: Image building tools for OpenStack
         ==================================
```

### Comparing `diskimage-builder-3.8.0/README.rst` & `diskimage-builder-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/bin/dib-lint` & `diskimage-builder-3.9.0/bin/dib-lint`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/bindep.txt` & `diskimage-builder-3.9.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/contrib/setup-gate-mirrors.sh` & `diskimage-builder-3.9.0/contrib/setup-gate-mirrors.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/blockdevice.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/blockdevice.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/cmd.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/cmd.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/config.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/config.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/exception.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/exception.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level0/localloop.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level0/localloop.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level1/lvm.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level1/lvm.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level1/mbr.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level1/mbr.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level1/partition.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level1/partition.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level1/partitioning.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level1/partitioning.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level2/mkfs.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level2/mkfs.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level3/mount.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level3/mount.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/level4/fstab.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/level4/fstab.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/plugin.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/plugin.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/duplicate_fs_labels.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/duplicate_fs_labels.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/gpt_efi.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/gpt_efi.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_graph.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_graph.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_partitions.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_partitions.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv_vg.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_multiple_pv_vg.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_partition_ordering.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_partition_ordering.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/lvm_tree_spanned_vg.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/lvm_tree_spanned_vg.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/multiple_partitions_graph.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/multiple_partitions_graph.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/multiple_partitions_tree.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/multiple_partitions_tree.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/config/rollback.yaml` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/config/rollback.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/test_a.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/test_a.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/plugin/test_b.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/plugin/test_b.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_base.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_config.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_gpt.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_lvm.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mbr.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mbr.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mkfs.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mkfs.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_mount_order.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_mount_order.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_state.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/tests/test_utils.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/block_device/utils.py` & `diskimage-builder-3.9.0/diskimage_builder/block_device/utils.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/disk_image_create.py` & `diskimage-builder-3.9.0/diskimage_builder/disk_image_create.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/element_dependencies.py` & `diskimage-builder-3.9.0/diskimage_builder/element_dependencies.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/apt-conf/extra-data.d/99-override-default-apt-conf` & `diskimage-builder-3.9.0/diskimage_builder/elements/apt-conf/extra-data.d/99-override-default-apt-conf`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/apt-preferences/extra-data.d/99-set-apt-package-pins` & `diskimage-builder-3.9.0/diskimage_builder/elements/apt-preferences/extra-data.d/99-set-apt-package-pins`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/apt-sources/extra-data.d/99-override-default-apt-sources` & `diskimage-builder-3.9.0/diskimage_builder/elements/apt-sources/extra-data.d/99-override-default-apt-sources`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/baremetal/cleanup.d/99-extract-kernel-and-ramdisk` & `diskimage-builder-3.9.0/diskimage_builder/elements/baremetal/cleanup.d/99-extract-kernel-and-ramdisk`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/base/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/base/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/base/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/base/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/block-device-efi/block-device-default.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/block-device-efi/block-device-default.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/block-device-gpt/block-device-ppc64el.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/block-device-gpt/block-device-ppc64el.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/block-device-mbr/block-device-ppc64el.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/block-device-mbr/block-device-ppc64el.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/cleanup.d/51-bootloader` & `diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/cleanup.d/51-bootloader`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/finalise.d/50-bootloader` & `diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/finalise.d/50-bootloader`

 * *Files 4% similar despite different names*

```diff
@@ -150,39 +150,39 @@
         # device.  ppc has a dedicated PReP boot partition.
         # For grub2 < 2.02~beta3 this needs to be a /dev/mapper/... node after
         # that a dev/loopXpN node will work fine.
         $GRUBNAME --modules="part_msdos" $GRUB_OPTS ${DEVICES[boot]} --no-nvram
     else
         # This set of modules is sufficient for all installs (mbr/gpt/efi)
         modules="part_msdos part_gpt lvm"
-        extra_options=""
         if [[ ${DIB_BLOCK_DEVICE} == "mbr" || ${DIB_BLOCK_DEVICE} == "gpt" ]]; then
             $GRUBNAME --modules="$modules biosdisk" $GRUB_OPTS $BOOT_DEV
         elif [[ ${DIB_BLOCK_DEVICE} == "efi" ]]; then
-            # This tells the EFI install to put the EFI binaries into
-            # the generic /BOOT directory and avoids trying to update
-            # nvram settings.
-            extra_options="--removable"
             # We need to manually set the target if it's different to
             # the host.  Setup for EFI
             case $ARCH in
                 "x86_64"|"amd64")
-                    GRUB_OPTS="--target=x86_64-efi"
                     # This call installs grub for BIOS compatability
                     # which makes portable EFI/BIOS images.
                     $GRUBNAME --modules="$modules" --target=i386-pc $BOOT_DEV
+                    # Set the x86_64 specific efi target for the generic
+                    # installation below.
+                    GRUB_OPTS="--target=x86_64-efi"
                     ;;
                 # At this point, we don't need to override the target
                 # for any other architectures.
             esac
-            if [ -d /boot/efi/$EFI_BOOT_DIR ]; then
-                # Make the grub config in the EFI directory for UEFI boot
-                $GRUB_MKCONFIG -o /boot/efi/$EFI_BOOT_DIR/grub.cfg
-            else
+            # If we don't have a distro specific dir with presigned efi targets
+            # we install a generic one.
+            if [ ! -d /boot/efi/$EFI_BOOT_DIR ]; then
                 echo "WARNING: /boot/efi/$EFI_BOOT_DIR does not exist, UEFI secure boot not supported"
+                # This tells the EFI install to put the EFI binaries into
+                # the generic /BOOT directory and avoids trying to update
+                # nvram settings.
+                extra_options="--removable"
                 $GRUBNAME --modules="$modules" $extra_options $GRUB_OPTS $BOOT_DEV
             fi
         fi
     fi
 
     # This might be better factored out into a per-distro 'install-bootblock'
     # helper.
@@ -222,14 +222,21 @@
     # Setting a flag to track whether the entry is already there in grub config
     PROBER_DISABLED=
     if ! grep -qe "^\s*GRUB_DISABLE_OS_PROBER=true" /etc/default/grub; then
         PROBER_DISABLED=true
         echo 'GRUB_DISABLE_OS_PROBER=true' >> /etc/default/grub
     fi
 
+    # GRUB_MKCONFIG call needs to happen after we configure
+    # /etc/default/grub above. Without this we can set inappropriate
+    # root device labels and then images don't boot.
+    #
+    # This produces a legacy config which both bios and uefi can boot
+    # Later we copy the final config to an efi specific location to
+    # support uefi specific functionality like secure boot.
     $GRUB_MKCONFIG -o $GRUB_CFG
 
     # Remove the fix to disable os_prober
     if [ -n "$PROBER_DISABLED" ]; then
         sed -i '$d' /etc/default/grub
     fi
 
@@ -248,14 +255,22 @@
 
     # when using efi, and having linux16/initrd16, it needs to be replaced
     # by linuxefi/initrdefi. When building images on a non-efi system,
     # the 16 suffix is added to linux/initrd entries, but we need it to be
     # linuxefi/initrdefi for the image to boot under efi
     if [[ ${DIB_BLOCK_DEVICE} == "efi" ]]; then
         sed -i 's%\(linux\|initrd\)16 /boot%\1efi /boot%g' $GRUB_CFG
+
+        # Finally copy the grub.cfg to the EFI specific dir to support
+        # functionality like secure boot. We make a copy because
+        # /boot and /boot/efi may be different partitions and uefi looks
+        # for a specific partition UUID preventing symlinks from working.
+        if [ -d /boot/efi/$EFI_BOOT_DIR ] ; then
+            cp $GRUB_CFG /boot/efi/$EFI_BOOT_DIR/grub.cfg
+        fi
     fi
 }
 
 DIB_EXTLINUX=${DIB_EXTLINUX:-0}
 if [ "$DIB_EXTLINUX" != "0" ]; then
     install_extlinux
 else
```

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/bootloader/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/bootloader/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/bin/cache-url` & `diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/bin/cache-url`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cache-url/tests/test_cache_url.py` & `diskimage-builder-3.9.0/diskimage_builder/elements/cache-url/tests/test_cache_url.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos/pre-install.d/00-02-set-centos-mirror` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos/pre-install.d/00-02-set-centos-mirror`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos/pre-install.d/02-set-machine-id` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos/pre-install.d/02-set-machine-id`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos/root.d/10-centos-cloud-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos/root.d/10-centos-cloud-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos-minimal/environment.d/10-centos-distro-name.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos-minimal/environment.d/10-centos-distro-name.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/centos7/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/centos7/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/99-cleanup-kernel-initrd` & `diskimage-builder-3.9.0/diskimage_builder/elements/cleanup-kernel-initrd/cleanup.d/99-cleanup-kernel-initrd`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init/post-install.d/21-cloud-init-allow-password-auth` & `diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init/post-install.d/21-cloud-init-allow-password-auth`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/cloud-init-datasources/install.d/05-set-cloud-init-sources` & `diskimage-builder-3.9.0/diskimage_builder/elements/cloud-init-datasources/install.d/05-set-cloud-init-sources`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debian/install.d/10-cloud-opinions` & `diskimage-builder-3.9.0/diskimage_builder/elements/debian/install.d/10-cloud-opinions`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/environment.d/10-debian-minimal.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/environment.d/10-debian-minimal.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debian-minimal/root.d/75-debian-minimal-baseinstall` & `diskimage-builder-3.9.0/diskimage_builder/elements/debian-minimal/root.d/75-debian-minimal-baseinstall`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debian-upstart/root.d/20-debian-fix-upstart-jobs` & `diskimage-builder-3.9.0/diskimage_builder/elements/debian-upstart/root.d/20-debian-fix-upstart-jobs`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/cleanup.d/99-clean-up-cache` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/cleanup.d/99-clean-up-cache`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/10-debian-networking` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/10-debian-networking`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/12-debian-locale-gen` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/12-debian-locale-gen`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/install.d/15-cleanup-debootstrap` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/install.d/15-cleanup-debootstrap`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/debootstrap/root.d/08-debootstrap` & `diskimage-builder-3.9.0/diskimage_builder/elements/debootstrap/root.d/08-debootstrap`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/deploy-baremetal/init.d/80-deploy` & `diskimage-builder-3.9.0/diskimage_builder/elements/deploy-baremetal/init.d/80-deploy`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/iscsi-func` & `diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/iscsi-func`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/module-setup.sh` & `diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/module-setup.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/targetcli-wrapper` & `diskimage-builder-3.9.0/diskimage_builder/elements/deploy-targetcli/extra-data.d/module/targetcli-wrapper`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/iscsi-func` & `diskimage-builder-3.9.0/diskimage_builder/elements/deploy-tgtadm/extra-data.d/scripts/iscsi-func`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/devuser/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/devuser/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/devuser/install.d/50-devuser` & `diskimage-builder-3.9.0/diskimage_builder/elements/devuser/install.d/50-devuser`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/50-dhcp-all-interfaces` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/50-dhcp-all-interfaces`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/60-remove-cloud-image-interfaces` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/60-remove-cloud-image-interfaces`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/NetworkManager-conf.d-00-main.conf` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/NetworkManager-conf.d-00-main.conf`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.init` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.sh` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-all-interfaces.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-interface@.service` & `diskimage-builder-3.9.0/diskimage_builder/elements/dhcp-all-interfaces/install.d/dhcp-interface@.service`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/environment.d/99-dib-init-system` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/environment.d/99-dib-init-system`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/install.d/20-install-init-scripts` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/install.d/20-install-init-scripts`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-init-system/post-install.d/10-enable-init-scripts` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-init-system/post-install.d/10-enable-init-scripts`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/environment.d/50-dib-python-version` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/environment.d/50-dib-python-version`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-python/pre-install.d/01-dib-python` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-python/pre-install.d/01-dib-python`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dib-run-parts/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dib-run-parts/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dkms/post-install.d/97-dkms` & `diskimage-builder-3.9.0/diskimage_builder/elements/dkms/post-install.d/97-dkms`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/docker/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/docker/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/docker/extra-data.d/01-docker-minimal` & `diskimage-builder-3.9.0/diskimage_builder/elements/docker/extra-data.d/01-docker-minimal`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/docker/root.d/08-docker` & `diskimage-builder-3.9.0/diskimage_builder/elements/docker/root.d/08-docker`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/bin/install-packages` & `diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/bin/install-packages`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/finalise.d/99-write-dpkg-manifest` & `diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/finalise.d/99-write-dpkg-manifest`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/09-apt-keyring` & `diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/09-apt-keyring`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dpkg/root.d/50-block-daemons` & `diskimage-builder-3.9.0/diskimage_builder/elements/dpkg/root.d/50-block-daemons`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/deploy-cmdline.sh` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/extra-data.d/scripts/module/deploy-cmdline.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/install.d/20-install-dracut-deps` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/install.d/20-install-dracut-deps`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/01-ensure-drivers` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/01-ensure-drivers`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/99-build-dracut-ramdisk` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-ramdisk/post-install.d/99-build-dracut-ramdisk`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/50-dracut-conf` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/extra-data.d/50-dracut-conf`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dracut-regenerate/finalise.d/50-dracut-regenerate` & `diskimage-builder-3.9.0/diskimage_builder/elements/dracut-regenerate/finalise.d/50-dracut-regenerate`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/dynamic-login.init` & `diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/init-scripts/sysv/dynamic-login.init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/dynamic-login` & `diskimage-builder-3.9.0/diskimage_builder/elements/dynamic-login/static/usr/local/bin/dynamic-login`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/enable-serial-console/install.d/20-stty` & `diskimage-builder-3.9.0/diskimage_builder/elements/enable-serial-console/install.d/20-stty`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/epel/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/epel/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/epel/pre-install.d/05-rpm-epel-release` & `diskimage-builder-3.9.0/diskimage_builder/elements/epel/pre-install.d/05-rpm-epel-release`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/environment.d/10-fedora-distro-name.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/environment.d/10-fedora-distro-name.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/package-installs.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/package-installs.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/pre-install.d/00-02-set-fedora-mirror` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/pre-install.d/00-02-set-fedora-mirror`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/pre-install.d/02-set-machine-id` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/pre-install.d/02-set-machine-id`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora/root.d/10-fedora-cloud-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora/root.d/10-fedora-cloud-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/yum.repo` & `diskimage-builder-3.9.0/diskimage_builder/elements/fedora-minimal/yum.repos.d/yum.repo`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/fix_shm` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/fix_shm`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/install-packages` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/install-packages`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/bin/unfix_shm` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/bin/unfix_shm`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/cleanup.d/05-unmount` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/cleanup.d/05-unmount`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/environment.d/00-gentoo-envars.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/environment.d/00-gentoo-envars.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/extra-data.d/gentoo-releng.gpg` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/extra-data.d/gentoo-releng.gpg`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/finalise.d/99-cleanup` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/finalise.d/99-cleanup`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-finalise.d/01-gentoo-cache` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-finalise.d/01-gentoo-cache`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-02-flags` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-02-flags`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-03-enable-overlays` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-03-enable-overlays`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-04-install-desired-python` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/pre-install.d/02-gentoo-04-install-desired-python`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/root.d/10-gentoo-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/root.d/10-gentoo-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/gentoo/root.d/50-gentoo-cache` & `diskimage-builder-3.9.0/diskimage_builder/elements/gentoo/root.d/50-gentoo-cache`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/growroot/static/usr/local/sbin/growroot` & `diskimage-builder-3.9.0/diskimage_builder/elements/growroot/static/usr/local/sbin/growroot`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/grub2/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/grub2/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/hpdsa/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/hpdsa/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/hwdiscovery/init.d/60-hwdiscovery` & `diskimage-builder-3.9.0/diskimage_builder/elements/hwdiscovery/init.d/60-hwdiscovery`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/init-ibft-interfaces.init` & `diskimage-builder-3.9.0/diskimage_builder/elements/ibft-interfaces/init-scripts/sysv/init-ibft-interfaces.init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ilo/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/ilo/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ilo/extra-data.d/50-ilo-firmware` & `diskimage-builder-3.9.0/diskimage_builder/elements/ilo/extra-data.d/50-ilo-firmware`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ilo/init.d/50-ilo-firmware` & `diskimage-builder-3.9.0/diskimage_builder/elements/ilo/init.d/50-ilo-firmware`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/install-types/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/install-types/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/install-types/extra-data.d/99-enable-install-types` & `diskimage-builder-3.9.0/diskimage_builder/elements/install-types/extra-data.d/99-enable-install-types`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/iscsi-boot/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/iscsi-boot/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/iso/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/iso/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/iso/cleanup.d/100-build-iso` & `diskimage-builder-3.9.0/diskimage_builder/elements/iso/cleanup.d/100-build-iso`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/iso/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/iso/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/iso/post-install.d/01-copy-bootloaders` & `diskimage-builder-3.9.0/diskimage_builder/elements/iso/post-install.d/01-copy-bootloaders`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/journal-to-console/post-install.d/30-journal-to-console` & `diskimage-builder-3.9.0/diskimage_builder/elements/journal-to-console/post-install.d/30-journal-to-console`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/local-config/install.d/62-ssh-key` & `diskimage-builder-3.9.0/diskimage_builder/elements/local-config/install.d/62-ssh-key`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/local-config/pre-install.d/02-proxy-settings` & `diskimage-builder-3.9.0/diskimage_builder/elements/local-config/pre-install.d/02-proxy-settings`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/lvm/finalise.d/60-bootloader` & `diskimage-builder-3.9.0/diskimage_builder/elements/lvm/finalise.d/60-bootloader`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/manifests/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/manifests/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/manifests/cleanup.d/01-copy-manifests-dir` & `diskimage-builder-3.9.0/diskimage_builder/elements/manifests/cleanup.d/01-copy-manifests-dir`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/manifests/environment.d/14-manifests` & `diskimage-builder-3.9.0/diskimage_builder/elements/manifests/environment.d/14-manifests`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/manifests/extra-data.d/20-manifest-dir` & `diskimage-builder-3.9.0/diskimage_builder/elements/manifests/extra-data.d/20-manifest-dir`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/install.d/65-mellanox` & `diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/install.d/65-mellanox`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/mellanox/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/mellanox/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/modprobe/extra-data.d/50-modprobe-blacklist` & `diskimage-builder-3.9.0/diskimage_builder/elements/modprobe/extra-data.d/50-modprobe-blacklist`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/no-final-image/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/no-final-image/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/oat-client/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/oat-client/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/post-install.d/80-enable-sshd-service` & `diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/post-install.d/80-enable-sshd-service`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/openssh-server/post-install.d/99-harden-sshd-config` & `diskimage-builder-3.9.0/diskimage_builder/elements/openssh-server/post-install.d/99-harden-sshd-config`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/11-dib-distribution-mirror.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/environment.d/11-dib-distribution-mirror.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/10-apt-disable-gpg` & `diskimage-builder-3.9.0/diskimage_builder/elements/openstack-ci-mirrors/root.d/10-apt-disable-gpg`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/environment.d/10-opensuse-distro-name.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/environment.d/10-opensuse-distro-name.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/opensuse/root.d/10-opensuse-cloud-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/opensuse/root.d/10-opensuse-cloud-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs-squash` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs-squash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-installs-v2` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-installs-v2`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/bin/package-uninstalls` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/bin/package-uninstalls`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/package-installs/tests/test_package_squash.py` & `diskimage-builder-3.9.0/diskimage_builder/elements/package-installs/tests/test_package_squash.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/51-pip-and-virutalenv-default.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/environment.d/51-pip-and-virutalenv-default.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/04-install-pip` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/install.d/pip-and-virtualenv-source-install/04-install-pip`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/package-installs.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/package-installs.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-and-virtualenv/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-and-virtualenv/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pip-cache/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/pip-cache/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pkg-map/bin/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/pkg-map/bin/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/posix/package-installs.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/posix/package-installs.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/posix/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/posix/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/proliant-tools/install.d/65-proliant-tools-install` & `diskimage-builder-3.9.0/diskimage_builder/elements/proliant-tools/install.d/65-proliant-tools-install`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pypi/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/pypi/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/pypi/pre-install.d/04-configure-pypi-mirror` & `diskimage-builder-3.9.0/diskimage_builder/elements/pypi/pre-install.d/04-configure-pypi-mirror`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/python-brickclient/post-install.d/55-brick-client-install` & `diskimage-builder-3.9.0/diskimage_builder/elements/python-brickclient/post-install.d/55-brick-client-install`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/install.d/70-python-build` & `diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/install.d/70-python-build`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/71-test-python-stow` & `diskimage-builder-3.9.0/diskimage_builder/elements/python-stow-versions/test-elements/test-python-stow/install.d/71-test-python-stow`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/init.d/10-start-base-system` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/init.d/10-start-base-system`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/init.d/30-start-network` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/init.d/30-start-network`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk/post-install.d/99-build-ramdisk` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk/post-install.d/99-build-ramdisk`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/init-func` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/d/init-func`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/extra-data.d/scripts/init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/init.d/20-init-variables` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/init.d/20-init-variables`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/post-install.d/01-ensure-binaries` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/post-install.d/01-ensure-binaries`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ramdisk-base/udev.d/60-persistent-storage.rules` & `diskimage-builder-3.9.0/diskimage_builder/elements/ramdisk-base/udev.d/60-persistent-storage.rules`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/install.d/05-xen-tools` & `diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/install.d/05-xen-tools`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rax-nova-agent/install.d/10-nova-agent` & `diskimage-builder-3.9.0/diskimage_builder/elements/rax-nova-agent/install.d/10-nova-agent`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/bin/extract-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/bin/extract-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/bin/map-packages` & `diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/bin/map-packages`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/finalise.d/01-clean-old-kernels` & `diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/finalise.d/01-clean-old-kernels`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/redhat-common/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/redhat-common/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel/pre-install.d/02-set-machine-id` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel/pre-install.d/02-set-machine-id`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel/root.d/10-rhel-cloud-image` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel/root.d/10-rhel-cloud-image`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 IMPORTANT NOTES:
 ----------------
 The 00-rhsm script is specific to RHEL6.  If you use the REG\_ variables to
 use with RHEL7, you do not need to set any DIB_RHSM variables.  The scripts
 named with "rhel-registration" have not been developed or tested for RHEL6.
 For information on building RHEL6 images, please see the rhel element README.
 
-The 01-module-configuration script is specific to RHEL8.  RHEL8 includes
-various versions of software which can be selected during installation, some
-may be older and/or incompatible with a given release of OpenStack.
-
 Environment Variables For Regisration during Image Creation
 -----------------------------------------------------------
 The following environment variables are used for registering a RHEL instance
 with either the Red Hat Customer Portal or Satellite 6.
 
 #### REG\_ACTIVATION\_KEY
 Attaches existing subscriptions as part of the registration process. The
@@ -245,25 +241,7 @@
             "repos":"rhel-7-server-optional-rpms,rhel-7-server-extras-rpms",
             "auto_attach":true,
             "activation_key": "my-key-SQQkh4",
             "org": "5643002",
             "method":"portal"
         }
     }
-
-
-Environment Variables for Module Selection during Image Creation
-----------------------------------------------------------------
-The following environment variable is used to select module streams to be
-enabled during an image build on RHEL8.  Any existing stream for the given
-module is first disabled prior to enabling the specified stream.
-
-#### DIB\_DNF\_MODULE\_STREAMS
-This is a space-separated list of module streams to enable prior to any
-RPMs being installed.
-
-Image Build Module Selection Example
-------------------------------------
-When using Train on RHEL8.2, one must select the appropriate virt and
-container-tools module streams:
-
-DIB_DNF_MODULE_STREAMS='virt:8.2 container-tools:2.0'
```

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/finalise.d/60-unregister` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/finalise.d/60-unregister`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/06-rhel-registration` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/06-rhel-registration`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhel-registration` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhel-registration`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhsm` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel-common/pre-install.d/00-rhsm`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel-common/pre-install.d/01-module-configuration` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/01-module-configuration`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rhel7/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/rhel7/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/cleanup.d/99-selinux-fixfiles-restore` & `diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/cleanup.d/99-selinux-fixfiles-restore`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/rpm-distro/pre-install.d/01-override-yum-arch` & `diskimage-builder-3.9.0/diskimage_builder/elements/rpm-distro/pre-install.d/01-override-yum-arch`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/80-ssh-keygen` & `diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/post-install.d/80-ssh-keygen`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/runtime-ssh-host-keys.sh` & `diskimage-builder-3.9.0/diskimage_builder/elements/runtime-ssh-host-keys/static/usr/local/sbin/runtime-ssh-host-keys.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/select-boot-kernel-initrd` & `diskimage-builder-3.9.0/diskimage_builder/elements/select-boot-kernel-initrd/bin/select-boot-kernel-initrd`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/50-simple-init` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/50-simple-init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/60-simple-init-remove-interfaces` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/60-simple-init-remove-interfaces`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/40-glean` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-repo-install/40-glean`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/40-glean` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/install.d/simple-init-source-install/40-glean`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/pkg-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/pkg-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/simple-init/post-install.d/80-simple-init` & `diskimage-builder-3.9.0/diskimage_builder/elements/simple-init/post-install.d/80-simple-init`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/source-repositories/extra-data.d/98-source-repositories` & `diskimage-builder-3.9.0/diskimage_builder/elements/source-repositories/extra-data.d/98-source-repositories`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/bin/svc-map` & `diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/bin/svc-map`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/extra-data.d/10-merge-svc-map-files` & `diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/extra-data.d/10-merge-svc-map-files`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/svc-map/tests/test_data_merge.py` & `diskimage-builder-3.9.0/diskimage_builder/elements/svc-map/tests/test_data_merge.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/bin/sysctl-set-value` & `diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/bin/sysctl-set-value`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/sysctl/bin/sysctl-write-value` & `diskimage-builder-3.9.0/diskimage_builder/elements/sysctl/bin/sysctl-write-value`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/uboot/cleanup.d/98-uboot` & `diskimage-builder-3.9.0/diskimage_builder/elements/uboot/cleanup.d/98-uboot`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/pre-install.d/01-set-ubuntu-mirror` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/pre-install.d/01-set-ubuntu-mirror`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu/root.d/10-cache-ubuntu-tarball` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu/root.d/10-cache-ubuntu-tarball`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/environment.d/10-ubuntu-distro-name.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/environment.d/10-ubuntu-distro-name.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-common/install.d/80-disable-rfc3041` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-common/install.d/80-disable-rfc3041`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/environment.d/11-ubuntu-kernel.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/environment.d/11-ubuntu-kernel.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/environment.d/12-ubuntu-repo-dists.bash` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/environment.d/12-ubuntu-repo-dists.bash`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/package-installs.yaml` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/package-installs.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-minimal/root.d/75-ubuntu-minimal-baseinstall` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-minimal/root.d/75-ubuntu-minimal-baseinstall`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-signed/post-install.d/90-get-signed-kernel` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-signed/post-install.d/90-get-signed-kernel`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/75-ubuntu-minimal-baseinstall` & `diskimage-builder-3.9.0/diskimage_builder/elements/ubuntu-systemd-container/root.d/75-ubuntu-minimal-baseinstall`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum/bin/install-packages` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum/bin/install-packages`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum/extra-data.d/99-yum-repo-conf` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum/extra-data.d/99-yum-repo-conf`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum/pre-install.d/01-00-centos-python3` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum/pre-install.d/01-00-centos-python3`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/cleanup.d/95-remove-yum-mirror` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/cleanup.d/95-remove-yum-mirror`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/install.d/10-base-networking` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/install.d/10-base-networking`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/install.d/11-ensure-dbus-daemon` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/install.d/11-ensure-dbus-daemon`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/pre-install.d/03-yum-cleanup` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/pre-install.d/03-yum-cleanup`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/yum-minimal/root.d/08-yum-chroot` & `diskimage-builder-3.9.0/diskimage_builder/elements/yum-minimal/root.d/08-yum-chroot`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zipl/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/zipl/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zipl/finalise.d/50-zipl` & `diskimage-builder-3.9.0/diskimage_builder/elements/zipl/finalise.d/50-zipl`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zipl/pre-install.d/kernel_config` & `diskimage-builder-3.9.0/diskimage_builder/elements/zipl/pre-install.d/kernel_config`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zypper/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/zypper/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zypper/bin/install-packages` & `diskimage-builder-3.9.0/diskimage_builder/elements/zypper/bin/install-packages`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zypper/post-install.d/10-mkinitrd` & `diskimage-builder-3.9.0/diskimage_builder/elements/zypper/post-install.d/10-mkinitrd`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/README.rst` & `diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/elements/zypper-minimal/root.d/08-zypper-chroot` & `diskimage-builder-3.9.0/diskimage_builder/elements/zypper-minimal/root.d/08-zypper-chroot`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/common-defaults` & `diskimage-builder-3.9.0/diskimage_builder/lib/common-defaults`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/common-functions` & `diskimage-builder-3.9.0/diskimage_builder/lib/common-functions`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/dib-run-parts` & `diskimage-builder-3.9.0/diskimage_builder/lib/dib-run-parts`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/die` & `diskimage-builder-3.9.0/diskimage_builder/lib/die`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/disk-image-create` & `diskimage-builder-3.9.0/diskimage_builder/lib/disk-image-create`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/img-defaults` & `diskimage-builder-3.9.0/diskimage_builder/lib/img-defaults`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/img-functions` & `diskimage-builder-3.9.0/diskimage_builder/lib/img-functions`

 * *Files 2% similar despite different names*

```diff
@@ -212,12 +212,15 @@
         fi
     elif [ -f $TARGET_ROOT/etc/SuSE-release ]; then
         KERNEL=$(basename $(readlink -e $BOOTDIR/vmlinuz))
         RAMDISK=$(basename $(readlink -e $BOOTDIR/initrd))
     elif [[ -f "${TARGET_ROOT}"/etc/gentoo-release ]]; then
         KERNEL="$(basename $(ls -1rv $BOOTDIR/vmlinuz-* | head -n 1))"
         RAMDISK="$(basename $(ls -1rv $BOOTDIR/initramfs-* | head -n 1))"
+    elif [[ $DISTRO_NAME = opensuse ]]; then
+        KERNEL=$(basename $(readlink -e $BOOTDIR/vmlinuz))
+        RAMDISK=$(basename $(readlink -e $BOOTDIR/initrd))
     else
         echo "ERROR: Unable to detect operating system"
         exit 1
     fi
 }
```

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/outfilter.py` & `diskimage-builder-3.9.0/diskimage_builder/lib/outfilter.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-defaults` & `diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-defaults`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-functions` & `diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-functions`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/lib/ramdisk-image-create` & `diskimage-builder-3.9.0/diskimage_builder/lib/ramdisk-image-create`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/logging_config.py` & `diskimage-builder-3.9.0/diskimage_builder/logging_config.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/paths.py` & `diskimage-builder-3.9.0/diskimage_builder/paths.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/tests/base.py` & `diskimage-builder-3.9.0/diskimage_builder/tests/base.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/tests/test_elementdeps.py` & `diskimage-builder-3.9.0/diskimage_builder/tests/test_elementdeps.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/tests/test_loggingconfig.py` & `diskimage-builder-3.9.0/diskimage_builder/tests/test_loggingconfig.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/tests/test_no_dup_filenames.py` & `diskimage-builder-3.9.0/diskimage_builder/tests/test_no_dup_filenames.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder/version.py` & `diskimage-builder-3.9.0/diskimage_builder/version.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/diskimage_builder.egg-info/PKG-INFO` & `diskimage-builder-3.9.0/diskimage_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: diskimage-builder
-Version: 3.8.0
+Version: 3.9.0
 Summary: Golden Disk Image builder.
 Home-page: https://docs.openstack.org/diskimage-builder/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License (2.0)
 Description: Image building tools for OpenStack
         ==================================
```

### Comparing `diskimage-builder-3.8.0/diskimage_builder.egg-info/SOURCES.txt` & `diskimage-builder-3.9.0/diskimage_builder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,14 @@
 diskimage_builder/elements/rhel/element-provides
 diskimage_builder/elements/rhel-common/README.rst
 diskimage_builder/elements/rhel-common/finalise.d/60-unregister
 diskimage_builder/elements/rhel-common/install.d/10-openstack-selinux-rhel
 diskimage_builder/elements/rhel-common/os-refresh-config/pre-configure.d/06-rhel-registration
 diskimage_builder/elements/rhel-common/pre-install.d/00-rhel-registration
 diskimage_builder/elements/rhel-common/pre-install.d/00-rhsm
-diskimage_builder/elements/rhel-common/pre-install.d/01-module-configuration
 diskimage_builder/elements/rhel-common/pre-install.d/10-rhel-blacklist
 diskimage_builder/elements/rhel/environment.d/10-rhel-distro-name.bash
 diskimage_builder/elements/rhel/environment.d/11-yum-dnf.bash
 diskimage_builder/elements/rhel/pre-install.d/02-set-machine-id
 diskimage_builder/elements/rhel/root.d/10-rhel-cloud-image
 diskimage_builder/elements/rhel7/README.rst
 diskimage_builder/elements/rhel7/element-deps
@@ -794,14 +793,15 @@
 diskimage_builder/elements/yum/bin/install-packages
 diskimage_builder/elements/yum/cleanup.d/99-remove-yum-repo-conf
 diskimage_builder/elements/yum/extra-data.d/99-yum-repo-conf
 diskimage_builder/elements/yum/post-install.d/99-reset-yum-conf
 diskimage_builder/elements/yum/pre-install.d/00-01-yum-keepcache
 diskimage_builder/elements/yum/pre-install.d/00-dnf-update
 diskimage_builder/elements/yum/pre-install.d/01-00-centos-python3
+diskimage_builder/elements/yum/pre-install.d/01-module-configuration
 diskimage_builder/elements/yum/root.d/50-yum-cache
 diskimage_builder/elements/zipl/README.rst
 diskimage_builder/elements/zipl/element-deps
 diskimage_builder/elements/zipl/element-provides
 diskimage_builder/elements/zipl/package-installs.yaml
 diskimage_builder/elements/zipl/environment.d/10-zipl-default-cmdline
 diskimage_builder/elements/zipl/finalise.d/50-zipl
```

### Comparing `diskimage-builder-3.8.0/diskimage_builder.egg-info/entry_points.txt` & `diskimage-builder-3.9.0/diskimage_builder.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/lib/element_deps.py` & `diskimage-builder-3.9.0/doc/lib/element_deps.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/ci.md` & `diskimage-builder-3.9.0/doc/source/ci.md`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/conf.py` & `diskimage-builder-3.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/caches.rst` & `diskimage-builder-3.9.0/doc/source/developer/caches.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/components.rst` & `diskimage-builder-3.9.0/doc/source/developer/components.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/design.rst` & `diskimage-builder-3.9.0/doc/source/developer/design.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/developing_elements.rst` & `diskimage-builder-3.9.0/doc/source/developer/developing_elements.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/dib_lint.rst` & `diskimage-builder-3.9.0/doc/source/developer/dib_lint.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/index.rst` & `diskimage-builder-3.9.0/doc/source/developer/index.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/invocation.rst` & `diskimage-builder-3.9.0/doc/source/developer/invocation.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/stable_interfaces.rst` & `diskimage-builder-3.9.0/doc/source/developer/stable_interfaces.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/developer/vhd_creation.rst` & `diskimage-builder-3.9.0/doc/source/developer/vhd_creation.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/index.rst` & `diskimage-builder-3.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/specs/README.rst` & `diskimage-builder-3.9.0/doc/source/specs/README.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/specs/v1/approved/block-device-lvl1-partitioning.rst` & `diskimage-builder-3.9.0/doc/source/specs/v1/approved/block-device-lvl1-partitioning.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/specs/v1/approved/block-device-overview.rst` & `diskimage-builder-3.9.0/doc/source/specs/v1/approved/block-device-overview.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/specs/v1/approved/v1-template.rst` & `diskimage-builder-3.9.0/doc/source/specs/v1/approved/v1-template.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/user_guide/building_an_image.rst` & `diskimage-builder-3.9.0/doc/source/user_guide/building_an_image.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/user_guide/install_types.rst` & `diskimage-builder-3.9.0/doc/source/user_guide/install_types.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/doc/source/user_guide/installation.rst` & `diskimage-builder-3.9.0/doc/source/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/lower-constraints.txt` & `diskimage-builder-3.9.0/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/1.16.0-updates-bad91fc0b36c1755.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/1.16.0-updates-bad91fc0b36c1755.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/1.17.0-ef744f36d277dba4.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/1.17.0-ef744f36d277dba4.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/block-device-handling-279cddba8a859718.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/block-device-handling-279cddba8a859718.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/centos-retired-f17ae9f6f03e57e3.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/centos-retired-f17ae9f6f03e57e3.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/dib-init-system-5647bad17a01c602.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/dib-init-system-5647bad17a01c602.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/dibv2-omnibus-b30e0c7ecd76db8d.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/dibv2-omnibus-b30e0c7ecd76db8d.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/ensure-venv-d7c16a2a04fd3b8f.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/ensure-venv-d7c16a2a04fd3b8f.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/start-using-reno-446b3d52a467a273.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/start-using-reno-446b3d52a467a273.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/notes/timestamp-43015aa5434e8ddb.yaml` & `diskimage-builder-3.9.0/releasenotes/notes/timestamp-43015aa5434e8ddb.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/releasenotes/source/conf.py` & `diskimage-builder-3.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/roles/dib-functests/tasks/main.yaml` & `diskimage-builder-3.9.0/roles/dib-functests/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/roles/dib-setup-gate-mirrors/tasks/main.yaml` & `diskimage-builder-3.9.0/roles/dib-setup-gate-mirrors/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/setup.cfg` & `diskimage-builder-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/setup.py` & `diskimage-builder-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/tests/install_test_deps.sh` & `diskimage-builder-3.9.0/tests/install_test_deps.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/tests/run_dib_library_tests.sh` & `diskimage-builder-3.9.0/tests/run_dib_library_tests.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/tests/run_functests.sh` & `diskimage-builder-3.9.0/tests/run_functests.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/tests/run_output_format_test.sh` & `diskimage-builder-3.9.0/tests/run_output_format_test.sh`

 * *Files identical despite different names*

### Comparing `diskimage-builder-3.8.0/tox.ini` & `diskimage-builder-3.9.0/tox.ini`

 * *Files identical despite different names*

