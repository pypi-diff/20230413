# Comparing `tmp/neon_phal_plugin_linear_led-0.1.0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_linear_led-0.1.1a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10511 bytes, number of entries: 9
--rw-r--r--  2.0 unx    12536 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led/__init__.py
--rw-r--r--  2.0 unx     2662 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led/neopixel_led.py
--rw-r--r--  2.0 unx     2455 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led/smbus_led.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3639 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      229 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      899 b- defN 23-Jan-25 00:43 neon_phal_plugin_linear_led-0.1.0.dist-info/RECORD
-9 files, 24174 bytes uncompressed, 8917 bytes compressed:  63.1%
+Zip file size: 11151 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    16507 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/__init__.py
+-rw-r--r--  2.0 unx     2662 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/neopixel_led.py
+-rw-r--r--  2.0 unx     2455 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/smbus_led.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3641 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      229 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      911 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD
+9 files, 28159 bytes uncompressed, 9533 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: neon_phal_plugin_linear_led/neopixel_led.py
 Comment: 
 
 Filename: neon_phal_plugin_linear_led/smbus_led.py
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/METADATA
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/WHEEL
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/top_level.txt
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.0.dist-info/RECORD
+Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_linear_led/__init__.py

```diff
@@ -34,14 +34,25 @@
 from ovos_plugin_manager.hardware.led import Color, AbstractLed
 from ovos_plugin_manager.hardware.led.animations import BreatheLedAnimation, \
     FillLedAnimation, BlinkLedAnimation, AlternatingLedAnimation,\
     animations, LedAnimation
 from ovos_utils.network_utils import is_connected
 
 
+def transient_animation(func):
+    """
+    Mark a method as transient and check for persistent states on animation end.
+    """
+    def wrapper(self, *args, **kwargs):
+        func(self, *args, **kwargs)
+        self.check_state()
+
+    return wrapper
+
+
 class LinearLed(PHALPlugin):
     def __init__(self, led: AbstractLed, bus=None, config=None, name=None):
         self.leds = led
         self.leds.fill(Color.BLACK.as_rgb_tuple())
 
         self._is_muted = False
         self._internet_disconnected = not is_connected()
@@ -173,20 +184,40 @@
         self.bus.on('recognizer_loop:utterance', self.on_utterance)
         self.bus.on('mycroft.skill.handler.start', self.on_skill_handler_start)
         self.bus.on('complete_intent_failure', self.on_complete_intent_failure)
         self.bus.on('mycroft.speech.recognition.unknown',
                     self.on_recognition_unknown)
         # TODO: Define method to stop any active/queued animations
 
+    def check_state(self):
+        """
+        Check current state and show a persistent animation as appropriate.
+        """
+        if self._is_muted:
+            LOG.debug("Mic Muted")
+            self.on_mic_mute()
+        elif self._internet_disconnected:
+            LOG.debug("Internet Disconnected")
+            self.on_no_internet()
+
+    @transient_animation
     def on_fully_offline(self, message):
+        """
+        Handle an event notifying the user selected offline operation
+        :param message: Message object
+        """
         LOG.info("Wifi plugin notified fully offline mode selected")
         self._internet_disconnected = False
         self._disconnected_animation.stop()
 
     def on_no_internet(self, message=None):
+        """
+        Handle an event notifying internet connection was unexpectedly lost.
+        :param message: Message object
+        """
         LOG.debug("Bus notified no internet")
         if self._internet_disconnected:
             LOG.debug(f"Already disconnected")
             return
         self._internet_disconnected = True
         message = message.forward("ovos.phal.wifi.plugin.status") if \
             message else Message("ovos.phal.wifi.plugin.status")
@@ -195,108 +226,202 @@
             LOG.info(f"Watchdog inactive: {resp.data}")
             return
         LOG.debug(f"Starting Internet Disconnected Animation")
         # TODO: Check ready settings and skill internet setting in config?
         with self._led_lock:
             self._disconnected_animation.start()
 
+    @transient_animation
     def on_internet_connected(self, message):
+        """
+        Handle an event notifying internet connection has been established.
+        :param message: Message object
+        """
         LOG.debug(f"Internet connection re-established")
         self._internet_disconnected = False
         self._disconnected_animation.stop()
 
+    @transient_animation
     def on_complete_intent_failure(self, message):
+        """
+        Handle an event notifying intent service failure.
+        :param message: Message object
+        """
         with self._led_lock:
             self._intent_error_animation.start(one_shot=True)
 
+    @transient_animation
     def on_recognition_unknown(self, message):
+        """
+        Handle an event notifying STT transcribed no words.
+        :param message: Message object
+        """
         with self._led_lock:
             self._speech_error_animation.start(one_shot=True)
 
+    @transient_animation
     def on_skill_handler_start(self, message):
+        """
+        Handle an event notifying a skill intent handler has been called.
+        :param message: Message object
+        """
         if self._handler_animation is not None:
             LOG.debug('handler animation')
             with self._led_lock:
                 self._handler_animation.start(one_shot=True)
 
+    @transient_animation
     def on_utterance(self, message):
         LOG.debug(f'utterance | {self._utterance_animation}')
+        """
+        Handle an event notifying an utterance is being processed.
+        :param message: Message object
+        """
         if self._utterance_animation is not None:
             LOG.debug('utterance animation')
             with self._led_lock:
                 self._utterance_animation.start(one_shot=True)
 
     def on_theme_update(self, message):
+        """
+        Handle an event notifying theme colors have been changed.
+        :param message: Message object
+        """
         LOG.debug(f"Updating theme color(s): {message.data}")
         try:
             color = message.data.get('secondaryColor')
             Color.set_theme(color)
             LOG.debug(f'LED Theme color set to {Color.THEME.as_rgb_tuple()}')
         except Exception as e:
             LOG.exception(e)
 
+    @transient_animation
     def on_show_animation(self, message):
+        """
+        Handle an event requesting a particular animation be displayed.
+        :param message: Message object containing animation request
+        """
         animation_name = message.data.get('animation')
         color_name = message.data.get('color')
         timeout = message.data.get('timeout', 5)
         color = Color.from_name(color_name)
         LOG.debug(f'showing animation: {animation_name}')
         animation: LedAnimation = animations[animation_name](self.leds, color)
         with self._led_lock:
             animation.start(timeout)
             animation.stop()
 
+    @transient_animation
     def on_mic_error(self, message):
+        """
+        Handle an event notifying a microphone error has occurred.
+        :param message: Message object
+        """
         err = message.data.get('error')
         LOG.debug(f'mic error: {err}')
         with self._led_lock:
             if err == 'mic_sw_muted':
                 self._mic_muted_animation.start()
                 self.leds.fill(self.mute_color.as_rgb_tuple())
             else:
                 LOG.info(f"unknown mic error: {err}")
 
-    def on_mic_mute(self, message):
+    def on_mic_mute(self, message=None):
+        """
+        Handle an event notifying the mic has been muted. (persistent LED state)
+        :param message: Message object
+        """
         LOG.debug('muted')
         with self._led_lock:
             self._is_muted = True
             self._mute_animation.start()
 
+    @transient_animation
     def on_mic_unmute(self, message):
+        """
+        Handle an event notifying the mic has been unmuted.
+        :param message: Message object
+        """
         LOG.debug('unmuted')
         with self._led_lock:
             self._is_muted = False
             self._unmute_animation.start()
 
+    @transient_animation
     def on_volume_increase(self, message):
+        """
+        Handle an event notifying volume was increased.
+        :param message: Message object
+        """
         # TODO: Get volume and fill LEDs accordingly
         pass
 
+    @transient_animation
     def on_volume_decrease(self, message):
+        """
+        Handle an event notifying volume was decreased.
+        :param message: Message object
+        """
         # TODO: Get volume and fill LEDs accordingly
         pass
 
     def on_record_begin(self, message=None):
+        """
+        Handle an event notifying recording has begun (wake word detected).
+        :param message: Message object
+        """
         LOG.debug('record begin')
         with self._led_lock:
             self._listen_animation.start(self.listen_timeout_sec)
 
+    @transient_animation
     def on_record_end(self, message=None):
+        """
+        Handle an event notifying utterance recording has ended.
+        :param message: Message object
+        """
         LOG.debug('record end')
         self._listen_animation.stop()
 
+    @transient_animation
     def on_awake(self, message=None):
+        """
+        Handle an event notifying the listener has woken up.
+        :param message: Message object
+        """
         with self._led_lock:
             self._awake_animation.start()
 
     def on_sleep(self, message=None):
+        """
+        Handle an event notifying listener has gone to sleep. (persistent)
+        :param message: Message object
+        """
         with self._led_lock:
             self._sleep_animation.start()
 
+    @transient_animation
     def on_reset(self, message=None):
+        """
+        Handle an event requesting LEDs be reset. Inserts a black fill animation
+        before returning to a persistent state.
+        :param message: Message object
+        """
+        # TODO: interrupt any other animations?
         self.leds.fill(Color.BLACK.as_rgb_tuple())
 
+    @transient_animation
     def on_system_reset(self, message=None):
+        """
+        Handle an event requesting LEDs be reset. Inserts a black fill animation
+        before returning to a persistent state.
+        :param message: Message object
+        """
+        # TODO: interrupt any other animations?
         self.leds.fill(Color.BLACK.as_rgb_tuple())
 
     def shutdown(self):
+        """
+        Handle a shutdown event. Reset LED's to an off state.
+        """
+        # TODO: interrupt any other animations?
         self.leds.fill(Color.BLACK.as_rgb_tuple())
```

## Comparing `neon_phal_plugin_linear_led-0.1.0.dist-info/LICENSE.md` & `neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_linear_led-0.1.0.dist-info/METADATA` & `neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear-led
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `neon_phal_plugin_linear_led-0.1.0.dist-info/RECORD` & `neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-neon_phal_plugin_linear_led/__init__.py,sha256=qwJw7vm2ZTHUKICk_-HvFMspWP_A8PiYAs4Pvt6zIvI,12536
+neon_phal_plugin_linear_led/__init__.py,sha256=JUQMmZi_NoTCU34cIO5lA3R3FRYO9Ad7IRtPvoDqEuU,16507
 neon_phal_plugin_linear_led/neopixel_led.py,sha256=j6tf2UQ8zO3zjj1MJkYbnxSKcRDUhISnKh_yBoeHavU,2662
 neon_phal_plugin_linear_led/smbus_led.py,sha256=DxXb5fuu6uvzX92Br3MEn5CbmF4KWVbTn2OvBQ9xUIQ,2455
-neon_phal_plugin_linear_led-0.1.0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_linear_led-0.1.0.dist-info/METADATA,sha256=roNTKUr6p5dbkdSyDUO8CPNXJzus0n_2Vk2vHyprFZ8,3639
-neon_phal_plugin_linear_led-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-neon_phal_plugin_linear_led-0.1.0.dist-info/entry_points.txt,sha256=kam9ztzRLdfMrjVQYjtbcVmtJZTxufNnjnWqMAH992o,229
-neon_phal_plugin_linear_led-0.1.0.dist-info/top_level.txt,sha256=Tbx4PyK54fa4KBJAb7RI0xMAqRPoUNmLHSEkVtQfzJ8,28
-neon_phal_plugin_linear_led-0.1.0.dist-info/RECORD,,
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA,sha256=6xxXRPQoUSN3oahWgW9-vlkTuLEUMOEaFPep1sEiPlM,3641
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt,sha256=kam9ztzRLdfMrjVQYjtbcVmtJZTxufNnjnWqMAH992o,229
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt,sha256=Tbx4PyK54fa4KBJAb7RI0xMAqRPoUNmLHSEkVtQfzJ8,28
+neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD,,
```

