# Comparing `tmp/pytac-0.5.0.tar.gz` & `tmp/pytac-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytac-0.5.0.tar", last modified: Fri Jul  1 14:46:07 2022, max compression
+gzip compressed data, was "pytac-0.6.0b1.tar", last modified: Wed Apr 12 14:55:22 2023, max compression
```

## Comparing `pytac-0.5.0.tar` & `pytac-0.6.0b1.tar`

### file list

```diff
@@ -1,120 +1,197 @@
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    11357 2022-06-22 13:59:22.000000 pytac-0.5.0/LICENSE
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)      100 2022-06-22 13:59:22.000000 pytac-0.5.0/MANIFEST.in
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2485 2022-07-01 14:46:07.000000 pytac-0.5.0/PKG-INFO
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     1738 2022-06-22 14:00:14.000000 pytac-0.5.0/README.rst
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       89 2022-06-30 18:03:11.000000 pytac-0.5.0/pyproject.toml
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)      681 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/__init__.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     4912 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/cothread_cs.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2695 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/cs.py
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/DIAD/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35909 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191034 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24702 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:55:51.000000 pytac-0.5.0/pytac/data/DIAD/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13795 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38135 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIAD/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/DIADSP/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35909 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191034 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24702 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:55:59.000000 pytac-0.5.0/pytac/data/DIADSP/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13795 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38135 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADSP/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/DIADTHz/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35909 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191034 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24702 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:56:07.000000 pytac-0.5.0/pytac/data/DIADTHz/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13795 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38135 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/DIADTHz/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/I04/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    36657 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191326 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    25189 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13915 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38254 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/I04SP/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    36657 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191326 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    25189 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13915 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38254 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04SP/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/I04THz/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    36657 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191326 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    25189 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13915 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38254 2022-07-01 14:40:26.000000 pytac-0.5.0/pytac/data/I04THz/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35909 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191034 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24702 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:56:20.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21518 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13795 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38135 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/SRI0913_MOGA/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/VMX/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35881 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191517 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24674 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:56:28.000000 pytac-0.5.0/pytac/data/VMX/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21638 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13855 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38224 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMX/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/VMXSP/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35881 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191517 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24674 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:56:41.000000 pytac-0.5.0/pytac/data/VMXSP/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21638 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13855 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38224 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXSP/unitconv.csv
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac/data/VMXTHz/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    35881 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/elements.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)   191517 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/epics_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24674 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/families.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       45 2022-06-22 14:56:50.000000 pytac-0.5.0/pytac/data/VMXTHz/simple_devices.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    21638 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/uc_pchip_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    13855 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/uc_poly_data.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    38224 2022-06-22 15:14:06.000000 pytac-0.5.0/pytac/data/VMXTHz/unitconv.csv
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    11757 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/data_source.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     8131 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/device.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    11676 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/element.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)      661 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/exceptions.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    24831 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/lattice.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     9358 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/load_csv.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)    18850 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/units.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     1150 2022-06-22 13:59:22.000000 pytac-0.5.0/pytac/utils.py
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2485 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/PKG-INFO
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     3012 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/SOURCES.txt
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)        1 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/dependency_links.txt
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)        1 2022-06-30 18:03:18.000000 pytac-0.5.0/pytac.egg-info/not-zip-safe
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       12 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/requires.txt
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)        6 2022-07-01 14:46:07.000000 pytac-0.5.0/pytac.egg-info/top_level.txt
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     1174 2022-07-01 14:46:07.000000 pytac-0.5.0/setup.cfg
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)       39 2022-06-22 13:59:22.000000 pytac-0.5.0/setup.py
-drwxrwxr-x   0 lkz95212 (1208238) lkz95212 (1208238)        0 2022-07-01 14:46:07.000000 pytac-0.5.0/test/
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     3984 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_cothread_cs.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2156 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_data_source.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2901 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_device.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     6086 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_element.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     5320 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_epics.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     1230 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_invalid_classes.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     8476 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_lattice.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     2508 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_load.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     6905 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_machine.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)     6949 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_units.py
--rw-rw-r--   0 lkz95212 (1208238) lkz95212 (1208238)      691 2022-06-22 13:59:22.000000 pytac-0.5.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.789343 pytac-0.6.0b1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 14:55:14.000000 pytac-0.6.0b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 14:55:14.000000 pytac-0.6.0b1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-12 14:55:14.000000 pytac-0.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-04-12 14:55:22.813344 pytac-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-12 14:55:14.000000 pytac-0.6.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/control-structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/explanations/docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/explanations/what-is-pytac.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.797343 pytac-0.6.0b1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/tutorials/basic-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-12 14:55:14.000000 pytac-0.6.0b1/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-12 14:55:14.000000 pytac-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:55:22.813344 pytac-0.6.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/cothread_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/cs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/src/pytac/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac/data/DIAD/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIAD/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/DIADSP/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADSP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/DIADTHz/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/DIADTHz/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/I04/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.805344 pytac-0.6.0b1/src/pytac/data/I04SP/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04SP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/I04THz/
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191326 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25189 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38254 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/I04THz/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191034 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38135 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.809344 pytac-0.6.0b1/src/pytac/data/VMX/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMX/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/src/pytac/data/VMXSP/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXSP/unitconv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/src/pytac/data/VMXTHz/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191517 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/simple_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_pchip_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_poly_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data/VMXTHz/unitconv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/load_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 14:55:14.000000 pytac-0.6.0b1/src/pytac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.801344 pytac-0.6.0b1/src/pytac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 14:55:22.000000 pytac-0.6.0b1/src/pytac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.793343 pytac-0.6.0b1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/tests/data/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/elements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/epics_devices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/data/dummy/families.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_cothread_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_invalid_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 14:55:14.000000 pytac-0.6.0b1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:55:22.813344 pytac-0.6.0b1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-04-12 14:55:14.000000 pytac-0.6.0b1/utils/load_mml.m
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-12 14:55:14.000000 pytac-0.6.0b1/utils/load_unitconv.m
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytac-0.5.0/LICENSE` & `pytac-0.6.0b1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -174,23 +174,23 @@
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
    APPENDIX: How to apply the Apache License to your work.
 
       To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
+      boilerplate notice, with the fields enclosed by brackets "{}"
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Diamond Light Source Ltd.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pytac-0.5.0/pytac/cothread_cs.py` & `pytac-0.6.0b1/src/pytac/cothread_cs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 
-from cothread.catools import caget, caput, ca_nothing
+from cothread.catools import ca_nothing, caget, caput
 
 from pytac.cs import ControlSystem
 from pytac.exceptions import ControlSystemException
 
 
 class CothreadControlSystem(ControlSystem):
     """A control system using cothread to communicate with EPICS.
 
     N.B. this is the default control system. It is used to communicate over
     channel access with the hardware in the ring.
 
     **Methods:**
     """
 
-    def __init__(self, timeout=1.0):
+    def __init__(self, timeout=1.0, wait=False):
         self._timeout = timeout
+        self._wait = wait
 
     def get_single(self, pv, throw=True):
         """Get the value of a given PV.
 
         Args:
             pv (string): The process variable given as a string. It can be a
                          readback or a setpoint PV.
@@ -86,15 +87,15 @@
         Returns:
             bool: True for success, False for failure
 
         Raises:
             ControlSystemException: if it cannot connect to the specified PV.
         """
         try:
-            caput(pv, value, timeout=self._timeout, throw=True)
+            caput(pv, value, timeout=self._timeout, throw=True, wait=self._wait)
             return True
         except ca_nothing:
             error_msg = f"Cannot connect to {pv}."
             if throw:
                 raise ControlSystemException(error_msg)
             else:
                 logging.warning(error_msg)
@@ -117,15 +118,15 @@
 
         Raises:
             ValueError: if the lists of values and PVs are diffent lengths.
             ControlSystemException: if it cannot connect to one or more PVs.
         """
         if len(pvs) != len(values):
             raise ValueError("Please enter the same number of values as PVs.")
-        status = caput(pvs, values, timeout=self._timeout, throw=False)
+        status = caput(pvs, values, timeout=self._timeout, throw=False, wait=self._wait)
         return_values = []
         failures = []
         for stat in status:
             if not stat.ok:
                 return_values.append(False)
                 failures.append(stat)
                 logging.warning(f"Cannot connect to {stat.name}.")
```

### Comparing `pytac-0.5.0/pytac/cs.py` & `pytac-0.6.0b1/src/pytac/cs.py`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIAD/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIAD/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADSP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIADSP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/families.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/DIADTHz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/DIADTHz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04SP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04SP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/families.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/I04THz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/I04THz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/elements.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/families.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/SRI0913_MOGA/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/SRI0913_MOGA/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMX/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMX/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXSP/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMXSP/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/elements.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/elements.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/epics_devices.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/epics_devices.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/families.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/families.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/uc_pchip_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_pchip_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/uc_poly_data.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/uc_poly_data.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data/VMXTHz/unitconv.csv` & `pytac-0.6.0b1/src/pytac/data/VMXTHz/unitconv.csv`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/data_source.py` & `pytac-0.6.0b1/src/pytac/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         Args:
             data_source_type (str): the type of the data source being set
                                      pytac.LIVE or pytac.SIM.
 
         Raises:
             DataSourceException: if there is no data source on the given field.
-            """
+        """
         try:
             return self._data_sources[data_source_type]
         except KeyError:
             raise DataSourceException(
                 f"No data source {data_source_type} on manager {self}."
             )
```

### Comparing `pytac-0.5.0/pytac/device.py` & `pytac-0.6.0b1/src/pytac/device.py`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/pytac/element.py` & `pytac-0.6.0b1/src/pytac/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,25 +44,23 @@
         # Families are case insensitive but stored in lowercase.
         self._families = set()
         self._lattice = lattice
         self._data_source_manager = DataSourceManager()
 
     @property
     def index(self):
-        """int: The element's index within the ring, starting at 1.
-        """
+        """int: The element's index within the ring, starting at 1."""
         if self._lattice is None:
             return None
         else:
             return self._lattice._elements.index(self) + 1
 
     @property
     def s(self):
-        """float: The element's start position within the lattice in metres.
-        """
+        """float: The element's start position within the lattice in metres."""
         if self._lattice is None:
             return None
         else:
             return sum([el.length for el in self._lattice[: self.index - 1]])
 
     @property
     def cell(self):
@@ -263,15 +261,20 @@
             )
         except DataSourceException as e:
             raise DataSourceException(f"{self}: {e}")
         except FieldException as e:
             raise FieldException(f"{self}: {e}")
 
     def set_value(
-        self, field, value, units=pytac.DEFAULT, data_source=pytac.DEFAULT, throw=True,
+        self,
+        field,
+        value,
+        units=pytac.DEFAULT,
+        data_source=pytac.DEFAULT,
+        throw=True,
     ):
         """Set the value for a field.
 
         This value can be set on the machine or the simulation.
 
         Args:
             field (str): The requested field.
```

### Comparing `pytac-0.5.0/pytac/exceptions.py` & `pytac-0.6.0b1/src/pytac/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 """Module containing all the exceptions used in pytac."""
 
 
 class FieldException(Exception):
-    """Exception associated with invalid field requests.
-    """
+    """Exception associated with invalid field requests."""
 
     pass
 
 
 class HandleException(Exception):
-    """Exception associated with requests with invalid handles.
-    """
+    """Exception associated with requests with invalid handles."""
 
     pass
 
 
 class DataSourceException(Exception):
     """Exception associated with Device misconfiguration or invalid requests to
-        a data source.
+    a data source.
     """
 
     pass
 
 
 class UnitsException(Exception):
-    """Conversion not understood.
-    """
+    """Conversion not understood."""
 
     pass
 
 
 class ControlSystemException(Exception):
-    """Exception associated with control system misconfiguration.
-    """
+    """Exception associated with control system misconfiguration."""
 
     pass
```

### Comparing `pytac-0.5.0/pytac/lattice.py` & `pytac-0.6.0b1/src/pytac/lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 """
 import logging
 from typing import List, Optional
 
 import numpy
 
 import pytac
-from pytac.element import Element
 from pytac.data_source import DataSource, DataSourceManager
-from pytac.exceptions import (
-    DataSourceException,
-    UnitsException,
-)
+from pytac.element import Element
+from pytac.exceptions import DataSourceException, UnitsException
 
 
 class Lattice:
     """Representation of a lattice.
 
     Represents a lattice object that contains all elements of the ring. It has
     a name and a control system to be used for unit conversion.
@@ -30,15 +27,15 @@
     .. Private Attributes:
            _elements: The list of all the element objects in the lattice
            _data_source_manager: A class that manages the
                                                       data sources associated
                                                       with this lattice.
     """
 
-    def __init__(self, name: str, symmetry: int = None) -> None:
+    def __init__(self, name: str, symmetry: Optional[int] = None) -> None:
         """Args:
             name: The name of the lattice.
             symmetry: The symmetry of the lattice (the number of cells).
 
         **Methods:**
         """
         self.name = name
@@ -47,16 +44,15 @@
         self._data_source_manager = DataSourceManager()
 
     def __str__(self) -> str:
         return f"Lattice {self.name}"
 
     @property
     def cell_length(self) -> Optional[float]:
-        """The average length of a cell in the lattice.
-        """
+        """The average length of a cell in the lattice."""
         if (self.symmetry is None) or (self.get_length() == 0):
             return None
         else:
             return self.get_length() / self.symmetry
 
     @property
     def cell_bounds(self) -> Optional[List[int]]:
@@ -215,15 +211,20 @@
             FieldException: if the lattice does not have the specified field.
         """
         return self._data_source_manager.get_value(
             field, handle, units, data_source, throw
         )
 
     def set_value(
-        self, field, value, units=pytac.DEFAULT, data_source=pytac.DEFAULT, throw=True,
+        self,
+        field,
+        value,
+        units=pytac.DEFAULT,
+        data_source=pytac.DEFAULT,
+        throw=True,
     ):
         """Set the value for a field.
 
         This value can be set on the machine or the simulation.
 
         Args:
             field (str): The requested field.
@@ -426,15 +427,19 @@
         if len(elements) != len(values):
             raise IndexError(
                 f"Number of elements in given array({len(values)}) must be "
                 f"equal to the number of elements in the family({len(elements)})."
             )
         for element, value in zip(elements, values):
             status = element.set_value(
-                field, value, units=units, data_source=data_source, throw=throw,
+                field,
+                value,
+                units=units,
+                data_source=data_source,
+                throw=throw,
             )
             if status is not None:
                 return status
 
     def set_default_units(self, units: str) -> None:
         """Sets the default unit type for the lattice and all its elements.
```

### Comparing `pytac-0.5.0/pytac/load_csv.py` & `pytac-0.6.0b1/src/pytac/load_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 import contextlib
 import copy
 import csv
 from pathlib import Path
 from typing import Dict, Iterator
 
 import pytac
-from pytac.device import SimpleDevice, EpicsDevice
-from pytac.lattice import EpicsLattice, Lattice
-from pytac.units import NullUnitConv, PchipUnitConv, PolyUnitConv, UnitConv
 from pytac import data_source, element, utils
+from pytac.device import EpicsDevice, SimpleDevice
 from pytac.exceptions import ControlSystemException
-
+from pytac.lattice import EpicsLattice, Lattice
+from pytac.units import NullUnitConv, PchipUnitConv, PolyUnitConv, UnitConv
 
 # Create a default unit conversion object that returns the input unchanged.
 DEFAULT_UC = NullUnitConv()
 
 ELEMENTS_FILENAME = "elements.csv"
 EPICS_DEVICES_FILENAME = "epics_devices.csv"
 SIMPLE_DEVICES_FILENAME = "simple_devices.csv"
```

### Comparing `pytac-0.5.0/pytac/units.py` & `pytac-0.6.0b1/src/pytac/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,22 +79,24 @@
         string_rep = self.__class__.__name__
         if self.name is not None:
             string_rep += f" {self.name}"
         return string_rep
 
     def set_post_eng_to_phys(self, post_eng_to_phys):
         """Set the function to be applied after the initial conversion.
+
         Args:
             post_eng_to_phys (function): Function to be applied after the
                                           initial conversion.
         """
         self._post_eng_to_phys = post_eng_to_phys
 
     def set_pre_phys_to_eng(self, pre_phys_to_eng):
         """Set the function to be applied before the initial conversion.
+
         Args:
             pre_phys_to_eng (function): Function to be applied before the
                                          initial conversion.
         """
         self._pre_phys_to_eng = pre_phys_to_eng
 
     def _raw_eng_to_phys(self, value):
```

### Comparing `pytac-0.5.0/pytac/utils.py` & `pytac-0.6.0b1/src/pytac/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utility functions."""
 import math
 
 import scipy.constants
 
-
 electron_mass_name = "electron mass energy equivalent in MeV"
 electron_mass_mev, _, _ = scipy.constants.physical_constants[electron_mass_name]
 
 
 def get_rigidity(energy_mev):
     """
     Args:
```

### Comparing `pytac-0.5.0/test/test_cothread_cs.py` & `pytac-0.6.0b1/tests/test_cothread_cs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,95 @@
 """Tests for the CothreadControlSystem class.
 
 This module depends on the cothread module being mocked.
 
 See pytest_sessionstart() in conftest.py for more.
 """
-from cothread.catools import caget, caput, ca_nothing
 import pytest
+from constants import RB_PV, SP_PV
+from cothread.catools import ca_nothing, caget, caput
 from testfixtures import LogCapture
 
-from constants import RB_PV, SP_PV
 import pytac
 from pytac.cothread_cs import CothreadControlSystem
 
 
 @pytest.fixture
 def cs():
-    return CothreadControlSystem()
+    return CothreadControlSystem(wait=True, timeout=2.0)
 
 
 def test_get_single_calls_caget_correctly(cs):
     caget.return_value = 42
     assert cs.get_single(RB_PV) == 42
-    caget.assert_called_with(RB_PV, throw=True, timeout=1.0)
+    caget.assert_called_with(RB_PV, throw=True, timeout=2.0)
 
 
 def test_get_multiple_calls_caget_correctly(cs):
     """caget is called with throw=False despite throw=True being the default
-        for get_multiple as we always want our get operation to fully complete,
-        rather than being stopped halway through by an error raised from
-        cothread, so that even if one get operation to a PV fails the rest will
-        complete sucessfully.
+    for get_multiple as we always want our get operation to fully complete,
+    rather than being stopped halway through by an error raised from
+    cothread, so that even if one get operation to a PV fails the rest will
+    complete sucessfully.
     """
     caget.return_value = [42, 6]
     assert cs.get_multiple([RB_PV, SP_PV]) == [42, 6]
-    caget.assert_called_with([RB_PV, SP_PV], throw=False, timeout=1.0)
+    caget.assert_called_with([RB_PV, SP_PV], throw=False, timeout=2.0)
 
 
 def test_set_single_calls_caput_correctly(cs):
     assert cs.set_single(SP_PV, 42) is True
-    caput.assert_called_with(SP_PV, 42, throw=True, timeout=1.0)
+    caput.assert_called_with(SP_PV, 42, throw=True, timeout=2.0, wait=True)
 
 
 def test_set_multiple_calls_caput_correctly(cs):
     """caput is called with throw=False despite throw=True being the default
-        for set_multiple as we always want our set operation to fully complete,
-        rather than being stopped halway through by an error raised from
-        cothread, so that even if one set operation to a PV fails the rest will
-        complete sucessfully.
+    for set_multiple as we always want our set operation to fully complete,
+    rather than being stopped halway through by an error raised from
+    cothread, so that even if one set operation to a PV fails the rest will
+    complete sucessfully.
     """
     cs.set_multiple([SP_PV, RB_PV], [42, 6])
-    caput.assert_called_with([SP_PV, RB_PV], [42, 6], throw=False, timeout=1.0)
+    caput.assert_called_with(
+        [SP_PV, RB_PV], [42, 6], throw=False, timeout=2.0, wait=True
+    )
 
 
 def test_get_multiple_raises_ControlSystemException(cs):
-    """Here we check that errors are thrown, suppressed and logged correctly.
-    """
+    """Here we check that errors are thrown, suppressed and logged correctly."""
     caget.return_value = [12, ca_nothing("pv", False)]
     with pytest.raises(pytac.exceptions.ControlSystemException):
         cs.get_multiple([RB_PV, SP_PV])
     with LogCapture() as log:
         assert cs.get_multiple([RB_PV, SP_PV], throw=False) == [12, None]
     log.check(("root", "WARNING", "Cannot connect to pv."))
 
 
 def test_set_multiple_raises_ControlSystemException(cs):
-    """Here we check that errors are thrown, suppressed and logged correctly.
-    """
+    """Here we check that errors are thrown, suppressed and logged correctly."""
     caput.return_value = [ca_nothing("pv1", True), ca_nothing("pv2", False)]
     with pytest.raises(pytac.exceptions.ControlSystemException):
         cs.set_multiple([RB_PV, SP_PV], [42, 6])
     with LogCapture() as log:
         assert cs.set_multiple([RB_PV, SP_PV], [42, 6], throw=False) == [True, False]
     log.check(("root", "WARNING", "Cannot connect to pv2."))
 
 
 def test_get_single_raises_ControlSystemException(cs):
-    """Here we check that errors are thrown, suppressed and logged correctly.
-    """
+    """Here we check that errors are thrown, suppressed and logged correctly."""
     caget.side_effect = ca_nothing("pv", False)
     with LogCapture() as log:
         assert cs.get_single(RB_PV, throw=False) is None
         with pytest.raises(pytac.exceptions.ControlSystemException):
             cs.get_single(RB_PV, throw=True)
     log.check(("root", "WARNING", "Cannot connect to prefix:rb."))
 
 
 def test_set_single_raises_ControlSystemException(cs):
-    """Here we check that errors are thrown, suppressed and logged correctly.
-    """
+    """Here we check that errors are thrown, suppressed and logged correctly."""
     caput.side_effect = ca_nothing("pv", False)
     with LogCapture() as log:
         assert cs.set_single(SP_PV, 42, throw=False) is False
         with pytest.raises(pytac.exceptions.ControlSystemException):
             cs.set_single(SP_PV, 42, throw=True)
     log.check(("root", "WARNING", "Cannot connect to prefix:sp."))
```

### Comparing `pytac-0.5.0/test/test_data_source.py` & `pytac-0.6.0b1/tests/test_data_source.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
+from constants import DUMMY_VALUE_2
 from pytest_lazyfixture import lazy_fixture
 
-from constants import DUMMY_VALUE_2
 import pytac
 
 
 @pytest.mark.parametrize(
     "simple_object",
     [
         lazy_fixture("simple_element"),
```

### Comparing `pytac-0.5.0/test/test_device.py` & `pytac-0.6.0b1/tests/test_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from pytac.exceptions import DataSourceException
 from unittest import mock
 
 import pytest
-
 from constants import PREFIX, RB_PV, SP_PV
+
 import pytac
-from pytac.device import SimpleDevice, EpicsDevice, PvEnabler
+from pytac.device import EpicsDevice, PvEnabler, SimpleDevice
+from pytac.exceptions import DataSourceException
 
 
 def create_epics_device(prefix=PREFIX, rb_pv=RB_PV, sp_pv=SP_PV, enabled=True):
     mock_cs = mock.MagicMock()
     mock_cs.get_single.return_value = 40.0
     device = EpicsDevice(prefix, mock_cs, enabled=enabled, rb_pv=rb_pv, sp_pv=sp_pv)
     return device
```

### Comparing `pytac-0.5.0/test/test_element.py` & `pytac-0.6.0b1/tests/test_element.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import mock
 
 import pytest
-
 from constants import DUMMY_VALUE_1, DUMMY_VALUE_2
+
 import pytac
 from pytac.device import SimpleDevice
 from pytac.element import Element
 from pytac.lattice import Lattice
 
 
 def test_create_element():
```

### Comparing `pytac-0.5.0/test/test_epics.py` & `pytac-0.6.0b1/tests/test_epics.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 import numpy
 import pytest
-
 from constants import DUMMY_ARRAY, RB_PV, SP_PV
+
 import pytac
 
 
 def test_get_values_live(simple_epics_lattice, mock_cs):
     simple_epics_lattice.get_element_values("family", "x", pytac.RB, pytac.PHYS)
     mock_cs.get_multiple.assert_called_with([RB_PV], True)
```

### Comparing `pytac-0.5.0/test/test_invalid_classes.py` & `pytac-0.6.0b1/tests/test_invalid_classes.py`

 * *Files identical despite different names*

### Comparing `pytac-0.5.0/test/test_lattice.py` & `pytac-0.6.0b1/tests/test_lattice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 import numpy
 import pytest
-
 from constants import DUMMY_ARRAY, LATTICE_NAME
+
 import pytac
 from pytac.element import Element
 from pytac.lattice import Lattice
 
 
 def test_create_lattice():
     lat = Lattice(LATTICE_NAME)
```

### Comparing `pytac-0.5.0/test/test_load.py` & `pytac-0.6.0b1/tests/test_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,27 +22,27 @@
         raise ImportError
 
     return CothreadControlSystem
 
 
 def test_default_control_system_import():
     """In this test we:
-        - assert that the lattice is indeed loaded if no execeptions are raised
-        - assert that the default control system is indeed cothread and that it
-           is loaded onto the lattice correctly
+    - assert that the lattice is indeed loaded if no execeptions are raised
+    - assert that the default control system is indeed cothread and that it
+       is loaded onto the lattice correctly
     """
     assert bool(load("VMX"))
     assert isinstance(load("VMX")._cs, pytac.cothread_cs.CothreadControlSystem)
 
 
 def test_import_fail_raises_ControlSystemException(mock_cs_raises_ImportError):
     """In this test we:
-        - check that load corectly fails if cothread cannot be imported
-        - check that when the import of the CothreadControlSystem fails the
-           ImportError raised is replaced with a ControlSystemException
+    - check that load corectly fails if cothread cannot be imported
+    - check that when the import of the CothreadControlSystem fails the
+       ImportError raised is replaced with a ControlSystemException
     """
     with patch("pytac.cothread_cs.CothreadControlSystem", mock_cs_raises_ImportError):
         with pytest.raises(pytac.exceptions.ControlSystemException):
             load("VMX")
 
 
 def test_elements_loaded(lattice):
```

### Comparing `pytac-0.5.0/test/test_machine.py` & `pytac-0.6.0b1/tests/test_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 
 import numpy
 import pytest
 from pytest_lazyfixture import lazy_fixture
 
 import pytac
 
-
 EPS = 1e-8
 
 
 def get_lattice(ring_mode):
-    """ Load the entire lattice from the data directory."""
+    """Load the entire lattice from the data directory."""
     lattice = pytac.load_csv.load(ring_mode, mock.MagicMock())
     return lattice
 
 
 def test_load_lattice_using_default_dir():
     lat = pytac.load_csv.load("VMX", mock.MagicMock())
     assert len(lat) == 2142
```

### Comparing `pytac-0.5.0/test/test_units.py` & `pytac-0.6.0b1/tests/test_units.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 import numpy
 import pytest
-
 from constants import DUMMY_VALUE_1, DUMMY_VALUE_2, DUMMY_VALUE_3
+
 import pytac
 from pytac.units import NullUnitConv, PchipUnitConv, PolyUnitConv, UnitConv
 
 
 def f1(value):
     return value * 2
```

### Comparing `pytac-0.5.0/test/test_utils.py` & `pytac-0.6.0b1/tests/test_utils.py`

 * *Files identical despite different names*

