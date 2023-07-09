# Comparing `tmp/neotools-0.3.3.tar.gz` & `tmp/neotools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neotools-0.3.3.tar", last modified: Sun Nov 20 20:18:47 2022, max compression
+gzip compressed data, was "neotools-0.3.4.tar", last modified: Sun Jul  9 04:16:13 2023, max compression
```

## Comparing `neotools-0.3.3.tar` & `neotools-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2022-11-20 20:18:47.081850 neotools-0.3.3/
--rw-rw-r--   0 borys     (1000) borys     (1000)    35149 2020-11-02 07:15:05.000000 neotools-0.3.3/LICENSE
--rw-rw-r--   0 borys     (1000) borys     (1000)     5356 2022-11-20 20:18:47.081850 neotools-0.3.3/PKG-INFO
--rw-rw-r--   0 borys     (1000) borys     (1000)     4601 2022-11-20 20:14:08.000000 neotools-0.3.3/README.md
-drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2022-11-20 20:18:47.081850 neotools-0.3.3/neotools/
--rw-rw-r--   0 borys     (1000) borys     (1000)        0 2020-11-02 07:15:05.000000 neotools-0.3.3/neotools/__init__.py
-drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2022-11-20 20:18:47.081850 neotools-0.3.3/neotools/applet/
--rw-rw-r--   0 borys     (1000) borys     (1000)        0 2021-08-07 17:55:18.000000 neotools-0.3.3/neotools/applet/__init__.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     2596 2021-08-07 18:00:41.000000 neotools-0.3.3/neotools/applet/applet.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     4335 2022-11-20 20:05:58.000000 neotools-0.3.3/neotools/applet/constants.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     7234 2022-11-20 20:11:55.000000 neotools-0.3.3/neotools/applet/manager.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     7924 2021-08-07 17:55:18.000000 neotools-0.3.3/neotools/applet/settings.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     7993 2022-11-20 19:59:55.000000 neotools-0.3.3/neotools/cli.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     7496 2022-11-20 19:56:32.000000 neotools-0.3.3/neotools/commands.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     8503 2021-11-21 22:52:44.000000 neotools-0.3.3/neotools/device.py
--rw-rw-r--   0 borys     (1000) borys     (1000)    11577 2022-11-20 19:44:42.000000 neotools-0.3.3/neotools/file.py
--rw-rw-r--   0 borys     (1000) borys     (1000)      131 2021-08-05 04:43:01.000000 neotools-0.3.3/neotools/main.py
--rw-rw-r--   0 borys     (1000) borys     (1000)    10120 2022-11-20 19:44:42.000000 neotools-0.3.3/neotools/message.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     6708 2020-11-02 07:15:05.000000 neotools-0.3.3/neotools/text_file.py
--rw-rw-r--   0 borys     (1000) borys     (1000)     1883 2021-08-05 03:04:44.000000 neotools-0.3.3/neotools/util.py
-drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2022-11-20 20:18:47.081850 neotools-0.3.3/neotools.egg-info/
--rw-rw-r--   0 borys     (1000) borys     (1000)     5356 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/PKG-INFO
--rw-rw-r--   0 borys     (1000) borys     (1000)      581 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/SOURCES.txt
--rw-rw-r--   0 borys     (1000) borys     (1000)        1 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/dependency_links.txt
--rw-rw-r--   0 borys     (1000) borys     (1000)       46 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/entry_points.txt
--rw-rw-r--   0 borys     (1000) borys     (1000)       45 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/requires.txt
--rw-rw-r--   0 borys     (1000) borys     (1000)        9 2022-11-20 20:18:47.000000 neotools-0.3.3/neotools.egg-info/top_level.txt
--rw-rw-r--   0 borys     (1000) borys     (1000)      100 2021-11-21 22:33:51.000000 neotools-0.3.3/pyproject.toml
--rw-rw-r--   0 borys     (1000) borys     (1000)      939 2022-11-20 20:18:47.085850 neotools-0.3.3/setup.cfg
--rw-rw-r--   0 borys     (1000) borys     (1000)       92 2021-04-13 01:16:05.000000 neotools-0.3.3/setup.py
+drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2023-07-09 04:16:13.452554 neotools-0.3.4/
+-rw-rw-r--   0 borys     (1000) borys     (1000)    35149 2020-11-02 07:15:05.000000 neotools-0.3.4/LICENSE
+-rw-rw-r--   0 borys     (1000) borys     (1000)     5356 2023-07-09 04:16:13.452554 neotools-0.3.4/PKG-INFO
+-rw-rw-r--   0 borys     (1000) borys     (1000)     4601 2022-11-20 20:14:08.000000 neotools-0.3.4/README.md
+drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2023-07-09 04:16:13.452554 neotools-0.3.4/neotools/
+-rw-rw-r--   0 borys     (1000) borys     (1000)        0 2020-11-02 07:15:05.000000 neotools-0.3.4/neotools/__init__.py
+drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2023-07-09 04:16:13.452554 neotools-0.3.4/neotools/applet/
+-rw-rw-r--   0 borys     (1000) borys     (1000)        0 2021-08-07 17:55:18.000000 neotools-0.3.4/neotools/applet/__init__.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     2596 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/applet/applet.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     4335 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/applet/constants.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     7234 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/applet/manager.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     7924 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/applet/settings.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     7993 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/cli.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     7496 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/commands.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)    10405 2023-07-09 04:04:54.000000 neotools-0.3.4/neotools/device.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)    11577 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/file.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)      131 2022-11-20 20:27:20.000000 neotools-0.3.4/neotools/main.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)    10120 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/message.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     6708 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/text_file.py
+-rw-rw-r--   0 borys     (1000) borys     (1000)     1883 2023-07-09 04:07:28.000000 neotools-0.3.4/neotools/util.py
+drwxrwxr-x   0 borys     (1000) borys     (1000)        0 2023-07-09 04:16:13.452554 neotools-0.3.4/neotools.egg-info/
+-rw-rw-r--   0 borys     (1000) borys     (1000)     5356 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/PKG-INFO
+-rw-rw-r--   0 borys     (1000) borys     (1000)      581 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 borys     (1000) borys     (1000)        1 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 borys     (1000) borys     (1000)       46 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/entry_points.txt
+-rw-rw-r--   0 borys     (1000) borys     (1000)       45 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/requires.txt
+-rw-rw-r--   0 borys     (1000) borys     (1000)        9 2023-07-09 04:16:13.000000 neotools-0.3.4/neotools.egg-info/top_level.txt
+-rw-rw-r--   0 borys     (1000) borys     (1000)      100 2021-11-21 22:33:51.000000 neotools-0.3.4/pyproject.toml
+-rw-rw-r--   0 borys     (1000) borys     (1000)      939 2023-07-09 04:16:13.452554 neotools-0.3.4/setup.cfg
+-rw-rw-r--   0 borys     (1000) borys     (1000)       92 2021-04-13 01:16:05.000000 neotools-0.3.4/setup.py
```

### Comparing `neotools-0.3.3/LICENSE` & `neotools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/PKG-INFO` & `neotools-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neotools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Command line tools for AlphaSmart NEO
 Home-page: https://github.com/lykahb/neotools
 Author: Borys Lykah
 License: GNU GPL 3
 Project-URL: Bug Tracker, https://github.com/lykahb/neotools/issues
 Platform: unix
 Platform: linux
```

### Comparing `neotools-0.3.3/README.md` & `neotools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/applet/applet.py` & `neotools-0.3.4/neotools/applet/applet.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/applet/constants.py` & `neotools-0.3.4/neotools/applet/constants.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/applet/manager.py` & `neotools-0.3.4/neotools/applet/manager.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/applet/settings.py` & `neotools-0.3.4/neotools/applet/settings.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/cli.py` & `neotools-0.3.4/neotools/cli.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/commands.py` & `neotools-0.3.4/neotools/commands.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/device.py` & `neotools-0.3.4/neotools/device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import errno
 import logging
 from collections import OrderedDict
 from contextlib import contextmanager
-from time import sleep
+from time import sleep, time
 
 import usb.core
 from usb import util
 
 from neotools.applet.constants import AppletIds
 from neotools.message import Message, MessageConst, send_message
 from neotools.util import NeotoolsError, calculate_data_checksum, data_from_buf
 
 logger = logging.getLogger(__name__)
 
-VENDOR_ID = 0x081e  # USB Vendor ID for the Neo, operating as a keyboard.
-HID_PRODUCT_ID = 0xbd04  # USB Product ID for the Neo, operating as a keyboard.
-COM_PRODUCT_ID = 0xbd01  # USB Product ID for the Neo, operating as a comms device
+VENDOR_ID = 0x081E  # USB Vendor ID for the Neo, operating as a keyboard.
+HID_PRODUCT_ID = 0xBD04  # USB Product ID for the Neo, operating as a keyboard.
+COM_PRODUCT_ID = 0xBD01  # USB Product ID for the Neo, operating as a comms device
 HUB_PRODUCT_ID = 0x0100
 PROTOCOL_VERSION = 0x0220  # Minimum ASM protocol version that the device must support.
 
 
 class Device:
     def __init__(self, dev):
         self.dev = dev
@@ -31,82 +32,131 @@
     @contextmanager
     def connect(flip_to_comms=True, dispose=True):
         device = None
         try:
             device = Device(Device.find())
             device.init(flip_to_comms)
             yield device
+        except usb.core.USBError as e:
+            if e.errno == errno.EACCES:
+                print(
+                    """
+Access denied (insufficient permissions)
+
+Add the following rule to the udev rules, into, for example /lib/udev/rules.d/50-alphasmart.rules.
+Make sure that your user is a member of the plugdev group.
+
+For systems based on Debian:
+
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="081e", ATTRS{idProduct}=="bd01", MODE="660", GROUP="plugdev"
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="081e", ATTRS{idProduct}=="bd04", MODE="660", GROUP="plugdev"
+
+For systems based on Arch:
+
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="081e", ATTRS{idProduct}=="bd01", TAG+="uaccess"
+ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="081e", ATTRS{idProduct}=="bd04", TAG+="uaccess"
+                """
+                )
+            else:
+                logger.exception(e)
         except Exception as e:
             logger.exception(e)
         finally:
             if device and dispose:
                 device.dispose()
 
     @staticmethod
     def find():
-        logger.debug('Searching for device')
+        logger.debug("Searching for device")
         devices = list(usb.core.find(find_all=True, idVendor=VENDOR_ID))
         if len(devices) == 0:
-            raise NeotoolsError('Device not found')
+            raise NeotoolsError("Device not found")
         elif len(devices) > 1:
-            raise NeotoolsError('More than one device is connected')
+            raise NeotoolsError("More than one device is connected")
         return devices[0]
 
     def init(self, flip_to_comms=True):
         self.is_kernel_driver_detached = False
         if flip_to_comms and self.dev.idProduct == HID_PRODUCT_ID:
-            if self.dev.is_kernel_driver_active(0):
-                logger.debug('Detaching kernel driver')
-                self.dev.detach_kernel_driver(0)
-                self.is_kernel_driver_detached = True
-            self.flip_to_comms_mode()
-            util.dispose_resources(self.dev)
-            self.dev = None
-            logger.debug('Connecting to Neo in communication mode')
-            while self.dev is None:
-                sleep(0.1)
-                self.dev = usb.core.find(idVendor=VENDOR_ID, idProduct=COM_PRODUCT_ID)
+            self.require_comms_mode()
 
         if self.dev.idProduct == COM_PRODUCT_ID:
             cfg = self.dev[0]
             intf = cfg[(0, 0)]
             endpoints = intf.endpoints()
 
             def get_endpoint(direction):
                 def predicate(ep):
-                    return \
-                        util.endpoint_type(ep.bmAttributes) == util.ENDPOINT_TYPE_BULK and \
-                        util.endpoint_direction(ep.bEndpointAddress) == direction
+                    return (
+                        util.endpoint_type(ep.bmAttributes) == util.ENDPOINT_TYPE_BULK
+                        and util.endpoint_direction(ep.bEndpointAddress) == direction
+                    )
+
                 eps = list(filter(predicate, endpoints))
                 if len(eps) == 0:
-                    raise NeotoolsError('Cannot find endpoint with direction %s' % direction)
+                    raise NeotoolsError(
+                        "Cannot find endpoint with direction %s" % direction
+                    )
                 return eps[0]
 
             self.in_endpoint = get_endpoint(util.ENDPOINT_IN)
             self.out_endpoint = get_endpoint(util.ENDPOINT_OUT)
 
     def dispose(self):
-        if self.original_product == HID_PRODUCT_ID and self.dev.idProduct == COM_PRODUCT_ID:
+        if (
+            self.original_product == HID_PRODUCT_ID
+            and self.dev.idProduct == COM_PRODUCT_ID
+        ):
             self.flip_to_keyboard_mode()
 
     def flip_to_comms_mode(self):
-        logger.debug('Switching Neo to communication mode')
+        logger.debug("Switching Neo to communication mode")
         # There is black magic here - the sequences used are not documented, but determined from a bus trace.
         self.dev.set_configuration()
-        for i in [0xe0, 0xe1, 0xe2, 0xe3, 0xe4]:
+        for i in [0xE0, 0xE1, 0xE2, 0xE3, 0xE4]:
             self.dev.ctrl_transfer(
-                bmRequestType=util.CTRL_OUT | util.CTRL_TYPE_CLASS | util.CTRL_RECIPIENT_DEVICE,
+                bmRequestType=util.CTRL_OUT
+                | util.CTRL_TYPE_CLASS
+                | util.CTRL_RECIPIENT_DEVICE,
                 bRequest=9,  # SET_CONFIGURATION
                 wValue=(0x02 << 8) | 0,  # report type and ID
                 wIndex=1,  # interface
-                data_or_wLength=[i]  # report value
+                data_or_wLength=[i],  # report value
             )
 
+    def require_comms_mode(self):
+        if self.dev.idProduct == COM_PRODUCT_ID:
+            return
+
+        if self.dev.is_kernel_driver_active(0):
+            logger.debug("Detaching kernel driver")
+            self.dev.detach_kernel_driver(0)
+            self.is_kernel_driver_detached = True
+
+        # Sometimes flipping to communication mode fails on the first attempt but the second one works.
+        timeout = 4  # Neo switches in roughly 2.6s. Four seconds is roughly when it is worth to try flipping to communication again.
+        comms_dev = None
+        for i in range(0, 2):
+            self.flip_to_comms_mode()
+            start_time = time()
+            logger.debug("Connecting to Neo in communication mode")
+            while comms_dev is None and time() - start_time < timeout:
+                sleep(0.1)
+                comms_dev = usb.core.find(idVendor=VENDOR_ID, idProduct=COM_PRODUCT_ID)
+            if comms_dev is not None:
+                break
+
+        if comms_dev is not None:
+            util.dispose_resources(self.dev)
+            self.dev = comms_dev
+        else:
+            raise NeotoolsError("Failed to switch Neo to communication mode")
+
     def flip_to_keyboard_mode(self):
-        logger.debug('Switching Neo to keyboard mode')
+        logger.debug("Switching Neo to keyboard mode")
         self.dialogue_start()
         restart(self)
         try:
             self.dialogue_end()
         except usb.USBError:
             # Neo does not always reply when restarting
             pass
@@ -129,102 +179,116 @@
         if timeout is None:
             timeout = 1000
         length = len(message)
         message_offset = 0
 
         while message_offset != length:
             block_size = min(8, length - message_offset)
-            block = message[message_offset:message_offset + block_size]
+            block = message[message_offset : message_offset + block_size]
             self.out_endpoint.write(block, timeout=timeout)
             message_offset = message_offset + block_size
 
     def dialogue_start(self, applet_id=AppletIds.SYSTEM):
         self.hello()
         self.reset()
         self.switch_applet(applet_id)
 
     def dialogue_end(self):
         self.reset()
 
     def reset(self):
-        """ Reset the device to a known state. Succeeds if device is supported and working correctly. """
-        command_request_reset = b'?\xff\x00reset'
+        """Reset the device to a known state. Succeeds if device is supported and working correctly."""
+        command_request_reset = b"?\xff\x00reset"
         self.write(command_request_reset)
 
     def switch_applet(self, applet_id):
-        applet_id_bytes = applet_id.to_bytes(length=2, byteorder='big')
-        command_request_switch = [0x3f, 0x53, 0x77, 0x74, 0x63, 0x68, applet_id_bytes[0],
-                                  applet_id_bytes[1]]  # '?SwtchXX'
-        command_response_switched = b'Switched'
+        applet_id_bytes = applet_id.to_bytes(length=2, byteorder="big")
+        command_request_switch = [
+            0x3F,
+            0x53,
+            0x77,
+            0x74,
+            0x63,
+            0x68,
+            applet_id_bytes[0],
+            applet_id_bytes[1],
+        ]  # '?SwtchXX'
+        command_response_switched = b"Switched"
 
         self.write(command_request_switch)
         response = self.read(8)
         if response != command_response_switched:
-            raise NeotoolsError('Failed to switch to applet %s' % applet_id)
+            raise NeotoolsError("Failed to switch to applet %s" % applet_id)
 
     def hello(self):
         """Ping the device for the ASM protocol version number. This will put the Neo in
-         to ASM mode and also return the protocol version. It is also used as a keep-alive
-         test.
-         """
+        to ASM mode and also return the protocol version. It is also used as a keep-alive
+        test.
+        """
         retries = 10
         buf = []
         while retries > 0:
             self.write([0x01], timeout=100)  # ascCommandRequestProtocol
             buf = self.read(8, timeout=100)
             if len(buf) == 2:
                 break  # success
-            logger.debug('Unexpected byte response %s', buf)
+            logger.debug("Unexpected byte response %s", buf)
             retries = retries - 1
             self.reset()
             sleep(0.1)  # seconds
         if retries < 0:
-            raise NeotoolsError("This device doesn't look like it wants to talk to us - bailing out.")
+            raise NeotoolsError(
+                "This device doesn't look like it wants to talk to us - bailing out."
+            )
 
-        version = int.from_bytes(buf[0:2], byteorder='big')
+        version = int.from_bytes(buf[0:2], byteorder="big")
         if version < PROTOCOL_VERSION:
-            raise NeotoolsError('ASM protocol version not supported: %s' % version)
+            raise NeotoolsError("ASM protocol version not supported: %s" % version)
 
 
 def get_available_space(device):
     device.dialogue_start()
     message = Message(MessageConst.REQUEST_GET_AVAIL_SPACE, [])
     response = send_message(device, message, MessageConst.RESPONSE_GET_AVAIL_SPACE)
     result = {
-        'free_rom': response.argument(1, 4),
-        'free_ram': response.argument(5, 2) * 256
+        "free_rom": response.argument(1, 4),
+        "free_ram": response.argument(5, 2) * 256,
     }
     device.dialogue_end()
     return result
 
 
 def restart(device):
     message = Message(MessageConst.REQUEST_RESTART, [])
     send_message(device, message, MessageConst.RESPONSE_RESTART)
 
 
 REVISION_FORMAT = {
-    'size': None,
-    'fields': OrderedDict([
-        ('unknown', (0x00, 3, int)),
-        ('revision_major', (0x04, 1, int)),
-        ('revision_minor', (0x05, 1, int)),
-        ('name', (0x06, 19, str)),
-        ('build_date', (0x19, 39, str))
-    ])
+    "size": None,
+    "fields": OrderedDict(
+        [
+            ("unknown", (0x00, 3, int)),
+            ("revision_major", (0x04, 1, int)),
+            ("revision_minor", (0x05, 1, int)),
+            ("name", (0x06, 19, str)),
+            ("build_date", (0x19, 39, str)),
+        ]
+    ),
 }
 
 
 def get_version(device):
     device.dialogue_start()
     message = Message(MessageConst.REQUEST_VERSION, [])
     response = send_message(device, message, MessageConst.RESPONSE_VERSION)
     size = response.argument(1, 4)
     expected_checksum = response.argument(5, 2)
 
     buf = device.read(size)
     checksum = calculate_data_checksum(buf)
     if calculate_data_checksum(buf) == expected_checksum:
         # OS 3.6 Neo device appear to calculate the checksum wrongly (off by one error?)
-        logger.debug(f'Ignoring data checksum error. Wanted {expected_checksum}, got {checksum}')
+        logger.debug(
+            f"Ignoring data checksum error. Wanted {expected_checksum}, got {checksum}"
+        )
     device.dialogue_end()
     return data_from_buf(REVISION_FORMAT, buf)
```

### Comparing `neotools-0.3.3/neotools/file.py` & `neotools-0.3.4/neotools/file.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/message.py` & `neotools-0.3.4/neotools/message.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/text_file.py` & `neotools-0.3.4/neotools/text_file.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools/util.py` & `neotools-0.3.4/neotools/util.py`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/neotools.egg-info/PKG-INFO` & `neotools-0.3.4/neotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neotools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Command line tools for AlphaSmart NEO
 Home-page: https://github.com/lykahb/neotools
 Author: Borys Lykah
 License: GNU GPL 3
 Project-URL: Bug Tracker, https://github.com/lykahb/neotools/issues
 Platform: unix
 Platform: linux
```

### Comparing `neotools-0.3.3/neotools.egg-info/SOURCES.txt` & `neotools-0.3.4/neotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neotools-0.3.3/setup.cfg` & `neotools-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neotools
-version = 0.3.3
+version = 0.3.4
 license = GNU GPL 3
 license_file = LICENSE
 author = Borys Lykah
 description = Command line tools for AlphaSmart NEO
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lykahb/neotools
```

