# Comparing `tmp/oakvar-2.9.7.tar.gz` & `tmp/oakvar-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakvar-2.9.7.tar", last modified: Thu Apr 13 13:08:15 2023, max compression
+gzip compressed data, was "oakvar-2.9.8.tar", last modified: Thu Apr 13 13:16:04 2023, max compression
```

## Comparing `oakvar-2.9.7.tar` & `oakvar-2.9.8.tar`

### file list

```diff
@@ -1,550 +1,551 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.410949 oakvar-2.9.7/
--rwxrwxrwx   0 root         (0) root         (0)     1725 2023-04-13 08:45:25.000000 oakvar-2.9.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 13:08:15.410689 oakvar-2.9.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3279 2023-04-13 08:45:25.000000 oakvar-2.9.7/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.022808 oakvar-2.9.7/cravat/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.025295 oakvar-2.9.7/cravat/api/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.026536 oakvar-2.9.7/cravat/api/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/module/ls_logic.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.027073 oakvar-2.9.7/cravat/api/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.027534 oakvar-2.9.7/cravat/api/store/account/
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/system.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/test.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/api/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.033944 oakvar-2.9.7/cravat/cli/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/config.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/gui.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/issue.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/license.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.035739 oakvar-2.9.7/cravat/cli/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/module/info_fn.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/module/ls.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/new.py
--rwxrwxrwx   0 root         (0) root         (0)      110 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/report.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.036111 oakvar-2.9.7/cravat/cli/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.036491 oakvar-2.9.7/cravat/cli/store/account/
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/system.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/test.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cli/update.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/util.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/cli/version.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/constants.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/cravat_report.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.041883 oakvar-2.9.7/cravat/gui/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/job_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/multiuser.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/server.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/serveradmindb.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/store_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/system_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/system_message_db.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/system_worker.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/userjob.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/util.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/web_submit.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.042978 oakvar-2.9.7/cravat/gui/webresult/
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/webresult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/webresult/jsonreporter.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-06 05:49:48.000000 oakvar-2.9.7/cravat/gui/webresult/webresult.py
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/gui/websocket_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/inout.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.044177 oakvar-2.9.7/cravat/lib/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.004647 oakvar-2.9.7/cravat/lib/assets/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.005528 oakvar-2.9.7/cravat/lib/assets/module_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.044594 oakvar-2.9.7/cravat/lib/assets/module_templates/annotator/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/annotator/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.044973 oakvar-2.9.7/cravat/lib/assets/module_templates/converter/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/converter/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.045350 oakvar-2.9.7/cravat/lib/assets/module_templates/mapper/
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/mapper/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.045797 oakvar-2.9.7/cravat/lib/assets/module_templates/postaggregator/
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/postaggregator/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.046169 oakvar-2.9.7/cravat/lib/assets/module_templates/preparer/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/preparer/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.046549 oakvar-2.9.7/cravat/lib/assets/module_templates/reporter/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/assets/module_templates/reporter/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.052055 oakvar-2.9.7/cravat/lib/base/
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/aggregator.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/annotator.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/commonmodule.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/converter.py
--rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/master_converter.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/mp_runners.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/postaggregator.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/preparer.py
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/report_filter.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/reporter.py
--rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/runner.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/base/vcf2vcf.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.053934 oakvar-2.9.7/cravat/lib/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/module/cache.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/module/data_cache.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/module/local.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/module/remote.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.055007 oakvar-2.9.7/cravat/lib/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/store/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/store/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/store/db.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.055356 oakvar-2.9.7/cravat/lib/store/ov/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/store/ov/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.055705 oakvar-2.9.7/cravat/lib/store/ov/account/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/store/ov/account/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.056396 oakvar-2.9.7/cravat/lib/system/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/system/consts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.060725 oakvar-2.9.7/cravat/lib/util/
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/admin_util.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/asyn.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/download.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/download_library.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/image.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/inout.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/run.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/seq.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.7/cravat/lib/util/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.061224 oakvar-2.9.7/oakvar/
--rwxrwxrwx   0 root         (0) root         (0)     4240 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.066924 oakvar-2.9.7/oakvar/api/
--rwxrwxrwx   0 root         (0) root         (0)    17617 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1312 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.068428 oakvar-2.9.7/oakvar/api/module/
--rwxrwxrwx   0 root         (0) root         (0)    15951 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/api/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3473 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)     3855 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/module/ls_logic.py
--rwxrwxrwx   0 root         (0) root         (0)     1528 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.069007 oakvar-2.9.7/oakvar/api/store/
--rwxrwxrwx   0 root         (0) root         (0)     5347 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.069445 oakvar-2.9.7/oakvar/api/store/account/
--rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-13 08:45:25.000000 oakvar-2.9.7/oakvar/api/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2578 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/api/system.py
--rwxrwxrwx   0 root         (0) root         (0)    32152 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/api/test.py
--rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/api/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.075407 oakvar-2.9.7/oakvar/cli/
--rwxrwxrwx   0 root         (0) root         (0)     2600 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6019 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3117 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/config.py
--rwxrwxrwx   0 root         (0) root         (0)     9134 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/gui.py
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/issue.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/license.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.077091 oakvar-2.9.7/oakvar/cli/module/
--rwxrwxrwx   0 root         (0) root         (0)    12395 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/module/info_fn.py
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)     5960 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/module/ls.py
--rwxrwxrwx   0 root         (0) root         (0)     2576 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/new.py
--rwxrwxrwx   0 root         (0) root         (0)     5567 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/report.py
--rwxrwxrwx   0 root         (0) root         (0)     9069 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.077507 oakvar-2.9.7/oakvar/cli/store/
--rwxrwxrwx   0 root         (0) root         (0)     7517 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.077972 oakvar-2.9.7/oakvar/cli/store/account/
--rwxrwxrwx   0 root         (0) root         (0)     6020 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4904 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/system.py
--rwxrwxrwx   0 root         (0) root         (0)     1054 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/test.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/update.py
--rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/util.py
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/cli/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.101467 oakvar-2.9.7/oakvar/gui/
--rwxrwxrwx   0 root         (0) root         (0)      940 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/consts.py
--rwxrwxrwx   0 root         (0) root         (0)    25702 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/job_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     9376 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/multiuser.py
--rwxrwxrwx   0 root         (0) root         (0)    15109 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/gui/server.py
--rwxrwxrwx   0 root         (0) root         (0)    22012 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/serveradmindb.py
--rwxrwxrwx   0 root         (0) root         (0)    13000 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/store_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     6706 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/system_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     2136 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/system_message_db.py
--rwxrwxrwx   0 root         (0) root         (0)     6412 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/system_worker.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/gui/userjob.py
--rwxrwxrwx   0 root         (0) root         (0)     4574 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/util.py
--rwxrwxrwx   0 root         (0) root         (0)    15737 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/gui/web_submit.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.116720 oakvar-2.9.7/oakvar/gui/webresult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.118409 oakvar-2.9.7/oakvar/gui/webresult/css/
--rwxrwxrwx   0 root         (0) root         (0)     2389 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/css/pqselect.min.css
--rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/email.png
--rwxrwxrwx   0 root         (0) root         (0)     1150 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/favicon.ico
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.132651 oakvar-2.9.7/oakvar/gui/webresult/fonts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.214668 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/
--rwxrwxrwx   0 root         (0) root         (0)   138764 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
--rwxrwxrwx   0 root         (0) root         (0)   102868 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
--rwxrwxrwx   0 root         (0) root         (0)   146824 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   108752 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   143208 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
--rwxrwxrwx   0 root         (0) root         (0)   106140 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   151052 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111808 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142920 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
--rwxrwxrwx   0 root         (0) root         (0)   106108 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150628 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111708 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   140724 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
--rwxrwxrwx   0 root         (0) root         (0)   104232 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
--rwxrwxrwx   0 root         (0) root         (0)   149996 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111392 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   144372 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
--rwxrwxrwx   0 root         (0) root         (0)   106876 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   140632 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
--rwxrwxrwx   0 root         (0) root         (0)   104332 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150092 2023-01-21 00:14:14.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111332 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142552 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
--rwxrwxrwx   0 root         (0) root         (0)   105924 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150988 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   112184 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   133844 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
--rwxrwxrwx   0 root         (0) root         (0)    98868 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142932 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
--rwxrwxrwx   0 root         (0) root         (0)   105804 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   151180 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   112048 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   135920 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
--rwxrwxrwx   0 root         (0) root         (0)    99632 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
--rwxrwxrwx   0 root         (0) root         (0)   145480 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   106496 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   245036 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)   227180 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)   324864 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)     5303 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/inter.css
--rwxrwxrwx   0 root         (0) root         (0)    26456 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    19508 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    25692 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    18980 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    26312 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    19416 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    33072 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    25740 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.228762 oakvar-2.9.7/oakvar/gui/webresult/images/
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      379 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-down-right-circle.svg
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-down-right.svg
--rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-down.svg
--rwxrwxrwx   0 root         (0) root         (0)      311 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-left.svg
--rwxrwxrwx   0 root         (0) root         (0)      312 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-right.svg
--rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrow-up.svg
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/arrows-move.svg
--rwxrwxrwx   0 root         (0) root         (0)     2140 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/camera.svg
--rwxrwxrwx   0 root         (0) root         (0)      291 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/caret-down.svg
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/caret-right.svg
--rwxrwxrwx   0 root         (0) root         (0)     3125 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/close.png
--rwxrwxrwx   0 root         (0) root         (0)     2390 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/close.svg
--rwxrwxrwx   0 root         (0) root         (0)      722 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/download-material-black.png
--rwxrwxrwx   0 root         (0) root         (0)     2066 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/download.svg
--rwxrwxrwx   0 root         (0) root         (0)      485 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/grip-vertical.svg
--rwxrwxrwx   0 root         (0) root         (0)     2219 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/pin.svg
--rwxrwxrwx   0 root         (0) root         (0)     2243 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/plus-circle-dotted.svg
--rwxrwxrwx   0 root         (0) root         (0)      280 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/plus-circle-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)     4645 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/sorry.png
--rwxrwxrwx   0 root         (0) root         (0)    25333 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/spinner.gif
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/x-lg.svg
--rwxrwxrwx   0 root         (0) root         (0)      332 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/images/x.svg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.256217 oakvar-2.9.7/oakvar/gui/webresult/js/
--rwxrwxrwx   0 root         (0) root         (0)   398184 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/Chart.js
--rwxrwxrwx   0 root         (0) root         (0)    26580 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/axios.min.js
--rwxrwxrwx   0 root         (0) root         (0)   137820 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/webresult/js/axios.min.js.map
--rwxrwxrwx   0 root         (0) root         (0)     9278 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/dom-to-image.min.js
--rwxrwxrwx   0 root         (0) root         (0)     5839 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/download.js
--rwxrwxrwx   0 root         (0) root         (0)    12091 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
--rwxrwxrwx   0 root         (0) root         (0)   954164 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/graphics.js
--rwxrwxrwx   0 root         (0) root         (0)    86659 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-3.2.1.min.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.276424 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
--rwxrwxrwx   0 root         (0) root         (0)    12660 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rwxrwxrwx   0 root         (0) root         (0)     1817 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.010411 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.277079 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rwxrwxrwx   0 root         (0) root         (0)   293430 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.283586 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
--rwxrwxrwx   0 root         (0) root         (0)     6992 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6988 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6999 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6299 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)    32588 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
--rwxrwxrwx   0 root         (0) root         (0)    35997 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rwxrwxrwx   0 root         (0) root         (0)   520714 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rwxrwxrwx   0 root         (0) root         (0)    30747 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rwxrwxrwx   0 root         (0) root         (0)   253668 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rwxrwxrwx   0 root         (0) root         (0)    18705 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rwxrwxrwx   0 root         (0) root         (0)    15548 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rwxrwxrwx   0 root         (0) root         (0)    17342 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rwxrwxrwx   0 root         (0) root         (0)    13847 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rwxrwxrwx   0 root         (0) root         (0)     1340 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
--rwxrwxrwx   0 root         (0) root         (0)    13171 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery.tools.min.js
--rwxrwxrwx   0 root         (0) root         (0)     5451 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/jquery.url.js
--rwxrwxrwx   0 root         (0) root         (0)    24103 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/masonry.pkgd.min.js
--rwxrwxrwx   0 root         (0) root         (0)    84772 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/packery.pkgd.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.299661 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/
--rwxrwxrwx   0 root         (0) root         (0)    11583 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)   103213 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.305656 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/
--rwxrwxrwx   0 root         (0) root         (0)      230 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      210 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      771 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
--rwxrwxrwx   0 root         (0) root         (0)     1668 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rwxrwxrwx   0 root         (0) root         (0)      216 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.306833 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rwxrwxrwx   0 root         (0) root         (0)    76985 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.315006 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rwxrwxrwx   0 root         (0) root         (0)      750 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rwxrwxrwx   0 root         (0) root         (0)      769 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rwxrwxrwx   0 root         (0) root         (0)      802 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rwxrwxrwx   0 root         (0) root         (0)      805 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rwxrwxrwx   0 root         (0) root         (0)      636 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rwxrwxrwx   0 root         (0) root         (0)      774 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rwxrwxrwx   0 root         (0) root         (0)      782 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rwxrwxrwx   0 root         (0) root         (0)      822 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rwxrwxrwx   0 root         (0) root         (0)      773 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rwxrwxrwx   0 root         (0) root         (0)      675 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.319491 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
--rwxrwxrwx   0 root         (0) root         (0)     1105 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)      613 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rwxrwxrwx   0 root         (0) root         (0)      541 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rwxrwxrwx   0 root         (0) root         (0)     2973 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rwxrwxrwx   0 root         (0) root         (0)    27759 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rwxrwxrwx   0 root         (0) root         (0)     2383 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rwxrwxrwx   0 root         (0) root         (0)    12577 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rwxrwxrwx   0 root         (0) root         (0)     2408 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rwxrwxrwx   0 root         (0) root         (0)     2026 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rwxrwxrwx   0 root         (0) root         (0)    16145 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rwxrwxrwx   0 root         (0) root         (0)   481365 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rwxrwxrwx   0 root         (0) root         (0)    12757 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
--rwxrwxrwx   0 root         (0) root         (0)   242931 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
--rwxrwxrwx   0 root         (0) root         (0)     1646 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rwxrwxrwx   0 root         (0) root         (0)     1278 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rwxrwxrwx   0 root         (0) root         (0)      555 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.014484 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.320265 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.320891 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.321513 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.322185 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.322853 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.323500 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.324250 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.324910 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.325540 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.326341 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.326996 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.327645 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.328288 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.328975 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.329794 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.333027 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
--rwxrwxrwx   0 root         (0) root         (0)     1042 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)     1164 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)     2677 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
--rwxrwxrwx   0 root         (0) root         (0)     3716 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rwxrwxrwx   0 root         (0) root         (0)     1847 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rwxrwxrwx   0 root         (0) root         (0)    12583 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/pqselect.min.js
--rwxrwxrwx   0 root         (0) root         (0)    92225 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/raphael-min.js
--rwxrwxrwx   0 root         (0) root         (0)   326538 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/js/tailwind.min.js
--rwxrwxrwx   0 root         (0) root         (0)      900 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/webresult/jsonreporter.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.334424 oakvar-2.9.7/oakvar/gui/webresult/nocache/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.336389 oakvar-2.9.7/oakvar/gui/webresult/nocache/css/
--rwxrwxrwx   0 root         (0) root         (0)     1714 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/css/singlevariantpage.css
--rwxrwxrwx   0 root         (0) root         (0)    22655 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/css/style.css
--rwxrwxrwx   0 root         (0) root         (0)     2658 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/css/widget.css
--rwxrwxrwx   0 root         (0) root         (0)    21597 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.344036 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/
--rwxrwxrwx   0 root         (0) root         (0)    24858 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/filter.js
--rwxrwxrwx   0 root         (0) root         (0)    13065 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/infomgr.js
--rwxrwxrwx   0 root         (0) root         (0)    30870 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/main.js
--rwxrwxrwx   0 root         (0) root         (0)   103450 2023-04-13 11:11:33.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/setup.js
--rwxrwxrwx   0 root         (0) root         (0)     4903 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/showvariant.js
--rwxrwxrwx   0 root         (0) root         (0)    35998 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/singlevariantpage.js
--rwxrwxrwx   0 root         (0) root         (0)    28858 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/util.js
--rwxrwxrwx   0 root         (0) root         (0)     1696 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/variables.js
--rwxrwxrwx   0 root         (0) root         (0)    22262 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/js/widgethelper.js
--rwxrwxrwx   0 root         (0) root         (0)     5440 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/nocache/variant.html
--rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/question.png
--rwxrwxrwx   0 root         (0) root         (0)    29682 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/webresult/webresult.py
--rwxrwxrwx   0 root         (0) root         (0)      163 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webresult/webviewer.yml
--rwxrwxrwx   0 root         (0) root         (0)     4075 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/gui/websocket_handlers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.015498 oakvar-2.9.7/oakvar/gui/webstore/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.354447 oakvar-2.9.7/oakvar/gui/webstore/images/
--rwxrwxrwx   0 root         (0) root         (0)      446 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/chat-dots-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      740 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/chat-dots.svg
--rwxrwxrwx   0 root         (0) root         (0)      396 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/chat-left-text-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      545 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/chat-left-text.svg
--rwxrwxrwx   0 root         (0) root         (0)    22268 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/done.png
--rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/email.png
--rwxrwxrwx   0 root         (0) root         (0)     2226 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/empty.png
--rwxrwxrwx   0 root         (0) root         (0)     1763 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/folder.png
--rwxrwxrwx   0 root         (0) root         (0)    38197 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/genericmodulelogo.png
--rwxrwxrwx   0 root         (0) root         (0)     4766 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/hamburger.png
--rwxrwxrwx   0 root         (0) root         (0)     1194 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/left_arrow.png
--rwxrwxrwx   0 root         (0) root         (0)     3524 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/new.png
--rwxrwxrwx   0 root         (0) root         (0)      474 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/no_logo_module.svg
--rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/question.png
--rwxrwxrwx   0 root         (0) root         (0)     1214 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/right_arrow.png
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/webstore/images/x-lg.svg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.016316 oakvar-2.9.7/oakvar/gui/websubmit/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.361820 oakvar-2.9.7/oakvar/gui/websubmit/images/
--rwxrwxrwx   0 root         (0) root         (0)   372952 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/images/background.png
--rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/images/logo.png
--rwxrwxrwx   0 root         (0) root         (0)    22716 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/images/logo_only.png
--rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/images/logo_transparent.png
--rwxrwxrwx   0 root         (0) root         (0)    22247 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/images/logo_transparent_bw.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.365671 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/
--rwxrwxrwx   0 root         (0) root         (0)      511 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/cravat.hg18.txt
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/cravat.hg19.txt
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/cravat.hg38.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:16.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg18.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg19.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg38.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.375610 oakvar-2.9.7/oakvar/gui/websubmit/nocache/
--rwxrwxrwx   0 root         (0) root         (0)      692 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/alerts.js
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/element_constructors.js
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/element_getters.js
--rwxrwxrwx   0 root         (0) root         (0)    55822 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/index.html
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/input.js
--rwxrwxrwx   0 root         (0) root         (0)    14408 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/jobstable.js
--rwxrwxrwx   0 root         (0) root         (0)     8242 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/login.html
--rwxrwxrwx   0 root         (0) root         (0)     3796 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/multiuser.css
--rwxrwxrwx   0 root         (0) root         (0)    16797 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/multiuser.js
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/select_modules.js
--rwxrwxrwx   0 root         (0) root         (0)      228 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/showhide.js
--rwxrwxrwx   0 root         (0) root         (0)     6783 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/submit.js
--rwxrwxrwx   0 root         (0) root         (0)      484 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/util.js
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/websubmit.css
--rwxrwxrwx   0 root         (0) root         (0)    39200 2023-02-22 05:21:01.000000 oakvar-2.9.7/oakvar/gui/websubmit/nocache/websubmit.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.376326 oakvar-2.9.7/oakvar/gui/www/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.377428 oakvar-2.9.7/oakvar/gui/www/assets/
--rwxrwxrwx   0 root         (0) root         (0)    47521 2023-04-13 12:03:53.000000 oakvar-2.9.7/oakvar/gui/www/assets/index.b35f4d23.css
--rwxrwxrwx   0 root         (0) root         (0)   381782 2023-04-13 12:03:53.000000 oakvar-2.9.7/oakvar/gui/www/assets/index.ef59c55d.js
--rwxrwxrwx   0 root         (0) root         (0)     2074 2023-04-13 12:03:53.000000 oakvar-2.9.7/oakvar/gui/www/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.381173 oakvar-2.9.7/oakvar/lib/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.383022 oakvar-2.9.7/oakvar/lib/assets/
--rwxrwxrwx   0 root         (0) root         (0)     9036 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/exampleinput
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.383822 oakvar-2.9.7/oakvar/lib/assets/license/
--rwxrwxrwx   0 root         (0) root         (0)     1707 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/license/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/license/liftover.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.018240 oakvar-2.9.7/oakvar/lib/assets/module_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.385215 oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/template.md
--rwxrwxrwx   0 root         (0) root         (0)      277 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1195 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.386632 oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.md
--rwxrwxrwx   0 root         (0) root         (0)     2534 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1249 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.388089 oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.md
--rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.389294 oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.md
--rwxrwxrwx   0 root         (0) root         (0)      731 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1335 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.390519 oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/template.md
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-04-13 08:45:26.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1327 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.391701 oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.md
--rwxrwxrwx   0 root         (0) root         (0)     1742 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.yml
--rwxrwxrwx   0 root         (0) root         (0)      135 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/oakvar.yml
--rwxrwxrwx   0 root         (0) root         (0)     3078 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/output_columns.yml
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/assets/system.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.400079 oakvar-2.9.7/oakvar/lib/base/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21656 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/base/aggregator.py
--rwxrwxrwx   0 root         (0) root         (0)    34429 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/annotator.py
--rwxrwxrwx   0 root         (0) root         (0)     2714 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/base/commonmodule.py
--rwxrwxrwx   0 root         (0) root         (0)     3035 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/converter.py
--rwxrwxrwx   0 root         (0) root         (0)    11639 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)    35485 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/master_converter.py
--rwxrwxrwx   0 root         (0) root         (0)     3036 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/mp_runners.py
--rwxrwxrwx   0 root         (0) root         (0)    25139 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/postaggregator.py
--rwxrwxrwx   0 root         (0) root         (0)     7018 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/preparer.py
--rwxrwxrwx   0 root         (0) root         (0)    43032 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/report_filter.py
--rwxrwxrwx   0 root         (0) root         (0)    42098 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/reporter.py
--rwxrwxrwx   0 root         (0) root         (0)    80093 2023-04-13 13:06:51.000000 oakvar-2.9.7/oakvar/lib/base/runner.py
--rwxrwxrwx   0 root         (0) root         (0)    15164 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/base/vcf2vcf.py
--rwxrwxrwx   0 root         (0) root         (0)     2620 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/consts.py
--rwxrwxrwx   0 root         (0) root         (0)     7397 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.402516 oakvar-2.9.7/oakvar/lib/module/
--rwxrwxrwx   0 root         (0) root         (0)    29864 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3915 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/module/cache.py
--rwxrwxrwx   0 root         (0) root         (0)     3523 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/module/data_cache.py
--rwxrwxrwx   0 root         (0) root         (0)    29962 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/module/local.py
--rwxrwxrwx   0 root         (0) root         (0)    10491 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/module/remote.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.403858 oakvar-2.9.7/oakvar/lib/store/
--rwxrwxrwx   0 root         (0) root         (0)     4330 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/store/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/store/consts.py
--rwxrwxrwx   0 root         (0) root         (0)    25288 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/store/db.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.404383 oakvar-2.9.7/oakvar/lib/store/ov/
--rwxrwxrwx   0 root         (0) root         (0)     8121 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/store/ov/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.404776 oakvar-2.9.7/oakvar/lib/store/ov/account/
--rwxrwxrwx   0 root         (0) root         (0)    19142 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/store/ov/account/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.405889 oakvar-2.9.7/oakvar/lib/system/
--rwxrwxrwx   0 root         (0) root         (0)    34376 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1294 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/system/consts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.410094 oakvar-2.9.7/oakvar/lib/util/
--rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5570 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/util/admin_util.py
--rwxrwxrwx   0 root         (0) root         (0)      744 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/util/asyn.py
--rwxrwxrwx   0 root         (0) root         (0)     5042 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/util/download.py
--rwxrwxrwx   0 root         (0) root         (0)    19071 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/util/download_library.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/util/image.py
--rwxrwxrwx   0 root         (0) root         (0)    20663 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/util/inout.py
--rwxrwxrwx   0 root         (0) root         (0)     4932 2023-04-13 08:45:27.000000 oakvar-2.9.7/oakvar/lib/util/run.py
--rwxrwxrwx   0 root         (0) root         (0)    11187 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/util/seq.py
--rwxrwxrwx   0 root         (0) root         (0)    20060 2023-04-13 11:41:53.000000 oakvar-2.9.7/oakvar/lib/util/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:08:15.064104 oakvar-2.9.7/oakvar.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    19018 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      275 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-13 13:08:14.000000 oakvar-2.9.7/oakvar.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      625 2023-04-13 08:45:27.000000 oakvar-2.9.7/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 13:08:15.411044 oakvar-2.9.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2398 2023-04-13 13:07:53.000000 oakvar-2.9.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.214432 oakvar-2.9.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1725 2023-04-13 08:45:25.000000 oakvar-2.9.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 13:16:04.214136 oakvar-2.9.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3279 2023-04-13 08:45:25.000000 oakvar-2.9.8/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.911869 oakvar-2.9.8/cravat/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.914288 oakvar-2.9.8/cravat/api/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.915434 oakvar-2.9.8/cravat/api/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/module/ls_logic.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.915809 oakvar-2.9.8/cravat/api/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.916265 oakvar-2.9.8/cravat/api/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/system.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/test.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/api/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.922568 oakvar-2.9.8/cravat/cli/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/config.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/gui.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/issue.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/license.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.924169 oakvar-2.9.8/cravat/cli/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/module/info_fn.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/module/ls.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/new.py
+-rwxrwxrwx   0 root         (0) root         (0)      110 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/report.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.924569 oakvar-2.9.8/cravat/cli/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.924977 oakvar-2.9.8/cravat/cli/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/system.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/test.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cli/update.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/util.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/cli/version.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/cravat_report.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.930512 oakvar-2.9.8/cravat/gui/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/job_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/multiuser.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/server.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/serveradmindb.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/store_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/system_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/system_message_db.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/system_worker.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/userjob.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/util.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/web_submit.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.931696 oakvar-2.9.8/cravat/gui/webresult/
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/webresult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/webresult/jsonreporter.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-06 05:49:48.000000 oakvar-2.9.8/cravat/gui/webresult/webresult.py
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/gui/websocket_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/inout.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.932938 oakvar-2.9.8/cravat/lib/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.894155 oakvar-2.9.8/cravat/lib/assets/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.895148 oakvar-2.9.8/cravat/lib/assets/module_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.933364 oakvar-2.9.8/cravat/lib/assets/module_templates/annotator/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/annotator/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.933900 oakvar-2.9.8/cravat/lib/assets/module_templates/converter/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/converter/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.934325 oakvar-2.9.8/cravat/lib/assets/module_templates/mapper/
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/mapper/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.934746 oakvar-2.9.8/cravat/lib/assets/module_templates/postaggregator/
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/postaggregator/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.935141 oakvar-2.9.8/cravat/lib/assets/module_templates/preparer/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/preparer/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.935533 oakvar-2.9.8/cravat/lib/assets/module_templates/reporter/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/assets/module_templates/reporter/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.941158 oakvar-2.9.8/cravat/lib/base/
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/aggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/annotator.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/commonmodule.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/converter.py
+-rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/master_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/mp_runners.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/postaggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/preparer.py
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/report_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/reporter.py
+-rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/runner.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/base/vcf2vcf.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.943231 oakvar-2.9.8/cravat/lib/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/module/cache.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/module/data_cache.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/module/local.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/module/remote.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.944378 oakvar-2.9.8/cravat/lib/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/store/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/store/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/store/db.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.944759 oakvar-2.9.8/cravat/lib/store/ov/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/store/ov/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.945140 oakvar-2.9.8/cravat/lib/store/ov/account/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/store/ov/account/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.946024 oakvar-2.9.8/cravat/lib/system/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/system/consts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.950412 oakvar-2.9.8/cravat/lib/util/
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/admin_util.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/asyn.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/download.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/download_library.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/image.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/inout.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/run.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/seq.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.8/cravat/lib/util/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.950809 oakvar-2.9.8/oakvar/
+-rwxrwxrwx   0 root         (0) root         (0)     3007 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.956622 oakvar-2.9.8/oakvar/api/
+-rwxrwxrwx   0 root         (0) root         (0)    17617 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1312 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.958130 oakvar-2.9.8/oakvar/api/module/
+-rwxrwxrwx   0 root         (0) root         (0)    15949 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/api/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3473 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)     3855 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/module/ls_logic.py
+-rwxrwxrwx   0 root         (0) root         (0)     1528 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.958510 oakvar-2.9.8/oakvar/api/store/
+-rwxrwxrwx   0 root         (0) root         (0)     5347 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.958920 oakvar-2.9.8/oakvar/api/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-13 08:45:25.000000 oakvar-2.9.8/oakvar/api/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2578 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/api/system.py
+-rwxrwxrwx   0 root         (0) root         (0)    32152 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/api/test.py
+-rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/api/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.964699 oakvar-2.9.8/oakvar/cli/
+-rwxrwxrwx   0 root         (0) root         (0)     2600 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6019 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3117 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     9134 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/gui.py
+-rwxrwxrwx   0 root         (0) root         (0)      465 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/issue.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/license.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.966378 oakvar-2.9.8/oakvar/cli/module/
+-rwxrwxrwx   0 root         (0) root         (0)    12395 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/module/info_fn.py
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)     5960 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/module/ls.py
+-rwxrwxrwx   0 root         (0) root         (0)     2576 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/new.py
+-rwxrwxrwx   0 root         (0) root         (0)     5567 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/report.py
+-rwxrwxrwx   0 root         (0) root         (0)     9069 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.966789 oakvar-2.9.8/oakvar/cli/store/
+-rwxrwxrwx   0 root         (0) root         (0)     7517 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.967192 oakvar-2.9.8/oakvar/cli/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)     6051 2023-04-13 13:14:57.000000 oakvar-2.9.8/oakvar/cli/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4904 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/system.py
+-rwxrwxrwx   0 root         (0) root         (0)     1054 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/test.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/update.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/util.py
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/cli/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.973073 oakvar-2.9.8/oakvar/gui/
+-rwxrwxrwx   0 root         (0) root         (0)      940 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)    25702 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/job_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9376 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/multiuser.py
+-rwxrwxrwx   0 root         (0) root         (0)    15108 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/gui/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    22012 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/serveradmindb.py
+-rwxrwxrwx   0 root         (0) root         (0)    13000 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/store_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/system_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     2136 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/system_message_db.py
+-rwxrwxrwx   0 root         (0) root         (0)     6412 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/system_worker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4209 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/gui/userjob.py
+-rwxrwxrwx   0 root         (0) root         (0)     4574 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    15736 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/gui/web_submit.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.976212 oakvar-2.9.8/oakvar/gui/webresult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.976615 oakvar-2.9.8/oakvar/gui/webresult/css/
+-rwxrwxrwx   0 root         (0) root         (0)     2389 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/css/pqselect.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/email.png
+-rwxrwxrwx   0 root         (0) root         (0)     1150 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/favicon.ico
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.981476 oakvar-2.9.8/oakvar/gui/webresult/fonts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.042937 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/
+-rwxrwxrwx   0 root         (0) root         (0)   138764 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
+-rwxrwxrwx   0 root         (0) root         (0)   102868 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   146824 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   108752 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   143208 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106140 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   151052 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111808 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142920 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106108 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150628 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111708 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   140724 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
+-rwxrwxrwx   0 root         (0) root         (0)   104232 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   149996 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111392 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   144372 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106876 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   140632 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
+-rwxrwxrwx   0 root         (0) root         (0)   104332 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150092 2023-01-21 00:14:14.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111332 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142552 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
+-rwxrwxrwx   0 root         (0) root         (0)   105924 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150988 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   112184 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   133844 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
+-rwxrwxrwx   0 root         (0) root         (0)    98868 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142932 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   105804 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   151180 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   112048 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   135920 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
+-rwxrwxrwx   0 root         (0) root         (0)    99632 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   145480 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106496 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   245036 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   227180 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   324864 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)     5303 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/inter.css
+-rwxrwxrwx   0 root         (0) root         (0)    26456 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    19508 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    25692 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    18980 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    26312 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    19416 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    33072 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    25740 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.056785 oakvar-2.9.8/oakvar/gui/webresult/images/
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      379 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-down-right-circle.svg
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-down-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-down.svg
+-rwxrwxrwx   0 root         (0) root         (0)      311 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-left.svg
+-rwxrwxrwx   0 root         (0) root         (0)      312 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrow-up.svg
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/arrows-move.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2140 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/camera.svg
+-rwxrwxrwx   0 root         (0) root         (0)      291 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/caret-down.svg
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/caret-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)     3125 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/close.png
+-rwxrwxrwx   0 root         (0) root         (0)     2390 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/close.svg
+-rwxrwxrwx   0 root         (0) root         (0)      722 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/download-material-black.png
+-rwxrwxrwx   0 root         (0) root         (0)     2066 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/download.svg
+-rwxrwxrwx   0 root         (0) root         (0)      485 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/grip-vertical.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2219 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/pin.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2243 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/plus-circle-dotted.svg
+-rwxrwxrwx   0 root         (0) root         (0)      280 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/plus-circle-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)     4645 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/sorry.png
+-rwxrwxrwx   0 root         (0) root         (0)    25333 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/spinner.gif
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/x-lg.svg
+-rwxrwxrwx   0 root         (0) root         (0)      332 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/images/x.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.078599 oakvar-2.9.8/oakvar/gui/webresult/js/
+-rwxrwxrwx   0 root         (0) root         (0)   398184 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/Chart.js
+-rwxrwxrwx   0 root         (0) root         (0)    26580 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/axios.min.js
+-rwxrwxrwx   0 root         (0) root         (0)   137820 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/webresult/js/axios.min.js.map
+-rwxrwxrwx   0 root         (0) root         (0)     9278 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/dom-to-image.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     5839 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/download.js
+-rwxrwxrwx   0 root         (0) root         (0)    12091 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
+-rwxrwxrwx   0 root         (0) root         (0)   954164 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/graphics.js
+-rwxrwxrwx   0 root         (0) root         (0)    86659 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-3.2.1.min.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.097004 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
+-rwxrwxrwx   0 root         (0) root         (0)    12660 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1817 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.899421 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.097504 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rwxrwxrwx   0 root         (0) root         (0)   293430 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.103207 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
+-rwxrwxrwx   0 root         (0) root         (0)     6992 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6988 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6999 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6299 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)    32588 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rwxrwxrwx   0 root         (0) root         (0)    35997 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rwxrwxrwx   0 root         (0) root         (0)   520714 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rwxrwxrwx   0 root         (0) root         (0)    30747 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rwxrwxrwx   0 root         (0) root         (0)   253668 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    18705 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rwxrwxrwx   0 root         (0) root         (0)    15548 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    17342 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rwxrwxrwx   0 root         (0) root         (0)    13847 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     1340 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rwxrwxrwx   0 root         (0) root         (0)    13171 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery.tools.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     5451 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/jquery.url.js
+-rwxrwxrwx   0 root         (0) root         (0)    24103 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/masonry.pkgd.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    84772 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/packery.pkgd.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.117958 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/
+-rwxrwxrwx   0 root         (0) root         (0)    11583 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)   103213 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.122519 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/
+-rwxrwxrwx   0 root         (0) root         (0)      230 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      771 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
+-rwxrwxrwx   0 root         (0) root         (0)     1668 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rwxrwxrwx   0 root         (0) root         (0)      216 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.123712 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rwxrwxrwx   0 root         (0) root         (0)    76985 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.129308 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rwxrwxrwx   0 root         (0) root         (0)      750 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rwxrwxrwx   0 root         (0) root         (0)      769 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rwxrwxrwx   0 root         (0) root         (0)      802 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rwxrwxrwx   0 root         (0) root         (0)      805 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rwxrwxrwx   0 root         (0) root         (0)      636 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rwxrwxrwx   0 root         (0) root         (0)      774 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rwxrwxrwx   0 root         (0) root         (0)      782 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rwxrwxrwx   0 root         (0) root         (0)      822 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rwxrwxrwx   0 root         (0) root         (0)      773 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rwxrwxrwx   0 root         (0) root         (0)      675 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.132452 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
+-rwxrwxrwx   0 root         (0) root         (0)     1105 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)      613 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)      541 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     2973 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)    27759 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    12577 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     2408 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)     2026 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    16145 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)   481365 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)    12757 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rwxrwxrwx   0 root         (0) root         (0)   242931 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     1646 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)     1278 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rwxrwxrwx   0 root         (0) root         (0)      555 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.903021 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.132941 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.133453 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.133979 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.134488 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.134982 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.135442 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.135977 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.136420 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.136895 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.137355 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.137947 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.138398 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.138836 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.139277 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.139726 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.142065 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
+-rwxrwxrwx   0 root         (0) root         (0)     1042 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1164 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2677 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     3716 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)     1847 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    12583 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/pqselect.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    92225 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/raphael-min.js
+-rwxrwxrwx   0 root         (0) root         (0)   326538 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/js/tailwind.min.js
+-rwxrwxrwx   0 root         (0) root         (0)      900 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/webresult/jsonreporter.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.143146 oakvar-2.9.8/oakvar/gui/webresult/nocache/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.144635 oakvar-2.9.8/oakvar/gui/webresult/nocache/css/
+-rwxrwxrwx   0 root         (0) root         (0)     1714 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/css/singlevariantpage.css
+-rwxrwxrwx   0 root         (0) root         (0)    22655 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/css/style.css
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/css/widget.css
+-rwxrwxrwx   0 root         (0) root         (0)    21597 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.150194 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/
+-rwxrwxrwx   0 root         (0) root         (0)    24858 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/filter.js
+-rwxrwxrwx   0 root         (0) root         (0)    13065 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/infomgr.js
+-rwxrwxrwx   0 root         (0) root         (0)    30870 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/main.js
+-rwxrwxrwx   0 root         (0) root         (0)   103450 2023-04-13 11:11:33.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/setup.js
+-rwxrwxrwx   0 root         (0) root         (0)     4903 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/showvariant.js
+-rwxrwxrwx   0 root         (0) root         (0)    35998 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/singlevariantpage.js
+-rwxrwxrwx   0 root         (0) root         (0)    28858 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/util.js
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/variables.js
+-rwxrwxrwx   0 root         (0) root         (0)    22262 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/js/widgethelper.js
+-rwxrwxrwx   0 root         (0) root         (0)     5440 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/nocache/variant.html
+-rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/question.png
+-rwxrwxrwx   0 root         (0) root         (0)    29682 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/webresult/webresult.py
+-rwxrwxrwx   0 root         (0) root         (0)      163 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webresult/webviewer.yml
+-rwxrwxrwx   0 root         (0) root         (0)     4075 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/gui/websocket_handlers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.903899 oakvar-2.9.8/oakvar/gui/webstore/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.157961 oakvar-2.9.8/oakvar/gui/webstore/images/
+-rwxrwxrwx   0 root         (0) root         (0)      446 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/chat-dots-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      740 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/chat-dots.svg
+-rwxrwxrwx   0 root         (0) root         (0)      396 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/chat-left-text-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      545 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/chat-left-text.svg
+-rwxrwxrwx   0 root         (0) root         (0)    22268 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/done.png
+-rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/email.png
+-rwxrwxrwx   0 root         (0) root         (0)     2226 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/empty.png
+-rwxrwxrwx   0 root         (0) root         (0)     1763 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/folder.png
+-rwxrwxrwx   0 root         (0) root         (0)    38197 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/genericmodulelogo.png
+-rwxrwxrwx   0 root         (0) root         (0)     4766 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/hamburger.png
+-rwxrwxrwx   0 root         (0) root         (0)     1194 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/left_arrow.png
+-rwxrwxrwx   0 root         (0) root         (0)     3524 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/new.png
+-rwxrwxrwx   0 root         (0) root         (0)      474 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/no_logo_module.svg
+-rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/question.png
+-rwxrwxrwx   0 root         (0) root         (0)     1214 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/right_arrow.png
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/webstore/images/x-lg.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.904518 oakvar-2.9.8/oakvar/gui/websubmit/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.162982 oakvar-2.9.8/oakvar/gui/websubmit/images/
+-rwxrwxrwx   0 root         (0) root         (0)   372952 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/images/background.png
+-rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/images/logo.png
+-rwxrwxrwx   0 root         (0) root         (0)    22716 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/images/logo_only.png
+-rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/images/logo_transparent.png
+-rwxrwxrwx   0 root         (0) root         (0)    22247 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/images/logo_transparent_bw.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.165812 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/
+-rwxrwxrwx   0 root         (0) root         (0)      511 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/cravat.hg18.txt
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/cravat.hg19.txt
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/cravat.hg38.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:16.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg18.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg19.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg38.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.174035 oakvar-2.9.8/oakvar/gui/websubmit/nocache/
+-rwxrwxrwx   0 root         (0) root         (0)      692 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/alerts.js
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/element_constructors.js
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/element_getters.js
+-rwxrwxrwx   0 root         (0) root         (0)    55822 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/index.html
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/input.js
+-rwxrwxrwx   0 root         (0) root         (0)    14408 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/jobstable.js
+-rwxrwxrwx   0 root         (0) root         (0)     8242 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/login.html
+-rwxrwxrwx   0 root         (0) root         (0)     3796 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/multiuser.css
+-rwxrwxrwx   0 root         (0) root         (0)    16797 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/multiuser.js
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/select_modules.js
+-rwxrwxrwx   0 root         (0) root         (0)      228 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/showhide.js
+-rwxrwxrwx   0 root         (0) root         (0)     6783 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/submit.js
+-rwxrwxrwx   0 root         (0) root         (0)      484 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/util.js
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/websubmit.css
+-rwxrwxrwx   0 root         (0) root         (0)    39200 2023-02-22 05:21:01.000000 oakvar-2.9.8/oakvar/gui/websubmit/nocache/websubmit.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.174927 oakvar-2.9.8/oakvar/gui/www/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.176565 oakvar-2.9.8/oakvar/gui/www/assets/
+-rwxrwxrwx   0 root         (0) root         (0)    47521 2023-04-13 12:03:53.000000 oakvar-2.9.8/oakvar/gui/www/assets/index.b35f4d23.css
+-rwxrwxrwx   0 root         (0) root         (0)   381782 2023-04-13 13:09:00.000000 oakvar-2.9.8/oakvar/gui/www/assets/index.ef59c55d.js
+-rwxrwxrwx   0 root         (0) root         (0)     2074 2023-04-13 13:09:00.000000 oakvar-2.9.8/oakvar/gui/www/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.181120 oakvar-2.9.8/oakvar/lib/
+-rwxrwxrwx   0 root         (0) root         (0)       83 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.183040 oakvar-2.9.8/oakvar/lib/assets/
+-rwxrwxrwx   0 root         (0) root         (0)     9036 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/exampleinput
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.183842 oakvar-2.9.8/oakvar/lib/assets/license/
+-rwxrwxrwx   0 root         (0) root         (0)     1707 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/license/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/license/liftover.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.906260 oakvar-2.9.8/oakvar/lib/assets/module_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.185071 oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      277 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1195 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.186579 oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     2534 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1249 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.188337 oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.190100 oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      731 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1335 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.191679 oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-04-13 08:45:26.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1327 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.193130 oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     1742 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.yml
+-rwxrwxrwx   0 root         (0) root         (0)      135 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/oakvar.yml
+-rwxrwxrwx   0 root         (0) root         (0)     3078 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/output_columns.yml
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/assets/system.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.201691 oakvar-2.9.8/oakvar/lib/base/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21656 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/base/aggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)    37148 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/annotator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2714 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/base/commonmodule.py
+-rwxrwxrwx   0 root         (0) root         (0)    31089 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/converter.py
+-rwxrwxrwx   0 root         (0) root         (0)    14913 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    34828 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/master_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)     2742 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/mp_runners.py
+-rwxrwxrwx   0 root         (0) root         (0)    25174 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/postaggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)     7052 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/preparer.py
+-rwxrwxrwx   0 root         (0) root         (0)    43005 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/report_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)    47089 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/reporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    81178 2023-04-13 13:09:32.000000 oakvar-2.9.8/oakvar/lib/base/runner.py
+-rwxrwxrwx   0 root         (0) root         (0)    15184 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/base/vcf2vcf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2620 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)     7397 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.204418 oakvar-2.9.8/oakvar/lib/module/
+-rwxrwxrwx   0 root         (0) root         (0)    29864 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4110 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/module/cache.py
+-rwxrwxrwx   0 root         (0) root         (0)     3523 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/module/data_cache.py
+-rwxrwxrwx   0 root         (0) root         (0)    30959 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/module/local.py
+-rwxrwxrwx   0 root         (0) root         (0)    10491 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/module/remote.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.205900 oakvar-2.9.8/oakvar/lib/store/
+-rwxrwxrwx   0 root         (0) root         (0)     4330 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/store/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/store/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)    25288 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/store/db.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.206562 oakvar-2.9.8/oakvar/lib/store/ov/
+-rwxrwxrwx   0 root         (0) root         (0)     8121 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/store/ov/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.207003 oakvar-2.9.8/oakvar/lib/store/ov/account/
+-rwxrwxrwx   0 root         (0) root         (0)    19142 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/store/ov/account/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.208238 oakvar-2.9.8/oakvar/lib/system/
+-rwxrwxrwx   0 root         (0) root         (0)    34374 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1294 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/system/consts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:04.213462 oakvar-2.9.8/oakvar/lib/util/
+-rwxrwxrwx   0 root         (0) root         (0)      417 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5569 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/admin_util.py
+-rwxrwxrwx   0 root         (0) root         (0)      744 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/util/asyn.py
+-rwxrwxrwx   0 root         (0) root         (0)     5042 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/util/download.py
+-rwxrwxrwx   0 root         (0) root         (0)    19071 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/util/download_library.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/util/image.py
+-rwxrwxrwx   0 root         (0) root         (0)    20781 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/inout.py
+-rwxrwxrwx   0 root         (0) root         (0)     4961 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/module.py
+-rwxrwxrwx   0 root         (0) root         (0)     4932 2023-04-13 08:45:27.000000 oakvar-2.9.8/oakvar/lib/util/run.py
+-rwxrwxrwx   0 root         (0) root         (0)    11478 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/seq.py
+-rwxrwxrwx   0 root         (0) root         (0)    21930 2023-04-13 13:08:55.000000 oakvar-2.9.8/oakvar/lib/util/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 13:16:03.953677 oakvar-2.9.8/oakvar.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    19044 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      275 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-13 13:16:03.000000 oakvar-2.9.8/oakvar.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      625 2023-04-13 08:45:27.000000 oakvar-2.9.8/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 13:16:04.214614 oakvar-2.9.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2398 2023-04-13 13:15:24.000000 oakvar-2.9.8/setup.py
```

### Comparing `oakvar-2.9.7/LICENSE` & `oakvar-2.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/PKG-INFO` & `oakvar-2.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.7
+Version: 2.9.8
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
 Project-URL: Tracker, https://github.com/rkimoakbioinformatics/oakvar/issues
```

### Comparing `oakvar-2.9.7/README.rst` & `oakvar-2.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/__init__.py` & `oakvar-2.9.8/oakvar/api/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/config.py` & `oakvar-2.9.8/oakvar/api/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/module/__init__.py` & `oakvar-2.9.8/oakvar/api/module/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
         `None` if the module does not exist. A dict of { "code": [Path], "data": [Path] } if successful.}
     """
     from ...lib.module.local import pack_module
 
     if not module_name:
         return
     if not outdir:
-        outdir = Path(".").absolute()
+        outdir = Path(".").resolve()
     if isinstance(outdir, str):
-        outdir = Path(outdir).absolute()
+        outdir = Path(outdir).resolve()
     ret = pack_module(
         module_name=module_name,
         outdir=outdir,
         code_only=code_only,
         split=split,
         outer=outer,
     )
```

### Comparing `oakvar-2.9.7/oakvar/api/module/install_defs.py` & `oakvar-2.9.8/oakvar/api/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/module/ls_logic.py` & `oakvar-2.9.8/oakvar/api/module/ls_logic.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/new.py` & `oakvar-2.9.8/oakvar/api/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/store/__init__.py` & `oakvar-2.9.8/oakvar/api/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/store/account/__init__.py` & `oakvar-2.9.8/oakvar/api/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/system.py` & `oakvar-2.9.8/oakvar/api/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/test.py` & `oakvar-2.9.8/oakvar/api/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/api/util.py` & `oakvar-2.9.8/oakvar/api/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/__init__.py` & `oakvar-2.9.8/oakvar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/__main__.py` & `oakvar-2.9.8/oakvar/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/config.py` & `oakvar-2.9.8/oakvar/cli/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/gui.py` & `oakvar-2.9.8/oakvar/cli/gui.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/module/__init__.py` & `oakvar-2.9.8/oakvar/cli/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/module/info_fn.py` & `oakvar-2.9.8/oakvar/cli/module/info_fn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/module/install_defs.py` & `oakvar-2.9.8/oakvar/cli/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/module/ls.py` & `oakvar-2.9.8/oakvar/cli/module/ls.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/new.py` & `oakvar-2.9.8/oakvar/cli/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/report.py` & `oakvar-2.9.8/oakvar/cli/report.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/run.py` & `oakvar-2.9.8/oakvar/cli/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/store/__init__.py` & `oakvar-2.9.8/oakvar/cli/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/store/account/__init__.py` & `oakvar-2.9.8/oakvar/cli/store/account/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     return create(args)
 
 
 @cli_func
 def create(args, __name__="store account create"):
     from ....api.store.account import create
 
+    args["interactive"] = True
     ret = create(**args)
     return ret
 
 
 @cli_entry
 def cli_store_deleteaccount(args):
     return store_deleteaccount(args)
```

### Comparing `oakvar-2.9.7/oakvar/cli/system.py` & `oakvar-2.9.8/oakvar/cli/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/test.py` & `oakvar-2.9.8/oakvar/cli/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/util.py` & `oakvar-2.9.8/oakvar/cli/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/cli/version.py` & `oakvar-2.9.8/oakvar/cli/version.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/consts.py` & `oakvar-2.9.8/oakvar/gui/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/job_handlers.py` & `oakvar-2.9.8/oakvar/gui/job_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/multiuser.py` & `oakvar-2.9.8/oakvar/gui/multiuser.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/server.py` & `oakvar-2.9.8/oakvar/gui/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
                     self.logger.exception(e)
         return True
 
     def add_static_routes(self):
         from pathlib import Path
 
         assert self.app is not None
-        source_dir = Path(__file__).absolute().parent
+        source_dir = Path(__file__).resolve().parent
         self.app.router.add_static("/store", source_dir / "webstore")
         self.app.router.add_static("/result", source_dir / "webresult")
         self.app.router.add_static("/submit", source_dir / "websubmit")
         self.app.router.add_static("/", source_dir / "www")
 
     def setup_cors(self):
         from aiohttp_cors import ResourceOptions
```

### Comparing `oakvar-2.9.7/oakvar/gui/serveradmindb.py` & `oakvar-2.9.8/oakvar/gui/serveradmindb.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/store_handlers.py` & `oakvar-2.9.8/oakvar/gui/store_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/system_handlers.py` & `oakvar-2.9.8/oakvar/gui/system_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/system_message_db.py` & `oakvar-2.9.8/oakvar/gui/system_message_db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/system_worker.py` & `oakvar-2.9.8/oakvar/gui/system_worker.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/userjob.py` & `oakvar-2.9.8/oakvar/gui/userjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     user_jobs_dir_list = []
     root_jobs_dir = get_jobs_dir()
     if not root_jobs_dir:
         return user_jobs_dir_list
     for user_p in root_jobs_dir.glob("*"):
         if not user_p.is_dir():
             continue
-        user_jobs_dir_list.append(str(user_p.absolute()))
+        user_jobs_dir_list.append(str(user_p.resolve()))
     return user_jobs_dir_list
 
 
 def get_log_path_in_job_dir(
     job_dir: Optional[str], run_name: Optional[str] = None
 ) -> Optional[str]:
     from pathlib import Path
```

### Comparing `oakvar-2.9.7/oakvar/gui/util.py` & `oakvar-2.9.8/oakvar/gui/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/web_submit.py` & `oakvar-2.9.8/oakvar/gui/web_submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
                         wf.write(chunk)
                         chunk = await part.read_chunk()
             elif part.name == "options":
                 job_options = self.update_job_options(job_options, await part.json())
             elif part.name.startswith("module_option_file__"):
                 [_, module_name, option_name] = part.name.split("__")
                 fname = f"{module_name}__{option_name}"
-                path = get_unique_path(str((Path(job_dir) / fname).absolute()))
+                path = get_unique_path(str((Path(job_dir) / fname).resolve()))
                 with open(path, "wb") as wf:
                     wf.write(await part.read())
                 self.add_module_option(job_options, module_name, option_name, path)
         submit_options["job_options"] = job_options
         submit_options["input_files"] = input_files
         return submit_options
```

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/css/pqselect.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/email.png` & `oakvar-2.9.8/oakvar/gui/webresult/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/favicon.ico` & `oakvar-2.9.8/oakvar/gui/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/Inter_Web/inter.css` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/Inter_Web/inter.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-light-webfont.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `oakvar-2.9.8/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/arrows-move.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/camera.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/close.png` & `oakvar-2.9.8/oakvar/gui/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/close.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/download-material-black.png` & `oakvar-2.9.8/oakvar/gui/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/download.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/pin.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/plus-circle-dotted.svg` & `oakvar-2.9.8/oakvar/gui/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/sorry.png` & `oakvar-2.9.8/oakvar/gui/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/images/spinner.gif` & `oakvar-2.9.8/oakvar/gui/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/Chart.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/axios.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/axios.min.js.map` & `oakvar-2.9.8/oakvar/gui/webresult/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/dom-to-image.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/download.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/draggabilly.pkgd.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/draggabilly.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/graphics.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-3.2.1.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery.tools.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/jquery.url.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/masonry.pkgd.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/packery.pkgd.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/pqselect.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/raphael-min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/js/tailwind.min.js` & `oakvar-2.9.8/oakvar/gui/webresult/js/tailwind.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/jsonreporter.py` & `oakvar-2.9.8/oakvar/gui/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/css/singlevariantpage.css` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/css/style.css` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/css/widget.css` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/index.html` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/filter.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/infomgr.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/main.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/setup.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/showvariant.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/singlevariantpage.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/util.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/variables.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/js/widgethelper.js` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/nocache/variant.html` & `oakvar-2.9.8/oakvar/gui/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/question.png` & `oakvar-2.9.8/oakvar/gui/webresult/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webresult/webresult.py` & `oakvar-2.9.8/oakvar/gui/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websocket_handlers.py` & `oakvar-2.9.8/oakvar/gui/websocket_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/chat-dots.svg` & `oakvar-2.9.8/oakvar/gui/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/chat-left-text.svg` & `oakvar-2.9.8/oakvar/gui/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/done.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/email.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/empty.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/folder.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/genericmodulelogo.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/hamburger.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/left_arrow.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/new.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/question.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/webstore/images/right_arrow.png` & `oakvar-2.9.8/oakvar/gui/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/images/background.png` & `oakvar-2.9.8/oakvar/gui/websubmit/images/background.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/images/logo.png` & `oakvar-2.9.8/oakvar/gui/websubmit/images/logo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/images/logo_only.png` & `oakvar-2.9.8/oakvar/gui/websubmit/images/logo_only.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/images/logo_transparent.png` & `oakvar-2.9.8/oakvar/gui/websubmit/images/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/images/logo_transparent_bw.png` & `oakvar-2.9.8/oakvar/gui/websubmit/images/logo_transparent_bw.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/input-examples/cravat.hg19.txt` & `oakvar-2.9.8/oakvar/gui/websubmit/input-examples/cravat.hg19.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/input-examples/cravat.hg38.txt` & `oakvar-2.9.8/oakvar/gui/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg18.txt` & `oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg18.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg19.txt` & `oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg19.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/input-examples/vcf.hg38.txt` & `oakvar-2.9.8/oakvar/gui/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/alerts.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/alerts.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/element_getters.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/element_getters.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/index.html` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/input.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/input.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/jobstable.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/jobstable.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/login.html` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/login.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/multiuser.css` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/multiuser.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/multiuser.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/multiuser.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/select_modules.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/select_modules.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/submit.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/submit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/websubmit.css` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/websubmit/nocache/websubmit.js` & `oakvar-2.9.8/oakvar/gui/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/www/assets/index.b35f4d23.css` & `oakvar-2.9.8/oakvar/gui/www/assets/index.b35f4d23.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/www/assets/index.ef59c55d.js` & `oakvar-2.9.8/oakvar/gui/www/assets/index.ef59c55d.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/gui/www/index.html` & `oakvar-2.9.8/oakvar/gui/www/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/exampleinput` & `oakvar-2.9.8/oakvar/lib/assets/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/license/LICENSE` & `oakvar-2.9.8/oakvar/lib/assets/license/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/license/liftover.txt` & `oakvar-2.9.8/oakvar/lib/assets/license/liftover.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/annotator/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/annotator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.py` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/converter/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/converter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.py` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/mapper/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/mapper/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.py` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/postaggregator/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/postaggregator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/preparer/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/preparer/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.md` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.py` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/module_templates/reporter/template.yml` & `oakvar-2.9.8/oakvar/lib/assets/module_templates/reporter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/output_columns.yml` & `oakvar-2.9.8/oakvar/lib/assets/output_columns.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/assets/system.yml` & `oakvar-2.9.8/oakvar/lib/assets/system.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/base/aggregator.py` & `oakvar-2.9.8/oakvar/lib/base/aggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/base/annotator.py` & `oakvar-2.9.8/oakvar/lib/base/annotator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,19 @@
 from typing import Optional
 from typing import Any
 from typing import List
 from typing import Dict
+import polars as pl
 
 
 class BaseAnnotator(object):
     """BaseAnnotator.
     """
 
 
-    from ..util.util import get_crv_def
-    from ..util.util import get_crx_def
-    from ..util.util import get_crg_def
-    from ..consts import INPUT_LEVEL_KEY
-    from ..consts import VARIANT_LEVEL_KEY
-    from ..consts import GENE_LEVEL_KEY
-
-    valid_levels = ["variant", "gene"]
-    valid_input_formats = [INPUT_LEVEL_KEY, VARIANT_LEVEL_KEY, GENE_LEVEL_KEY]
-    id_col_defs = {"variant": get_crv_def()[0], "gene": get_crg_def()[0]}
-    default_input_columns: Dict[str, List[Any]] = {
-        INPUT_LEVEL_KEY: [x["name"] for x in get_crv_def()],
-        VARIANT_LEVEL_KEY: [x["name"] for x in get_crx_def()],
-        GENE_LEVEL_KEY: [x["name"] for x in get_crg_def()],
-    }
-    required_conf_keys = ["level", "output_columns"]
-
     def __init__(
         self,
         input_file: Optional[str] = None,
         secondary_inputs=None,
         run_name: Optional[str] = None,
         output_dir: Optional[str] = None,
         plainoutput: bool = False,
@@ -40,14 +24,15 @@
         title: Optional[str] = None,
         level: Optional[str] = None,
         input_format: Optional[str] = None,
         input_columns: List[str] = [],
         output_columns: List[Dict[str, Any]] = [],
         module_conf: Dict[str, Any] = {},
         code_version: Optional[str] = None,
+        df_mode: bool = False,
     ):
         """__init__.
 
         Args:
             input_file (Optional[str]): input_file
             secondary_inputs:
             run_name (Optional[str]): run_name
@@ -73,18 +58,34 @@
         from ..consts import GENE_LEVEL
         from ..consts import INPUT_LEVEL_KEY
         from ..consts import GENE_LEVEL_KEY
         from ..module.local import get_module_conf
         from ..module.data_cache import ModuleDataCache
         from ..exceptions import ModuleLoadingError
         from ..exceptions import LoggerError
+        from ..util.util import get_crv_def
+        from ..util.util import get_crx_def
+        from ..util.util import get_crg_def
+        from ..consts import INPUT_LEVEL_KEY
+        from ..consts import VARIANT_LEVEL_KEY
+        from ..consts import GENE_LEVEL_KEY
 
+        self.valid_levels = ["variant", "gene"]
+        self.valid_input_formats = [INPUT_LEVEL_KEY, VARIANT_LEVEL_KEY, GENE_LEVEL_KEY]
+        self.id_col_defs = {"variant": get_crv_def()[0], "gene": get_crg_def()[0]}
+        self.default_input_columns: Dict[str, List[Any]] = {
+            INPUT_LEVEL_KEY: [x["name"] for x in get_crv_def()],
+            VARIANT_LEVEL_KEY: [x["name"] for x in get_crx_def()],
+            GENE_LEVEL_KEY: [x["name"] for x in get_crg_def()],
+        }
+        self.required_conf_keys = ["level", "output_columns"]
+        self.script_path: str = ""
         self.module_options = module_options
         if input_file:
-            self.primary_input_path = Path(input_file).absolute()
+            self.primary_input_path = Path(input_file).resolve()
         else:
             self.primary_input_path = None
         self.secondary_inputs = secondary_inputs
         self.run_name = run_name
         self.output_dir = output_dir
         self.plain_output = plainoutput
         self.logtofile = logtofile
@@ -103,29 +104,33 @@
         self.dbconn = None
         self.cursor = None
         self.cmd_arg_parser = None
         self.json_colnames = None
         self.primary_input_reader = None
         self.output_path = None
         self.last_status_update_time = None
-        self.output_columns: Optional[List[Dict[str, Any]]] = None
+        self.output_columns: List[Dict[str, Any]] = []
         self.secondary_readers = {}
         self.output_writer = None
         self.log_path = None
         self.unique_excs = []
         self.log_handler = None
         self.parse_cmd_args()
         self.serveradmindb = serveradmindb
         self.supported_chroms = set(cannonical_chroms)
         self.module_type = "annotator"
         self.conf = {}
+        self.col_names: List[str] = []
+        self.full_col_names: Dict[str, str] = {}
+        self.df_dtypes: Dict[str, Any] = {}
+        self.df_mode: bool = df_mode
         if not self.main_fpath:
             if name:
                 self.module_name = name
-                self.module_dir = Path(os.getcwd()).absolute()
+                self.module_dir = Path(os.getcwd()).resolve()
             else:
                 raise ModuleLoadingError(msg="name argument should be given.")
             self.conf = module_conf.copy()
         else:
             self.module_name = self.main_fpath.stem
             self.module_dir = self.main_fpath.parent
             self.conf = get_module_conf(
@@ -201,14 +206,17 @@
             if "code_version" in self.conf:
                 self.code_version: str = self.conf["version"]
             elif "version" in self.conf:
                 self.code_version: str = self.conf["version"]
             else:
                 self.code_version: str = ""
         self.cache = ModuleDataCache(self.module_name, module_type=self.module_type)
+        self.var_ld: Dict[str, List[Any]] = {}
+        if self.df_mode:
+            self.setup_df()
 
     def set_output_columns(self, output_columns: List[Dict[str, Any]]):
         if not self.level:
             return
         key_col_name: str = self.id_col_defs[self.level].get("name", "")
         if not key_col_name:
             return
@@ -219,14 +227,15 @@
                 break
         if not key_col_found:
             output_columns = [self.id_col_defs[self.level]] + output_columns
         self.output_columns = output_columns
         if not self.conf:
             self.conf = {}
         self.conf["output_columns"] = output_columns
+        self.col_names = [v.get("name", "") for v in output_columns if v.get("name") != "uid"]
 
     def set_ref_colname(self):
         """set_ref_colname.
         """
         ref_colnames = {
             "variant": "uid",
             "gene": "hugo",
@@ -319,15 +328,15 @@
         """
         import re
         from pathlib import Path
 
         if self.secondary_inputs:
             for secondary_def in self.secondary_inputs:
                 sec_name, sec_path = re.split(r"(?<!\\)=", secondary_def)
-                self.secondary_paths[sec_name] = str(Path(sec_path).absolute())
+                self.secondary_paths[sec_name] = str(Path(sec_path).resolve())
         if not self.output_dir and self.primary_input_path:
             self.output_dir = str(self.primary_input_path.parent)
         if self.run_name is not None:
             self.output_basename = self.run_name
         elif self.primary_input_path:
             self.output_basename = self.primary_input_path.name
             if Path(self.output_basename).suffix in [".crv", ".crg", ".crx"]:
@@ -423,21 +432,73 @@
 
         Args:
             df:
         """
         _ = df
         raise NotImplementedError("annotate_df method should be implemented.")
 
-    def run_df(self, df):
+    def setup_df(self):
+        self.full_col_names = {col_name: f"{self.module_name}__{col_name}" for col_name in self.col_names if col_name != "uid"}
+        self.df_dtypes = {}
+        for col_def in self.output_columns:
+            col_name = col_def.get("name")
+            if not col_name or col_name == "uid":
+                continue
+            ty = col_def.get("type")
+            if ty == "string":
+                dtype = pl.Utf8
+            elif ty == "int":
+                dtype = pl.Int64
+            elif ty == "float":
+                dtype = pl.Float64
+            else:
+                dtype = pl.Utf8
+            self.df_dtypes[self.full_col_names[col_name]] = dtype
+        self.base_setup(mode="df")
+        self.make_json_colnames()
+
+    def run_df(self, df: pl.DataFrame):
         """run_df.
 
         Args:
             df:
         """
-        return self.annotate_df(df)
+        for col_name in self.col_names:
+            full_col_name = self.full_col_names[col_name]
+            self.var_ld[full_col_name] = []
+        for row in df.iter_rows(named=True):
+            input_data: Dict[str, Dict[str, Any]] = {}
+            for k, v in row.items():
+                if "__" in k:
+                    module_name, col_name = k.split("__")
+                    if module_name not in input_data:
+                        input_data[module_name] = {}
+                    input_data[module_name][col_name] = v
+                else:
+                    input_data[k] = v
+            output_dict = self.annotate(input_data)
+            for col_name in self.col_names:
+                if not output_dict:
+                    val = None
+                else:
+                    val = output_dict.get(col_name)
+                self.var_ld[self.full_col_names[col_name]].append(val)
+        num_cols = df.shape[1]
+        for i, col_name in enumerate(self.col_names):
+            full_col_name = self.full_col_names[col_name]
+            dtype = self.df_dtypes[full_col_name]
+            df.insert_at_idx(num_cols + i, pl.Series(full_col_name, self.var_ld[full_col_name], dtype=dtype))
+        return df
+
+
+    def get_output_col_def(self, col_name):
+        for col_def in self.output_columns:
+            if col_def.get("name") == col_name:
+                return col_def
+        return None
 
     def run(self, df=None):
         """run.
 
         Args:
             df:
         """
@@ -617,20 +678,21 @@
                 print(err_str_log)
         err_logger_s = f"{fn}:{lnum}\t{str(e)}"
         if self.error_logger:
             self.error_logger.error(err_logger_s)
         else:
             print(err_logger_s)
 
-    def base_setup(self):
+    def base_setup(self, mode: str="old"):
         """base_setup.
         """
-        self._setup_primary_input()
-        self._setup_secondary_inputs()
-        self._setup_outputs()
+        if mode == "old":
+            self._setup_primary_input()
+            self._setup_secondary_inputs()
+            self._setup_outputs()
         self.connect_db()
         self.setup()
         if not hasattr(self, "supported_chroms"):
             self.supported_chroms = set(
                 ["chr" + str(n) for n in range(1, 23)] + ["chrX", "chrY"]
             )
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/commonmodule.py` & `oakvar-2.9.8/oakvar/lib/base/commonmodule.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/base/mapper.py` & `oakvar-2.9.8/oakvar/lib/base/mapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from typing import Optional
+from typing import Any
 from typing import List
 from typing import Dict
+import polars as pl
 
 
 class BaseMapper(object):
     def __init__(
         self,
+        name: str = "",
         input_file: Optional[str] = None,
         run_name: Optional[str] = None,
         output_dir: Optional[str] = None,
         seekpos: Optional[int] = None,
         chunksize: Optional[int] = None,
         primary_transcript: List[str] = ["mane"],
         serveradmindb=None,
         module_options: Dict = {},
+        output_columns: List[Dict[str, Any]] = [],
         postfix: str = "",
+        df_mode: bool = False,
     ):
         from time import time
         from pathlib import Path
         from os import makedirs
         import sys
         from ..module.local import get_module_conf
         from ..consts import STANDARD_INPUT_FILE_SUFFIX
 
         self.input_dir: Optional[Path] = None
         self.output_dir: Optional[Path] = None
         self.input_fname: Optional[str] = None
         self.input_path: Optional[Path] = None
         if input_file:
-            p = Path(input_file).absolute()
+            p = Path(input_file).resolve()
             self.input_dir = p.parent
             self.input_fname = p.name
             self.input_path = p
         if output_dir:
             self.output_dir = Path(output_dir)
         elif self.input_dir:
             self.output_dir = self.input_dir
@@ -55,22 +60,57 @@
         self.crx_path = None
         self.crg_path = None
         self.crx_writer = None
         self.crg_writer = None
         self.input_fname = None
         self.logger = None
         self.error_logger = None
+        self.col_names: List[str] = []
+        self.full_col_names: Dict[str, str] = {}
         self.unique_excs = []
+        self.df_mode = df_mode
         self.t = time()
         main_fpath = Path(sys.modules[self.__class__.__module__].__file__ or "")
-        self.module_name = main_fpath.stem
+        if name:
+            self.module_name = name
+        else:
+            self.module_name = main_fpath.stem
+        self.name = self.module_name
         self.module_dir = main_fpath.parent
         self.gene_info = {}
         self.setup_logger()
-        self.conf = get_module_conf(self.module_name, module_type="mapper")
+        self.conf: Dict[str, Any] = (
+            get_module_conf(self.module_name, module_type="mapper") or {}
+        )
+        self.set_output_columns(output_columns)
+        self.var_ld: Dict[str, List[Any]] = {}
+        self.df_dtypes: Dict[str, Any] = {}
+        self.setup()
+        self.extra_setup()
+        if self.df_mode:
+            self.setup_df()
+
+    def set_output_columns(self, output_columns: List[Dict[str, Any]] = []):
+        from ..util.util import get_crv_def
+        from ..util.util import get_crx_def
+
+        if output_columns:
+            self.output_columns = output_columns.copy()
+            self.conf["output_columns"] = self.output_columns.copy()
+        elif "output_columns" in self.conf:
+            self.output_columns = self.conf["output_columns"].copy()
+        else:
+            self.output_columns = get_crx_def().copy()
+            self.conf["output_columns"] = self.output_columns.copy()
+        crv_col_names = [col_def.get("name") for col_def in get_crv_def()]
+        self.col_names = [
+            v.get("name", "")
+            for v in self.output_columns
+            if v.get("name") not in crv_col_names
+        ]
 
     def setup(self):
         raise NotImplementedError("Mapper must have a setup() method.")
 
     def extra_setup(self):
         pass
 
@@ -278,19 +318,68 @@
                         )
                 else:
                     if value in rs_dic[colname]:
                         value = rs_dic[colname][value]
                 d[colname] = value
         return d
 
+    def setup_df(self):
+        self.full_col_names = {
+            col_name: f"{col_name}" for col_name in self.col_names if col_name != "uid"
+        }
+        self.df_dtypes = {}
+        for col_def in self.output_columns:
+            col_name = col_def.get("name")
+            if not col_name or col_name not in self.col_names:
+                continue
+            if col_name == "uid":
+                continue
+            ty = col_def.get("type")
+            if ty == "string":
+                dtype = pl.Utf8
+            elif ty == "int":
+                dtype = pl.Int64
+            elif ty == "float":
+                dtype = pl.Float64
+            else:
+                dtype = pl.Utf8
+            self.df_dtypes[self.full_col_names[col_name]] = dtype
+
+    def run_df(self, df: pl.DataFrame) -> pl.DataFrame:
+        for full_col_name in self.full_col_names:
+            self.var_ld[full_col_name] = []
+        for input_data in df.iter_rows(named=True):
+            if input_data["alt_base"] == "*":
+                output_dict = {}
+            else:
+                output_dict = self.map(input_data)
+            for col_name in self.col_names:
+                if not output_dict:
+                    self.var_ld[self.full_col_names[col_name]].append(None)
+                else:
+                    self.var_ld[self.full_col_names[col_name]].append(
+                        output_dict.get(col_name)
+                    )
+        num_cols = df.shape[1]
+        for i, full_col_name in enumerate(self.full_col_names):
+            df.insert_at_idx(
+                num_cols + i,
+                pl.Series(
+                    full_col_name,
+                    self.var_ld[full_col_name],
+                    dtype=self.df_dtypes[full_col_name],
+                ),
+            )
+        return df
+
     def run(self, __pos_no__):
         from time import time, asctime, localtime
         from ..util.run import update_status
 
-        self.setup()
+        # self.setup()
         self.setup_input_output()
         self.extra_setup()
         if (
             self.logger is None
             or self.conf is None
             or self.reader is None
             or self.crx_writer is None
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/master_converter.py` & `oakvar-2.9.8/oakvar/lib/base/master_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 from typing import Any
 from typing import Optional
-from typing import Union
 from typing import List
 from typing import Dict
 from typing import Tuple
-from typing import TextIO
-from oakvar import BaseConverter
+from oakvar.lib.base.converter import BaseConverter
 from pyliftover import LiftOver
-from io import BufferedReader
 from re import compile
 
 chromdict = {
     "chrx": "chrX",
     "chry": "chrY",
     "chrMT": "chrM",
     "chrMt": "chrM",
     "chr23": "chrX",
     "chr24": "chrY",
 }
 base_re = compile("^[ATGC]+|[-]+$")
 
-class LinesData:
-    def __init__(self, lines_data: Dict[int, List[Tuple[int, Dict[str, Any]]]]):
-        self.lines_data = lines_data
-
 def handle_genotype(variant):
     if "genotype" in variant and "." in variant["genotype"]:
         variant["genotype"] = variant["genotype"].replace(".", variant["ref_base"])
 
 def flush_err_holder(err_holder: list, error_logger, force: bool=False):
     if len(err_holder) > 1000 or force:
         for err_line in err_holder:
@@ -257,15 +250,15 @@
 
 
 class MasterConverter(object):
     def __init__(
         self,
         inputs: List[str] = [],
         input_format: Optional[str] = None,
-        name: Optional[str] = None,
+        run_name: Optional[str] = None,
         output_dir: Optional[str] = None,
         genome: Optional[str] = None,
         serveradmindb=None,
         conf: Dict = {},
         module_options: Dict = {},
         input_encoding=None,
         ignore_sample: bool=False,
@@ -279,15 +272,15 @@
         self.logger = None
         self.crv_writer = None
         self.crs_writer = None
         self.crm_writer = None
         self.crl_writer = None
         self.converters = {}
         self.available_input_formats = []
-        self.input_paths = None
+        self.input_paths: List[str] = []
         self.input_dir = None
         self.input_path_dict = {}
         self.input_path_dict2 = {}
         self.input_file_handles: Dict[str, str] = {}
         self.output_base_fname: Optional[str] = None
         self.error_logger = None
         self.unique_excs: Dict[str, int] = {}
@@ -298,15 +291,15 @@
         self.crl_path = None
         self.do_liftover = None
         self.do_liftover_chrM = None
         self.lifter = None
         self.module_options = None
         self.given_input_assembly: Optional[str] = None
         self.converter_by_input_path: Dict[str, Optional[BaseConverter]] = {}
-        self.extra_output_columns = []
+        self.extra_output_columns: List[Dict[str, Any]] = []
         self.file_num_valid_variants = 0
         self.file_error_lines = 0
         self.total_num_valid_variants = 0
         self.total_error_lines = 0
         self.fileno = 0
         self.ignore_sample = ignore_sample
         self.total_num_converted_variants = 0
@@ -323,15 +316,15 @@
             "chr23": "chrX",
             "chr24": "chrY",
         }
         if not inputs:
             raise ExpectedException("Input files are not given.")
         self.inputs = inputs
         self.format = input_format
-        self.name = name
+        self.run_name = run_name
         self.output_dir = output_dir
         self.genome = genome
         self.parse_inputs()
         self.parse_output_dir()
         self.given_input_assembly = genome
         self.conf: Dict = {}
         self.module_options = module_options
@@ -379,15 +372,15 @@
         self.lifter = get_lifter(source_assembly=genome_assembly)
 
     def parse_inputs(self):
         from pathlib import Path
 
         self.input_paths = []
         self.input_paths = [
-            str(Path(x).absolute()) for x in self.inputs if x != "-"
+            str(Path(x).resolve()) for x in self.inputs if x != "-"
         ]
         self.input_dir = str(Path(self.input_paths[0]).parent)
         for i in range(len(self.input_paths)):
             self.input_path_dict[i] = self.input_paths[i]
             self.input_path_dict2[self.input_paths[i]] = i
 
     def parse_output_dir(self):
@@ -396,15 +389,15 @@
 
         if not self.output_dir:
             self.output_dir = self.input_dir
         if not self.output_dir:
             raise
         if not (Path(self.output_dir).exists()):
             makedirs(self.output_dir)
-        self.output_base_fname: Optional[str] = self.name
+        self.output_base_fname: Optional[str] = self.run_name
         if not self.output_base_fname:
             if not self.input_paths:
                 raise
             self.output_base_fname = Path(self.input_paths[0]).name
 
     def get_file_object_for_input_path(self, input_path: str):
         from pathlib import Path
@@ -444,53 +437,47 @@
         from logging import getLogger
 
         self.logger = getLogger("oakvar.converter")
         self.error_logger = getLogger("err.converter")
 
     def collect_converters(self):
         from oakvar.lib.module.local import get_local_module_infos_of_type
-        from oakvar.lib.util.util import load_class
+        from ..util.module import get_converter_class
 
         for module_name, module_info in get_local_module_infos_of_type(
             "converter"
         ).items():
             try:
-                cls = load_class(module_info.script_path)
-                converter = cls(ignore_sample=self.ignore_sample)
-            except Exception:
+                cls = get_converter_class(module_name)
+                converter = cls(inputs=self.input_paths, code_version=module_info.version)
+            except Exception as e:
+                import traceback
+
                 if self.logger:
-                    self.logger.error(f"Skipping {module_name} as it could not be loaded.")
+                    self.logger.error(f"{traceback.format_exc()}\nSkipping {module_name} as it could not be loaded. ({e})")
                 continue
             # TODO: backward compatibility
-            converter.output_dir = None
-            converter.run_name = None
-            converter.module_name = module_name
-            converter.name = module_info.name
-            converter.version = module_info.version
-            converter.conf = module_info.conf
-            converter.script_path = module_info.script_path
-            format_name = module_info.conf.get("format_name")
+            format_name: str = module_info.conf.get("format_name", "")
             # end of backward compatibility
             if format_name:
                 converter.format_name = format_name
             elif not hasattr(converter, "format_name"):
                 converter.format_name = module_name.split("-")[0]
             if not converter.format_name:
                 if self.logger:
                     self.logger.info(
                         f"Skipping {module_info.name} as it does not "
                         + "have format_name defined."
                     )
                 continue
-            converter.module_name = module_info.name
             if converter.format_name not in self.converters:
                 self.converters[converter.format_name] = converter
             else:
                 if self.outer:
-                    self.outer.write(
+                    self.outer.error(
                         f"{module_info.name} is skipped because "
                         + f"{converter.format_name} is already handled by "
                         + f"{self.converters[converter.format_name].name}."
                     )
                 continue
         self.available_input_formats = list(self.converters.keys())
 
@@ -535,32 +522,31 @@
                         self.error_logger.error(traceback.format_exc())
                     check_success = False
                 if check_success:
                     converter = check_converter
                     break
         if converter:
             if self.logger:
-                self.logger.info(f"Using {converter.module_name} for {input_path}")
+                self.logger.info(f"Using {converter.name} for {input_path}")
             return converter
         return None
 
     def set_converter_properties(self, converter):
         from oakvar.lib.exceptions import SetupError
         from oakvar.lib.module.local import get_module_code_version
 
         if self.conf is None:
             raise SetupError()
         converter.output_dir = self.output_dir
         converter.run_name = self.output_base_fname
-        module_name = converter.module_name
-        converter.version = get_module_code_version(converter.module_name)
-        if module_name in self.conf:
+        converter.version = get_module_code_version(converter.name)
+        if converter.name in self.conf:
             if hasattr(converter, "conf") is False:
                 converter.conf = {}
-            converter.conf.update(self.conf[module_name])
+            converter.conf.update(self.conf[converter.name])
 
     def setup_crv_writer(self):
         from pathlib import Path
         from oakvar.lib.util.util import get_crv_def
         from oakvar.lib.util.inout import FileWriter
         from oakvar.lib.consts import crv_idx
         from oakvar.lib.consts import STANDARD_INPUT_FILE_SUFFIX
@@ -632,18 +618,14 @@
         )
         self.crl_writer = FileWriter(self.crl_path)
         self.crl_writer.add_columns(crl_def)
         self.crl_writer.write_definition()
         self.crl_writer.write_names("original_input", "Original Input", "")
 
     def open_output_files(self):
-        from oakvar.lib.exceptions import SetupError
-
-        if not self.output_base_fname or not self.output_dir:
-            raise SetupError()
         self.setup_crv_writer()
         self.setup_crs_writer()
         self.setup_crm_writer()
         self.setup_crl_writer()
 
     def log_input_and_genome_assembly(self, input_path, genome_assembly, converter):
         if not self.logger:
@@ -657,21 +639,21 @@
         from oakvar.lib.util.util import log_module
         from oakvar.lib.exceptions import NoConverterFound
 
         encoding = self.input_file_handles[input_path]
         converter = self.converter_by_input_path[input_path]
         if not converter:
             raise NoConverterFound(input_path)
-        if not converter.module_name or not converter.format_name:
+        if not converter.name or not converter.format_name:
             raise NoConverterFound(input_path)
         self.input_formats.append(converter.format_name)
         self.fileno += 1
         self.set_converter_properties(converter)
         log_module(converter, self.logger)
-        self.error_logger = getLogger("err." + converter.module_name)
+        self.error_logger = getLogger("err." + converter.name)
         converter.input_path = input_path
         converter.input_paths = self.input_paths
         converter.setup(input_path, encoding=encoding)
         genome_assembly = self.get_genome_assembly(converter)
         self.genome_assemblies.append(genome_assembly)
         self.log_input_and_genome_assembly(input_path, genome_assembly, converter)
         self.set_do_liftover(genome_assembly, converter, input_path)
@@ -695,30 +677,30 @@
 
         if "ref_base" not in variant or variant["ref_base"] in [
             "",
             ".",
         ]:
             if not self.wgs_reader:
                 raise
-            variant["ref_base"] = self.wgs_reader.get_bases(
+            variant["ref_base"] = self.wgs_reader.get_bases( # type: ignore
                 variant.get("chrom"), int(variant["pos"])
             ).upper()
         else:
             ref_base = variant["ref_base"]
             if ref_base == "" and variant["alt_base"] not in [
                 "A",
                 "T",
                 "C",
                 "G",
             ]:
                 raise IgnoredVariant("Reference base required for non SNV")
             elif ref_base is None or ref_base == "":
                 if not self.wgs_reader:
                     raise
-                variant["ref_base"] = self.wgs_reader.get_bases(
+                variant["ref_base"] = self.wgs_reader.get_bases( # type: ignore
                     variant.get("chrom"), int(variant.get("pos"))
                 )
 
     def handle_genotype(self, variant):
         if "genotype" in variant and "." in variant["genotype"]:
             variant["genotype"] = variant["genotype"].replace(".", variant["ref_base"])
 
@@ -892,15 +874,14 @@
         update_status(status, logger=self.logger, serveradmindb=self.serveradmindb)
 
     def perform_liftover_if_needed(self, variant) -> Optional[Dict[str, Any]]:
         from copy import copy
         from oakvar.lib.util.seq import liftover_one_pos
         from oakvar.lib.util.seq import liftover
 
-        assert self.crl_writer is not None
         if self.is_chrM(variant):
             needed = self.do_liftover_chrM
         else:
             needed = self.do_liftover
         if needed:
             prelift_wdict = copy(variant)
             #prelift_wdict["uid"] = self.uid
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/mp_runners.py` & `oakvar-2.9.8/oakvar/lib/base/mp_runners.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def annot_from_queue(
     start_queue, end_queue, queue_populated, serveradmindb, logtofile, log_path
 ):
     from ..util.util import load_class
     from logging import getLogger, StreamHandler, FileHandler, Formatter
     from queue import Empty
     from ..exceptions import ModuleLoadingError
+    from ..base.annotator import BaseAnnotator
 
     while True:
         try:
             task = start_queue.get(True, 1)
         except Empty:
             if queue_populated:
                 break
@@ -38,23 +39,23 @@
             logger.addHandler(log_handler)
         except Exception:
             import traceback
 
             traceback.print_exc()
         try:
             kwargs["serveradmindb"] = serveradmindb
-            annotator_class = load_class(module.script_path, "Annotator")
-            if not annotator_class:
-                annotator_class = load_class(module.script_path, "CravatAnnotator")
-            if annotator_class:
-                annotator = annotator_class(**kwargs)
-                annotator.run()
-                end_queue.put(module.name)
-            else:
-                raise ModuleLoadingError(msg=f"Annotator of {module.name} could not be loaded.")
+            annotator_class = load_class(module.script_path)
+            if not issubclass(annotator_class, BaseAnnotator):
+                err = ModuleLoadingError(module_name=module.name)
+                if logger:
+                    logger.exception(err)
+                continue
+            annotator = annotator_class(**kwargs)
+            annotator.run()
+            end_queue.put(module.name)
         except Exception:
             err = ModuleLoadingError(module_name=module.name)
             if logger:
                 logger.exception(err)
 
 
 def mapper_runner(
@@ -64,33 +65,29 @@
     run_name,
     output_dir,
     module_name,
     pos_no,
     primary_transcript,
     serveradmindb,
 ):
-    from ..util.util import load_class
+    from ..util.module import get_mapper_class
     from ..module.local import get_local_module_info
     from .mapper import BaseMapper
-    from ..exceptions import ModuleLoadingError
 
-    output = None
     module = get_local_module_info(module_name)
-    if module is not None:
-        if primary_transcript:
-            primary_transcript = primary_transcript.split(";")
-        genemapper_class = load_class(module.script_path, "Mapper")
-        if genemapper_class:
-            genemapper = genemapper_class(
-                input_file=crv_path,
-                run_name=run_name,
-                seekpos=seekpos,
-                chunksize=chunksize,
-                postfix=f".{pos_no:010.0f}",
-                primary_transcript=primary_transcript,
-                serveradmindb=serveradmindb,
-                output_dir=output_dir,
-            )
-            output = genemapper.run(pos_no)
-        else:
-            raise ModuleLoadingError(msg=f"Mapper of {module_name} could not be loaded.")
+    if not module:
+        return None
+    if primary_transcript:
+        primary_transcript = primary_transcript.split(";")
+    genemapper_class: Type[BaseMapper] = get_mapper_class(module_name)
+    genemapper = genemapper_class(
+        input_file=crv_path,
+        run_name=run_name,
+        seekpos=seekpos,
+        chunksize=chunksize,
+        postfix=f".{pos_no:010.0f}",
+        primary_transcript=primary_transcript,
+        serveradmindb=serveradmindb,
+        output_dir=output_dir,
+    )
+    output = genemapper.run(pos_no)
     return output
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/postaggregator.py` & `oakvar-2.9.8/oakvar/lib/base/postaggregator.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         serveradmindb=None,
         outer=None,
         module_options: Dict = {},
     ):
         from ..exceptions import ArgumentError
         from ..util.util import get_result_dbpath
 
+        self.script_path: str = ""
         self.serveradmindb = serveradmindb
         self.run_name = run_name
         self.output_dir = output_dir
         self.level = None
         self.levelno = None
         self.module_options = None
         self.db_path = None
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/preparer.py` & `oakvar-2.9.8/oakvar/lib/base/preparer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         from pathlib import Path
         from os.path import split
         from os import makedirs
         from ..module.local import get_module_conf
         from ..exceptions import ModuleLoadingError
         from ..exceptions import NoInput
 
+        self.script_path: str = ""
         self.serveradmindb = serveradmindb
         self.outer = outer
         self.cmd_parser = None
         self.input_path = None
         self.input_dir = None
         self.reader = None
         self.output_dir: Optional[str] = None
@@ -37,15 +38,15 @@
         self.unique_excs = []
         self.uid = 0
         fp = sys.modules[self.__module__].__file__
         if not fp:
             raise ModuleLoadingError(module_name=self.__module__)
         self.main_fpath = Path(fp).resolve()
         self.module_name = self.main_fpath.stem
-        self.input_path = Path(input_file).absolute() if input_file else None
+        self.input_path = Path(input_file).resolve() if input_file else None
         if not self.input_path:
             raise NoInput()
         self.output_path = f"{self.input_path}.{self.module_name}.prep.crv"
         self.input_dir, self.input_fname = split(self.input_path)
         if output_dir:
             self.output_dir = output_dir
         else:
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/report_filter.py` & `oakvar-2.9.8/oakvar/lib/base/report_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,15 @@
         self.mode = mode
         if self.mode == "main":
             self.stdout = True
         else:
             self.stdout = False
         self.dbpath = dbpath
         if self.dbpath is not None:
-            self.dbpath = str(Path(dbpath).absolute())
-        #self.conn = None
+            self.dbpath = str(Path(dbpath).resolve())
         self.filterpath = filterpath
         self.cmd = None
         self.level = None
         self.filter = filter
         self.filtername = None
         self.filterstring = filterstring
         self.filtersql = filtersql
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/reporter.py` & `oakvar-2.9.8/oakvar/lib/base/reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from typing import Any
 from typing import Optional
 from typing import Union
 from typing import Dict
 from typing import List
 from pathlib import Path
+import polars as pl
 
 
 class BaseReporter:
     def __init__(
         self,
         dbpath: str="",
         report_types: List[str] = [],
         filterpath: Optional[str] = None,
         filter=None,
         filtersql: Optional[str] = None,
         filtername: Optional[str] = None,
         filterstring: Optional[str] = None,
         savepath: Optional[Path] = None,
         confpath: Optional[str] = None,
-        module_name: Optional[str] = None,
+        name: Optional[str] = None,
         nogenelevelonvariantlevel: bool = False,
         inputfiles: Optional[List[str]] = None,
         separatesample: bool = False,
         output_dir: Optional[str] = None,
         run_name: str = "",
         module_options: Dict = {},
         includesample: Optional[List[str]] = [],
         excludesample: Optional[List[str]] = None,
         package: Optional[str] = None,
         cols: Optional[List[str]] = None,
         level: Optional[str] = None,
         user: Optional[str] = None,
+        module_conf: Dict[str, Any] = {},
         no_summary: bool = False,
         logtofile: bool = False,
+        df_mode: bool = False,
         serveradmindb=None,
         outer=None,
     ):
+        import sys
+        import os
         from ..system.consts import DEFAULT_SERVER_DEFAULT_USERNAME
+        from ..exceptions import ModuleLoadingError
+        from ..module.local import get_module_conf
 
+        self.module_type = "annotator"
+        self.script_path: str = ""
         self.dbpath = dbpath
         self.report_types = report_types
         self.filterpath = filterpath
         self.filter = filter
         self.filtersql = filtersql
         self.filtername = filtername
         self.filterstring = filterstring
         self.savepath = savepath
         self.confpath = confpath
-        self.module_name = module_name
+        self.module_name = name
         self.nogenelevelonvariantlevel = nogenelevelonvariantlevel
         self.inputfiles = inputfiles
         self.separatesample = separatesample
         self.output_dir = output_dir
         self.run_name = run_name
         self.module_options = module_options
         self.includesample = includesample
@@ -80,31 +89,56 @@
         self.display_select_columns = {}
         self.extracted_cols: Dict[str, Any] = {}
         self.extracted_col_names: Dict[str, List[str]] = {}
         self.extracted_col_nos: Dict[str, List[int]] = {}
         self.retrieved_col_names: Dict[str, List[str]] = {}
         self.conn = None
         self.levels_to_write = None
-        self.conf = None
         self.module_conf = None
         self.output_basename = None
         self.extract_columns_multilevel = {}
         self.logger = None
         self.error_logger = None
         self.unique_excs = None
         self.mapper_name: str = ""
         self.no_log = False
         self.colcount = {}
         self.columns = {}
         self.conns = []
         self.logtofile = logtofile
         self.dictrow: bool = True
+        if self.__module__ == "__main__":
+            fp = None
+            self.main_fpath = None
+        else:
+            fp = sys.modules[self.__module__].__file__
+            if not fp:
+                raise ModuleLoadingError(module_name=self.__module__)
+            self.main_fpath = Path(fp).resolve()
+        if not self.main_fpath:
+            if name:
+                self.module_name = name
+                self.module_dir = Path(os.getcwd()).resolve()
+            else:
+                raise ModuleLoadingError(msg="name argument should be given.")
+            self.conf = module_conf.copy()
+        else:
+            self.module_name = self.main_fpath.stem
+            self.module_dir = self.main_fpath.parent
+            self.conf = get_module_conf(
+                self.module_name,
+                module_type=self.module_type,
+                module_dir=self.module_dir,
+            )
+            if not self.conf:
+                self.conf = {}
         self.gene_summary_datas = {}
         self.total_norows: Optional[int] = None
         self.legacy_samples_col = False
+        self.df_mode = df_mode
         self.modules_to_add_to_base = []
         self.check_and_setup_args()
         self._setup_logger()
 
     async def exec_db(self, func, *args, **kwargs):
         from ..exceptions import DatabaseConnectionError
 
@@ -123,33 +157,34 @@
     def check_and_setup_args(self):
         import sqlite3
         import json
         from pathlib import Path
         from ..module.local import get_module_conf
         from ..exceptions import WrongInput
 
-        if not Path(self.dbpath).exists():
+        if not self.df_mode and not Path(self.dbpath).exists():
             raise WrongInput(msg=self.dbpath)
-        try:
-            with sqlite3.connect(self.dbpath) as db:
-                db.execute("select count(*) from info")
-                db.execute("select count(*) from variant")
-                db.execute("select count(*) from gene")
-        except Exception:
-            raise WrongInput(msg=f"{self.dbpath} is not an OakVar result database")
+        if not self.df_mode:
+            try:
+                with sqlite3.connect(self.dbpath) as db:
+                    db.execute("select count(*) from info")
+                    db.execute("select count(*) from variant")
+                    db.execute("select count(*) from gene")
+            except Exception:
+                raise WrongInput(msg=f"{self.dbpath} is not an OakVar result database")
         if not self.output_dir:
             self.output_dir = str(Path(self.dbpath).parent)
         if not self.output_dir:
-            self.output_dir = str(Path(".").absolute())
+            self.output_dir = Path(".").resolve()
         if self.savepath and self.savepath.parent == "":
-            self.savepath = Path(self.output_dir) / self.savepath
+            self.savepath = self.output_dir / self.savepath
         self.module_conf = get_module_conf(self.module_name, module_type="reporter")
         self.confs = self.module_options  # TODO: backward compatibility. Delete later.
         self.output_basename = Path(self.dbpath).name[:-7]
-        if not self.inputfiles and self.dbpath:
+        if not self.df_mode and not self.inputfiles and self.dbpath:
             db = sqlite3.connect(self.dbpath)
             c = db.cursor()
             q = 'select colval from info where colkey="_input_paths"'
             c.execute(q)
             r = c.fetchone()
             if r is not None:
                 self.inputfiles = []
@@ -382,14 +417,18 @@
             levels = [tab]
         if type(levels) is not list:
             return []
         if not levels:
             return []
         return levels
 
+    def run_df(self, df: pl.DataFrame, columns: List[Dict[str, Any]], savepath: str = ""):
+        self.write_data_df(df, columns, savepath)
+        self.end()
+
     async def run(
         self,
         tab="all",
         add_summary=None,
         pagesize=None,
         page=None,
         make_filtered_table=True,
@@ -449,14 +488,75 @@
         except Exception as e:
             await self.close_db()
             import traceback
 
             traceback.print_exc()
             raise e
 
+    def write_preface_df(self, df, columns):
+        pass
+
+    def write_header_df(self, columns):
+        pass
+
+    def write_data_df(
+        self, df, columns, savepath
+    ):
+        import time
+        import copy
+        from ..exceptions import SetupError
+
+        colnos = {columns[i]["name"]: i for i in range(len(columns))}
+        self.write_preface_df(df, savepath)
+        self.write_header_df(columns)
+        #self.extracted_cols[level] = self.get_extracted_header_columns(level)
+        #self.extracted_col_names[level] = [
+        #    col_def.get("col_name") for col_def in self.extracted_cols[level]
+        #]
+        #self.hugo_colno = self.colnos[level].get("base__hugo", None)
+        #datacols = await self.cf.exec_db(self.cf.get_variant_data_cols)
+        #self.total_norows = await self.cf.exec_db(
+        #    self.cf.get_ftable_num_rows, level=level, uid=self.ftable_uid, ftype=level
+        #)  # type: ignore
+        #if datacols is None or self.total_norows is None:
+        #    return
+        #if level == "variant" and self.separatesample:
+        #    self.write_variant_sample_separately = True
+        #else:
+        #    self.write_variant_sample_separately = False
+        row_count = 0
+        #conn_read, conn_write = await self.cf.get_db_conns()
+        #if not conn_read or not conn_write:
+        #    return None
+        #cursor_read = await conn_read.cursor()
+        #await self.cf.get_level_data_iterator(
+        #    level, page=page, pagesize=pagesize, uid=self.ftable_uid, cursor_read=cursor_read, var_added_cols=self.var_added_cols
+        #)
+        ctime = time.time()
+        #self.retrieved_col_names[level] = [d[0] for d in cursor_read.description]
+        #self.extracted_col_nos[level] = [self.retrieved_col_names[level].index(col_name) for col_name in self.extracted_col_names[level]]
+        #self.num_retrieved_cols = len(self.retrieved_col_names[level])
+        #self.colnos_to_display[level] = [self.retrieved_col_names[level].index(c) for c in self.colnames_to_display[level]]
+        #self.extracted_colnos_in_retrieved = [self.retrieved_col_names[level].index(c) for c in self.extracted_col_names[level]]
+        self.vcf_format = False
+        self.level = "variant"
+        self.extracted_col_names = {"variant": copy.deepcopy(df.columns)}
+        for datarow in df.iter_rows():
+            #self.stringify_all_mapping(level, datarow)
+            self.escape_characters_df(datarow)
+            self.write_row_with_samples_separate_or_not_df(datarow, columns, colnos)
+            row_count += 1
+            if row_count % 10000 == 0:
+                t = time.time()
+                msg = f"Wrote {row_count} rows. {(t - ctime) / row_count}"
+                if self.logger is not None:
+                    self.logger.info(msg)
+                elif self.outer is not None:
+                    self.outer.write(msg)
+
     async def write_data(
         self,
         level: str,
         add_summary=True,
         pagesize=None,
         page=None,
         make_filtered_table=True,
@@ -524,14 +624,20 @@
                     self.outer.write(msg)
             if pagesize and row_count == pagesize:
                 break
         await cursor_read.close()
         await conn_read.close()
         await conn_write.close()
 
+    def write_table_row_df(self, datarow, columns):
+        pass
+
+    def write_row_with_samples_separate_or_not_df(self, datarow, columns, colnos):
+        self.write_table_row_df(datarow, columns)
+
     def write_row_with_samples_separate_or_not(self, datarow):
         if self.legacy_samples_col:
             col_name = "base__samples"
         else:
             col_name = "tagsampler__samples"
         if self.write_variant_sample_separately:
             samples = datarow[col_name]
@@ -542,14 +648,19 @@
                     sample_datarow[col_name] = sample
                     self.write_table_row(self.get_extracted_row(sample_datarow))
             else:
                 self.write_table_row(self.get_extracted_row(datarow))
         else:
             self.write_table_row(self.get_extracted_row(datarow))
 
+    def escape_characters_df(self, datarow):
+        for i, v in enumerate(datarow):
+            if isinstance(v, str) and "\n" in v:
+                datarow[i] = v.replace("\n", "%0A")
+
     def escape_characters(self, datarow):
         if self.dictrow:
             for k, v in datarow.items():
                 if isinstance(v, str) and "\n" in v:
                     datarow[k] = v.replace("\n", "%0A")
         else:
             for col_no in range(self.num_retrieved_cols):
@@ -832,16 +943,17 @@
         self, add_summary=True, conn=Any, cursor=Any
     ):
         from os.path import dirname
         import sys
         from ..exceptions import ModuleLoadingError
         from ..module.local import get_local_module_infos_of_type
         from ..module.local import get_local_module_info
-        from ..util.util import load_class
         from ..util.inout import ColumnDefinition
+        from ..util.module import get_annotator_class
+        from ..util.module import get_mapper_class
 
         _ = conn
         if not add_summary:
             return
         q = "select name from variant_annotator"
         await cursor.execute(q)
         done_var_annotators = [v[0] for v in await cursor.fetchall()]
@@ -866,35 +978,40 @@
                         f"Skipping gene level summarization with {module_name} "
                         + "as it does not exist in the system."
                     )
                 continue
             module = local_modules[module_name]
             if "can_summarize_by_gene" in module.conf:
                 summarizer_module_names.append(module_name)
-        local_modules[self.mapper_name] = get_local_module_info(self.mapper_name)
+        mapper = get_local_module_info(self.mapper_name)
+        if not mapper:
+            raise ModuleLoadingError(module_name=self.mapper_name)
+        local_modules[self.mapper_name] = mapper
         summarizer_module_names = [self.mapper_name] + summarizer_module_names
         for module_name in summarizer_module_names:
             if not module_name:
                 continue
             mi = local_modules[module_name]
             if not mi:
                 continue
             sys.path = sys.path + [dirname(mi.script_path)]
             annot_cls = None
-            if mi.name in done_var_annotators or mi.name == self.mapper_name:
-                annot_cls = load_class(mi.script_path)
-            if not annot_cls:
-                raise ModuleLoadingError(module_name=mi.name)
+            if mi.name in done_var_annotators:
+                annot_cls = get_annotator_class(module_name)
+            elif mi.name == self.mapper_name:
+                annot_cls = get_mapper_class(module_name)
+            else:
+                continue
             cmd = {
                 "script_path": mi.script_path,
                 "input_file": "__dummy__",
                 "output_dir": self.output_dir,
                 "serveradmindb": self.serveradmindb,
             }
-            annot = annot_cls(cmd)
+            annot = annot_cls(**cmd)
             cols = mi.conf["gene_summary_output_columns"]
             columngroup = {
                 "name": mi.name,
                 "displayname": mi.title,
                 "count": len(cols),
             }
             level = "gene"
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/runner.py` & `oakvar-2.9.8/oakvar/lib/base/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 from typing import Tuple
 from typing import Dict
 
 
 class Runner(object):
     def __init__(self, **kwargs):
-        from pathlib import Path
+        from types import SimpleNamespace
         from ..module.local import LocalModule
 
         self.runlevels = {
             "converter": 1,
             "preparer": 2,
             "mapper": 3,
             "annotator": 4,
@@ -33,21 +33,21 @@
         self.error_logger = None
         self.log_handler = None
         self.error_log_handler = None
         self.start_time = None
         self.manager = None
         self.result_path = None
         self.package_conf = {}
-        self.args = None
+        self.args = SimpleNamespace()
         self.main_conf = {}
         self.run_conf = {}
         self.conf_path = None
         self.conf = {}
         self.first_non_url_input = None
-        self.inputs: Optional[List[Path]] = None
+        self.input_paths: List[str] = []
         self.run_name: Optional[List[str]] = None
         self.output_dir: Optional[List[str]] = None
         self.startlevel = self.runlevels["converter"]
         self.endlevel = self.runlevels["postaggregator"]
         self.cleandb = False
         self.excludes = []
         self.preparer_names = []
@@ -145,24 +145,22 @@
             if self.logger:
                 self.logger.info(msg)
             remove(fn)
 
     def download_url_input(self, ip):
         import requests
         from pathlib import Path
-        from ..util.util import is_url, humanize_bytes
+        from ..util.util import humanize_bytes
         from ..util.run import update_status
 
-        if not self.inputs:
+        if not self.input_paths:
             raise
         if " " in ip:
             print(f"Space is not allowed in input file paths ({ip})")
             exit()
-        if not is_url(ip):
-            return
         update_status(
             f"Fetching {ip}... ",
             logger=self.logger,
             serveradmindb=self.serveradmindb,
         )
         try:
             r = requests.head(ip)
@@ -185,15 +183,15 @@
                         f"[{cur_prog}{rem_prog}] {humanize_bytes(cur_size)} "
                         + f"/ {humanize_bytes(total_size)} ({perc * 100.0:.0f}%)",
                         end="\r",
                         flush=True,
                     )
                     if cur_size == total_size:
                         print("\n")
-            return str(Path(fpath).absolute())
+            return str(Path(fpath).resolve())
         except Exception:
             print("File downloading unsuccessful. Exiting.")
             exit()
 
     def get_logger(self, run_no: int):
         import logging
         from pathlib import Path
@@ -243,22 +241,26 @@
         msg = f"deleting previous output files for {self.run_name[run_no]}..."
         if self.logger:
             self.logger.info(msg)
         self.delete_output_files(run_no)
 
     def log_input(self, run_no: int):
 
-        if not self.inputs or not self.args:
+        if not self.input_paths or not self.args:
             raise
         if self.logger:
             if self.args.combine_input:
-                for input_file in self.inputs:
+                for input_file in self.input_paths:
                     self.logger.info(f"input file: {input_file}")
             else:
-                self.logger.info(f"input file: {self.inputs[run_no]}")
+                if self.args.combine_input:
+                    for input_file in self.input_paths:
+                        self.logger.info(f"input file: {input_file}")
+                else:
+                    self.logger.info(f"input file: {self.input_paths[run_no]}")
 
     def start_log(self, run_no: int):
         from time import asctime, localtime
         from sys import argv
 
         self.get_logger(run_no)
         if not self.logger:
@@ -356,15 +358,15 @@
         self.set_annotators()
         self.set_postaggregators()
         self.add_required_modules_for_postaggregators()
         self.sort_annotators()
         self.sort_postaggregators()
         self.set_reporters()
         self.set_start_end_levels()
-        self.set_self_inputs()  # self.inputs is list.
+        self.set_self_inputs()  # self.input_paths is list.
         self.set_and_create_output_dir()  # self.output_dir is list.
         self.set_run_name()  # self.run_name is list.
         self.set_job_name()  # self.job_name is list.
         self.set_append_mode()  # self.append_mode is list.
         self.set_genome_assemblies()  # self.genome_assemblies is list.
 
     def make_self_args_considering_package_conf(self, args):
@@ -469,54 +471,56 @@
                 [module_name, key] = k.split(".")
                 if module_name not in self.run_conf:
                     self.run_conf[module_name] = {}
                 v = toks[1]
                 self.run_conf[module_name][key] = v
 
     def remove_absent_inputs(self):
-        if not self.inputs:
+        from pathlib import Path
+
+        if not self.input_paths:
             return
-        inputs_to_remove = [v for v in self.inputs if not v.exists() and not "*" in str(v)]
+        inputs_to_remove = [v for v in self.input_paths if not Path(v).exists() and v != "-"]
         for v in inputs_to_remove:
-            self.inputs.remove(v)
+            self.input_paths.remove(v)
 
     def process_url_and_pipe_inputs(self):
         from pathlib import Path
         from ..util.util import is_url
 
         if not self.args:
             raise
         self.first_non_url_input = None
         if self.args.inputs is not None:
-            self.inputs = [
-                Path(x).resolve() if not is_url(x) and x != "-" else x
+            self.input_paths = [
+                str(Path(x).resolve()) if not is_url(x) else x
                 for x in self.args.inputs
             ]
-            if self.inputs is None:
+            if self.input_paths is None:
                 raise
-            for input_no in range(len(self.inputs)):
-                inp = self.inputs[input_no]
-                if is_url(str(inp)):
+            for input_no in range(len(self.input_paths)):
+                inp = self.input_paths[input_no]
+                if is_url(inp):
                     fpath = self.download_url_input(inp)
-                    self.inputs[input_no] = fpath
+                    self.input_paths[input_no] = fpath
                 elif not self.first_non_url_input:
                     self.first_non_url_input = inp
         else:
-            self.inputs = []
+            self.input_paths = []
 
     def regenerate_from_db(self, run_no: int):
         import sqlite3
         from ..util.inout import FileWriter
         from ..util.util import get_crv_def
         from ..util.util import get_crx_def
         from ..util.util import get_crg_def
 
-        if not self.inputs:
+        if not self.input_paths:
             raise
-        dbpath = self.inputs[run_no]
+        dbpath = self.input_paths[run_no]
         db = sqlite3.connect(dbpath)
         c = db.cursor()
         crv_def = get_crv_def()
         crx_def = get_crx_def()
         crg_def = get_crg_def()
         # Variant
         if not self.crv_present:
@@ -562,76 +566,88 @@
         c.close()
         db.close()
 
     def set_append_mode(self):
         import shutil
         from pathlib import Path
 
-        if not self.inputs:
+        if not self.input_paths:
             raise
         if not self.run_name or not self.output_dir or not self.args:
             raise
         self.append_mode = [False] * len(self.run_name)
         for run_no in range(len(self.run_name)):
-            inp = self.inputs[run_no]
+            inp = self.input_paths[run_no]
             run_name = self.run_name[run_no]
             output_dir = self.output_dir[run_no]
-            if not inp.suffix == ".sqlite":
+            if not Path(inp).suffix == ".sqlite":
                 continue
             self.append_mode[run_no] = True
             if run_name.endswith(".sqlite"):
                 self.run_name[run_no] = run_name[:-7]
             if "converter" not in self.args.skip:
                 self.args.skip.append("converter")
             if "mapper" not in self.args.skip:
                 self.args.skip.append("mapper")
             target_name = run_name + ".sqlite"
             target_path = Path(output_dir) / target_name
             shutil.copyfile(inp, target_path)
-            self.inputs[run_no] = target_path
+            self.input_paths[run_no] = str(target_path)
 
     def set_genome_assemblies(self):
         if self.run_name:
             self.genome_assemblies = [[] for _ in range(len(self.run_name))]
         else:
             self.genome_assemblies = []
 
     def set_and_create_output_dir(self):
         from pathlib import Path
         from os import getcwd
         from os import mkdir
         from ..exceptions import ArgumentError
 
-        if not self.args or not self.inputs:
+        if not self.args or not self.input_paths:
             raise
         cwd = getcwd()
         if not self.args.output_dir:
             if self.args.combine_input:
                 self.output_dir = [cwd]
             else:
-                self.output_dir = [
-                    str(Path(inp).absolute().parent) for inp in self.inputs
-                ]
+                if self.args.combine_input:
+                    self.output_dir = [cwd]
+                else:
+                    self.output_dir = [
+                        str(Path(inp).resolve().parent) for inp in self.input_paths
+                    ]
         else:
             if self.args.combine_input:
                 if len(self.args.output_dir) != 1:
                     raise ArgumentError(
                         msg="-d should have one value when --combine-input is used."
                     )
                 self.output_dir = [
                     str(Path(v).absolute()) for v in self.args.output_dir
                 ]
             else:
-                if len(self.args.output_dir) != len(self.inputs):
-                    raise ArgumentError(
-                        msg="-d should have the same number of values as inputs."
-                    )
-                self.output_dir = [
-                    str(Path(v).absolute()) for v in self.args.output_dir
-                ]
+                if self.args.combine_input:
+                    if len(self.args.output_dir) != 1:
+                        raise ArgumentError(
+                            msg="-d should have one value when --combine-input is used."
+                        )
+                    self.output_dir = [
+                        str(Path(v).resolve()) for v in self.args.output_dir
+                    ]
+                else:
+                    if len(self.args.output_dir) != len(self.input_paths):
+                        raise ArgumentError(
+                            msg="-d should have the same number of values as inputs."
+                        )
+                    self.output_dir = [
+                        str(Path(v).resolve()) for v in self.args.output_dir
+                    ]
         for output_dir in self.output_dir:
             if not Path(output_dir).exists():
                 mkdir(output_dir)
 
     def set_package_conf(self, args):
         from ..module.cache import get_module_cache
 
@@ -664,49 +680,49 @@
     def set_run_name(self):
         from pathlib import Path
         from ..exceptions import ArgumentError
 
         if not self.args or not self.output_dir:
             raise
         if not self.args.run_name:
-            if self.inputs:
+            if self.input_paths:
                 if self.args.combine_input:
-                    run_name = Path(self.inputs[0]).name
-                    if len(self.inputs) > 1:
+                    run_name = Path(self.input_paths[0]).name
+                    if len(self.input_paths) > 1:
                         run_name = run_name + "_etc"
                         run_name = self.get_unique_run_name(
                             self.output_dir[0], run_name
                         )
                     self.run_name = [run_name]
                 else:
-                    self.run_name = [Path(v).name for v in self.inputs]
+                    self.run_name = [Path(v).name for v in self.input_paths]
         else:
             if self.args.combine_input:
                 if len(self.args.run_name) != 1:
                     raise ArgumentError(
                         msg="-n should have only one value when --combine-input "
                         + "is given."
                     )
                 self.run_name = self.args.run_name
             else:
                 if len(self.args.run_name) == 1:
-                    if self.inputs:
+                    if self.input_paths:
                         if self.output_dir and len(self.output_dir) != len(
                             set(self.output_dir)
                         ):
                             raise ArgumentError(
                                 msg="-n should have a unique value for each "
                                 + "input when -d has duplicate directories."
                             )
-                        self.run_name = self.args.run_name * len(self.inputs)
+                        self.run_name = self.args.run_name * len(self.input_paths)
                     else:
                         raise
                 else:
-                    if self.inputs:
-                        if len(self.inputs) != len(self.args.run_name):
+                    if self.input_paths:
+                        if len(self.input_paths) != len(self.args.run_name):
                             raise ArgumentError(
                                 msg="Just one or the same number of -n option "
                                 + "values as input files should be given."
                             )
                         self.run_name = self.args.run_name
                     else:
                         raise
@@ -727,27 +743,27 @@
             if len(self.args.job_name) != 1:
                 raise ArgumentError(
                     msg="--j should have only one value when --combine-input is given."
                 )
             self.job_name = self.args.job_name
         else:
             if len(self.args.job_name) == 1:
-                if self.inputs:
+                if self.input_paths:
                     if len(self.output_dir) != len(set(self.output_dir)):
                         raise ArgumentError(
                             msg="-j should have a unique value for each input "
                             + "when -d has duplicate directories. Or, give "
                             + "--combine-input to combine input files into one job."
                         )
-                    self.job_name = self.args.job_name * len(self.inputs)
+                    self.job_name = self.args.job_name * len(self.input_paths)
                 else:
                     raise
             else:
-                if self.inputs:
-                    if len(self.inputs) != len(self.args.job_name):
+                if self.input_paths:
+                    if len(self.input_paths) != len(self.args.job_name):
                         raise ArgumentError(
                             msg="Just one or the same number of -j option values "
                             + "as input files should be given."
                         )
                     self.job_name = self.args.job_name
             return
 
@@ -755,15 +771,15 @@
         from ..exceptions import NoInput
 
         if self.args is None:
             raise
         self.use_inputs_from_run_conf()
         self.process_url_and_pipe_inputs()
         self.remove_absent_inputs()
-        if not self.inputs:
+        if not self.input_paths:
             raise NoInput()
 
     def use_inputs_from_run_conf(self):
         if self.args and not self.args.inputs:
             inputs = self.run_conf.get("inputs")
             if inputs:
                 if type(inputs) == list:
@@ -793,15 +809,15 @@
         from pathlib import Path
         from ..consts import STANDARD_INPUT_FILE_SUFFIX
         from ..consts import VARIANT_LEVEL_MAPPED_FILE_SUFFIX
         from ..consts import GENE_LEVEL_MAPPED_FILE_SUFFIX
 
         if not self.run_name or not self.output_dir:
             raise
-        if not self.inputs:
+        if not self.input_paths:
             raise
         if not self.append_mode:
             raise
         run_name = self.run_name[run_no]
         output_dir = self.output_dir[run_no]
         self.crvinput = str(Path(output_dir) / (run_name + STANDARD_INPUT_FILE_SUFFIX))
         self.crxinput = str(
@@ -1292,21 +1308,20 @@
     async def write_info_table_create_data_if_needed(self, run_no: int, cursor):
         from datetime import datetime
         import json
         from ..exceptions import DatabaseError
 
         if self.append_mode[run_no]:
             return
-        if not self.inputs or not self.job_name or not self.args:
+        if not self.input_paths or not self.job_name or not self.args:
             raise
         if self.args.combine_input:
-            inputs = self.inputs
+            inputs = self.input_paths
         else:
-            inputs = [self.inputs[run_no]]
-        inputs = [str(v) for v in inputs]
+            inputs = [self.input_paths[run_no]]
         job_name = self.job_name[run_no]
         genome_assemblies = (
             list(set(self.genome_assemblies[run_no])) if self.genome_assemblies else []
         )
         created = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         await self.write_info_row("created_at", created, cursor)
         await self.write_info_row("inputs", json.dumps(inputs), cursor)
@@ -1487,25 +1502,25 @@
         await db.close()
 
     def write_initial_info_json(self, run_no: int):
         from datetime import datetime
         from pathlib import Path
         from ..util.admin_util import oakvar_version
 
-        if not self.run_name or not self.inputs or not self.args or not self.output_dir:
+        if not self.run_name or not self.input_paths or not self.args or not self.output_dir:
             raise
         run_name = self.run_name[run_no]
         output_dir = self.output_dir[run_no]
         self.info_json = {}
         self.info_json["job_dir"] = self.output_dir
         self.info_json["job_name"] = self.args.job_name
         self.info_json["run_name"] = run_name
         self.info_json["db_path"] = str(Path(output_dir) / (run_name + ".sqlite"))
-        self.info_json["orig_input_fname"] = [Path(x).name for x in self.inputs]
-        self.info_json["orig_input_path"] = [str(v) for v in self.inputs]
+        self.info_json["orig_input_fname"] = [Path(x).name for x in self.input_paths]
+        self.info_json["orig_input_path"] = self.input_paths
         self.info_json["submission_time"] = datetime.now().isoformat()
         self.info_json["viewable"] = False
         self.info_json["note"] = self.args.note
         self.info_json["report_types"] = (
             self.args.report_types if self.args.report_types is not None else []
         )
         self.pkg_ver = oakvar_version()
@@ -1520,63 +1535,59 @@
             for v in list(self.postaggregators.keys())
             if v not in ["tagsampler", "vcfinfo"]
         ]
         postagg_names.sort()
         self.info_json["postaggregators"] = postagg_names
 
     async def run_converter(self, run_no: int):
-        import os
-        from ..util.util import load_class
+        from .master_converter import MasterConverter
         from types import SimpleNamespace
         from ..util.admin_util import get_packagedir
         from ..util.run import announce_module
+        from .master_converter import MasterConverter
 
         if (
             self.conf is None
             or not self.args
-            or not self.inputs
+            or not self.input_paths
             or not self.run_name
             or not self.output_dir
         ):
             raise
         if self.args.combine_input:
-            input_files = self.inputs
+            input_files = self.input_paths
         else:
-            input_files = [self.inputs[run_no]]
-        converter_path = os.path.join(
-            get_packagedir(), "lib", "base", "master_converter.py"
-        )
+            input_files = [self.input_paths[run_no]]
+        converter_path = get_packagedir() / "lib" / "base" / "master_converter.py"
         module = SimpleNamespace(
             title="Converter", name="converter", script_path=converter_path
         )
         announce_module(module, logger=self.logger, serveradmindb=self.serveradmindb)
-        converter_class = load_class(module.script_path, "MasterConverter")
-        if not converter_class:
-            converter_class = load_class(module.script_path, "MasterCravatConverter")
-        converter = converter_class(
+        converter = MasterConverter(
             inputs=input_files,
-            name=self.run_name[run_no],
+            run_name=self.run_name[run_no],
             output_dir=self.output_dir[run_no],
             genome=self.args.genome,
             input_format=self.args.input_format,
             serveradmindb=self.serveradmindb,
             ignore_sample=self.ignore_sample,
-            mp=self.args.mp,
             outer=self.outer,
         )
         ret = converter.run()
         self.total_num_converted_variants = ret.get("total_lnum")
         self.total_num_valid_variants = ret.get("write_lnum")
         self.converter_format = ret.get("input_formats") or []
         genome_assembly: List[str] = ret.get("assemblies") or []
         self.genome_assemblies[run_no] = genome_assembly
 
     async def run_preparers(self, run_no: int):
         from ..util.util import load_class
         from ..consts import MODULE_OPTIONS_KEY
+        from ..exceptions import ModuleLoadingError
+        from .preparer import BasePreparer
 
         if self.conf is None or not self.run_name or not self.output_dir:
             raise
         run_name = self.run_name[run_no]
         output_dir = self.output_dir[run_no]
         for module_name, module in self.preparers.items():
             module_conf = self.run_conf.get(module_name, {})
@@ -1585,15 +1596,17 @@
                 "input_file": self.crvinput,
                 "run_name": run_name,
                 "output_dir": output_dir,
                 MODULE_OPTIONS_KEY: module_conf,
                 "serveradmindb": self.serveradmindb,
             }
             module_cls = load_class(module.script_path, "Preparer")
-            module_ins = module_cls(kwargs)
+            if not issubclass(module_cls, BasePreparer):
+                raise ModuleLoadingError(module_name=module.name)
+            module_ins = module_cls(**kwargs)
             await self.log_time_of_func(module_ins.run, work=module_name)
 
     async def run_mapper(self, run_no: int):
         import multiprocessing as mp
         from ..base.mp_runners import init_worker, mapper_runner
         from ..util.inout import FileReader
 
@@ -1823,18 +1836,20 @@
         )
         return v_aggregator.db_path
 
     async def run_postaggregators(self, run_no: int):
         from time import time
         from ..util.run import announce_module
         from ..exceptions import SetupError
+        from ..exceptions import ModuleLoadingError
         from ..util.util import load_class
         from ..util.run import update_status
         from ..system.consts import default_postaggregator_names
         from ..consts import MODULE_OPTIONS_KEY
+        from ..base.postaggregator import BasePostAggregator
 
         if self.conf is None:
             raise SetupError()
         if not self.run_name or not self.output_dir:
             raise
         run_name = self.run_name[run_no]
         output_dir = self.output_dir[run_no]
@@ -1846,17 +1861,17 @@
                 "run_name": run_name,
                 "output_dir": output_dir,
                 "serveradmindb": self.serveradmindb,
             }
             postagg_conf = self.run_conf.get(module_name, {})
             if postagg_conf:
                 arg_dict[MODULE_OPTIONS_KEY] = postagg_conf
-            post_agg_cls = load_class(module.script_path, "PostAggregator")
-            if not post_agg_cls:
-                post_agg_cls = load_class(module.script_path, "CravatPostAggregator")
+            post_agg_cls = load_class(module.script_path)
+            if not issubclass(post_agg_cls, BasePostAggregator):
+                raise ModuleLoadingError(module_name=module.name)
             post_agg = post_agg_cls(**arg_dict)
             announce_module(module, serveradmindb=self.serveradmindb)
             stime = time()
             post_agg.run()
             rtime = time() - stime
             update_status(
                 f"{module_name} finished in {rtime:.3f}s",
@@ -1864,26 +1879,29 @@
                 serveradmindb=self.serveradmindb,
             )
 
     async def run_vcf2vcf(self, run_no: int):
         from time import time
         from os.path import abspath
         from types import SimpleNamespace
+        import traceback
         from ..util.util import load_class
         from ..util.run import update_status
         from ..base import vcf2vcf
+        from ..exceptions import ModuleLoadingError
+        from ..base.vcf2vcf import VCF2VCF
 
         if (
             self.conf is None
             or not self.args
             or not self.output_dir
             or not self.run_name
         ):
             raise
-        if not self.inputs:
+        if not self.input_paths:
             raise
         response = {}
         module = {
             "name": "vcf2vcf",
             "title": "VCF to VCF",
             "script_path": abspath(vcf2vcf.__file__),
         }
@@ -1892,55 +1910,50 @@
         arg_dict["output_dir"] = self.output_dir[run_no]
         arg_dict["module_name"] = module.name
         arg_dict["conf"] = self.conf
         arg_dict["mapper_name"] = self.mapper_name
         arg_dict["annotator_names"] = self.annotator_names
         arg_dict["run_name"] = self.run_name[run_no]
         Module = load_class(module.script_path, "VCF2VCF")
+        if not issubclass(Module, VCF2VCF):
+            raise ModuleLoadingError(msg="VCF2VCF class could not be loaded.")
         m = Module(**arg_dict)
         stime = time()
-        response_t = m.run()
-        output_fns = None
-        response_type = type(response_t)
-        if response_type == list:
-            output_fns = " ".join(response_t)
-        elif response_type == str:
-            output_fns = response_t
-        if output_fns is not None:
-            update_status(
-                f"report created: {output_fns} ",
-                logger=self.logger,
-                serveradmindb=self.serveradmindb,
-            )
+        try:
+            ran_ok = m.run()
+        except Exception:
+            ran_ok = False
+            traceback.print_exc()
         report_type = "vcf2vcf"
-        response[report_type] = response_t
+        response[report_type] = ran_ok
         rtime = time() - stime
         update_status(
             f"vcf2vcf finished in {rtime:.3f}s",
             logger=self.logger,
             serveradmindb=self.serveradmindb,
         )
         self.report_response = response
 
     async def run_reporter(self, run_no: int):
         from pathlib import Path
         from ..module.local import get_local_module_info
-        from ..util.util import load_class
+        from ..util.module import get_reporter_class
         from ..util.run import update_status
         from ..exceptions import ModuleNotExist
+        from ..exceptions import ModuleLoadingError
         from ..util.run import announce_module
         from ..consts import MODULE_OPTIONS_KEY
         from .reporter import BaseReporter
 
         if (
             not self.run_name
             or self.conf is None
             or not self.args
             or not self.output_dir
-            or not self.inputs
+            or not self.input_paths
         ):
             raise
         run_name = self.run_name[run_no]
         output_dir = Path(self.output_dir[run_no])
         if len(self.reporters) > 0:
             module_names = [v for v in self.reporters.keys()]
             report_types = [v.replace("reporter", "") for v in self.reporters.keys()]
@@ -1955,17 +1968,18 @@
             if module is None:
                 raise ModuleNotExist(module_name)
             arg_dict = {}  # dict(vars(self.args))
             arg_dict["dbpath"] = output_dir / (run_name + ".sqlite")
             arg_dict["savepath"] = output_dir / run_name
             arg_dict["output_dir"] = output_dir
             arg_dict["run_name"] = run_name
-            arg_dict["module_name"] = module_name
             arg_dict[MODULE_OPTIONS_KEY] = self.run_conf.get(module_name, {})
-            Reporter: Type[BaseReporter] = load_class(module.script_path, "Reporter")
+            Reporter: Type[BaseReporter] = get_reporter_class(module_name)
+            if not issubclass(Reporter, BaseReporter):
+                raise ModuleLoadingError(module_name=module.name)
             reporter = Reporter(**arg_dict)
             response_t = await self.log_time_of_func(reporter.run, work=module_name)
             output_fns = None
             response_type = type(response_t)
             if response_type == list:
                 output_fns = " ".join(response_t)
             elif response_type == str:
@@ -1985,15 +1999,15 @@
             and self.startlevel <= self.runlevels[step]
             and (self.args and step not in self.args.skip)
         )
 
     async def do_step_converter(self, run_no: int):
         from ..util.run import update_status
 
-        if not self.inputs or not self.args:
+        if not self.input_paths or not self.args:
             raise
         step = "converter"
         if not self.should_run_step("converter"):
             return
         await self.log_time_of_func(self.run_converter, run_no, work=f"{step} step")
         if self.total_num_converted_variants == 0:
             msg = "No variant found in input"
```

### Comparing `oakvar-2.9.7/oakvar/lib/base/vcf2vcf.py` & `oakvar-2.9.8/oakvar/lib/base/vcf2vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,15 @@
                         error_logger=self.error_logger,
                         e=e,
                     )
                     if hasattr(e, "halt") and getattr(e, "halt"):
                         break
             f.close()
             wf.close()
+        return True
 
     def setup_logger(self):
         import logging
         from oakvar.lib.exceptions import LoggerError
 
         self.logger = logging.getLogger(f"oakvar.{self.module_name}")
         self.error_logger = logging.getLogger("err." + self.module_name)
```

### Comparing `oakvar-2.9.7/oakvar/lib/consts.py` & `oakvar-2.9.8/oakvar/lib/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/exceptions.py` & `oakvar-2.9.8/oakvar/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/module/__init__.py` & `oakvar-2.9.8/oakvar/lib/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/module/cache.py` & `oakvar-2.9.8/oakvar/lib/module/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+from typing import Dict
+from pathlib import Path
 from collections.abc import MutableMapping
 
 
 class LocalModuleCache(MutableMapping):
+    from .local import LocalModule
+
     def __init__(self, *args, **kwargs):
+        from .local import LocalModule
+
         self.version = None
-        self.store = dict()
+        self.store: Dict[str, LocalModule] = dict()
         self.update(dict(*args, **kwargs))  # use the free update to set keys
 
-    def __getitem__(self, key):
-        from pathlib import Path
+    def __getitem__(self, key: str) -> LocalModule:
         from .local import LocalModule
 
         if key not in self.store:
             raise KeyError(key)
         if not isinstance(self.store[key], LocalModule):
-            self.store[key] = LocalModule(Path(self.store[key]))
+            self.store[key] = LocalModule(Path(key))
         return self.store[key]
 
-    def __setitem__(self, key, value):
-        from os.path import isdir
+    def __setitem__(self, key, value: LocalModule):
         from .local import LocalModule
 
-        if not (isinstance(value, LocalModule) or isdir(value)):
+        if not (isinstance(value, LocalModule) or Path(value).is_dir()):
             raise ValueError(value)
         self.store[key] = value
 
     def __delitem__(self, key):
         del self.store[key]
 
     def __iter__(self):
         return iter(self.store)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.store)
 
 
 class ModuleCache(object):
     def __init__(self):
         from ..system import get_modules_dir
 
@@ -47,62 +51,65 @@
         self.update_local()
 
     def get_local(self):
         return self.local
 
     def add_local(self, module_name):
         from .local import get_module_dir
+        from .local import LocalModule
 
         # from .local import get_local_module_info
         mdir = get_module_dir(module_name)
         if not mdir:
             return
         # module = get_local_module_info(module_name)
-        self.local[module_name] = mdir
+        self.local[module_name] = LocalModule(mdir)
         return mdir
 
     def remove_local(self, module_name):
         if module_name in self.local:
             del self.local[module_name]
 
     def update_local(self):
-        import os
         from ..consts import install_tempdir_name
         from ..system import get_modules_dir
         from ..exceptions import SystemMissingException
+        from .local import LocalModule
 
         self.local = LocalModuleCache()
         self._modules_dir = get_modules_dir()
         if self._modules_dir is None:
             raise SystemMissingException(msg="Modules directory is not set")
-        if not (os.path.exists(self._modules_dir)):
+        if not self._modules_dir.exists():
             return None
-        for mg in os.listdir(self._modules_dir):
-            if mg == install_tempdir_name:
+        for mg in self._modules_dir.iterdir():
+            basename = mg.name
+            if basename == install_tempdir_name:
                 continue
-            mg_path = os.path.join(self._modules_dir, mg)
-            basename = os.path.basename(mg_path)
+            mg_path = self._modules_dir / mg
             if (
-                not (os.path.isdir(mg_path))
+                not mg_path.is_dir()
                 or basename.startswith(".")
                 or basename.startswith("_")
             ):
                 continue
-            for module_name in os.listdir(mg_path):
+            for path in mg_path.iterdir():
+                module_name = path.name
                 if module_name == "hgvs":  # deprecate hgvs
                     continue
-                module_dir = os.path.join(mg_path, module_name)
+                module_dir = mg_path / module_name
+                yml_path = module_dir / (module_name + ".yml")
                 if (
-                    module_dir.startswith(".") is False
-                    and os.path.isdir(module_dir)
+                    module_name.startswith(".") is False
+                    and module_dir.is_dir()
                     and not module_name.startswith(".")
                     and not module_name.startswith("_")
-                    and os.path.exists(os.path.join(module_dir, module_name + ".yml"))
+                    and yml_path.exists()
                 ):
-                    self.local[module_name] = module_dir
+                    self.local[path.name] = LocalModule(Path(module_dir))
 
     def get_remote_readme(self, module_name, version=None):
         from .remote import get_readme
 
         if module_name not in self.remote_readme:
             self.remote_readme[module_name] = {}
         if version in self.remote_readme[module_name]:
```

### Comparing `oakvar-2.9.7/oakvar/lib/module/data_cache.py` & `oakvar-2.9.8/oakvar/lib/module/data_cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/module/local.py` & `oakvar-2.9.8/oakvar/lib/module/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class LocalModule(object):
     def __init__(self, dir_path: Path, __module_type__=None, name=None):
         from ..util.util import load_yml_conf
         from ..store import get_developer_dict
 
-        self.directory = Path(dir_path).absolute()
+        self.directory = Path(dir_path).resolve()
         if not name:
             self.name = self.directory.name
         else:
             self.name = name
         self.script_path = self.directory / (self.name + ".py")
         self.script_exists = self.script_path.exists()
         self.conf_path = self.directory / (self.name + ".yml")
@@ -41,15 +41,15 @@
         else:
             self.readme = ""
         self.helphtml_path = self.directory / "help.html"
         self.helphtml_exists = self.helphtml_path.exists()
         self.conf: dict = {}
         if self.conf_exists:
             self.conf = load_yml_conf(self.conf_path)
-        self.type = self.conf.get("type")
+        self.type: str = self.conf.get("type") or ""
         self.code_version: Optional[str] = self.conf.get("code_version")
         if not self.code_version:
             self.code_version = self.conf.get("version")
         self.version = self.code_version
         self.latest_code_version = self.code_version
         self.latest_data_source = self.conf.get("datasource", "")
         self.description = self.conf.get("description")
@@ -127,29 +127,30 @@
             if isinstance(v, Path):
                 v = str(v)
             d[k] = v
         return d
 
 
 def get_local_module_info(
-    module_name: Union[str, Path], fresh=False
+        module_name: Union[str, Path], module_type: str="", fresh=False
 ) -> Optional[LocalModule]:
     from .cache import get_module_cache
 
     if isinstance(module_name, str):
         p = Path(module_name)
     else:
         p = module_name
     if p.exists():
         module_info = LocalModule(p)
     else:
         module_info = None
         mc = get_module_cache(fresh=fresh)
         if fresh:
-            module_path = get_module_dir(str(module_name))
+            module_path = get_module_dir(str(module_name), module_type=module_type)
+            print(f"@ module_path={module_path}")
             if module_path:
                 module_info = LocalModule(module_path)
                 if module_info:
                     mc.get_local()[module_name] = module_info
         else:
             module_info = mc.get_local().get(module_name)
     return module_info
@@ -183,23 +184,26 @@
     return modules
 
 
 def get_local_module_info_by_name(module_name) -> Optional[LocalModule]:
     return get_local_module_info(module_name)
 
 
-def get_local_module_infos_of_type(t, update=False):
+def get_local_module_infos_of_type(module_type: str, update=False) -> Dict[str, LocalModule]:
     from .cache import get_module_cache
+    from .cache import LocalModuleCache
 
-    modules = {}
+    modules: Dict[str, LocalModule] = {}
     if update:
         get_module_cache().update_local()
-    for module_name in get_module_cache().get_local():
-        if get_module_cache().get_local()[module_name].type == t:
-            modules[module_name] = get_module_cache().get_local()[module_name]
+    local_module_cache: LocalModuleCache = get_module_cache().get_local()
+    for module_name in local_module_cache:
+        local_module = local_module_cache[module_name]
+        if local_module.type == module_type:
+            modules[module_name] = local_module
     return modules
 
 
 def get_module_code_version(
     module_name: str, module_dir: Optional[Path] = None
 ) -> Optional[str]:
     module_conf = get_module_conf(module_name, module_dir=module_dir)
@@ -233,14 +237,21 @@
         return None
     module_dir = Path(modules_dir) / (module_type + "s") / module_name
     if not module_dir.exists():
         module_dir.mkdir(parents=True)
     return str(module_dir)
 
 
+def get_module_py(module_name: str, module_type: str = "") -> Optional[Path]:
+    module_dir = get_module_dir(module_name, module_type=module_type)
+    if not module_dir:
+        return None
+    return module_dir / (module_name + ".py")
+
+
 def get_module_dir(module_name: str, module_type: str = "") -> Optional[Path]:
     from ..system import get_modules_dir
 
     if Path(module_name).exists():
         return Path(module_name)
     modules_dir = get_modules_dir()
     assert modules_dir is not None
@@ -538,15 +549,15 @@
         raise ArgumentError(msg=f"argument kind={kind} is wrong.")
     return pack_dir, outdir
 
 
 def pack_module_zip(
     module_name: str,
     kind: str,
-    outdir: Path = Path(".").absolute(),
+    outdir: Path = Path(".").resolve(),
     split: bool = False,
     outer=None,
 ) -> Optional[Path]:
     from zipfile import ZipFile
     from os import walk
     from os import sep
     from pathlib import Path
@@ -632,14 +643,29 @@
             module_name, "data", outdir=outdir, split=split, outer=outer
         )
     else:
         data_zip_path = None
     return {"code": code_zip_path, "data": data_zip_path}
 
 
+def get_module_names_for_module_type(module_type: str) -> List[str]:
+    from ..system import get_modules_dir
+
+    module_names = []
+    modules_dir = get_modules_dir()
+    if not modules_dir:
+        return module_names
+    module_type_dir = modules_dir / (module_type + "s")
+    if not module_type_dir.exists():
+        return module_names
+    for item in module_type_dir.iterdir():
+        if item.is_dir():
+            module_names.append(item.name)
+    return module_names
+
 def load_modules(annotators: list = [], mapper: Optional[str] = None, input_file=None):
     from ... import get_mapper
     from ... import get_annotator
 
     modules = {}
     if mapper:
         modules[mapper] = get_mapper(mapper, input_file=input_file)
```

### Comparing `oakvar-2.9.7/oakvar/lib/module/remote.py` & `oakvar-2.9.8/oakvar/lib/module/remote.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/store/__init__.py` & `oakvar-2.9.8/oakvar/lib/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/store/consts.py` & `oakvar-2.9.8/oakvar/lib/store/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/store/db.py` & `oakvar-2.9.8/oakvar/lib/store/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/store/ov/__init__.py` & `oakvar-2.9.8/oakvar/lib/store/ov/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/store/ov/account/__init__.py` & `oakvar-2.9.8/oakvar/lib/store/ov/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/system/__init__.py` & `oakvar-2.9.8/oakvar/lib/system/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
 
 def get_conf_dirvalue(conf_key, conf=None) -> Optional[Path]:
     from pathlib import Path
 
     d: Optional[str] = get_sys_conf_str_value(conf_key, conf=conf)
     if d:
-        return Path(d).absolute()
+        return Path(d).resolve()
     else:
         return None
 
 
 def get_cache_dir(cache_key, conf=None) -> Optional[Path]:
     d = get_conf_dir(conf=conf)
     if d:
@@ -990,15 +990,15 @@
     job_dir: Optional[str], run_name=None
 ) -> Optional[str]:
     from pathlib import Path
 
     legacy_status_suffix = ".status.json"
     if not job_dir:
         return None
-    job_dir_p = Path(job_dir).absolute()
+    job_dir_p = Path(job_dir).resolve()
     if run_name:
         legacy_status_json_path = job_dir_p / (run_name + legacy_status_suffix)
         return str(legacy_status_json_path)
     legacy_status_json_paths = list(job_dir_p.glob("*" + legacy_status_suffix))
     if not legacy_status_json_paths:
         return None
     return str(legacy_status_json_paths[0])
```

### Comparing `oakvar-2.9.7/oakvar/lib/system/consts.py` & `oakvar-2.9.8/oakvar/lib/system/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/util/admin_util.py` & `oakvar-2.9.8/oakvar/lib/util/admin_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         pkg_version = get_current_package_version()
     return pkg_version
 
 
 def get_packagedir():
     from pathlib import Path
 
-    return Path(__file__).parent.parent.parent.absolute()
+    return Path(__file__).parent.parent.parent.resolve()
 
 
 def get_platform():
     from platform import platform
 
     pl = platform()
     if pl.startswith("Windows"):
```

### Comparing `oakvar-2.9.7/oakvar/lib/util/asyn.py` & `oakvar-2.9.8/oakvar/lib/util/asyn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/util/download.py` & `oakvar-2.9.8/oakvar/lib/util/download.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/util/download_library.py` & `oakvar-2.9.8/oakvar/lib/util/download_library.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/util/inout.py` & `oakvar-2.9.8/oakvar/lib/util/inout.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 class BaseFile(object):
     valid_types = ["string", "int", "float"]
 
     def __init__(self, path):
         from os.path import abspath
 
-        self.path = abspath(path)
+        if path:
+            self.path = abspath(path)
+        else:
+            self.path = path
         self.columns = {}
 
     def _validate_col_type(self, col_type):
         if col_type not in self.valid_types:
             raise Exception(
                 "Invalid column type {} in {}. Choose from {}".format(
                     col_type, self.path, ", ".join(self.valid_types)
@@ -244,23 +247,24 @@
         fmt="csv",
     ):
         super().__init__(path)
         self.csvfmt: bool = False
         if fmt == "csv":
             self.csvfmt = True
         self.csvwriter = None
-        if fmt == "csv":
-            self.wf = open(self.path, mode, newline="", encoding="utf-8")
-            from csv import writer
-
-            self.csvwriter = writer(self.wf)
-            if mode == "w":
-                self.wf.write("#fmt=csv\n")
-        else:
-            self.wf = open(self.path, mode, encoding="utf-8")
+        if self.path:
+            if fmt == "csv":
+                self.wf = open(self.path, mode, newline="", encoding="utf-8")
+                from csv import writer
+
+                self.csvwriter = writer(self.wf)
+                if mode == "w":
+                    self.wf.write("#fmt=csv\n")
+            else:
+                self.wf = open(self.path, mode, encoding="utf-8")
         self.mode: str = mode
         self.ready_to_write = False
         self.ordered_columns = []
         self.name_to_col_index = {}
         self.title_toks = []
         self.include_definition = include_definition
         self.include_titles = include_titles
```

### Comparing `oakvar-2.9.7/oakvar/lib/util/run.py` & `oakvar-2.9.8/oakvar/lib/util/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/oakvar/lib/util/seq.py` & `oakvar-2.9.8/oakvar/lib/util/seq.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Optional
 from typing import Tuple
 from pyliftover import LiftOver
+from ..base.commonmodule import BaseCommonModule
+
 
 complementary_base = {
     "A": "T",
     "T": "A",
     "C": "G",
     "G": "C",
     "-": "-",
@@ -379,15 +381,15 @@
         if get_ref:
             if not wgs_reader:
                 wgs_reader = get_wgs_reader()
                 if not wgs_reader:
                     raise LiftoverFailure(
                         "No wgs_reader was given. Use oakvar.get_wgs_reader to get one."
                     )
-            ref = wgs_reader.get_bases(newchrom, newpos).upper()
+            ref = wgs_reader.get_bases(newchrom, newpos).upper()  # type: ignore
         return [newchrom, newpos, ref, alt]
     reflen = len(ref)
     altlen = len(alt) if alt else 1
     if reflen == 1 and altlen == 1:
         converted = liftover_one_pos(chrom, pos, lifter=lifter)
         if converted is None:
             raise LiftoverFailure("Liftover failure")
@@ -424,32 +426,34 @@
         newpos = min(newpos1, newpos2)
     if not wgs_reader:
         wgs_reader = get_wgs_reader()
         if not wgs_reader:
             raise LiftoverFailure(
                 "No wgs_reader was given. Use oakvar.get_wgs_reader to get one."
             )
-    hg38_ref = wgs_reader.get_bases(newchrom, newpos)
+    hg38_ref = wgs_reader.get_bases(newchrom, newpos)  # type: ignore
     if hg38_ref == reverse_complement(ref):  # strand reversal
         newref = hg38_ref
         newalt = reverse_complement(alt)
     else:  # same strand
         newref = ref
         newalt = alt
     return [newchrom, newpos, newref, newalt]
 
 
-def get_wgs_reader(assembly="hg38"):
+def get_wgs_reader(assembly="hg38") -> BaseCommonModule:
     """get_wgs_reader.
 
     Args:
         assembly:
     """
-    from ... import get_module
+    from .module import get_module_class
 
-    ModuleClass = get_module(assembly + "wgs")
-    if ModuleClass is None:
-        wgs = None
-    else:
-        wgs = ModuleClass()
-        wgs.setup()
+    module_name = assembly + "wgs"
+    ModuleClass = get_module_class(module_name)
+    if not issubclass(ModuleClass, BaseCommonModule):
+        raise ValueError(
+            f"Could not obtain whole genome sequence reader {module_name} for {assembly}. Instead got {ModuleClass}."
+        )
+    wgs = ModuleClass()
+    wgs.setup()
     return wgs
```

### Comparing `oakvar-2.9.7/oakvar/lib/util/util.py` & `oakvar-2.9.8/oakvar/lib/util/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from typing import Any
+from typing import Union
 from typing import List
 from typing import Dict
 from typing import Optional
+from typing import Type
 from pathlib import Path
 from polars import DataFrame
+from ..base.converter import BaseConverter
+from ..base.preparer import BasePreparer
+from ..base.mapper import BaseMapper
+from ..base.annotator import BaseAnnotator
+from ..base.postaggregator import BasePostAggregator
+from ..base.reporter import BaseReporter
+from ..base.vcf2vcf import VCF2VCF
+from ..base.commonmodule import BaseCommonModule
 
 ov_system_output_columns: Optional[Dict[str, List[Dict[str, Any]]]] = None
 
 
 def get_ucsc_bins(start, stop=None):
     """get_ucsc_bins.
 
@@ -43,79 +53,117 @@
     return [
         x
         for first, last in range_per_level(start, stop)
         for x in range(first, last + 1)
     ]
 
 
-def load_class(path, class_name=None):
+def load_class(
+    path: Optional[Path], class_name=None
+) -> Union[
+    Type[BaseConverter],
+    Type[BasePreparer],
+    Type[BaseMapper],
+    Type[BaseAnnotator],
+    Type[BasePostAggregator],
+    Type[BaseReporter],
+    Type[VCF2VCF],
+    Type[BaseCommonModule],
+]:
     """load_class.
 
     Args:
         path:
         class_name:
     """
     from importlib.util import spec_from_file_location, module_from_spec
     from importlib import import_module
+    from importlib import reload
     import sys
     import inspect
-    from pathlib import Path
+    import traceback
     from ..exceptions import ModuleLoadingError
 
-    p = Path(path)
-    path_dir = str(p.parent)
-    sys.path = [path_dir] + sys.path
+    if not path:
+        raise ValueError(f"{path} does not exist.")
+    sys.path = [str(path.parent)] + sys.path
     module = None
-    module_class = None
-    module_name = p.stem
+    module_name = path.stem
+    module_class: Optional[
+        Union[
+            Type[BaseConverter],
+            Type[BasePreparer],
+            Type[BaseMapper],
+            Type[BaseAnnotator],
+            Type[BasePostAggregator],
+            Type[BaseReporter],
+            Type[VCF2VCF],
+            Type[BaseCommonModule],
+        ]
+    ] = None
     try:
         module = import_module(module_name)
+        module = reload(module)
     except Exception:
-        import traceback
-
         traceback.print_exc()
         try:
             if class_name:
                 spec = spec_from_file_location(class_name, path)
                 if spec is not None:
                     module = module_from_spec(spec)
                     loader = spec.loader
                     if loader is not None:
                         loader.exec_module(module)
         except Exception:
-            import traceback
-
             traceback.print_exc()
             raise ModuleLoadingError(module_name=module_name)
     if module:
         if class_name:
             if hasattr(module, class_name):
                 module_class = getattr(module, class_name)
                 if not inspect.isclass(module_class):
-                    module_class = None
+                    raise ValueError(
+                        f"{class_name} not found in {module.name} does not exist."
+                    )
         else:
             for n in dir(module):
                 if n in [
                     "Converter",
+                    "MasterConverter",
                     "Mapper",
                     "Annotator",
                     "PostAggregator",
                     "Reporter",
                     "CommonModule",
                     "CravatConverter",
                     "CravatMapper",
                     "CravatAnnotator",
                     "CravatPostAggregator",
                     "CravatReporter",
                     "CravatCommonModule",
+                    "VCF2VCF",
                 ]:
                     if hasattr(module, n):
                         module_class = getattr(module, n)
                         if not inspect.isclass(module_class):
-                            module_class = None
+                            raise ValueError(f"{module_class} is not a class.")
+    if not module_class:
+        raise ValueError(f"No OakVar class was found at {path}.")
+    if (
+        not issubclass(module_class, BaseConverter)
+        and not issubclass(module_class, BasePreparer)
+        and not issubclass(module_class, BaseMapper)
+        and not issubclass(module_class, BaseAnnotator)
+        and not issubclass(module_class, BasePostAggregator)
+        and not issubclass(module_class, BaseReporter)
+        and not issubclass(module_class, BaseReporter)
+        and not issubclass(module_class, VCF2VCF)
+        and not issubclass(module_class, BaseCommonModule)
+    ):
+        raise ValueError(f"{module_class} is not a proper OakVar class.")
     del sys.path[0]
     return module_class
 
 
 def get_directory_size(start_path):
     """
     Recursively get directory filesize.
@@ -237,24 +285,25 @@
         if job_version_ov < max_version_supported_for_migration:
             compatible = False
         else:
             compatible = True
         return compatible, job_version_ov, ov_version
 
 
-def is_url(s: str) -> bool:
+def is_url(s: Union[str, Path]) -> bool:
     """is_url.
 
     Args:
         s (str): s
 
     Returns:
         bool:
     """
-    if s.startswith("http://") or s.startswith("https://"):
+    ss = str(s)
+    if ss.startswith("http://") or ss.startswith("https://"):
         return True
     else:
         return False
 
 
 def get_current_time_str():
     """get_current_time_str."""
@@ -786,15 +835,15 @@
     partition_ons = {
         "variant": "base__uid",
         "gene": "base__hugo",
         "sample": "base__uid",
         "mapping": "base__uid",
     }
     df = None
-    db_path_to_use = str(Path(db_path).absolute())
+    db_path_to_use = str(Path(db_path).resolve())
     partition_on = partition_ons.get(table_name)
     db_conn = get_result_db_conn(db_path_to_use)
     if not db_conn:
         return None
     if partition_on and table_name:
         c = db_conn.cursor()
         c.execute(f"select {partition_on} from {table_name} limit 1")
```

### Comparing `oakvar-2.9.7/oakvar.egg-info/PKG-INFO` & `oakvar-2.9.8/oakvar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.7
+Version: 2.9.8
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
 Project-URL: Tracker, https://github.com/rkimoakbioinformatics/oakvar/issues
```

### Comparing `oakvar-2.9.7/oakvar.egg-info/SOURCES.txt` & `oakvar-2.9.8/oakvar.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -440,10 +440,11 @@
 oakvar/lib/util/__init__.py
 oakvar/lib/util/admin_util.py
 oakvar/lib/util/asyn.py
 oakvar/lib/util/download.py
 oakvar/lib/util/download_library.py
 oakvar/lib/util/image.py
 oakvar/lib/util/inout.py
+oakvar/lib/util/module.py
 oakvar/lib/util/run.py
 oakvar/lib/util/seq.py
 oakvar/lib/util/util.py
```

### Comparing `oakvar-2.9.7/pyproject.toml` & `oakvar-2.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.7/setup.py` & `oakvar-2.9.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 long_description = (this_directory / "README.rst").read_text()
 oakvar_files = []
 cravat_files = []
 walk_and_add("oakvar", oakvar_files)
 walk_and_add("cravat", cravat_files)
 setup(
     name="oakvar",
-    version="2.9.7",
+    version="2.9.8",
     description="A genomic variant analysis platform",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rkimoakbioinformatics/oakvar",
     author="Ryangguk Kim",
     author_email="rkim@oakbioinformatics.com",
     license="",
```

