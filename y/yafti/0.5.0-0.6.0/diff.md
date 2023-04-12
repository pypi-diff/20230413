# Comparing `tmp/yafti-0.5.0.tar.gz` & `tmp/yafti-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafti-0.5.0.tar", max compression
+gzip compressed data, was "yafti-0.6.0.tar", max compression
```

## Comparing `yafti-0.5.0.tar` & `yafti-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-04-01 00:08:45.771630 yafti-0.5.0/LICENSE
--rw-r--r--   0        0        0    10052 2023-04-01 00:08:45.771630 yafti-0.5.0/README.md
--rw-r--r--   0        0        0     1528 2023-04-01 00:08:45.771630 yafti-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/__main__.py
--rw-r--r--   0        0        0     2081 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/abc.py
--rw-r--r--   0        0        0     1901 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/app.py
--rw-r--r--   0        0        0     1813 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/events.py
--rw-r--r--   0        0        0      532 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/log.py
--rw-r--r--   0        0        0     1571 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/parser.py
--rw-r--r--   0        0        0     6795 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/plugin/flatpak.py
--rw-r--r--   0        0        0     2760 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/plugin/run.py
--rw-r--r--   0        0        0      302 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/registry.py
--rw-r--r--   0        0        0     3278 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/consent.py
--rw-r--r--   0        0        0     2227 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/console.py
--rw-r--r--   0        0        0     1817 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/dialog.py
--rw-r--r--   0        0        0       50 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/package/__init__.py
--rw-r--r--   0        0        0      310 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/package/models.py
--rw-r--r--   0        0        0       98 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/package/screen/__init__.py
--rw-r--r--   0        0        0     4353 2023-04-01 00:08:45.771630 yafti-0.5.0/yafti/screen/package/screen/install.py
--rw-r--r--   0        0        0     3705 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/package/screen/package.py
--rw-r--r--   0        0        0     5311 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/package/screen/picker.py
--rw-r--r--   0        0        0     1368 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/package/state.py
--rw-r--r--   0        0        0      402 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/package/utils.py
--rw-r--r--   0        0        0     3104 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/title.py
--rw-r--r--   0        0        0     1214 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/utils.py
--rw-r--r--   0        0        0     5216 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/screen/window.py
--rw-r--r--   0        0        0      448 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/setup.py
--rw-r--r--   0        0        0       32 2023-04-01 00:08:45.775631 yafti-0.5.0/yafti/share.py
--rw-r--r--   0        0        0    10952 1970-01-01 00:00:00.000000 yafti-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-12 22:19:04.769860 yafti-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10052 2023-04-12 22:19:04.769860 yafti-0.6.0/README.md
+-rw-r--r--   0        0        0     1528 2023-04-12 22:19:04.769860 yafti-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/__main__.py
+-rw-r--r--   0        0        0     2081 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/abc.py
+-rw-r--r--   0        0        0     1901 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/app.py
+-rw-r--r--   0        0        0     1813 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/events.py
+-rw-r--r--   0        0        0      532 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/log.py
+-rw-r--r--   0        0        0     1571 2023-04-12 22:19:04.769860 yafti-0.6.0/yafti/parser.py
+-rw-r--r--   0        0        0     6823 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/plugin/flatpak.py
+-rw-r--r--   0        0        0     2760 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/plugin/run.py
+-rw-r--r--   0        0        0      302 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/registry.py
+-rw-r--r--   0        0        0     3278 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/consent.py
+-rw-r--r--   0        0        0     2227 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/console.py
+-rw-r--r--   0        0        0     1817 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/dialog.py
+-rw-r--r--   0        0        0       50 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/__init__.py
+-rw-r--r--   0        0        0      317 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/models.py
+-rw-r--r--   0        0        0       98 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/__init__.py
+-rw-r--r--   0        0        0     5151 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/install.py
+-rw-r--r--   0        0        0     4002 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/package.py
+-rw-r--r--   0        0        0     5522 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/screen/picker.py
+-rw-r--r--   0        0        0     1368 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/state.py
+-rw-r--r--   0        0        0      509 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/package/utils.py
+-rw-r--r--   0        0        0     3104 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/title.py
+-rw-r--r--   0        0        0     1214 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/utils.py
+-rw-r--r--   0        0        0     5216 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/screen/window.py
+-rw-r--r--   0        0        0      448 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/setup.py
+-rw-r--r--   0        0        0       32 2023-04-12 22:19:04.773860 yafti-0.6.0/yafti/share.py
+-rw-r--r--   0        0        0    10952 1970-01-01 00:00:00.000000 yafti-0.6.0/PKG-INFO
```

### Comparing `yafti-0.5.0/LICENSE` & `yafti-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/README.md` & `yafti-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/pyproject.toml` & `yafti-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yafti"
-version = "0.5.0"
+version = "0.6.0"
 description = "Yet another first time installer"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/ublue-os/yafti"
 repository = "https://github.com/ublue-os/yafti"
 classifiers = [
@@ -37,15 +37,15 @@
 "yafti.screen.console" = "yafti.screen.console:ConsoleScreen"
 "yafti.screen.consent" = "yafti.screen.consent:ConsentScreen"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
-ruff = ">=0.0.254,<0.0.258"
+ruff = ">=0.0.254,<0.0.262"
 coverage = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `yafti-0.5.0/yafti/__init__.py` & `yafti-0.6.0/yafti/__init__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/__main__.py` & `yafti-0.6.0/yafti/__main__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/abc.py` & `yafti-0.6.0/yafti/abc.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/app.py` & `yafti-0.6.0/yafti/app.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/events.py` & `yafti-0.6.0/yafti/events.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/log.py` & `yafti-0.6.0/yafti/log.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/parser.py` & `yafti-0.6.0/yafti/parser.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/plugin/flatpak.py` & `yafti-0.6.0/yafti/plugin/flatpak.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,26 +146,26 @@
         """Map a series of boolean keyword arguments to command-line flags"""
         arg_map = {"update": "or-update"}
 
         return [f"--{arg_map.get(k, k)}" for k, v in kwargs.items() if v is True]
 
     async def install(
         self,
-        pkg: str,
+        package: str,
         user: bool = True,
         system: bool = False,
         assumeyes: bool = True,
         reinstall: bool = False,
         noninteractive: bool = True,
         update: bool = True,
     ) -> YaftiPluginReturn:
         """Install flatpak package on the host system
 
         Args:
-          pkg: Name of the flatpak package to install
+          package: Name of the flatpak package to install
           user: Install on the user installation
           system: Install on the system-wide installation
           assumeyes:
 
         Returns:
           An object containing the stdout and stderr from the flatpak command
 
@@ -178,46 +178,46 @@
             assumeyes=assumeyes,
             reinstall=reinstall,
             update=update,
             noninteractive=noninteractive,
         )
         cmd = [self.bin, "install"]
         cmd.extend(args)
-        cmd.append(pkg)
+        cmd.append(package)
         return await self.exec(" ".join(cmd))
 
     async def remove(
         self,
-        pkg: str,
+        package: str,
         user: bool = False,
         system: bool = True,
         force: bool = False,
         noninteractive: bool = True,
     ) -> YaftiPluginReturn:
         """Remove flatpak package on the host system"""
         args = self._parse_args(
             user=user, system=system, force=force, noninteractive=noninteractive
         )
         cmd = [self.bin, "remove"]
         cmd.extend(args)
-        cmd.append(pkg)
+        cmd.append(package)
         return self.exec(cmd)
 
     def ls(self) -> list[ApplicationDetail]:
         pass
 
     def __call__(self, options) -> YaftiPluginReturn:
         try:
             params = self.validate(options)
         except ValidationError as e:
             return YaftiPluginReturn(errors=str(e), code=1)
 
         # TODO: when a string is passed, make sure it maps to the "pkg" key.
         if params.install:
             if isinstance(params.install, str):
-                params.install = {"pkg": params.install}
+                params.install = {"package": params.install}
             r = asyncio.ensure_future(self.install(**params.install))
         else:
             if isinstance(params.remove, str):
-                params.remove = {"pkg": params.remove}
+                params.remove = {"package": params.remove}
             r = asyncio.ensure_future(self.remove(**params.install))
         return YaftiPluginReturn(output=r.stdout, errors=r.stderr, code=r.returncode)
```

### Comparing `yafti-0.5.0/yafti/plugin/run.py` & `yafti-0.6.0/yafti/plugin/run.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/consent.py` & `yafti-0.6.0/yafti/screen/consent.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/console.py` & `yafti-0.6.0/yafti/screen/console.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/dialog.py` & `yafti-0.6.0/yafti/screen/dialog.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/package/screen/install.py` & `yafti-0.6.0/yafti/screen/package/screen/install.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import asyncio
+import json
+
 from gi.repository import Gtk
+from typing import Optional
 
 import yafti.share
 from yafti import events
-from yafti.abc import YaftiScreen, YaftiScreenConfig
+from yafti import log
+from yafti.abc import YaftiScreen
 from yafti.screen.console import ConsoleScreen
 from yafti.screen.package.state import STATE
 
 _xml = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
   <requires lib="gtk" version="4.0"/>
@@ -63,28 +68,28 @@
 class PackageInstallScreen(YaftiScreen, Gtk.Box):
     __gtype_name__ = "YaftiPackageInstallScreen"
 
     pkg_progress = Gtk.Template.Child()
     btn_console = Gtk.Template.Child()
     started = False
     already_run = False
-
-    class Config(YaftiScreenConfig):
-        package_manager: str = "yafti.plugin.flatpak"
+    pulse = True
 
     def __init__(
         self,
         title: str = "Package Installation",
         package_manager: str = "yafti.plugin.flatpak",
+        package_manager_defaults: Optional[dict] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         from yafti.registry import PLUGINS
 
         self.package_manager = PLUGINS.get(package_manager)
+        self.package_manager_defaults = package_manager_defaults or {}
         self.btn_console.connect("clicked", self.toggle_console)
 
     async def on_activate(self):
         if self.started or self.already_run:
             return
         self.console = ConsoleScreen()
         self.started = True
@@ -94,30 +99,48 @@
     async def next(self, _):
         return self.started
 
     def toggle_console(self, btn):
         btn.set_label("Show Console" if self.console.get_visible() else "Hide Console")
         self.console.toggle_visible()
 
-    async def draw(self):
+    async def do_pulse(self):
+        self.pkg_progress.set_pulse_step(1.0)
+        while self.pulse:
+            self.pkg_progress.pulse()
+            await asyncio.sleep(0.5)
+
+    def draw(self):
         self.console.hide()
         self.append(self.console)
         packages = [item.replace("pkg:", "") for item in STATE.get_on("pkg:")]
-        await self.install(packages)
+        asyncio.create_task(self.do_pulse())
+        return self.install(packages)
+
+    def run_package_manager(self, packge_config):
+        try:
+            config = json.loads(packge_config)
+        except json.decoder.JSONDecodeError as e:
+            log.debug("could not parse", config=packge_config, e=e)
+            config = {"package": packge_config}
+
+        log.debug("parsed packages config", config=config)
+        opts = self.package_manager_defaults.copy()
+        opts.update(config)
+        return self.package_manager.install(**opts)
 
     async def install(self, packages: list):
         total = len(packages)
-        self.pkg_progress.set_fraction(0.01)
         yafti.share.BTN_NEXT.set_label("Installing...")
         yafti.share.BTN_BACK.set_visible(False)
-
         for idx, pkg in enumerate(packages):
-            r = await self.package_manager.install(pkg)
-            self.console.stdout(r.stdout)
-            self.console.stderr(r.stderr)
+            results = await self.run_package_manager(pkg)
+            self.console.stdout(results.stdout)
+            self.console.stderr(results.stderr)
+            self.pulse = False
             self.pkg_progress.set_fraction((idx + 1) / total)
 
         self.console.stdout(b"Installation Complete!")
 
         self.started = False
         self.already_run = True
         yafti.share.BTN_NEXT.set_label("Next")
```

### Comparing `yafti-0.5.0/yafti/screen/package/screen/package.py` & `yafti-0.6.0/yafti/screen/package/screen/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,39 +39,46 @@
     pkg_carousel = Gtk.Template.Child()
 
     class Config(YaftiScreenConfig):
         show_terminal: bool = True
         package_manager: str
         groups: Optional[PackageGroupConfig] = None
         packages: Optional[list[PackageConfig]] = None
+        package_manager_defaults: Optional[dict] = None
 
     def __init__(
         self,
         title: str = "Package Installation",
         package_manager: str = "yafti.plugin.flatpak",
         packages: list[PackageConfig] = None,
         groups: PackageGroupConfig = None,
         show_terminal: bool = True,
+        package_manager_defaults: Optional[dict] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.title = title
         self.packages = groups or packages
         self.show_terminal = show_terminal
         self.package_manager = package_manager
+        self.package_manager_defaults = package_manager_defaults
         STATE.load(parse_packages(self.packages))
         self.pkg_carousel.connect("page-changed", self.changed)
         self.draw()
 
     def draw(self):
         self.pkg_carousel.append(
             PackagePickerScreen(title=self.title, packages=self.packages)
         )
         self.pkg_carousel.append(
-            PackageInstallScreen(title=self.title, package_manager=self.package_manager)
+            PackageInstallScreen(
+                title=self.title,
+                package_manager=self.package_manager,
+                package_manager_defaults=self.package_manager_defaults,
+            )
         )
 
     def on_activate(self):
         events.on("btn_next", self.next)
         events.on("btn_back", self.back)
         yafti.share.BTN_NEXT.set_label("Install")
```

### Comparing `yafti-0.5.0/yafti/screen/package/screen/picker.py` & `yafti-0.6.0/yafti/screen/package/screen/picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import partial
+import json
 
 from gi.repository import Adw, Gtk
 from pydantic import BaseModel
 
 from yafti import log
 from yafti.abc import YaftiScreen
 from yafti.screen.dialog import DialogBox
@@ -75,14 +76,16 @@
             action_row = Adw.ActionRow(title=name, subtitle=details.get("description"))
 
             def state_set(group, _, value):
                 STATE.set(f"group:{group}", value)
                 d = self.packages.get(group)
                 for pkg in d.get("packages", []):
                     for pkg_name in pkg.values():
+                        if isinstance(pkg_name, dict):
+                            pkg_name = json.dumps(pkg_name)
                         STATE.set(f"pkg:{pkg_name}", value)
 
             state_set(name, None, details.get("default", True))
             _switcher = Gtk.Switch()
             _switcher.set_active(STATE.get(f"group:{name}"))
             _switcher.set_valign(Gtk.Align.CENTER)
 
@@ -139,14 +142,16 @@
     def _build_apps(self, packages: list):
         for item in packages:
             for name, pkg in item.items():
                 _apps_action_row = Adw.ActionRow(
                     title=name,
                 )
                 _app_switcher = Gtk.Switch()
+                if isinstance(pkg, dict):
+                    pkg = json.dumps(pkg)
                 _app_switcher.set_active(STATE.get(f"pkg:{pkg}"))
                 _app_switcher.set_valign(Gtk.Align.CENTER)
 
                 def set_state(pkg, btn, value):
                     log.debug("state-set", pkg=pkg, value=value)
                     STATE.set(f"pkg:{pkg}", value)
```

### Comparing `yafti-0.5.0/yafti/screen/package/state.py` & `yafti-0.6.0/yafti/screen/package/state.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/title.py` & `yafti-0.6.0/yafti/screen/title.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from functools import partial
-from typing import Optional, List
+from typing import List, Optional
 
 from gi.repository import Adw, Gtk
 
-from yafti.abc import YaftiScreen, YaftiScreenConfig
 from yafti import events
+from yafti.abc import YaftiScreen, YaftiScreenConfig
 from yafti.registry import PLUGINS
 
 _xml = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
     <requires lib="gtk" version="4.0"/>
     <requires lib="libadwaita" version="1.0" />
```

### Comparing `yafti-0.5.0/yafti/screen/utils.py` & `yafti-0.6.0/yafti/screen/utils.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/yafti/screen/window.py` & `yafti-0.6.0/yafti/screen/window.py`

 * *Files identical despite different names*

### Comparing `yafti-0.5.0/PKG-INFO` & `yafti-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafti
-Version: 0.5.0
+Version: 0.6.0
 Summary: Yet another first time installer
 Home-page: https://github.com/ublue-os/yafti
 License: Apache 2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: X11 Applications :: GTK
```

