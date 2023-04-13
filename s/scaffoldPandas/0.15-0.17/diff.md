# Comparing `tmp/scaffoldpandas-0.15.tar.gz` & `tmp/scaffoldPandas-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "scaffoldPandas-0.17.tar", last modified: Thu Apr 13 03:54:27 2023, max compression
```

## Comparing `scaffoldpandas-0.15.tar` & `scaffoldPandas-0.17.tar`

### file list

```diff
@@ -1,9 +1,4 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/requirements.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/setup.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/scaffoldPandas/__init__.py
--rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/scaffoldPandas/pdscaffold.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/LICENSE
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/pyproject.toml
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 scaffoldpandas-0.15/PKG-INFO
+-rw-r--r--   0        0        0    33041 2023-04-13 03:52:36.301911 scaffoldPandas-0.17/LICENSE
+-rw-r--r--   0        0        0      458 2023-04-13 03:52:36.301911 scaffoldPandas-0.17/pyproject.toml
+-rw-r--r--   0        0        0    13168 2023-04-13 03:50:50.949447 scaffoldPandas-0.17/scaffoldPandas.py
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 scaffoldPandas-0.17/PKG-INFO
```

### Comparing `scaffoldpandas-0.15/scaffoldPandas/pdscaffold.py` & `scaffoldPandas-0.17/scaffoldPandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/python
 
 """A set of functions to make working with Python Pandas a little easier,
 and to collect idioms and patterns that are useful."""
 
+__version__ = "0.17"
+
 import pandas
 import dateutil
 
 ###### Functions ######
 
 # Collect the elements of a series by type - may be used for counting, but
 # also has utility for testing for maximum and minimum values in 
@@ -282,14 +284,19 @@
     po = po + f"Number of nulls: {nulls}\n"
 
     if printout == True:
         print(po)
     
     return info
 
+def main():
+    return True
+
+if __name__ == "__main__":
+    main()
 
 ###### Patterns ######
 
 ## Connect two or more dataframes together that probably overlap, dropping 
 ## whatever is duplicated
 #firstDataFrame = pandas.DataFrame()
 #secondDataFrame = pandas.DataFrame()
```

### Comparing `scaffoldpandas-0.15/LICENSE` & `scaffoldPandas-0.17/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
   The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
@@ -613,62 +613,7 @@
 
   If the disclaimer of warranty and limitation of liability provided
 above cannot be given local legal effect according to their terms,
 reviewing courts shall apply local law that most closely approximates
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

