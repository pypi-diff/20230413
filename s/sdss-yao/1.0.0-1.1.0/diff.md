# Comparing `tmp/sdss_yao-1.0.0.tar.gz` & `tmp/sdss_yao-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_yao-1.0.0.tar", max compression
+gzip compressed data, was "sdss_yao-1.1.0.tar", max compression
```

## Comparing `sdss_yao-1.0.0.tar` & `sdss_yao-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0     1504 2022-10-19 18:49:28.680204 sdss_yao-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      386 2022-10-19 18:49:28.680204 sdss_yao-1.0.0/README.md
--rw-r--r--   0        0        0     2377 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      450 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/__init__.py
--rw-r--r--   0        0        0     1410 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/__main__.py
--rw-r--r--   0        0        0     4487 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/actor.py
--rw-r--r--   0        0        0     3140 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/commands.py
--rw-r--r--   0        0        0    15417 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/delegate.py
--rw-r--r--   0        0        0    32902 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/etc/BOSS_extra.acf
--rw-r--r--   0        0        0     2419 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/etc/schema.json
--rw-r--r--   0        0        0     1675 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/etc/yao.yml
--rw-r--r--   0        0        0     1064 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/exceptions.py
--rw-r--r--   0        0        0    15318 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/mech_commands.py
--rw-r--r--   0        0        0    19486 2022-10-19 18:49:28.684204 sdss_yao-1.0.0/yao/mech_controller.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 sdss_yao-1.0.0/setup.py
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 sdss_yao-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0      386 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/README.md
+-rw-r--r--   0        0        0     2317 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/__init__.py
+-rw-r--r--   0        0        0     1410 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/__main__.py
+-rw-r--r--   0        0        0     4797 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/actor.py
+-rw-r--r--   0        0        0     6680 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/alerts.py
+-rw-r--r--   0        0        0     4893 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/commands.py
+-rw-r--r--   0        0        0     3831 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/controller.py
+-rw-r--r--   0        0        0    17514 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/delegate.py
+-rw-r--r--   0        0        0    32902 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra.acf
+-rw-r--r--   0        0        0    49124 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v2.acf
+-rw-r--r--   0        0        0    49106 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v3.acf
+-rw-r--r--   0        0        0    55310 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v4.acf
+-rw-r--r--   0        0        0    57565 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v5.acf
+-rw-r--r--   0        0        0    55553 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v6.acf
+-rw-r--r--   0        0        0     1258 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/README.md
+-rw-r--r--   0        0        0     2649 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/schema.json
+-rw-r--r--   0        0        0     2136 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/yao.yml
+-rw-r--r--   0        0        0     1062 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/exceptions.py
+-rw-r--r--   0        0        0    15317 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/mech_commands.py
+-rw-r--r--   0        0        0    19483 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/mech_controller.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sdss_yao-1.1.0/PKG-INFO
```

### Comparing `sdss_yao-1.0.0/LICENSE.md` & `sdss_yao-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.0.0/pyproject.toml` & `sdss_yao-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-yao"
-version = "1.0.0"
+version = "1.1.0"
 description = "BOSS spectrograph actor that uses an STA Archon controller"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Aidan Gray <Aidan.Gray@idg.jhu.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/yao"
 repository = "https://github.com/sdss/yao"
 documentation = "https://sdss-yao.readthedocs.org"
@@ -24,30 +24,27 @@
 ]
 include = ["yao/etc/*"]
 
 [tool.poetry.scripts]
 yao = "yao.__main__:yao"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
-sdss-archon = ">=0.6.0"
-sdsstools = ">=0.4.0"
-click = "^8.1.2"
+python = ">=3.9,<3.12"
+sdss-archon = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.0.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
 isort = ">=4.3.21"
-codecov = ">=2.0.15"
 coverage = {version = ">=5.0", extras = ["toml"]}
 ipdb = ">=0.12.3"
 rstcheck = ">=3.3.1"
 Sphinx = ">=3.0.0"
 black = ">=20.8b1"
 jedi = ">=0.17.2"
 sphinx-click = ">=2.6.0"
```

### Comparing `sdss_yao-1.0.0/yao/__main__.py` & `sdss_yao-1.1.0/yao/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.0.0/yao/actor.py` & `sdss_yao-1.1.0/yao/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,53 +18,59 @@
 from clu.legacy import LegacyActor
 
 from archon import log as archon_log
 from archon.actor.actor import ArchonBaseActor
 from archon.actor.tools import get_schema
 
 from yao import __version__, config
+from yao.alerts import AlertsBot
 from yao.commands import parser
+from yao.controller import YaoController
 from yao.delegate import YaoDelegate
 from yao.exceptions import YaoUserWarning
 from yao.mech_controller import MechController
 
 
 class YaoActor(ArchonBaseActor, LegacyActor):
     """Yao actor."""
 
     is_legacy = True
 
     DELEGATE_CLASS = YaoDelegate
+    CONTROLLER_CLASS = YaoController
+
     parser = parser
 
     def __init__(self, *args, **kwargs):
-
         self._message_processor = self._process_message
 
         schema = self.merge_schemas(kwargs.pop("schema", None))
 
         # We are going to append "spX_" to every keyword that contains the
         # controller sub-keyword, so for now let's accept additionalProperties.
         schema["additionalProperties"] = True
 
         super().__init__(*args, schema=schema, **kwargs)
 
         self.version = __version__
 
+        self.alerts_bot: AlertsBot | None = None
+
         # TODO: this assumes one single mech controller, not one per spectrograph,
         # but in practice for now that's fine.
         self.spec_mech = MechController(
             self.config["specMech"]["address"],
             self.config["specMech"]["port"],
         )
 
         # Add actor log handlers to the archon library to also get that logging.
         archon_log.addHandler(self.log.sh)
         if self.log.fh:
             archon_log.addHandler(self.log.fh)
+            self.log.fh.setLevel(10)
 
     async def start(self):
         """Starts the actor and connects the specMech client."""
 
         try:
             await self.spec_mech.start()
         except asyncio.TimeoutError:
@@ -74,15 +80,20 @@
             )
         except Exception as err:
             warnings.warn(
                 f"Failed connecting to mech controller: {err}",
                 YaoUserWarning,
             )
 
-        return await super().start()
+        new_self = await super().start()
+
+        if self.alerts_bot is None:
+            self.alerts_bot = AlertsBot(self)
+
+        return new_self
 
     def merge_schemas(self, yao_schema_path: str | None = None):
         """Merge default schema with the one from yao."""
 
         schema = get_schema()  # Default archon schema.
 
         if yao_schema_path:
```

### Comparing `sdss_yao-1.0.0/yao/delegate.py` & `sdss_yao-1.1.0/yao/delegate.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,57 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2022-04-13
 # @Filename: delegate.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+import asyncio
+
+from typing import TYPE_CHECKING, Any, List
 
 import numpy
 from astropy.io import fits
 from astropy.time import Time
 from clu.legacy.types.pvt import PVT
 
 from archon.actor.delegate import ExposureDelegate
 from archon.controller import ArchonController
 from sdsstools.time import get_sjd
 
 from .exceptions import SpecMechError
 
 
 if TYPE_CHECKING:
+    from clu.command import Command
+
     from yao.actor import YaoActor
+    from yao.controller import YaoController
 
 
 # TODO: LCOTCC cards are copied from flicamera. Should reunify code.
 
 
 class YaoDelegate(ExposureDelegate["YaoActor"]):
     """Exposure delegate for BOSS."""
 
+    def __init__(self, actor: YaoActor):
+        super().__init__(actor)
+
+        self.header_data = {}
+
+    async def pre_expose(self, controllers: List[YaoController]):
+        """Runs the e-purge routine before the exposure."""
+
+        self.command.info("E-purging and flushing.")
+
+        await asyncio.gather(*[controller.purge() for controller in controllers])
+
+        return True
+
     async def shutter(self, open: bool = False) -> bool:
         """Open/close the shutter."""
 
         expose_data = self.expose_data
         assert expose_data
 
         # TODO: this should be part of the ExposureDelegate.
@@ -50,14 +69,195 @@
             )
         except SpecMechError as err:
             self.command.error(f"Failed moving shutter: {err}")
             return False
 
         return True
 
+    async def readout(
+        self,
+        command: Command[YaoActor],
+        extra_header=...,
+        delay_readout: int = 0,
+        write: bool = True,
+    ):
+        """Reads detectors."""
+
+        # Finish exposure tasks.
+        try:
+            if self._expose_cotasks:
+                self.command.debug(text="Awaiting for exposure cotasks to finishing.")
+                await asyncio.wait_for(self._expose_cotasks, 10)
+        except asyncio.TimeoutError:
+            self.command.warning("Timed out running exposure cotasks.")
+
+        return await super().readout(command, extra_header, delay_readout, write)
+
+    async def expose_cotasks(self):
+        """Grab header information during exposure."""
+
+        self.command.debug(text="Starting exposure cotasks.")
+
+        self.header_data = {}
+
+        self.header_data["fps_cards"] = [
+            (
+                "CONFID",
+                get_keyword(
+                    self.actor,
+                    "jaeger",
+                    "configuration_loaded",
+                    idx=0,
+                    cnv=int,
+                ),
+                "Configuration ID",
+            ),
+            (
+                "DESIGNID",
+                get_keyword(
+                    self.actor,
+                    "jaeger",
+                    "configuration_loaded",
+                    idx=1,
+                    cnv=int,
+                ),
+                "Design ID associated with CONFIGID",
+            ),
+            (
+                "FIELDID",
+                get_keyword(
+                    self.actor,
+                    "jaeger",
+                    "configuration_loaded",
+                    idx=2,
+                    cnv=int,
+                ),
+                "Field ID associated with CONFIGID",
+            ),
+        ]
+
+        self.header_data["lcotcc_cards"] = get_lcotcc_cards(self.actor)
+
+        cherno_cards = []
+        for idx, card in enumerate(["OFFRA", "OFFDEC", "OFFPA"]):
+            default = get_keyword(
+                self.actor,
+                "cherno",
+                "default_offset",
+                idx=idx,
+                default=0.0,
+                cnv=float,
+            )
+            offset = get_keyword(
+                self.actor,
+                "cherno",
+                "offset",
+                idx=idx,
+                default=0.0,
+                cnv=float,
+            )
+            cherno_cards.append(
+                (
+                    card,
+                    default + offset,
+                    "Absolute guider offset in " + card.replace("OFF", ""),
+                )
+            )
+        cherno_cards.append(
+            (
+                "SEEING",
+                get_keyword(
+                    self.actor,
+                    "cherno",
+                    "astrometry_fit",
+                    idx=4,
+                    cnv=float,
+                ),
+                "Seeing from the guider [arcsec]",
+            )
+        )
+        self.header_data["cherno_cards"] = cherno_cards
+
+        lamp_cards = []
+        for lamp in ["FF", "Ne", "HeAr"]:
+            value = get_keyword(self.actor, "lcolamps", lamp, idx=0, default="?")
+            if value == "ON":
+                card_value = "1 1 1 1"
+            elif value == "OFF":
+                card_value = "0 0 0 0"
+            else:
+                card_value = "? ? ? ?"
+            lamp_cards.append((lamp.upper(), card_value, f"{lamp} lamps 1:On 0:Off"))
+        self.header_data["lamp_cards"] = lamp_cards
+
+        specmech_cards = []
+
+        status_left = await self.actor.spec_mech.pneumatic_status("left")
+        status_right = await self.actor.spec_mech.pneumatic_status("right")
+        if status_left == "closed" and status_right == "closed":
+            hartmann = "Left,Right"
+        elif status_left == "closed" and status_right == "open":
+            hartmann = "Left"
+        elif status_left == "open" and status_right == "closed":
+            hartmann = "Right"
+        elif status_left == "open" and status_right == "open":
+            hartmann = "Out"
+        else:
+            hartmann = "?"
+        specmech_cards.append(("HARTMANN", hartmann, "Hartmanns: Left,Right,Out"))
+
+        for motor in ["a", "b", "c"]:
+            _, pos, *_ = await self.actor.spec_mech.get_stat(f"motor-{motor}")
+            specmech_cards.append(
+                (
+                    f"COLL{motor.upper()}",
+                    int(pos),
+                    f"The position of the {motor.upper()} collimator motor",
+                )
+            )
+
+        # specMech data
+        ori = [-999, -999, -999]
+        try:
+            ori = await self.actor.spec_mech.get_stat("orientation")
+        except Exception as err:
+            self.command.warning(f"Cannot get specMech orientation: {err}")
+        finally:
+            for ii, axis in enumerate(["X", "Y", "Z"]):
+                specmech_cards.append(
+                    (
+                        f"MECHORI{axis}",
+                        ori[ii],
+                        f"Orientation in {axis} axis [cm/s2]",
+                    )
+                )
+
+        mech_env = [-999] * 7
+        try:
+            mech_env = await self.actor.spec_mech.get_stat("environment")
+        except Exception as err:
+            self.command.warning(f"Cannot get specMech environment: {err}")
+        finally:
+            for ii, (label, comment) in enumerate(
+                [
+                    ("B2CAMT", "B2 camera temperature [degC]"),
+                    ("B2CAMH", "B2 camera RH [%]"),
+                    ("R2CAMT", "R2 camera temperature [degC]"),
+                    ("R2CAMH", "R2 camera RH [%]"),
+                    ("COLLT", "Collimator temperature [degC]"),
+                    ("COLLH", "Collimator RH [%]"),
+                    ("SPECMT", "specMech temperature [degC]"),
+                ]
+            ):
+                specmech_cards.append((label, mech_env[ii], comment))
+
+        self.header_data["specmech_cards"] = specmech_cards
+
+        return await super().expose_cotasks()
+
     async def post_process(
         self,
         controller: ArchonController,
         hdus: list[fits.PrimaryHDU],
     ) -> tuple[ArchonController, list[fits.PrimaryHDU]]:
         """Post-process images and rearrange overscan regions."""
 
@@ -74,56 +274,60 @@
             assert isinstance(data, numpy.ndarray)
 
             ccd = hdu.header["CCD"]
             if ccd not in ["b2", "r2"]:
                 self.command.warning(text=f"Unknown CCD {ccd}.")
                 continue
 
-            if WIN_MODE != "hartmann":
-                OL = config["controllers"]["sp2"]["overscan_regions"][ccd]["lines"]
-                OL_END = -OL
-            else:
-                OL = 0
-                OL_END = None
+            # Decide whether we want to do some callisthenics with the data to move
+            # the overscan regions to the edges and to make things look exactly like
+            # at APO.
+            if config["controllers"]["sp2"].get("raw_mode", False) is False:
+                if WIN_MODE != "hartmann":
+                    OL = config["controllers"]["sp2"]["overscan_regions"][ccd]["lines"]
+                    OL_END = -OL
+                else:
+                    OL = 0
+                    OL_END = None
 
-            OP = config["controllers"]["sp2"]["overscan_regions"][ccd]["pixels"]
+                OP = config["controllers"]["sp2"]["overscan_regions"][ccd]["pixels"]
 
-            # Copy original data.
-            raw = data.copy()
+                # Copy original data.
+                rr = data.copy()
 
-            # Rearrange pixel overscan.
-            data[:, :OP] = raw[:, PIXELS - OP : PIXELS]
-            data[:, -OP:] = raw[:, PIXELS : PIXELS + OP]
-
-            # Rearrange line overscan.
-            if OL > 0:
-                data[:OL, OP:PIXELS] = raw[LINES - OL : LINES, : PIXELS - OP]  # BL
-                data[-OL:, OP:PIXELS] = raw[LINES : LINES + OL, : PIXELS - OP]  # TL
-                data[:OL, PIXELS:-OP] = raw[LINES - OL : LINES, PIXELS + OP :]  # BL
-                data[-OL:, PIXELS:-OP] = raw[LINES : LINES + OL, PIXELS + OP :]  # BR
-
-            # Rearrange data.
-            data[OL:LINES, OP:PIXELS] = raw[: LINES - OL, : PIXELS - OP]  # BL
-            data[LINES:OL_END, OP:PIXELS] = raw[LINES + OL :, : PIXELS - OP]  # TL
-            data[OL:LINES, PIXELS:-OP] = raw[: LINES - OL, PIXELS + OP :]  # BR
-            data[LINES:OL_END, PIXELS:-OP] = raw[LINES + OL :, PIXELS + OP :]  # TR
-
-            if WIN_MODE == "hartmann":
-                DEF_LINES = controller.default_window["lines"]
-                DEF_PIXELS = controller.default_window["pixels"]
-                new_data = numpy.zeros((DEF_LINES * 2, DEF_PIXELS * 2), dtype="u2")
+                # Rearrange pixel overscan.
+                data[:, :OP] = rr[:, PIXELS - OP : PIXELS]
+                data[:, -OP:] = rr[:, PIXELS : PIXELS + OP]
+
+                # Rearrange line overscan.
+                if OL > 0:
+                    data[:OL, OP:PIXELS] = rr[LINES - OL : LINES, : PIXELS - OP]  # BL
+                    data[-OL:, OP:PIXELS] = rr[LINES : LINES + OL, : PIXELS - OP]  # TL
+                    data[:OL, PIXELS:-OP] = rr[LINES - OL : LINES, PIXELS + OP :]  # BL
+                    data[-OL:, PIXELS:-OP] = rr[LINES : LINES + OL, PIXELS + OP :]  # BR
+
+                # Rearrange data.
+                data[OL:LINES, OP:PIXELS] = rr[: LINES - OL, : PIXELS - OP]  # BL
+                data[LINES:OL_END, OP:PIXELS] = rr[LINES + OL :, : PIXELS - OP]  # TL
+                data[OL:LINES, PIXELS:-OP] = rr[: LINES - OL, PIXELS + OP :]  # BR
+                data[LINES:OL_END, PIXELS:-OP] = rr[LINES + OL :, PIXELS + OP :]  # TR
+
+                if WIN_MODE == "hartmann":
+                    DEF_LINES = controller.default_window["lines"]
+                    DEF_PIXELS = controller.default_window["pixels"]
+                    new_data = numpy.zeros((DEF_LINES * 2, DEF_PIXELS * 2), dtype="u2")
 
-                PRELINES = controller.current_window["preskiplines"]
+                    PRELINES = controller.current_window["preskiplines"]
 
-                new_data[PRELINES : PRELINES + LINES, :] = data[:LINES, :]
-                new_data[-PRELINES - LINES : -PRELINES, :] = data[LINES:, :]
+                    new_data[PRELINES : PRELINES + LINES, :] = data[:LINES, :]
+                    new_data[-PRELINES - LINES : -PRELINES, :] = data[LINES:, :]
 
-                hdu.data = new_data
-            else:
-                hdu.data = data
+                    hdu.data = new_data
+                else:
+                    hdu.data = data
 
             # Rename some keywords and add others to match APO BOSS datamodel.
             header.insert("CCD", ("CAMERAS", header["CCD"]))
 
             header.rename_keyword("IMAGETYP", "FLAVOR")
             header.rename_keyword("OBSTIME", "DATE-OBS")
 
@@ -143,174 +347,41 @@
 
             reqtime_card = ("REQTIME", header["EXPTIME"], "Requested exposure time")
             header.insert("EXPTIME", reqtime_card)
 
             # Instrument cards
             header.append(("CARTID", "FPS-S", "Instrument ID"))
 
-            fps_cards = [
-                (
-                    "CONFID",
-                    get_keyword(
-                        self.actor,
-                        "jaeger",
-                        "configuration_loaded",
-                        idx=0,
-                        cnv=int,
-                    ),
-                    "Configuration ID",
-                ),
-                (
-                    "DESIGNID",
-                    get_keyword(
-                        self.actor,
-                        "jaeger",
-                        "configuration_loaded",
-                        idx=1,
-                        cnv=int,
-                    ),
-                    "Design ID associated with CONFIGID",
-                ),
-                (
-                    "FIELDID",
-                    get_keyword(
-                        self.actor,
-                        "jaeger",
-                        "configuration_loaded",
-                        idx=2,
-                        cnv=int,
-                    ),
-                    "Field ID associated with CONFIGID",
-                ),
-            ]
-            for card in fps_cards:
+            for card in self.header_data.get("fps_cards", []):
                 header.append(card)
 
             # TCC Cards
-            for card in get_lcotcc_cards(self.actor):
+            for card in self.header_data.get("lcotcc_cards", []):
                 header.append(card)
 
             # Cherno offset cards
-            for idx, card in enumerate(["OFFRA", "OFFDEC", "OFFPA"]):
-                default = get_keyword(
-                    self.actor,
-                    "cherno",
-                    "default_offset",
-                    idx=idx,
-                    default=0.0,
-                    cnv=float,
-                )
-                offset = get_keyword(
-                    self.actor,
-                    "cherno",
-                    "offset",
-                    idx=idx,
-                    default=0.0,
-                    cnv=float,
-                )
-                header.append(
-                    (
-                        card,
-                        default + offset,
-                        "Absolute guider offset in " + card.replace("OFF", ""),
-                    )
-                )
-            header.append(
-                (
-                    "SEEING",
-                    get_keyword(
-                        self.actor,
-                        "cherno",
-                        "astrometry_fit",
-                        idx=4,
-                        cnv=float,
-                    ),
-                    "Seeing from the guider [arcsec]",
-                )
-            )
+            for card in self.header_data.get("cherno_cards", []):
+                header.append(card)
 
             # Lamps
-            for lamp in ["FF", "Ne", "HeAr"]:
-                value = get_keyword(self.actor, "lcolamps", lamp, idx=0, default="?")
-                if value == "ON":
-                    card_value = "1 1 1 1"
-                elif value == "OFF":
-                    card_value = "0 0 0 0"
-                else:
-                    card_value = "? ? ? ?"
-                header.append((lamp.upper(), card_value, f"{lamp} lamps 1:On 0:Off"))
+            for card in self.header_data.get("lamp_cards", []):
+                header.append(card)
 
             # Hacking FFS and FF for now.
             if self.expose_data and self.expose_data.flavour == "flat":
                 header["FF"] = "1 1 1 1"
             if self.expose_data and self.expose_data.flavour in ["flat", "arc"]:
                 ffs_value = "1 1 1 1 1 1 1 1"
             else:
                 ffs_value = "0 0 0 0 0 0 0 0"
             header.append(("FFS", ffs_value, "FFS 0:Closed 1:Open"))
 
-            # Collimator and hartmann
-            status_left = await self.actor.spec_mech.pneumatic_status("left")
-            status_right = await self.actor.spec_mech.pneumatic_status("right")
-            if status_left == "closed" and status_right == "closed":
-                hartmann = "Left,Right"
-            elif status_left == "closed" and status_right == "open":
-                hartmann = "Left"
-            elif status_left == "open" and status_right == "closed":
-                hartmann = "Right"
-            elif status_left == "open" and status_right == "open":
-                hartmann = "Out"
-            else:
-                hartmann = "?"
-            header.append(("HARTMANN", hartmann, "Hartmanns: Left,Right,Out"))
-
-            for motor in ["a", "b", "c"]:
-                _, pos, *_ = await self.actor.spec_mech.get_stat(f"motor-{motor}")
-                header.append(
-                    (
-                        f"COLL{motor.upper()}",
-                        int(pos),
-                        f"The position of the {motor.upper()} collimator motor",
-                    )
-                )
-
-            # specMech data
-            ori = [-999, -999, -999]
-            try:
-                ori = await self.actor.spec_mech.get_stat("orientation")
-            except Exception as err:
-                self.command.warning(f"Cannot get specMech orientation: {err}")
-            finally:
-                for ii, axis in enumerate(["X", "Y", "Z"]):
-                    header.append(
-                        (
-                            f"MECHORI{axis}",
-                            ori[ii],
-                            f"Orientation in {axis} axis [cm/s2]",
-                        )
-                    )
-
-            mech_env = [-999] * 7
-            try:
-                mech_env = await self.actor.spec_mech.get_stat("environment")
-            except Exception as err:
-                self.command.warning(f"Cannot get specMech environment: {err}")
-            finally:
-                for ii, (label, comment) in enumerate(
-                    [
-                        ("B2CAMT", "B2 camera temperature [degC]"),
-                        ("B2CAMH", "B2 camera RH [%]"),
-                        ("R2CAMT", "R2 camera temperature [degC]"),
-                        ("R2CAMH", "R2 camera RH [%]"),
-                        ("COLLT", "Collimator temperature [degC]"),
-                        ("COLLH", "Collimator RH [%]"),
-                        ("SPECMT", "specMech temperature [degC]"),
-                    ]
-                ):
-                    header.append((label, mech_env[ii], comment))
+            # specMech
+            for card in self.header_data.get("specmech_cards", []):
+                header.append(card)
 
         return controller, hdus
 
 
 def pvt2pos(tup):
     pvt = PVT(*tup)
     return pvt.getPos()
@@ -334,14 +405,22 @@
 
     try:
         value = model[key].value
         if idx is not None:
             value = value[idx]
         if cnv:
             value = cnv(value)
+
+        # Headers cannot have NaN values as floats.
+        try:
+            if numpy.isnan(value):
+                value = "NaN"
+        except TypeError:
+            pass
+
         return value
     except BaseException:
         return default
 
 
 def get_lcotcc_cards(actor: YaoActor):
     """Return a list of cards describing the LCO TCC state."""
```

### Comparing `sdss_yao-1.0.0/yao/etc/BOSS_extra.acf` & `sdss_yao-1.1.0/yao/etc/BOSS_extra.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.0.0/yao/etc/schema.json` & `sdss_yao-1.1.0/yao/etc/schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878048780487806%*

 * *Differences: {"'properties'": "{'alive_at': OrderedDict([('type', 'number')]), 'b2_ccd_temp_alert': "*

 * *                 "OrderedDict([('type', 'integer')]), 'r2_ccd_temp_alert': OrderedDict([('type', "*

 * *                 "'integer')]), 'b2_ln2_temp_alert': OrderedDict([('type', 'integer')]), "*

 * *                 "'r2_ln2_temp_alert': OrderedDict([('type', 'integer')])}"}*

```diff
@@ -27,14 +27,23 @@
                 "type": "number"
             },
             "type": "array"
         },
         "air_pressure": {
             "type": "string"
         },
+        "alive_at": {
+            "type": "number"
+        },
+        "b2_ccd_temp_alert": {
+            "type": "integer"
+        },
+        "b2_ln2_temp_alert": {
+            "type": "integer"
+        },
         "blue_dewar_thermistor_status": {
             "enum": [
                 "cold",
                 "warm",
                 "?"
             ]
         },
@@ -127,14 +136,20 @@
                 "type": "integer"
             },
             "type": "array"
         },
         "power_supply_volts": {
             "type": "number"
         },
+        "r2_ccd_temp_alert": {
+            "type": "integer"
+        },
+        "r2_ln2_temp_alert": {
+            "type": "integer"
+        },
         "red_dewar_thermistor_status": {
             "enum": [
                 "cold",
                 "warm",
                 "?"
             ]
         },
```

### Comparing `sdss_yao-1.0.0/yao/etc/yao.yml` & `sdss_yao-1.1.0/yao/etc/yao.yml`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 enabled_controllers: [sp2]
 excluded_cameras: []
 
 controllers:
   sp2:
     host: 192.168.1.2
     port: 4242
+    raw_mode: false
     detectors:
       r2:
         taps: 4
         gain: 1.6
         readnoise: 10
       b2:
         taps: 4
@@ -70,21 +71,39 @@
 
 files:
   data_dir: '/data/spectro'
   use_sjd: true
   split: true
   template: 'sdR-{ccd}-{exposure_no:08d}.fit.gz'
 
+checksum:
+  write: true
+  mode: sha1
+
 archon:
-  acf_file: BOSS_extra.acf
+  acf_file: BOSS_extra_purge_erase_v6.acf
 
 timeouts:
   controller_connect: 5
   write_config_timeout: 2
   write_config_delay: 0.0001
   expose_timeout: 2
   readout_expected: 40
   readout_max: 60
   fetching_expected: 5
   fetching_max: 10
-  flushing: 1.2
+  flushing: 8.2
+  fast_flushing: 2.2
   pneumatics: 1.5
+  purge: 0.2
+
+alerts:
+  sp2:
+    ln2_base_temperature: -182.5
+    ln2_temperature_max_increase: 3
+    ccd_temperature_max_increase: 2.0
+    r2_ccd_status_param: mod2/tempa
+    b2_ccd_status_param: mod11/tempa
+    r2_ln2_status_param: mod2/tempb
+    b2_ln2_status_param: mod11/tempb
+    r2_setpoint_param: MOD2\HEATERATARGET
+    b2_setpoint_param: MOD11\HEATERATARGET
```

### Comparing `sdss_yao-1.0.0/yao/exceptions.py` & `sdss_yao-1.1.0/yao/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 
 class YaoError(Exception):
     """A custom core Yao exception"""
 
     def __init__(self, message=None):
-
         message = "There has been an error" if not message else message
         super(YaoError, self).__init__(message)
 
 
 class YaoNotImplemented(YaoError):
     """A custom exception for not yet implemented features."""
 
     def __init__(self, message=None):
-
         message = "This feature is not implemented yet." if not message else message
         super(YaoNotImplemented, self).__init__(message)
 
 
 class SpecMechError(YaoError):
     """A specMech error."""
```

### Comparing `sdss_yao-1.0.0/yao/mech_commands.py` & `sdss_yao-1.1.0/yao/mech_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 
     if debug:
         write_func = command.debug
     else:
         write_func = command.info
 
     for this_stat in process_stats:
-
         if this_stat not in STATS:
             return command.fail(f"Invalid specMech status command {this_stat!r}.")
 
         mech = command.actor.spec_mech
 
         try:
             values = await mech.get_stat(this_stat)
```

### Comparing `sdss_yao-1.0.0/yao/mech_controller.py` & `sdss_yao-1.1.0/yao/mech_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     CONNECTION_FAILED = enum.auto()
 
 
 class SpecMechReply:
     """A valid response to a command to the specMech."""
 
     def __init__(self, raw: bytes):
-
         self.command_id = 0
         self.raw = raw
 
         self.code = ReplyCode.VALID
 
         self.reply_sentence: str = ""
         self.data: list[list[str]] = []
@@ -230,15 +229,14 @@
         The port of the host of the mech server.
     log
         A logger to which to write.
 
     """
 
     def __init__(self, address: str, port: int = 23, log: SDSSLogger | None = None):
-
         self.reader: asyncio.StreamReader | None = None
         self.writer: asyncio.StreamWriter | None = None
 
         self.reboot: bool = False
         self.command_number: int = 0
 
         self.log = log or SDSSLogger("boss-spech-mech-client")
@@ -576,15 +574,14 @@
         reply = await self.send_data(spec_command)
         check_reply(reply)
 
         # Check that all the mechanisms have arrived to their desired position.
         # Try twice, then fail.
 
         for ii in [1, 2]:
-
             await asyncio.sleep(config["timeouts"]["pneumatics"])
 
             reached = True
 
             status = await self.send_data("rp")
             try:
                 check_reply(status)
```

### Comparing `sdss_yao-1.0.0/PKG-INFO` & `sdss_yao-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: sdss-yao
-Version: 1.0.0
+Version: 1.1.0
 Summary: BOSS spectrograph actor that uses an STA Archon controller
 Home-page: https://github.com/sdss/yao
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: click (>=8.1.2,<9.0.0)
-Requires-Dist: sdss-archon (>=0.6.0)
-Requires-Dist: sdsstools (>=0.4.0)
+Requires-Dist: sdss-archon (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://sdss-yao.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/yao
 Description-Content-Type: text/markdown
 
 # yao
 
 ![Versions](https://img.shields.io/badge/python->3.9-blue)
```

