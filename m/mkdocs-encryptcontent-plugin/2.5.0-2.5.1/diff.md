# Comparing `tmp/mkdocs-encryptcontent-plugin-2.5.0.tar.gz` & `tmp/mkdocs-encryptcontent-plugin-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.0.tar", last modified: Tue Apr 11 19:45:56 2023, max compression
+gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.1.tar", last modified: Thu Apr 13 19:40:36 2023, max compression
```

## Comparing `mkdocs-encryptcontent-plugin-2.5.0.tar` & `mkdocs-encryptcontent-plugin-2.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.562727 mkdocs-encryptcontent-plugin-2.5.0/
--rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/LICENSE.md
--rw-rw-rw-   0        0        0    33921 2023-04-11 19:45:56.561728 mkdocs-encryptcontent-plugin-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    27027 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.475730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/
--rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.454730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.454730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.538730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/
--rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/lunr.js
--rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/main.js
--rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/worker.js
--rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-contents.tpl.js
--rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-form.tpl.html
--rw-rw-rw-   0        0        0    35943 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.559730 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/
--rw-rw-rw-   0        0        0    33921 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 19:45:56.562727 mkdocs-encryptcontent-plugin-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1780 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.683699 mkdocs-encryptcontent-plugin-2.5.1/
+-rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/LICENSE.md
+-rw-rw-rw-   0        0        0    33922 2023-04-13 19:40:36.682707 mkdocs-encryptcontent-plugin-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27028 2023-04-13 19:36:57.000000 mkdocs-encryptcontent-plugin-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.648699 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/
+-rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.640704 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.640704 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.652701 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/
+-rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/lunr.js
+-rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/main.js
+-rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/worker.js
+-rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-contents.tpl.js
+-rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-form.tpl.html
+-rw-rw-rw-   0        0        0    36211 2023-04-13 19:36:16.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.680698 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/
+-rw-rw-rw-   0        0        0    33922 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:40:36.683699 mkdocs-encryptcontent-plugin-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2023-04-13 19:37:10.000000 mkdocs-encryptcontent-plugin-2.5.1/setup.py
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/LICENSE.md` & `mkdocs-encryptcontent-plugin-2.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.0
+Version: 2.5.1
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -73,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
@@ -604,15 +604,15 @@
         
         Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
         If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
         and would be able to download them despite not having the password to the page.
         
         This feature should make it impossible or at least way harder for an external attacker to guess the file names.
         Please also check and disable directory listing for that matter.
-        Keep in mind that you hosting provider is still able to see all your images and files.
+        Keep in mind that your hosting provider is still able to see all your images and files.
         
         To counter file name guessing you could active the feature like this:
         
         ```yaml
         plugins:
             - encryptcontent:
                 selfhost: true
@@ -634,15 +634,15 @@
         You can define multiple exceptions at the `except` list.
         The file names that end with these strings will be skipped.
         You should use this if some images are used by themes or other plugins.
         Otherwise, you'd need to change these file names to the obfuscated ones.
         
         The file names are obfuscated in a way that the corresponding file is hashed with MD5
         and the hash is added to the file name
-        (If the file content is not changed the file name also not changes), like this:
+        (If the file content is not changed the file name remains the same), like this:
         
         some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
         ("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
         
         > The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
         
         # Contributing
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/README.md` & `mkdocs-encryptcontent-plugin-2.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-encryptcontent-plugin/
 python setup.py sdist bdist_wheel
-pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
+pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
 ```
 
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search: {}
@@ -596,15 +596,15 @@
 
 Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
 If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
 and would be able to download them despite not having the password to the page.
 
 This feature should make it impossible or at least way harder for an external attacker to guess the file names.
 Please also check and disable directory listing for that matter.
-Keep in mind that you hosting provider is still able to see all your images and files.
+Keep in mind that your hosting provider is still able to see all your images and files.
 
 To counter file name guessing you could active the feature like this:
 
 ```yaml
 plugins:
     - encryptcontent:
         selfhost: true
@@ -626,15 +626,15 @@
 You can define multiple exceptions at the `except` list.
 The file names that end with these strings will be skipped.
 You should use this if some images are used by themes or other plugins.
 Otherwise, you'd need to change these file names to the obfuscated ones.
 
 The file names are obfuscated in a way that the corresponding file is hashed with MD5
 and the hash is added to the file name
-(If the file content is not changed the file name also not changes), like this:
+(If the file content is not changed the file name remains the same), like this:
 
 some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
 ("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
 
 > The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
 
 # Contributing
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/lunr.js` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/main.js` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/worker.js` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-contents.tpl.js` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-contents.tpl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-form.tpl.html` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-form.tpl.html`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/plugin.py` & `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,39 +610,46 @@
         decrypt_js_path = Path(config.data["site_dir"] + '/assets/javascripts/decrypt-contents.js')
         with open(decrypt_js_path, "w") as file:
             file.write(self.__generate_decrypt_js__())
 
         #modify search_index in the style of mkdocs-exclude-search
         if self.setup['search_plugin_found'] and self.config['search_index'] != 'clear':
             search_index_filename = Path(config.data["site_dir"] + "/search/search_index.json")
-            #TODO: Check if search_index.json exists and error if not found (moved its location)
-            with open(search_index_filename, "r") as f:
-                search_entries = json.load(f)
+            try:
+                with open(search_index_filename, "r") as f:
+                    search_entries = json.load(f)
+            except:
+                logger.error('Search index needs modification, but could not read "search_index.json"!')
+                os._exit(1)
 
             for entry in search_entries['docs'].copy(): #iterate through all entries of search_index
                 for location in self.setup['locations'].keys():
                     if entry['location'] == location or entry['location'].startswith(location+"#"): #find the ones located at encrypted pages
                         page_password = self.setup['locations'][location][0]
                         if self.config['search_index'] == 'encrypted':
-                            search_entries.remove(entry)
+                            search_entries['docs'].remove(entry)
                         elif self.config['search_index'] == 'dynamically' and page_password is not None:
                             #encrypt text/title/location(anchor only)
                             text = entry['text']
                             title = entry['title']
                             toc_anchor = entry['location'].replace(location, '')
                             code = self.__encrypt_text_aes__(text, page_password )
                             entry['text'] = b';'.join(code).decode('ascii')
                             code = self.__encrypt_text_aes__(title, page_password)
                             entry['title'] = b';'.join(code).decode('ascii')
                             code = self.__encrypt_text_aes__(toc_anchor, page_password)
                             entry['location'] = location + ';' + b';'.join(code).decode('ascii')
                         break
 
-            with open(search_index_filename, "w") as f:
-                json.dump(search_entries, f)
+            try:
+                with open(search_index_filename, "w") as f:
+                    json.dump(search_entries, f)
+            except:
+                logger.error('Search index needs modification, but could not write "search_index.json"!')
+                os._exit(1)
             logger.info('Modified search_index.')
 
         # optionally download cryptojs
         if self.config['selfhost'] and self.config['selfhost_download']:
             logger.info('Downloading cryptojs for self-hosting (if needed)...')
             if self.config['selfhost_dir']:
                 configpath = Path(config['config_file_path']).parents[0]
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.0
+Version: 2.5.1
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -73,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
@@ -604,15 +604,15 @@
         
         Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
         If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
         and would be able to download them despite not having the password to the page.
         
         This feature should make it impossible or at least way harder for an external attacker to guess the file names.
         Please also check and disable directory listing for that matter.
-        Keep in mind that you hosting provider is still able to see all your images and files.
+        Keep in mind that your hosting provider is still able to see all your images and files.
         
         To counter file name guessing you could active the feature like this:
         
         ```yaml
         plugins:
             - encryptcontent:
                 selfhost: true
@@ -634,15 +634,15 @@
         You can define multiple exceptions at the `except` list.
         The file names that end with these strings will be skipped.
         You should use this if some images are used by themes or other plugins.
         Otherwise, you'd need to change these file names to the obfuscated ones.
         
         The file names are obfuscated in a way that the corresponding file is hashed with MD5
         and the hash is added to the file name
-        (If the file content is not changed the file name also not changes), like this:
+        (If the file content is not changed the file name remains the same), like this:
         
         some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
         ("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
         
         > The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
         
         # Contributing
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt` & `mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.0/setup.py` & `mkdocs-encryptcontent-plugin-2.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-encryptcontent-plugin',
-    version='2.5.0',
+    version='2.5.1',
     author='unverbuggt',
     author_email='unverbuggt@xn--rthlein-n2a.de',
     description='A MkDocs plugin that encrypt/decrypt markdown content with AES',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown encrypt decrypt content',
     url='https://github.com/unverbuggt/mkdocs-encryptcontent-plugin',
```

