# Comparing `tmp/prelude-cli-0.9.96.tar.gz` & `tmp/prelude-cli-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-0.9.96.tar", last modified: Fri Apr  7 19:52:22 2023, max compression
+gzip compressed data, was "prelude-cli-0.9.97.tar", last modified: Thu Apr 13 13:54:34 2023, max compression
```

## Comparing `prelude-cli-0.9.96.tar` & `prelude-cli-0.9.97.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.814551 prelude-cli-0.9.96/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-07 19:52:22.814601 prelude-cli-0.9.96/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-0.9.96/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.810638 prelude-cli-0.9.96/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1007 2023-02-28 15:28:14.000000 prelude-cli-0.9.96/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.811769 prelude-cli-0.9.96/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.814359 prelude-cli-0.9.96/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-0.9.96/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     5805 2023-03-28 21:39:17.000000 prelude-cli-0.9.96/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3355 2023-04-07 19:23:14.000000 prelude-cli-0.9.96/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    31024 2023-04-07 19:23:14.000000 prelude-cli-0.9.96/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.811573 prelude-cli-0.9.96/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      579 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      679 2023-04-07 19:52:22.814817 prelude-cli-0.9.96/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.145863 prelude-cli-0.9.97/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-13 13:54:34.145909 prelude-cli-0.9.97/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-0.9.97/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.142739 prelude-cli-0.9.97/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1078 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/cli.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.143715 prelude-cli-0.9.97/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.145648 prelude-cli-0.9.97/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-0.9.97/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     5966 2023-04-13 13:44:46.000000 prelude-cli-0.9.97/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3714 2023-04-13 13:44:46.000000 prelude-cli-0.9.97/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    31169 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/views/interactive.py
+-rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.143526 prelude-cli-0.9.97/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      679 2023-04-13 13:54:34.146135 prelude-cli-0.9.97/setup.cfg
```

### Comparing `prelude-cli-0.9.96/LICENSE` & `prelude-cli-0.9.97/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.96/PKG-INFO` & `prelude-cli-0.9.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.96
+Version: 0.9.97
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.96/prelude_cli/cli.py` & `prelude-cli-0.9.97/prelude_cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import click
 
 from prelude_cli.views.iam import iam
 from prelude_cli.views.build import build
 from prelude_cli.views.detect import detect
+from prelude_cli.views.partner import partner
 from prelude_sdk.models.account import Account
 from prelude_cli.views.configure import configure
 from prelude_cli.views.interactive import interactive as interactive_command
 
 
 @click.group(invoke_without_command=True)
 @click.version_option()
@@ -22,11 +23,12 @@
             click.echo(ctx.get_help())
 
 
 cli.add_command(iam)
 cli.add_command(configure)
 cli.add_command(detect)
 cli.add_command(build)
+cli.add_command(partner)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `prelude-cli-0.9.96/prelude_cli/views/build.py` & `prelude-cli-0.9.97/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.96/prelude_cli/views/configure.py` & `prelude-cli-0.9.97/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.96/prelude_cli/views/detect.py` & `prelude-cli-0.9.97/prelude_cli/views/detect.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 
 @detect.command('create-endpoint')
 @click.option('-h', '--host', help='hostname of this machine', type=str, required=True)
 @click.option('-s', '--serial_num', help='serial number of this machine', type=str, required=True)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default='')
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default='')
+@click.option('-i', '--endpoint_id', help='update a specific endpoint_id with the provided values', type=str, default='')
 @click.pass_obj
 @handle_api_error
-def register_endpoint(controller, host, serial_num, edr_id, tags):
+def register_endpoint(controller, host, serial_num, edr_id, tags, endpoint_id):
     """ Register a new endpoint """
-    token = controller.register_endpoint(host=host, serial_num=serial_num, edr_id=edr_id, tags=tags)
+    token = controller.register_endpoint(host=host, serial_num=serial_num, edr_id=edr_id, tags=tags, endpoint_id=endpoint_id)
     click.secho(token)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
@@ -37,16 +38,16 @@
 
 
 @detect.command('enable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only enable for these tags (comma-separated list)', type=str, default='')
 @click.option('-r', '--run_code',
               help='provide a run_code',
-              default='daily', show_default=True,
-              type=click.Choice(['daily', 'weekly', 'monthly'], case_sensitive=False))
+              default=RunCode.DAILY.name, show_default=True,
+              type=click.Choice([r.name for r in RunCode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def activate_test(controller, test, run_code, tags):
     """ Add test to your queue """
     controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
 
 
@@ -160,8 +161,7 @@
         filters['tags'] = tags
     if endpoints:
         filters['endpoints'] = endpoints
     if dos:
         filters['dos'] = dos
 
     print_json(data=controller.describe_activity(view=view, filters=filters))
-
```

### Comparing `prelude-cli-0.9.96/prelude_cli/views/iam.py` & `prelude-cli-0.9.97/prelude_cli/views/iam.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,34 +70,44 @@
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
     """ Remove a user from your account """
     controller.delete_user(handle=handle)
 
 
-@iam.command('attach-control')
+@iam.command('attach-partner')
 @click.argument('name')
-@click.option('--api', required=True, help='API endpoint of the control')
+@click.option('--api', required=True, help='API endpoint of the partner')
 @click.option('--user', required=True, help='user identifier')
 @click.option('--secret', default='', help='secret for OAUTH use cases')
 @click.pass_obj
 @handle_api_error
-def attach_control(controller, name, api, user, secret):
-    """ Attach an EDR or SIEM to Detect """
-    controller.attach_control(name=name, api=api, user=user, secret=secret)
+def attach_partner(controller, name, api, user, secret):
+    """ Attach an EDR to Detect """
+    controller.attach_partner(name=name, api=api, user=user, secret=secret)
 
 
-@iam.command('detach-control')
+@iam.command('detach-partner')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('name')
 @click.pass_obj
 @handle_api_error
-def detach_control(controller, name):
-    """ Detach an existing control from your account """
-    controller.detach_control(name=name)
+def detach_partner(controller, name):
+    """ Detach an existing partner from your account """
+    controller.detach_partner(name=name)
+
+
+@iam.command('logs')
+@click.option('-d', '--days', help='days back to search from today', default=7, type=int)
+@click.option('-l', '--limit', help='limit the number of results', default=1000, type=int)
+@click.pass_obj
+@handle_api_error
+def logs(controller, days, limit):
+    """ Get audit logs """
+    print_json(data=controller.audit_logs(days=days, limit=limit))
 
 
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def purge(controller):
```

### Comparing `prelude-cli-0.9.96/prelude_cli/views/interactive.py` & `prelude-cli-0.9.97/prelude_cli/views/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,33 +768,33 @@
             username = control['username']
             secret = control['secret']
             entry = f'{self.wiz.normalize(name, 20)} {self.wiz.normalize(api, 40)} {self.wiz.normalize(username, 10)} {self.wiz.normalize(secret, 10)} '
             menu[entry] = None
         TerminalMenu(menu.keys()).show()
 
 
-class AttachControl:
+class AttachPartner:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print('Learn about integrations: https://docs.preludesecurity.com/docs/defensive-integrations')
         menu = ['crowdstrike']
         answer = TerminalMenu(menu).show()
 
         name = menu[answer]
         api = Prompt.ask('API FQDN', default='https://api.us-2.crowdstrike.com')
         user = Prompt.ask('User or client ID', default=os.getlogin())
         secret = Prompt.ask('API token', default='password123')
         print(f'Attaching "{name}" to your account')
-        self.wiz.iam.attach_control(name=name, api=api, user=user, secret=secret)
+        self.wiz.iam.attach_partner(name=name, api=api, user=user, secret=secret)
 
 
-class DetachControl:
+class DetachPartner:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         account = self.wiz.iam.get_account()
         controls = [ctrl['name'] for ctrl in account['controls']]
@@ -804,15 +804,15 @@
             return
 
         menu = TerminalMenu(controls, multi_select=True, show_multi_select_hint=True)
         menu.show()
 
         for name in menu.chosen_menu_entries:
             print(f'Detaching "{name}" from your account')
-            self.wiz.iam.detach_control(name=name)
+            self.wiz.iam.detach_partner(name=name)
 
 
 class DeleteAccount:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
@@ -849,16 +849,16 @@
         self.wiz.splash(self.SPLASH, helper='Prelude accounts can contain multiple users with different permissions')
 
         menu = OrderedDict()
         menu['List users'] = ListUser
         menu['Create user'] = CreateUser
         menu['Delete user'] = DeleteUser
         menu['List integrations'] = ListControls
-        menu['Attach integration'] = AttachControl
-        menu['Detach integration'] = DetachControl
+        menu['Attach integration'] = AttachPartner
+        menu['Detach integration'] = DetachPartner
         menu['Delete account'] = DeleteAccount
 
         while True:
             try:
                 index = TerminalMenu(menu.keys(), title=self.title).show()
                 answer = list(menu.items())
                 answer[index][1](self.wiz).enter()
@@ -869,15 +869,17 @@
 class ExecutiveDashboard:
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     def enter(self):
-        webbrowser.open('https://platform.preludesecurity.com/detect', new=2)
+        account = self.wiz.detect.account.headers['account']
+        token = self.wiz.detect.account.headers['token']
+        webbrowser.open(f'{self.wiz.detect.account.hq}/iam/user?account={account}&token={token}', new=2)
 
 
 @click.command()
 @click.pass_obj
 def interactive(account):
     """ Interactive shell for Prelude Detect """
     wizard = Wizard(account=account)
```

### Comparing `prelude-cli-0.9.96/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-0.9.97/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.96
+Version: 0.9.97
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.96/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-0.9.97/prelude_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 prelude_cli/templates/template.go
 prelude_cli/views/__init__.py
 prelude_cli/views/build.py
 prelude_cli/views/configure.py
 prelude_cli/views/detect.py
 prelude_cli/views/iam.py
 prelude_cli/views/interactive.py
+prelude_cli/views/partner.py
 prelude_cli/views/shared.py
```

### Comparing `prelude-cli-0.9.96/setup.cfg` & `prelude-cli-0.9.97/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 0.9.96
+version = 0.9.97
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 0.9.96
+	prelude-sdk == 0.9.97
 	click
 	rich
 	simple-term-menu
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

