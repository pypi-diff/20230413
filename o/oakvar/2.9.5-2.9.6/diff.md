# Comparing `tmp/oakvar-2.9.5.tar.gz` & `tmp/oakvar-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakvar-2.9.5.tar", last modified: Thu Apr 13 11:03:23 2023, max compression
+gzip compressed data, was "oakvar-2.9.6.tar", last modified: Thu Apr 13 12:05:12 2023, max compression
```

## Comparing `oakvar-2.9.5.tar` & `oakvar-2.9.6.tar`

### file list

```diff
@@ -1,550 +1,550 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.757938 oakvar-2.9.5/
--rwxrwxrwx   0 root         (0) root         (0)     1725 2023-04-13 08:45:25.000000 oakvar-2.9.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 11:03:23.757535 oakvar-2.9.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3279 2023-04-13 08:45:25.000000 oakvar-2.9.5/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.466946 oakvar-2.9.5/cravat/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.469535 oakvar-2.9.5/cravat/api/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.470889 oakvar-2.9.5/cravat/api/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/module/ls_logic.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.471303 oakvar-2.9.5/cravat/api/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.471714 oakvar-2.9.5/cravat/api/store/account/
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/system.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/test.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/api/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.478281 oakvar-2.9.5/cravat/cli/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/config.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/gui.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/issue.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/license.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.479858 oakvar-2.9.5/cravat/cli/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/module/info_fn.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/module/ls.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/new.py
--rwxrwxrwx   0 root         (0) root         (0)      110 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/report.py
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.480251 oakvar-2.9.5/cravat/cli/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.480637 oakvar-2.9.5/cravat/cli/store/account/
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/system.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/test.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cli/update.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/util.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/cli/version.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/constants.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/cravat_report.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.485886 oakvar-2.9.5/cravat/gui/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/job_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/multiuser.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/server.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/serveradmindb.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/store_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/system_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/system_message_db.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/system_worker.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/userjob.py
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/util.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/web_submit.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.487065 oakvar-2.9.5/cravat/gui/webresult/
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/webresult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/webresult/jsonreporter.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-06 05:49:48.000000 oakvar-2.9.5/cravat/gui/webresult/webresult.py
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/gui/websocket_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/inout.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.488237 oakvar-2.9.5/cravat/lib/
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.450048 oakvar-2.9.5/cravat/lib/assets/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.450894 oakvar-2.9.5/cravat/lib/assets/module_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.488657 oakvar-2.9.5/cravat/lib/assets/module_templates/annotator/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/annotator/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.489057 oakvar-2.9.5/cravat/lib/assets/module_templates/converter/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/converter/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.489451 oakvar-2.9.5/cravat/lib/assets/module_templates/mapper/
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/mapper/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.489888 oakvar-2.9.5/cravat/lib/assets/module_templates/postaggregator/
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/postaggregator/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.490286 oakvar-2.9.5/cravat/lib/assets/module_templates/preparer/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/preparer/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.490682 oakvar-2.9.5/cravat/lib/assets/module_templates/reporter/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/assets/module_templates/reporter/template.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.496256 oakvar-2.9.5/cravat/lib/base/
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/aggregator.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/annotator.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/commonmodule.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/converter.py
--rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/master_converter.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/mp_runners.py
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/postaggregator.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/preparer.py
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/report_filter.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/reporter.py
--rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/runner.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/base/vcf2vcf.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.498252 oakvar-2.9.5/cravat/lib/module/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/module/cache.py
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/module/data_cache.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/module/local.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/module/remote.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.499395 oakvar-2.9.5/cravat/lib/store/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/store/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/store/consts.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/store/db.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.499775 oakvar-2.9.5/cravat/lib/store/ov/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/store/ov/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.500157 oakvar-2.9.5/cravat/lib/store/ov/account/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/store/ov/account/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.500916 oakvar-2.9.5/cravat/lib/system/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/system/consts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.504818 oakvar-2.9.5/cravat/lib/util/
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/admin_util.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/asyn.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/download.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/download_library.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/image.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/inout.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/run.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/seq.py
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.5/cravat/lib/util/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.505211 oakvar-2.9.5/oakvar/
--rwxrwxrwx   0 root         (0) root         (0)     4240 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.511103 oakvar-2.9.5/oakvar/api/
--rwxrwxrwx   0 root         (0) root         (0)    17617 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1312 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.512461 oakvar-2.9.5/oakvar/api/module/
--rwxrwxrwx   0 root         (0) root         (0)    15951 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3473 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)     3855 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/module/ls_logic.py
--rwxrwxrwx   0 root         (0) root         (0)     1528 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.512848 oakvar-2.9.5/oakvar/api/store/
--rwxrwxrwx   0 root         (0) root         (0)     5347 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.513310 oakvar-2.9.5/oakvar/api/store/account/
--rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-13 08:45:25.000000 oakvar-2.9.5/oakvar/api/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2578 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/api/system.py
--rwxrwxrwx   0 root         (0) root         (0)    32152 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/api/test.py
--rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/api/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.519937 oakvar-2.9.5/oakvar/cli/
--rwxrwxrwx   0 root         (0) root         (0)     2600 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6019 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3117 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/config.py
--rwxrwxrwx   0 root         (0) root         (0)     9134 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/gui.py
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/issue.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/license.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.521681 oakvar-2.9.5/oakvar/cli/module/
--rwxrwxrwx   0 root         (0) root         (0)    12395 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/module/info_fn.py
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/module/install_defs.py
--rwxrwxrwx   0 root         (0) root         (0)     5960 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/module/ls.py
--rwxrwxrwx   0 root         (0) root         (0)     2576 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/new.py
--rwxrwxrwx   0 root         (0) root         (0)     5567 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/report.py
--rwxrwxrwx   0 root         (0) root         (0)     9069 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.522130 oakvar-2.9.5/oakvar/cli/store/
--rwxrwxrwx   0 root         (0) root         (0)     7517 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/store/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.522569 oakvar-2.9.5/oakvar/cli/store/account/
--rwxrwxrwx   0 root         (0) root         (0)     6020 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/store/account/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4904 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/system.py
--rwxrwxrwx   0 root         (0) root         (0)     1054 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/test.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/update.py
--rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/util.py
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/cli/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.528816 oakvar-2.9.5/oakvar/gui/
--rwxrwxrwx   0 root         (0) root         (0)      940 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/consts.py
--rwxrwxrwx   0 root         (0) root         (0)    25702 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/job_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     9376 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/multiuser.py
--rwxrwxrwx   0 root         (0) root         (0)    15109 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/server.py
--rwxrwxrwx   0 root         (0) root         (0)    22012 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/serveradmindb.py
--rwxrwxrwx   0 root         (0) root         (0)    13000 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/store_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     6706 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/system_handlers.py
--rwxrwxrwx   0 root         (0) root         (0)     2136 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/system_message_db.py
--rwxrwxrwx   0 root         (0) root         (0)     6412 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/system_worker.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/userjob.py
--rwxrwxrwx   0 root         (0) root         (0)     4574 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/util.py
--rwxrwxrwx   0 root         (0) root         (0)    15737 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/web_submit.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.531989 oakvar-2.9.5/oakvar/gui/webresult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.532392 oakvar-2.9.5/oakvar/gui/webresult/css/
--rwxrwxrwx   0 root         (0) root         (0)     2389 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/css/pqselect.min.css
--rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/email.png
--rwxrwxrwx   0 root         (0) root         (0)     1150 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/favicon.ico
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.536873 oakvar-2.9.5/oakvar/gui/webresult/fonts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.599058 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/
--rwxrwxrwx   0 root         (0) root         (0)   138764 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
--rwxrwxrwx   0 root         (0) root         (0)   102868 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
--rwxrwxrwx   0 root         (0) root         (0)   146824 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   108752 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   143208 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
--rwxrwxrwx   0 root         (0) root         (0)   106140 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   151052 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111808 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142920 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
--rwxrwxrwx   0 root         (0) root         (0)   106108 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150628 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111708 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   140724 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
--rwxrwxrwx   0 root         (0) root         (0)   104232 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
--rwxrwxrwx   0 root         (0) root         (0)   149996 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111392 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   144372 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
--rwxrwxrwx   0 root         (0) root         (0)   106876 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   140632 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
--rwxrwxrwx   0 root         (0) root         (0)   104332 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150092 2023-01-21 00:14:14.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   111332 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142552 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
--rwxrwxrwx   0 root         (0) root         (0)   105924 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
--rwxrwxrwx   0 root         (0) root         (0)   150988 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   112184 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   133844 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
--rwxrwxrwx   0 root         (0) root         (0)    98868 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
--rwxrwxrwx   0 root         (0) root         (0)   142932 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
--rwxrwxrwx   0 root         (0) root         (0)   105804 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
--rwxrwxrwx   0 root         (0) root         (0)   151180 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   112048 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   135920 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
--rwxrwxrwx   0 root         (0) root         (0)    99632 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
--rwxrwxrwx   0 root         (0) root         (0)   145480 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
--rwxrwxrwx   0 root         (0) root         (0)   106496 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
--rwxrwxrwx   0 root         (0) root         (0)   245036 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)   227180 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)   324864 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
--rwxrwxrwx   0 root         (0) root         (0)     5303 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/inter.css
--rwxrwxrwx   0 root         (0) root         (0)    26456 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    19508 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    25692 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    18980 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    26312 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    19416 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
--rwxrwxrwx   0 root         (0) root         (0)    33072 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
--rwxrwxrwx   0 root         (0) root         (0)    25740 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.610917 oakvar-2.9.5/oakvar/gui/webresult/images/
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      379 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-down-right-circle.svg
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-down-right.svg
--rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-down.svg
--rwxrwxrwx   0 root         (0) root         (0)      311 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-left.svg
--rwxrwxrwx   0 root         (0) root         (0)      312 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-right.svg
--rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrow-up.svg
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/arrows-move.svg
--rwxrwxrwx   0 root         (0) root         (0)     2140 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/camera.svg
--rwxrwxrwx   0 root         (0) root         (0)      291 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/caret-down.svg
--rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/caret-right.svg
--rwxrwxrwx   0 root         (0) root         (0)     3125 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/close.png
--rwxrwxrwx   0 root         (0) root         (0)     2390 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/close.svg
--rwxrwxrwx   0 root         (0) root         (0)      722 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/download-material-black.png
--rwxrwxrwx   0 root         (0) root         (0)     2066 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/download.svg
--rwxrwxrwx   0 root         (0) root         (0)      485 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/grip-vertical.svg
--rwxrwxrwx   0 root         (0) root         (0)     2219 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/pin.svg
--rwxrwxrwx   0 root         (0) root         (0)     2243 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/plus-circle-dotted.svg
--rwxrwxrwx   0 root         (0) root         (0)      280 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/plus-circle-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)     4645 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/sorry.png
--rwxrwxrwx   0 root         (0) root         (0)    25333 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/spinner.gif
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/x-lg.svg
--rwxrwxrwx   0 root         (0) root         (0)      332 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/images/x.svg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.631881 oakvar-2.9.5/oakvar/gui/webresult/js/
--rwxrwxrwx   0 root         (0) root         (0)   398184 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/Chart.js
--rwxrwxrwx   0 root         (0) root         (0)    26580 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/axios.min.js
--rwxrwxrwx   0 root         (0) root         (0)   137820 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/webresult/js/axios.min.js.map
--rwxrwxrwx   0 root         (0) root         (0)     9278 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/dom-to-image.min.js
--rwxrwxrwx   0 root         (0) root         (0)     5839 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/download.js
--rwxrwxrwx   0 root         (0) root         (0)    12091 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
--rwxrwxrwx   0 root         (0) root         (0)   954164 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/graphics.js
--rwxrwxrwx   0 root         (0) root         (0)    86659 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-3.2.1.min.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.648260 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
--rwxrwxrwx   0 root         (0) root         (0)    12660 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rwxrwxrwx   0 root         (0) root         (0)     1817 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.454518 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.648880 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rwxrwxrwx   0 root         (0) root         (0)   293430 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.653715 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
--rwxrwxrwx   0 root         (0) root         (0)     6992 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6988 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6999 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6299 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)    32588 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
--rwxrwxrwx   0 root         (0) root         (0)    35997 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rwxrwxrwx   0 root         (0) root         (0)   520714 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rwxrwxrwx   0 root         (0) root         (0)    30747 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rwxrwxrwx   0 root         (0) root         (0)   253668 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rwxrwxrwx   0 root         (0) root         (0)    18705 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rwxrwxrwx   0 root         (0) root         (0)    15548 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rwxrwxrwx   0 root         (0) root         (0)    17342 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rwxrwxrwx   0 root         (0) root         (0)    13847 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rwxrwxrwx   0 root         (0) root         (0)     1340 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
--rwxrwxrwx   0 root         (0) root         (0)    13171 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery.tools.min.js
--rwxrwxrwx   0 root         (0) root         (0)     5451 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/jquery.url.js
--rwxrwxrwx   0 root         (0) root         (0)    24103 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/masonry.pkgd.min.js
--rwxrwxrwx   0 root         (0) root         (0)    84772 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/packery.pkgd.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.664960 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/
--rwxrwxrwx   0 root         (0) root         (0)    11583 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)   103213 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.669631 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/
--rwxrwxrwx   0 root         (0) root         (0)      230 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      210 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      771 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
--rwxrwxrwx   0 root         (0) root         (0)     1668 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rwxrwxrwx   0 root         (0) root         (0)      216 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.670506 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rwxrwxrwx   0 root         (0) root         (0)    76985 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.676578 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rwxrwxrwx   0 root         (0) root         (0)      750 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rwxrwxrwx   0 root         (0) root         (0)      769 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rwxrwxrwx   0 root         (0) root         (0)      802 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rwxrwxrwx   0 root         (0) root         (0)      805 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rwxrwxrwx   0 root         (0) root         (0)      636 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rwxrwxrwx   0 root         (0) root         (0)      774 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rwxrwxrwx   0 root         (0) root         (0)      782 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rwxrwxrwx   0 root         (0) root         (0)      822 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rwxrwxrwx   0 root         (0) root         (0)      773 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rwxrwxrwx   0 root         (0) root         (0)      675 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.679889 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
--rwxrwxrwx   0 root         (0) root         (0)     1105 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)      613 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rwxrwxrwx   0 root         (0) root         (0)      541 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rwxrwxrwx   0 root         (0) root         (0)     2973 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rwxrwxrwx   0 root         (0) root         (0)    27759 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rwxrwxrwx   0 root         (0) root         (0)     2383 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rwxrwxrwx   0 root         (0) root         (0)    12577 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rwxrwxrwx   0 root         (0) root         (0)     2408 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rwxrwxrwx   0 root         (0) root         (0)     2026 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rwxrwxrwx   0 root         (0) root         (0)    16145 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rwxrwxrwx   0 root         (0) root         (0)   481365 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rwxrwxrwx   0 root         (0) root         (0)    12757 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
--rwxrwxrwx   0 root         (0) root         (0)   242931 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
--rwxrwxrwx   0 root         (0) root         (0)     1646 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rwxrwxrwx   0 root         (0) root         (0)     1278 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rwxrwxrwx   0 root         (0) root         (0)      555 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.458307 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.680404 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.680833 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.681267 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.681772 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.682208 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.682639 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.683072 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.683500 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.683938 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.684372 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.684809 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.685241 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.685694 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.686131 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.686564 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.688600 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
--rwxrwxrwx   0 root         (0) root         (0)     1042 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rwxrwxrwx   0 root         (0) root         (0)     1164 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)     2677 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
--rwxrwxrwx   0 root         (0) root         (0)     3716 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rwxrwxrwx   0 root         (0) root         (0)     1847 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rwxrwxrwx   0 root         (0) root         (0)    12583 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/pqselect.min.js
--rwxrwxrwx   0 root         (0) root         (0)    92225 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/raphael-min.js
--rwxrwxrwx   0 root         (0) root         (0)   326538 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/js/tailwind.min.js
--rwxrwxrwx   0 root         (0) root         (0)      900 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/webresult/jsonreporter.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.689562 oakvar-2.9.5/oakvar/gui/webresult/nocache/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.690971 oakvar-2.9.5/oakvar/gui/webresult/nocache/css/
--rwxrwxrwx   0 root         (0) root         (0)     1714 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/css/singlevariantpage.css
--rwxrwxrwx   0 root         (0) root         (0)    22655 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/css/style.css
--rwxrwxrwx   0 root         (0) root         (0)     2658 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/css/widget.css
--rwxrwxrwx   0 root         (0) root         (0)    21597 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.696282 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/
--rwxrwxrwx   0 root         (0) root         (0)    24858 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/filter.js
--rwxrwxrwx   0 root         (0) root         (0)    13065 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/infomgr.js
--rwxrwxrwx   0 root         (0) root         (0)    30870 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/main.js
--rwxrwxrwx   0 root         (0) root         (0)   103450 2023-04-13 09:16:13.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/setup.js
--rwxrwxrwx   0 root         (0) root         (0)     4903 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/showvariant.js
--rwxrwxrwx   0 root         (0) root         (0)    35998 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/singlevariantpage.js
--rwxrwxrwx   0 root         (0) root         (0)    28858 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/util.js
--rwxrwxrwx   0 root         (0) root         (0)     1696 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/variables.js
--rwxrwxrwx   0 root         (0) root         (0)    22262 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/js/widgethelper.js
--rwxrwxrwx   0 root         (0) root         (0)     5440 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/nocache/variant.html
--rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/question.png
--rwxrwxrwx   0 root         (0) root         (0)    29682 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/webresult/webresult.py
--rwxrwxrwx   0 root         (0) root         (0)      163 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webresult/webviewer.yml
--rwxrwxrwx   0 root         (0) root         (0)     4075 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/gui/websocket_handlers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.459478 oakvar-2.9.5/oakvar/gui/webstore/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.704317 oakvar-2.9.5/oakvar/gui/webstore/images/
--rwxrwxrwx   0 root         (0) root         (0)      446 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/chat-dots-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      740 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/chat-dots.svg
--rwxrwxrwx   0 root         (0) root         (0)      396 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/chat-left-text-fill.svg
--rwxrwxrwx   0 root         (0) root         (0)      545 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/chat-left-text.svg
--rwxrwxrwx   0 root         (0) root         (0)    22268 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/done.png
--rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/email.png
--rwxrwxrwx   0 root         (0) root         (0)     2226 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/empty.png
--rwxrwxrwx   0 root         (0) root         (0)     1763 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/folder.png
--rwxrwxrwx   0 root         (0) root         (0)    38197 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/genericmodulelogo.png
--rwxrwxrwx   0 root         (0) root         (0)     4766 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/hamburger.png
--rwxrwxrwx   0 root         (0) root         (0)     1194 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/left_arrow.png
--rwxrwxrwx   0 root         (0) root         (0)     3524 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/new.png
--rwxrwxrwx   0 root         (0) root         (0)      474 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/no_logo_module.svg
--rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/question.png
--rwxrwxrwx   0 root         (0) root         (0)     1214 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/right_arrow.png
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/webstore/images/x-lg.svg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.459997 oakvar-2.9.5/oakvar/gui/websubmit/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.709331 oakvar-2.9.5/oakvar/gui/websubmit/images/
--rwxrwxrwx   0 root         (0) root         (0)   372952 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/images/background.png
--rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/images/logo.png
--rwxrwxrwx   0 root         (0) root         (0)    22716 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/images/logo_only.png
--rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/images/logo_transparent.png
--rwxrwxrwx   0 root         (0) root         (0)    22247 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/images/logo_transparent_bw.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.711951 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/
--rwxrwxrwx   0 root         (0) root         (0)      511 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/cravat.hg18.txt
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/cravat.hg19.txt
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/cravat.hg38.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:16.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg18.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg19.txt
--rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg38.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.718848 oakvar-2.9.5/oakvar/gui/websubmit/nocache/
--rwxrwxrwx   0 root         (0) root         (0)      692 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/alerts.js
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/element_constructors.js
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/element_getters.js
--rwxrwxrwx   0 root         (0) root         (0)    55822 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/index.html
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/input.js
--rwxrwxrwx   0 root         (0) root         (0)    14408 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/jobstable.js
--rwxrwxrwx   0 root         (0) root         (0)     8242 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/login.html
--rwxrwxrwx   0 root         (0) root         (0)     3796 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/multiuser.css
--rwxrwxrwx   0 root         (0) root         (0)    16797 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/multiuser.js
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/select_modules.js
--rwxrwxrwx   0 root         (0) root         (0)      228 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/showhide.js
--rwxrwxrwx   0 root         (0) root         (0)     6783 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/submit.js
--rwxrwxrwx   0 root         (0) root         (0)      484 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/util.js
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/websubmit.css
--rwxrwxrwx   0 root         (0) root         (0)    39200 2023-02-22 05:21:01.000000 oakvar-2.9.5/oakvar/gui/websubmit/nocache/websubmit.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.719707 oakvar-2.9.5/oakvar/gui/www/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.723055 oakvar-2.9.5/oakvar/gui/www/assets/
--rwxrwxrwx   0 root         (0) root         (0)   381800 2023-04-13 11:01:29.000000 oakvar-2.9.5/oakvar/gui/www/assets/index.43af1864.js
--rwxrwxrwx   0 root         (0) root         (0)    47521 2023-04-13 11:01:29.000000 oakvar-2.9.5/oakvar/gui/www/assets/index.b35f4d23.css
--rwxrwxrwx   0 root         (0) root         (0)     2074 2023-04-13 11:01:29.000000 oakvar-2.9.5/oakvar/gui/www/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.724598 oakvar-2.9.5/oakvar/lib/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.726460 oakvar-2.9.5/oakvar/lib/assets/
--rwxrwxrwx   0 root         (0) root         (0)     9036 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/exampleinput
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.727312 oakvar-2.9.5/oakvar/lib/assets/license/
--rwxrwxrwx   0 root         (0) root         (0)     1707 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/license/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/license/liftover.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.462151 oakvar-2.9.5/oakvar/lib/assets/module_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.728665 oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/template.md
--rwxrwxrwx   0 root         (0) root         (0)      277 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1195 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.730155 oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.md
--rwxrwxrwx   0 root         (0) root         (0)     2534 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1249 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.731617 oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.md
--rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.733119 oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.md
--rwxrwxrwx   0 root         (0) root         (0)      731 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1335 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.734453 oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/template.md
--rwxrwxrwx   0 root         (0) root         (0)      201 2023-04-13 08:45:26.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1327 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/template.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.735594 oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.md
--rwxrwxrwx   0 root         (0) root         (0)     1742 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.py
--rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.yml
--rwxrwxrwx   0 root         (0) root         (0)      135 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/oakvar.yml
--rwxrwxrwx   0 root         (0) root         (0)     3078 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/output_columns.yml
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/assets/system.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.744213 oakvar-2.9.5/oakvar/lib/base/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21656 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/aggregator.py
--rwxrwxrwx   0 root         (0) root         (0)    34429 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/annotator.py
--rwxrwxrwx   0 root         (0) root         (0)     2714 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/commonmodule.py
--rwxrwxrwx   0 root         (0) root         (0)     3035 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/converter.py
--rwxrwxrwx   0 root         (0) root         (0)    11639 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)    35485 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/master_converter.py
--rwxrwxrwx   0 root         (0) root         (0)     3036 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/mp_runners.py
--rwxrwxrwx   0 root         (0) root         (0)    25139 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/postaggregator.py
--rwxrwxrwx   0 root         (0) root         (0)     7018 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/preparer.py
--rwxrwxrwx   0 root         (0) root         (0)    43032 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/report_filter.py
--rwxrwxrwx   0 root         (0) root         (0)    42098 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/reporter.py
--rwxrwxrwx   0 root         (0) root         (0)    80001 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/runner.py
--rwxrwxrwx   0 root         (0) root         (0)    15164 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/base/vcf2vcf.py
--rwxrwxrwx   0 root         (0) root         (0)     2620 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/consts.py
--rwxrwxrwx   0 root         (0) root         (0)     7397 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.747557 oakvar-2.9.5/oakvar/lib/module/
--rwxrwxrwx   0 root         (0) root         (0)    29864 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3915 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/module/cache.py
--rwxrwxrwx   0 root         (0) root         (0)     3523 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/module/data_cache.py
--rwxrwxrwx   0 root         (0) root         (0)    29962 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/module/local.py
--rwxrwxrwx   0 root         (0) root         (0)    10491 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/module/remote.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.749246 oakvar-2.9.5/oakvar/lib/store/
--rwxrwxrwx   0 root         (0) root         (0)     4330 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/store/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/store/consts.py
--rwxrwxrwx   0 root         (0) root         (0)    25288 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/store/db.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.750128 oakvar-2.9.5/oakvar/lib/store/ov/
--rwxrwxrwx   0 root         (0) root         (0)     8121 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/store/ov/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.750721 oakvar-2.9.5/oakvar/lib/store/ov/account/
--rwxrwxrwx   0 root         (0) root         (0)    19142 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/store/ov/account/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.752186 oakvar-2.9.5/oakvar/lib/system/
--rwxrwxrwx   0 root         (0) root         (0)    34376 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1294 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/system/consts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.756954 oakvar-2.9.5/oakvar/lib/util/
--rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5570 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/admin_util.py
--rwxrwxrwx   0 root         (0) root         (0)      744 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/asyn.py
--rwxrwxrwx   0 root         (0) root         (0)     5042 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/download.py
--rwxrwxrwx   0 root         (0) root         (0)    19071 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/download_library.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/image.py
--rwxrwxrwx   0 root         (0) root         (0)    20663 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/inout.py
--rwxrwxrwx   0 root         (0) root         (0)     4932 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/run.py
--rwxrwxrwx   0 root         (0) root         (0)    11187 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/seq.py
--rwxrwxrwx   0 root         (0) root         (0)    20060 2023-04-13 08:45:27.000000 oakvar-2.9.5/oakvar/lib/util/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 11:03:23.508119 oakvar-2.9.5/oakvar.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    19018 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      275 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-13 11:03:23.000000 oakvar-2.9.5/oakvar.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      625 2023-04-13 08:45:27.000000 oakvar-2.9.5/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 11:03:23.758107 oakvar-2.9.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2398 2023-04-13 11:02:11.000000 oakvar-2.9.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.782457 oakvar-2.9.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1725 2023-04-13 08:45:25.000000 oakvar-2.9.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 12:05:12.782110 oakvar-2.9.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3279 2023-04-13 08:45:25.000000 oakvar-2.9.6/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.470810 oakvar-2.9.6/cravat/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.473951 oakvar-2.9.6/cravat/api/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.475479 oakvar-2.9.6/cravat/api/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/module/ls_logic.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.475999 oakvar-2.9.6/cravat/api/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.476508 oakvar-2.9.6/cravat/api/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/system.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/test.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/api/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.483535 oakvar-2.9.6/cravat/cli/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/config.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/gui.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/issue.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/license.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.485073 oakvar-2.9.6/cravat/cli/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/module/info_fn.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/module/ls.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/new.py
+-rwxrwxrwx   0 root         (0) root         (0)      110 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/report.py
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.485502 oakvar-2.9.6/cravat/cli/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.486586 oakvar-2.9.6/cravat/cli/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/system.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/test.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cli/update.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/util.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/cli/version.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/cravat_report.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.491849 oakvar-2.9.6/cravat/gui/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/job_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/multiuser.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/server.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/serveradmindb.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/store_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/system_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/system_message_db.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/system_worker.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/userjob.py
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/util.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/web_submit.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.493072 oakvar-2.9.6/cravat/gui/webresult/
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/webresult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/webresult/jsonreporter.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-06 05:49:48.000000 oakvar-2.9.6/cravat/gui/webresult/webresult.py
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/gui/websocket_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/inout.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.494351 oakvar-2.9.6/cravat/lib/
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.454462 oakvar-2.9.6/cravat/lib/assets/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.455239 oakvar-2.9.6/cravat/lib/assets/module_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.494763 oakvar-2.9.6/cravat/lib/assets/module_templates/annotator/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/annotator/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.495147 oakvar-2.9.6/cravat/lib/assets/module_templates/converter/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/converter/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.495528 oakvar-2.9.6/cravat/lib/assets/module_templates/mapper/
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/mapper/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.495917 oakvar-2.9.6/cravat/lib/assets/module_templates/postaggregator/
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/postaggregator/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.496327 oakvar-2.9.6/cravat/lib/assets/module_templates/preparer/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/preparer/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.496738 oakvar-2.9.6/cravat/lib/assets/module_templates/reporter/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/assets/module_templates/reporter/template.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.502304 oakvar-2.9.6/cravat/lib/base/
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/aggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/annotator.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/commonmodule.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/converter.py
+-rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/master_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/mp_runners.py
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/postaggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/preparer.py
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/report_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/reporter.py
+-rwxrwxrwx   0 root         (0) root         (0)       37 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/runner.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/base/vcf2vcf.py
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.504180 oakvar-2.9.6/cravat/lib/module/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/module/cache.py
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/module/data_cache.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/module/local.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/module/remote.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.505301 oakvar-2.9.6/cravat/lib/store/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/store/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/store/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/store/db.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.505737 oakvar-2.9.6/cravat/lib/store/ov/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/store/ov/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.506109 oakvar-2.9.6/cravat/lib/store/ov/account/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/store/ov/account/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.506843 oakvar-2.9.6/cravat/lib/system/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/system/consts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.510997 oakvar-2.9.6/cravat/lib/util/
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/admin_util.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/asyn.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/download.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/download_library.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/image.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/inout.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/run.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/seq.py
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-04-13 08:45:25.000000 oakvar-2.9.6/cravat/lib/util/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.511605 oakvar-2.9.6/oakvar/
+-rwxrwxrwx   0 root         (0) root         (0)     4240 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.517044 oakvar-2.9.6/oakvar/api/
+-rwxrwxrwx   0 root         (0) root         (0)    17617 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1312 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.518531 oakvar-2.9.6/oakvar/api/module/
+-rwxrwxrwx   0 root         (0) root         (0)    15951 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/api/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3473 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)     3855 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/module/ls_logic.py
+-rwxrwxrwx   0 root         (0) root         (0)     1528 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.518932 oakvar-2.9.6/oakvar/api/store/
+-rwxrwxrwx   0 root         (0) root         (0)     5347 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.519359 oakvar-2.9.6/oakvar/api/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-13 08:45:25.000000 oakvar-2.9.6/oakvar/api/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2578 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/api/system.py
+-rwxrwxrwx   0 root         (0) root         (0)    32152 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/api/test.py
+-rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/api/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.525638 oakvar-2.9.6/oakvar/cli/
+-rwxrwxrwx   0 root         (0) root         (0)     2600 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6019 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3117 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     9134 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/gui.py
+-rwxrwxrwx   0 root         (0) root         (0)      465 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/issue.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/license.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.527780 oakvar-2.9.6/oakvar/cli/module/
+-rwxrwxrwx   0 root         (0) root         (0)    12395 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/module/info_fn.py
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/module/install_defs.py
+-rwxrwxrwx   0 root         (0) root         (0)     5960 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/module/ls.py
+-rwxrwxrwx   0 root         (0) root         (0)     2576 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/new.py
+-rwxrwxrwx   0 root         (0) root         (0)     5567 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/report.py
+-rwxrwxrwx   0 root         (0) root         (0)     9069 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.528325 oakvar-2.9.6/oakvar/cli/store/
+-rwxrwxrwx   0 root         (0) root         (0)     7517 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/store/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.528904 oakvar-2.9.6/oakvar/cli/store/account/
+-rwxrwxrwx   0 root         (0) root         (0)     6020 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/store/account/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4904 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/system.py
+-rwxrwxrwx   0 root         (0) root         (0)     1054 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/test.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/update.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/util.py
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/cli/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.535874 oakvar-2.9.6/oakvar/gui/
+-rwxrwxrwx   0 root         (0) root         (0)      940 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)    25702 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/job_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9376 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/multiuser.py
+-rwxrwxrwx   0 root         (0) root         (0)    15109 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/gui/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    22012 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/serveradmindb.py
+-rwxrwxrwx   0 root         (0) root         (0)    13000 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/store_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6706 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/system_handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     2136 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/system_message_db.py
+-rwxrwxrwx   0 root         (0) root         (0)     6412 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/system_worker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/gui/userjob.py
+-rwxrwxrwx   0 root         (0) root         (0)     4574 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    15737 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/gui/web_submit.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.539264 oakvar-2.9.6/oakvar/gui/webresult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.539695 oakvar-2.9.6/oakvar/gui/webresult/css/
+-rwxrwxrwx   0 root         (0) root         (0)     2389 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/css/pqselect.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/email.png
+-rwxrwxrwx   0 root         (0) root         (0)     1150 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/favicon.ico
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.546160 oakvar-2.9.6/oakvar/gui/webresult/fonts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.611587 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/
+-rwxrwxrwx   0 root         (0) root         (0)   138764 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
+-rwxrwxrwx   0 root         (0) root         (0)   102868 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   146824 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   108752 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   143208 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106140 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   151052 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111808 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142920 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106108 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150628 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111708 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   140724 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
+-rwxrwxrwx   0 root         (0) root         (0)   104232 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   149996 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111392 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   144372 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106876 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   140632 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
+-rwxrwxrwx   0 root         (0) root         (0)   104332 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150092 2023-01-21 00:14:14.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   111332 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142552 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
+-rwxrwxrwx   0 root         (0) root         (0)   105924 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   150988 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   112184 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   133844 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
+-rwxrwxrwx   0 root         (0) root         (0)    98868 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   142932 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
+-rwxrwxrwx   0 root         (0) root         (0)   105804 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   151180 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   112048 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   135920 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
+-rwxrwxrwx   0 root         (0) root         (0)    99632 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   145480 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
+-rwxrwxrwx   0 root         (0) root         (0)   106496 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   245036 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   227180 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)   324864 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
+-rwxrwxrwx   0 root         (0) root         (0)     5303 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/inter.css
+-rwxrwxrwx   0 root         (0) root         (0)    26456 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    19508 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    25692 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    18980 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    26312 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    19416 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    33072 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rwxrwxrwx   0 root         (0) root         (0)    25740 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.623409 oakvar-2.9.6/oakvar/gui/webresult/images/
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      379 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-down-right-circle.svg
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-down-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-down.svg
+-rwxrwxrwx   0 root         (0) root         (0)      311 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-left.svg
+-rwxrwxrwx   0 root         (0) root         (0)      312 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)      309 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrow-up.svg
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/arrows-move.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2140 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/camera.svg
+-rwxrwxrwx   0 root         (0) root         (0)      291 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/caret-down.svg
+-rwxrwxrwx   0 root         (0) root         (0)      289 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/caret-right.svg
+-rwxrwxrwx   0 root         (0) root         (0)     3125 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/close.png
+-rwxrwxrwx   0 root         (0) root         (0)     2390 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/close.svg
+-rwxrwxrwx   0 root         (0) root         (0)      722 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/download-material-black.png
+-rwxrwxrwx   0 root         (0) root         (0)     2066 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/download.svg
+-rwxrwxrwx   0 root         (0) root         (0)      485 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/grip-vertical.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2219 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/pin.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2243 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/plus-circle-dotted.svg
+-rwxrwxrwx   0 root         (0) root         (0)      280 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/plus-circle-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)     4645 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/sorry.png
+-rwxrwxrwx   0 root         (0) root         (0)    25333 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/spinner.gif
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/x-lg.svg
+-rwxrwxrwx   0 root         (0) root         (0)      332 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/images/x.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.648470 oakvar-2.9.6/oakvar/gui/webresult/js/
+-rwxrwxrwx   0 root         (0) root         (0)   398184 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/Chart.js
+-rwxrwxrwx   0 root         (0) root         (0)    26580 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/axios.min.js
+-rwxrwxrwx   0 root         (0) root         (0)   137820 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/webresult/js/axios.min.js.map
+-rwxrwxrwx   0 root         (0) root         (0)     9278 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/dom-to-image.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     5839 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/download.js
+-rwxrwxrwx   0 root         (0) root         (0)    12091 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
+-rwxrwxrwx   0 root         (0) root         (0)   954164 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/graphics.js
+-rwxrwxrwx   0 root         (0) root         (0)    86659 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-3.2.1.min.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.663143 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
+-rwxrwxrwx   0 root         (0) root         (0)    12660 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1817 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.458593 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.663582 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rwxrwxrwx   0 root         (0) root         (0)   293430 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.669007 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
+-rwxrwxrwx   0 root         (0) root         (0)     6992 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6988 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6999 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6299 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)    32588 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rwxrwxrwx   0 root         (0) root         (0)    35997 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rwxrwxrwx   0 root         (0) root         (0)   520714 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rwxrwxrwx   0 root         (0) root         (0)    30747 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rwxrwxrwx   0 root         (0) root         (0)   253668 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    18705 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rwxrwxrwx   0 root         (0) root         (0)    15548 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    17342 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rwxrwxrwx   0 root         (0) root         (0)    13847 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     1340 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rwxrwxrwx   0 root         (0) root         (0)    13171 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery.tools.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     5451 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/jquery.url.js
+-rwxrwxrwx   0 root         (0) root         (0)    24103 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/masonry.pkgd.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    84772 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/packery.pkgd.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.683419 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/
+-rwxrwxrwx   0 root         (0) root         (0)    11583 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)   103213 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.687759 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/
+-rwxrwxrwx   0 root         (0) root         (0)      230 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      771 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
+-rwxrwxrwx   0 root         (0) root         (0)     1668 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rwxrwxrwx   0 root         (0) root         (0)      216 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.688604 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rwxrwxrwx   0 root         (0) root         (0)    76985 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.694502 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rwxrwxrwx   0 root         (0) root         (0)      750 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rwxrwxrwx   0 root         (0) root         (0)      769 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rwxrwxrwx   0 root         (0) root         (0)      802 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rwxrwxrwx   0 root         (0) root         (0)      805 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rwxrwxrwx   0 root         (0) root         (0)      636 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rwxrwxrwx   0 root         (0) root         (0)      774 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rwxrwxrwx   0 root         (0) root         (0)      782 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rwxrwxrwx   0 root         (0) root         (0)      822 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rwxrwxrwx   0 root         (0) root         (0)      773 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rwxrwxrwx   0 root         (0) root         (0)      675 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.697757 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
+-rwxrwxrwx   0 root         (0) root         (0)     1105 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)      613 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)      541 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rwxrwxrwx   0 root         (0) root         (0)     2973 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)    27759 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    12577 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     2408 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)     2026 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rwxrwxrwx   0 root         (0) root         (0)    16145 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)   481365 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)    12757 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rwxrwxrwx   0 root         (0) root         (0)   242931 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rwxrwxrwx   0 root         (0) root         (0)     1646 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rwxrwxrwx   0 root         (0) root         (0)     1278 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rwxrwxrwx   0 root         (0) root         (0)      555 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.462013 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.698277 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.698758 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.699210 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:15.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.699674 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.700120 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.700574 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.701051 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.701503 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.702061 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.702602 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.703108 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.703617 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.704172 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.704755 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.705242 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.707504 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
+-rwxrwxrwx   0 root         (0) root         (0)     1042 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1164 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2677 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     3716 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rwxrwxrwx   0 root         (0) root         (0)     1847 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    12583 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/pqselect.min.js
+-rwxrwxrwx   0 root         (0) root         (0)    92225 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/raphael-min.js
+-rwxrwxrwx   0 root         (0) root         (0)   326538 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/js/tailwind.min.js
+-rwxrwxrwx   0 root         (0) root         (0)      900 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/webresult/jsonreporter.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.708493 oakvar-2.9.6/oakvar/gui/webresult/nocache/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.710001 oakvar-2.9.6/oakvar/gui/webresult/nocache/css/
+-rwxrwxrwx   0 root         (0) root         (0)     1714 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/css/singlevariantpage.css
+-rwxrwxrwx   0 root         (0) root         (0)    22655 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/css/style.css
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/css/widget.css
+-rwxrwxrwx   0 root         (0) root         (0)    21597 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.715641 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/
+-rwxrwxrwx   0 root         (0) root         (0)    24858 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/filter.js
+-rwxrwxrwx   0 root         (0) root         (0)    13065 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/infomgr.js
+-rwxrwxrwx   0 root         (0) root         (0)    30870 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/main.js
+-rwxrwxrwx   0 root         (0) root         (0)   103450 2023-04-13 11:11:33.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/setup.js
+-rwxrwxrwx   0 root         (0) root         (0)     4903 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/showvariant.js
+-rwxrwxrwx   0 root         (0) root         (0)    35998 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/singlevariantpage.js
+-rwxrwxrwx   0 root         (0) root         (0)    28858 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/util.js
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/variables.js
+-rwxrwxrwx   0 root         (0) root         (0)    22262 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/js/widgethelper.js
+-rwxrwxrwx   0 root         (0) root         (0)     5440 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/nocache/variant.html
+-rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/question.png
+-rwxrwxrwx   0 root         (0) root         (0)    29682 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/webresult/webresult.py
+-rwxrwxrwx   0 root         (0) root         (0)      163 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webresult/webviewer.yml
+-rwxrwxrwx   0 root         (0) root         (0)     4075 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/gui/websocket_handlers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.462775 oakvar-2.9.6/oakvar/gui/webstore/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.723509 oakvar-2.9.6/oakvar/gui/webstore/images/
+-rwxrwxrwx   0 root         (0) root         (0)      446 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/chat-dots-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      740 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/chat-dots.svg
+-rwxrwxrwx   0 root         (0) root         (0)      396 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/chat-left-text-fill.svg
+-rwxrwxrwx   0 root         (0) root         (0)      545 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/chat-left-text.svg
+-rwxrwxrwx   0 root         (0) root         (0)    22268 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/done.png
+-rwxrwxrwx   0 root         (0) root         (0)     4948 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/email.png
+-rwxrwxrwx   0 root         (0) root         (0)     2226 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/empty.png
+-rwxrwxrwx   0 root         (0) root         (0)     1763 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/folder.png
+-rwxrwxrwx   0 root         (0) root         (0)    38197 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/genericmodulelogo.png
+-rwxrwxrwx   0 root         (0) root         (0)     4766 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/hamburger.png
+-rwxrwxrwx   0 root         (0) root         (0)     1194 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/left_arrow.png
+-rwxrwxrwx   0 root         (0) root         (0)     3524 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/new.png
+-rwxrwxrwx   0 root         (0) root         (0)      474 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/no_logo_module.svg
+-rwxrwxrwx   0 root         (0) root         (0)    10263 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/question.png
+-rwxrwxrwx   0 root         (0) root         (0)     1214 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/right_arrow.png
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/webstore/images/x-lg.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.463495 oakvar-2.9.6/oakvar/gui/websubmit/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.728590 oakvar-2.9.6/oakvar/gui/websubmit/images/
+-rwxrwxrwx   0 root         (0) root         (0)   372952 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/images/background.png
+-rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/images/logo.png
+-rwxrwxrwx   0 root         (0) root         (0)    22716 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/images/logo_only.png
+-rwxrwxrwx   0 root         (0) root         (0)    24659 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/images/logo_transparent.png
+-rwxrwxrwx   0 root         (0) root         (0)    22247 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/images/logo_transparent_bw.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.731374 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/
+-rwxrwxrwx   0 root         (0) root         (0)      511 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/cravat.hg18.txt
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/cravat.hg19.txt
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/cravat.hg38.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:16.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg18.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg19.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2023-01-21 00:14:17.000000 oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg38.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.739995 oakvar-2.9.6/oakvar/gui/websubmit/nocache/
+-rwxrwxrwx   0 root         (0) root         (0)      692 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/alerts.js
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/element_constructors.js
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/element_getters.js
+-rwxrwxrwx   0 root         (0) root         (0)    55822 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/index.html
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/input.js
+-rwxrwxrwx   0 root         (0) root         (0)    14408 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/jobstable.js
+-rwxrwxrwx   0 root         (0) root         (0)     8242 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/login.html
+-rwxrwxrwx   0 root         (0) root         (0)     3796 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/multiuser.css
+-rwxrwxrwx   0 root         (0) root         (0)    16797 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/multiuser.js
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/select_modules.js
+-rwxrwxrwx   0 root         (0) root         (0)      228 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/showhide.js
+-rwxrwxrwx   0 root         (0) root         (0)     6783 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/submit.js
+-rwxrwxrwx   0 root         (0) root         (0)      484 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/util.js
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/websubmit.css
+-rwxrwxrwx   0 root         (0) root         (0)    39200 2023-02-22 05:21:01.000000 oakvar-2.9.6/oakvar/gui/websubmit/nocache/websubmit.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.741004 oakvar-2.9.6/oakvar/gui/www/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.742432 oakvar-2.9.6/oakvar/gui/www/assets/
+-rwxrwxrwx   0 root         (0) root         (0)    47521 2023-04-13 12:03:53.000000 oakvar-2.9.6/oakvar/gui/www/assets/index.b35f4d23.css
+-rwxrwxrwx   0 root         (0) root         (0)   381782 2023-04-13 12:03:53.000000 oakvar-2.9.6/oakvar/gui/www/assets/index.ef59c55d.js
+-rwxrwxrwx   0 root         (0) root         (0)     2074 2023-04-13 12:03:53.000000 oakvar-2.9.6/oakvar/gui/www/index.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.747283 oakvar-2.9.6/oakvar/lib/
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.749003 oakvar-2.9.6/oakvar/lib/assets/
+-rwxrwxrwx   0 root         (0) root         (0)     9036 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/exampleinput
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.749930 oakvar-2.9.6/oakvar/lib/assets/license/
+-rwxrwxrwx   0 root         (0) root         (0)     1707 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/license/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/license/liftover.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.465640 oakvar-2.9.6/oakvar/lib/assets/module_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.751146 oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      277 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1195 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.752312 oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     2534 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1249 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.753493 oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.754702 oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      731 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1335 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.755886 oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/template.md
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-04-13 08:45:26.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1327 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/template.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.757492 oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.md
+-rwxrwxrwx   0 root         (0) root         (0)     1742 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.py
+-rwxrwxrwx   0 root         (0) root         (0)     1246 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.yml
+-rwxrwxrwx   0 root         (0) root         (0)      135 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/oakvar.yml
+-rwxrwxrwx   0 root         (0) root         (0)     3078 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/output_columns.yml
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/assets/system.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.766708 oakvar-2.9.6/oakvar/lib/base/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21656 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/base/aggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)    34429 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/annotator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2714 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/base/commonmodule.py
+-rwxrwxrwx   0 root         (0) root         (0)     3035 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/converter.py
+-rwxrwxrwx   0 root         (0) root         (0)    11639 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    35485 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/master_converter.py
+-rwxrwxrwx   0 root         (0) root         (0)     3036 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/mp_runners.py
+-rwxrwxrwx   0 root         (0) root         (0)    25139 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/postaggregator.py
+-rwxrwxrwx   0 root         (0) root         (0)     7018 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/preparer.py
+-rwxrwxrwx   0 root         (0) root         (0)    43032 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/report_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)    42098 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/reporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    80001 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/runner.py
+-rwxrwxrwx   0 root         (0) root         (0)    15164 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/base/vcf2vcf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2620 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)     7397 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.770191 oakvar-2.9.6/oakvar/lib/module/
+-rwxrwxrwx   0 root         (0) root         (0)    29864 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3915 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/module/cache.py
+-rwxrwxrwx   0 root         (0) root         (0)     3523 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/module/data_cache.py
+-rwxrwxrwx   0 root         (0) root         (0)    29962 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/module/local.py
+-rwxrwxrwx   0 root         (0) root         (0)    10491 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/module/remote.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.771799 oakvar-2.9.6/oakvar/lib/store/
+-rwxrwxrwx   0 root         (0) root         (0)     4330 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/store/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/store/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)    25288 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/store/db.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.772790 oakvar-2.9.6/oakvar/lib/store/ov/
+-rwxrwxrwx   0 root         (0) root         (0)     8121 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/store/ov/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.773358 oakvar-2.9.6/oakvar/lib/store/ov/account/
+-rwxrwxrwx   0 root         (0) root         (0)    19142 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/store/ov/account/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.774904 oakvar-2.9.6/oakvar/lib/system/
+-rwxrwxrwx   0 root         (0) root         (0)    34376 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1294 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/system/consts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.781311 oakvar-2.9.6/oakvar/lib/util/
+-rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5570 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/util/admin_util.py
+-rwxrwxrwx   0 root         (0) root         (0)      744 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/util/asyn.py
+-rwxrwxrwx   0 root         (0) root         (0)     5042 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/util/download.py
+-rwxrwxrwx   0 root         (0) root         (0)    19071 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/util/download_library.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/util/image.py
+-rwxrwxrwx   0 root         (0) root         (0)    20663 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/util/inout.py
+-rwxrwxrwx   0 root         (0) root         (0)     4932 2023-04-13 08:45:27.000000 oakvar-2.9.6/oakvar/lib/util/run.py
+-rwxrwxrwx   0 root         (0) root         (0)    11187 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/util/seq.py
+-rwxrwxrwx   0 root         (0) root         (0)    20060 2023-04-13 11:41:53.000000 oakvar-2.9.6/oakvar/lib/util/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-13 12:05:12.514263 oakvar-2.9.6/oakvar.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3852 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    19018 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      275 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-13 12:05:12.000000 oakvar-2.9.6/oakvar.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      625 2023-04-13 08:45:27.000000 oakvar-2.9.6/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-13 12:05:12.782694 oakvar-2.9.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2398 2023-04-13 12:04:34.000000 oakvar-2.9.6/setup.py
```

### Comparing `oakvar-2.9.5/LICENSE` & `oakvar-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/PKG-INFO` & `oakvar-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.5
+Version: 2.9.6
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
 Project-URL: Tracker, https://github.com/rkimoakbioinformatics/oakvar/issues
```

### Comparing `oakvar-2.9.5/README.rst` & `oakvar-2.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/__init__.py` & `oakvar-2.9.6/oakvar/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/__init__.py` & `oakvar-2.9.6/oakvar/api/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/config.py` & `oakvar-2.9.6/oakvar/api/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/module/__init__.py` & `oakvar-2.9.6/oakvar/api/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/module/install_defs.py` & `oakvar-2.9.6/oakvar/api/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/module/ls_logic.py` & `oakvar-2.9.6/oakvar/api/module/ls_logic.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/new.py` & `oakvar-2.9.6/oakvar/api/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/store/__init__.py` & `oakvar-2.9.6/oakvar/api/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/store/account/__init__.py` & `oakvar-2.9.6/oakvar/api/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/system.py` & `oakvar-2.9.6/oakvar/api/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/test.py` & `oakvar-2.9.6/oakvar/api/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/api/util.py` & `oakvar-2.9.6/oakvar/api/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/__init__.py` & `oakvar-2.9.6/oakvar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/__main__.py` & `oakvar-2.9.6/oakvar/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/config.py` & `oakvar-2.9.6/oakvar/cli/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/gui.py` & `oakvar-2.9.6/oakvar/cli/gui.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/module/__init__.py` & `oakvar-2.9.6/oakvar/cli/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/module/info_fn.py` & `oakvar-2.9.6/oakvar/cli/module/info_fn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/module/install_defs.py` & `oakvar-2.9.6/oakvar/cli/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/module/ls.py` & `oakvar-2.9.6/oakvar/cli/module/ls.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/new.py` & `oakvar-2.9.6/oakvar/cli/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/report.py` & `oakvar-2.9.6/oakvar/cli/report.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/run.py` & `oakvar-2.9.6/oakvar/cli/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/store/__init__.py` & `oakvar-2.9.6/oakvar/cli/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/store/account/__init__.py` & `oakvar-2.9.6/oakvar/cli/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/system.py` & `oakvar-2.9.6/oakvar/cli/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/test.py` & `oakvar-2.9.6/oakvar/cli/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/util.py` & `oakvar-2.9.6/oakvar/cli/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/cli/version.py` & `oakvar-2.9.6/oakvar/cli/version.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/consts.py` & `oakvar-2.9.6/oakvar/gui/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/job_handlers.py` & `oakvar-2.9.6/oakvar/gui/job_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/multiuser.py` & `oakvar-2.9.6/oakvar/gui/multiuser.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/server.py` & `oakvar-2.9.6/oakvar/gui/server.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/serveradmindb.py` & `oakvar-2.9.6/oakvar/gui/serveradmindb.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/store_handlers.py` & `oakvar-2.9.6/oakvar/gui/store_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/system_handlers.py` & `oakvar-2.9.6/oakvar/gui/system_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/system_message_db.py` & `oakvar-2.9.6/oakvar/gui/system_message_db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/system_worker.py` & `oakvar-2.9.6/oakvar/gui/system_worker.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/userjob.py` & `oakvar-2.9.6/oakvar/gui/userjob.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/util.py` & `oakvar-2.9.6/oakvar/gui/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/web_submit.py` & `oakvar-2.9.6/oakvar/gui/web_submit.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/css/pqselect.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/email.png` & `oakvar-2.9.6/oakvar/gui/webresult/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/favicon.ico` & `oakvar-2.9.6/oakvar/gui/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/Inter_Web/inter.css` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/Inter_Web/inter.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-light-webfont.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `oakvar-2.9.6/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/arrows-move.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/camera.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/close.png` & `oakvar-2.9.6/oakvar/gui/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/close.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/download-material-black.png` & `oakvar-2.9.6/oakvar/gui/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/download.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/pin.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/plus-circle-dotted.svg` & `oakvar-2.9.6/oakvar/gui/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/sorry.png` & `oakvar-2.9.6/oakvar/gui/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/images/spinner.gif` & `oakvar-2.9.6/oakvar/gui/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/Chart.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/axios.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/axios.min.js.map` & `oakvar-2.9.6/oakvar/gui/webresult/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/dom-to-image.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/download.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/draggabilly.pkgd.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/draggabilly.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/graphics.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-3.2.1.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery.tools.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/jquery.url.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/masonry.pkgd.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/packery.pkgd.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/pqselect.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/raphael-min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/js/tailwind.min.js` & `oakvar-2.9.6/oakvar/gui/webresult/js/tailwind.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/jsonreporter.py` & `oakvar-2.9.6/oakvar/gui/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/css/singlevariantpage.css` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/css/style.css` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/css/widget.css` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/index.html` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/filter.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/infomgr.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/main.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/setup.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/showvariant.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/singlevariantpage.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/util.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/variables.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/js/widgethelper.js` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/nocache/variant.html` & `oakvar-2.9.6/oakvar/gui/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/question.png` & `oakvar-2.9.6/oakvar/gui/webresult/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webresult/webresult.py` & `oakvar-2.9.6/oakvar/gui/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websocket_handlers.py` & `oakvar-2.9.6/oakvar/gui/websocket_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/chat-dots.svg` & `oakvar-2.9.6/oakvar/gui/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/chat-left-text.svg` & `oakvar-2.9.6/oakvar/gui/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/done.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/email.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/empty.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/folder.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/genericmodulelogo.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/hamburger.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/left_arrow.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/new.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/question.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/webstore/images/right_arrow.png` & `oakvar-2.9.6/oakvar/gui/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/images/background.png` & `oakvar-2.9.6/oakvar/gui/websubmit/images/background.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/images/logo.png` & `oakvar-2.9.6/oakvar/gui/websubmit/images/logo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/images/logo_only.png` & `oakvar-2.9.6/oakvar/gui/websubmit/images/logo_only.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/images/logo_transparent.png` & `oakvar-2.9.6/oakvar/gui/websubmit/images/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/images/logo_transparent_bw.png` & `oakvar-2.9.6/oakvar/gui/websubmit/images/logo_transparent_bw.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/input-examples/cravat.hg19.txt` & `oakvar-2.9.6/oakvar/gui/websubmit/input-examples/cravat.hg19.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/input-examples/cravat.hg38.txt` & `oakvar-2.9.6/oakvar/gui/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg18.txt` & `oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg18.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg19.txt` & `oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg19.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/input-examples/vcf.hg38.txt` & `oakvar-2.9.6/oakvar/gui/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/alerts.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/alerts.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/element_getters.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/element_getters.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/index.html` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/input.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/input.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/jobstable.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/jobstable.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/login.html` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/login.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/multiuser.css` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/multiuser.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/multiuser.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/multiuser.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/select_modules.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/select_modules.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/submit.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/submit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/websubmit.css` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/websubmit/nocache/websubmit.js` & `oakvar-2.9.6/oakvar/gui/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/www/assets/index.43af1864.js` & `oakvar-2.9.6/oakvar/gui/www/assets/index.ef59c55d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9773,22 +9773,21 @@
         (s == null || s.type != "webviewerwidget") && r.push(s)
     }
     if (r.length > 0) {
         let i = `The following modules should be installed to run this module:
 `;
         for (const o of r) i += o.name + `
 `;
-        let s = {
+        Z({
             response: {
                 data: {
                     msg: i
                 }
             }
-        };
-        handleError(s);
+        });
         return
     }
     for (const i of e) {
         const s = Xt[i],
             o = s.type;
         if (o == "annotator") Rr(i, s);
         else if (o == "postaggregator") Pr(i, s);
```

### Comparing `oakvar-2.9.5/oakvar/gui/www/assets/index.b35f4d23.css` & `oakvar-2.9.6/oakvar/gui/www/assets/index.b35f4d23.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/gui/www/index.html` & `oakvar-2.9.6/oakvar/gui/www/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <link rel="shortcut icon" type="image/ico" href="data:image/x-icon;base64,AAABAAEAEBAAAAEAIABoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAD+/v///////+bm/v/Z2f7/3t7+/8/P/f/h4f7/4+P+/+vr/v/u7v7/0tL9/9nZ/v/o6P7//v7//////////////f3////////Gxv3/uLj8/8PD/f+xsfz/qan8/8zM/f/Cwv3/y8v9/7u7/f+9vf3/wMD9/+np/v///////v7///7+////////5+f+/9bW/v/9/f///Pz//97e/v/29v//4OD+/+Tk/v/6+v///f3///f3///29v////////////////////////////////////////7+///+/v////////7+///9/f///v7////////////////////////////////////////+/v///f3///39///+/v///////+/v/v/s7P7///////39///9/f///////////////////////////////////v7///7+/////////Pz//8zM/f+Dg/v/Wlr5/7W1/P/8/P////////39///+/v//////////////////////////////////29v+/5aW+/93d/r/r6/8/5CQ+/8/P/j/bGz6/9DQ/f///////v7//////////////v7////////w8P7/q6v8/4GB+v+Vlfv/5OT+//b2///39///29v+/2tr+v9HR/j/i4v7//Hx/v///////v7///z8////////vr79/0pK+P+trfz//////9LS/f+AgPr/WFj5/76+/f//////oKD8/z4++P/Cwv3///////z8///9/f///////+Li/v9kZPn/XV35/39/+v99ffr/tbX8/5GR+/9HR/j/cXH6/4iI+/+Skvv/5eX+///////+/v///v7////////19f//o6P8/2ho+v9MTPn/U1P5/8HB/f/T0/3/dHT6/1dX+f9LS/j/hob7//b2/////////v7///z8////////vr79/05O+f+0tPz/7Oz+/4SE+/9HR/j/d3f6/7Cw/P/x8f7/oKD8/0FB+P/Cwv3///////z8///9/f///////97e/v9eXvn/UVH5/6en/P/9/f//09P9/9zc/v/7+///vLz9/4qK+/+Jifv/4eH+///////+/v////////7+////////8fH//5ub+/9HR/j/WFj5/8jI/f/V1f3/hYX7/319+v+4uPz/9vb//////////////////////////////v7///7+////////4uL+/4CA+v9LS/j/enr6/6mp/P/r6/7///////7+///+/v/////////////////////////////+/v///f3/////////////w8P9/9HR/f////////////39///+/v//////////////////AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==" />
     <title>OakVar</title>
-    <script type="module" crossorigin src="/assets/index.43af1864.js"></script>
+    <script type="module" crossorigin src="/assets/index.ef59c55d.js"></script>
     <link rel="stylesheet" href="/assets/index.b35f4d23.css">
   </head>
   <body>
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div id="root"></div>
```

### Comparing `oakvar-2.9.5/oakvar/lib/assets/exampleinput` & `oakvar-2.9.6/oakvar/lib/assets/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/license/LICENSE` & `oakvar-2.9.6/oakvar/lib/assets/license/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/license/liftover.txt` & `oakvar-2.9.6/oakvar/lib/assets/license/liftover.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/annotator/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/annotator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.py` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/converter/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/converter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.py` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/mapper/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/mapper/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.py` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/postaggregator/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/postaggregator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/preparer/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/preparer/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.md` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.py` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/module_templates/reporter/template.yml` & `oakvar-2.9.6/oakvar/lib/assets/module_templates/reporter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/output_columns.yml` & `oakvar-2.9.6/oakvar/lib/assets/output_columns.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/assets/system.yml` & `oakvar-2.9.6/oakvar/lib/assets/system.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/aggregator.py` & `oakvar-2.9.6/oakvar/lib/base/aggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/annotator.py` & `oakvar-2.9.6/oakvar/lib/base/annotator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/commonmodule.py` & `oakvar-2.9.6/oakvar/lib/base/commonmodule.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/converter.py` & `oakvar-2.9.6/oakvar/lib/base/converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/mapper.py` & `oakvar-2.9.6/oakvar/lib/base/mapper.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/master_converter.py` & `oakvar-2.9.6/oakvar/lib/base/master_converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/mp_runners.py` & `oakvar-2.9.6/oakvar/lib/base/mp_runners.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/postaggregator.py` & `oakvar-2.9.6/oakvar/lib/base/postaggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/preparer.py` & `oakvar-2.9.6/oakvar/lib/base/preparer.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/report_filter.py` & `oakvar-2.9.6/oakvar/lib/base/report_filter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/reporter.py` & `oakvar-2.9.6/oakvar/lib/base/reporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/runner.py` & `oakvar-2.9.6/oakvar/lib/base/runner.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/base/vcf2vcf.py` & `oakvar-2.9.6/oakvar/lib/base/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/consts.py` & `oakvar-2.9.6/oakvar/lib/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/exceptions.py` & `oakvar-2.9.6/oakvar/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/module/__init__.py` & `oakvar-2.9.6/oakvar/lib/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/module/cache.py` & `oakvar-2.9.6/oakvar/lib/module/cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/module/data_cache.py` & `oakvar-2.9.6/oakvar/lib/module/data_cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/module/local.py` & `oakvar-2.9.6/oakvar/lib/module/local.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/module/remote.py` & `oakvar-2.9.6/oakvar/lib/module/remote.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/store/__init__.py` & `oakvar-2.9.6/oakvar/lib/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/store/consts.py` & `oakvar-2.9.6/oakvar/lib/store/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/store/db.py` & `oakvar-2.9.6/oakvar/lib/store/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/store/ov/__init__.py` & `oakvar-2.9.6/oakvar/lib/store/ov/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/store/ov/account/__init__.py` & `oakvar-2.9.6/oakvar/lib/store/ov/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/system/__init__.py` & `oakvar-2.9.6/oakvar/lib/system/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/system/consts.py` & `oakvar-2.9.6/oakvar/lib/system/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/admin_util.py` & `oakvar-2.9.6/oakvar/lib/util/admin_util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/asyn.py` & `oakvar-2.9.6/oakvar/lib/util/asyn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/download.py` & `oakvar-2.9.6/oakvar/lib/util/download.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/download_library.py` & `oakvar-2.9.6/oakvar/lib/util/download_library.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/inout.py` & `oakvar-2.9.6/oakvar/lib/util/inout.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/run.py` & `oakvar-2.9.6/oakvar/lib/util/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/seq.py` & `oakvar-2.9.6/oakvar/lib/util/seq.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar/lib/util/util.py` & `oakvar-2.9.6/oakvar/lib/util/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/oakvar.egg-info/PKG-INFO` & `oakvar-2.9.6/oakvar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.5
+Version: 2.9.6
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
 Project-URL: Tracker, https://github.com/rkimoakbioinformatics/oakvar/issues
```

### Comparing `oakvar-2.9.5/oakvar.egg-info/SOURCES.txt` & `oakvar-2.9.6/oakvar.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -378,16 +378,16 @@
 oakvar/gui/websubmit/nocache/select_modules.js
 oakvar/gui/websubmit/nocache/showhide.js
 oakvar/gui/websubmit/nocache/submit.js
 oakvar/gui/websubmit/nocache/util.js
 oakvar/gui/websubmit/nocache/websubmit.css
 oakvar/gui/websubmit/nocache/websubmit.js
 oakvar/gui/www/index.html
-oakvar/gui/www/assets/index.43af1864.js
 oakvar/gui/www/assets/index.b35f4d23.css
+oakvar/gui/www/assets/index.ef59c55d.js
 oakvar/lib/__init__.py
 oakvar/lib/consts.py
 oakvar/lib/exceptions.py
 oakvar/lib/assets/exampleinput
 oakvar/lib/assets/oakvar.yml
 oakvar/lib/assets/output_columns.yml
 oakvar/lib/assets/system.yml
```

### Comparing `oakvar-2.9.5/pyproject.toml` & `oakvar-2.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.5/setup.py` & `oakvar-2.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 long_description = (this_directory / "README.rst").read_text()
 oakvar_files = []
 cravat_files = []
 walk_and_add("oakvar", oakvar_files)
 walk_and_add("cravat", cravat_files)
 setup(
     name="oakvar",
-    version="2.9.5",
+    version="2.9.6",
     description="A genomic variant analysis platform",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rkimoakbioinformatics/oakvar",
     author="Ryangguk Kim",
     author_email="rkim@oakbioinformatics.com",
     license="",
```

