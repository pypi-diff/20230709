# Comparing `tmp/astrometry_net_client-0.2.9.tar.gz` & `tmp/astrometry_net_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrometry_net_client-0.2.9.tar", last modified: Thu Nov 17 08:24:29 2022, max compression
+gzip compressed data, was "astrometry_net_client-0.3.0.tar", last modified: Sun Jul  9 11:07:54 2023, max compression
```

## Comparing `astrometry_net_client-0.2.9.tar` & `astrometry_net_client-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/
--rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.2.9/LICENSE
--rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.2.9/README.rst
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/astrometry_net_client/
--rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.2.9/astrometry_net_client/__init__.py
--rw-r--r--   0 sten      (1000) sten      (1000)     8994 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/client.py
--rw-r--r--   0 sten      (1000) sten      (1000)      448 2022-11-02 18:32:11.000000 astrometry_net_client-0.2.9/astrometry_net_client/config.py
--rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.2.9/astrometry_net_client/exceptions.py
--rw-r--r--   0 sten      (1000) sten      (1000)     6688 2022-11-02 19:09:33.000000 astrometry_net_client-0.2.9/astrometry_net_client/request.py
--rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.2.9/astrometry_net_client/session.py
--rw-r--r--   0 sten      (1000) sten      (1000)     7743 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/settings.py
--rw-r--r--   0 sten      (1000) sten      (1000)    16080 2022-11-02 18:34:56.000000 astrometry_net_client-0.2.9/astrometry_net_client/statusables.py
--rw-r--r--   0 sten      (1000) sten      (1000)     3774 2022-11-02 18:32:30.000000 astrometry_net_client-0.2.9/astrometry_net_client/uploads.py
-drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/
--rw-r--r--   0 sten      (1000) sten      (1000)     6277 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/PKG-INFO
--rw-r--r--   0 sten      (1000) sten      (1000)      565 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/SOURCES.txt
--rw-r--r--   0 sten      (1000) sten      (1000)        1 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/dependency_links.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       17 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/requires.txt
--rw-r--r--   0 sten      (1000) sten      (1000)       22 2022-11-17 08:24:29.000000 astrometry_net_client-0.2.9/astrometry_net_client.egg-info/top_level.txt
--rw-r--r--   0 sten      (1000) sten      (1000)      128 2022-11-17 08:24:29.592383 astrometry_net_client-0.2.9/setup.cfg
--rw-r--r--   0 sten      (1000) sten      (1000)     1140 2022-11-17 08:17:40.000000 astrometry_net_client-0.2.9/setup.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/
+-rw-r--r--   0 sten      (1000) sten      (1000)     1067 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/LICENSE
+-rw-r--r--   0 sten      (1000) sten      (1000)     6328 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)     5396 2022-08-30 09:48:22.000000 astrometry_net_client-0.3.0/README.rst
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/astrometry_net_client/
+-rw-r--r--   0 sten      (1000) sten      (1000)      345 2022-11-02 18:32:15.000000 astrometry_net_client-0.3.0/astrometry_net_client/__init__.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8638 2023-07-09 11:07:15.000000 astrometry_net_client-0.3.0/astrometry_net_client/client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      448 2022-11-02 18:32:11.000000 astrometry_net_client-0.3.0/astrometry_net_client/config.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      663 2022-11-02 18:32:13.000000 astrometry_net_client-0.3.0/astrometry_net_client/exceptions.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     6688 2022-11-02 19:09:33.000000 astrometry_net_client-0.3.0/astrometry_net_client/request.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     5036 2022-11-02 18:32:23.000000 astrometry_net_client-0.3.0/astrometry_net_client/session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     8102 2023-07-09 11:07:15.000000 astrometry_net_client-0.3.0/astrometry_net_client/settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)    16080 2022-11-02 18:34:56.000000 astrometry_net_client-0.3.0/astrometry_net_client/statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     3774 2023-07-09 10:19:18.000000 astrometry_net_client-0.3.0/astrometry_net_client/uploads.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/
+-rw-r--r--   0 sten      (1000) sten      (1000)     6328 2023-07-09 11:07:54.000000 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/PKG-INFO
+-rw-r--r--   0 sten      (1000) sten      (1000)      731 2023-07-09 11:07:54.000000 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)        1 2023-07-09 11:07:54.000000 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       17 2023-07-09 11:07:54.000000 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/requires.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)       22 2023-07-09 11:07:54.000000 astrometry_net_client-0.3.0/astrometry_net_client.egg-info/top_level.txt
+-rw-r--r--   0 sten      (1000) sten      (1000)      128 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/setup.cfg
+-rw-r--r--   0 sten      (1000) sten      (1000)     1190 2023-07-09 11:07:15.000000 astrometry_net_client-0.3.0/setup.py
+drwxr-xr-x   0 sten      (1000) sten      (1000)        0 2023-07-09 11:07:54.487506 astrometry_net_client-0.3.0/tests/
+-rw-r--r--   0 sten      (1000) sten      (1000)     2992 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1674 2023-07-09 11:07:15.000000 astrometry_net_client-0.3.0/tests/test_client.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2489 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test_job.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2366 2023-07-09 11:07:15.000000 astrometry_net_client-0.3.0/tests/test_online.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     1736 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test_session.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     3673 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test_settings.py
+-rw-r--r--   0 sten      (1000) sten      (1000)     2987 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test_statusables.py
+-rw-r--r--   0 sten      (1000) sten      (1000)      924 2022-08-30 07:13:54.000000 astrometry_net_client-0.3.0/tests/test_upload.py
```

### Comparing `astrometry_net_client-0.2.9/LICENSE` & `astrometry_net_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/PKG-INFO` & `astrometry_net_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: astrometry_net_client
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `astrometry_net_client-0.2.9/README.rst` & `astrometry_net_client-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/client.py` & `astrometry_net_client-0.3.0/astrometry_net_client/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import time
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from queue import Queue
 
 from astrometry_net_client.session import Session
 from astrometry_net_client.settings import Settings
 from astrometry_net_client.uploads import FileUpload
 
 log = logging.getLogger(__name__)
 
@@ -58,118 +58,117 @@
 
         log.info("Logging in")
         self.session.login()
 
     def upload_files_gen(
         self,
         files_iter,
-        filter_func=None,
-        filter_args=None,
-        workers=MAX_WORKERS,
+        queue_size=MAX_WORKERS,
     ):
         """
         Generator which uploads a number of files concurrently, yielding the
         :py:class:`astrometry_net_client.statusables.Job` & filename when done.
 
         Note that the ``files_iter`` argument is fully consumed when submitting
         to the executor is done. This means that the results will only be
         yielded once the iterator is consumed.
 
         Parameters
         ----------
         files_iter: iterable
             Some iterable containing paths to the files which will be uploaded.
             Is fully consumed before any result is yielded.
-        workers: int, optional
-            A positive integer, controlling the amount of workers to use for
-            the processing. Will not exceed the value of
+        queue_size: int, optional
+            A positive integer, controlling the size of the queue. This will
+            determine the maximum number of simultaneous submissions. Must be
+            greater than 0 and lower than :py:const:`MAX_WORKERS`. Default is
             :py:const:`MAX_WORKERS`.
-        filter_func: Callable
-            Predicate filter function which takes in the `filename` and
-            optionally some argument (`filter_args`).
-        filter_args: List
-            Arguments which are to be passed to the filter function.
 
         Yields
         ------
         (:py:class:`astrometry_net_client.statusables.Job`, ``str``):
             A tuple containing the finished
             :py:class:`astrometry_net_client.statusables.Job` and the
             corresponding filename. Yields when the Job is finished.
             NOTE: Order of yielded filenames can (and likely will) be different
             from the given ``files_iter``
+
+        Raises
+        ------
+        ValueError
+            When the queue_size is invalid.
         """
-        workers = min(MAX_WORKERS, workers)
-        with ThreadPoolExecutor(max_workers=workers) as executor:
-            log.info("Spawned executor {}".format(executor))
-
-            # submit the files & save which future corresponds to which
-            #  filename
-            future_to_file = {
-                executor.submit(
-                    self.filtered_upload_wrapper,
-                    filename,
-                    filter_func=filter_func,
-                    filter_args=filter_args,
-                ): filename
-                for filename in files_iter
-            }
+        SLEEP_TIME = 0.3  # seconds
+
+        files_iter = iter(files_iter)
+        if queue_size < 1 or queue_size > MAX_WORKERS:
+            raise ValueError(
+                "queue_size must be greater than 0 and less or equal to ",
+                f"{MAX_WORKERS}, was: {queue_size}",
+            )
+        processing_queue = Queue(maxsize=queue_size)
+
+        # Populate queue initially
+        for _, filename in zip(range(queue_size), files_iter):
+            self._insert_submission(filename, processing_queue)
+
+        while not processing_queue.empty():
+            filename, submission, job = processing_queue.get()
+            log_msg = "Checking file {}, job exists: {}"
+            log.debug(log_msg.format(filename, job is not None))
+            # The item in the queue has 2 states; if it is still only a
+            # submission job will be None and we have to create a job out of
+            # it. When the job is made, we can check if the job is done. When
+            # the job is finished return (yield) the value, otherwise put it
+            # back in the queue.
+
+            if job is None:
+                submission.status()
+                if submission.done():
+                    job = submission.jobs[0]
+                else:
+                    processing_queue.put((filename, submission, job))
+                    continue
 
-            # iterate over the results once they are completed.
-            for future in as_completed(future_to_file):
-                result_filename = future_to_file[future]
+            job.status()
+            if job.done():
                 try:
-                    res_job = future.result()
-                except Exception as e:
-                    # This exception is thrown inside the computed function.
-                    err_msg = "File {} stopped with exception {}"
-                    log.error(err_msg.format(result_filename, e))
+                    filename = next(files_iter)
+                except StopIteration:
+                    pass
                 else:
-                    if res_job is not None:  # ignore if file was filtered out
-                        yield res_job, result_filename
+                    self._insert_submission(filename, processing_queue)
+                log_msg = "FINISHED submission {}, yielding..."
+                log.info(log_msg.format(filename))
+                yield (job, filename)
+            else:
+                processing_queue.put((filename, submission, job))
 
-    def filtered_upload_wrapper(
-        self, filename, filter_func=None, filter_args=None, *args, **kwargs
-    ):
+            time.sleep(SLEEP_TIME)
+
+    def _insert_submission(self, filename, queue):
         """
-        Wrapper around :py:func:`upload_file` which filters the given file
-        based on a specified filter function.  Main use for this is a
-        computationally heavy filter function, like counting number of sources
-        locally, and only uploading if not enough are detected.
+        Helper function which creates an upload for the given filename, and
+        inserts the submission in a queue. This is not intended to be used
+        by a user.
 
         Parameters
         ----------
         filename: str
-            File to be uploaded. See :py:func:`upload_file`.
-        filter_func: Callable
-            Predicate filter function which takes in the `filename` and
-            optionally some argument (`filter_args`).
-        filter_args: List
-            Arguments which are to be passed to the filter function.
-        args: other arguments
-            Directly passed to :py:func:`upload_file`
-        kwargs: keyword arguments
-            Directly passed to :py:func:`upload_file`
-
-        Returns
-        -------
-        Job or None: :py:class:`astrometry_net_client.statusables.Job`, `None`
-            Will be the job of the resulting upload (see
-            :py:func:`upload_file`), or `None` when `filter_func` evaluated to
-            `False`.
+            The filename of the file to be submitted into the queue.
+        queue: Queue
+            The queue in which to insert the submission.
         """
-        if filter_args is None:
-            # allow arguments to be unpackable if it is not specified
-            filter_args = []
-
-        if filter_func is not None and not filter_func(filename, *filter_args):
-            log.info("Filter function failed, skipping upload")
-            return None
-
-        return self.upload_file(filename, *args, **kwargs)
+        log_msg = "Submitting file {}"
+        log.info(log_msg.format(filename))
+        upl = FileUpload(
+            filename, session=self.session, settings=self.settings
+        )
+        submission = upl.submit()
+        queue.put((filename, submission, None))
 
     def upload_file(self, filename, settings=None):
         """
         Uploads file and returns completed job when finished solving.
 
         Parameters
         ----------
```

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/exceptions.py` & `astrometry_net_client-0.3.0/astrometry_net_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/request.py` & `astrometry_net_client-0.3.0/astrometry_net_client/request.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/session.py` & `astrometry_net_client-0.3.0/astrometry_net_client/session.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/settings.py` & `astrometry_net_client-0.3.0/astrometry_net_client/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,20 +157,24 @@
     def __setattr__(self, name, value):
         if name == "data":
             return super().__setattr__(name, value)
         return self.__setitem__(name, value)
 
     def set_scale_range(self, lower, upper, unit="arcminwidth"):
         """
-        Specify the size of your field using a range.
+        Specify the size of your field (units 'arcminwidth' or 'degwitdth') or
+        the plate scale (unit 'arcsecperpix') using a range.
 
         Set the upper and lower limits for the field size of your upload. The
         unit is defined by the ``unit`` parameter, which defaults to
         ``'arcminwidth'``.
 
+        Do not set the range too small, otherwise Astrometry might not be able
+        to solve your upload.
+
         Incompatible with :py:func:`set_scale_estimate`
 
         Parameters
         ----------
         lower: float
             Number which defines the lowest value for your field size.
         upper: float
@@ -198,16 +202,20 @@
         # Commit changes, only if all are valid (e.g. no exception was raised)
         self.update(tmp)
 
     def set_scale_estimate(self, estimate, error, unit="arcminwidth"):
         """
         Specify the size of your field using an estimate + a deviation (error)
 
-        Sets the size of your field by an estimate + error pair. Will result in
-        a range of (estimate - error, estimate + error).
+        Sets the size of your field by an estimate + error pair. The estimate
+        is the central value, and the error (given in percent) specifies the
+        deviation around this value.
+
+        Do not set the error too low, otherwise Astrometry might not be able to
+        solve your upload.
 
         Incompatible with :py:func:`set_scale_range`
 
         Parameters
         ----------
         estimate: float
             The estimate center value for your field size.
```

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/statusables.py` & `astrometry_net_client-0.3.0/astrometry_net_client/statusables.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client/uploads.py` & `astrometry_net_client-0.3.0/astrometry_net_client/uploads.py`

 * *Files identical despite different names*

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client.egg-info/PKG-INFO` & `astrometry_net_client-0.3.0/astrometry_net_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: astrometry-net-client
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python interface for the Astrometry.net API.
 Home-page: https://github.com/StenSipma/astrometry_net_client
 Author: Sten Sipma
 Author-email: sten.sipma@ziggo.nl
 Keywords: astronomy astrometry client coordinates wcs api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `astrometry_net_client-0.2.9/astrometry_net_client.egg-info/SOURCES.txt` & `astrometry_net_client-0.3.0/astrometry_net_client.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,8 +11,16 @@
 astrometry_net_client/settings.py
 astrometry_net_client/statusables.py
 astrometry_net_client/uploads.py
 astrometry_net_client.egg-info/PKG-INFO
 astrometry_net_client.egg-info/SOURCES.txt
 astrometry_net_client.egg-info/dependency_links.txt
 astrometry_net_client.egg-info/requires.txt
-astrometry_net_client.egg-info/top_level.txt
+astrometry_net_client.egg-info/top_level.txt
+tests/test.py
+tests/test_client.py
+tests/test_job.py
+tests/test_online.py
+tests/test_session.py
+tests/test_settings.py
+tests/test_statusables.py
+tests/test_upload.py
```

### Comparing `astrometry_net_client-0.2.9/setup.py` & `astrometry_net_client-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="astrometry_net_client",
-    version="0.2.9",
+    version="0.3.0",
     author="Sten Sipma",
     author_email="sten.sipma@ziggo.nl",
     description="A Python interface for the Astrometry.net API.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/StenSipma/astrometry_net_client",
     packages=["astrometry_net_client"],
@@ -18,14 +18,15 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Operating System :: POSIX :: Linux",
         "Natural Language :: English",
     ],
     python_requires=">=3.8",
 )
```

