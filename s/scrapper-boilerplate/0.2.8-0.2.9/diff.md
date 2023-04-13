# Comparing `tmp/scrapper-boilerplate-0.2.8.tar.gz` & `tmp/scrapper-boilerplate-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapper-boilerplate-0.2.8.tar", last modified: Wed Jul 20 15:32:08 2022, max compression
+gzip compressed data, was "scrapper-boilerplate-0.2.9.tar", last modified: Tue Mar 28 21:09:49 2023, max compression
```

## Comparing `scrapper-boilerplate-0.2.8.tar` & `scrapper-boilerplate-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.679143 scrapper-boilerplate-0.2.8/
--rw-rw-rw-   0        0        0     2124 2022-07-20 15:32:08.679143 scrapper-boilerplate-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1332 2021-11-08 16:21:49.000000 scrapper-boilerplate-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.507269 scrapper-boilerplate-0.2.8/scrapper_boilerplate/
--rw-rw-rw-   0        0        0      577 2022-05-30 19:09:28.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.554145 scrapper-boilerplate-0.2.8/scrapper_boilerplate/account/
--rw-rw-rw-   0        0        0      206 2021-11-08 16:07:26.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/account/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.554145 scrapper-boilerplate-0.2.8/scrapper_boilerplate/build/
--rw-rw-rw-   0        0        0      218 2021-11-08 16:07:26.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/build/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.554145 scrapper-boilerplate-0.2.8/scrapper_boilerplate/cookies/
--rw-rw-rw-   0        0        0      441 2021-11-08 16:07:26.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/cookies/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.554145 scrapper-boilerplate-0.2.8/scrapper_boilerplate/datababase_state/
--rw-rw-rw-   0        0        0     2041 2022-06-22 14:18:18.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/datababase_state/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.569768 scrapper-boilerplate-0.2.8/scrapper_boilerplate/file_handler/
--rw-rw-rw-   0        0        0     2848 2022-07-18 14:25:10.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/file_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.585393 scrapper-boilerplate-0.2.8/scrapper_boilerplate/output/
--rw-rw-rw-   0        0        0      642 2022-06-14 15:48:51.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/output/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.585393 scrapper-boilerplate-0.2.8/scrapper_boilerplate/parser_handler/
--rw-rw-rw-   0        0        0     2948 2022-07-18 15:49:16.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/parser_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.601020 scrapper-boilerplate-0.2.8/scrapper_boilerplate/proxy/
--rw-rw-rw-   0        0        0     1301 2021-11-08 17:00:19.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/proxy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.616659 scrapper-boilerplate-0.2.8/scrapper_boilerplate/setup/
--rw-rw-rw-   0        0        0     4071 2022-07-20 14:59:34.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.647903 scrapper-boilerplate-0.2.8/scrapper_boilerplate/telegram/
--rw-rw-rw-   0        0        0     1390 2022-06-22 15:50:30.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/telegram/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.663522 scrapper-boilerplate-0.2.8/scrapper_boilerplate/timer/
--rw-rw-rw-   0        0        0      227 2021-11-08 16:07:26.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/timer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.663522 scrapper-boilerplate-0.2.8/scrapper_boilerplate/warnings/
--rw-rw-rw-   0        0        0      195 2022-06-22 15:50:03.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/warnings/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.663522 scrapper-boilerplate-0.2.8/scrapper_boilerplate/webdriver_handler/
--rw-rw-rw-   0        0        0     3962 2022-07-18 15:40:43.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate/webdriver_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-20 15:32:08.538519 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/
--rw-rw-rw-   0        0        0     2124 2022-07-20 15:32:06.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2022-07-20 15:32:06.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-20 15:32:06.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2022-07-20 15:32:06.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-07-20 15:32:06.000000 scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-20 15:32:08.679143 scrapper-boilerplate-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1336 2022-07-20 14:59:15.000000 scrapper-boilerplate-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.503555 scrapper-boilerplate-0.2.9/
+-rw-rw-rw-   0        0        0     1942 2023-03-28 21:09:49.502562 scrapper-boilerplate-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1332 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.472937 scrapper-boilerplate-0.2.9/scrapper_boilerplate/
+-rw-rw-rw-   0        0        0      577 2023-03-28 20:56:42.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.481469 scrapper-boilerplate-0.2.9/scrapper_boilerplate/account/
+-rw-rw-rw-   0        0        0      206 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/account/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.483471 scrapper-boilerplate-0.2.9/scrapper_boilerplate/build/
+-rw-rw-rw-   0        0        0      218 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.485469 scrapper-boilerplate-0.2.9/scrapper_boilerplate/cookies/
+-rw-rw-rw-   0        0        0      441 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/cookies/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.486469 scrapper-boilerplate-0.2.9/scrapper_boilerplate/file_handler/
+-rw-rw-rw-   0        0        0     2931 2023-03-28 19:51:09.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/file_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.488500 scrapper-boilerplate-0.2.9/scrapper_boilerplate/output/
+-rw-rw-rw-   0        0        0      642 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/output/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.490503 scrapper-boilerplate-0.2.9/scrapper_boilerplate/parser_handler/
+-rw-rw-rw-   0        0        0     3837 2023-03-28 20:53:58.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/parser_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.491497 scrapper-boilerplate-0.2.9/scrapper_boilerplate/proxy/
+-rw-rw-rw-   0        0        0     1301 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/proxy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.492500 scrapper-boilerplate-0.2.9/scrapper_boilerplate/setup/
+-rw-rw-rw-   0        0        0     5253 2023-03-28 21:02:10.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.494500 scrapper-boilerplate-0.2.9/scrapper_boilerplate/state_manager/
+-rw-rw-rw-   0        0        0     2041 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/state_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.496500 scrapper-boilerplate-0.2.9/scrapper_boilerplate/telegram/
+-rw-rw-rw-   0        0        0     1390 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/telegram/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.498556 scrapper-boilerplate-0.2.9/scrapper_boilerplate/timer/
+-rw-rw-rw-   0        0        0      227 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/timer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.499562 scrapper-boilerplate-0.2.9/scrapper_boilerplate/warnings/
+-rw-rw-rw-   0        0        0      195 2023-03-28 19:39:21.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/warnings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.501561 scrapper-boilerplate-0.2.9/scrapper_boilerplate/webdriver_handler/
+-rw-rw-rw-   0        0        0     4332 2023-03-28 20:59:03.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate/webdriver_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-28 21:09:49.480471 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/
+-rw-rw-rw-   0        0        0     1942 2023-03-28 21:09:49.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-03-28 21:09:49.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-28 21:09:49.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-03-28 21:09:49.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 21:09:49.000000 scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-28 21:09:49.503555 scrapper-boilerplate-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-03-28 19:51:50.000000 scrapper-boilerplate-0.2.9/setup.py
```

### Comparing `scrapper-boilerplate-0.2.8/PKG-INFO` & `scrapper-boilerplate-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: scrapper-boilerplate
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scrapping/Automating tools, userSwitching, anti-bot detection and more...
 Home-page: https://job-hunting.readthedocs.io/
 Author: Jeferson/MxJeff
 Author-email: mx.jeferson.10@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # scrapper-boilerplate
 
 
 Scrapping functions and for making easy for further scrapping
@@ -89,8 +84,7 @@
     sleep(10)
     driver.quit()
 
 if __name__ == "__main__":
     main()
 
 ```
-
```

### Comparing `scrapper-boilerplate-0.2.8/README.md` & `scrapper-boilerplate-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/datababase_state/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/state_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/file_handler/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/file_handler/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import pandas as pd
 import os
 
 
-def remove_duplicates():
+def remove_duplicates(input_filename:str='input.txt', output_filename:str="output.txt"):
     print('Terminado! Verificando se existe linhas duplicadas...')
     lines_seen = set()
-    with open('profiles.txt', "w") as output_file:
-        for each_line in open('raw_profile.txt', "r"):
+    with open(output_filename, "w") as output_file:
+        for each_line in open(input_filename, "r"):
             if each_line not in lines_seen:  # check if line is not duplicate
                 output_file.write(each_line)
                 lines_seen.add(each_line)
 
     print('Terminado! link duplicados removidos')
 
 
@@ -20,27 +20,27 @@
     Save data to json file
     """
     print('Salvando os dados em JSON')
     with open(f'{filename}', 'w', encoding='utf-8') as file:
         json.dump(data, file, indent=4, ensure_ascii=False)
 
 
-def load_links(file_text):
+def load_txt_file(file_text:str):
     print('Iniciando leitura de links...')
-    with open(f'{file_text}.txt', 'r') as text:
+    with open(f'{file_text}', 'r') as text:
         return text.readlines()
 
 
-def JSONtoExcel(filename):
+def JSONtoExcel(filename:str):
     try:
         print('Iniciando convensão...')
         # temp_df = pd.read_json(f'{filename}.json')
         temp_df = load_json(filename)
         df = pd.json_normalize(temp_df)
-        df.to_excel(f'{filename}.xlsx')
+        df.to_excel(filename.replace(".json", '.xlsx'))
         print('Convensão realizada com sucesso!')
 
     except Exception as error:
         print('Falha na conversão, Arquivo incorreto ou não existe...')
 
 
 def CSVtoExcel(filename:str):
@@ -61,15 +61,15 @@
     """
     with open(f'{json_name}','r', encoding="utf-8") as file:
         data = json.load(file)
 
     return data
 
 
-def save_to_html(data:str, filename:str='coment.html', mode='w'):
+def save_to_html(data:str, filename:str='data.html', mode='w'):
     """
     save data to html
 
     data: str: data to save
     filename: str: filename to save
     mode: str: append file ou write file
     return: void"""
```

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/output/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/output/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/parser_handler/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/parser_handler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import requests
+import re
+import logging
 
 from bs4 import BeautifulSoup
 from requests.exceptions import InvalidSchema
 
 
 def init_crawler(url, params={"method":"GET", 'headers': None, 'body': None, 'timeout':10, "engine": "lxml" }):
     
@@ -86,7 +88,40 @@
 
 def remove_whitespaces(text):
     return " ".join(text.split())
 
 
 def remove_duplicates_on_list(array):
     return list(dict.fromkeys(array))
+
+
+def check_telephone(word):
+    """
+    Check if word contains a valid telephone number
+    """
+    target_tel = word.replace('.', ' ')
+    match = re.findall(r'\(\d{2}\)|\d{2}\s* \d{4,5}-\d{4}', target_tel)
+    if match:  
+        return "".join(match)
+    else:
+        return False
+
+
+def check_tag(soap, tag, first=True, check_text=True):
+    """
+    Check if the tag is valid
+    args:
+        - tag: str, the tag you want to check
+    returns:
+        - bool: True if the tag is valid, 'Não localizado...':str otherwise
+    """
+    try:
+        if first:
+            element = soap.select_one(tag).text if check_text else soap.select_one(tag)
+            if not element: return
+
+        element = soap.select(tag)
+        if not element: return
+
+    except Exception as error:
+        logging.error(error)
+        return
```

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/proxy/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/setup/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/setup/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 from dotenv import load_dotenv
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from selenium.webdriver.chrome.service import Service
 
 
-def choose_driver(driver_name):
+def choose_driver(driver_name:str):
     if driver_name == "chrome":
         return ChromeDriverManager().install()
     elif driver_name == "firefox":
         return GeckoDriverManager().install()
     elif driver_name == "edge":
         return EdgeChromiumDriverManager().install()
     else:
         return ChromeDriverManager().install()
 
 
-def setSelenium(headless=True, rotate_useragent=False, remote_webdriver=False, driver_name="chrome", profile=False, profile_name="default"):
+def setSelenium(headless:bool=True, rotate_useragent:bool=False, remote_webdriver:bool=True, driver_name:str="chrome", profile:bool=False, profile_name:str="default") -> webdriver.Chrome :
     """
     Set Selenium Webdriver
     args: 
         - headless: bool, True if you want to run the browser in headless mode
         - rotate_useragent: bool, True if you want to rotate the useragent
         - remote_webdriver: bool, True if you want to download and use the remote webdriver
         - driver_name: str, the name of the driver you want to use
+        - profile_name: str, the name of the profile
+        - profile:bool, True if you want to use profiles
 
     returns:
-        - webdriver: Selenium Webdriver
+        - webdriver: Selenium Webdriver instance
     """
 
 
     chrome_options = Options()
     load_dotenv()
 
     if headless:
@@ -84,20 +86,45 @@
     # if proxy:
     #     PROXY = init_proxy()
     #     chrome_options.add_argument('--proxy-server=%s' % PROXY)
 
     return webdriver.Chrome(options=chrome_options, service=Service(executable_path=resource_path(path), log_path='NUL'))
 
 
-def init_log(filesave=False, filename="debug.log", level=logging.INFO):
-    """
-    Initialize the log
-    args: 
-        - filesave: bool, True if you want to save the log in a file
-        - filename: str, the name of the file you want to save the log
+def init_log(filesave:bool=False, filename:str="debug.log", level=logging.INFO, **kwargs) -> None:
+    
+    """setup a configured custom log handler
+
+    parameters:
+        - filename (str): log filename
+        - filesave (bool): if save to file or not (default:False)
+        - level (logging): log leve (default:logging.INFO)
+
+    returns:
+        None
     """
+
+    logger = logging.getLogger()
+    logger.setLevel(logging.DEBUG)
+     
+    # create console handler and set level to info
+    handler = logging.StreamHandler()
+    handler.setLevel(logging.INFO)
+    formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s", datefmt='%d/%m/%Y %H:%M:%S')
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
     
+    if kwargs.get("error_sep") and filesave:
+        # create error file handler and set level to error
+        handler = logging.FileHandler(os.path.join("error.log"),"w", encoding=None, delay="true")
+        handler.setLevel(logging.ERROR)
+        formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s", datefmt='%d/%m/%Y %H:%M:%S')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+   
     if filesave:
-        logging.basicConfig(level=level, format='%(asctime)s %(message)s', datefmt='%d/%m/%Y %H:%M:%S', filename=filename, filemode='a')
-
-    else:
-        logging.basicConfig(level=level, format='%(asctime)s - %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S')
+        # create debug file handler and set level to debug
+        handler = logging.FileHandler(os.path.join(filename),"w")
+        handler.setLevel(level)
+        formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s", datefmt='%d/%m/%Y %H:%M:%S')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
```

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/telegram/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate/webdriver_handler/__init__.py` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate/webdriver_handler/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import logging
+import random
+
 from time import sleep
+
 from scrapper_boilerplate.setup import setSelenium
 from scrapper_boilerplate.parser_handler import init_parser
 
-
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 
+from selenium.common.exceptions import TimeoutException
+
 
 def scrolldown(driver, element=None):
     """
     Scroll down the page
     args:
         - driver: Selenium Webdriver
     return: void
@@ -67,27 +71,39 @@
             driver.execute_script("window.scrollTo(0, document.body.scrollHeight/%s);" % scroll)
         
         else:
             driver.execute_script("arguments[0].scrollTo(0, arguments[0].scrollHeight/%s);" % (element, scroll))
         scroll += .01
 
 
-def load_dynamic_page(url, headless=True):
+def load_dynamic_page(url, headless=True, remote=True, scroll=False,**kwargs):
     """
     Load a dynamic page
     args:
         - url: str, the url of the page you want to load
         - headless: bool, True if you want to run the browser in headless mode
     returns:
         - driver: Selenium Webdriver
     """
 
-    with setSelenium(headless=headless) as driver:
+    with setSelenium(
+        headless=headless, 
+        remote_webdriver=remote, 
+        profile=kwargs.get("profile"), 
+        profile_name=kwargs.get("profile_name")
+    ) as driver:
         driver.get(url)
         driver.implicitly_wait(220)
+        
+        if scroll:
+            scrolldown(driver)
+
+        if kwargs.get("screenshot"):
+            driver.save_screenshot(kwargs.get("screenshot_name"))
+            
         html = driver.find_element(By.TAG_NAME, 'html')
         return init_parser(html.get_attribute('outerHTML'))
 
 
 def load_code(driver, full_page=False):
     """
     Load code from a page
@@ -102,33 +118,15 @@
         code = driver.page_source
         return init_parser(code)
 
     code = driver.get_attribute('outerHTML')
     return init_parser(code)
 
 
-def check_tag(tag):
-    """
-    Check if the tag is valid
-    args:
-        - tag: str, the tag you want to check
-    returns:
-        - bool: True if the tag is valid, 'Não localizado...':str otherwise
-    """
-    try:
-        handler = tag
-        return handler
-
-    except Exception as error:
-        print('Error')
-        logging.error(error)
-        return 'Não localizado...'
-
-
-def explicit_wait(driver, tag, element, timeout=10):
+def explicit_wait(driver, tag, element, timeout=10, screenshot=False, screenshot_name="screenshot.png"):
     """
     Explicit wait for a tag
     args:
         - driver: Selenium Webdriver
         - tag: str, the tag you want to wait for
         - timeout: int, the timeout of the wait
     returns:
@@ -136,10 +134,21 @@
     """
     try:
         handler = WebDriverWait(driver, timeout).until(
             EC.presence_of_element_located((tag, element))
         )
         return handler
     
-    except Exception as error:
-        logging.error(error)
+    except TimeoutException:
+        if screenshot:
+            driver.save_screenshot(screenshot_name)
+        logging.error("error to explicitly wait")
         return
+
+
+def mimic_user_input(webElement, text:str):
+    """
+    Mimic user input.
+    """
+    for char in text:
+        sleep(random.uniform(0.1, 0.2))
+        webElement.send_keys(char)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/PKG-INFO` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: scrapper-boilerplate
-Version: 0.2.8
+Version: 0.2.9
 Summary: Scrapping/Automating tools, userSwitching, anti-bot detection and more...
 Home-page: https://job-hunting.readthedocs.io/
 Author: Jeferson/MxJeff
 Author-email: mx.jeferson.10@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # scrapper-boilerplate
 
 
 Scrapping functions and for making easy for further scrapping
@@ -89,8 +84,7 @@
     sleep(10)
     driver.quit()
 
 if __name__ == "__main__":
     main()
 
 ```
-
```

### Comparing `scrapper-boilerplate-0.2.8/scrapper_boilerplate.egg-info/SOURCES.txt` & `scrapper-boilerplate-0.2.9/scrapper_boilerplate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 scrapper_boilerplate.egg-info/SOURCES.txt
 scrapper_boilerplate.egg-info/dependency_links.txt
 scrapper_boilerplate.egg-info/requires.txt
 scrapper_boilerplate.egg-info/top_level.txt
 scrapper_boilerplate/account/__init__.py
 scrapper_boilerplate/build/__init__.py
 scrapper_boilerplate/cookies/__init__.py
-scrapper_boilerplate/datababase_state/__init__.py
 scrapper_boilerplate/file_handler/__init__.py
 scrapper_boilerplate/output/__init__.py
 scrapper_boilerplate/parser_handler/__init__.py
 scrapper_boilerplate/proxy/__init__.py
 scrapper_boilerplate/setup/__init__.py
+scrapper_boilerplate/state_manager/__init__.py
 scrapper_boilerplate/telegram/__init__.py
 scrapper_boilerplate/timer/__init__.py
 scrapper_boilerplate/warnings/__init__.py
 scrapper_boilerplate/webdriver_handler/__init__.py
```

### Comparing `scrapper-boilerplate-0.2.8/setup.py` & `scrapper-boilerplate-0.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 # This call to setup() does all the work
 setup(
     name="scrapper-boilerplate",
-    version="0.2.8",
+    version="0.2.9",
     description="Scrapping/Automating tools, userSwitching, anti-bot detection and more...",
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
     url="https://job-hunting.readthedocs.io/",
     author="Jeferson/MxJeff",
     author_email="mx.jeferson.10@hotmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "selenium", 
         "requests", 
         "pandas", 
         "beautifulsoup4", 
         "python-dotenv", 
         "python-telegram-bot",
         "lxml",
         "fake-useragent",
         "webdriver-manager",
-        "SQLAlchemy"
+        "SQLAlchemy",
+        "openpyxl"
     ]
 )
```

