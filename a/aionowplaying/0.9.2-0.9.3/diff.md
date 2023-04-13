# Comparing `tmp/aionowplaying-0.9.2.tar.gz` & `tmp/aionowplaying-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aionowplaying-0.9.2.tar", max compression
+gzip compressed data, was "aionowplaying-0.9.3.tar", max compression
```

## Comparing `aionowplaying-0.9.2.tar` & `aionowplaying-0.9.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      534 2022-03-13 10:25:48.567329 aionowplaying-0.9.2/aionowplaying/__init__.py
--rw-r--r--   0        0        0      581 2022-01-23 06:51:27.828858 aionowplaying-0.9.2/aionowplaying/interface/__init__.py
--rw-r--r--   0        0        0     1758 2022-01-23 06:51:27.830864 aionowplaying-0.9.2/aionowplaying/interface/_windows.py
--rw-r--r--   0        0        0     7817 2022-03-13 10:25:48.569330 aionowplaying-0.9.2/aionowplaying/interface/base.py
--rw-r--r--   0        0        0    12271 2022-03-13 10:25:48.571836 aionowplaying-0.9.2/aionowplaying/interface/mpris2.py
--rw-r--r--   0        0        0     8615 2022-03-13 10:25:48.573884 aionowplaying-0.9.2/aionowplaying/interface/windows.py
--rw-r--r--   0        0        0    35823 2022-01-17 13:48:39.325261 aionowplaying-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0      816 2022-03-13 10:26:52.338506 aionowplaying-0.9.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-17 13:48:39.326293 aionowplaying-0.9.2/README.md
--rw-r--r--   0        0        0      876 2022-03-13 10:28:12.266362 aionowplaying-0.9.2/setup.py
--rw-r--r--   0        0        0      987 2022-03-13 10:28:12.267373 aionowplaying-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-01-17 01:33:16.709617 aionowplaying-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-01-17 01:23:49.022832 aionowplaying-0.9.3/README.md
+-rw-r--r--   0        0        0      522 2022-02-07 03:32:14.444699 aionowplaying-0.9.3/aionowplaying/__init__.py
+-rw-r--r--   0        0        0      626 2022-04-08 05:52:38.131792 aionowplaying-0.9.3/aionowplaying/interface/__init__.py
+-rw-r--r--   0        0        0     7604 2022-04-08 05:52:08.749871 aionowplaying-0.9.3/aionowplaying/interface/base.py
+-rw-r--r--   0        0        0     2745 2022-05-12 11:12:29.545349 aionowplaying-0.9.3/aionowplaying/interface/macos.py
+-rw-r--r--   0        0        0    11957 2022-01-26 09:17:40.338085 aionowplaying-0.9.3/aionowplaying/interface/mpris2.py
+-rw-r--r--   0        0        0    10211 2023-04-13 15:30:05.909042 aionowplaying-0.9.3/aionowplaying/interface/windows.py
+-rw-r--r--   0        0        0      845 2023-04-13 15:34:24.635413 aionowplaying-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 aionowplaying-0.9.3/PKG-INFO
```

### Comparing `aionowplaying-0.9.2/aionowplaying/__init__.py` & `aionowplaying-0.9.3/aionowplaying/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-__all__ = ['select_interface', 'BaseInterface', 'PropertyName', 'LoopStatus', 'PlaybackPropertyName',
-           'PlaybackProperties', 'PlaybackStatus', 'NowPlayingInterface']
-
-from typing import Type
-
-from aionowplaying.interface import select_interface, BaseInterface
-from aionowplaying.interface.base import PropertyName, LoopStatus, PlaybackPropertyName, PlaybackProperties, \
-    PlaybackStatus
-
-NowPlayingInterface: Type[BaseInterface] = select_interface()
-if NowPlayingInterface is None:
-    raise NotImplemented()
+__all__ = ['select_interface', 'BaseInterface', 'PropertyName', 'LoopStatus', 'PlaybackPropertyName',
+           'PlaybackProperties', 'PlaybackStatus', 'NowPlayingInterface']
+
+from typing import Type
+
+from aionowplaying.interface import select_interface, BaseInterface
+from aionowplaying.interface.base import PropertyName, LoopStatus, PlaybackPropertyName, PlaybackProperties, \
+    PlaybackStatus
+
+NowPlayingInterface: Type[BaseInterface] = select_interface()
+if NowPlayingInterface is None:
+    raise NotImplemented()
```

### Comparing `aionowplaying-0.9.2/aionowplaying/interface/base.py` & `aionowplaying-0.9.3/aionowplaying/interface/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,253 +1,256 @@
-from enum import Enum
-from typing import Any, List
-from pydantic import BaseModel
-
-
-class TrackListPropertyName(str, Enum):
-    Tracks = 'Tracks'
-    CanEditTracks = 'CanEditTracks'
-
-
-class PropertyName(str, Enum):
-    CanQuit = "CanQuit"
-    CanSetFullscreen = "CanSetFullscreen"
-    CanRaise = "CanRaise"
-    HasTrackList = "HasTrackList"
-    Identity = "Identity"
-    DesktopEntry = "DesktopEntry"
-    SupportedUriSchemes = "SupportedUriSchemes"
-    SupportedMimeTypes = "SupportedMimeTypes"
-    Fullscreen = "Fullscreen"
-
-
-class PlaybackPropertyName(str, Enum):
-    PlaybackStatus = "PlaybackStatus"
-    LoopStatus = "LoopStatus"
-    Rate = "Rate"
-    Shuffle = "Shuffle"
-    Metadata = "Metadata"
-    Volume = "Volume"
-    Position = "Position"
-    MinimumRate = "MinimumRate"
-    MaximumRate = "MaximumRate"
-    CanGoNext = "CanGoNext"
-    CanGoPrevious = "CanGoPrevious"
-    CanPlay = "CanPlay"
-    CanPause = "CanPause"
-    CanSeek = "CanSeek"
-    CanControl = "CanControl"
-
-
-class PlaybackStatus(str, Enum):
-    Playing = "Playing"
-    Paused = "Paused"
-    Stopped = "Stopped"
-
-
-class LoopStatus(str, Enum):
-    None_ = "None"
-    Track = "Track"
-    Playlist = "Playlist"
-
-
-class MediaType(str, Enum):
-    Music = "Music"
-    Video = "Video"
-    Image = "Image"
-
-
-class TrackListProperties(BaseModel):
-    Tracks: List[str] = []
-    CanEditTracks: bool = False
-
-
-class PlayerProperties(BaseModel):
-    Fullscreen: bool = False
-    CanQuit: bool = False
-    CanSetFullscreen: bool = False
-    CanRaise: bool = False
-    HasTrackList: bool = False
-    Identity: str = ""
-    DesktopEntry: str = ""
-    SupportedUriSchemes: List[str] = []
-    SupportedMimeTypes: List[str] = []
-
-
-class PlaybackProperties(BaseModel):
-    class MetadataBean(BaseModel):
-        id_: str = ''
-        media_type: 'MediaType' = MediaType.Music
-        duration: int = 0  # in microseconds
-        cover: str = ''
-        album: str = ''
-        albumArtist: List[str] = []
-        artist: List[str] = []
-        lyrics: str = ''
-        comments: List[str] = []
-        composer: List[str] = []
-        genre: List[str] = []
-        lyricist: List[str] = []
-        title: str = "Unknown"
-        trackNumber: int = 0
-        url: str = ''
-
-    PlaybackStatus: 'PlaybackStatus' = PlaybackStatus.Stopped
-    LoopStatus: 'LoopStatus' = LoopStatus.None_
-    Rate: float = 1.0
-    Shuffle: bool = False
-    Metadata: MetadataBean = MetadataBean()
-    Volume: float = 1.0
-    Position: int = 0  # in microseconds
-    MinimumRate: float = 1.0
-    MaximumRate: float = 1.0
-    CanGoNext: bool = False
-    CanGoPrevious: bool = False
-    CanPlay: bool = False
-    CanPause: bool = False
-    CanSeek: bool = False
-    CanControl: bool = False
-
-
-class BaseInterface:
-    def __init__(self, name: str):
-        pass
-
-    async def start(self):
-        """
-        Call this method to start nowplaying backend.
-        Wrap with :meth:`asyncio.ensure_future` if you want to run in background.
-        """
-        pass
-
-    async def on_fullscreen(self, fullscreen: bool):
-        """
-        This will be called when nowplaying backend want to set player fullscreen state.
-        This will only be called if you set :attr:`PlayerProperties.CanSetFullscreen` to True.
-        :param fullscreen: True if fullscreen, False otherwise.
-        :type fullscreen: bool
-        """
-        pass
-
-    async def on_raise(self):
-        """
-        This will be called when nowplaying backend want to raise player window.
-        This will only be called if you set :attr:`PlayerProperties.CanRaise` to True.
-        """
-        pass
-
-    async def on_quit(self):
-        """
-        This will be called when nowplaying backend want to quit player.
-        This will only be called if you set :attr:`PlayerProperties.CanQuit` to True.
-        """
-        pass
-
-    async def on_loop_status(self, status: LoopStatus):
-        """
-        This will be called when nowplaying backend want to set loop status.
-        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
-        :param status: Loop status.
-        :type status: LoopStatus
-        """
-        pass
-
-    async def on_rate(self, rate: float):
-        """
-        This will be called when nowplaying backend want to set playback rate.
-        The rate is a float value between :attr:`PlaybackProperties.MinimumRate`
-        and :attr:`PlaybackProperties.MaximumRate`.
-        :param rate: Playback rate.
-        :type rate: float
-        """
-        pass
-
-    async def on_shuffle(self, shuffle: bool):
-        """
-        This will be called when nowplaying backend want to set shuffle status.
-        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
-        :param shuffle: True if shuffle, False otherwise.
-        :type shuffle: bool
-        """
-        pass
-
-    async def on_volume(self, volume: float):
-        """
-        This will be called when nowplaying backend want to set playback volume.
-        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
-        :param volume: Volume value between 0.0 and 1.0 (both inclusive).
-        :type volume: float
-        """
-        pass
-
-    async def on_next(self):
-        """
-        This will be called when nowplaying backend want to play next track.
-        This will only be called if you set :attr:`PlaybackProperties.CanGoNext` to True.
-        """
-        pass
-
-    async def on_previous(self):
-        """
-        This will be called when nowplaying backend want to play previous track.
-        This will only be called if you set :attr:`PlaybackProperties.CanGoPrevious` to True.
-        """
-        pass
-
-    async def on_pause(self):
-        """
-        This will be called when nowplaying backend want to pause playback.
-        This will only be called if you set :attr:`PlaybackProperties.CanPause` to True.
-        """
-        pass
-
-    async def on_play_pause(self):
-        """
-        This will be called when nowplaying backend want to play or pause playback.
-        This will only be called if you set :attr:`PlaybackProperties.CanPause` to True.
-        """
-        if self.get_playback_property(PlaybackPropertyName.PlaybackStatus) == PlaybackStatus.Playing:
-            await self.on_pause()
-            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Paused)
-        else:
-            await self.on_play()
-            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Playing)
-
-    async def on_play(self):
-        """
-        This will be called when nowplaying backend want to play playback.
-        This will only be called if you set :attr:`PlaybackProperties.CanPlay` to True.
-        """
-        pass
-
-    async def on_stop(self):
-        pass
-
-    async def on_seek(self, offset: int):
-        pass
-
-    async def on_open_uri(self, uri: str):
-        pass
-
-    async def on_set_position(self, track_id: str, position: int):
-        pass
-
-    async def seeked(self, position: int):
-        pass
-
-    def set_property(self, name: PropertyName, value: Any):
-        pass
-
-    def set_playback_property(self, name: PlaybackPropertyName, value: Any):
-        pass
-
-    def set_tracklist_property(self, name: TrackListPropertyName, value: Any):
-        pass
-
-    def get_property(self, name: PropertyName) -> Any:
-        pass
-
-    def get_playback_property(self, name: PlaybackPropertyName) -> Any:
-        pass
-
-    def get_tracklist_property(self, name: TrackListPropertyName) -> Any:
-        pass
+from enum import Enum
+from typing import Any, List
+from pydantic import BaseModel
+
+
+class TrackListPropertyName(str, Enum):
+    Tracks = 'Tracks'
+    CanEditTracks = 'CanEditTracks'
+
+
+class PropertyName(str, Enum):
+    CanQuit = "CanQuit"
+    CanSetFullscreen = "CanSetFullscreen"
+    CanRaise = "CanRaise"
+    HasTrackList = "HasTrackList"
+    Identity = "Identity"
+    DesktopEntry = "DesktopEntry"
+    SupportedUriSchemes = "SupportedUriSchemes"
+    SupportedMimeTypes = "SupportedMimeTypes"
+    Fullscreen = "Fullscreen"
+
+
+class PlaybackPropertyName(str, Enum):
+    PlaybackStatus = "PlaybackStatus"
+    LoopStatus = "LoopStatus"
+    Rate = "Rate"
+    Shuffle = "Shuffle"
+    Metadata = "Metadata"
+    Volume = "Volume"
+    Position = "Position"
+    MinimumRate = "MinimumRate"
+    MaximumRate = "MaximumRate"
+    CanGoNext = "CanGoNext"
+    CanGoPrevious = "CanGoPrevious"
+    CanPlay = "CanPlay"
+    CanPause = "CanPause"
+    CanSeek = "CanSeek"
+    CanControl = "CanControl"
+
+
+class PlaybackStatus(str, Enum):
+    Playing = "Playing"
+    Paused = "Paused"
+    Stopped = "Stopped"
+
+
+class LoopStatus(str, Enum):
+    None_ = "None"
+    Track = "Track"
+    Playlist = "Playlist"
+
+
+class MediaType(str, Enum):
+    Music = "Music"
+    Video = "Video"
+    Image = "Image"
+
+
+class TrackListProperties(BaseModel):
+    Tracks: List[str] = []
+    CanEditTracks: bool = False
+
+
+class PlayerProperties(BaseModel):
+    Fullscreen: bool = False
+    CanQuit: bool = False
+    CanSetFullscreen: bool = False
+    CanRaise: bool = False
+    HasTrackList: bool = False
+    Identity: str = ""
+    DesktopEntry: str = ""
+    SupportedUriSchemes: List[str] = []
+    SupportedMimeTypes: List[str] = []
+
+
+class PlaybackProperties(BaseModel):
+    class MetadataBean(BaseModel):
+        id_: str = ''
+        media_type: 'MediaType' = MediaType.Music
+        duration: int = 0  # in microseconds
+        cover: str = ''
+        album: str = ''
+        albumArtist: List[str] = []
+        artist: List[str] = []
+        lyrics: str = ''
+        comments: List[str] = []
+        composer: List[str] = []
+        genre: List[str] = []
+        lyricist: List[str] = []
+        title: str = "Unknown"
+        trackNumber: int = 0
+        url: str = ''
+
+    PlaybackStatus: 'PlaybackStatus' = PlaybackStatus.Stopped
+    LoopStatus: 'LoopStatus' = LoopStatus.None_
+    Rate: float = 1.0
+    Shuffle: bool = False
+    Metadata: MetadataBean = MetadataBean()
+    Volume: float = 1.0
+    Position: int = 0  # in microseconds
+    MinimumRate: float = 1.0
+    MaximumRate: float = 1.0
+    CanGoNext: bool = False
+    CanGoPrevious: bool = False
+    CanPlay: bool = False
+    CanPause: bool = False
+    CanSeek: bool = False
+    CanControl: bool = False
+
+
+class BaseInterface:
+    def __init__(self, name: str):
+        pass
+
+    async def start(self):
+        """
+        Call this method to start nowplaying backend.
+        Wrap with :meth:`asyncio.ensure_future` if you want to run in background.
+        """
+        pass
+
+    async def stop(self):
+        pass
+
+    async def on_fullscreen(self, fullscreen: bool):
+        """
+        This will be called when nowplaying backend want to set player fullscreen state.
+        This will only be called if you set :attr:`PlayerProperties.CanSetFullscreen` to True.
+        :param fullscreen: True if fullscreen, False otherwise.
+        :type fullscreen: bool
+        """
+        pass
+
+    async def on_raise(self):
+        """
+        This will be called when nowplaying backend want to raise player window.
+        This will only be called if you set :attr:`PlayerProperties.CanRaise` to True.
+        """
+        pass
+
+    async def on_quit(self):
+        """
+        This will be called when nowplaying backend want to quit player.
+        This will only be called if you set :attr:`PlayerProperties.CanQuit` to True.
+        """
+        pass
+
+    async def on_loop_status(self, status: LoopStatus):
+        """
+        This will be called when nowplaying backend want to set loop status.
+        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
+        :param status: Loop status.
+        :type status: LoopStatus
+        """
+        pass
+
+    async def on_rate(self, rate: float):
+        """
+        This will be called when nowplaying backend want to set playback rate.
+        The rate is a float value between :attr:`PlaybackProperties.MinimumRate`
+        and :attr:`PlaybackProperties.MaximumRate`.
+        :param rate: Playback rate.
+        :type rate: float
+        """
+        pass
+
+    async def on_shuffle(self, shuffle: bool):
+        """
+        This will be called when nowplaying backend want to set shuffle status.
+        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
+        :param shuffle: True if shuffle, False otherwise.
+        :type shuffle: bool
+        """
+        pass
+
+    async def on_volume(self, volume: float):
+        """
+        This will be called when nowplaying backend want to set playback volume.
+        This will only be called if you set :attr:`PlaybackProperties.CanControl` to True.
+        :param volume: Volume value between 0.0 and 1.0 (both inclusive).
+        :type volume: float
+        """
+        pass
+
+    async def on_next(self):
+        """
+        This will be called when nowplaying backend want to play next track.
+        This will only be called if you set :attr:`PlaybackProperties.CanGoNext` to True.
+        """
+        pass
+
+    async def on_previous(self):
+        """
+        This will be called when nowplaying backend want to play previous track.
+        This will only be called if you set :attr:`PlaybackProperties.CanGoPrevious` to True.
+        """
+        pass
+
+    async def on_pause(self):
+        """
+        This will be called when nowplaying backend want to pause playback.
+        This will only be called if you set :attr:`PlaybackProperties.CanPause` to True.
+        """
+        pass
+
+    async def on_play_pause(self):
+        """
+        This will be called when nowplaying backend want to play or pause playback.
+        This will only be called if you set :attr:`PlaybackProperties.CanPause` to True.
+        """
+        if self.get_playback_property(PlaybackPropertyName.PlaybackStatus) == PlaybackStatus.Playing:
+            await self.on_pause()
+            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Paused)
+        else:
+            await self.on_play()
+            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Playing)
+
+    async def on_play(self):
+        """
+        This will be called when nowplaying backend want to play playback.
+        This will only be called if you set :attr:`PlaybackProperties.CanPlay` to True.
+        """
+        pass
+
+    async def on_stop(self):
+        pass
+
+    async def on_seek(self, offset: int):
+        pass
+
+    async def on_open_uri(self, uri: str):
+        pass
+
+    async def on_set_position(self, track_id: str, position: int):
+        pass
+
+    async def seeked(self, position: int):
+        pass
+
+    def set_property(self, name: PropertyName, value: Any):
+        pass
+
+    def set_playback_property(self, name: PlaybackPropertyName, value: Any):
+        pass
+
+    def set_tracklist_property(self, name: TrackListPropertyName, value: Any):
+        pass
+
+    def get_property(self, name: PropertyName) -> Any:
+        pass
+
+    def get_playback_property(self, name: PlaybackPropertyName) -> Any:
+        pass
+
+    def get_tracklist_property(self, name: TrackListPropertyName) -> Any:
+        pass
```

### Comparing `aionowplaying-0.9.2/aionowplaying/interface/mpris2.py` & `aionowplaying-0.9.3/aionowplaying/interface/mpris2.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-from typing import Any
-
-from dbus_next import PropertyAccess, Variant
-from dbus_next.aio import MessageBus
-from dbus_next.service import ServiceInterface, dbus_property, method, signal
-
-from aionowplaying.interface.base import BaseInterface, PropertyName, PlayerProperties, PlaybackProperties, \
-    PlaybackPropertyName, LoopStatus, TrackListPropertyName, TrackListProperties
-
-
-class DBusBeanMapper:
-    @staticmethod
-    def metadata(metadata: PlaybackProperties.MetadataBean) -> dict:
-        metadata_map = dict()
-        metadata_map['mpris:trackid'] = Variant('s', metadata.id_)
-        metadata_map['mpris:length'] = Variant('x', metadata.duration)
-        metadata_map['mpris:artUrl'] = Variant('s', metadata.cover)
-        metadata_map['xesam:album'] = Variant('s', metadata.album)
-        metadata_map['xesam:albumArtist'] = Variant('as', metadata.albumArtist)
-        metadata_map['xesam:artist'] = Variant('as', metadata.artist)
-        metadata_map['xesam:asText'] = Variant('s', metadata.lyrics)
-        metadata_map['xesam:comment'] = Variant('as', metadata.comments)
-        metadata_map['xesam:composer'] = Variant('as', metadata.composer)
-        metadata_map['xesam:genre'] = Variant('as', metadata.genre)
-        metadata_map['xesam:lyricist'] = Variant('as', metadata.lyricist)
-        metadata_map['xesam:title'] = Variant('s', metadata.title)
-        metadata_map['xesam:trackNumber'] = Variant('i', metadata.trackNumber)
-        metadata_map['xesam:url'] = Variant('s', metadata.url)
-        return metadata_map
-
-
-class MprisPlayerServiceInterface(ServiceInterface):
-    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
-        super().__init__(bus_name)
-        self._properties = PlaybackProperties()
-        self._it = it
-
-    def set_property(self, name: str, value: Any):
-        setattr(self._properties, name, value)
-        if isinstance(value, PlaybackProperties.MetadataBean):
-            value = DBusBeanMapper.metadata(value)
-        self.emit_properties_changed({name: value})
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.PlaybackStatus.value)
-    def playback_status(self) -> 's':
-        return self._properties.PlaybackStatus.value
-
-    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.LoopStatus.value)
-    def loop_status(self) -> 's':
-        return self._properties.LoopStatus.value
-
-    @loop_status.setter
-    async def loop_status(self, value: 's'):
-        if self._properties.CanControl:
-            await self._it.on_loop_status(LoopStatus(value))
-            self._properties.LoopStatus = LoopStatus(value)
-
-    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Rate.value)
-    def rate(self) -> 'd':
-        return self._properties.Rate
-
-    @rate.setter
-    async def rate(self, value: 'd'):
-        await self._it.on_rate(value)
-        self._properties.Rate = value
-
-    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Shuffle.value)
-    def shuffle(self) -> 'b':
-        return self._properties.Shuffle
-
-    @shuffle.setter
-    async def shuffle(self, value: 'b'):
-        if self._properties.CanControl:
-            await self._it.on_shuffle(value)
-            self._properties.Shuffle = value
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.Metadata.value)
-    def metadata(self) -> 'a{sv}':
-        metadata = self._properties.Metadata
-        return DBusBeanMapper.metadata(metadata)
-
-    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Volume.value)
-    def volume(self) -> 'd':
-        return self._properties.Volume
-
-    @volume.setter
-    async def volume(self, value: 'd'):
-        if self._properties.CanControl:
-            await self._it.on_volume(value)
-            self._properties.Volume = value
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.Position.value)
-    def position(self) -> 'x':
-        return self._properties.Position
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.MinimumRate.value)
-    def minimum_rate(self) -> 'd':
-        return self._properties.MinimumRate
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.MaximumRate.value)
-    def maximum_rate(self) -> 'd':
-        return self._properties.MaximumRate
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanGoNext.value)
-    def can_go_next(self) -> 'b':
-        return self._properties.CanGoNext
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanGoPrevious.value)
-    def can_go_previous(self) -> 'b':
-        return self._properties.CanGoPrevious
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanPlay.value)
-    def can_play(self) -> 'b':
-        return self._properties.CanPlay
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanPause.value)
-    def can_pause(self) -> 'b':
-        return self._properties.CanPause
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanSeek.value)
-    def can_seek(self) -> 'b':
-        return self._properties.CanSeek
-
-    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanControl.value)
-    def can_control(self) -> 'b':
-        return self._properties.CanControl
-
-    @signal(name='Seeked')
-    async def seeked(self, position: int) -> 'x':
-        return position
-
-    @method(name="Next")
-    async def next(self):
-        if self._properties.CanGoNext:
-            await self._it.on_next()
-
-    @method(name="Previous")
-    async def previous(self):
-        if self._properties.CanGoPrevious:
-            await self._it.on_previous()
-
-    @method(name="Pause")
-    async def pause(self):
-        if self._properties.CanPause:
-            await self._it.on_pause()
-
-    @method(name="PlayPause")
-    async def play_pause(self):
-        if self._properties.CanPause:
-            await self._it.on_play_pause()
-
-    @method(name="Stop")
-    async def stop(self):
-        if self._properties.CanControl:
-            await self._it.on_stop()
-
-    @method(name="Play")
-    async def play(self):
-        if self._properties.CanPlay:
-            await self._it.on_play()
-
-    @method(name="Seek")
-    async def seek(self, offset: 'x'):
-        if self._properties.CanSeek:
-            await self._it.on_seek(offset)
-
-    @method(name="OpenUri")
-    async def open_uri(self, uri: 's'):
-        await self._it.on_open_uri(uri)
-
-    @method(name="SetPosition")
-    async def set_position(self, track_id: 'o', position: 'x'):
-        if self._properties.CanSeek:
-            await self._it.on_set_position(track_id, position)
-
-    def get_property(self, key):
-        return getattr(self._properties, key)
-
-
-class MprisServiceInterface(ServiceInterface):
-    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
-        super().__init__(bus_name)
-        self._properties = PlayerProperties()
-        self._it = it
-
-    @dbus_property(access=PropertyAccess.READWRITE, name=PropertyName.Fullscreen.value)
-    def fullscreen(self) -> 'b':
-        return self._properties.Fullscreen
-
-    @fullscreen.setter
-    async def fullscreen(self, value: 'b'):
-        if self._properties.CanSetFullscreen:
-            await self._it.on_fullscreen(value)
-            self._properties.Fullscreen = value
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanQuit.value)
-    def can_quit(self) -> 'b':
-        return self._properties.CanQuit
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanSetFullscreen.value)
-    def can_set_fullscreen(self) -> 'b':
-        return self._properties.CanSetFullscreen
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.HasTrackList.value)
-    def has_track_list(self) -> 'b':
-        return self._properties.HasTrackList
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanRaise.value)
-    def can_raise(self) -> 'b':
-        return self._properties.CanRaise
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.Identity.value)
-    def identity(self) -> 's':
-        return self._properties.Identity
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.DesktopEntry.value)
-    def desktop_entry(self) -> 's':
-        return self._properties.DesktopEntry
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.SupportedUriSchemes.value)
-    def supported_uri_schemes(self) -> 'as':
-        return self._properties.SupportedUriSchemes
-
-    @dbus_property(access=PropertyAccess.READ, name=PropertyName.SupportedMimeTypes.value)
-    def supported_mime_types(self) -> 'as':
-        return self._properties.SupportedMimeTypes
-
-    @method(name='Raise')
-    async def raise_(self):
-        if self._properties.CanRaise:
-            await self._it.on_raise()
-
-    @method(name='Quit')
-    async def quit(self):
-        if self._properties.CanQuit:
-            await self._it.on_quit()
-
-    def set_property(self, name: str, value: Any):
-        setattr(self._properties, name, value)
-        self.emit_properties_changed({name: value})
-
-    def get_property(self, key):
-        return getattr(self._properties, key)
-
-
-class MprisTracklistServiceInterface(ServiceInterface):
-    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
-        super().__init__(bus_name)
-        self._properties = TrackListProperties()
-        self._it = it
-
-    def set_property(self, name: str, value: Any):
-        setattr(self._properties, name, value)
-
-    @dbus_property(access=PropertyAccess.READ, name=TrackListPropertyName.CanEditTracks.value)
-    def can_edit_tracks(self) -> 'b':
-        return self._properties.CanEditTracks
-
-    @dbus_property(access=PropertyAccess.READ, name=TrackListPropertyName.Tracks.value)
-    def tracks(self) -> 'ao':
-        return self._properties.Tracks
-
-    def get_property(self, key):
-        return getattr(self._properties, key)
-
-
-class Mpris2Interface(BaseInterface):
-    def __init__(self, name: str):
-        super().__init__(name)
-        self._bus_name = f'org.mpris.MediaPlayer2.{name}'
-        self._entry_name = 'org.mpris.MediaPlayer2'
-        self._player_entry_name = 'org.mpris.MediaPlayer2.Player'
-        self._player_tracklist_name = 'org.mpris.MediaPlayer2.TrackList'
-        self._object_path = '/org/mpris/MediaPlayer2'
-        self._bus = MprisServiceInterface(self._entry_name, it=self)
-        self._player_bus = MprisPlayerServiceInterface(self._player_entry_name, it=self)
-        self._tracklist_bus = MprisTracklistServiceInterface(self._player_tracklist_name, it=self)
-
-    def set_property(self, name: PropertyName, value: Any):
-        self._bus.set_property(name.value, value)
-
-    def set_playback_property(self, name: PlaybackPropertyName, value: Any):
-        self._player_bus.set_property(name.value, value)
-
-    def set_tracklist_property(self, name: TrackListPropertyName, value: Any):
-        self._tracklist_bus.set_property(name.value, value)
-
-    def get_property(self, name: PropertyName) -> Any:
-        return self._bus.get_property(name.value)
-
-    def get_playback_property(self, name: PlaybackPropertyName) -> Any:
-        return self._player_bus.get_property(name.value)
-
-    def get_tracklist_property(self, name: TrackListPropertyName) -> Any:
-        return self._tracklist_bus.get_property(name.value)
-
-    async def seeked(self, position: int):
-        await self._player_bus.seeked(position)
-
-    async def start(self):
-        bus = await MessageBus().connect()
-        bus.export(self._object_path, self._bus)
-        bus.export(self._object_path, self._player_bus)
-        await bus.request_name(self._bus_name)
-        await bus.wait_for_disconnect()
-
-
-if __name__ == '__main__':
-    import asyncio
-
-    mp = Mpris2Interface('aionowplaying')
-    mp.set_property(PropertyName.CanQuit, True)
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(mp.start())
+from typing import Any
+
+from dbus_next import PropertyAccess, Variant
+from dbus_next.aio import MessageBus
+from dbus_next.service import ServiceInterface, dbus_property, method, signal
+
+from aionowplaying.interface.base import BaseInterface, PropertyName, PlayerProperties, PlaybackProperties, \
+    PlaybackPropertyName, LoopStatus, TrackListPropertyName, TrackListProperties
+
+
+class DBusBeanMapper:
+    @staticmethod
+    def metadata(metadata: PlaybackProperties.MetadataBean) -> dict:
+        metadata_map = dict()
+        metadata_map['mpris:trackid'] = Variant('s', metadata.id_)
+        metadata_map['mpris:length'] = Variant('x', metadata.duration)
+        metadata_map['mpris:artUrl'] = Variant('s', metadata.cover)
+        metadata_map['xesam:album'] = Variant('s', metadata.album)
+        metadata_map['xesam:albumArtist'] = Variant('as', metadata.albumArtist)
+        metadata_map['xesam:artist'] = Variant('as', metadata.artist)
+        metadata_map['xesam:asText'] = Variant('s', metadata.lyrics)
+        metadata_map['xesam:comment'] = Variant('as', metadata.comments)
+        metadata_map['xesam:composer'] = Variant('as', metadata.composer)
+        metadata_map['xesam:genre'] = Variant('as', metadata.genre)
+        metadata_map['xesam:lyricist'] = Variant('as', metadata.lyricist)
+        metadata_map['xesam:title'] = Variant('s', metadata.title)
+        metadata_map['xesam:trackNumber'] = Variant('i', metadata.trackNumber)
+        metadata_map['xesam:url'] = Variant('s', metadata.url)
+        return metadata_map
+
+
+class MprisPlayerServiceInterface(ServiceInterface):
+    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
+        super().__init__(bus_name)
+        self._properties = PlaybackProperties()
+        self._it = it
+
+    def set_property(self, name: str, value: Any):
+        setattr(self._properties, name, value)
+        if isinstance(value, PlaybackProperties.MetadataBean):
+            value = DBusBeanMapper.metadata(value)
+        self.emit_properties_changed({name: value})
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.PlaybackStatus.value)
+    def playback_status(self) -> 's':
+        return self._properties.PlaybackStatus.value
+
+    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.LoopStatus.value)
+    def loop_status(self) -> 's':
+        return self._properties.LoopStatus.value
+
+    @loop_status.setter
+    async def loop_status(self, value: 's'):
+        if self._properties.CanControl:
+            await self._it.on_loop_status(LoopStatus(value))
+            self._properties.LoopStatus = LoopStatus(value)
+
+    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Rate.value)
+    def rate(self) -> 'd':
+        return self._properties.Rate
+
+    @rate.setter
+    async def rate(self, value: 'd'):
+        await self._it.on_rate(value)
+        self._properties.Rate = value
+
+    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Shuffle.value)
+    def shuffle(self) -> 'b':
+        return self._properties.Shuffle
+
+    @shuffle.setter
+    async def shuffle(self, value: 'b'):
+        if self._properties.CanControl:
+            await self._it.on_shuffle(value)
+            self._properties.Shuffle = value
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.Metadata.value)
+    def metadata(self) -> 'a{sv}':
+        metadata = self._properties.Metadata
+        return DBusBeanMapper.metadata(metadata)
+
+    @dbus_property(access=PropertyAccess.READWRITE, name=PlaybackPropertyName.Volume.value)
+    def volume(self) -> 'd':
+        return self._properties.Volume
+
+    @volume.setter
+    async def volume(self, value: 'd'):
+        if self._properties.CanControl:
+            await self._it.on_volume(value)
+            self._properties.Volume = value
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.Position.value)
+    def position(self) -> 'x':
+        return self._properties.Position
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.MinimumRate.value)
+    def minimum_rate(self) -> 'd':
+        return self._properties.MinimumRate
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.MaximumRate.value)
+    def maximum_rate(self) -> 'd':
+        return self._properties.MaximumRate
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanGoNext.value)
+    def can_go_next(self) -> 'b':
+        return self._properties.CanGoNext
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanGoPrevious.value)
+    def can_go_previous(self) -> 'b':
+        return self._properties.CanGoPrevious
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanPlay.value)
+    def can_play(self) -> 'b':
+        return self._properties.CanPlay
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanPause.value)
+    def can_pause(self) -> 'b':
+        return self._properties.CanPause
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanSeek.value)
+    def can_seek(self) -> 'b':
+        return self._properties.CanSeek
+
+    @dbus_property(access=PropertyAccess.READ, name=PlaybackPropertyName.CanControl.value)
+    def can_control(self) -> 'b':
+        return self._properties.CanControl
+
+    @signal(name='Seeked')
+    async def seeked(self, position: int) -> 'x':
+        return position
+
+    @method(name="Next")
+    async def next(self):
+        if self._properties.CanGoNext:
+            await self._it.on_next()
+
+    @method(name="Previous")
+    async def previous(self):
+        if self._properties.CanGoPrevious:
+            await self._it.on_previous()
+
+    @method(name="Pause")
+    async def pause(self):
+        if self._properties.CanPause:
+            await self._it.on_pause()
+
+    @method(name="PlayPause")
+    async def play_pause(self):
+        if self._properties.CanPause:
+            await self._it.on_play_pause()
+
+    @method(name="Stop")
+    async def stop(self):
+        if self._properties.CanControl:
+            await self._it.on_stop()
+
+    @method(name="Play")
+    async def play(self):
+        if self._properties.CanPlay:
+            await self._it.on_play()
+
+    @method(name="Seek")
+    async def seek(self, offset: 'x'):
+        if self._properties.CanSeek:
+            await self._it.on_seek(offset)
+
+    @method(name="OpenUri")
+    async def open_uri(self, uri: 's'):
+        await self._it.on_open_uri(uri)
+
+    @method(name="SetPosition")
+    async def set_position(self, track_id: 'o', position: 'x'):
+        if self._properties.CanSeek:
+            await self._it.on_set_position(track_id, position)
+
+    def get_property(self, key):
+        return getattr(self._properties, key)
+
+
+class MprisServiceInterface(ServiceInterface):
+    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
+        super().__init__(bus_name)
+        self._properties = PlayerProperties()
+        self._it = it
+
+    @dbus_property(access=PropertyAccess.READWRITE, name=PropertyName.Fullscreen.value)
+    def fullscreen(self) -> 'b':
+        return self._properties.Fullscreen
+
+    @fullscreen.setter
+    async def fullscreen(self, value: 'b'):
+        if self._properties.CanSetFullscreen:
+            await self._it.on_fullscreen(value)
+            self._properties.Fullscreen = value
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanQuit.value)
+    def can_quit(self) -> 'b':
+        return self._properties.CanQuit
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanSetFullscreen.value)
+    def can_set_fullscreen(self) -> 'b':
+        return self._properties.CanSetFullscreen
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.HasTrackList.value)
+    def has_track_list(self) -> 'b':
+        return self._properties.HasTrackList
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.CanRaise.value)
+    def can_raise(self) -> 'b':
+        return self._properties.CanRaise
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.Identity.value)
+    def identity(self) -> 's':
+        return self._properties.Identity
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.DesktopEntry.value)
+    def desktop_entry(self) -> 's':
+        return self._properties.DesktopEntry
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.SupportedUriSchemes.value)
+    def supported_uri_schemes(self) -> 'as':
+        return self._properties.SupportedUriSchemes
+
+    @dbus_property(access=PropertyAccess.READ, name=PropertyName.SupportedMimeTypes.value)
+    def supported_mime_types(self) -> 'as':
+        return self._properties.SupportedMimeTypes
+
+    @method(name='Raise')
+    async def raise_(self):
+        if self._properties.CanRaise:
+            await self._it.on_raise()
+
+    @method(name='Quit')
+    async def quit(self):
+        if self._properties.CanQuit:
+            await self._it.on_quit()
+
+    def set_property(self, name: str, value: Any):
+        setattr(self._properties, name, value)
+        self.emit_properties_changed({name: value})
+
+    def get_property(self, key):
+        return getattr(self._properties, key)
+
+
+class MprisTracklistServiceInterface(ServiceInterface):
+    def __init__(self, bus_name: str, it: 'Mpris2Interface' = None):
+        super().__init__(bus_name)
+        self._properties = TrackListProperties()
+        self._it = it
+
+    def set_property(self, name: str, value: Any):
+        setattr(self._properties, name, value)
+
+    @dbus_property(access=PropertyAccess.READ, name=TrackListPropertyName.CanEditTracks.value)
+    def can_edit_tracks(self) -> 'b':
+        return self._properties.CanEditTracks
+
+    @dbus_property(access=PropertyAccess.READ, name=TrackListPropertyName.Tracks.value)
+    def tracks(self) -> 'ao':
+        return self._properties.Tracks
+
+    def get_property(self, key):
+        return getattr(self._properties, key)
+
+
+class Mpris2Interface(BaseInterface):
+    def __init__(self, name: str):
+        super().__init__(name)
+        self._bus_name = f'org.mpris.MediaPlayer2.{name}'
+        self._entry_name = 'org.mpris.MediaPlayer2'
+        self._player_entry_name = 'org.mpris.MediaPlayer2.Player'
+        self._player_tracklist_name = 'org.mpris.MediaPlayer2.TrackList'
+        self._object_path = '/org/mpris/MediaPlayer2'
+        self._bus = MprisServiceInterface(self._entry_name, it=self)
+        self._player_bus = MprisPlayerServiceInterface(self._player_entry_name, it=self)
+        self._tracklist_bus = MprisTracklistServiceInterface(self._player_tracklist_name, it=self)
+
+    def set_property(self, name: PropertyName, value: Any):
+        self._bus.set_property(name.value, value)
+
+    def set_playback_property(self, name: PlaybackPropertyName, value: Any):
+        self._player_bus.set_property(name.value, value)
+
+    def set_tracklist_property(self, name: TrackListPropertyName, value: Any):
+        self._tracklist_bus.set_property(name.value, value)
+
+    def get_property(self, name: PropertyName) -> Any:
+        return self._bus.get_property(name.value)
+
+    def get_playback_property(self, name: PlaybackPropertyName) -> Any:
+        return self._player_bus.get_property(name.value)
+
+    def get_tracklist_property(self, name: TrackListPropertyName) -> Any:
+        return self._tracklist_bus.get_property(name.value)
+
+    async def seeked(self, position: int):
+        await self._player_bus.seeked(position)
+
+    async def start(self):
+        bus = await MessageBus().connect()
+        bus.export(self._object_path, self._bus)
+        bus.export(self._object_path, self._player_bus)
+        await bus.request_name(self._bus_name)
+        await bus.wait_for_disconnect()
+
+
+if __name__ == '__main__':
+    import asyncio
+
+    mp = Mpris2Interface('aionowplaying')
+    mp.set_property(PropertyName.CanQuit, True)
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(mp.start())
```

### Comparing `aionowplaying-0.9.2/LICENSE.txt` & `aionowplaying-0.9.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
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
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `aionowplaying-0.9.2/pyproject.toml` & `aionowplaying-0.9.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-[tool.poetry]
-name = "aionowplaying"
-version = "0.9.2"
-license = "GPL-3.0-only"
-description = "A cross-platform Now Playing client"
-authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
-keywords = ["nowplaying", "mpris"]
-readme = "README.md"
-repository = "https://github.com/BruceZhang1993/aionowplaying"
-
-[tool.poetry.dependencies]
-python = ">=3.7,<3.11"
-pydantic = "*"
-dbus-next = { version = "*", platform = "linux" }
-winrt = { version = "*", platform = "win32" }
-pyobjc = { version = "*", platform = "darwin" }
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-pytest-asyncio = "*"
-poetry2setup = "^1.0.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/BruceZhang1993/aionowplaying/issues"
+[tool.poetry]
+name = "aionowplaying"
+version = "0.9.3"
+license = "GPL-3.0-only"
+description = "A cross-platform Now Playing client"
+authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
+maintainers = ["Bruce Zhang <zttt183525594@gmail.com>"]
+keywords = ["nowplaying", "mpris"]
+readme = "README.md"
+repository = "https://github.com/BruceZhang1993/aionowplaying"
+
+[tool.poetry.dependencies]
+python = ">=3.7,<3.11"
+pydantic = "*"
+dbus-next = { version = "*", platform = "linux" }
+winsdk = { version = "*", platform = "win32" }
+pyobjc = { version = "*", platform = "darwin" }
+
+[tool.poetry.dev-dependencies]
+pytest = "*"
+pytest-asyncio = "*"
+poetry2setup = "^1.0.0"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/BruceZhang1993/aionowplaying/issues"
```

### Comparing `aionowplaying-0.9.2/PKG-INFO` & `aionowplaying-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: aionowplaying
-Version: 0.9.2
+Version: 0.9.3
 Summary: A cross-platform Now Playing client
 Home-page: https://github.com/BruceZhang1993/aionowplaying
 License: GPL-3.0-only
 Keywords: nowplaying,mpris
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
+Maintainer: Bruce Zhang
+Maintainer-email: zttt183525594@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dbus-next; sys_platform == "linux"
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dbus-next ; sys_platform == "linux"
 Requires-Dist: pydantic
-Requires-Dist: pyobjc; sys_platform == "darwin"
-Requires-Dist: winrt; sys_platform == "win32"
+Requires-Dist: pyobjc ; sys_platform == "darwin"
+Requires-Dist: winsdk ; sys_platform == "win32"
 Project-URL: Bug Tracker, https://github.com/BruceZhang1993/aionowplaying/issues
 Project-URL: Repository, https://github.com/BruceZhang1993/aionowplaying
 Description-Content-Type: text/markdown
```

