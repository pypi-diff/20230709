# Comparing `tmp/dmglib-0.9.3.tar.gz` & `tmp/dmglib-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmglib-0.9.3.tar", last modified: Mon Oct 18 18:41:56 2021, max compression
+gzip compressed data, was "dmglib-0.9.4.tar", last modified: Sun Jul  9 20:58:29 2023, max compression
```

## Comparing `dmglib-0.9.3.tar` & `dmglib-0.9.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2021-10-18 18:41:56.650913 dmglib-0.9.3/
--rw-r--r--   0 jakob      (501) staff       (20)     1050 2019-01-26 16:19:48.000000 dmglib-0.9.3/LICENSE
--rw-r--r--   0 jakob      (501) staff       (20)     1020 2021-10-18 18:41:56.650408 dmglib-0.9.3/PKG-INFO
--rw-r--r--   0 jakob      (501) staff       (20)      465 2019-01-26 16:19:48.000000 dmglib-0.9.3/README.md
--rw-r--r--   0 jakob      (501) staff       (20)       38 2021-10-18 18:41:56.651066 dmglib-0.9.3/setup.cfg
--rw-r--r--   0 jakob      (501) staff       (20)      783 2021-10-18 18:37:53.000000 dmglib-0.9.3/setup.py
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2021-10-18 18:41:56.647993 dmglib-0.9.3/src/
-drwxr-xr-x   0 jakob      (501) staff       (20)        0 2021-10-18 18:41:56.649649 dmglib-0.9.3/src/dmglib.egg-info/
--rw-r--r--   0 jakob      (501) staff       (20)     1020 2021-10-18 18:41:56.000000 dmglib-0.9.3/src/dmglib.egg-info/PKG-INFO
--rw-r--r--   0 jakob      (501) staff       (20)      176 2021-10-18 18:41:56.000000 dmglib-0.9.3/src/dmglib.egg-info/SOURCES.txt
--rw-r--r--   0 jakob      (501) staff       (20)        1 2021-10-18 18:41:56.000000 dmglib-0.9.3/src/dmglib.egg-info/dependency_links.txt
--rw-r--r--   0 jakob      (501) staff       (20)        7 2021-10-18 18:41:56.000000 dmglib-0.9.3/src/dmglib.egg-info/top_level.txt
--rw-r--r--   0 jakob      (501) staff       (20)    15280 2021-10-18 18:35:24.000000 dmglib-0.9.3/src/dmglib.py
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2023-07-09 20:58:29.180822 dmglib-0.9.4/
+-rw-r--r--   0 jakob      (501) staff       (20)     1050 2023-07-09 15:52:07.000000 dmglib-0.9.4/LICENSE
+-rw-r--r--   0 jakob      (501) staff       (20)     1001 2023-07-09 20:58:29.180308 dmglib-0.9.4/PKG-INFO
+-rw-r--r--   0 jakob      (501) staff       (20)      465 2023-07-09 15:52:07.000000 dmglib-0.9.4/README.md
+-rw-r--r--   0 jakob      (501) staff       (20)       38 2023-07-09 20:58:29.181006 dmglib-0.9.4/setup.cfg
+-rw-r--r--   0 jakob      (501) staff       (20)      784 2023-07-09 16:25:19.000000 dmglib-0.9.4/setup.py
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2023-07-09 20:58:29.174717 dmglib-0.9.4/src/
+drwxr-xr-x   0 jakob      (501) staff       (20)        0 2023-07-09 20:58:29.179843 dmglib-0.9.4/src/dmglib.egg-info/
+-rw-r--r--   0 jakob      (501) staff       (20)     1001 2023-07-09 20:58:29.000000 dmglib-0.9.4/src/dmglib.egg-info/PKG-INFO
+-rw-r--r--   0 jakob      (501) staff       (20)      176 2023-07-09 20:58:29.000000 dmglib-0.9.4/src/dmglib.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob      (501) staff       (20)        1 2023-07-09 20:58:29.000000 dmglib-0.9.4/src/dmglib.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob      (501) staff       (20)        7 2023-07-09 20:58:29.000000 dmglib-0.9.4/src/dmglib.egg-info/top_level.txt
+-rw-r--r--   0 jakob      (501) staff       (20)    14574 2023-07-09 16:24:41.000000 dmglib-0.9.4/src/dmglib.py
```

### Comparing `dmglib-0.9.3/LICENSE` & `dmglib-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmglib-0.9.3/PKG-INFO` & `dmglib-0.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dmglib
-Version: 0.9.3
+Version: 0.9.4
 Summary: Work with macOS DMG disk images
 Home-page: https://github.com/0xbf00/dmglib
 Author: Jakob Rieck
 Author-email: jakobrieck+pypi@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Provides: dmglib
 Description-Content-Type: text/markdown
@@ -21,8 +20,7 @@
 `dmglib` is a tiny python wrapper built around the `hdiutil` command line tool on macOS. It is intended to be used to work with the contents of DMG files on macOS.
 
 `dmglib` provides functions for the following tasks:
 * Querying the list of currently attached disk images on the system
 * Checking whether a target disk image is password-protected
 * Checking whether a given password is correct for a target disk image
 * Attaching and detaching disk images
-
```

### Comparing `dmglib-0.9.3/setup.py` & `dmglib-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_desc = fh.read()
 
 setuptools.setup(
       name='dmglib',
-      version='0.9.3',
+      version='0.9.4',
       description='Work with macOS DMG disk images',
       long_description=long_desc,
       long_description_content_type="text/markdown",
       author='Jakob Rieck',
       author_email='jakobrieck+pypi@gmail.com',
       url='https://github.com/0xbf00/dmglib',
       license='MIT License',
@@ -20,8 +20,8 @@
 		'Programming Language :: Python :: 3.6',
 		'Operating System :: MacOS',
 		'Development Status :: 5 - Production/Stable',
 		'Intended Audience :: Developers',
 		'License :: OSI Approved :: MIT License'
 	  ],
       provides=['dmglib']
-)
+)
```

### Comparing `dmglib-0.9.3/src/dmglib.egg-info/PKG-INFO` & `dmglib-0.9.4/src/dmglib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dmglib
-Version: 0.9.3
+Version: 0.9.4
 Summary: Work with macOS DMG disk images
 Home-page: https://github.com/0xbf00/dmglib
 Author: Jakob Rieck
 Author-email: jakobrieck+pypi@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Provides: dmglib
 Description-Content-Type: text/markdown
@@ -21,8 +20,7 @@
 `dmglib` is a tiny python wrapper built around the `hdiutil` command line tool on macOS. It is intended to be used to work with the contents of DMG files on macOS.
 
 `dmglib` provides functions for the following tasks:
 * Querying the list of currently attached disk images on the system
 * Checking whether a target disk image is password-protected
 * Checking whether a given password is correct for a target disk image
 * Attaching and detaching disk images
-
```

### Comparing `dmglib-0.9.3/src/dmglib.py` & `dmglib-0.9.4/src/dmglib.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,33 +145,39 @@
         disk_format,
         '-o',
         output_path,
         input_path
     ])
 
 
-def _hdiutil_attach(path, keyphrase=None) -> (bool, dict):
+def _hdiutil_attach(path, keyphrase=None, mountpoint=None) -> (bool, dict):
     """Attaches a disk image.
 
     The image is mounted using the `-nobrowse` flag so that it is not visible in
     Finder.app.
 
     Args:
         path: The disk image to attach.
         keyphrase: Optional parameter for encrypted images.
+        mountpoint: Optional path where disk image should be mounted.
 
     Returns:
         Tuple containing status code and information on mounted volume,
         if successful.
     """
-    return _hdiutil([
+    args: list[str] = [
         'attach',
         path,
         '-nobrowse'  # Do not make the mounted volumes visible in Finder.app
-    ], keyphrase=keyphrase)
+    ]
+
+    if mountpoint is not None:
+        args.extend(['-mountpoint', mountpoint])
+
+    return _hdiutil(args, keyphrase=keyphrase)
 
 
 def _hdiutil_detach(dev_node, force=False) -> bool:
     """Detaches a disk image.
 
     Args:
         dev_node: Filesystem path to attached volume, e.g. `/dev/disk1s1`.
@@ -344,17 +350,20 @@
     def has_license_agreement(self) -> bool:
         """Checks whether the disk image has an attached license agreement.
 
         DMGs with license agreements cannot be attached using this package.
         """
         return self._lookup_property('Software License Agreement', False)
 
-    def attach(self):
+    def attach(self, mountpoint=None):
         """Attaches a disk image.
 
+        Args:
+            mountpoint: Optional path where disk image should be mounted.
+
         Returns:
             List of mount points.
 
         Raises:
             InvalidOperation: This disk image has already been attached.
             LicenseAgreementNeedsAccepting: The image cannot be automatically 
                 mounted due to a license agreement.
@@ -363,31 +372,28 @@
         """
         if self.status.is_attached():
             raise InvalidOperation()
 
         if self.has_license_agreement():
             raise LicenseAgreementNeedsAccepting()
 
-        success, result = _hdiutil_attach(self.path, keyphrase=self.keyphrase)
+        success, result = _hdiutil_attach(self.path, keyphrase=self.keyphrase, mountpoint=mountpoint)
         if not success:
             raise AttachingFailed('Attaching failed for unknown reasons.')
 
         mounted_volumes = [MountedVolume(mount_point=entity['mount-point'],
                                          volume_kind=entity['volume-kind'])
                            for entity in result.get('system-entities', [])
                            if 'mount-point' in entity and 'volume-kind' in entity]
 
         if len(mounted_volumes) == 0:
             raise AttachingFailed('Attaching the disk image mounted no volumes.')
 
         # The root dev entry is the smallest '/dev/disk...' entry when sorted
         # lexicographically. (/dev/disk2 < /dev/disk3 < /dev/disk3s1)
-        # In the case of disk images containing APFS volumes, we need to detach this disk _after_
-        # detaching the main volumes. This is a bug in Apple's code -- for all other types of volumes,
-        # detaching the volume automatically detaches the entire disk image.
         root_dev_entry = sorted(entity['dev-entry']
                                 for entity in result.get('system-entities', [])
                                 if 'dev-entry' in entity)[0]
 
         self.status.record_attached(mounted_volumes, root_dev_entry)
         return [volume.mount_point for volume in self.status.mount_points]
 
@@ -400,29 +406,14 @@
         Raises:
             InvalidOperation: The disk image was not attached on the system.
             DetachingFailed: Detaching failed for unknown reasons.
         """
         if not self.status.is_attached():
             raise InvalidOperation()
 
-        # Detaching any mount point of an attached image automatically unmounts
-        # all associated volumes.
-        # ... unless one of these volumes is an APFS volume. In that case,
-        # it needs to be detached separately. Additionally, the root dev entry
-        # also needs to be detached explicitly.
-
-        # First detach all APFS volumes, otherwise detaching other volumes appears to
-        # succeeds but really fails with an error code (!)
-        for volume in self.status.mount_points:
-            if volume.volume_kind == 'apfs':
-                success = _hdiutil_detach(volume.mount_point, force=force)
-                if not success:
-                    raise DetachingFailed()
-
-        # Finally, detach the root dev entry.
         success = _hdiutil_detach(self.status.root_dev_entry, force=force)
         if not success:
             raise DetachingFailed()
 
         self.status.record_detached()
 
     def convert(self, path: str, disk_format: DiskFormat) -> str:
```

