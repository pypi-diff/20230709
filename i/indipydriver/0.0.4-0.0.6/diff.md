# Comparing `tmp/indipydriver-0.0.4.tar.gz` & `tmp/indipydriver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-0.0.4.tar", last modified: Thu Jun 29 13:38:39 2023, max compression
+gzip compressed data, was "indipydriver-0.0.6.tar", last modified: Sun Jul  9 10:55:57 2023, max compression
```

## Comparing `indipydriver-0.0.4.tar` & `indipydriver-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.4/LICENSE
--rw-r--r--   0        0        0     2261 2023-06-17 14:59:33.000000 indipydriver-0.0.4/README.md
--rw-r--r--   0        0        0      541 2023-06-29 09:54:28.000000 indipydriver-0.0.4/indipydriver/__init__.py
--rw-r--r--   0        0        0    12223 2023-06-25 17:20:07.000000 indipydriver-0.0.4/indipydriver/comms.py
--rw-r--r--   0        0        0    20935 2023-06-12 18:46:59.000000 indipydriver-0.0.4/indipydriver/events.py
--rw-r--r--   0        0        0    20634 2023-06-29 09:38:24.000000 indipydriver-0.0.4/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    11134 2023-06-23 22:47:31.000000 indipydriver-0.0.4/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    42856 2023-06-29 09:25:28.000000 indipydriver-0.0.4/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-06-29 09:53:53.000000 indipydriver-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 indipydriver-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2261 2023-06-17 14:59:33.000000 indipydriver-0.0.6/README.md
+-rw-r--r--   0        0        0      573 2023-07-08 14:17:28.000000 indipydriver-0.0.6/indipydriver/__init__.py
+-rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-0.0.6/indipydriver/comms.py
+-rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-0.0.6/indipydriver/events.py
+-rw-r--r--   0        0        0    20883 2023-07-09 10:29:51.000000 indipydriver-0.0.6/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0     8206 2023-07-09 10:17:52.000000 indipydriver-0.0.6/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-0.0.6/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-0.0.6/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-07-08 14:16:54.000000 indipydriver-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 indipydriver-0.0.6/PKG-INFO
```

### Comparing `indipydriver-0.0.4/LICENSE` & `indipydriver-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.4/README.md` & `indipydriver-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.4/indipydriver/__init__.py` & `indipydriver-0.0.6/indipydriver/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
+from .ipyserver import IPyServer
 
-
-version = "0.0.4"
+version = "0.0.6"
```

### Comparing `indipydriver-0.0.4/indipydriver/comms.py` & `indipydriver-0.0.6/indipydriver/comms.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,39 +50,33 @@
     attriblist.append(">")
     return "".join(attriblist)
 
 
 def blob_xml_bytes(xmldata):
     """A generator yielding blob xml byte strings
        for a setBLOBVector.
-       reads member files, b64 encodes the data
-       closes the files, and yields the binary
-       string including tags."""
+       reads member bytes, b64 encodes the data
+       and yields the byte string including tags."""
 
     # yield initial setBLOBVector
     setblobvector = _makestart(xmldata)
     yield setblobvector.encode()
-
     for oneblob in xmldata.iter('oneBLOB'):
-        # get the filepointer
-        fp = oneblob.text
-        # set seek(0) so is read from start of file
-        fp.seek(0)
-        bytescontent = fp.read()
-        fp.close()
-        if bytescontent == b"":
-            continue
+        bytescontent = oneblob.text
         size = oneblob.get("size")
         if size == "0":
             oneblob.set("size", str(len(bytescontent)))
         # yield start of oneblob
         start = _makestart(oneblob)
         yield start.encode()
-        # yield body, b64 encoded
-        yield standard_b64encode(bytescontent)
+        # yield body, b64 encoded, in chunks
+        encoded_data = standard_b64encode(bytescontent)
+        chunksize = 1000
+        for b in range(0, len(encoded_data), chunksize):
+            yield encoded_data[b:b+chunksize]
         yield b"</oneBLOB>"
     yield b"</setBLOBVector>\n"
 
 
 class STDOUT_TX:
     "An object that transmits data on stdout, used by STDINOUT as one half of the communications path"
 
@@ -117,17 +111,17 @@
         source = self.datasource()
         while True:
             await asyncio.sleep(0)
             if readerque is None:
                 continue
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
-            root = await anext(source)
-            if root is not None:
-                await readerque.put(root)
+            rxdata = await anext(source)
+            if rxdata is not None:
+                await readerque.put(rxdata)
 
     async def datasource(self):
         # get received data, parse it, and yield it as xml.etree.ElementTree object
         data_in = self.datainput()
         message = b''
         messagetagnumber = None
         while True:
@@ -201,25 +195,22 @@
             while b">" in data:
                 await asyncio.sleep(0)
                 binarydata, data = data.split(b'>', maxsplit=1)
                 binarydata += b">"
                 yield binarydata
 
 
-# useful test strings
-# <getProperties version="1.7" />
-# <newNumberVector device="Thermostat" name="targetvector"><oneNumber name="target">40</oneNumber></newNumberVector>
-# sys.stderr.write((binarydata+b'\n').decode("ascii"))   - note, the + b'\n' is necessary to send this text.
-# telnet localhost 7624
-
-
 class STDINOUT():
     """If indipydriver.comms is set to an instance of this class it is
        used to implement communications via stdin and stdout"""
 
+    def __init__(self):
+        self.connected = True
+
+
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         # Set stdin to non-blocking mode
         flags = fcntl.fcntl(sys.stdin.fileno(), fcntl.F_GETFL)
         fcntl.fcntl(sys.stdin.fileno(), fcntl.F_SETFL, flags | os.O_NONBLOCK)
 
         rx = STDIN_RX()
@@ -228,23 +219,30 @@
         await asyncio.gather(rx.run_rx(readerque),
                              tx.run_tx(writerque)
                              )
 
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
-    def __init__(self, writer):
+    def __init__(self, blobstatus, writer):
+        self.blobstatus = blobstatus
         self.writer = writer
 
+
     async def run_tx(self, writerque):
-        """Gets data from writerque, and transmits it out on stdout"""
+        """Gets data from writerque, and transmits it out on the port writer"""
         while True:
             await asyncio.sleep(0)
-            # get block of data from writerque and transmit down stdout
+            # get block of data from writerque and transmit
             txdata = await writerque.get()
+            if not self.blobstatus.allowed(txdata):
+                # this data should not be transmitted, discard it
+                writerque.task_done()
+                continue
+            # this data can be transmitted
             if txdata.tag == "setBLOBVector" and len(txdata):
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # Send to the port
                     self.writer.write(binarydata)
                     await self.writer.drain()
@@ -257,19 +255,38 @@
             writerque.task_done()
 
 
 
 class Port_RX(STDIN_RX):
     """Produces xml.etree.ElementTree data from data received on the port,
        this is used by Portcomms as one half of the communications path.
-       This overwrites the datainput method of the STDIN_RX parent class."""
+       This overwrites methods of the STDIN_RX parent class."""
 
-    def __init__(self, reader):
+    def __init__(self, blobstatus, reader):
+        self.blobstatus = blobstatus
         self.reader = reader
 
+    async def run_rx(self, readerque):
+        "pass data to readerque"
+        source = self.datasource()
+        while True:
+            await asyncio.sleep(0)
+            if readerque is None:
+                continue
+            # get block of xml.etree.ElementTree data
+            # from source and append it to  readerque
+            rxdata = await anext(source)
+            if rxdata is not None:
+                if rxdata.tag == "enableBLOB":
+                    # set permission flags in the blobstatus object
+                    self.blobstatus.setpermissions(rxdata)
+                # and place rxdata into readerque
+                await readerque.put(rxdata)
+
+
     async def datainput(self):
         "Generator producing binary string of data from the port"
         binarydata = b""
         while True:
             await asyncio.sleep(0)
             try:
                 data = await self.reader.readuntil(separator=b'>')
@@ -290,15 +307,17 @@
                 # could put a max value here to stop this increasing indefinetly
 
 
 class Portcomms():
     """If indipydriver.comms is set to an instance of this class it is
        used to implement communications via a port"""
 
-    def __init__(self, host="localhost", port=7624):
+    def __init__(self, devices, host="localhost", port=7624):
+        # devices is a dictionary of device name to device this driver owns
+        self.blobstatus = BLOBSstatus(devices)
         self.host = host
         self.port = port
         self.connected = False
 
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         self.readerque = readerque
@@ -314,18 +333,117 @@
         "Used by asyncio.start_server, called to handle a client connection"
         if self.connected:
             # already connected, can only handle one connection
             writer.close()
             await writer.wait_closed()
             return
         self.connected = True
-        rx = Port_RX(reader)
-        tx = Port_TX(writer)
+        rx = Port_RX(self.blobstatus, reader)
+        tx = Port_TX(self.blobstatus, writer)
         try:
             txtask = asyncio.create_task(tx.run_tx(self.writerque))
             rxtask = asyncio.create_task(rx.run_rx(self.readerque))
             await txtask
             await rxtask
         except ConnectionResetError:
             self.connected = False
             txtask.cancel()
             rxtask.cancel()
+            cleanque(self.writerque)
+
+
+def cleanque(que):
+    "Clears out a que"
+    try:
+        while True:
+            xmldata = que.get_nowait()
+            que.task_done()
+    except asyncio.QueueEmpty:
+        # que is now empty, nothing further to do
+        pass
+
+
+class BLOBSstatus:
+    "Carries the enableBLOB status on a device or property"
+
+    def __init__(self, devices):
+        "For every device, propertyvector create a status list of (Other allowed, BLOB allowed)"
+        self.devicestatus = {}
+        # create a dictionary of devicenames : list of propertynames for that device
+        self.deviceproperties = {}
+        for devicename, device in devices.items():
+            self.deviceproperties[devicename] = []
+            for propertyvector in device.values():
+                # Initially set with BLOBs not allowed
+                self.devicestatus[(devicename, propertyvector.name)] = (True, False)
+                self.deviceproperties[devicename].append(propertyvector.name)
+
+
+    def allowed(self, xmldata):
+        "Return True if this xmldata can be transmitted, False otherwise"
+        devicename = xmldata.get("device")
+        if devicename is None:
+            # either a getproperties or message, only deny it if ALL Other allowed are False
+            # so this connection is dedictated to BLOBs only
+            for status in self.devicestatus.values():
+                if status[0]:
+                    return True
+            return False
+        if not (devicename in self.deviceproperties):
+            # devicename not recognised
+            return False
+        # so we have a devicename, get propertyname
+        name = xmldata.get("name")
+        # if name missing, could be a message, cannot be a setBLOBVector
+        if name is None:
+            # only deny it if ALL other allowed are False for this device
+            properties = self.deviceproperties[devicename]
+            for name in properties:
+                status = self.devicestatus[devicename, name]
+                if status[0]:
+                    return True
+            return False
+        # so we have a devicename, propertyname
+        status = self.devicestatus.get((devicename, name))
+        if status is None:
+            # this property is not recognised as belonging to the device
+            return False
+        if xmldata.tag == "setBLOBVector":
+            return status[1]
+        else:
+            return status[0]
+
+
+    def setpermissions(self, rxdata):
+        "Read the received enableBLOB xml and set permission in self.devicestatus"
+
+        # Command to control whether setBLOBs should be sent to this channel from a given Device. They can
+        # be turned off completely by setting Never (the default), allowed to be intermixed with other INDI
+        # commands by setting Also or made the only command by setting Only.
+
+        devicename = rxdata.get("device")
+        if devicename is None:
+            # invalid
+            return
+        if not (devicename in self.deviceproperties):
+            # devicename not recognised
+            return
+        value = rxdata.text.strip()
+        if value == "Never":
+            perm = (True, False)    # (Other allowed, BLOB not allowed)
+        elif value == "Also":
+            perm = (True, True)     # (Other allowed, BLOB allowed)
+        elif value == "Only":
+            perm = (False, True)   # (Only not allowed, BLOB allowed)
+        else:
+            # value not recognised
+            return
+        propertyname = rxdata.get("name")
+        if propertyname is None:
+            # This applies to all properties of the device
+            properties = self.deviceproperties[devicename]
+            for name in properties:
+                self.devicestatus[devicename, name] = perm
+        elif (devicename, propertyname) in self.devicestatus:
+            self.devicestatus[devicename, propertyname] = perm
+        # otherwise the (devicename, propertyname) are not recognised
+        # so return without setting any permissions
```

### Comparing `indipydriver-0.0.4/indipydriver/events.py` & `indipydriver-0.0.6/indipydriver/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     "defines an event that a getProperties has been received"
     def __init__(self, devicename, vectorname, vector, root):
         super().__init__(devicename, vectorname, vector, root)
 
 
 
 class enableBLOB(Event):
-    "defines an event with self.value one of Never, Also, Only"
+    """Defines an event with self.value being one of Never, Also,
+       or Only. This can be ignored by the driver. It is automatically
+       acted on, if the driver listen() method is used."""
 
     def __init__(self, devicename, vectorname, vector, root):
         super().__init__(devicename, vectorname, vector, root)
         value = root.text.strip()
         if value in ("Never", "Also", "Only"):
             self.value = value
         else:
```

### Comparing `indipydriver-0.0.4/indipydriver/ipydriver.py` & `indipydriver-0.0.6/indipydriver/ipydriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,25 @@
 
     def _reporterror(self, message):
         "Prints message to stderr"
         print(message, file=sys.stderr)
 
     def listen(self, host="localhost", port=7624):
         """If called, listens on the given host and port. Only one connection is accepted,
-           further connection attempts while a client is already connected will be refused."""
+           further connection attempts while a client is already connected will be refused.
+           This method also checks for enableBLOB instructions, and implements them."""
         if not self.comms is None:
              raise RuntimeError("A communications method has already been set, there can only be one")
-        self.comms = Portcomms(host, port)
+        self.comms = Portcomms(self.devices, host, port)
+
+
+    async def send(self, xmldata):
+        "Transmits xmldata, this is an internal method, not normally called by a user."
+        if self.comms.connected:
+            await self.writerque.put(xmldata)
 
     def __setitem__(self, devicename):
         raise KeyError
 
     async def _read_readerque(self):
         client_tags = ("enableBLOB", "newSwitchVector", "newNumberVector", "newTextVector", "newBLOBVector")
         snoop_tags = ("message", 'delProperty', 'defSwitchVector', 'setSwitchVector', 'defLightVector',
@@ -234,33 +241,33 @@
             self._reporterror("The timestamp given in send_message must be a datetime.datetime object")
             return
         xmldata = ET.Element('message')
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
-        await self.writerque.put(xmldata)
+        await self.send(xmldata)
 
     async def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request - which is used to snoop data from other devices
            on the network, if devicename given, it must not be a device of this driver as
            the point of this is to snoop on remote devices."""
         xmldata = ET.Element('getProperties')
         if devicename is None:
-            await self.writerque.put(xmldata)
+            await self.send(xmldata)
             return
         if devicename in self.devices:
             self._reporterror("Cannot snoop on a device already controlled by this driver")
             return
         xmldata.set("device", devicename)
         if vectorname is None:
-            await self.writerque.put(xmldata)
+            await self.send(xmldata)
             return
         xmldata.set("name", vectorname)
-        await self.writerque.put(xmldata)
+        await self.send(xmldata)
 
     async def hardware(self):
         """Override this to operate device hardware, and transmit updates
 
         For example: call your own code to operate hardware
         then update the appropriate vectors, and send updated
         values to the client using
@@ -367,15 +374,15 @@
             return
         xmldata = ET.Element('message')
         xmldata.set("device", self.devicename)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
     async def send_delProperty(self, message="", timestamp=None):
         """Sending delProperty with this device method, (as opposed to the vector send_delProperty method)
            informs the client this device is not available, it also sets a device.enable attribute to
            False, which stops any data being transmitted between the client and this device.
            Setting device.enable to True re-enables communications.
            The message argument is any appropriate string which the client could display to the user.
@@ -388,15 +395,15 @@
             return
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
         self.enable = False
 
 
     async def devhardware(self, *args, **kwargs):
         """As default, does nothing and is not called.
 
            If required, override this to handle any necessary device actions.
```

### Comparing `indipydriver-0.0.4/indipydriver/propertymembers.py` & `indipydriver-0.0.6/indipydriver/propertymembers.py`

 * *Files 5% similar despite different names*

```diff
@@ -306,22 +306,34 @@
 
     def oneblob(self):
         """Returns xml of a oneBLOB"""
         xmldata = ET.Element('oneBLOB')
         xmldata.set("name", self.name)
         xmldata.set("size", str(self.blobsize))
         xmldata.set("format", self.blobformat)
-        # the value set in the xmldata object should be a file-like object
+        # the value set in the xmldata object should be a bytes object
         if isinstance(self._membervalue, bytes):
-            xmldata.text = io.BytesIO(self._membervalue)
+            xmldata.text = self._membervalue
         elif hasattr(self._membervalue, "read") and callable(self._membervalue.read):
             # a file-like object
-            xmldata.text = self._membervalue
+            # set seek(0) so is read from start of file
+            self._membervalue.seek(0)
+            bytescontent = self._membervalue.read()
+            self._membervalue.close()
+            if not isinstance(bytescontent, bytes):
+                raise ValueError(f"On being read, the BLOBMember {self.name} does not give bytes")
+            if bytescontent == b"":
+                raise ValueError(f"The BLOBMember {self.name} value is empty")
+            xmldata.text = bytescontent
         else:
             # could be a path to a file
             try:
-                xmldata.text = open(self._membervalue, "rb")
+                with open(self._membervalue, "rb") as fp:
+                    bytescontent = fp.read()
             except:
                 raise ValueError(f"The BLOBMember {self.name} value cannot be openned")
-         # old value was
+            if bytescontent == b"":
+                raise ValueError(f"The BLOBMember {self.name} value is empty")
+            xmldata.text = bytescontent
+        # old value was
         # xmldata.text = standard_b64encode(self._membervalue).decode('ascii')
         return xmldata
```

### Comparing `indipydriver-0.0.4/indipydriver/propertyvectors.py` & `indipydriver-0.0.6/indipydriver/propertyvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
         self.enable = False
         for member in self.data.values():
             # set all members as changed, so when re-enabled, all values are ready to be sent again
             member.changed = True
 
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
@@ -199,15 +199,15 @@
         if message:
             xmldata.set("message", message)
         for switch in self.data.values():
             xmldata.append(switch.defswitch())
             # after a defswitch sent, assume new client connection, and set all members as changed
             # so they will all be included in the first 'send_setVector'
             switch.changed = True
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setSwitchVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -262,15 +262,15 @@
             # only send member if its value has changed or if allvalues is True
             if allvalues or switch.changed:
                 xmldata.append(switch.oneswitch())
                 switch.changed = False
                 membersincluded = True
         if membersincluded:
             # only send xmldata if a member is included in the vector
-            await self.driver.writerque.put(xmldata)
+            await self.driver.send(xmldata)
 
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setSwitchVector) and members with their values to the client.
            Similar to the send_setVector method however the members list specifies the
            member names which will have their values sent.
 
@@ -305,15 +305,15 @@
         Onswitches = (switch for switch in self.data.values() if switch.membervalue == 'On' and switch.name in members)
         for switch in Offswitches:
             xmldata.append(switch.oneswitch())
             switch.changed = False
         for switch in Onswitches:
             xmldata.append(switch.oneswitch())
             switch.changed = False
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
 
 class LightVector(PropertyVector):
 
     """A LightVector is an instrument indicator, and sends one or more members
        with values 'Idle', 'Ok', 'Busy' or 'Alert'. In general a client will
        indicate this state with different colours."""
@@ -377,15 +377,15 @@
         if message:
             xmldata.set("message", message)
         for light in self.data.values():
             xmldata.append(light.deflight())
             # after a deflight sent, assume new client connection, and set all members as changed
             # so they will all be included in the first 'send_setVector'
             light.changed = True
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setLightVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
@@ -427,15 +427,15 @@
             # only send member if its value has changed or if allvalues is True
             if allvalues or light.changed:
                 xmldata.append(light.onelight())
                 light.changed = False
                 membersincluded = True
         if membersincluded:
             # only send xmldata if a member is included in the vector
-            await self.driver.writerque.put(xmldata)
+            await self.driver.send(xmldata)
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setLightVector) and members with their values to the client.
            Similar to the send_setVector method however the members list specifies the
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
@@ -460,15 +460,15 @@
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
         for light in self.data.values():
             if light.name in  members:
                 xmldata.append(light.onelight())
                 light.changed = False
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
 
 
 class TextVector(PropertyVector):
 
     """A TextVector is used to send and receive text between instrument and client."""
 
@@ -547,15 +547,15 @@
         if message:
             xmldata.set("message", message)
         for text in self.data.values():
             xmldata.append(text.deftext())
             # after a deftext sent, assume new client connection, and set all members as changed
             # so they will all be included in the first 'send_setVector'
             text.changed = True
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setTextVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -600,15 +600,15 @@
             # only send member if its value has changed or if allvalues is True
             if allvalues or text.changed:
                 xmldata.append(text.onetext())
                 text.changed = False
                 membersincluded = True
         if membersincluded:
             # only send xmldata if a member is included in the vector
-            await self.driver.writerque.put(xmldata)
+            await self.driver.send(xmldata)
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setTextVector) and members with their values to the client.
            Similar to the send_setVector method however the members list specifies the
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
@@ -636,15 +636,15 @@
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for text in self.data.values():
             if text.name in members:
                 xmldata.append(text.onetext())
                 text.changed = False
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
 
 class NumberVector(PropertyVector):
 
     def __init__(self, name, label, group, perm, state, numbermembers):
         super().__init__(name, label, group, state)
         self.perm = perm
@@ -720,15 +720,15 @@
         if message:
             xmldata.set("message", message)
         for number in self.data.values():
             xmldata.append(number.defnumber())
             # after a defnumber sent, assume new client connection, and set all members as changed
             # so they will all be included in the first 'send_setVector'
             number.changed = True
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setNumberVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -773,15 +773,15 @@
             # only send member if its value has changed or if allvalues is True
             if allvalues or number.changed:
                 xmldata.append(number.onenumber())
                 number.changed = False
                 membersincluded = True
         if membersincluded:
             # only send xmldata if a member is included in the vector
-            await self.driver.writerque.put(xmldata)
+            await self.driver.send(xmldata)
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setNumberVector) and members with their values to the client.
            Similar to the send_setVector method however the members list specifies the
            member names which will have their values sent.
 
            This allows members to be explicitly specified. If the members list is empty
@@ -809,15 +809,15 @@
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for number in self.data.values():
             if number.name in members:
                 xmldata.append(number.onenumber())
                 number.changed = False
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
 
 class BLOBVector(PropertyVector):
 
     def __init__(self, name, label, group, perm, state, blobmembers):
         super().__init__(name, label, group, state)
         self.perm = perm
@@ -909,26 +909,26 @@
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
             xmldata.append(blob.defblob())
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
 
     # NOTE: BLOBVectors do not have a send_setVector method
     #       only the more explicit send_setVectorMembers is available
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setBLOBVector) and members with their values to the client.
            The members list specifies the member names which will have their values sent.
 
            Members contain either a bytes string, a file-like object, or a path to a file. If
-           a file-like object is given, it's close() method will automatically be called after
-           the BLOB is sent, so you do not have to close it.
+           a file-like object is given, its contents will be read and its close() method
+           will be called, so you do not have to close it.
         """
         if not isinstance(timeout, str):
             self._reporterror("Aborting sending setBLOBVector: The given send_setVectorMembers timeout value must be a string object")
             return
         if not self.device.enable:
             return
         if not self.enable:
@@ -949,8 +949,8 @@
             xmldata.set("message", message)
         for blob in self.data.values():
             if (blob.name in members) and (blob.membervalue is not None):
                 try:
                     xmldata.append(blob.oneblob())
                 except ValueError as ex:
                     self._reporterror(ex)
-        await self.driver.writerque.put(xmldata)
+        await self.driver.send(xmldata)
```

### Comparing `indipydriver-0.0.4/pyproject.toml` & `indipydriver-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.4"
+version = "0.0.6"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-0.0.4/PKG-INFO` & `indipydriver-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 0.0.4
+Version: 0.0.6
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

