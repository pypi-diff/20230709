# Comparing `tmp/hydrusvideodeduplicator-0.2.2.tar.gz` & `tmp/hydrusvideodeduplicator-0.2.3.tar.gz`

## Comparing `hydrusvideodeduplicator-0.2.2.tar` & `hydrusvideodeduplicator-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/docker-compose.yml
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/docker-entrypoint.sh
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/LICENSE
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/README.md
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/docker-compose.yml
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/docker-entrypoint.sh
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    17840 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/README.md
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.2.2/docker-compose.yml` & `hydrusvideodeduplicator-0.2.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.2.3/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import typer
 from rich import print as rprint
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 
 from .__about__ import __version__
-from .config import HYDRUS_API_KEY, HYDRUS_API_URL, HYDRUS_QUERY, REQUESTS_CA_BUNDLE
+from .config import HYDRUS_API_KEY, HYDRUS_API_URL, REQUESTS_CA_BUNDLE, HYDRUS_QUERY, HYDRUS_LOCAL_FILE_SERVICE_KEYS
 from .dedup import HydrusVideoDeduplicator
 
 """
 Parameters:
 - api_key will be read from env var $HYDRUS_API_KEY or .env file
 - api_url will be read from env var $HYDRUS_API_URL or .env file
 - to add custom queries, do
@@ -30,24 +30,24 @@
     query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = HYDRUS_QUERY,
     threshold: Annotated[
         Optional[float], typer.Option(help="Similarity threshold for a pair of videos where 100 is identical")
     ] = 75.0,
     skip_hashing: Annotated[
         Optional[bool], typer.Option(help="Skip perceptual hashing and just search for duplicates")
     ] = False,
+    file_service_key: Annotated[Optional[List[str]], typer.Option(help="Local file service key")] = HYDRUS_LOCAL_FILE_SERVICE_KEYS,
     verify_cert: Annotated[
         Optional[str], typer.Option(help="Path to TLS cert. This forces verification.")
     ] = REQUESTS_CA_BUNDLE,
     clear_search_cache: Annotated[
         Optional[bool], typer.Option(help="Clear the cache that tracks what files have already been compared")
     ] = False,
     verbose: Annotated[Optional[bool], typer.Option(help="Verbose logging")] = False,
     debug: Annotated[Optional[bool], typer.Option(hidden=True)] = False,
 ):
-
     # CLI debug parameter sets log level to info or debug
     loglevel = logging.WARNING
     if debug:
         loglevel = logging.DEBUG
         verbose = True
 
     logging.basicConfig(format=' %(asctime)s - %(name)s: %(message)s', datefmt='%H:%M:%S', level=loglevel)
@@ -59,19 +59,17 @@
         logging.disable()
 
     # Clear cache
     if clear_search_cache:
         HydrusVideoDeduplicator.clear_search_cache()
         rprint("[green] Cleared search cache.")
 
-    # CLI overwrites env vars
+    # CLI overwrites env vars with no default value
     if not api_key:
         api_key = HYDRUS_API_KEY
-    if not api_url:
-        api_url = HYDRUS_API_URL
 
     # Check for necessary variables
     if not api_key:
         print("API key not set. Exiting...")
         raise typer.Exit(code=1)
     # This should not happen because there's a default val in secret.py
     if not api_url:
@@ -135,15 +133,16 @@
         rprint("[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
         raise typer.Exit(code=1)
     superdeduper.threshold = threshold
 
     superdeduper.clear_trashed_files_from_db()
 
     # Run all deduplicate functionality
-    superdeduper.deduplicate(overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing)
+    superdeduper.deduplicate(overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing,
+                             file_service_keys=file_service_key)
 
     raise typer.Exit()
 
 
 try:
     typer.run(main)
 except KeyboardInterrupt as exc:
```

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 
 from joblib import Parallel, delayed
 from rich import print as rprint
 from sqlitedict import SqliteDict
 from tqdm import tqdm
 
 if TYPE_CHECKING:
-    pass
+    from typing import Any
+    from collections.abc import Iterable, Sequence, Generator
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 import hydrusvideodeduplicator.hydrus_api.utils
-from .vpdqpy.vpdqpy import Vpdq
 
-from .config import DEDUP_DATABASE_DIR, DEDUP_DATABASE_FILE, DEDUP_DATABASE_NAME
-from .dedup_util import database_accessible, find_tag_in_tags, get_file_names_hydrus
+from .config import DEDUP_DATABASE_DIR, DEDUP_DATABASE_FILE
+from .dedup_util import database_accessible
+from .vpdqpy.vpdqpy import Vpdq
 
 
 class HydrusVideoDeduplicator:
     hydlog = logging.getLogger("hydlog")
     threshold: float = 75.0
     _DEBUG = False
 
@@ -35,70 +36,101 @@
 
         # Commonly used things from the Hydrus database
         # If any of these are large they should probably be lazily loaded
         self.all_services = self.client.get_services()
 
     # Verify client connection and permissions
     # Will throw a hydrus_api.APIError if something is wrong
-    def verify_api_connection(self):
+    def verify_api_connection(self) -> None:
         self.hydlog.info(
             f"Client API version: v{self.client.VERSION} | Endpoint API version: v{self.client.get_api_version()['version']}"
         )
         hydrus_api.utils.verify_permissions(self.client, hydrus_api.utils.Permission)
 
+    # Verify that the supplied file_service_key is a valid key for a local file service
+    def verify_file_service_keys(self, file_service_keys: Iterable[str]) -> None:
+        VALID_SERVICE_TYPES = [hydrus_api.ServiceType.ALL_LOCAL_FILES, hydrus_api.ServiceType.FILE_DOMAIN]
+
+        for file_service_key in file_service_keys:
+            file_service = self.all_services['services'].get(file_service_key)
+            if file_service is None:
+                raise KeyError(f"Invalid file service key: '{file_service_key}'")
+
+            service_type = file_service.get('type')
+            if service_type not in VALID_SERVICE_TYPES:
+                raise KeyError("File service key must be a local file service")
+
     # This is the master function of the class
-    def deduplicate(self, overwrite: bool = False, custom_query: list | None = None, skip_hashing: bool | None = False):
+    def deduplicate(
+        self,
+        overwrite: bool = False,
+        custom_query: Sequence[str] | None = None,
+        skip_hashing: bool = False,
+        file_service_keys: Sequence[str] | None = None,
+    ) -> None:
         # Add perceptual hashes to video files
         # system:filetype tags are really inconsistent
         search_tags = ['system:filetype=video, gif, apng', 'system:has duration']
 
         query = False
         if custom_query is not None:
-            custom_query = [x for x in custom_query if x.strip()]  # Remove whitespace and empty strings
+            # Remove whitespace and empty strings
+            custom_query = [x for x in custom_query if x.strip()]
             if len(custom_query) > 0:
                 search_tags.extend(custom_query)
                 rprint(f"[yellow] Custom Query: {custom_query}")
                 query = True
 
+        # Set the file service keys to be used for hashing
+        # Default is "all local files"
+        if file_service_keys is None or not file_service_keys:
+            file_service_keys = [self.all_services["all_local_files"][0]["service_key"]]
+        else:
+            file_service_keys = [x for x in file_service_keys if x.strip()]
+        self.verify_file_service_keys(file_service_keys)
+
         video_hashes = None
         if skip_hashing:
             rprint("[yellow] Skipping perceptual hashing")
             if query:
-                video_hashes = set(self._retrieve_video_hashes(search_tags))
+                video_hashes = set(self._retrieve_video_hashes(search_tags, file_service_keys))
         else:
-            all_video_hashes = self._retrieve_video_hashes(search_tags)
+            all_video_hashes = self._retrieve_video_hashes(search_tags, file_service_keys)
             self._add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=all_video_hashes)
-        
+
         if query and not skip_hashing:
-            video_hashes = set(self._retrieve_video_hashes(search_tags))
+            video_hashes = set(self._retrieve_video_hashes(search_tags, file_service_keys))
 
         if query:
-            self._find_potential_duplicates(limited_video_hashes=video_hashes)
+            self._find_potential_duplicates(limited_video_hashes=video_hashes, file_service_keys=file_service_keys)
         else:
-            self._find_potential_duplicates(limited_video_hashes=None)
+            self._find_potential_duplicates(limited_video_hashes=None, file_service_keys=file_service_keys)
 
         self.hydlog.info("Deduplication done.")
 
     @staticmethod
-    def _calculate_perceptual_hash(video: str | bytes) -> str:
+    def _calculate_perceptual_hash(video: Path | str | bytes) -> str:
         perceptual_hash = Vpdq.vpdq_to_json(Vpdq.computeHash(video))
         assert perceptual_hash != "[]"
         return perceptual_hash
 
-    def _retrieve_video_hashes(self, search_tags) -> list:
+    def _retrieve_video_hashes(
+        self, search_tags: Iterable[str], file_service_keys: Iterable[str] | None = None
+    ) -> Iterable[str]:
         all_video_hashes = self.client.search_files(
-            search_tags,
+            tags=search_tags,
+            file_service_keys=file_service_keys,
             file_sort_type=hydrus_api.FileSortType.FILE_SIZE,
             return_hashes=True,
             file_sort_asc=True,
             return_file_ids=False,
         )["hashes"]
         return all_video_hashes
 
-    def _add_perceptual_hashes_to_db(self, overwrite: bool, video_hashes=set | list) -> None:
+    def _add_perceptual_hashes_to_db(self, overwrite: bool, video_hashes: Sequence[str]) -> None:
         # Create database folder
         try:
             os.makedirs(DEDUP_DATABASE_DIR, exist_ok=False)
             # Exception before this log if directory already exists
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
         except OSError:
             pass
@@ -164,20 +196,18 @@
             else:
                 rprint("[green] Finished perceptual hash processing.")
 
             finally:
                 hashdb.commit()
                 self.hydlog.info("Finished perceptual hash processing.")
 
-    def get_potential_duplicate_count_hydrus(self) -> int:
-        return self.client.get_potentials_count(
-            file_service_keys=[self.all_services["all_local_files"][0]["service_key"]]
-        )["potential_duplicates_count"]
+    def get_potential_duplicate_count_hydrus(self, file_service_keys: Iterable[str]) -> int:
+        return self.client.get_potentials_count(file_service_keys=file_service_keys)["potential_duplicates_count"]
 
-    def compare_videos(self, video1_hash: str, video2_hash: str, video1_phash: str, video2_phash: str):
+    def compare_videos(self, video1_hash: str, video2_hash: str, video1_phash: str, video2_phash: str) -> None:
         vpdq_hash1 = Vpdq.json_to_vpdq(video1_phash)
         vpdq_hash2 = Vpdq.json_to_vpdq(video2_phash)
         similar, similarity = Vpdq.is_similar(vpdq_hash1, vpdq_hash2, self.threshold)
 
         if similar:
             if self._DEBUG:
                 # Getting the file names will be VERY slow because of the API call
@@ -192,35 +222,37 @@
                 "do_default_content_merge": True,
             }
 
             self.client.set_file_relationships([new_relationship])
 
     # Delete cache row in database
     @staticmethod
-    def clear_search_cache():
+    def clear_search_cache() -> None:
         try:
             with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
                 for key in hashdb:
                     row = hashdb[key]
                     if "farthest_search_index" in row:
                         del row["farthest_search_index"]
                     hashdb[key] = row
                 hashdb.commit()
         except OSError:
             rprint(f"[red] Database does not exist. Cannot clear search cache.")
 
     # Sliding window duplicate comparisons
     # Alternatively, I could scan duplicates when added and never do it again which would be one of the best ways without a VP tree
-    def _find_potential_duplicates(self, limited_video_hashes: list | set | None = None) -> None:
+    def _find_potential_duplicates(
+        self, limited_video_hashes: Sequence[str] | None = None, file_service_keys: Iterable[str] | None = None
+    ) -> None:
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos", verbose=True):
             rprint(f"[red] Could not search for duplicates.")
             return
 
         # Number of potential duplicates before adding more. Just for user info.
-        pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
+        pre_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
 
         # BUG: If this process is interrupted, the farthest_search_index will not save for ANY entries.
         #      I think it might be because every entry in the column needs an entry for SQlite but I'm not sure.
         video_counter = 0
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
             try:
                 if limited_video_hashes is not None:
@@ -291,48 +323,52 @@
 
             except KeyboardInterrupt:
                 pass
             finally:
                 hashdb.commit()
 
         # Statistics for user
-        post_dedupe_count = self.get_potential_duplicate_count_hydrus()
+        post_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
         new_dedupes_count = post_dedupe_count - pre_dedupe_count
         if new_dedupes_count > 0:
             rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
         else:
             rprint("[green] No new potential duplicates found.")
 
     @staticmethod
-    def batched(iterable, n):
+    def batched(iterable, n) -> Generator[tuple, Any, None]:
         "Batch data into tuples of length n. The last batch may be shorter."
         # batched('ABCDEFG', 3) --> ABC DEF G
         if n < 1:
             raise ValueError('n must be at least one')
         it = iter(iterable)
         while batch := tuple(islice(it, n)):
             yield batch
 
     # Check if files are trashed
     # Returns a dictionary of hash : trashed_or_not
-    def is_files_trashed_hydrus(self, file_hashes: list[str]) -> dict:
+    def is_files_trashed_hydrus(self, file_hashes: Iterable[str]) -> dict:
         videos_metadata = self.client.get_file_metadata(hashes=file_hashes, only_return_basic_information=False)[
             "metadata"
         ]
 
         result = {}
         for video_metadata in videos_metadata:
+            # This should never happen
+            if "hash" not in video_metadata:
+                logging.error("Hash not found for potentially trashed file.")
+                continue
             video_hash = video_metadata['hash']
-            is_trashed = video_metadata['is_trashed']
-            is_deleted = video_metadata['is_deleted']
+            is_trashed: bool = video_metadata.get('is_trashed', False)
+            is_deleted: bool = video_metadata.get('is_deleted', False)
             result[video_hash] = is_trashed or is_deleted
         return result
 
     # Delete trashed and deleted files from Hydrus from the database
-    def clear_trashed_files_from_db(self):
+    def clear_trashed_files_from_db(self) -> None:
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
             return
 
         try:
             CHUNK_SIZE = 32
             delete_count = 0
             with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
```

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,24 +127,27 @@
         return self.pdqHash256FromFloatLuma(
             buffer1, buffer2, numRows, numCols, buffer64x64, buffer16x64, buffer16x16
         )
 
     def fillFloatLumaFromBufferImage(self, img, luma):
         numCols, numRows = img.size
         rgb_image = img.convert("RGB")
-        numCols, numRows = img.size
+        pixels = rgb_image.load()
+
         for i in range(numRows):
             for j in range(numCols):
-                r, g, b = rgb_image.getpixel((j, i))
+                r, g, b = pixels[j, i]
                 luma[i * numCols + j] = (
                     self.LUMA_FROM_R_COEFF * r
                     + self.LUMA_FROM_G_COEFF * g
                     + self.LUMA_FROM_B_COEFF * b
                 )
 
+
+
     def pdqHash256FromFloatLuma(
         self,
         fullBuffer1,
         fullBuffer2,
         numRows,
         numCols,
         buffer64x64,
@@ -161,16 +164,16 @@
             windowSizeAlongRows,
             windowSizeAlongCols,
             self.PDQ_NUM_JAROSZ_XY_PASSES,
         )
         self.decimateFloat(fullBuffer1, numRows, numCols, buffer64x64)
         quality = self.computePDQImageDomainQualityMetric(buffer64x64)
         self.dct64To16(buffer64x64, buffer16x64, buffer16x16)
-        hash = self.pdqBuffer16x16ToBits(buffer16x16)
-        return HashAndQuality(hash, quality)
+        _hash = self.pdqBuffer16x16ToBits(buffer16x16)
+        return HashAndQuality(_hash, quality)
 
     def dihedralFromFile(self, filename, hashingMetadata, dihFlags):
         t1 = time.time()
         img = None
         try:
             img = Image.open(filename)
         except IOError as e:
@@ -247,24 +250,24 @@
             windowSizeAlongRows,
             windowSizeAlongCols,
             self.PDQ_NUM_JAROSZ_XY_PASSES,
         )
         self.decimateFloat(fullBuffer1, numRows, numCols, buffer64x64)
         quality = self.computePDQImageDomainQualityMetric(buffer64x64)
         self.dct64To16(buffer64x64, buffer16x64, buffer16x16)
-        hash = None
+        _hash = None
         hashRotate90 = None
         hashRotate180 = None
         hashRotate270 = None
         hashFlipX = None
         hashFlipY = None
         hashFlipPlus1 = None
         hashFlipMinus1 = None
         if (dihFlags & self.PDQ_DO_DIH_ORIGINAL) != 0:
-            hash = self.pdqBuffer16x16ToBits(buffer16x16)
+            _hash = self.pdqBuffer16x16ToBits(buffer16x16)
         if (dihFlags & self.PDQ_DO_DIH_ROTATE_90) != 0:
             self.dct16OriginalToRotate90(buffer16x16, buffer16x16Aux)
             hashRotate90 = self.pdqBuffer16x16ToBits(buffer16x16Aux)
         if (dihFlags & self.PDQ_DO_DIH_ROTATE_180) != 0:
             self.dct16OriginalToRotate180(buffer16x16, buffer16x16Aux)
             hashRotate180 = self.pdqBuffer16x16ToBits(buffer16x16Aux)
         if (dihFlags & self.PDQ_DO_DIH_ROTATE_270) != 0:
@@ -279,15 +282,15 @@
         if (dihFlags & self.PDQ_DO_DIH_FLIP_PLUS1) != 0:
             self.dct16OriginalToFlipPlus1(buffer16x16, buffer16x16Aux)
             hashFlipPlus1 = self.pdqBuffer16x16ToBits(buffer16x16Aux)
         if (dihFlags & self.PDQ_DO_DIH_FLIP_MINUS1) != 0:
             self.dct16OriginalToFlipMinus1(buffer16x16, buffer16x16Aux)
             hashFlipMinus1 = self.pdqBuffer16x16ToBits(buffer16x16Aux)
         return HashesAndQuality(
-            hash,
+            _hash,
             hashRotate90,
             hashRotate180,
             hashRotate270,
             hashFlipX,
             hashFlipY,
             hashFlipPlus1,
             hashFlipMinus1,
@@ -438,21 +441,21 @@
                     B[j][i] = A[i][j]
 
     def pdqBuffer16x16ToBits(self, dctOutput16x16):
         """
         Each bit of the 16x16 output hash is for whether the given frequency
         component is greater than the median frequency component or not.
         """
-        hash = Hash256()
+        _hash = Hash256()
         dctMedian = MatrixUtil.torben(dctOutput16x16, 16, 16)
         for i in range(16):
             for j in range(16):
                 if dctOutput16x16[i][j] > dctMedian:
-                    hash.setBit(i * 16 + j)
-        return hash
+                    _hash.setBit(i * 16 + j)
+        return _hash
 
     @classmethod
     def computeJaroszFilterWindowSize(cls, dimension):
         """Round up. See comments at top of file for details."""
         return int(
             (dimension + cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR - 1)
             / cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR
@@ -594,84 +597,64 @@
         inStartOffset,
         outvec,
         outStartOffset,
         vectorLength,
         stride,
         fullWindowSize,
     ):
-
-        halfWindowSize = int((fullWindowSize + 2) / 2)  # 7->4, 8->5
-        phase_1_nreps = int(halfWindowSize - 1)
-        phase_2_nreps = int(fullWindowSize - halfWindowSize + 1)
-        phase_3_nreps = int(vectorLength - fullWindowSize)
-        phase_4_nreps = int(halfWindowSize - 1)
-        li = 0  # Index of left edge of read window, for subtracts
-        ri = 0  # Index of right edge of read windows, for adds
-        oi = 0  # Index into output vector
-        sum = float(0.0)
+        halfWindowSize = (fullWindowSize + 2) // 2
+        phase_1_nreps = halfWindowSize - 1
+        phase_2_nreps = fullWindowSize - halfWindowSize + 1
+        phase_3_nreps = vectorLength - fullWindowSize
+        phase_4_nreps = halfWindowSize - 1
+        _sum = 0.0
         currentWindowSize = 0
 
         # PHASE 1: ACCUMULATE FIRST SUM NO WRITES
-        i = 0
-        while i < phase_1_nreps:
-            sum += invec[inStartOffset + ri]
+        for i in range(phase_1_nreps):
+            _sum += invec[inStartOffset + i * stride]
             currentWindowSize += 1
-            ri += stride
-            i += 1
+
         # PHASE 2: INITIAL WRITES WITH SMALL WINDOW
-        i = 0
-        while i < phase_2_nreps:
-            sum += invec[inStartOffset + ri]
+        for i in range(phase_2_nreps):
+            _sum += invec[inStartOffset + (i + phase_1_nreps) * stride]
             currentWindowSize += 1
-            outvec[outStartOffset + oi] = sum / currentWindowSize
-            ri += stride
-            oi += stride
-            i += 1
+            outvec[outStartOffset + i * stride] = _sum / currentWindowSize
+
         # PHASE 3: WRITES WITH FULL WINDOW
-        i = 0
-        while i < phase_3_nreps:
-            sum += invec[inStartOffset + ri]
-            sum -= invec[inStartOffset + li]
-            outvec[outStartOffset + oi] = sum / currentWindowSize
-            li += stride
-            ri += stride
-            oi += stride
-            i += 1
+        for i in range(phase_3_nreps):
+            _sum += invec[inStartOffset + (i + phase_2_nreps + phase_1_nreps) * stride]
+            _sum -= invec[inStartOffset + i * stride]
+            outvec[outStartOffset + (i + phase_2_nreps) * stride] = _sum / currentWindowSize
+
         # PHASE 4: FINAL WRITES WITH SMALL WINDOW
-        i = 0
-        while i < phase_4_nreps:
-            sum -= invec[inStartOffset + li]
+        for i in range(phase_4_nreps):
+            _sum -= invec[inStartOffset + (i + phase_3_nreps + phase_2_nreps) * stride]
             currentWindowSize -= 1
-            outvec[outStartOffset + oi] = sum / currentWindowSize
-            li += stride
-            oi += stride
-            i += 1
+            outvec[outStartOffset + (i + phase_3_nreps + phase_2_nreps) * stride] = _sum / currentWindowSize
+
 
     @classmethod
-    def boxAlongRowsFloat(cls, input, output, numRows, numCols, windowSize):
+    def boxAlongRowsFloat(cls, _input, output, numRows, numCols, windowSize):
         """
         input - matrix as numRows x numCols in row-major order
         output - matrix as numRows x numCols in row-major order
         """
-        i = 0
-        while i < numRows:
+        for i in range(numRows):
             cls.box1DFloat(
-                input,
+                _input,
                 i * numCols,
                 output,
                 i * numCols,
                 numCols,
                 1,  # stride
                 windowSize,
             )
-            i += 1
 
     @classmethod
-    def boxAlongColsFloat(cls, input, output, numRows, numCols, windowSize):
+    def boxAlongColsFloat(cls, _input, output, numRows, numCols, windowSize):
         """
         input - matrix as numRows x numCols in row-major order
         out - matrix as numRows x numCols in row-major order
         """
-        j = 0
-        while j < numCols:
-            cls.box1DFloat(input, j, output, j, numRows, numCols, windowSize)
-            j += 1
+        for j in range(numCols):
+            cls.box1DFloat(_input, j, output, j, numRows, numCols, windowSize)
```

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 #!/usr/bin/env python
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 
 
 class MatrixUtil:
     @classmethod
     def allocateMatrix(cls, numRows, numCols):
-        rv = [0.0] * numRows
-        for i in range(numRows):
-            rv[i] = [0.0] * numCols
+        rv = [[0.0] * numCols for _ in range(numRows)]
         return rv
 
     @classmethod
     def allocateMatrixAsRowMajorArray(cls, numRows, numCols):
         return [0.0] * numRows * numCols
 
     @classmethod
     def torben(cls, m, numRows, numCols):
         n = numRows * numCols
-        midn = int((n + 1) / 2)
-        less = int()
-        greater = int()
-        equal = int()
-        min = float()
-        max = float()
-        guess = float()
-        maxltguess = float()
-        mingtguess = float()
-        min = max = m[0][0]
+        midn = (n + 1) // 2
+        min_val = max_val = m[0][0]
+
         for i in range(numRows):
             for j in range(numCols):
                 v = m[i][j]
-                if v < min:
-                    min = v
-                if v > max:
-                    max = v
+                if v < min_val:
+                    min_val = v
+                if v > max_val:
+                    max_val = v
 
         while True:
-            guess = float((min + max) / 2)
+            guess = (min_val + max_val) / 2
             less = 0
             greater = 0
             equal = 0
-            maxltguess = min
-            mingtguess = max
+            maxltguess = min_val
+            mingtguess = max_val
 
-            for _i in range(numRows):
-                for _j in range(numCols):
-                    v = m[_i][_j]
+            for i in range(numRows):
+                for j in range(numCols):
+                    v = m[i][j]
                     if v < guess:
                         less += 1
                         if v > maxltguess:
                             maxltguess = v
                     elif v > guess:
                         greater += 1
                         if v < mingtguess:
                             mingtguess = v
                     else:
                         equal += 1
+
             if less <= midn and greater <= midn:
                 break
             elif less > greater:
-                max = maxltguess
+                max_val = maxltguess
             else:
-                min = mingtguess
+                min_val = mingtguess
+
         if less >= midn:
             return maxltguess
         elif less + equal >= midn:
             return guess
         else:
-            return mingtguess
+            return mingtguess
```

### Comparing `hydrusvideodeduplicator-0.2.2/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/.gitignore` & `hydrusvideodeduplicator-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.2/LICENSE` & `hydrusvideodeduplicator-0.2.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 appleappleapplenanner
+Copyright (c) 2023 hydrusvideodeduplicator
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hydrusvideodeduplicator-0.2.2/pyproject.toml` & `hydrusvideodeduplicator-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 dynamic = ["version"]
 description = "Video deduplicator utility for Hydrus Network"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "appleappleapplenanner", email = "applenannerapple@gmail.com" },
+  { name = "hydrusvideodeduplicator", email = "applenannerapple@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "appdirs",
     "rich",
     "numpy",
     "tqdm",
     "python-dotenv",
@@ -33,17 +32,17 @@
     "joblib",
     # Below is for vpdqpy
     "Pillow",
     "av",
 ]
 
 [project.urls]
-Documentation = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme"
-Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
-Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
+Documentation = "https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator#readme"
+Issues = "https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/issues"
+Source = "https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator"
 
 [tool.hatch.dependencies]
 hydrus_api = {path = "src/hydrusvideodeduplicator/hydrus_api"}
 vpdqpy = {path = "src/hydrusvideodeduplicator/vpdqpy"}
 
 [tool.hatch.build]
 exclude = [
```

