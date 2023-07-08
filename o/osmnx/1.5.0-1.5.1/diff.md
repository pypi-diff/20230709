# Comparing `tmp/osmnx-1.5.0.tar.gz` & `tmp/osmnx-1.5.1.tar.gz`

## Comparing `osmnx-1.5.0.tar` & `osmnx-1.5.1.tar`

### file list

```diff
@@ -1,75 +1,30 @@
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 osmnx-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20892 2020-02-02 00:00:00.000000 osmnx-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 osmnx-1.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 osmnx-1.5.0/MANIFEST.in
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 osmnx-1.5.0/.github/workflows/test-minimal.yml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/Makefile
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/conf.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/further-reading.rst
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/getting-started.rst
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/index.rst
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/installation.rst
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/internals-reference.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/make.bat
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/requirements.txt
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 osmnx-1.5.0/docs/user-reference.rst
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/Dockerfile
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/docker-build-single_platform.sh
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/docker-build.sh
--rw-r--r--   0        0        0    13614 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/environment.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/overrides.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/readme.md
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/docker/requirements.txt
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/linux/create-environment.sh
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/linux/environment.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/windows/create-environment.bat
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 osmnx-1.5.0/environments/windows/environment.yml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/__init__.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/_api.py
--rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/_downloader.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/_errors.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/_version.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/bearing.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/distance.py
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/elevation.py
--rw-r--r--   0        0        0    41870 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/features.py
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/folium.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/geocoder.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/geometries.py
--rw-r--r--   0        0        0    29480 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/graph.py
--rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/io.py
--rw-r--r--   0        0        0    18149 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/osm_xml.py
--rw-r--r--   0        0        0    31934 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/plot.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/projection.py
--rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/settings.py
--rw-r--r--   0        0        0    25680 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/simplification.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/speed.py
--rw-r--r--   0        0        0    12691 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/stats.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/truncate.py
--rw-r--r--   0        0        0    10548 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/utils.py
--rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/utils_geo.py
--rw-r--r--   0        0        0    18217 2020-02-02 00:00:00.000000 osmnx-1.5.0/osmnx/utils_graph.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/format.sh
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/git_repack.sh
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/lint_test.sh
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/packaging.sh
--rwxr-xr-x   0        0        0    21856 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/test_osmnx.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/environments/env-ci.yml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/environments/env-test-minimal.yml
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/input_data/West-Oakland.osm.bz2
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/input_data/elevation1.tif
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/input_data/elevation2.tif
--rw-r--r--   0        0        0    40557 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/input_data/planet_10.068,48.135_10.071,48.137.osm
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 osmnx-1.5.0/tests/input_data/short.graphml
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.5.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 osmnx-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 osmnx-1.5.0/README.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 osmnx-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 osmnx-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/__init__.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_api.py
+-rw-r--r--   0        0        0    29173 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_downloader.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_errors.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/_version.py
+-rw-r--r--   0        0        0    10407 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/bearing.py
+-rw-r--r--   0        0        0    18195 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/distance.py
+-rw-r--r--   0        0        0     9637 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/elevation.py
+-rw-r--r--   0        0        0    41877 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/features.py
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/folium.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/geocoder.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/geometries.py
+-rw-r--r--   0        0        0    30380 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/graph.py
+-rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/io.py
+-rw-r--r--   0        0        0    19063 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/osm_xml.py
+-rw-r--r--   0        0        0    31934 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/plot.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/projection.py
+-rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/settings.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/simplification.py
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/speed.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/stats.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/truncate.py
+-rw-r--r--   0        0        0    11228 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils_geo.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 osmnx-1.5.1/osmnx/utils_graph.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 osmnx-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 osmnx-1.5.1/README.md
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 osmnx-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 osmnx-1.5.1/PKG-INFO
```

### Comparing `osmnx-1.5.0/osmnx/_api.py` & `osmnx-1.5.1/osmnx/_api.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/_downloader.py` & `osmnx-1.5.1/osmnx/_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import numpy as np
 import requests
 
 from . import projection
 from . import settings
 from . import utils
 from . import utils_geo
-from ._errors import CacheOnlyModeInterrupt
 
 # capture getaddrinfo function to use original later after mutating it
 _original_getaddrinfo = socket.getaddrinfo
 
 
 def _get_osm_filter(network_type):
     """
@@ -526,49 +525,38 @@
     polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
         boundary to fetch the network ways/nodes within
     network_type : string
         what type of street network to get if custom_filter is None
     custom_filter : string
         a custom ways filter to be used instead of the network_type presets
 
-    Returns
-    -------
-    response_jsons : list
-        list of JSON responses from the Overpass server
+    Yields
+    ------
+    response_json : dict
+        a generator of JSON responses from the Overpass server
     """
     # create a filter to exclude certain kinds of ways based on the requested
     # network_type, if provided, otherwise use custom_filter
     if custom_filter is not None:
         osm_filter = custom_filter
     else:
         osm_filter = _get_osm_filter(network_type)
 
-    response_jsons = []
-
     # create overpass settings string
     overpass_settings = _make_overpass_settings()
 
     # subdivide query polygon to get list of sub-divided polygon coord strings
     polygon_coord_strs = _make_overpass_polygon_coord_strs(polygon)
     utils.log(f"Requesting data from API in {len(polygon_coord_strs)} request(s)")
 
     # pass each polygon exterior coordinates in the list to the API, one at a
     # time. The '>' makes it recurse so we get ways and the ways' nodes.
     for polygon_coord_str in polygon_coord_strs:
         query_str = f"{overpass_settings};(way{osm_filter}(poly:{polygon_coord_str!r});>;);out;"
-        response_json = _overpass_request(data={"data": query_str})
-        response_jsons.append(response_json)
-    utils.log(
-        f"Got all network data within polygon from API in {len(polygon_coord_strs)} request(s)"
-    )
-
-    if settings.cache_only_mode:  # pragma: no cover
-        raise CacheOnlyModeInterrupt("settings.cache_only_mode=True")
-
-    return response_jsons
+        yield _overpass_request(data={"data": query_str})
 
 
 def _osm_features_download(polygon, tags):
     """
     Retrieve OSM features within boundary from the Overpass API.
 
     Parameters
```

### Comparing `osmnx-1.5.0/osmnx/_errors.py` & `osmnx-1.5.1/osmnx/_errors.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/bearing.py` & `osmnx-1.5.1/osmnx/bearing.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
     """
     Calculate undirected graph's orientation entropy.
 
     Orientation entropy is the entropy of its edges' bidirectional bearings
     across evenly spaced bins. Ignores self-loop edges as their bearings are
     undefined.
 
+    For more info see: Boeing, G. 2019. "Urban Spatial Order: Street Network
+    Orientation, Configuration, and Entropy." Applied Network Science, 4 (1),
+    67. https://doi.org/10.1007/s41109-019-0189-1
+
     Parameters
     ----------
     Gu : networkx.MultiGraph
         undirected, unprojected graph with `bearing` attributes on each edge
     num_bins : int
         number of bins; for example, if `num_bins=36` is provided, then each
         bin will represent 10° around the compass
```

### Comparing `osmnx-1.5.0/osmnx/distance.py` & `osmnx-1.5.1/osmnx/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,24 +466,23 @@
         destination node ID
     k : int
         number of shortest paths to solve
     weight : string
         edge attribute to minimize when solving shortest paths. default is
         edge length in meters.
 
-    Returns
-    -------
-    paths : generator
+    Yields
+    ------
+    path : list
         a generator of `k` shortest paths ordered by total weight. each path
         is a list of node IDs.
     """
     _verify_edge_attribute(G, weight)
     paths_gen = nx.shortest_simple_paths(utils_graph.get_digraph(G, weight), orig, dest, weight)
-    for path in itertools.islice(paths_gen, 0, k):
-        yield path
+    yield from itertools.islice(paths_gen, 0, k)
 
 
 def _verify_edge_attribute(G, attr):
     """
     Verify attribute values are numeric and non-null across graph edges.
 
     Raises a `ValueError` if attribute contains non-numeric values and raises
```

### Comparing `osmnx-1.5.0/osmnx/elevation.py` & `osmnx-1.5.1/osmnx/elevation.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     function. See also the `add_edge_grades` function.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     api_key : string
-        a valid API key, сan be None if the API does not require a key
+        a valid API key, can be None if the API does not require a key
     max_locations_per_batch : int
         max number of coordinate pairs to submit in each API call (if this is
         too high, the server will reject the request because its character
         limit exceeds the max allowed)
     pause_duration : float
         time to pause between API calls, which can be increased if you get
         rate limited
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osmnx-1.5.0/osmnx/features.py` & `osmnx-1.5.1/osmnx/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     south : float
         southern latitude of bounding box
     east : float
         eastern longitude of bounding box
     west : float
         western longitude of bounding box
     tags : dict
-        Dict of tags used for finding objects in the selected area. Results
+        Dict of tags used for finding elements in the selected area. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
@@ -132,15 +132,15 @@
     For more details, see: https://wiki.openstreetmap.org/wiki/Map_features
 
     Parameters
     ----------
     center_point : tuple
         the (lat, lng) center point around which to get the features
     tags : dict
-        Dict of tags used for finding objects in the selected area. Results
+        Dict of tags used for finding elements in the selected area. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
@@ -178,15 +178,15 @@
 
     Parameters
     ----------
     address : string
         the address to geocode and use as the central point around which to
         get the features
     tags : dict
-        Dict of tags used for finding objects in the selected area. Results
+        Dict of tags used for finding elements in the selected area. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
@@ -233,15 +233,15 @@
     For more details, see: https://wiki.openstreetmap.org/wiki/Map_features
 
     Parameters
     ----------
     query : string or dict or list
         the query or queries to geocode to get place boundary polygon(s)
     tags : dict
-        Dict of tags used for finding objects in the selected area. Results
+        Dict of tags used for finding elements in the selected area. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
@@ -292,15 +292,15 @@
     For more details, see: https://wiki.openstreetmap.org/wiki/Map_features
 
     Parameters
     ----------
     polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
         geographic boundaries to fetch features within
     tags : dict
-        Dict of tags used for finding objects in the selected area. Results
+        Dict of tags used for finding elements in the selected area. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
@@ -346,17 +346,17 @@
     For more details, see: https://wiki.openstreetmap.org/wiki/Map_features
 
     Parameters
     ----------
     filepath : string or pathlib.Path
         path to file containing OSM XML data
     polygon : shapely.geometry.Polygon
-        optional geographic boundary to filter objects
+        optional geographic boundary to filter elements
     tags : dict
-        optional dict of tags for filtering objects from the XML. Results
+        optional dict of tags for filtering elements from the XML. Results
         returned are the union, not intersection of each individual tag.
         Each result matches at least one given tag. The dict keys should be
         OSM tags, (e.g., `building`, `landuse`, `highway`, etc) and the dict
         values should be either `True` to retrieve all items with the given
         tag, or a string to get a single tag-value combination, or a list of
         strings to get multiple values for the given tag. For example,
         `tags = {'building': True}` would return all building footprints in
```

### Comparing `osmnx-1.5.0/osmnx/folium.py` & `osmnx-1.5.1/osmnx/folium.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/geocoder.py` & `osmnx-1.5.1/osmnx/geocoder.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/geometries.py` & `osmnx-1.5.1/osmnx/geometries.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/graph.py` & `osmnx-1.5.1/osmnx/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from . import settings
 from . import simplification
 from . import stats
 from . import truncate
 from . import utils
 from . import utils_geo
 from . import utils_graph
+from ._errors import CacheOnlyModeInterrupt
 from ._errors import EmptyOverpassResponse
 from ._version import __version__
 
 
 def graph_from_bbox(
     north,
     south,
@@ -91,15 +92,15 @@
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
         clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
 
-    utils.log(f"graph_from_bbox returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_bbox returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def graph_from_point(
     center_point,
     dist=1000,
     dist_type="bbox",
@@ -179,15 +180,15 @@
 
     if dist_type == "network":
         # if dist_type is network, find node in graph nearest to center point
         # then truncate graph by network dist from it
         node = distance.nearest_nodes(G, X=[center_point[1]], Y=[center_point[0]])[0]
         G = truncate.truncate_graph_dist(G, node, max_dist=dist)
 
-    utils.log(f"graph_from_point returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_point returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def graph_from_address(
     address,
     dist=1000,
     dist_type="bbox",
@@ -260,15 +261,15 @@
         network_type=network_type,
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
         clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
-    utils.log(f"graph_from_address returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_address returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
 
     if return_coords:
         return G, point
     else:
         return G
 
 
@@ -364,15 +365,15 @@
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
         clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
 
-    utils.log(f"graph_from_place returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_place returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def graph_from_polygon(
     polygon,
     network_type="all_private",
     simplify=True,
@@ -496,22 +497,27 @@
         nx.set_node_attributes(G, values=spn, name="street_count")
         warn(
             "the graph-level street_count attribute will likely be inaccurate "
             "when you set clean_periphery=False",
             stacklevel=2,
         )
 
-    utils.log(f"graph_from_polygon returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_polygon returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def graph_from_xml(filepath, bidirectional=False, simplify=True, retain_all=False):
     """
     Create a graph from data in a .osm formatted XML file.
 
+    Do not load an XML file generated by OSMnx: this use case is not supported
+    and may not behave as expected. To save/load graphs to/from disk for later
+    use in OSMnx, use the `io.save_graphml` and `io.load_graphml` functions
+    instead.
+
     Parameters
     ----------
     filepath : string or pathlib.Path
         path to file containing OSM XML data
     bidirectional : bool
         if True, create bi-directional edges for one-way streets
     simplify : bool
@@ -530,75 +536,85 @@
     # create graph using this response JSON
     G = _create_graph(response_jsons, bidirectional=bidirectional, retain_all=retain_all)
 
     # simplify the graph topology as the last step
     if simplify:
         G = simplification.simplify_graph(G)
 
-    utils.log(f"graph_from_xml returned graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"graph_from_xml returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def _create_graph(response_jsons, retain_all=False, bidirectional=False):
     """
     Create a networkx MultiDiGraph from Overpass API responses.
 
     Adds length attributes in meters (great-circle distance between endpoints)
     to all of the graph's (pre-simplified, straight-line) edges via the
     `distance.add_edge_lengths` function.
 
     Parameters
     ----------
-    response_jsons : list
-        list of dicts of JSON responses from from the Overpass API
+    response_jsons : iterable
+        iterable of dicts of JSON responses from from the Overpass API
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     bidirectional : bool
         if True, create bi-directional edges for one-way streets
 
     Returns
     -------
     G : networkx.MultiDiGraph
     """
-    utils.log("Creating graph from downloaded OSM data...")
+    response_count = 0
+    nodes = {}
+    paths = {}
 
-    # make sure we got data back from the server request(s)
-    if not any(rj["elements"] for rj in response_jsons):  # pragma: no cover
-        msg = "There are no data elements in the server response. Check log and query location/filters."
-        raise EmptyOverpassResponse(msg)
+    # consume response_jsons generator to download data from server
+    for response_json in response_jsons:
+        response_count += 1
+        if settings.cache_only_mode:  # pragma: no cover
+            # if cache_only_mode, consume response_jsons then continue loop
+            continue
+        else:
+            # otherwise, extract nodes and paths from the downloaded OSM data
+            nodes_temp, paths_temp = _parse_nodes_paths(response_json)
+            nodes.update(nodes_temp)
+            paths.update(paths_temp)
+
+    utils.log(f"Retrieved all data from API in {response_count} request(s)")
+    if settings.cache_only_mode:  # pragma: no cover
+        # after consuming all response_jsons in loop, raise exception to catch
+        raise CacheOnlyModeInterrupt("Interrupted because `settings.cache_only_mode=True`")
+
+    # ensure we got some node/way data back from the server request(s)
+    if (len(nodes) == 0) and (len(paths) == 0):  # pragma: no cover
+        raise EmptyOverpassResponse(
+            "No data elements in server response. Check query location/filters and log."
+        )
 
-    # create the graph as a MultiDiGraph and set its meta-attributes
+    # create the MultiDiGraph and set its graph-level attributes
     metadata = {
         "created_date": utils.ts(),
         "created_with": f"OSMnx {__version__}",
         "crs": settings.default_crs,
     }
     G = nx.MultiDiGraph(**metadata)
 
-    # extract nodes and paths from the downloaded osm data
-    nodes = {}
-    paths = {}
-    for response_json in response_jsons:
-        nodes_temp, paths_temp = _parse_nodes_paths(response_json)
-        nodes.update(nodes_temp)
-        paths.update(paths_temp)
-
-    # add each osm node to the graph
-    for node, data in nodes.items():
-        G.add_node(node, **data)
-
-    # add each osm way (ie, a path of edges) to the graph
+    # add each OSM node and way (a path of edges) to the graph
+    utils.log(f"Creating graph from {len(nodes):,} OSM nodes and {len(paths):,} OSM ways...")
+    G.add_nodes_from(nodes.items())
     _add_paths(G, paths.values(), bidirectional)
 
-    # retain only the largest connected component if retain_all is False
+    # retain only the largest connected component if retain_all=False
     if not retain_all:
         G = utils_graph.get_largest_component(G)
 
-    utils.log(f"Created graph with {len(G)} nodes and {len(G.edges)} edges")
+    utils.log(f"Created graph with {len(G):,} nodes and {len(G.edges):,} edges")
 
     # add length (great-circle distance between nodes) attribute to each edge
     if len(G.edges) > 0:
         G = distance.add_edge_lengths(G)
 
     return G
```

### Comparing `osmnx-1.5.0/osmnx/io.py` & `osmnx-1.5.1/osmnx/io.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/osm_xml.py` & `osmnx-1.5.1/osmnx/osm_xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Read/write .osm formatted XML files."""
 import bz2
 import xml.sax
 from pathlib import Path
 from warnings import warn
-from xml.etree import ElementTree as etree
+from xml.etree import ElementTree as ET
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from . import settings
 from . import utils
 from . import utils_graph
+from ._version import __version__
 
 
 class _OSMContentHandler(xml.sax.handler.ContentHandler):
     """
     SAX content handler for OSM XML.
 
     Used to build an Overpass-like response JSON object in self.object. For
-    format notes, see https://overpass-api.de/ and
-    https://wiki.openstreetmap.org/wiki/OSM_XML#OSM_XML_file_format_notes
+    format notes, see https://wiki.openstreetmap.org/wiki/OSM_XML and
+    https://overpass-api.de
     """
 
     def __init__(self):
         self._element = None
         self.object = {"elements": []}
 
     def startElement(self, name, attrs):
@@ -70,21 +71,35 @@
         path to file containing OSM XML data
 
     Returns
     -------
     OSMContentHandler object
     """
 
+    # open the XML file, handling bz2 or regular XML
     def _opener(filepath):
         if filepath.suffix == ".bz2":
             return bz2.BZ2File(filepath)
         else:
-            # assume an unrecognized file extension is just XML
-            return filepath.open(mode="rb")
+            return filepath.open()
 
+    # warn if this XML file was generated by OSMnx itself
+    with _opener(Path(filepath)) as f:
+        root_attrs = ET.parse(f).getroot().attrib
+        if "generator" in root_attrs and "OSMnx" in root_attrs["generator"]:
+            warn(
+                "The XML file you are loading appears to have been generated "
+                "by OSMnx: this use case is not supported and may not behave "
+                "as expected. To save/load graphs to/from disk for later use "
+                "in OSMnx, use the `io.save_graphml` and `io.load_graphml` "
+                "functions instead. Refer to the documentation for details.",
+                stacklevel=2,
+            )
+
+    # parse the XML to Overpass-like JSON
     with _opener(Path(filepath)) as f:
         handler = _OSMContentHandler()
         xml.sax.parse(f, handler)
         return handler.object
 
 
 def save_graph_xml(
@@ -99,14 +114,18 @@
     edge_tag_aggs=None,
     api_version=0.6,
     precision=6,
 ):
     """
     Do not use: deprecated.
 
+    The `save_graph_xml` has moved from the `osm_xml` module to the `io`
+    module. `osm_xml.save_graph_xml` has been deprecated and will be removed
+    in a future release. Access the function via the `io` module instead.
+
     Parameters
     ----------
     data : networkx.multidigraph
         do not use, deprecated
     filepath : string or pathlib.Path
         do not use, deprecated
     node_tags : list
@@ -258,22 +277,24 @@
         gdf_edges.loc[pd.isnull(gdf_edges["oneway"]), "oneway"] = oneway
         gdf_edges.loc[:, "oneway"] = gdf_edges["oneway"].astype(str)
         gdf_edges.loc[:, "oneway"] = (
             gdf_edges["oneway"].str.replace("False", "no").replace("True", "yes")
         )
 
     # initialize XML tree with an OSM root element then append nodes/edges
-    root = etree.Element("osm", attrib={"version": str(api_version), "generator": "OSMnx"})
+    root = ET.Element(
+        "osm", attrib={"version": str(api_version), "generator": f"OSMnx {__version__}"}
+    )
     root = _append_nodes_xml_tree(root, gdf_nodes, node_attrs, node_tags)
     root = _append_edges_xml_tree(
         root, gdf_edges, edge_attrs, edge_tags, edge_tag_aggs, merge_edges
     )
 
     # write to disk
-    etree.ElementTree(root).write(filepath, encoding="utf-8", xml_declaration=True)
+    ET.ElementTree(root).write(filepath, encoding="utf-8", xml_declaration=True)
     utils.log(f"Saved graph as .osm file at {filepath!r}")
 
 
 def _append_nodes_xml_tree(root, gdf_nodes, node_attrs, node_tags):
     """
     Append nodes to an XML tree.
 
@@ -291,19 +312,19 @@
     Returns
     -------
     root : ElementTree.Element
         xml tree with nodes appended
     """
     for _, row in gdf_nodes.iterrows():
         row = row.dropna().astype(str)
-        node = etree.SubElement(root, "node", attrib=row[node_attrs].to_dict())
+        node = ET.SubElement(root, "node", attrib=row[node_attrs].to_dict())
 
         for tag in node_tags:
             if tag in row:
-                etree.SubElement(node, "tag", attrib={"k": tag, "v": row[tag]})
+                ET.SubElement(node, "tag", attrib={"k": tag, "v": row[tag]})
     return root
 
 
 def _create_way_for_each_edge(root, gdf_edges, edge_attrs, edge_tags):
     """
     Append a new way to an empty XML tree graph for each edge in way.
 
@@ -322,20 +343,20 @@
     edge_attrs : list
         osm way attributes to include in output OSM XML
     edge_tags : list
         osm way tags to include in output OSM XML
     """
     for _, row in gdf_edges.iterrows():
         row = row.dropna().astype(str)
-        edge = etree.SubElement(root, "way", attrib=row[edge_attrs].to_dict())
-        etree.SubElement(edge, "nd", attrib={"ref": row["u"]})
-        etree.SubElement(edge, "nd", attrib={"ref": row["v"]})
+        edge = ET.SubElement(root, "way", attrib=row[edge_attrs].to_dict())
+        ET.SubElement(edge, "nd", attrib={"ref": row["u"]})
+        ET.SubElement(edge, "nd", attrib={"ref": row["v"]})
         for tag in edge_tags:
             if tag in row:
-                etree.SubElement(edge, "tag", attrib={"k": tag, "v": row[tag]})
+                ET.SubElement(edge, "tag", attrib={"k": tag, "v": row[tag]})
     return
 
 
 def _append_merged_edge_attrs(xml_edge, sample_edge, all_edges_df, edge_tags, edge_tag_aggs):
     """
     Extract edge attributes and append to XML edge.
 
@@ -359,23 +380,23 @@
         component edges. Otherwise, the length attribute will simply reflect
         the length of the first edge associated with the way.
 
     """
     if edge_tag_aggs is None:
         for tag in edge_tags:
             if tag in sample_edge:
-                etree.SubElement(xml_edge, "tag", attrib={"k": tag, "v": sample_edge[tag]})
+                ET.SubElement(xml_edge, "tag", attrib={"k": tag, "v": sample_edge[tag]})
     else:
         for tag in edge_tags:
             if (tag in sample_edge) and (tag not in (t for t, agg in edge_tag_aggs)):
-                etree.SubElement(xml_edge, "tag", attrib={"k": tag, "v": sample_edge[tag]})
+                ET.SubElement(xml_edge, "tag", attrib={"k": tag, "v": sample_edge[tag]})
 
         for tag, agg in edge_tag_aggs:
             if tag in all_edges_df.columns:
-                etree.SubElement(
+                ET.SubElement(
                     xml_edge,
                     "tag",
                     attrib={
                         "k": tag,
                         "v": str(all_edges_df[tag].aggregate(agg)),
                     },
                 )
@@ -392,26 +413,26 @@
         XML representation of an output graph edge
     sample_edge: pandas.Series
         sample row from the the dataframe of way edges
     all_edges_df: pandas.DataFrame
         a dataframe with one row for each edge in an OSM way
     """
     if len(all_edges_df) == 1:
-        etree.SubElement(xml_edge, "nd", attrib={"ref": sample_edge["u"]})
-        etree.SubElement(xml_edge, "nd", attrib={"ref": sample_edge["v"]})
+        ET.SubElement(xml_edge, "nd", attrib={"ref": sample_edge["u"]})
+        ET.SubElement(xml_edge, "nd", attrib={"ref": sample_edge["v"]})
     else:
         # topological sort
         try:
             ordered_nodes = _get_unique_nodes_ordered_from_way(all_edges_df)
         except nx.NetworkXUnfeasible:
             first_node = all_edges_df.iloc[0]["u"]
             ordered_nodes = _get_unique_nodes_ordered_from_way(all_edges_df.iloc[1:])
             ordered_nodes = [first_node] + ordered_nodes
         for node in ordered_nodes:
-            etree.SubElement(xml_edge, "nd", attrib={"ref": str(node)})
+            ET.SubElement(xml_edge, "nd", attrib={"ref": str(node)})
     return
 
 
 def _append_edges_xml_tree(root, gdf_edges, edge_attrs, edge_tags, edge_tag_aggs, merge_edges):
     """
     Append edges to an XML tree.
 
@@ -445,15 +466,15 @@
     root : ElementTree.Element
         XML tree with edges appended
     """
     gdf_edges.reset_index(inplace=True)
     if merge_edges:
         for _, all_way_edges in gdf_edges.groupby("id"):
             first = all_way_edges.iloc[0].dropna().astype(str)
-            edge = etree.SubElement(root, "way", attrib=first[edge_attrs].dropna().to_dict())
+            edge = ET.SubElement(root, "way", attrib=first[edge_attrs].dropna().to_dict())
             _append_nodes_as_edge_attrs(
                 xml_edge=edge, sample_edge=first, all_edges_df=all_way_edges
             )
             _append_merged_edge_attrs(
                 xml_edge=edge,
                 sample_edge=first,
                 edge_tags=edge_tags,
```

### Comparing `osmnx-1.5.0/osmnx/plot.py` & `osmnx-1.5.1/osmnx/plot.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/projection.py` & `osmnx-1.5.1/osmnx/projection.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,44 +12,45 @@
     """
     Determine if a coordinate reference system is projected or not.
 
     Parameters
     ----------
     crs : string or pyproj.CRS
         the identifier of the coordinate reference system, which can be
-        anything accepted by pyproj.CRS.from_user_input() such as an authority
-        string or a WKT string
+        anything accepted by `pyproj.CRS.from_user_input()` such as an
+        authority string or a WKT string
 
     Returns
     -------
     projected : bool
         True if crs is projected, otherwise False
     """
     return gpd.GeoSeries(crs=crs).crs.is_projected
 
 
 def project_geometry(geometry, crs=None, to_crs=None, to_latlong=False):
     """
-    Project a shapely geometry from its current CRS to another.
+    Reproject a shapely geometry from its current CRS to another.
 
-    If to_crs is None, project to the UTM CRS for the UTM zone in which the
-    geometry's centroid lies. Otherwise project to the CRS defined by to_crs.
+    If `to_crs` is None, project to the UTM CRS for the UTM zone in which the
+    geometry's centroid lies. Otherwise project to the CRS defined by
+    `to_crs`.
 
     Parameters
     ----------
     geometry : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
         the geometry to project
     crs : string or pyproj.CRS
         the starting CRS of the passed-in geometry. if None, it will be set to
-        settings.default_crs
+        `settings.default_crs`
     to_crs : string or pyproj.CRS
-        if None, project to UTM zone in which geometry's centroid lies,
-        otherwise project to this CRS
+        if None, reproject to the UTM zone in which `geometry`'s centroid
+        lies, otherwise reproject to this CRS
     to_latlong : bool
-        if True, project to settings.default_crs and ignore to_crs
+        if True, reproject to `settings.default_crs` and ignore `to_crs`
 
     Returns
     -------
     geometry_proj, crs : tuple
         the projected geometry and its new CRS
     """
     if crs is None:
@@ -59,31 +60,31 @@
     gdf_proj = project_gdf(gdf, to_crs=to_crs, to_latlong=to_latlong)
     geometry_proj = gdf_proj["geometry"].iloc[0]
     return geometry_proj, gdf_proj.crs
 
 
 def project_gdf(gdf, to_crs=None, to_latlong=False):
     """
-    Project a GeoDataFrame from its current CRS to another.
+    Reroject a GeoDataFrame from its current CRS to another.
 
-    If to_crs is None, project to the UTM CRS for the UTM zone in which the
+    If `to_crs` is None, project to the UTM CRS for the UTM zone in which the
     GeoDataFrame's centroid lies. Otherwise project to the CRS defined by
-    to_crs. The simple UTM zone calculation in this function works well for
+    `to_crs`. The simple UTM zone calculation in this function works well for
     most latitudes, but may not work for some extreme northern locations like
     Svalbard or far northern Norway.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         the GeoDataFrame to be projected
     to_crs : string or pyproj.CRS
-        if None, project to UTM zone in which gdf's centroid lies, otherwise
+        if None, project to UTM zone in which `gdf`'s centroid lies, otherwise
         project to this CRS
     to_latlong : bool
-        if True, project to settings.default_crs and ignore to_crs
+        if True, project to `settings.default_crs` and ignore `to_crs`
 
     Returns
     -------
     gdf_proj : geopandas.GeoDataFrame
         the projected GeoDataFrame
     """
     if gdf.crs is None or len(gdf) < 1:  # pragma: no cover
@@ -116,19 +117,19 @@
         utils.log(f"Projected GeoDataFrame to {gdf_proj.crs}")
 
     return gdf_proj
 
 
 def project_graph(G, to_crs=None):
     """
-    Project graph from its current CRS to another.
+    Reproject a graph from its current CRS to another.
 
-    If to_crs is None, project the graph to the UTM CRS for the UTM zone in
+    If `to_crs` is None, project the graph to the UTM CRS for the UTM zone in
     which the graph's centroid lies. Otherwise, project the graph to the CRS
-    defined by to_crs.
+    defined by `to_crs`.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         the graph to be projected
     to_crs : string or pyproj.CRS
         if None, project graph to UTM zone in which graph centroid lies,
```

### Comparing `osmnx-1.5.0/osmnx/settings.py` & `osmnx-1.5.1/osmnx/settings.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/osmnx/simplification.py` & `osmnx-1.5.1/osmnx/simplification.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,18 +173,19 @@
     strict : bool
         if False, allow nodes to be end points even if they fail all other rules
         but have edges with different OSM IDs
 
     Yields
     ------
     path_to_simplify : list
+        a generator of paths to simplify
     """
     # first identify all the nodes that are endpoints
     endpoints = {n for n in G.nodes if _is_endpoint(G, n, strict=strict)}
-    utils.log(f"Identified {len(endpoints)} edge endpoints")
+    utils.log(f"Identified {len(endpoints):,} edge endpoints")
 
     # for each endpoint node, look at each of its successor nodes
     for endpoint in endpoints:
         for successor in G.successors(endpoint):
             if successor not in endpoints:
                 # if endpoint node's successor is not an endpoint, build path
                 # from the endpoint node, through the successor, and on to the
@@ -340,16 +341,16 @@
     if remove_rings:
         G = _remove_rings(G)
 
     # mark graph as having been simplified
     G.graph["simplified"] = True
 
     msg = (
-        f"Simplified graph: {initial_node_count} to {len(G)} nodes, "
-        f"{initial_edge_count} to {len(G.edges)} edges"
+        f"Simplified graph: {initial_node_count:,} to {len(G):,} nodes, "
+        f"{initial_edge_count:,} to {len(G.edges):,} edges"
     )
     utils.log(msg)
     return G
 
 
 def consolidate_intersections(
     G, tolerance=10, rebuild_graph=True, dead_ends=False, reconnect_edges=True
```

### Comparing `osmnx-1.5.0/osmnx/speed.py` & `osmnx-1.5.1/osmnx/speed.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,19 +112,17 @@
         edges[["highway", "speed_kph"]].set_index("highway").iloc[:, 0].fillna(hwy_speed_avg)
     )
 
     # all speeds will be null if edges had no preexisting maxspeed data and
     # caller did not pass in hwy_speeds or fallback arguments
     if pd.isnull(speed_kph).all():
         raise ValueError(
-            (
-                "this graph's edges have no preexisting `maxspeed` "
-                "attribute values so you must pass `hwy_speeds` or "
-                "`fallback` arguments."
-            )
+            "this graph's edges have no preexisting `maxspeed` "
+            "attribute values so you must pass `hwy_speeds` or "
+            "`fallback` arguments."
         )
 
     # add speed kph attribute to graph edges
     edges["speed_kph"] = speed_kph.round(precision).values
     nx.set_edge_attributes(G, values=edges["speed_kph"], name="speed_kph")
 
     return G
```

### Comparing `osmnx-1.5.0/osmnx/stats.py` & `osmnx-1.5.1/osmnx/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,26 +311,26 @@
     intersection measures are only calculated if `clean_int_tol` is provided.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     area : float
-        if not None, calculate density measures and use this area value (in
-        square meters) as the denominator
+        if not None, calculate density measures and use this value (in square
+        meters) as the denominator
     clean_int_tol : float
         if not None, calculate consolidated intersections count (and density,
         if `area` is also provided) and use this tolerance value; refer to the
         `simplification.consolidate_intersections` function documentation for
         details
 
     Returns
     -------
     stats : dict
-        dictionary containing the following attributes
+        dictionary containing the following keys
           - `circuity_avg` - see `circuity_avg` function documentation
           - `clean_intersection_count` - see `clean_intersection_count` function documentation
           - `clean_intersection_density_km` - `clean_intersection_count` per sq km
           - `edge_density_km` - `edge_length_total` per sq km
           - `edge_length_avg` - `edge_length_total / m`
           - `edge_length_total` - see `edge_length_total` function documentation
           - `intersection_count` - see `intersection_count` function documentation
```

### Comparing `osmnx-1.5.0/osmnx/truncate.py` & `osmnx-1.5.1/osmnx/truncate.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     else:
         nodes_to_remove = nodes_outside_poly
 
     # now remove from the graph all those nodes that lie outside the polygon
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
     G.remove_nodes_from(nodes_to_remove)
-    utils.log(f"Removed {len(nodes_to_remove)} nodes outside polygon")
+    utils.log(f"Removed {len(nodes_to_remove):,} nodes outside polygon")
 
     if not retain_all:
         # remove any isolated nodes and retain only the largest component
         G = utils_graph.remove_isolated_nodes(G)
         G = utils_graph.get_largest_component(G)
 
     utils.log("Truncated graph by polygon")
```

### Comparing `osmnx-1.5.0/osmnx/utils.py` & `osmnx-1.5.1/osmnx/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,65 +8,81 @@
 from contextlib import redirect_stdout
 from pathlib import Path
 from warnings import warn
 
 from . import settings
 
 
-def citation():
+def citation(style="bibtex"):
     """
     Print the OSMnx package's citation information.
 
-    Boeing, G. 2017. OSMnx: New Methods for Acquiring, Constructing, Analyzing,
-    and Visualizing Complex Street Networks. Computers, Environment and Urban
-    Systems, 65, 126-139. https://doi.org/10.1016/j.compenvurbsys.2017.05.004
+    Boeing, G. (2017). OSMnx: New Methods for Acquiring, Constructing,
+    Analyzing, and Visualizing Complex Street Networks. Computers, Environment
+    and Urban Systems, 65, 126-139.
+    https://doi.org/10.1016/j.compenvurbsys.2017.05.004
+
+    Parameters
+    ----------
+    style : string {"apa", "bibtex", "ieee"}
+        citation format, either APA or BibTeX or IEEE
 
     Returns
     -------
     None
     """
-    cite = (
-        "Citation:\n\n"
-        "Boeing, G. 2017. OSMnx: New Methods for Acquiring, "
-        "Constructing, Analyzing, and Visualizing Complex Street "
-        "Networks. Computers, Environment and Urban Systems, 65, 126-139. "
-        "https://doi.org/10.1016/j.compenvurbsys.2017.05.004\n\n"
-        "BibTeX entry for LaTeX users:\n\n"
-        "@article{boeing_osmnx_2017,\n"
-        "    title = {{OSMnx}: {New} {Methods} for {Acquiring}, "
-        "{Constructing}, {Analyzing}, and {Visualizing} {Complex} "
-        "{Street} {Networks}},\n"
-        "    volume = {65},\n"
-        "    doi = {10.1016/j.compenvurbsys.2017.05.004},\n"
-        "    number = {126-139},\n"
-        "    journal = {Computers, Environment and Urban Systems},\n"
-        "    author = {Boeing, Geoff},\n"
-        "    year = {2017}\n"
-        "}"
-    )
-
-    print(cite)
+    if style == "apa":
+        print(
+            "Boeing, G. (2017). OSMnx: New Methods for Acquiring, Constructing, "
+            "Analyzing, and Visualizing Complex Street Networks. Computers, "
+            "Environment and Urban Systems, 65, 126-139. "
+            "https://doi.org/10.1016/j.compenvurbsys.2017.05.004"
+        )
+    elif style == "bibtex":
+        print(
+            "@article{boeing_osmnx_2017,\n"
+            "    title = {{OSMnx}: {New} {Methods} for {Acquiring}, "
+            "{Constructing}, {Analyzing}, and {Visualizing} {Complex} "
+            "{Street} {Networks}},\n"
+            "    volume = {65},\n"
+            "    doi = {10.1016/j.compenvurbsys.2017.05.004},\n"
+            "    number = {126-139},\n"
+            "    journal = {Computers, Environment and Urban Systems},\n"
+            "    author = {Boeing, Geoff},\n"
+            "    year = {2017},\n"
+            "    pages = {126--139}\n"
+            "}"
+        )
+    elif style == "ieee":
+        print(
+            'G. Boeing, "OSMnx: New Methods for Acquiring, Constructing, '
+            'Analyzing, and Visualizing Complex Street Networks," Computers, '
+            "Environment and Urban Systems, vol. 65, pp. 126-139, 2017, "
+            "doi: 10.1016/j.compenvurbsys.2017.05.004."
+        )
+    else:  # pragma: no cover
+        raise ValueError(f"unrecognized citation style {style!r}")
 
 
 def ts(style="datetime", template=None):
     """
-    Get current timestamp as string.
+    Return current timestamp as a string.
 
     Parameters
     ----------
     style : string {"datetime", "date", "time"}
-        format the timestamp with this built-in template
+        format the timestamp with this built-in style
     template : string
-        if not None, format the timestamp with this template instead of one of
-        the built-in styles
+        if not None, format the timestamp with this format string instead of
+        one of the built-in styles
 
     Returns
     -------
     ts : string
-        the string timestamp
+        timestamp string
     """
     if template is None:
         if style == "datetime":
             template = "{:%Y-%m-%d %H:%M:%S}"
         elif style == "date":
             template = "{:%Y-%m-%d}"
         elif style == "time":
```

### Comparing `osmnx-1.5.0/osmnx/utils_geo.py` & `osmnx-1.5.1/osmnx/utils_geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         a LineString geometry
     dist : float
         spacing distance between interpolated points, in same units as `geom`.
         smaller values generate more points.
 
     Yields
     ------
-    points : generator
+    point : tuple of floats
         a generator of (x, y) tuples of the interpolated points' coordinates
     """
     if isinstance(geom, LineString):
         num_vert = max(round(geom.length / dist), 1)
         for n in range(num_vert + 1):
             point = geom.interpolate(n / num_vert, normalized=True)
             yield point.x, point.y
@@ -395,15 +395,15 @@
     Returns
     -------
     geoms_in_poly : set
         index labels of geometries that intersected polygon
     """
     # create an r-tree spatial index for the geometries
     sindex = geometries.sindex
-    utils.log(f"Created r-tree spatial index for {len(geometries)} geometries")
+    utils.log(f"Created r-tree spatial index for {len(geometries):,} geometries")
 
     # cut the polygon into chunks for spatial index intersecting
     multipoly = _quadrat_cut_geometry(polygon, quadrat_width=quadrat_width, min_num=min_num)
     geoms_in_poly = set()
 
     # loop through each chunk of the polygon to find intersecting geometries
     for poly in multipoly.geoms:
@@ -412,15 +412,15 @@
         poly = poly.buffer(0)
         if poly.is_valid and poly.area > 0:
             possible_matches_iloc = sindex.intersection(poly.bounds)
             possible_matches = geometries.iloc[list(possible_matches_iloc)]
             precise_matches = possible_matches[possible_matches.intersects(poly)]
             geoms_in_poly.update(precise_matches.index)
 
-    utils.log(f"Identified {len(geoms_in_poly)} geometries inside polygon")
+    utils.log(f"Identified {len(geoms_in_poly):,} geometries inside polygon")
     return geoms_in_poly
 
 
 def bbox_from_point(point, dist=1000, project_utm=False, return_crs=False):
     """
     Create a bounding box from a (lat, lng) center point.
```

### Comparing `osmnx-1.5.0/osmnx/utils_graph.py` & `osmnx-1.5.1/osmnx/utils_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
     """
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
 
     # get the set of all isolated nodes, then remove them
     isolated_nodes = {node for node, degree in G.degree() if degree < 1}
     G.remove_nodes_from(isolated_nodes)
-    utils.log(f"Removed {len(isolated_nodes)} isolated nodes")
+    utils.log(f"Removed {len(isolated_nodes):,} isolated nodes")
     return G
 
 
 def get_largest_component(G, strongly=False):
     """
     Get subgraph of G's largest weakly/strongly connected component.
 
@@ -299,15 +299,15 @@
     if not is_connected(G):
         # get all the connected components in graph then identify the largest
         largest_cc = max(connected_components(G), key=len)
         n = len(G)
 
         # induce (frozen) subgraph then unfreeze it by making new MultiDiGraph
         G = nx.MultiDiGraph(G.subgraph(largest_cc))
-        utils.log(f"Got largest {kind} connected component ({len(G)} of {n} total nodes)")
+        utils.log(f"Got largest {kind} connected component ({len(G):,} of {n:,} total nodes)")
 
     return G
 
 
 def get_digraph(G, weight="length"):
     """
     Convert MultiDiGraph to DiGraph.
```

### Comparing `osmnx-1.5.0/.gitignore` & `osmnx-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/LICENSE.txt` & `osmnx-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.5.0/README.md` & `osmnx-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 ## Citation
 
 If you use OSMnx in your work, please cite the journal article:
 
 Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." *Computers, Environment and Urban Systems* 65, 126–139.
 
-## Installation
+## Getting Started
 
-Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
+Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
 
-## Getting Started
+## Installation
 
-Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide and work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
 
 If you have any trouble, consult the [User Reference](https://osmnx.readthedocs.io/en/stable/user-reference.html). The OSMnx repository is hosted on [GitHub](https://github.com/gboeing/osmnx). If you have a "how-to" or usage question, please ask it on [StackOverflow](https://stackoverflow.com/search?q=osmnx), as we reserve the repository's issue tracker for bug tracking and feature development.
 
 ## License
```

### Comparing `osmnx-1.5.0/pyproject.toml` & `osmnx-1.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 authors = [{name = "Geoff Boeing", email = "boeing@usc.edu"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
@@ -34,26 +35,29 @@
 dynamic = ["version"]
 keywords = ["GIS", "Networks", "OpenStreetMap", "Routing"]
 license = {text = "MIT License"}
 maintainers = [{name = "OSMnx contributors"}]
 name = "osmnx"
 readme = "README.md"
 requires-python = ">=3.8"
-urls.Documentation = "https://osmnx.readthedocs.io/"
+urls.Documentation = "https://osmnx.readthedocs.io"
 urls.Repository = "https://github.com/gboeing/osmnx"
 
 [project.optional-dependencies]
 entropy = ["scipy>=1.5"]
 neighbors = ["scikit-learn>=0.23", "scipy>=1.5"]
 raster = ["gdal", "rasterio>=1.3"]
 visualization = ["matplotlib>=3.5"]
 
 [tool.black]
 line_length = 100
 
+[tool.hatch.build]
+packages = ["osmnx"]
+
 [tool.hatch.version]
 path = "osmnx/_version.py"
 
 [tool.ruff]
 cache-dir = "~/.cache/ruff"
 exclude = ["build/*"]
 ignore = ["E501"]
```

### Comparing `osmnx-1.5.0/PKG-INFO` & `osmnx-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.5.0
+Version: 1.5.1
 Summary: Download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap
-Project-URL: Documentation, https://osmnx.readthedocs.io/
+Project-URL: Documentation, https://osmnx.readthedocs.io
 Project-URL: Repository, https://github.com/gboeing/osmnx
 Author-email: Geoff Boeing <boeing@usc.edu>
 Maintainer: OSMnx contributors
 License: MIT License
 License-File: LICENSE.txt
 Keywords: GIS,Networks,OpenStreetMap,Routing
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -57,21 +58,21 @@
 
 ## Citation
 
 If you use OSMnx in your work, please cite the journal article:
 
 Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." *Computers, Environment and Urban Systems* 65, 126–139.
 
-## Installation
+## Getting Started
 
-Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
+Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package, then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
 
-## Getting Started
+## Installation
 
-Read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide and work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
 
 If you have any trouble, consult the [User Reference](https://osmnx.readthedocs.io/en/stable/user-reference.html). The OSMnx repository is hosted on [GitHub](https://github.com/gboeing/osmnx). If you have a "how-to" or usage question, please ask it on [StackOverflow](https://stackoverflow.com/search?q=osmnx), as we reserve the repository's issue tracker for bug tracking and feature development.
 
 ## License
```

