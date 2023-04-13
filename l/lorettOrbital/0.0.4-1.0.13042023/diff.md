# Comparing `tmp/lorettOrbital-0.0.4.tar.gz` & `tmp/lorettOrbital-1.0.13042023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorettOrbital-0.0.4.tar", last modified: Sat Apr  2 13:35:19 2022, max compression
+gzip compressed data, was "lorettOrbital-1.0.13042023.tar", last modified: Thu Apr 13 02:59:43 2023, max compression
```

## Comparing `lorettOrbital-0.0.4.tar` & `lorettOrbital-1.0.13042023.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-02 13:35:19.125820 lorettOrbital-0.0.4/
--rwxrwxrwx   0 root         (0) root         (0)     1086 2021-09-19 18:38:20.000000 lorettOrbital-0.0.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      637 2022-04-02 13:35:19.125342 lorettOrbital-0.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      146 2021-09-19 18:38:20.000000 lorettOrbital-0.0.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-02 13:35:19.121239 lorettOrbital-0.0.4/lorettOrbital/
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-04-02 13:21:20.000000 lorettOrbital-0.0.4/lorettOrbital/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      971 2022-03-10 20:42:04.000000 lorettOrbital-0.0.4/lorettOrbital/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)    26022 2022-04-02 13:18:19.000000 lorettOrbital-0.0.4/lorettOrbital/orbital.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-04-02 13:35:19.124538 lorettOrbital-0.0.4/lorettOrbital.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      637 2022-04-02 13:35:18.000000 lorettOrbital-0.0.4/lorettOrbital.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      289 2022-04-02 13:35:18.000000 lorettOrbital-0.0.4/lorettOrbital.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-04-02 13:35:18.000000 lorettOrbital-0.0.4/lorettOrbital.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       94 2022-04-02 13:35:18.000000 lorettOrbital-0.0.4/lorettOrbital.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2022-04-02 13:35:18.000000 lorettOrbital-0.0.4/lorettOrbital.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2022-04-02 13:35:19.126014 lorettOrbital-0.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      854 2022-04-02 11:18:14.000000 lorettOrbital-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.432335 lorettOrbital-1.0.13042023/
+-rw-rw-rw-   0        0        0     1086 2022-06-25 18:31:46.000000 lorettOrbital-1.0.13042023/LICENSE
+-rw-rw-rw-   0        0        0      649 2023-04-13 02:59:43.431335 lorettOrbital-1.0.13042023/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2022-06-25 18:31:46.000000 lorettOrbital-1.0.13042023/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.414337 lorettOrbital-1.0.13042023/lorettOrbital/
+-rw-rw-rw-   0        0        0      636 2023-04-13 02:57:40.000000 lorettOrbital-1.0.13042023/lorettOrbital/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.423336 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/
+-rw-rw-rw-   0        0        0      337 2023-03-23 04:11:03.000000 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      971 2022-07-16 19:16:18.000000 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/exceptions.py
+-rw-rw-rw-   0        0        0     8951 2022-12-02 21:46:20.000000 lorettOrbital-1.0.13042023/lorettOrbital/orbital.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.426341 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/
+-rw-rw-rw-   0        0        0      595 2023-03-23 04:24:14.000000 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/__init__.py
+-rw-rw-rw-   0        0        0    29209 2023-04-13 02:28:56.000000 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.429337 lorettOrbital-1.0.13042023/lorettOrbital/tests/
+-rw-rw-rw-   0        0        0      411 2023-03-23 04:30:24.000000 lorettOrbital-1.0.13042023/lorettOrbital/tests/SchedulerUnitTest.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 03:01:19.000000 lorettOrbital-1.0.13042023/lorettOrbital/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.420341 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 02:59:43.433338 lorettOrbital-1.0.13042023/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-03-23 03:15:31.000000 lorettOrbital-1.0.13042023/setup.py
```

### Comparing `lorettOrbital-0.0.4/LICENSE` & `lorettOrbital-1.0.13042023/LICENSE`

 * *Files identical despite different names*

### Comparing `lorettOrbital-0.0.4/lorettOrbital/exceptions.py` & `lorettOrbital-1.0.13042023/lorettOrbital/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `lorettOrbital-0.0.4/lorettOrbital/orbital.py` & `lorettOrbital-1.0.13042023/lorettOrbital/scheduler/scheduler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,392 +1,509 @@
-import matplotlib.pyplot as plt
+##
+# @file scheduler.py
+#
+# @brief A group of classes describing interaction with satellites. TLE, orbital position and schedule.
+#
+# @section schedulerDependencies Libraries/Modules
+# - datetime standart library (https://docs.python.org/3/library/datetime.html)
+#   - Access to datetime and timedelta classes.
+#
+# - math standart library (https://docs.python.org/3/library/math.html)
+#   - Access to radians, tan, sin and cos functions.
+#
+# - pathlib standart library (https://docs.python.org/3/library/pathlib.html)
+#   - Access to Path class.
+#
+# - typing standart library (https://docs.python.org/3/library/typing.html)
+#   - Access to List, Tuple, Any and Callable class.
+#
+# - dataclasses standart library (https://docs.python.org/3/library/dataclasses.html)
+#   - Access to dataclass decorator and field function.
+#
+# - pyorbital library (https://pypi.org/project/pyorbital/)
+#   - Access to Orbital and tlefile classes.
+#
+# - prettytable library (https://pypi.org/project/prettytable/)
+#   - Access to the PrettyTable class for beautiful schedule formatting.
+#
+# - verboselogs library (https://pypi.org/project/verboselogs/)
+#   - Access to VerboseLogger class.
+#
+# - requests library (https://pypi.org/project/requests/)
+#   - Access to get function and exceptions.
+#
+# - exceptions module (local)
+#   - Access to lorettOrbital exceptions classes.
+#
+# @section todo TODO
+# - Adaptation of pyephem to the pyorbital style.
+#
+# @section autor Author(s)
+# - Created by MrFentazis on 23/03/2023.
+#
 
-from pyorbital.orbital import Orbital
+
+# Impors
+from pyorbital.orbital import Orbital, tlefile
 from datetime import datetime, timedelta
 from math import radians, tan, sin, cos
-from numpy import arange, float32, float64, abs
 from prettytable import PrettyTable
-
-from os.path import join
 from pathlib import Path
+#!!!
 
-from logging import Logger
+from verboselogs import VerboseLogger
+from lorettOrbital.exceptions import *
 
-###
 from requests import get, exceptions
-from bs4 import BeautifulSoup as bs
-
-from .exceptions import *
-
-# TODO Проверка вменяемости конфига
-# TODO сделать отрисовку пролетов не только для станций с перемещением облучателя в факальной плоскости 
-
-__all__ = [
-    "Scheduler",
-    "satListLband",
-    "satListAPTBand",
-    "supportedStationTypes",
-    "__version__"
-]
-
-__version__ = "0.0.4"
-
-satListLband = ["NOAA 18",
-                "NOAA 19",
-                "METEOR-M 2",
-                "METEOR-M2 2",
-                "METOP-B",
-                "METOP-C",
-                "FENGYUN 3C"]
-                
-satListAPTBand = ["NOAA 15",
-                  "NOAA 18",
-                  "NOAA 19",
-                  "METEOR-M 2"]
-
-supportedStationTypes = {
-                        'l2s': {
-                                    'kinematic': 'focal',
-                                    'band': 'L',
-                                    'satList': satListLband,
-                                    'sampleRate': 6e6,
-                                    'horizon': 55,
-                                    'minApogee': 65,
-                                    'focus': 0.77,
-                                    'radius': 0.55
-                                },
-                         'c4s': {
-                                    'kinematic': 'focal',
-                                    'band': 'L',
-                                    'satList': satListLband,
-                                    'sampleRate': 6e6,
-                                    'horizon': 55,
-                                    'minApogee': 65,
-                                    'focus': 0.77,
-                                    'radius': 0.55
-                                },
-                         'r8s': {
-                                    'kinematic': 'rotate',
-                                    'band': 'L',
-                                    'satList': satListLband,
-                                    'sampleRate': 6e6,
-                                    'horizon': 15,
-                                    'minApogee': 35
-                                },
-                         'apt': {
-                                    'kinematic': 'apt',
-                                    'band': 'apt',
-                                    'satList': satListAPTBand,
-                                    'sampleRate': 11025,
-                                    'horizon': 15,
-                                    'minApogee': 20
-                                }
-                        }
-
-
-'''Класс для работы с расписанием и траекториями спутников'''
-class Scheduler():
-    '''
-    A class for working with the schedule and trajectories of satellites    
-
-    In:
-        str stationName
+from typing import List, Tuple, Any, Callable
 
-        float lon
+from dataclasses import dataclass, field
 
-        float lat
+# Global Constants
+## Station types list; rotator - classic azimuth and elevation systems; legacy - minutes:seconds special type for V. Rosental lorett systems.
+stationTypes = [
+                "rotator",
+                "legacy" # for Rosental systems
+                ]
+
+## Satellite TLE sources list.
+sources = {
+    "default": ["https://celestrak.com/NORAD/elements/active.txt"],
+    "weather": ["https://celestrak.org/NORAD/elements/weather.txt"]
+}
+
+## List of active satellites by communication bands
+satLists = {
+    ### Actual X-band satellites list.
+    "X": [
+            "TERRA",
+            "AQUA",
+            "HAISI 1",
+            "NOAA 20",
+            "NOAA 21 (JPSS-2)",
+            "SUOMI NPP",
+            "FENGYUN 3E",
+            "FENGYUN 3D",
+            "2022-019J",
+            #"EOS-6 (OCEANSAT-3)", # It has both a transmitter and equipment and the frequency is known, but it seems to transmit data only over certain territories.
+            #"ARKTIKA-M 1", # No info
+    ],
+    
+    ### Actual L-band HRPT satellites list.
+    "L": [
+            "NOAA 18",
+            "NOAA 19",
+            "METEOR-M 2",
+            "METEOR-M2 2",
+            "METOP-B",
+            "METOP-C",
+            #"ARKTIKA-M 1", # It has a transmitter and the necessary equipment, but it doesn't seem to be working at the moment
+    ],
+    
+    ### Actual APT-band satellites list.
+    "APT": [
+           "NOAA 15",
+            "NOAA 18",
+            "NOAA 19",
+            "METEOR-M 2" 
+    ]
+}
+
+# Classes
+@dataclass
+class SchedulerConfig:
+    """The class for contain data of station config
+        dataclass that defines the settings of the Scheduler object
+        
+            @param stationName: str
+            @param lat: float
+            @param lon: float
+            @param alt: float in kilometers
+            @param satList: dict = satListLBand
+            @param sampleRate: int = 6e6
+            @param horizon: int = 10
+            @param minApogee: int = 30
+   
+            @param path: str = '.'
+            @param timeZone: int = 0
+            
+    """    
+    stationName: str
+    lat: float
+    lon: float
+    alt: float
+    
+    source: Any = field(default_factory= lambda: sources["default"]) # List or str
+    satList: list = field(default_factory= lambda: satLists["L"])
+    stationType: str = field(default_factory= lambda: stationTypes[0])
+    horizon: int = 10
+    minApogee: int = 30
+    
+    path: str = '.'
+    timeZone: int = 0
+    
 
-        float alt
+@dataclass
+class SatPass:
+    """The class for contain data of sat pass
+        dataclass describing a certain flight of the satellite over the observer.
+            @param satName: str
+            @param orb: Orbital
+            @param culmination: float
+            @param timeStart: datetime
+            @param timeEnd: datetime
+            @param timeCulmination: datetime
+            @param status: str
+    """
+    satName: str
+    orb: Orbital
+    culmination: float
+    timeStart: datetime
+    timeEnd: datetime
+    timeCulmination: datetime
+    status: str = "wait"
+    
+    def __str__(self) -> str:
+        return f"""SatPass(satName={self.satName}, culmination={round(self.culmination, 2)}, timeStart={self.timeStart.strftime("%d.%m.%Y")}, timeEnd={self.timeEnd.strftime("%d.%m.%Y")}, timeCulmination={self.timeCulmination.strftime("%d.%m.%Y")})"""
 
-        str path
 
-        str stationType
+@dataclass
+class TrackFile:
+    """The class for contain data of trackFile
+        dataclass describing the exported trajectory file
+            @param satName: str
+            @param timeStart: datetime
+            @param trackPath: Path
+    """
+    satName: str
+    timeStart: datetime
+    trackPath: Path
+
+
+@dataclass
+class SphereCoordinates:
+    """The class for contain pair sphere coordinates 
+        dataclass describing a point in spherical coordinates.
+            @param azimuth: float
+            @param elevation: float
+            @param time: datetime
+    """
+    azimuth: float
+    elevation: float
+    time: datetime
+    
+    
+@dataclass
+class SphereAltCoordinates:
+    """The class for contain pair sphere alternative coordinates 
+        dataclass describing a point in alternative spherical coordinates. Uses Degrees:Minutes as a string.
+            @param azimuth: str
+            @param elevation: str
+            @param time: datetime
+    """
+    azimuth: str
+    elevation: str
+    time: datetime
+    
+    
+@dataclass
+class XYCoordinates:
+    """The class for contain pair XY coordinates
+        dataclass describing a point in XY coordinates. 
+    
+            @param x: float
+            @param y: float
+    """
+    x: float
+    y: float
+    time: datetime
+    
 
-        int timeZone
 
-        float azimuthCorrection
+class Scheduler:
+    '''
+        The Scheduler class for working with the schedule and trajectories of satellites    
     '''
 
-    def __init__(self, stationName: str,
-                 lat: float = 0,
-                 lon: float = 0,
-                 alt: float = 0,
-                 path: str = '',
-                 stationType: str = '',
-                 timeZone: int = 0,
-                 azimuthCorrection: float = 0,
-                 config: dict = {}
+    def __init__(self, 
+                 config: SchedulerConfig,
+                 logger: VerboseLogger = None
                  ) -> None:
+        
+        """ The Scheduler class initilisazer
+        
+        @param config: StationConfig
+        @param logger: VerboseLogger = None
+        
+        @return An instance of the Scheduler class initialized with the specified name.
+        
+        """
 
-        # определение типа станции по названию
-        if stationType != '':
-            if stationType.lower() in supportedStationTypes.keys():
-                self.stationType = stationType.lower()
-            else:
-                raise UnknownStationType(stationType)
-
-        else:
-            for type in supportedStationTypes.keys():
-                if type in stationName.lower():
-                    self.stationType = type
-                    break
+        self.logger: VerboseLogger = logger
+        
+        ## Check of sources
+        ## TODO fix multisources mode
+        if isinstance(config.source, str):
+            
+            ## if it is name of source from sources list
+            if config.source in sources.keys():
+                config.source = sources[config.source]
+            
             else:
-                raise UnknownStationType(type)
-
-        if len(config):
-            # 'apt' contains the minimum required list of parameters
-            if all([x in supportedStationTypes['apt'].keys() for x in config.keys()]):
-                self.stationType = 'castom'
+                if self.logger != None:
+                    self.logger.warning(f'Unknown source "{config.source}", use default')
+                    config.source = sources['default']
+        
+        self.config: SchedulerConfig = config
 
-            self.config = config
+        self.satList: list = self.config.satList
+        self.horizon: int = self.config.horizon
+        self.minApogee: int = self.config.minApogee
+        self.path = config.path
+        
+        ## Check station type
+        if self.config.stationType not in stationTypes:
+            if self.logger != None:
+                self.logger.warning(f'Unexpected stationType "{self.config.stationType}", use default')
+            
+            self.config.stationType = stationTypes[0]
             
-        else:
-            self.config = supportedStationTypes[self.stationType]
+        self.stationType: str = self.config.stationType
 
+        ## alt <= 9km - most higest earth place
+        if not all([(abs(self.config.lon) <= 180, abs(self.config.lat) <= 90), self.config.alt <= 9]):
+            raise InvalidCoordinates
         
-        self.lon = round(lon, 5)
-        self.lat = round(lat, 5)
-        self.alt = round(alt, 5)
+        self.lon = round(self.config.lon, 5)
+        self.lat = round(self.config.lat, 5)
+        self.alt = round(self.config.alt, 5)
 
-        self.timeZone = timeZone
-        self.stationName = stationName
+        self.timeZone = self.config.timeZone
+        self.stationName = self.config.stationName
 
-        self.azimuthCorrection = azimuthCorrection
-        
-        self.mirrorCircleColor = '#66ccff'
+        if self.path == ".":
+            self.path = Path.cwd()
 
-        self.path = path
+        self.path = Path(self.path)
 
         self._createSubDirectories()
-
-
-    '''Сервисный метод для получения количества дней с начала года'''
-    def _getDays(self, date: datetime) -> int:
-        '''
-        Service method for getting the number of days since the beginning of the year
-
-        In:
-            datetime date
-
-        Out:
-            int data
-        '''
-        daysForMonth = [
-            0,
-            31,     # January
-            59,     # February
-            90,     # March
-            120,    # April
-            151,    # May
-            181,    # June
-            212,    # July
-            243,    # August
-            273,    # September
-            304,    # October
-            334,    # November
-            365     # December
-        ]
-
-        days = date.day
-        days += daysForMonth[date.month-1]
-
-        return days
-
-
-    '''Сервисный медод для проверки координат'''
-    def _checkCoordinates(self) -> None:
-        """
-        Service method for checking coordinates
-        """
-        if not all((self.lon, self.lat, self.alt)):
-            raise CoordinatesAreNotGiven(self.lon, self.lat, self.alt)
-
-        if any((abs(self.lon) > 90, abs(self.lat) > 90)):
-            raise InvalidCoordinates
+        
+        self.update()
 
     
-    '''Сервисный метод для создания дополнительных директорий'''
     def _createSubDirectories(self) -> None:
+        """ The Service method for creating additional directories in path
         """
-        Service method for creating additional directories
-        """
-
-        self.tlePath = join( self.path, "tle" )
-        Path( self.tlePath ).mkdir(parents=True, exist_ok=True)
 
-        self.tracksPath = join( self.path, "tracks" )
-        Path( self.tracksPath ).mkdir(parents=True, exist_ok=True)
-
-        self.tracksSchemesPath = join( self.path, "tracksSchemes" )
-        Path( self.tracksSchemesPath ).mkdir(parents=True, exist_ok=True)
-
-        self.schedulePath = join( self.path, "schedule" )
-        Path( self.schedulePath ).mkdir(parents=True, exist_ok=True)
+        self.tlePath = self.path / "tle" 
+        
+        if not self.tlePath.exists():
+            if self.logger != None:
+                self.logger.info("Create tle subdirectory")
+            self.tlePath.mkdir(parents=True, exist_ok=True)
 
+        
+        self.tracksPath = self.path / "tracks" 
+        
+        if not self.tracksPath.exists():
+            if self.logger != None:
+                self.logger.info("Create tracks subdirectory")
+            self.tracksPath.mkdir(parents=True, exist_ok=True)
 
-    '''Сервисный метод для перевода из сферичиских координат в декартовы'''
-    def sphericalToDecart(self, azimuth: float, elevation: float) -> tuple:
-        """
-        Service method for translation from spherical coordinates to Cartesian coordinates
 
-        In:
-                float azimuth
+        self.schedulePath = self.path / "schedule"
+        
+        if not self.schedulePath.exists():
+            if self.logger != None:
+                self.logger.info("Create schedule subdirectory")
+            self.schedulePath.mkdir(parents=True, exist_ok=True)
 
-                float elevation
-        Out:
-                float x
 
-                float y
+    def sphericalToDecart(self, azimuth: float, elevation: float, time: datetime, convert: Callable[[float, float], list[float, float]]) -> XYCoordinates:
+        """ The service method for converting from spherical coordinates to custom X Y coordinates using a custom function
+            
+        @param azimuth: float
+        @param elevation: float
+        
+        @return coordinates: XYCoordinates
         """
 
-        if elevation == 90:
-            return 0, 0
+        #if elevation == 90:
+        #    return 0, 0
 
         azimuth = radians((azimuth + self.azimuthCorrection) % 360)
         elevation = radians(elevation)
 
-        y = -(self.config['focus'] / tan(elevation)) * cos(azimuth)
-        x = -(self.config['focus'] / tan(elevation)) * sin(azimuth)
-
-        return x, y
-
+        x, y = convert(azimuth, elevation)
+        
+        return XYCoordinates(x=x, y=y)
     
-    '''Метод который преобразует угловые координаты в форму градусы:минуты (a, e) --> (a:m, e:m)'''
-    def degreesToDegreesAndMinutes(self, azimuth: float, elevation: float) -> tuple:
-        """
-        Method that translates angular coordinates to the form degrees:minutes (a, e) --> (a:m, e:m)
+        #return XYCoordinates(y=-(self.config.focus / tan(elevation)) * cos(azimuth),
+        #                     x=-(self.config.focus / tan(elevation)) * sin(azimuth), time=time)
 
-        In:
-                float azimuth (градусы)
-
-                float elevation (градусы)
-        Out:
-                str azimuth (минуты)
+    
+    def degreesToDegreesAndMinutes(self, azimuth: float, elevation: float, time: datetime) -> SphereAltCoordinates:
+        """ The method that translates angular coordinates to the form degrees:minutes (a, e) --> SphereAltCoordinates(a:m, e:m)
 
-                str elevation (минуты)
+        @param azimuth: float (degree)
+        @param elevation: float (degree)
+        
+        @return coordinates: SphereAltCoordinates
+        
         """
-        typeAz = type(azimuth)
-        if typeAz == float or typeAz == float32 or typeAz == float64:
+        azimuthM = '000:00'
+        elevationM = '000:00'
+        
+        if isinstance(azimuth, (float, int)):
             minutes = azimuth * 60
             degrees = minutes // 60
             minutes %= 60
 
             azimuthM = f"{int(degrees):03}:{int(minutes):02}"
-
-        elif typeAz == int:
-            azimuthM = f"{azimuth:03}:00"
-
-        else:
-            return False
-
-        typeEl = type(elevation)
-        if typeEl == float or typeEl == float32 or typeEl == float64:
+            
+        if isinstance(elevation, (float, int)):
             minutes = elevation * 60
             degrees = minutes // 60
             minutes %= 60
 
             elevationM = f"{int(degrees):03}:{int(minutes):02}"
 
-        elif typeEl == int:
-            elevationM = f"{elevation:03}:00"
-
-        else:
-            return False
-
-        return azimuthM, elevationM
+        return SphereAltCoordinates(azimuth=azimuthM, elevation=elevationM, time=time)
 
     
-    '''Метод для обновления TLE файлов'''
     def update(self) -> bool:
+        """ The method that updates TLE files
+        
+        @return status: bool
         """
-        Method that updates TLE files
-
-        In:
-                bool showLog
-        """
-
-        name = join(self.path, "tle", "tle.txt")
+        if self.logger != None:
+            self.logger.info("Check update TLE")
+            
+        tleFile = self.tlePath / "tle.txt"
         now = datetime.utcnow()
         
         try:
-            with open(name, "r") as file:
-                yearInTLE, daysPassInTLE = map(int, file.readline().strip().split(' '))
-        except:
-            yearInTLE = now.year
-            daysPassInTLE = 0
-
-        if (yearInTLE == now.year) and (self._getDays(now) - daysPassInTLE <= 5):
-            return True
-
-        try:
-            page = get("http://celestrak.com/NORAD/elements/")
-            html = bs(page.content, "html.parser")
-            now = datetime.utcnow()
-
-            # Getting TLE date with server
             try:
-                year = int(html.select('h3.center')[0].text.split(' ')[3])
-                dayPass = int(html.select('h3.center')[
-                              0].text.replace(')', '').rsplit(' ', 1)[1])
-
-            except:
-                year = now.year
-                dayPass = 0
-                daysPassInTLE = 0
-
-            # if TLE is outdated then update TLE
-            if (yearInTLE < year) or ((yearInTLE == year) and (daysPassInTLE < dayPass)):
-
-                with open(name, "wb") as file:
-                    file.write(
-                        f"{now.year} {self._getDays(now)}\n".encode('utf-8'))
-                    file.write(
-                        get("http://www.celestrak.com/NORAD/elements/weather.txt").content)
-
-        except exceptions.ConnectionError:
-            #print('Error when update TLE')
-            #print("No internet connection\n")
-            return False
+                if tleFile.exists():
+                    with open(tleFile, "r") as file:
+                        lines = file.readlines()
+                        dateTLE = datetime.strptime(lines[1].strip(), "# %Y%m%d %H%M%S")
+
+                        ## Check old tles
+                        oldSats = []
+                        for i in range(2, len(lines), 3):
+                            name = lines[i].strip()
+                                
+                            if len(lines) - i > 3:
+                                try:
+                                    line1 = lines[i+1].strip()
+                                    line2 = lines[i+2].strip()
+                                    tlefile.Tle(platform=name, line1=line1, line2=line2)
+                                    oldSats.append(name)
+                                        
+                                except tlefile.ChecksumError:
+                                    if self.logger != None:
+                                        self.logger.info("Found bad TLE")
+                                        self.logger.verbose(f"Found bad TLE name: {name}")
+                                    continue
+                            
+                        ## If all satellites are found in the file and it is relevant
+                        if all(i in oldSats for i in self.satList) and (now - dateTLE < timedelta(days=1)):
+                            if self.logger != None:
+                                self.logger.info("Use actual TLE")
+                            return True
+                            
+                else:
+                    oldSats = []
+            
+            except ValueError as e:
+                self.logger.warning(f"Found bad tle data in {tleFile}")
+                
+            content = ""
+            newSats = []
+            for i in self.config.source:
+                tle = get(i)
+
+                if tle.status_code == 200:
+                    lines = tle.text.split("\n")
+                    for i in range(0, len(lines), 3):
+                        name = lines[i].strip()
+                            
+                        if len(lines) - i > 3:
+                            try:
+                                line1 = lines[i+1].strip()
+                                line2 = lines[i+2].strip()
+                                tlefile.Tle(platform=name, line1=line1, line2=line2)
+                                newSats.append(name)
+                                content += f"{name}\n{line1}\n{line2}\n"
+                                    
+                            except (tlefile.ChecksumError, IndexError):
+                                if self.logger != None:
+                                    self.logger.info(f"Found bad TLE for {name}. skip")
+                                continue
+                    
+                else:
+                    if self.logger != None:
+                        self.logger.warning(f"Connection failed code {tle.status_code}")
+            
+            ## if it was possible to get the tle of all the necessary satellites
+            if all(i in newSats for i in self.satList):
+                with open(tleFile, "w") as file:
+                    ## dont remove this line, stupid pyorbital 
+                    ## does not perceive comments in TLE and breaks down
+                    file.write("# Autoupdated tle\n")
+                    
+                    file.write( now.strftime("# %Y%m%d %H%M%S\n"))
+                    file.write(content)
+
+                if self.logger != None:
+                    self.logger.info("TLE updated")
+
+                return True
+
+            if content == "" and self.logger != None:
+                self.logger.warning("Failed update TLE")
+
+            ## the update failed, but the old file has all the satellites
+            if content == "" and all(i in oldSats for i in self.config.satList) and self.logger != None:
+                self.logger.warning(f"Use old TLE {dateTLE}")
+                return False
+                
+            else:
+                if self.logger != None:
+                    self.logger.error(f"Failed to get TLE. exit")
+                    
 
+            return True
+                    
         except Exception as e:
-            #print('Error when update TLE')
-            #print(str(e), "\n")
-            return False
-
-        return True
+            if self.logger != None:
+                self.logger.info(f"Exception in Scheduler.update {repr(e)}")
+                self.logger.verbose(f"Exception message: {e}")
 
+            return False
+        
 
-    '''Метод для получения координат станции по ip-адресу.'''
-    def getCoordinatesByIp(self) -> tuple:
-        """
-        Method that gets the station coordinates by his ip.
+    @staticmethod
+    def getCoordinatesByIp() -> Tuple[float, float, float]:
+        """ The method that gets the station coordinates by his ip.
 
-        Returned Altitude in kilometers.\n\n
+        Returned Altitude in kilometers.
 
         ATTENTION!
 
         THESE COORDINATES MAY BE VERY INACCURATE.
 
         USE IT ONLY FOR MAKING AN APPROXIMATE SCHEDULE.\n\n
 
 
-        Out:
-                float lon
-
-                float lat
-
-                float alt
-
-
-        If there is an error:
-                float lon=None
+        @return list[lon: float, lat: float, alt: float]
 
-                float lat=None
 
-                float alt=None
+        If there is an error: lon = 0; lat = 0; alt = 0
 
         """
 
         try:
             query = get("http://ip-api.com/json").json()
 
             lon = query['lon']
@@ -410,427 +527,316 @@
             return 0, 0, 0
 
         alt /= 1000
 
         return lon, lat, alt
 
 
-    '''Метод который вычисляет проходы спутника по входным параметрам'''
-    def getSatellitePasses(self, start: datetime, length: int, satellite: str, tol: float = 0.001, updateTLE: bool = True) -> list:
-        """
-        Method that calculates satellite passes by input parametres
-
-        In:
-                str satellite
-
-                datetime start
-
-                int length
+    def getSatellitePasses(self, start: datetime, length: int, satellite: str, tol: float = 0.001, updateTLE: bool = False) -> Tuple[Orbital, List[datetime]]:
+        """ The method that calculates satellite passes by input parametres
 
-                float tol
+        @param satellite: str
+        @param start: datetime
+        @param length: int
+        @param tol: float
+        @param updateTLE: bool
 
-                bool updateTLE
-
-        Out:
-                datetime start, datetime end, datetime apogee
+        @return passes: list[Orbital, list[datetime, datetime, datetime]]
+        
         """
 
-        self._checkCoordinates()
-
         if updateTLE:
             self.update()
 
-        orb = Orbital(satellite, join( self.tlePath, "tle.txt" ) )
-
-        return orb.get_next_passes(start, length, self.lon, self.lat, self.alt, tol, self.config['horizon'])
-
-
-    '''Метод который составляет расписание в соответствии с параметрами'''
-    def getSchedule(self, length: int, tol: float = 0.001, saveSchedule: bool = False, returnTable: bool = False, returnNameSatellite: bool = False, updateTLE: bool = True) -> PrettyTable:
-        """
-        Method that makes up the schedule, according to the parameters.
-
-        In:
-
-                int length
-
-                float tol
-
-                bool printTable
+        orb = Orbital(satellite, tle_file=str(self.tlePath / "tle.txt") )
 
-                bool saveSchedule
+        return orb, orb.get_next_passes(start, length, self.lon, self.lat, self.alt, tol, self.horizon)
 
-                bool returnTable
 
-                bool returnNameSatellite
-
-                bool updateTLE
-
-        Out:
-                str table or list passesForReturn or list massout
+    def getSchedule(self, timeStart: datetime, length: int, saveSchedule: bool=False, updateTLE: bool=False) -> List[SatPass]:
+        """ The method that makes up the schedule, according to the parameters.
+        
+        It does not take into account time zone curves, since I am too lazy to saw the implementation for the sake of several points of the planet
+        
+        @param length: int
+        @param saveSchedule: bool
+        @param updateTLE: bool
 
-        Not the best implementation but there is no other one yet.
+        @return schedule: list[SatPass]
 
-        It does not take into account time zone curves, since I am too lazy to saw the implementation for the sake of several points of the planet
         """
-        self._checkCoordinates()
+
+        #self._checkCoordinates()
 
         if updateTLE:
             self.update()
 
-        passes = {}
-        allPasses = []
-        start = datetime.utcnow()
-
-        th = ["Satellite", "DateTime", "Azimuth", "Elevation"]
-        td = []
-        passesForReturn = []
-
-        # Iterating through all the passes
-        for satellite in self.config['satList']:
-            pas = self.getSatellitePasses(start, length, satellite, tol)
-
-            # Flights of a specific satellite
-            passes[satellite] = pas
-
-            # All passes
-            for i in pas:
-                allPasses.append(i)
-        
-        # Generate table
-        for onePass in sorted(allPasses):
-            satName = ''
-            
-            # Going through the list of satellites
-            for satellite in self.config['satList']:
-                # If the selected span corresponds to a satellite
-                if onePass in passes[satellite]:
-                    satName = satellite
-                    break
-
-            name = join(self.path, 'tle', 'tle.txt')
-            orb = Orbital(satellite, name)
-
-            
-            # if apogee > minApogee
-            if orb.get_observer_look(onePass[2], self.lon, self.lat, self.alt)[1] >= self.config['minApogee']:
-                passesForReturn.append((orb, onePass))
-                td.append([satName, (onePass[0] + timedelta(hours=self.timeZone)).strftime("%Y.%m.%d %H:%M:%S"),
-                            *map(lambda x: round(x, 2), orb.get_observer_look(onePass[0], self.lon, self.lat, self.alt))])
+        schedule = []
+        
+        for i in self.satList:
+            orb, passes = self.getSatellitePasses(start=timeStart, length=length, satellite=i)
+        
+            for j in passes:
+                culmination = orb.get_observer_look(j[2], lat = self.lat, lon = self.lon, alt = self.alt)[1]
+                # if apogee > minApogee
+                if culmination >= self.config.minApogee:
+                    schedule.append(SatPass(satName = i, orb = orb, culmination=culmination, timeStart=j[0], timeEnd=j[1], timeCulmination=j[2]))
+        
+        ## Sort by time start 
+        schedule = sorted(schedule, key=lambda p: p.timeStart)
+        self.schedule = schedule
 
-                td.append([satName, (onePass[2] + timedelta(hours=self.timeZone)).strftime("%Y.%m.%d %H:%M:%S"),
-                            *map(lambda x: round(x, 2), orb.get_observer_look(onePass[2], self.lon, self.lat, self.alt))])
+        timeCorrection = timedelta(hours=self.timeZone)
+        
+        ## Generate pretty string and file for schedule
+        if saveSchedule:
+            th = ["Satellite", "DateTime", "Azimuth", "Elevation"]
+            td = []
 
-                td.append([satName, (onePass[1] + timedelta(hours=self.timeZone)).strftime("%Y.%m.%d %H:%M:%S"),
-                            *map(lambda x: round(x, 2), orb.get_observer_look(onePass[1], self.lon, self.lat, self.alt))])
+            for satPass in schedule:
+                start = satPass.timeStart
+                stop = satPass.timeEnd
+                apogee = satPass.timeCulmination
+
+                td.append([satPass.satName,
+                           (start + timeCorrection).strftime("%Y.%m.%d %H:%M:%S"),
+                           *map(lambda x: round(x, 2), 
+                           satPass.orb.get_observer_look(start, self.lon, self.lat, self.alt))])
+
+                td.append([satPass.satName,
+                           (apogee + timeCorrection).strftime("%Y.%m.%d %H:%M:%S"),
+                           *map(lambda x: round(x, 2), 
+                           satPass.orb.get_observer_look(apogee, self.lon, self.lat, self.alt))])
+
+                td.append([satPass.satName,
+                           (stop + timeCorrection).strftime("%Y.%m.%d %H:%M:%S"),
+                           *map(lambda x: round(x, 2), 
+                           satPass.orb.get_observer_look(stop, self.lon, self.lat, self.alt))])
 
                 td.append([" ", " ", " ", " "])
 
-        table = PrettyTable(th)
+                table = PrettyTable(th)
 
-        # Adding rows to tables
-        for i in td:
-            table.add_row(i)
-
-        start += timedelta(hours=self.timeZone)
-        stop = start + timedelta(hours=length) + timedelta(hours=self.timeZone)
-
-        # Generate schedule string
-        schedule = f"Satellits Schedule / LorettOrbital {__version__}\n"
-        schedule += f"Coordinates of the position: {round(self.lon, 4)}° {round(self.lat, 4)}° {self.alt}km\n"
-        schedule += f"Time zone: UTC {'+' if self.timeZone >= 0 else '-'}{abs(self.timeZone)}:00\n"
-        schedule += f"Start: {start.strftime('%Y.%m.%d %H:%M:%S')}\n"
-        schedule += f"Stop:  {stop.strftime('%Y.%m.%d %H:%M:%S')}\n"
+            ## Adding rows to tables
+            for i in td:
+                table.add_row(i)
 
-        schedule += f"Minimum Elevation: {self.config['horizon']}°\n"
-        schedule += f"Minimum Apogee: {self.config['minApogee']}°\n"
-
-        schedule += f"Number of passes: {len(td)//4}\n\n"
-        schedule += table.get_string()
-
-        if saveSchedule:
-            try:
-                name = join(self.schedulePath, f'Schedule_{datetime.now().strftime("%Y-%m-%dT%H-%M")}.txt')
+            if self.logger != None:
+                self.logger.info(f"Calculate schedule. {len(schedule)} passes found")
+            
+            ## Generate schedule string
+            schedule = f"Satellits Schedule / LorettOrbital {__version__}\n"
+            schedule += f"Coordinates of the position: {round(self.lon, 4)}° {round(self.lat, 4)}° {self.alt}km\n"
+            schedule += f"Time zone: UTC {'+' if self.timeZone >= 0 else '-'}{abs(self.timeZone)}:00\n"
+            schedule += f"Start: {(timeStart + timeCorrection).strftime('%Y.%m.%d %H:%M:%S')}\n"
+            schedule += f"Stop:  {(start + timedelta(hours=length)).strftime('%Y.%m.%d %H:%M:%S')}\n"
 
-                with open(name, 'w') as file:
-                    file.write(schedule)
+            schedule += f"Minimum Elevation: {self.config.horizon}°\n"
+            schedule += f"Minimum Apogee: {self.config.minApogee}°\n"
 
-            except Exception as e:
-                print("ERROR:", e)
-                return None
+            schedule += f"Number of passes: {len(td)//4}\n\n"
+            schedule += table.get_string()
 
-        if returnTable:
-            return schedule
+            name = self.schedulePath / f'Schedule_{datetime.now().strftime("%Y-%m-%dT%H-%M")}.txt'
 
-        elif returnNameSatellite:
-            massout = []
-            for pas in passesForReturn:
-                massout.append((pas[0].satellite_name, pas[1]))
+            with open(name, 'w') as file:
+                file.write(schedule)
 
-            return massout
-            
-        else:
-            return passesForReturn
+        return self.schedule
 
 
-    '''Метод для генерирации трек файла'''
-    def generateTrack(self, satellite: str, satPass: list, savePlotTrack: bool = False):
+    def generateTrackFile(self, satPass: SatPass, timestep: int = 1) -> TrackFile:
         """
-        Method for generating a track file
-
-        In:
-            str satellite
-
-            list satPass
+        The method for generating a track file for Rosental systems
+        
 
-            bool  savePlotTrack
+        @param satPass: list[SatPass] 
+        @param timestep: float
 
-        Out:
-            tuple (satellite [time, azimuth, altitude])
+        @return TrackFile
         """
-
-        orb = Orbital(satellite, join(self.path, "tle", "tle.txt"))
-
-        trackPath = join(self.path, 'tracks', f"{satellite.replace(' ', '-')}_{self.stationType.upper()}_{satPass[0].strftime('%Y-%m-%dT%H-%M')}.txt")
-
-        with open(trackPath, "w") as file:
-
-            times = []
+        
+        ## timestep should only be an integer due to the format of the time record in the file: %H:%M:%S. The real part is simply lost.
+        if timestep < 1:
+            timestep = 1
             
-            сoordsAZ = []
-            сoordsEL = []
-
-            if self.config['kinematic'] == 'focal':
-                coordsX = []
-                coordsY = []
-
-            startTime = satPass[0].strftime('%Y-%m-%d   %H:%M:%S') + " UTC"
-
-            metaData = f"{self.stationType.upper()} track file / LorettOrbital {__version__}\n" + \
-                       f"StationName: {self.stationName}\n" +                                     \
-                       f"Station Position: {self.lon}° {self.lat}° {self.alt}km\n" +              \
-                       f"Satellite: {satellite}\n" +                                              \
-                       f"Start date & time: {startTime}\n" +                                      \
-                       f"Orbit: {orb.get_orbit_number(satPass[0])}\n"
-
-            metaData += "Time (UTC)   Azimuth (deg:min)   Elevation (deg:min)\n\n" if self.config['kinematic'] == 'focal' \
-                       else "Time (UTC)   Azimuth (deg)   Elevation (deg)\n\n"
-
-            # Write metadata
-            file.write(metaData)
-
-            # Generating track steps
-            for i in range((satPass[1] - satPass[0]).seconds):
-
-                dateTimeForCalc = satPass[0] + timedelta(seconds=i)
-                strTime = dateTimeForCalc.strftime("%H:%M:%S")
-
-                # Convert degrees to degrees:minutes
-                observerLook = orb.get_observer_look(
-                    dateTimeForCalc, self.lon, self.lat, self.alt)
-
-                sphCoords = self.degreesToDegreesAndMinutes(*observerLook)
-
-                times.append(strTime)
-
-                if self.config['kinematic'] == 'focal':
-                    сoordsAZ.append(sphCoords[0])
-                    сoordsEL.append(sphCoords[1])
-
-                    coords = self.sphericalToDecart(*observerLook)
-
-                    coordsX.append(coords[0])
-                    coordsY.append(coords[1])
-
-                elif self.config['kinematic'] == 'rotate':
-                    сoordsAZ.append(f'{observerLook[0]:.2f}')
-                    сoordsEL.append(f'{observerLook[1]:.2f}')
-
-                string = f"{strTime}   {сoordsAZ[-1]}   {сoordsEL[-1]}\n"
-                file.write(string)
-
-        if savePlotTrack and (self.config['kinematic'] == 'focal'):
-            self.SavePlotTrack(coordsX, coordsY, satellite, startTime)
-
-        return satellite, list(zip(times, сoordsAZ, сoordsEL))
-
-
-    '''Метод для отрисовки трека и сохренения в файл'''
-    def SavePlotTrack(self, coordsX: list, coordsY: list, satellite: str = "Untitled", start: str = "") -> None:
-        """
-        Method for drawing a track and saving it to a file
-
-        In:
-                float coordsX[]
-
-                float coordsY[]
+        if isinstance(timestep, float):
+            timestep = int(timestep)
+        
+        t = (satPass.timeEnd - satPass.timeStart)
+        time = satPass.timeStart
+        
+        satTrack = []
+        
+        for i in range(0, int(t.total_seconds()/timestep)+1): 
+            time += timedelta(seconds=timestep) 
+            azimuth, elevation  = satPass.orb.get_observer_look(time, lat = self.lat, lon = self.lon, alt = self.alt)
+            
+            sphCoords = self.degreesToDegreesAndMinutes(azimuth, elevation, time)
+            
+            satTrack.append(sphCoords)
 
-                str satellite
+        
+        trackPath = self.tracksPath / f"{satPass.satName.replace(' ', '-')}_{self.stationType}_{satPass.timeStart.strftime('%Y-%m-%dT%H-%M')}.txt"
+        
+        try:
+            with open(trackPath, "w") as file:
+                startTime = satPass.timeStart.strftime('%Y-%m-%d   %H:%M:%S') + " UTC"
 
-                str start
+                metaData = f"Satellite: {satPass.satName}\n" +                                        \
+                            f"Start date & time: {startTime}\n" +                                      \
+                            f"Orbit: {satPass.orb.get_orbit_number(satPass.timeStart)}\n\n"
+                metaData += "Time (UTC)   Azimuth (deg:min)   Elevation (deg:min)\n\n"
+
+                ## Write metadata
+                file.write(metaData)
+
+                for i in satTrack:
+                    file.write(f"{i.time.strftime('%H:%M:%S')}   {i.azimuth}   {i.elevation}\n")
+                    
+        except:
+            if self.logger != None:
+                self.logger.error(f"Failed generate legacy track for {satPass.satName}")
 
-                bool savePlotTrack
+        if self.logger != None:
+            self.logger.info(f"Generate legacy track for {satPass.satName}")
+        
+        return TrackFile(satName=satPass.satName, timeStart=satPass.timeStart, trackPath=trackPath)
+    
+    
+    def getSateliteTrack(self, satPass: SatPass, timestep: float = 0.5, save: bool = True) -> List[SphereCoordinates]:
+        """ The method for getting satellite trajectory
+        
+        @param satPass: SatPass
+        @param timestep: float
+        @param save: bool
+        
+        @return satTrack: list[SphereCoordinates]
+        
         """
-
-        ax = plt.gca()
-        ax.set_aspect('equal', adjustable='box')
-
-        # Plot mirror
-        circle = plt.Circle((0, 0), self.config['radius'],
-                                color=self.mirrorCircleColor)
-        ax.add_patch(circle)
-
-        # Set window title
-        fig = plt.figure(1)
-        fig.canvas.manager.set_window_title(satellite + "   " + start)
-
-        # Generate OX and OY Axes
-        steps = list(round(i, 1) for i in arange(
-            -self.config['radius'], self.config['radius'] + 0.1, 0.1))
-
-        plt.title(satellite + "   " + start)
-
-        # Plot OX and OY Axes
-        plt.plot([0]*len(steps), steps, '--k')
-        plt.plot(steps, [0]*len(steps), '--k')
-
-        # Plot track
-        plt.plot(coordsX, coordsY, '-.r')
-
-        # Plot start and end points
-        plt.plot(coordsX[0], coordsY[0], ".b")
-        plt.plot(coordsX[-1], coordsY[-1], ".r")
-
-        # Plot north
-        plt.plot(0, self.config['radius'], "^r")
-
-        fileName = join(self.path, 'tracksSchemes', f"TracksSchemes_{satellite.replace(' ', '-')}_{start.replace('   ', '-').replace(':', '-')}.png")
-        plt.savefig(fileName)
-
-
-    '''Метод для расчета трека ближайщего следующего пролета'''
-    def nextPass(self, length = 12, printTrack: bool = False, savePlotTrack: bool = False):
-        '''
-        Method for calculating the track of the nearest next span
-
-        In:
-            bool  printTrack
-
-            bool  savePlotTrack
-
-        Out:
-            tuple (Satellite [time, azimuth, altitute])'''
-
         
-        passesList = self.getSchedule(length)
-
-        count = 1
-        td = []
-
-        for satPass, satPasTimeList in passesList:
-
-            td.append([count, satPass.satellite_name, *satPasTimeList, round(
-                satPass.get_observer_look(satPasTimeList[2], self.lon, self.lat, self.alt)[1], 2)])
-            td.append(("", "", "", "", "", ""))
-
-            count += 1
-
-        satPass, satPasTimeList = passesList[0]
-
-        if self.config['kinematic']:
-            outTrack =  self.generateTrack(satPass.satellite_name, satPasTimeList, savePlotTrack)
+        t = (satPass.timeEnd - satPass.timeStart)
+        
+        satTrack = []
+        time = satPass.timeStart
+        
+        for i in range(0, int(t.total_seconds()/timestep)+1): 
+            time += timedelta(seconds=timestep) 
+            azimuth, elevation  = satPass.orb.get_observer_look(time, lat = self.lat, lon = self.lon, alt = self.alt)
+            azimuth = round(azimuth, 2)
+            elevation = round(elevation, 2)
+            
+            satTrack.append(SphereCoordinates(azimuth = round(azimuth, 2),
+                                        elevation = round(elevation, 2),
+                                        time=time))
+        
+        if self.logger != None:
+            self.logger.info(f"Generate track for {satPass.satName}")
+        
+        ## Save track file if needed
+        if save:
+            trackPath = self.tracksPath / f"{satPass.satName.replace(' ', '-')}_{self.stationType}_{satPass.timeStart.strftime('%Y-%m-%dT%H-%M')}.txt"
 
-            if printTrack:
-                print('         ',outTrack[0])
-                for stepp in outTrack[1]:
-                    print(stepp[0], stepp[1], stepp[2], sep='   ')
+            try:
+                with open(trackPath, "w") as file:
+                    startTime = satPass.timeStart.strftime('%Y-%m-%d   %H:%M:%S') + " UTC"
 
-            return outTrack
+                    metaData = f"{self.stationType.upper()} track file / LorettOrbital {__version__}\n" + \
+                            f"StationName: {self.stationName}\n" +                                     \
+                            f"Station Position: {self.lon}° {self.lat}° {self.alt}km\n" +              \
+                            f"Satellite: {satPass.satName}\n" +                                        \
+                            f"Start date & time: {startTime}\n" +                                      \
+                            f"Orbit: {satPass.orb.get_orbit_number(satPass.timeStart)}\n\n"
 
+                    metaData += "Time (UTC)   Azimuth (deg)   Elevation (deg)\n\n"
 
-    '''Функция для установки местоположения станции'''
-    def setCoordinates(self, lon: float, lat: float, alt: float) -> None:
-        '''
-        Function for setting the station location
+                    ## Write metadata
+                    file.write(metaData)
 
-        In:
+                    for i in satTrack:
+                        file.write(f"{i.time}   {i.azimuth:.2f}   {i.elevation:.2f}\n")  
+            except:
+                if self.logger != None:
+                    self.logger.error(f"Failed generate legacy track for {satPass.satName}") 
+            
+        return satTrack
 
-            float lon
 
-            float lat
+    def setCoordinates(self, lat: float, lon: float, alt: float) -> bool:
+        """ The method for setting the station location
 
-            float alt
-        '''
+        @param lat: float
+        @param lon: float
+        @param alt: float
+            
+        @return status: bool
+        """
+            
+        if self._checkCoordinates(lat, lon, alt):
+            self.lat = round(lat, 5)
+            self.lon = round(lon, 5)
+            self.alt = round(alt, 5)
+            
+            if self.logger != None:
+                self.logger.info(f"Set coordinates {self.lat} {self.lon} {self.alt}")
 
-        self.lon = round(lon, 5)
-        self.lat = round(lat, 5)
-        self.alt = round(alt, 5)
+            return True
 
-        self._checkCoordinates()
+        return False
 
 
-    def setTimeZone(self, timeZone: int) -> None:
+    def setTimeZone(self, timeZone: int) -> bool:
+        """ The Method for change timezone
+            
+            @param timeZone: int
+            @return status: bool
+        """
         if abs(timeZone) > 12:
-            raise InvalidTimeCorrection
+            if self.logger != None:
+                self.logger.warning(f"Fail set timezone UTC {self.timeZone:+}")
+            
+            return False
 
         self.timeZone = timeZone
+        
+        if self.logger != None:
+            self.logger.info(f"Set timezone UTC {self.timeZone:+}")
+        
+        return True
 
     
-    def getStation(self):
+    def getStation(self) -> dict:
+        """ The Method returned station info
+            
+            @return info: dict
+        """
         return {"stationName": self.stationName,
-                "stationType": self.stationType,
 
                 "lon": self.lon,
                 "lat": self.lat,
                 "alt": self.alt,
 
-                'kinematic': self.config['kinematic'],
-                'band': self.config['band'],
-                'satList': self.config['satList'],
-                'sampleRate': self.config['sampleRate'],
-                'horizon': self.config['horizon'],
-                'minApogee': self.config['minApogee']}
+                'satList': [i[0] for i in self.satList],
+                'horizon': self.config.horizon,
+                'minApogee': self.config.minApogee
+                }
 
 
-    def getCoordinates(self):
+    def getCoordinates(self) -> dict:
+        """ The method returned station coordinates
+            
+            @return coordinates: dict
+        """
         return {"lon": self.lon,
                 "lat": self.lat,
                 "alt": self.alt}
+        
+    def getTLEPath(self) -> str:
+        """The method returned TLE Path
+        
+            @return tlePath: Path
+        """
+        return self.tlePath / "tle.txt" 
 
 
 
-class StationLogger:
-    def __init__(self, stationName: str, level:int) -> None:
-        self.logger = Logger(stationName, level)
-    
-    def scheduleMessage(self):
-        pass
-
-
-class lorettLBandLogger(StationLogger):
-    def __init__(self, level: int) -> None:
-        super().__init__(level)
-
-    def scheduleMessage(self):
-        pass
-
-
-class lorettAPTBandLogger(StationLogger):
-    def __init__(self, level: int) -> None:
-        super().__init__(level)
-
-    def scheduleMessage(self):
-        pass
-
-
-class StreamReader:
-    def __init__(self, source) -> None:
-        pass
-
-
-class SDRReader(StreamReader):
-    def __init__(self, source) -> None:
-        super().__init__(source)
 
-class Station:
-    def __init__(self, scheduler: Scheduler, streamReader: StreamReader, logger: StationLogger) -> None:
-        pass
```

### Comparing `lorettOrbital-0.0.4/setup.py` & `lorettOrbital-1.0.13042023/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
-from lorettOrbital.orbital import __version__
+from lorettOrbital import __version__
 
 
 with open("requirements.txt", 'r') as file:
       requirements =  file.readlines()
  
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setup(name='lorettOrbital',
       version=__version__,
       url='https://gitlab.com/lpmrfentazis/lorettorbital',
       license='MIT',
       author='MrFentazis',
       author_email='lpmrfentazis@mail.ru',
-      description='A module that makes it easier to interact with LORETT hardware and software complexes.',
+      description='LorettOrbital Python 3 library for orbital calculations and planning',
       long_description=long_description,
       packages=find_packages(),
       install_requires=requirements,
+      test_suite="tests",
       classifiers=[
-		"Programming Language :: Python :: 3.7",
+		"Programming Language :: Python :: 3.9",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
-      python_requires='>=3.7'
+      python_requires='>=3.9'
       )
```

