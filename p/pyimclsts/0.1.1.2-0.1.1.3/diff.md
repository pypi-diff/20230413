# Comparing `tmp/pyimclsts-0.1.1.2.tar.gz` & `tmp/pyimclsts-0.1.1.3.tar.gz`

## Comparing `pyimclsts-0.1.1.2.tar` & `pyimclsts-0.1.1.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/example/followRef.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/__init__.py
--rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/_base_templates.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/core.py
--rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/extract.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/extractutils.py
--rw-r--r--   0        0        0    31222 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/src/pyimclsts/network.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/LICENSE
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/example/followRef.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/example/lsf2csv.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/example/selectedlsf2csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/__init__.py
+-rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/_base_templates.py
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/core.py
+-rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/extract.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/extractutils.py
+-rw-r--r--   0        0        0    32250 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/src/pyimclsts/network.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/LICENSE
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 pyimclsts-0.1.1.3/PKG-INFO
```

### Comparing `pyimclsts-0.1.1.2/example/followRef.py` & `pyimclsts-0.1.1.3/example/followRef.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,25 @@
             request.info = "MyPlan"
             
             print("Requesting Follow Reference Manuever...")
             print(request)
             send_callback(request, dst = self.peers.get(self.target, 0xFFFF))
 
     def send_refs(self, send_callback):
-        referenceToFollow = pg.messages.Reference()
+        if self.EstimatedState is not None:
+            referenceToFollow = pg.messages.Reference()
 
-        referenceToFollow.flags = pg.messages.Reference.FLAGS.LOCATION | pg.messages.Reference.FLAGS.SPEED | pg.messages.Reference.FLAGS.Z
-        referenceToFollow.speed = pg.messages.DesiredSpeed(value=50, speed_units=pg.enumerations.SpeedUnits.PERCENTAGE)
-        referenceToFollow.z = pg.messages.DesiredZ(value=1, z_units=pg.enumerations.ZUnits.DEPTH)
-        referenceToFollow.lat = self.EstimatedState.lat + 0.001
-        referenceToFollow.lon = self.EstimatedState.lon
-        referenceToFollow.radius = 0
+            referenceToFollow.flags = pg.messages.Reference.FLAGS.LOCATION | pg.messages.Reference.FLAGS.SPEED | pg.messages.Reference.FLAGS.Z
+            referenceToFollow.speed = pg.messages.DesiredSpeed(value=50, speed_units=pg.enumerations.SpeedUnits.PERCENTAGE)
+            referenceToFollow.z = pg.messages.DesiredZ(value=1, z_units=pg.enumerations.ZUnits.DEPTH)
+            referenceToFollow.lat = self.EstimatedState.lat + 0.001
+            referenceToFollow.lon = self.EstimatedState.lon
+            referenceToFollow.radius = 0
 
-        send_callback(referenceToFollow, dst = self.peers.get(self.target, 0xFFFF))
+            send_callback(referenceToFollow, dst = self.peers.get(self.target, 0xFFFF))
 
     def update_vehicle_state(self, msg : pg.messages.EstimatedState, send_callback):
         self.EstimatedState = msg
 
     def update_plan_state(self, msg : pg.messages.FollowRefState, send_callback):
         self.FollowRefState = msg
     
@@ -67,17 +68,16 @@
     vehicle = FollowRef_Vehicle('lauv-xplore-2')
 
     sub = p.subscriber(conn)
 
     # Set a delay, so that we receive the Announcements
     sub.call_once(vehicle.request_followRef, 5)
 
-    sub.subscribe_async(pg.messages.Announce, vehicle.update_peers)
-    sub.subscribe_async(pg.messages.EstimatedState, vehicle.update_vehicle_state)
-    sub.subscribe_async(pg.messages.FollowReference, vehicle.update_plan_state)
-    #sub.subscribe_async(pg.messages.PlanControlState, lambda msg, c : print(msg))
+    sub.subscribe_async(vehicle.update_peers, pg.messages.Announce)
+    sub.subscribe_async(vehicle.update_vehicle_state, pg.messages.EstimatedState)
+    sub.subscribe_async(vehicle.update_plan_state, pg.messages.FollowReference)
 
     sub.periodic_async(vehicle.send_refs, 1)
 
     #sub.periodic_async(lambda _ : print(vehicle.peers), 1)
 
     sub.run()
```

### Comparing `pyimclsts-0.1.1.2/src/pyimclsts/_base_templates.py` & `pyimclsts-0.1.1.3/src/pyimclsts/_base_templates.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.2/src/pyimclsts/extract.py` & `pyimclsts-0.1.1.3/src/pyimclsts/extract.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.2/src/pyimclsts/extractutils.py` & `pyimclsts-0.1.1.3/src/pyimclsts/extractutils.py`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.2/src/pyimclsts/network.py` & `pyimclsts-0.1.1.3/src/pyimclsts/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 import asyncio as _asyncio
 import time as _time
 
 import importlib.util as _import
 import sys as _sys
 import os as _os
 
-import pyimclsts.core as core
+import pyimclsts.core as _core
 
-module_name = 'pyimc_generated' # and folder name
-location = _os.getcwd() + '/' + module_name + '/__init__.py'
+_module_name = 'pyimc_generated' # and folder name
+_location = _os.getcwd() + '/' + _module_name + '/__init__.py'
 
-spec = _import.spec_from_file_location(module_name, location)
+_spec = _import.spec_from_file_location(_module_name, _location)
 
-_pg = _import.module_from_spec(spec)
-_sys.modules[module_name] = _pg
-spec.loader.exec_module(_pg)
+_pg = _import.module_from_spec(_spec)
+_sys.modules[_module_name] = _pg
+_spec.loader.exec_module(_pg)
 
 def unpack(message : bytes, *, is_big_endian : bool, is_field_message : bool = False, fast_mode : bool = False) -> _pg._base_templates.IMC_message:
     '''Expects a serializable (= exactly long (header + fields + CRC)) string of bits, but may fail (returns None)
     if the string is invalid. 
     
     Fast mode skips all type checking performed by the descriptor by directly invoking the constructor.
     '''
-    unpack_functions = core.unpack_functions_big if is_big_endian else core.unpack_functions_little
+    unpack_functions = _core.unpack_functions_big if is_big_endian else _core.unpack_functions_little
     cursor = 0
     
     if not is_field_message:
         # deserialize header
         (m, size) = unpack_functions['header'](message[cursor:])
         deserialized_header = _pg._base_templates.header_data(*m)
         cursor += size
         # Magic number 2 = CRC size in bytes
         contents = message[:-2]
         crc = unpack_functions['uint16_t'](message[-2:])[0]
-        crc_valid = crc == core.CRC16IMB(contents)
+        crc_valid = crc == _core.CRC16IMB(contents)
     else:
         crc_valid = None
     
     # check CRC-16.
     if crc_valid or is_field_message:
         if is_field_message:
             msgid = unpack_functions['uint16_t'](message[cursor:cursor+2])[0]
@@ -120,125 +120,69 @@
         if not is_field_message:
             message_class._header = deserialized_header
             return message_class
         else:
             return (message_class, cursor)
     return None
 
-async def _async_wrapper(func, *args):
-    return func(*args)
+# Re-export some classes:
 
-class base_IO_interface:
-    '''
-        An 'abstract'* class that describes the basic implementation of an I/O interface.
+tcp_interface = _core.tcp_interface
+file_interface = _core.file_interface
 
-        * Not really abstract as in Java, but consider it so. 
-        I will not use abc and its decorators.
-    '''
-    __slots__ = ['_input', '_output', '_o', '_i']
+class _message_bus():
+    '''Injected dependency to 'simplify' common functionalities'''
+    __slots__ = ['_io_interface', '_timeout', '_big_endian', '_block_outgoing']
 
-    def __init__(self, _input : any = None, _output : any = None) -> None:
-        self._input = _input
-        self._output = _output
+    def __init__(self, IO_interface : _core.base_IO_interface, timeout = 60, big_endian=False):
+        self._io_interface = IO_interface
+        self._timeout = timeout
 
-    async def open(self) -> None:
-        raise NotImplementedError
+        # mode to send messages
+        self._big_endian = big_endian
+        self._block_outgoing = False
     
-    async def read(self, n_bytes : int) -> bytes:
-        raise NotImplementedError
-        
-    async def write(self, byte_string : bytes) -> None:
-        raise NotImplementedError
+    def __enter__(self):
+        raise NotImplemented
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        raise NotImplemented
     
-    async def close(self) -> None:
-        raise NotImplementedError
+    def block_outgoing(self):
+        '''Blocks (and discards) outgoing messages'''
+        self._block_outgoing = True
+    def unblock_outgoing(self):
+        '''Unblock outgoing messages'''
+        self._block_outgoing = False
 
-class file_interface(base_IO_interface):
-    '''
-        A minimal implemenation of a file interface. Receives an input
-        file name and (optionally) an output file name, to which it appends.
-    '''
-    __slots__ = ['_input', '_output', '_o', '_i']
-
-    def __init__(self, _input : any = None, _output : any = None) -> None:
-        self._input = _input
-        self._output = _output
-
-    async def open(self) -> None:
-        self._o = open(self._output, 'ab') if self._output is not None else None
-        self._i = open(self._input, 'rb')
-    
-    async def read(self, n_bytes : int) -> bytes:
-        r = self._i.read(n_bytes)
-        if r == b'':
-            raise EOFError('End of File reached')
-        return r
-        
-    async def write(self, byte_string : bytes) -> None:
-        if self._o is not None:
-            self._o.write(byte_string)
-    
-    async def close(self) -> None:
-        if self._o is not None:
-            self._o.close()
-        self._i.close()
-
-class tcp_interface(base_IO_interface):
-    '''
-        A minimal implementation of a TPC interface. It wraps a
-        connection established with the asyncio module.
-    '''
-    __slots__ = ['_ip', '_port', '_reader', '_writer']
-
-    def __init__(self, ip : str, port : int) -> None:
-        self._ip = ip
-        self._port = port
-
-    async def open(self) -> None:
-        self._reader, self._writer = await _asyncio.open_connection(self._ip, self._port)
-    
-    async def read(self, n_bytes : int) -> bytes:
-        r = await self._reader.read(n_bytes)
-        if r == b'':
-            raise EOFError('Connection returned empty byte string')
-        return r
-        
-    async def write(self, byte_string : bytes) -> None:
-        self._writer.write(byte_string)
-        await self._writer.drain()
-    
-    async def close(self) -> None:
-        self._writer.close()
-        await self._writer.wait_closed()
+    def send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+                        dst : int = None, dst_ent : int = None) -> None:
+        '''Wrapper around a queue (actually a pipe end).'''
+        if not self.block_outgoing:
+            self._send(message.pack(is_big_endian=self._big_endian, src = src, src_ent = src_ent, 
+                        dst = dst, dst_ent = dst_ent))
+    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+                        dst : int = None, dst_ent : int = None) -> None:
+        raise NotImplemented
 
-class message_bus():
+class message_bus(_message_bus):
     '''
         Send and receives messages as bytes, but exposes them as IMC messages
 
         Receives a base_IO_interface, which must implement open(), read(), write() and close()
         asynchronous methods.
 
         Starts another process that continuously reads/writes to the base_IO_interface.
     '''
 
-    __slots__ = ['_io_interface', '_timeout', '_child_end', '_parent_end', '_child_process', '_keep_running', '_big_endian']
-    
-    def __init__(self, IO_interface : base_IO_interface, timeout = 60, big_endian=False):
-        super().__init__()
-
-        self._io_interface = IO_interface
-        self._timeout = timeout
-
-        # mode to send messages
-        self._big_endian = big_endian
+    __slots__ = ['_child_end', '_parent_end', '_child_process', '_keep_running', '_big_endian']
 
     def _external_listener_loop(self, child_end, timeout : int, keep_running : _multiprocessing.Value):
         '''All code bellow is executed in a separate process.'''
 
-        async def consume_output(io_interface : base_IO_interface):
+        async def consume_output(io_interface : _core.base_IO_interface):
             '''Continuously read the pipe end to send messages'''
             
             while keep_running.value:
                 try:
                     has_message = child_end.poll()
                     while has_message:
                         message = child_end.recv_bytes()
@@ -247,15 +191,15 @@
                 finally:
                     pass
                 # Yield an exit point to the event loop
                 await _asyncio.sleep(0)
             
             print("Writer stream has been closed.")
 
-        async def consume_input(io_interface : base_IO_interface):
+        async def consume_input(io_interface : _core.base_IO_interface):
             '''Continuously read the socket to deserialize messages'''
 
             buffer = bytearray()
             while keep_running.value:
                 try:
                     # magic number: 6 = sync number + (msgid + msgsize) size in bytes
                     if len(buffer) < 6:
@@ -266,30 +210,30 @@
                         size = int.from_bytes(buffer[4:6], byteorder='little')
                         # magic number: 22 = 20(header size) + 2(CRC) sizes in bytes.
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         # Validate message, but do not unpack yet
                         unparsed_msg = bytes(buffer[:(size + 22)])
-                        if core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='little'):
+                        if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='little'):
                             child_end.send_bytes(unparsed_msg)
                             # eliminate message from buffer
                             del buffer[:size + 22]
                         else:
                             # deserialization failed:
                             # sync number is not followed by a sound/valid message. Remove it from buffer
                             # to look for next message
                             del buffer[:2]
                     elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base_templates._sync_number:
                         size = int.from_bytes(buffer[4:6], byteorder='big')
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         unparsed_msg = bytes(buffer[:(size + 22)])
-                        if core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
+                        if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
                             child_end.send_bytes(unparsed_msg)
                             del buffer[:size + 22]
                         else:
                             del buffer[:2]
                     else:
                         # buffer does not start with a sync number. Remove it to search
                         # for a valid sync number.
@@ -352,18 +296,16 @@
     def close(self, max_wait : float = 1) -> None:        
         with self._keep_running.get_lock():
             self._keep_running.value = False
         
         self._child_process.join()
         self._child_process.close()
 
-    def send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
-        '''Wrapper around a queue (actually a pipe end).'''
-        
         self._parent_end.send_bytes(message.pack(is_big_endian=self._big_endian, src = src, src_ent = src_ent, 
                         dst = dst, dst_ent = dst_ent))
 
     def recv(self) -> _pg._base_templates.base_message:
         '''Wrapper around a queue (actually a pipe end). Blocks until a message is available.
         The _external_listener_loop is supposed to send complete messages (as per multiprocessing 
         documentation).'''       
@@ -392,42 +334,33 @@
         self.close()
         if exc_type == EOFError:
             print('Child process has been closed due to end of file.')
             return True
         print('Child process has been closed.')
         return None
 
-class message_bus_st():
+class message_bus_st(_message_bus):
     '''
         Send and receives messages as bytes, but exposes them as IMC messages
 
         Receives a base_IO_interface, which must implement open(), read(), write() and close()
         asynchronous methods.
 
         DOES NOT start another process. Runs in the main process.
     '''
 
-    __slots__ = ['_io_interface', '_timeout', '_writer_queue', '_reader_queue', '_keep_running', '_big_endian', '_task']
+    __slots__ = ['_writer_queue', '_reader_queue', '_keep_running', '_big_endian', '_task']
     
-    def __init__(self, IO_interface : base_IO_interface, timeout = 60, big_endian=False):
-        super().__init__()
-
-        self._io_interface = IO_interface
-        self._timeout = timeout
-
-        # mode to send messages
-        self._big_endian = big_endian
-
     async def open(self):
         self._keep_running = True
 
         self._writer_queue = _asyncio.Queue()
         self._reader_queue = _asyncio.Queue()
 
-        async def consume_output(io_interface : base_IO_interface):
+        async def consume_output(io_interface : _core.base_IO_interface):
             '''Continuously read the pipe end to send messages'''
             
             while self._keep_running:
                 try:
                     # flush queue or wait.
                     while not self._writer_queue.empty():
                         message = await self._writer_queue.get()
@@ -435,15 +368,15 @@
                     else:
                         await _asyncio.sleep(0.5)
                 finally:
                     pass
             
             print("Writer stream has been closed.")
 
-        async def consume_input(io_interface : base_IO_interface):
+        async def consume_input(io_interface : _core.base_IO_interface):
             '''Continuously read the socket to deserialize messages'''
             
             buffer = bytearray()
             while self._keep_running:
                 try:
                     # magic number: 6 = sync number + (msgid + msgsize) size in bytes
                     if len(buffer) < 6:
@@ -454,30 +387,30 @@
                         size = int.from_bytes(buffer[4:6], byteorder='little')
                         # magic number: 22 = 20(header size) + 2(CRC) sizes in bytes.
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         # Validate message, but do not unpack yet
                         unparsed_msg = bytes(buffer[:(size + 22)])
-                        if core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='little'):
+                        if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='little'):
                             await self._reader_queue.put(unparsed_msg)
                             # eliminate message from buffer
                             del buffer[:size + 22]
                         else:
                             # deserialization failed:
                             # sync number is not followed by a sound/valid message. Remove it from buffer
                             # to look for next message
                             del buffer[:2]
                     elif int.from_bytes(buffer[:2], byteorder='big') == _pg._base_templates._sync_number:
                         size = int.from_bytes(buffer[4:6], byteorder='big')
                         read_size = max(size + 22 - len(buffer), 0)
                         buffer += await io_interface.read(read_size)
 
                         unparsed_msg = bytes(buffer[:(size + 22)])
-                        if core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
+                        if _core.CRC16IMB(unparsed_msg[:-2]) == int.from_bytes(unparsed_msg[-2:], byteorder='big'):
                             await self._reader_queue.put(unparsed_msg)
                             del buffer[:size + 22]
                         else:
                             del buffer[:2]
                     else:
                         # buffer does not start with a sync number. Remove it to search
                         # for a valid sync number.
@@ -509,19 +442,16 @@
         self._task = _asyncio.create_task(main_loop())
     
     def close(self, max_wait : float = 1) -> None:
         self._keep_running = False
         self._task.cancel()
         print('Message Bus has been closed.')
 
-    def send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
+    def _send(self, message : _pg._base_templates.base_message, *, src : int = None, src_ent : int = None, 
                         dst : int = None, dst_ent : int = None) -> None:
-        '''Wrapper around a queue (actually a pipe end).'''
-        
-        # this looks dangerous (But it is an infinite queue)
         self._writer_queue.put_nowait(message.pack(is_big_endian=self._big_endian, src = src, src_ent = src_ent, 
                         dst = dst, dst_ent = dst_ent))
 
     async def recv(self) -> _pg._base_templates.base_message:
         '''Wrapper around a queue (actually a pipe end). Blocks until a message is available.
         The _external_listener_loop is supposed to send complete messages (as per multiprocessing 
         documentation).'''
@@ -537,100 +467,172 @@
                 msg = unpack(msg, is_big_endian=False, fast_mode=True)
             return msg
             
     def poll(self, timeout : int = 0) -> bool:
         '''Extra function to check whether there are any available messages.
         '''
         return not self._reader_queue.empty()
-
-    def __enter__(self):
-        self.open()
-        return self
     
     def __exit__(self, exc_type, exc_value, exc_tb):
         self.close()
         if exc_type == EOFError:
             print('Message bus event loop has been closed due to end of file.')
             return True
         print('Message bus event loop has been closed.')
         return None
 
 class subscriber:
 
-    __slots__ = ['msg_manager', '_subscriptions', '_subscripted_all', '_periodic', '_call_once', '_use_mp']
+    __slots__ = ['_msg_manager', '_subscriptions', '_subscripted_all', '_periodic', '_call_once', '_use_mp', '_peers', '_src2name']
 
-    def __init__(self, IO_interface : base_IO_interface, *,big_endian=False, use_mp = False) -> None:
+    def __init__(self, IO_interface : _core.base_IO_interface, *,big_endian=False, use_mp = False) -> None:
         self._use_mp = use_mp
         if self._use_mp:
-            self.msg_manager = message_bus(IO_interface, big_endian)
+            self._msg_manager = message_bus(IO_interface, big_endian)
         else:
-            self.msg_manager = message_bus_st(IO_interface, big_endian)
+            self._msg_manager = message_bus_st(IO_interface, big_endian)
         self._subscriptions = dict()
         self._subscripted_all = []
         self._periodic = []
         self._call_once = []
-    
-    def _event_loop(self):
 
-        async def periodic_wrapper_coro(_period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
-            loop = _asyncio.get_running_loop()
-            while True:
-                last_exec = loop.time()
-                await f(send_callback)
-                now = loop.time()
-                await _asyncio.sleep(max(last_exec - now + _period, 0))
+        # a dictionary of {vehicle name : {'src' : 1, 'entities' : { 1 : 'Entity name'...} ...}}
+        self._peers = dict()
+        # a dictionary of {2: 'vehicle name'}
+        self._src2name = dict()
+        
+        self.subscribe_async(self._abort, _pg.messages.Abort)
+        
+        self.call_once(self._queryEntityList, delay=1)
+        self.periodic_async(self._queryEntityList, period=300)
+        self.subscribe_async(self._update_peers, _pg.messages.EntityList)
+        self.subscribe_async(self._update_peers, _pg.messages.Announce)
+
+    async def _periodic_wrapper_coro(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+        loop = _asyncio.get_running_loop()
+        while True:
+            last_exec = loop.time()
+            await f(send_callback)
+            now = loop.time()
+            await _asyncio.sleep(max(last_exec - now + _period, 0))
                 
-        async def periodic_wrapper(_period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+    async def _periodic_wrapper(self, _period : float, f : _typing.Callable, send_callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+        loop = _asyncio.get_running_loop()
+        f(send_callback)
+        while True:
+            await _asyncio.sleep(_period)
+            loop.call_later(_period, f, send_callback)
+
+    async def _event_loop(self):
+        msg_mgr = self._msg_manager
+        try:
+            if self._use_mp:
+                msg_mgr.open()
+            else:
+                await msg_mgr.open()
             loop = _asyncio.get_running_loop()
-            f(send_callback)
-            while True:
-                await _asyncio.sleep(_period)
-                loop.call_later(_period, f, send_callback)
 
-        async def main_loop():
-            msg_mgr = self.msg_manager
-            try:
-                if self._use_mp:
-                    msg_mgr.open()
+            for f, delay in self._call_once:
+                if delay is not None:
+                    loop.call_later(delay, f, msg_mgr.send)
                 else:
-                    await msg_mgr.open()
-                loop = _asyncio.get_running_loop()
+                    f(msg_mgr.send)
+            
+            # Binding references to background task objects so that they are not garbage collected
+            tasks = []
+            for f, period in self._periodic:
+                if _inspect.iscoroutinefunction(f):
+                    tasks.append(loop.create_task(self._periodic_wrapper_coro(period, f, msg_mgr.send)))
+                elif callable(f):
+                    tasks.append(loop.create_task(self._periodic_wrapper(period, f, msg_mgr.send)))
+                else:
+                    print(f'Warning: Given function {f} is neither _typing.Callable nor a coroutine.')
 
-                for f, delay in self._call_once:
-                    if delay is not None:
-                        loop.call_later(delay, f, msg_mgr.send)
-                    else:
-                        f(msg_mgr.send)
+            while True:
+                msg = msg_mgr.recv() if self._use_mp else await msg_mgr.recv()
+                if msg._header.mgid in self._subscriptions:
+                    for f in self._subscriptions[msg._header.mgid]:
+                        if self._validate_call(msg, f[1], f[2]):
+                            await f[0](msg, msg_mgr.send)
                 
-                tasks = []
-                for f, period in self._periodic:
-                    if _inspect.iscoroutinefunction(f):
-                        tasks.append(loop.create_task(periodic_wrapper_coro(period, f, msg_mgr.send)))
-                    elif callable(f):
-                        tasks.append(loop.create_task(periodic_wrapper(period, f, msg_mgr.send)))
-                    else:
-                        print(f'Warning: Given function {f} is neither _typing.Callable nor a coroutine.')
+                [await f[0](msg, msg_mgr.send) for f in self._subscripted_all if self._validate_call(msg, f[1], f[2])]
+                # Offer an exit point
+                await _asyncio.sleep(0)
+        except EOFError:
+            print('Stream has ended.')
+        finally:
+            msg_mgr.close()
 
-                while True:
-                    msg = msg_mgr.recv() if self._use_mp else await msg_mgr.recv()
-                    if msg._header.mgid in self._subscriptions:
-                        for f in self._subscriptions[msg._header.mgid]:
-                            await f(msg, msg_mgr.send)
-                    
-                    [f(msg, msg_mgr.send) for f in self._subscripted_all]
-                    # Offer an exit point
-                    await _asyncio.sleep(0)
-            except EOFError:
-                print('Stream has ended.')
-            finally:
-                msg_mgr.close()
-        _asyncio.run(main_loop())
+    async def _abort(self, msg, send_callback):
+        if msg._header is not None:
+            my_src = 0x4000 | (_core.get_initial_IP() & 0xFFFF)
+            if msg._header.dst == my_src:
+                loop = _asyncio.get_running_loop()
+                loop.close()
+
+    def _update_peers(self, msg : _typing.Union[_pg.messages.EntityList, _pg.messages.Announce], send_callback):
+        if msg._header is not None:
+            src = msg._header.src
+            
+            if isinstance(msg, _pg.messages.EntityList):
+                if msg.op == msg.OP.REPORT:
+                    entList =  [i.split(sep='=') for i in msg.list.split(sep=';')]
+                    entList = {k : int(v) for [k, v] in entList}
+
+                    name = self._src2name.get(src, None)
+                    if name is not None:
+                        # if it exists, update; else, create entry
+                        if self._peers.get(name, None) is not None:
+                            self._peers[name]['EntityList'] = entList
+                        else:
+                            self._peers[name] = {'EntityList' : entList}
+
+            elif isinstance(msg, _pg.messages.Announce):
+                name = msg.sys_name
 
-    def subscribe_async(self, msg_id : _typing.Union[int, _pg._base_templates.IMC_message], callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+                self._src2name[src] = name
+                # if it exists, update; else, create entry
+                if self._peers.get(name, None) is not None:
+                    self._peers[name]['src'] = src
+                else:
+                    self._peers[name] = {'src' : src}
+        else:
+            pass
+    
+    def _get_src(self, vehicle_name : str):
+        return self._peers[vehicle_name].get('src', None) if self._peers.get(vehicle_name, None) is not None else None
+    
+    def _get_src_ent(self, vehicle_name : str, entityName : str):
+        entityList = self._peers[vehicle_name].get('EntityList', None) if self._peers.get(vehicle_name, None) is not None else None
+        if entityList is not None:
+            return entityList.get(entityName, None)
+        return None
+    
+    def _queryEntityList(self, send):
+        query = _pg.messages.EntityList(op=_pg.messages.EntityList.OP.QUERY, list='')
+        send(query)
+    
+    def _validate_call(self, msg, desired_src : str, desired_src_ent : str) -> bool:
+        if desired_src is None and desired_src_ent is None:
+            return True
+        else:
+            correct_src = msg._header.src == self._get_src(desired_src) 
+            correct_src_ent = msg._header.src_ent == self._get_src_ent(desired_src, desired_src_ent)
+            
+            if (correct_src or correct_src_ent) and (desired_src is None or desired_src_ent is None):
+                return True
+            elif correct_src and correct_src_ent:
+                return True
+            
+        return False
+    
+    def subscribe_async(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], msg_id : _typing.Union[int, _pg._base_templates.IMC_message] = None, *, src : str = None, src_ent : str = None):
         '''Appends the callback to the list of subscripted functions.
+        msg_id can be provided as an int or the class of the message.
+        src and src_ent can be provided as strings. If None, then defaults to all.
         
         The main loop calls the function and pass the message and a callback to send messages.
         The return value is discarded and the function must have exactly two parameters (the message and the callback)
         and must not have additional parameters, to avoid unintended behavior*.
         
         *Due to python's pass-by-assignment, the argument values are evaluated when a function is called.
         This means that even if we pass, say "x", to the .subscribe_async method and then try to
@@ -646,69 +648,51 @@
         if isinstance(msg_id, _pg._base_templates.IMC_message):
             key = msg_id._Attributes.id
         elif isinstance(msg_id, int):
             key = msg_id
         elif _inspect.isclass(msg_id):
             if issubclass(msg_id, _pg._base_templates.IMC_message):
                 key = msg_id()._Attributes.id
+        elif msg_id is None:
+            pass
         else:
-            print(f'Warning: Given message id {msg_id} is not a valid message.')
+            print(f'Warning: Given message id {msg_id} is not a known message.')
             
-        if key is not None:
+        # There is either an explicit subscription (the key is not None) or 'all'
+        # (msg_id is None). There cannot be both nor neither.
+        if (key is not None) ^ (msg_id is None):
             c = None
             if _inspect.iscoroutinefunction(callback):
                 c = callback
             elif callable(callback):
-                c = _functools.partial(_async_wrapper, callback)
+                c = _functools.partial(_core._async_wrapper, callback)
             else:
                 print(f'Warning: Given function {callback} is neither callable nor a coroutine.')
             
             if c is not None:
-                if self._subscriptions.get(key, None):
-                    self._subscriptions[key].append(c)
+                if msg_id is None:
+                    self._subscripted_all.append((c, src, src_ent))
                 else:
-                    self._subscriptions[key] = [c]
-
-    def subscribe_all(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
-        '''Append to the list of callbacks that will be called to every *received* message
-        
-        The main loop calls the function and pass the message and a callback to send messages.
-        The return value is discarded and the function must have exactly two parameters (the message and the callback)
-        and must not have additional parameters, to avoid unintended behavior*.
-        '''
-        self._subscripted_all.append(callback)
+                    if self._subscriptions.get(key, None) is not None:
+                        self._subscriptions[key].append((c, src, src_ent))
+                    else:
+                        self._subscriptions[key] = [(c, src, src_ent)]
 
     def periodic_async(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], period = float):
         '''Add callback to a list to be called every period seconds. Function must take
         a send callback as parameter. This callback can be used to send messages.'''
         self._periodic.append((callback, period))
 
-    def subscribe_mp(self, msg_id : _typing.Union[int, _pg._base_templates.IMC_message], callback : _typing.Callable[[_pg._base_templates.IMC_message], None]):
+    def subscribe_mp(self, callback : _typing.Callable[[_pg._base_templates.IMC_message], None], msg_id : _typing.Union[int, _pg._base_templates.IMC_message], *, src : str = None, scr_ent : str = None):
         '''Calls a function and pass the message and a callback to send messages to it.
         Runs the given callback in a different process and should be used only with heavy load
         functions.
         '''
         raise NotImplemented
 
     def call_once(self, callback : _typing.Callable[[_typing.Callable[[_pg._base_templates.IMC_message], None]], None], delay : float = None):
         '''Calls the given callbacks as soon as the main loop starts or according to their delay in seconds.
         Callback parameters must be exactly one callback (that can be used to send messages).'''
         self._call_once.append((callback, delay))
 
     def run(self):
-        self._event_loop()
-
-if __name__ == '__main__':
-
-    io_interface = tcp_interface('localhost', 6006)
-    f_interface = file_interface('Data.lsf', 'output_test.lsf')
-    
-    s = subscriber(io_interface, big_endian=False)
-    s.subscribe_all(lambda x, y : print(x))
-    #s.subscribe_async(_pg.messages.EstimatedState, lambda x, y : print('oi'))
-
-    s.call_once(lambda _: print("hi"))
-    s.call_once(lambda _: print("hi2"), 1)
-
-    #s.periodic_async(lambda _ : print('oi'), 1)
-    #s.periodic_async(x, 2)
-    s.run()
+        _asyncio.run(self._event_loop())
```

### Comparing `pyimclsts-0.1.1.2/.gitignore` & `pyimclsts-0.1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.2/LICENSE` & `pyimclsts-0.1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimclsts-0.1.1.2/README.md` & `pyimclsts-0.1.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: pyimclsts
+Version: 0.1.1.3
+Summary: Python bindings of the IMC message schema
+Project-URL: Homepage, https://github.com/choiwd/pyimctrans
+Project-URL: Bug Tracker, https://github.com/choiwd/pyimctrans/issues
+Author: Choi Wang Dzak
+License: Copyright (c) 2023 Laboratório de Sistemas e Tecnologia Subaquática
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Keywords: IMC,IMC message protocol,LSTS
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: ifaddr~=0.2.0
+Requires-Dist: ipaddress~=1.0.23
+Description-Content-Type: text/markdown
+
 ## PyIMCtrans
 
 This tool reads the IMC schema from a XML file, locally creates files containing the messages and connects (imports) the main global machinery.
 
 See `/example` to check an example implementation of the Follow Reference maneuver.
 
 ### End-User
@@ -33,49 +69,24 @@
 ```python
 import pyimclsts.network as n
 
 conn = n.tcp_interface('localhost', 6006)
 sub = n.subscriber(conn)
 
 # for example:
-sub.subscribe_async(pg.messages.Announce, myfunction)
+sub.subscribe_async(myfunction, pg.messages.Announce)
 ```
 Check `/example` for further details.
 
 ### Change log:
-#### Version 0.1.1.2
-    - Parse command line arguments when pyimclsts.extract is called
-        - Accept a black- or whitelist
-        - Add minimal message list
-    - [EXPERIMENTAL] Add the option to use asyncio or multiprocessing when using the subscriber
-        - It's not clear-cut yet which approach is better, so both are provided until one proves to be superior
-
-#### Version 0.1.1.1
-    - Fix `Unknown message` being used for all messages
-    - Fix string (IMC plaintext) decode/encode
-    - Fix blocked termination when reading file
-
-#### Version 0.1.1
-    - Handle lost TCP connection/End of file:
-        - Gracefully terminates, if EOF (or equivalent) is encountered.
-    - Added a .subscribe_all() function.
-    - Added MIT License
-    - On extract, downloads IMC.xml definition from main git repository, when none is found.
-    - Added an 'Unknown message', used when a message with valid sync number and valid crc but unknown id is received.
-    - Update pyproject.toml
-        - Corrected version
-        - Added license
-        - Added keywords
-
-### Current TODO list:
-    - Improve README
-        - Add a description of the general functioning of the tool.
-    - Implement a message whitelist
-        - Although it works without problems, it is a little cumbersome to have +300 available messages.
-    - Implement logging?
-        - In the subscriber, message bus or the IO Interface?
-
-    - Notes:
-    - Users MUST be warned (documentation?) that the constructor does not type check, because the other operations (serialization) may fail if not correctly used. However, failure by type checking or failure by serialization is ultimately a failure during runtime, which begs the question: How to avoid a runtime error?
-    - Currently using IntFlag to make bitfields. It works, but does not throw exceptions when using an invalid combination of flags.
-        - Should it throw errors in this case?
+#### Version 0.1.1.3
+
+    - Hide imports and variables of core.py
+    - Move IO interface classes to core.py
+    - Implement .block_outgoing() through an injected dependency in the message bus
+    - Improve subscriber class:
+        - Exits when Abort message is received
+        - Queries Entity List when started
+        - Tracks src and src_ent and their corresponding names
+        - Removed .subscribe_all
+            - Same functionality can be achieved with .subscribe_async()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyimclsts-0.1.1.2/pyproject.toml` & `pyimclsts-0.1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyimclsts"
-version = "0.1.1.2"
+version = "0.1.1.3"
 authors = [
   { name = "Choi Wang Dzak" },
 ]
 description = "Python bindings of the IMC message schema"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["IMC", "IMC message protocol", "LSTS"]
```

