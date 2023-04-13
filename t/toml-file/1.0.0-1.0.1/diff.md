# Comparing `tmp/toml_file-1.0.0.tar.gz` & `tmp/toml_file-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_file-1.0.0.tar", last modified: Thu Apr 13 10:16:42 2023, max compression
+gzip compressed data, was "toml_file-1.0.1.tar", last modified: Thu Apr 13 15:19:06 2023, max compression
```

## Comparing `toml_file-1.0.0.tar` & `toml_file-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 10:16:42.199332 toml_file-1.0.0/
--rw-rw-rw-   0        0        0     1456 2023-04-13 10:16:42.199332 toml_file-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2023-04-13 10:05:41.000000 toml_file-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 10:16:42.199332 toml_file-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4206 2023-04-13 10:04:37.000000 toml_file-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:16:42.173700 toml_file-1.0.0/toml_file/
--rw-rw-rw-   0        0        0      890 2023-03-20 12:20:34.000000 toml_file-1.0.0/toml_file/__init__.py
--rw-rw-rw-   0        0        0    10087 2023-04-11 11:09:10.000000 toml_file-1.0.0/toml_file/config.py
--rw-rw-rw-   0        0        0     2822 2023-04-13 08:21:31.000000 toml_file-1.0.0/toml_file/encoder.py
--rw-rw-rw-   0        0        0    38783 2023-04-13 06:52:37.000000 toml_file-1.0.0/toml_file/parser.py
--rw-rw-rw-   0        0        0    45907 2023-04-13 08:57:44.000000 toml_file-1.0.0/toml_file/types.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:16:42.199332 toml_file-1.0.0/toml_file.egg-info/
--rw-rw-rw-   0        0        0     1456 2023-04-13 10:16:41.000000 toml_file-1.0.0/toml_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-13 10:16:42.000000 toml_file-1.0.0/toml_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 10:16:41.000000 toml_file-1.0.0/toml_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 10:16:41.000000 toml_file-1.0.0/toml_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.733468 toml_file-1.0.1/
+-rw-rw-rw-   0        0        0     1456 2023-04-13 15:19:06.733468 toml_file-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2023-04-13 10:05:41.000000 toml_file-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:19:06.733468 toml_file-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4206 2023-04-13 15:19:02.000000 toml_file-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.717849 toml_file-1.0.1/toml_file/
+-rw-rw-rw-   0        0        0      890 2023-03-20 12:20:34.000000 toml_file-1.0.1/toml_file/__init__.py
+-rw-rw-rw-   0        0        0    10745 2023-04-13 15:14:12.000000 toml_file-1.0.1/toml_file/config.py
+-rw-rw-rw-   0        0        0     2822 2023-04-13 08:21:31.000000 toml_file-1.0.1/toml_file/encoder.py
+-rw-rw-rw-   0        0        0    39307 2023-04-13 13:02:28.000000 toml_file-1.0.1/toml_file/parser.py
+-rw-rw-rw-   0        0        0    45989 2023-04-13 11:14:37.000000 toml_file-1.0.1/toml_file/types.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:19:06.733468 toml_file-1.0.1/toml_file.egg-info/
+-rw-rw-rw-   0        0        0     1456 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 15:19:06.000000 toml_file-1.0.1/toml_file.egg-info/top_level.txt
```

### Comparing `toml_file-1.0.0/PKG-INFO` & `toml_file-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml_file
-Version: 1.0.0
+Version: 1.0.1
 Summary: TOML file reader - python module to read/write toml configuration files
 Home-page: https://gitlab.com/tcharrett/totoml
 Author: Tom Charrett
 Author-email: tcharrett@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `toml_file-1.0.0/README.md` & `toml_file-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.0/setup.py` & `toml_file-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 # Package meta-data.
 NAME = "toml_file"
 DESCRIPTION = "TOML file reader - python module to read/write toml configuration files"
 URL = "https://gitlab.com/tcharrett/totoml"
 EMAIL = "tcharrett@gmail.com"
 AUTHOR = "Tom Charrett"
 REQUIRES_PYTHON = ">=3.7.6"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {}
```

### Comparing `toml_file-1.0.0/toml_file/__init__.py` & `toml_file-1.0.1/toml_file/__init__.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.0/toml_file/config.py` & `toml_file-1.0.1/toml_file/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,30 +129,51 @@
             - allow multilevel indexing
             - return sub-dicts as Configs
             - return default value if key is templated but not set
             todo:
             - return lists/tuples as ConfigList with template info
         """
         if isinstance(key, str) is False:
-            raise KeyError(f'Config keys much be strings {key}')
+            raise KeyError(f'Config keys much be strings {key}')
             
-        # get dicts for a multilevel key
-        *parents, key = key.split('.')
         table = self.data       # start with data dict
-        ttable = self.template  # start with template dict
-        for part in parents:
-            # get next table
-            table = table[part]
-            
-            # get next template
-            ttable = ttable.get(part, {} )
-
+        ttable = self.template  # start with template dict
+        
+        #---
+        while True:
+            #check if key in the table
+            if key in table:
+                break
+        
+            #Check if first parent is quoted key
+            if key.startswith( ('"',"'")):
+                end = key.find(key[0], 1)
+                parent = key[1:end]
+                key = key[end+2:] #skip next dot!
+                if key=='': #no more parts
+                    key = parent
+                    break
+            
+            #check for dotted part
+            else: 
+                parent, *rest = key.split('.',1)
+                if rest==[]:#no remaining parts get current key
+                    key = parent
+                    break
+                key = rest[0]
+                
+            #get parent
+            table = table[parent]
+            ttable = ttable[parent]
+           
+            #print('parent ', repr(parent),'key', repr(key))
+        
         #get the value and template type
         value = table.get( key, None)
-        tvalue = ttable.get( key, None)
+        tvalue = ttable.get( key, None)
         
         # no value - try template for default
         if (value is None) and (tvalue is not None):
             value = tvalue.get_default()
         
         # still no value assoicated with the key
         if value is None:
```

### Comparing `toml_file-1.0.0/toml_file/encoder.py` & `toml_file-1.0.1/toml_file/encoder.py`

 * *Files identical despite different names*

### Comparing `toml_file-1.0.0/toml_file/parser.py` & `toml_file-1.0.1/toml_file/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,17 @@
         while True:
             #read next line
             try:
                 rawline = self._read_more()
             except EOFError:
                 break
             
-            line = rawline.strip()
+            line = rawline.lstrip()
             if line.startswith('#'):
-                self.template.pre_comments.append(line)
+                self.template.pre_comments.append(line.strip())
             else:
                 break
         #add a blank line comment after to seperate main table comments to key pre-comment
         self.template.pre_comments.append('')
         
         #current data and template tables
         self.curent_dtable = self.data
@@ -110,15 +110,15 @@
             if line=='' and len(self.pre_comments)==0:
                 pass
             elif line=='' and len(self.pre_comments)>0:
                 self.pre_comments.append('')
 
             #check for comment line
             elif line.startswith('#'):
-                self.pre_comments.append(line)
+                self.pre_comments.append(line.strip())
                 
             #check for array of tables (list of dicts)
             elif line.startswith('[['):
                 self._parse_array_of_tables(line)
             
             #check for table
             elif line.startswith('['):
@@ -173,15 +173,15 @@
             #read next line
             try:
                 rawline = self._read_more()
             except EOFError:
                 break
 
             #strip whitespace
-            line = rawline.strip()
+            line = rawline.lstrip()
             
         #clear cache and return
         data = self.data
         template = self.template
         self.data = None
         self.template = None
         self.curent_dtable = self.data
@@ -533,27 +533,27 @@
     def _parse_ml_string(self, line):
         """
         Parse multi-line string (triple \") - reading more if required.
         """
         #check for string start
         if line.startswith('"""') is False:
             return None, line
-            
+                
         #strip 1st newline (as per toml spec)
         if line[3]=='\n':
             #need to start with next line
             try:
                 line = self._read_more()
             except EOFError:
                 raise ParsingError(f'Unclosed multiline string at line number {self.linenum}: {line}')
         else:
             #otherwise trim starting quotes
             line = line[3:]
-
-        #find the first sequence of unescaped """
+            
+        #find the last sequence of unescaped """
         i=-1
         while True:
             #find next triple quote
             i = line.find('"""', i+1) 
             if i==-1:
                 #read next line
                 try:
@@ -562,37 +562,45 @@
                     raise ParsingError(f'Unclosed multiline string at line number {self.linenum}: {line}')
                 #strip whitespace when lines end with \
                 if line.endswith('\\\n'):
                     line = line.rstrip('\\\n')
                     newline = newline.lstrip()
                 line = line+newline
                 
-            #check if unescaped end found
-            elif line[i-1]!='\\':
-                break
+            #check if there is another "
+            elif line[i+3] == '"':
+                pass #keep looking
+
+            #check if escaped
+            elif line[i-1]=='\\':
+                pass
                 
+            else:
+                break
+
             #print(f'ml_string next {repr(line)}')                
 
         # split out value and remainder
         value = line[:i]
         remainder = line[i+3:]
-        
+
         #hack check for possible extra quotes upto |""|"""
-        if remainder.startswith('""'):
-            value = value + '""'
-            remainder = remainder[2:]
-        elif remainder.startswith('"'):
-            value = value + '"'
-            remainder = remainder[1:]
-        
+        #if remainder.startswith('""'):
+        #    value = value + '""'
+        #    remainder = remainder[2:]
+        #elif remainder.startswith('"'):
+        #    value = value + '"'
+        #    remainder = remainder[1:]
+
         try:
             #value = str(value)
             #fix to keep \r inside strings replace with escape sequence
             value = value.replace('\r','\\r')
-            value = literal_eval('"""'+value+'"""')
+            value = literal_eval('""" '+value+' """') #add spaces to ensure it works even if " immediately before/after """
+            value = value[1:-1] #trim spaces
         except Exception as e:
             raise ParsingError( f"{e} at line number {self.linenum} : {line}") 
         
         #print(f'ml_string {repr(value)} , remainder {repr(remainder)}')
         ttype = StringType()
         
         return value, ttype, remainder
@@ -663,14 +671,23 @@
             i = line.find("'''", i+1) 
             if i==-1:
                 #read next line
                 try:
                     line = line + self._read_more()
                 except EOFError:
                     raise ParsingError(f'Unclosed multiline literal string at line number {self.linenum}: {line}')
+            
+            #check if there is another "
+            elif line[i+3] == "'":
+                pass #keep looking
+
+            #check if escaped
+            elif line[i-1]=='\\':
+                pass
+                
             #check if unescaped end found
             else:
                 break
                 
             #print(f'ml_literal next {repr(line)}') 
         
         # split out value and remainder
```

### Comparing `toml_file-1.0.0/toml_file/types.py` & `toml_file-1.0.1/toml_file/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,15 @@
             
     def __repr__(self):
         return 'Table'+dict.__repr__(self)
     
     # --- overload dict methods to only accept TomlBaseTypes
     def __setitem__(self, key, value):
         if isinstance(value, TomlBaseType) is False:
-            raise ValueError('Can only add TomlBaseType to TableType')
+            raise ValueError(f'Can only add TomlBaseType to TableType not {type(value)}')
         dict.__setitem__(self, key, value)
 
     def update(self, ttable):
         if isinstance(ttable, TableType) is False:
             raise ValueError('Can only update from TableType')
         dict.update(self, ttable)
         
@@ -1292,19 +1292,21 @@
             # write precomments
             precomments =  (os.linesep + sindent).join(ttable.pre_comments) 
             if precomments:
                 s += sindent + precomments + os.linesep
             
             # write section header
             if table_name:
-                s += sindent + f'[[{table_name}]]'
+                s += os.linesep + sindent + f'[[{table_name}]]'
                 
             # write post comment and indent new line
             if ttable.post_comment is not None:
                 s += sindent + ttable.post_comment + os.linesep
+            else:
+                s += os.linesep
                 
             # write the dict items
             s += _write_dict(ttable, dtable, 
                                 indent, indent_subtables, table_name)
         return s
     
     # Default value
```

### Comparing `toml_file-1.0.0/toml_file.egg-info/PKG-INFO` & `toml_file-1.0.1/toml_file.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml-file
-Version: 1.0.0
+Version: 1.0.1
 Summary: TOML file reader - python module to read/write toml configuration files
 Home-page: https://gitlab.com/tcharrett/totoml
 Author: Tom Charrett
 Author-email: tcharrett@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering
```

