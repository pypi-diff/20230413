# Comparing `tmp/torf-cli-4.0.4.tar.gz` & `tmp/torf-cli-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torf-cli-4.0.4.tar", last modified: Sat Dec 17 16:21:24 2022, max compression
+gzip compressed data, was "torf-cli-5.0.0.tar", last modified: Thu Apr 13 08:27:34 2023, max compression
```

## Comparing `torf-cli-4.0.4.tar` & `torf-cli-5.0.0.tar`

### file list

```diff
@@ -1,25 +1,41 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2022-12-17 16:21:24.063437 torf-cli-4.0.4/
--rw-------   0 ich       (1000) ich       (1000)    35147 2018-01-11 12:25:16.000000 torf-cli-4.0.4/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     8603 2022-12-17 16:21:24.063437 torf-cli-4.0.4/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     8011 2022-05-03 14:08:27.000000 torf-cli-4.0.4/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2022-12-17 16:21:24.059437 torf-cli-4.0.4/docs/
--rw-------   0 ich       (1000) ich       (1000)    16248 2022-06-02 14:54:17.000000 torf-cli-4.0.4/docs/torf.1
--rw-------   0 ich       (1000) ich       (1000)       38 2022-12-17 16:21:24.063437 torf-cli-4.0.4/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1180 2022-12-17 16:14:42.000000 torf-cli-4.0.4/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2022-12-17 16:21:24.059437 torf-cli-4.0.4/torf_cli.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     8603 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      395 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       37 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       24 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        8 2022-12-17 16:21:24.000000 torf-cli-4.0.4/torf_cli.egg-info/top_level.txt
-drwx------   0 ich       (1000) ich       (1000)        0 2022-12-17 16:21:24.063437 torf-cli-4.0.4/torfcli/
--rw-------   0 ich       (1000) ich       (1000)     1236 2022-03-16 17:49:06.000000 torf-cli-4.0.4/torfcli/__init__.py
--rw-------   0 ich       (1000) ich       (1000)      646 2020-06-21 10:43:26.000000 torf-cli-4.0.4/torfcli/__main__.py
--rw-------   0 ich       (1000) ich       (1000)    14016 2022-12-17 16:14:42.000000 torf-cli-4.0.4/torfcli/_config.py
--rw-------   0 ich       (1000) ich       (1000)     3533 2020-06-21 10:43:26.000000 torf-cli-4.0.4/torfcli/_errors.py
--rw-------   0 ich       (1000) ich       (1000)     9261 2022-12-17 16:14:42.000000 torf-cli-4.0.4/torfcli/_main.py
--rw-------   0 ich       (1000) ich       (1000)     3027 2022-04-30 14:21:11.000000 torf-cli-4.0.4/torfcli/_term.py
--rw-------   0 ich       (1000) ich       (1000)    23553 2022-05-05 13:04:31.000000 torf-cli-4.0.4/torfcli/_ui.py
--rw-------   0 ich       (1000) ich       (1000)    10327 2022-04-27 10:12:31.000000 torf-cli-4.0.4/torfcli/_utils.py
--rw-------   0 ich       (1000) ich       (1000)      707 2022-12-17 16:15:23.000000 torf-cli-4.0.4/torfcli/_vars.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/
+-rw-------   0 ich       (1000) ich       (1000)    35147 2018-01-11 12:25:16.000000 torf-cli-5.0.0/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-13 08:27:34.511725 torf-cli-5.0.0/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     8011 2022-05-03 14:08:27.000000 torf-cli-5.0.0/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.507725 torf-cli-5.0.0/docs/
+-rw-------   0 ich       (1000) ich       (1000)    16248 2023-04-10 10:11:45.000000 torf-cli-5.0.0/docs/torf.1
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-04-13 08:27:34.511725 torf-cli-5.0.0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1180 2022-12-17 16:14:42.000000 torf-cli-5.0.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/tests/
+-rw-------   0 ich       (1000) ich       (1000)      999 2020-06-21 10:43:26.000000 torf-cli-5.0.0/tests/test_basics.py
+-rw-------   0 ich       (1000) ich       (1000)     8204 2020-08-11 10:31:28.000000 torf-cli-5.0.0/tests/test_configfile.py
+-rw-------   0 ich       (1000) ich       (1000)     2165 2020-08-11 10:31:17.000000 torf-cli-5.0.0/tests/test_configformat.py
+-rw-------   0 ich       (1000) ich       (1000)    31261 2022-12-17 16:14:42.000000 torf-cli-5.0.0/tests/test_create.py
+-rw-------   0 ich       (1000) ich       (1000)    19428 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_edit.py
+-rw-------   0 ich       (1000) ich       (1000)     3864 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_errors.py
+-rw-------   0 ich       (1000) ich       (1000)    17888 2022-06-02 14:41:48.000000 torf-cli-5.0.0/tests/test_info.py
+-rw-------   0 ich       (1000) ich       (1000)     4453 2022-06-02 14:48:45.000000 torf-cli-5.0.0/tests/test_json.py
+-rw-------   0 ich       (1000) ich       (1000)     8610 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_metainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     4335 2020-08-11 13:03:24.000000 torf-cli-5.0.0/tests/test_profiles.py
+-rw-------   0 ich       (1000) ich       (1000)     5666 2020-06-21 10:43:26.000000 torf-cli-5.0.0/tests/test_progress.py
+-rw-------   0 ich       (1000) ich       (1000)     8686 2023-04-10 10:22:01.000000 torf-cli-5.0.0/tests/test_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)     2313 2020-08-10 10:16:28.000000 torf-cli-5.0.0/tests/test_stdin.py
+-rw-------   0 ich       (1000) ich       (1000)     1375 2023-04-12 14:07:26.000000 torf-cli-5.0.0/tests/test_utils.py
+-rw-------   0 ich       (1000) ich       (1000)    12745 2022-04-30 14:21:11.000000 torf-cli-5.0.0/tests/test_verify.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/torf_cli.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     8603 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      717 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       37 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       24 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)        8 2023-04-13 08:27:34.000000 torf-cli-5.0.0/torf_cli.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-04-13 08:27:34.511725 torf-cli-5.0.0/torfcli/
+-rw-------   0 ich       (1000) ich       (1000)     1236 2022-03-16 17:49:06.000000 torf-cli-5.0.0/torfcli/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)      646 2020-06-21 10:43:26.000000 torf-cli-5.0.0/torfcli/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)    14028 2023-04-12 13:57:52.000000 torf-cli-5.0.0/torfcli/_config.py
+-rw-------   0 ich       (1000) ich       (1000)     3533 2020-06-21 10:43:26.000000 torf-cli-5.0.0/torfcli/_errors.py
+-rw-------   0 ich       (1000) ich       (1000)     9261 2022-12-17 16:14:42.000000 torf-cli-5.0.0/torfcli/_main.py
+-rw-------   0 ich       (1000) ich       (1000)     3027 2022-04-30 14:21:11.000000 torf-cli-5.0.0/torfcli/_term.py
+-rw-------   0 ich       (1000) ich       (1000)    23553 2022-05-05 13:04:31.000000 torf-cli-5.0.0/torfcli/_ui.py
+-rw-------   0 ich       (1000) ich       (1000)    10424 2023-04-12 14:02:02.000000 torf-cli-5.0.0/torfcli/_utils.py
+-rw-------   0 ich       (1000) ich       (1000)      707 2023-04-13 08:26:36.000000 torf-cli-5.0.0/torfcli/_vars.py
```

### Comparing `torf-cli-4.0.4/LICENSE` & `torf-cli-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/PKG-INFO` & `torf-cli-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-cli
-Version: 4.0.4
+Version: 5.0.0
 Summary: CLI tool to create, read and edit torrent files
 Home-page: https://github.com/rndusr/torf-cli
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet file cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-cli-4.0.4/README.rst` & `torf-cli-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/docs/torf.1` & `torf-cli-5.0.0/docs/torf.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: torf
 .\"    Author: [see the "AUTHOR(S)" section]
-.\" Generator: Asciidoctor 2.0.16
-.\"      Date: 2022-05-03
+.\" Generator: Asciidoctor 2.0.18
+.\"      Date: 2023-04-10
 .\"    Manual: \ \&
 .\"    Source: \ \&
 .\"  Language: English
 .\"
-.TH "TORF" "1" "2022-05-03" "\ \&" "\ \&"
+.TH "TORF" "1" "2023-04-10" "\ \&" "\ \&"
 .ie \n(.g .ds Aq \(aq
 .el       .ds Aq '
 .ss \n[.ss] 0
 .nh
 .ad l
 .de URL
 \fI\\$2\fP <\\$1>\\$3
@@ -37,16 +37,16 @@
 .br
 \fBtorf\fP \fB\-i\fP \fIINPUT\fP [\fIOPTIONS\fP] \fB\-o\fP \fITORRENT\fP
 .br
 \fBtorf\fP \fB\-i\fP \fITORRENT\fP \fIPATH\fP
 .br
 .SH "DESCRIPTION"
 .sp
-torf can create, display and edit torrent files and verify the integrity of a
-torrent\(cqs files.
+torf can create, display and edit torrent files and verify the integrity of the
+files in a torrent.
 .sp
 .RS 4
 .ie n \{\
 \h'-04'\(bu\h'+03'\c
 .\}
 .el \{\
 .  sp -1
@@ -143,15 +143,15 @@
 Copy piece size and piece hashes from existing torrent \fIPATH\fP.  The existing
 torrent must have identical files.  If \fIPATH\fP is a directory, it is searched
 recursively for a matching torrent.  This option may be given multiple times.
 .RE
 .sp
 \fB\-\-noreuse\fP, \fB\-R\fP
 .RS 4
-Ignore all \fB\-\-reuse\fP arguments.  This is particularly useful you have reuse
+Ignore all \fB\-\-reuse\fP arguments.  This is particularly useful if you have reuse
 paths in your configuration file.
 .RE
 .sp
 \fB\-\-exclude\fP, \fB\-e\fP \fIPATTERN\fP
 .RS 4
 Exclude files from \fIPATH\fP that match the glob pattern \fIPATTERN\fP.  This option
 may be given multiple times.  See \fBEXCLUDING FILES\fP.
@@ -606,17 +606,17 @@
 quoted with single or double quotes to preserve leading and/or trailing spaces.
 Lines that start with \(lq#\(rq are ignored.
 .sp
 All of the options listed in the \fBOPTIONS\fP section are allowed except for
 \fIPATH\fP, \fBin\fP, \fBout\fP, \fBname\fP, \fBconfig\fP, \fBnoconfig\fP, \fBprofile\fP, \fBhelp\fP, \fBversion\fP.
 .sp
 There is rudimental support for environment variables in parameters. As usual,
-\(lq$FOO\(rq or \(lq${FOO}\(rq will be replaced with the value of the variable \fBFOO\fP,
-\(lq$\(rq is escaped with \(lq\(rs\(rq (backslash) and a literal \(lq\(rs\(rq is represented by
-two \(lq\(rs\(rq.  More complex string manipulation syntax (e.g. \(lq${FOO:3}\(rq) is not
+\(lq$FOO\(rq or \(lq${FOO}\(rq is replaced with the value of the variable \fBFOO\fP, \(lq$\(rq
+is escaped with \(lq\(rs\(rq (backslash) and a literal \(lq\(rs\(rq is represented by two
+\(lq\(rs\(rq.  More complex string manipulation syntax (e.g. \(lq${FOO:3}\(rq) is not
 supported.
 .SS "Profiles"
 .sp
 A profile is a set of options bound to a name that is given to the \fB\-\-profile\fP
 option.  In the configuration file it is specified as \(lq[\fIPROFILE NAME\fP]\(rq
 followed by a list of options.  Profiles inherit any options specified globally
 at the top of the file, but they can overload them.
```

### Comparing `torf-cli-4.0.4/setup.py` & `torf-cli-5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torf_cli.egg-info/PKG-INFO` & `torf-cli-5.0.0/torf_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torf-cli
-Version: 4.0.4
+Version: 5.0.0
 Summary: CLI tool to create, read and edit torrent files
 Home-page: https://github.com/rndusr/torf-cli
 Author: Random User
 Author-email: rndusr@posteo.de
 License: GPLv3+
 Keywords: bittorrent torrent magnet file cli
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `torf-cli-4.0.4/torfcli/__init__.py` & `torf-cli-5.0.0/torfcli/__init__.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/__main__.py` & `torf-cli-5.0.0/torfcli/__main__.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/_config.py` & `torf-cli-5.0.0/torfcli/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 def get_cfg(cliargs):
     """Combine values from CLI, config file, profiles and defaults"""
     clicfg = parse_args(cliargs)
 
     if clicfg['debug_file']:
         import logging
-        logging.basicConfig(level=logging.DEBUG, format='%(message)s',
+        logging.basicConfig(level=logging.DEBUG, format='%(asctime)s %(message)s',
                             filename=clicfg['debug_file'])
 
     # If we don't need to read a config file, return parsed CLI arguments
     cfgfile = clicfg['config'] or DEFAULT_CONFIG_FILE
     if clicfg['noconfig'] or (not clicfg['config'] and not os.path.exists(cfgfile)):
         return clicfg
```

### Comparing `torf-cli-4.0.4/torfcli/_errors.py` & `torf-cli-5.0.0/torfcli/_errors.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/_main.py` & `torf-cli-5.0.0/torfcli/_main.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/_term.py` & `torf-cli-5.0.0/torfcli/_term.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/_ui.py` & `torf-cli-5.0.0/torfcli/_ui.py`

 * *Files identical despite different names*

### Comparing `torf-cli-4.0.4/torfcli/_utils.py` & `torf-cli-5.0.0/torfcli/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,16 +77,19 @@
 
 def get_torrent_filepath(torrent, cfg):
     """Return the file path of the output torrent file"""
     if cfg['out']:
         # User-given torrent file path
         return cfg['out']
     else:
-        # Default to torrent's name in cwd
-        return torrent.name + '.torrent'
+        filename = torrent.name
+        profiles = cfg.get('profile', ())
+        if profiles:
+            filename += '.' + '.'.join(profiles)
+        return filename + '.torrent'
 
 
 def is_magnet(string):
     return not os.path.exists(string) and string.startswith('magnet:')
 
 
 class Average():
```

### Comparing `torf-cli-4.0.4/torfcli/_vars.py` & `torf-cli-5.0.0/torfcli/_vars.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-__version__     = '4.0.4'
+__version__     = '5.0.0'
 __appname__     = 'torf'
 __url__         = 'https://github.com/rndusr/torf-cli'
 __description__ = 'CLI tool to create, read and edit torrent files'
```

