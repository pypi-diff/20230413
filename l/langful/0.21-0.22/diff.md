# Comparing `tmp/langful-0.21-py2.py3-none-any.whl.zip` & `tmp/langful-0.22-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6517 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1476 b- defN 23-Mar-25 11:54 langful/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 23-Apr-09 05:45 langful/define.py
+Zip file size: 6765 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1469 b- defN 23-Apr-13 11:45 langful/__init__.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-13 11:13 langful/define.py
 -rw-rw-rw-  2.0 fat     1556 b- defN 23-Mar-25 12:16 langful/functions.py
--rw-rw-rw-  2.0 fat     8012 b- defN 23-Apr-09 06:29 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2605 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/RECORD
-9 files, 15744 bytes uncompressed, 5361 bytes compressed:  65.9%
+-rw-rw-rw-  2.0 fat     8834 b- defN 23-Apr-13 11:41 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-Apr-13 12:40 langful-0.22.dist-info/RECORD
+9 files, 16677 bytes uncompressed, 5609 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: langful/functions.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.21.dist-info/LICENSE
+Filename: langful-0.22.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.21.dist-info/METADATA
+Filename: langful-0.22.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.21.dist-info/WHEEL
+Filename: langful-0.22.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.21.dist-info/top_level.txt
+Filename: langful-0.22.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.21.dist-info/RECORD
+Filename: langful-0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/__init__.py

```diff
@@ -1,11 +1,11 @@
 """
 # langful
 
-Help developers to localize
+Help to localization
 
 # example
 
 - test.py
 - lang
     - zh_cn.json
     - en_us.json
```

## langful/define.py

```diff
@@ -1,10 +1,14 @@
 FILE = "file"
 DICT = "dict"
 
-def get_type( obj ) :
+UTF8 = "utf-8"
+
+def TheTypeError( obj , message : str = "" ) -> None : raise TypeError(f"{ message }can't use type { type( obj ) }")
+
+def get_type( obj ) -> str :
     if isinstance( obj , str ) :
         return FILE
     elif isinstance( obj , dict ) :
         return DICT
     else :
-        raise TypeError(f"can't use type {type(obj)}")
+        TheTypeError( obj )
```

## langful/lang.py

```diff
@@ -33,86 +33,91 @@
 
         """
 
         default_locale = locale.getdefaultlocale()[0].lower() # 默认语言
         self.type = get_type( lang_dir )
 
         if self.type == FILE :
+
             if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
                 raise KeyError( f"'{lang_dir}' dir not find" )
             if not len( os.listdir(lang_dir) ) :
-                raise RuntimeError( f"In '{lang_dir}' dir has no lang file!" ) # lang文件夹里没有语言文件
+                raise FileNotFoundError( f"'{lang_dir}' has no file!" ) # lang文件夹里没有语言文件
             if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
                 raise KeyError( f"'{default_lang}' not find" )
+
             lang_file = os.path.join( lang_dir , default_locale + file_suffix )
             file_suffix_len=len(file_suffix)
             lang_file_list = []
-            lang_str_list = []
             language_dict = {}
             use_locale = default_locale
             if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
                 use_locale = default_lang
                 lang_file = default_lang + file_suffix
+
             for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
                 if len( filename ) > file_suffix_len and filename[-file_suffix_len:] == file_suffix :
                     try :
-                        with open( os.path.join( lang_dir , filename ) , encoding = "utf-8" ) as file :
-                            language_dict[ filename[ :-file_suffix_len ] ] = json.load( file )
-                        lang_str_list.append( filename[ :-file_suffix_len ] )
+                        with open( os.path.join( lang_dir , filename ) , encoding = UTF8 ) as file :
+                            language_dict[ filename[ :-file_suffix_len ] ] = json.load( file ) # 加载文件
                         lang_file_list.append( filename )
                     except : pass
 
         elif self.type == DICT :
+            use_locale = default_lang
             if default_lang not in lang_dir :
                 raise KeyError( f"'{default_lang}' not find" )
-            if default_locale not in lang_dir :
-                use_locale = default_lang
+            if default_locale in lang_dir :
+                use_locale = default_locale
             language_dict = lang_dir
-            lang_str_list = list( lang_dir.keys() )
-
-        else :
-            raise TypeError(f"lang_dir can't use type {type(lang_dir)}")
 
         #lang_dir: Translation file storage directory
         #lang_dir: 翻译文件的存放目录
         self.lang_dir = lang_dir
         #default_lang: Default translation
         #default_lang: 默认使用的翻译
         self.default_lang = default_lang
-        #file_suffix: Such as '.json' '.lang' '.txt' and more
-        #file_suffix: 文件后缀 例如 '.json' '.lang' '.txt' 等等
-        if self.type == FILE :
-            self.file_suffix = file_suffix
-        # lang_file: Choose to use's language file
-        # lang_file: 选择使用的语言文件
-        if self.type == FILE :
-            self.lang_file = lang_file
-        # lang_file_list: All can find's language file
-        # lang_file_list: 所有能找到的语言文件
-        if self.type == FILE :
-            self.lang_file_list = lang_file_list
-        # lang_str_list: All can find's language file's name
-        # lang_str_list: 所有能找到的语言文件的名字
-        self.lang_str_list = lang_str_list
         # language_dict: Load all can read's language file
         # language_dict: 加载所有可以读取的语言文件
         self.language_dict = language_dict
-        # language: Load need's language file
-        # language: 加载需要的语言文件
-        self.language = language_dict[ use_locale ]
         # default_locale: The default language
         # default_locale:  默认语言
         self.default_locale = default_locale
         # use_locale: The selected language
         # use_locale: 选定的语言
         self.use_locale = use_locale
         # change: Specifies what character to use for substitution , default is '%'
         # change: 选择用什么符号做替换 默认为'%'
         self.change = change
 
+        if self.type == FILE :
+            #file_suffix: Such as '.json' '.lang'
+            #file_suffix: 文件后缀 例如 '.json' '.lang'
+            self.file_suffix = file_suffix
+            # lang_file: Choose to use's language file
+            # lang_file: 选择使用的语言文件
+            self.lang_file = lang_file
+            # lang_file_list: All can find's language file
+            # lang_file_list: 所有能找到的语言文件
+            self.lang_file_list = lang_file_list
+
+        self._reload()
+
+    def _lang_str_list_reload( self ) -> None :
+        # lang_str_list: All can find's language file's name
+        # lang_str_list: 所有能找到的语言文件的名字
+        self.lang_str_list = list( self.language_dict.keys() )
+    def _language_reload( self ) -> None :
+        # language: Load need's language file
+        # language: 加载需要的语言文件
+        self.language = self.language_dict[ self.use_locale ]
+    def _reload( self ) -> None :
+        self._lang_str_list_reload()
+        self._language_reload()
+
     def get( self , key:str , lang_str:str = None ) -> str : # 输入键 获取对应的值
         """
 
         # get
 
         Get one value in some one dictionary
 
@@ -134,18 +139,18 @@
         if not lang_str :
             lang_str = self.use_locale
 
         if lang_str in self.lang_str_list :
             if key in self.language_dict[ lang_str ] :
                 return self.language_dict[ lang_str ] [ key ]
             else :
-                raise KeyError( f"Key '{key}' has not in dictionary!" )
+                raise KeyError( f"key '{key}' has not in dictionary!" )
             
         else :
-            raise KeyError( f"Lang '{lang_str}' has not find!" )
+            raise KeyError( f"lang '{lang_str}' has not find!" )
 
     def set( self , key : str , value : str , lang_str : str = None ) -> None : # 设置某个键值
         """
 
         Set one value with one key in some one dictionary
 
         在某个字典中用一个值来设置一个键
@@ -172,21 +177,51 @@
         if not lang_str :
             lang_str = self.use_locale
 
         if lang_str in self.lang_str_list :
             self.language_dict[ lang_str ] [ key ] = value
 
         else :
-            raise KeyError( f"Lang '{lang_str}' has not find!" )
+            raise KeyError( f"lang '{lang_str}' has not find!" )
+
+    def add( self , lang_str : str , set : dict = {} ) -> None :
+        """
+
+        # add a new language
+
+        lang_str: the language's name
+
+        set: the language dictionary
+
+        ps: It can't change the file
+
+        ---
+
+        # 添加新语言
 
-        if lang_str == self.use_locale :
-            self.language = self.language_dict[ lang_str ]
+        lang_str: 语言名称
 
-    def add( self , lang_str : str ) -> None : #todo
-        pass
+        set: 语言字典
+
+        ps: 它不会影响文件
+
+        """
+        self.language_dict[ lang_str ] = set
+        if lang_str == self.default_locale :
+            self.use_locale = lang_str
+        self._reload()
+
+    def remove( self , lang_str : str ) -> None : #todo
+        """
+        # todo
+        """
+        if lang_str == self.use_locale or lang_str == self.default_lang or lang_str == self.default_locale :
+            raise RuntimeError( f"can't remove '{lang_str}' " )
+        del self.language_dict[ lang_str ]
+        del self.lang_str_list[ self.lang_str_list.index( lang_str ) ]
 
     def replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
         """
 
         Replace string with some one dictionary
 
         用某个字典替换字符串
@@ -219,25 +254,26 @@
         if not lang_str :
             lang_str = self.use_locale
 
         if lang_str in self.lang_str_list :
             language = self.language_dict[ lang_str ]
 
         else :
-            raise KeyError( f"Lang '{lang_str}' has not find!" )
+            raise KeyError( f"lang '{lang_str}' has not find!" )
 
         i = 0
         Ret = ""
         text = "".join( args ).split( change )
-        for I in text :
 
+        for I in text :
             if i % 2 :
-                if I in language : Ret += language[I]
-
-                elif not I : Ret += change
-
-                else : raise KeyError( f"Key '{I}' has not find!" )
-            else : Ret += I
-
+                if I in language :
+                    Ret += language[I]
+                elif not I :
+                    Ret += change
+                else :
+                    raise KeyError( f"key '{I}' has not find!" )
+            else :
+                Ret += I
             i += 1
 
         return Ret
```

## Comparing `langful-0.21.dist-info/LICENSE` & `langful-0.22.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.21.dist-info/METADATA` & `langful-0.22.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.21
+Version: 0.22
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langful Version: 0.21 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.22 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
```

