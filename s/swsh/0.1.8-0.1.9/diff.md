# Comparing `tmp/swsh-0.1.8.tar.gz` & `tmp/swsh-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swsh-0.1.8.tar", last modified: Fri Apr  7 20:00:03 2023, max compression
+gzip compressed data, was "swsh-0.1.9.tar", last modified: Thu Apr 13 19:18:48 2023, max compression
```

## Comparing `swsh-0.1.8.tar` & `swsh-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.003085 swsh-0.1.8/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 20:00:03.002282 swsh-0.1.8/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.8/README.md
--rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-07 20:00:03.003138 swsh-0.1.8/setup.cfg
--rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-07 19:59:40.000000 swsh-0.1.8/setup.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.000056 swsh-0.1.8/swsh/
--rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-05 20:48:52.000000 swsh-0.1.8/swsh/buy_a_phone_number.py
--rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.8/swsh/functions.py
--rwxr-xr-x   0 shane      (501) staff       (20)   136494 2023-04-07 19:57:21.000000 swsh-0.1.8/swsh/swsh.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.002069 swsh-0.1.8/swsh.egg-info/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/SOURCES.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/dependency_links.txt
--rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/entry_points.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.8/swsh.egg-info/not-zip-safe
--rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/requires.txt
--rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/top_level.txt
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-13 19:18:48.194524 swsh-0.1.9/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-13 19:18:48.194387 swsh-0.1.9/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.9/README.md
+-rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-13 19:18:48.194570 swsh-0.1.9/setup.cfg
+-rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-13 19:16:53.000000 swsh-0.1.9/setup.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-13 19:18:48.189759 swsh-0.1.9/swsh/
+-rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-13 19:02:10.000000 swsh-0.1.9/swsh/buy_a_phone_number.py
+-rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.9/swsh/functions.py
+-rwxr-xr-x   0 shane      (501) staff       (20)   135836 2023-04-13 19:13:23.000000 swsh-0.1.9/swsh/swsh.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-13 19:18:48.194179 swsh-0.1.9/swsh.egg-info/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/SOURCES.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/dependency_links.txt
+-rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/entry_points.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.9/swsh.egg-info/not-zip-safe
+-rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/requires.txt
+-rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-13 19:18:48.000000 swsh-0.1.9/swsh.egg-info/top_level.txt
```

### Comparing `swsh-0.1.8/PKG-INFO` & `swsh-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.8
+Version: 0.1.9
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `swsh-0.1.8/README.md` & `swsh-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `swsh-0.1.8/setup.py` & `swsh-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Natural Language :: English',
   'Topic :: Communications',
   'Topic :: Software Development'
 ]
 
 setup(
   name='swsh',
-  version='0.1.8',
+  version='0.1.9',
   description='SignalWire interactive SHell',
   entry_points={
     'console_scripts': ['swsh=swsh.swsh:main']
   },
   #long_description=read('README.md'),
   long_description_content_type="text/markdown",
   classifiers=CLASSIFIERS,
```

### Comparing `swsh-0.1.8/swsh/buy_a_phone_number.py` & `swsh-0.1.9/swsh/buy_a_phone_number.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.8/swsh/functions.py` & `swsh-0.1.9/swsh/functions.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.8/swsh/swsh.py` & `swsh-0.1.9/swsh/swsh.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,28 +160,14 @@
         else:
             print (' '.join(inp))
     
     def do_env(self, args):
         '''Return the SWiSH Environment Variables'''
         get_shell_env_all()
 
-    def do_ngrok_tunnel(self, inp):
-        '''Show and Attach to ngrok Tunnel Screen'''
-        tunnel_url = os.popen("curl -s http://127.0.0.1:4040/api/tunnels | jq -r '.tunnels[0].public_url'").read()
-        if tunnel_url == "":
-            # The Tunnel isn't active
-            print('There are no active NGROK tunnels established.\n')
-        else:
-            print("NGROK Tunnel URL = " + tunnel_url + "\n")
-            print("The NGROK console runs in SCREEN.  Press ctrl+a ctrl+d to disconnect. ")
-            selection = input("Would you like to connect to the NGROK console? (y/n): ")
-            if selection.lower() == "y" or selection.lower == "yes":
-                os.system("screen -r ngrok")
-                os.system("clear")
-
 ## SIP ENDPOINT COMMAND ##
     # Create the top level parser for sip endpoints: sip_endpoint
     base_sip_endpoint_parser = cmd2.Cmd2ArgumentParser()
     base_sip_endpoint_subparsers = base_sip_endpoint_parser.add_subparsers(title='SIP ENDPOINT',help='sip_endpoint help')
 
     # create the sip_endpoint list subcommand
     sip_endpoint_parser_list = base_sip_endpoint_subparsers.add_parser('list', help='List SIP Endpoints')
@@ -260,33 +246,33 @@
                     set_shell_env(key + "=" + value)
 
                 print(k_val + ")")
                 print("  SignalWire ID:\t" + str(output["id"]))
                 print("  Username:\t\t" + str(output["username"]))
                 print("  Caller Name:\t\t" + str(output["caller_id"]))
                 print("  Caller Number:\t" + str(output["send_as"]))
-                print("  Codecs:\t\t" + str(', '.join(output["codecs"])))
-                print("  Encryption Ciphers:\t" + str(', '.join(output["ciphers"])))
+                print("  Codecs:\t\t" + str(', '.join((list(filter(None, output["codecs"]))))))
+                print("  Encryption Ciphers:\t" +str(', '.join((list(filter(None, output["ciphers"]))))))
                 print("  Encrytion Enabled:\t" + str(output["encryption"]))
                 print("")
 
             elif args.json:
                 json_nice_print(output["data"])
 
             else:
                 for k, v in enumerate(output["data"]):
                     k_num = str(k + 1)
 
                     print(k_num + ")")
-                    print(" SignalWire ID:\t" + str(output["data"][k]["id"]))
+                    print(" SignalWire ID:\t\t" + str(output["data"][k]["id"]))
                     print(" Username:\t\t" + str(output["data"][k]["username"]))
                     print(" Caller ID Name:\t" + str(output["data"][k]["caller_id"]))
                     print(" Caller ID Number:\t" + str(output["data"][k]["send_as"]))
-                    print(" Codecs:\t\t" + str(', '.join(output["data"][k]["codecs"])))
-                    print(" Encryption Ciphers:\t" + str(', '.join(output["data"][k]["ciphers"])))
+                    print(" Codecs:\t\t" + str(', '.join((list(filter(None, output["data"][k]["codecs"]))))))
+                    print(" Encryption Ciphers:\t" + str(', '.join((list(filter(None, output["data"][k]["ciphers"]))))))
                     print(" Encrytion Enabled:\t" + str(output["data"][k]["encryption"]))
                     print("")
    
         else:
             is_json = validate_json(output)
             if is_json:
                 print_error_json(output)
```

### Comparing `swsh-0.1.8/swsh.egg-info/PKG-INFO` & `swsh-0.1.9/swsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.8
+Version: 0.1.9
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

