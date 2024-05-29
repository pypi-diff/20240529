# Comparing `tmp/mapbox_vector_tile-2.0.1.tar.gz` & `tmp/mapbox_vector_tile-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbox_vector_tile-2.0.1.tar", max compression
+gzip compressed data, was "mapbox_vector_tile-2.1.0.tar", max compression
```

## Comparing `mapbox_vector_tile-2.0.1.tar` & `mapbox_vector_tile-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5310 2023-01-22 18:51:35.823995 mapbox_vector_tile-2.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2022-12-21 03:25:51.181735 mapbox_vector_tile-2.0.1/LICENSE
--rw-r--r--   0        0        0    15725 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.0.1/README.md
--rw-r--r--   0        0        0        0 2022-12-15 02:50:18.507609 mapbox_vector_tile-2.0.1/mapbox_vector_tile/Mapbox/__init__.py
--rw-r--r--   0        0        0     3793 2022-12-21 03:25:51.185735 mapbox_vector_tile-2.0.1/mapbox_vector_tile/Mapbox/vector_tile.proto
--rw-r--r--   0        0        0     2708 2022-12-21 03:25:51.185735 mapbox_vector_tile-2.0.1/mapbox_vector_tile/Mapbox/vector_tile_pb2.py
--rw-r--r--   0        0        0     5056 2023-01-22 18:49:56.734314 mapbox_vector_tile-2.0.1/mapbox_vector_tile/__init__.py
--rw-r--r--   0        0        0     6798 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.0.1/mapbox_vector_tile/decoder.py
--rw-r--r--   0        0        0    10285 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.0.1/mapbox_vector_tile/encoder.py
--rw-r--r--   0        0        0     4419 2023-01-03 01:05:53.548899 mapbox_vector_tile-2.0.1/mapbox_vector_tile/geom_encoder.py
--rw-r--r--   0        0        0     7666 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.0.1/mapbox_vector_tile/optimise.py
--rw-r--r--   0        0        0     8101 2022-12-22 14:44:59.164612 mapbox_vector_tile-2.0.1/mapbox_vector_tile/polygon.py
--rw-r--r--   0        0        0     4110 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.0.1/mapbox_vector_tile/utils.py
--rw-r--r--   0        0        0     1420 2023-01-16 03:53:33.412062 mapbox_vector_tile-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    17471 1970-01-01 00:00:00.000000 mapbox_vector_tile-2.0.1/setup.py
--rw-r--r--   0        0        0    16804 1970-01-01 00:00:00.000000 mapbox_vector_tile-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5452 2024-05-29 00:47:38.398125 mapbox_vector_tile-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2022-12-21 03:25:51.181735 mapbox_vector_tile-2.1.0/LICENSE
+-rw-r--r--   0        0        0    15637 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-15 02:50:18.507609 mapbox_vector_tile-2.1.0/mapbox_vector_tile/Mapbox/__init__.py
+-rw-r--r--   0        0        0     3793 2022-12-21 03:25:51.185735 mapbox_vector_tile-2.1.0/mapbox_vector_tile/Mapbox/vector_tile.proto
+-rw-r--r--   0        0        0     2708 2022-12-21 03:25:51.185735 mapbox_vector_tile-2.1.0/mapbox_vector_tile/Mapbox/vector_tile_pb2.py
+-rw-r--r--   0        0        0     5080 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/mapbox_vector_tile/__init__.py
+-rw-r--r--   0        0        0     6732 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/mapbox_vector_tile/decoder.py
+-rw-r--r--   0        0        0    10145 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/mapbox_vector_tile/encoder.py
+-rw-r--r--   0        0        0     4419 2023-01-03 01:05:53.548899 mapbox_vector_tile-2.1.0/mapbox_vector_tile/geom_encoder.py
+-rw-r--r--   0        0        0     7657 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/mapbox_vector_tile/optimise.py
+-rw-r--r--   0        0        0     8013 2024-05-29 00:31:48.783906 mapbox_vector_tile-2.1.0/mapbox_vector_tile/polygon.py
+-rw-r--r--   0        0        0     4110 2023-01-16 03:00:57.095856 mapbox_vector_tile-2.1.0/mapbox_vector_tile/utils.py
+-rw-r--r--   0        0        0     1627 2024-05-29 00:47:38.398125 mapbox_vector_tile-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17379 1970-01-01 00:00:00.000000 mapbox_vector_tile-2.1.0/setup.py
+-rw-r--r--   0        0        0    16671 1970-01-01 00:00:00.000000 mapbox_vector_tile-2.1.0/PKG-INFO
```

### Comparing `mapbox_vector_tile-2.0.1/CHANGELOG.md` & `mapbox_vector_tile-2.1.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,167 +1,151 @@
-Version 2.0.1
--------------
+## Version 2.1.0
 
-* Support previous pre 2.0 encode/decode method signatures with deprecation warning.
+- Drop the support for Python 3.8 and add the support for Python 3.12
+- Update the minimum required version for `protobuf`
+- Replace Isort, Flake8 and Black by Ruff in the `.pre-commit-config.yaml` file
+- Use `prettier` pre-commit tool to prettify Markdown and Yaml files
+- Use `poetry-check` pre-commit tool to avoid incompatibilities between `poetry.lock` and `pyproject.toml`
+
+## Version 2.0.1
+
+- Support previous pre 2.0 encode/decode method signatures with deprecation warning.
   [#129](https://github.com/tilezen/mapbox-vector-tile/pull/129)
 
-Version 2.0.0
--------------
+## Version 2.0.0
 
-* Drop Python 2 support
-* Usage of `tox` for tests
-* Add GitHub Actions
-* Add pre-commit tool
-* Regenerate the vector tile protobuf Python code to solve
+- Drop Python 2 support
+- Usage of `tox` for tests
+- Add GitHub Actions
+- Add pre-commit tool
+- Regenerate the vector tile protobuf Python code to solve
   [#113](https://github.com/tilezen/mapbox-vector-tile/issues/113)
-* Support for Python 3.11
-* Delete the `round_fn` argument as Python 2 has been dropped
-* Use `pyproject.toml` and Poetry to replace the `setup.py` file
-* Use `geom_type` property instead of deprecated `type`
-* Add the possibility to give a coordinates transformer
-* Add a `geojson` option. See [#107](https://github.com/tilezen/mapbox-vector-tile/issues/107)
-* Refactor the options using the `per_layer_options` and `default_options` dictionaries.
-* Add the option `max_geometry_validate_tries`.
-
+- Support for Python 3.11
+- Delete the `round_fn` argument as Python 2 has been dropped
+- Use `pyproject.toml` and Poetry to replace the `setup.py` file
+- Use `geom_type` property instead of deprecated `type`
+- Add the possibility to give a coordinates transformer
+- Add a `geojson` option. See [#107](https://github.com/tilezen/mapbox-vector-tile/issues/107)
+- Refactor the options using the `per_layer_options` and `default_options` dictionaries.
+- Add the option `max_geometry_validate_tries`.
 
-Version 1.2.1
--------------
+## Version 1.2.1
 
-* Add the trove classifiers to the setup.py
+- Add the trove classifiers to the setup.py
 
-Version 1.2.0
--------------
+## Version 1.2.0
 
-* Performance focused release, including:
-* Enable Shapely speedups, when available
-* Skip inners which cause exceptions
-* Union inners in blocks when making valid
-* Make benchmark script python3 compatible
-* Fix test to support different versions of GEOS
+- Performance focused release, including:
+- Enable Shapely speedups, when available
+- Skip inners which cause exceptions
+- Union inners in blocks when making valid
+- Make benchmark script python3 compatible
+- Fix test to support different versions of GEOS
 
-Version 1.1.0
--------------
+## Version 1.1.0
 
-* Include LICENSE & CHANGELOG.md in sdist tarballs
-* Refactor geometry encoding logic, including skipping tiny geometries
-* Decoded geometry is now geojson-ish dict
-* Winding order is now optional
-* Add benchmarking around round function and document how to improve performance
-* Document performance tip for protobuf encoding with C bindings for Debian
+- Include LICENSE & CHANGELOG.md in sdist tarballs
+- Refactor geometry encoding logic, including skipping tiny geometries
+- Decoded geometry is now geojson-ish dict
+- Winding order is now optional
+- Add benchmarking around round function and document how to improve performance
+- Document performance tip for protobuf encoding with C bindings for Debian
 
-Version 1.0.0
--------------
+## Version 1.0.0
 
-* Generate more valid polygons and multipolygons using [pyclipper](https://pypi.python.org/pypi/pyclipper) library for v2 MVT compliance (but we're still not fully v2 compliant for [other](https://github.com/tilezen/mapbox-vector-tile/issues/42) reasons).
-* Handle edge cases where polygon buffer makes a multi-polygon, ensuring inner rings are dropped when subtracting them from the polygon would make it invalid, and not adding multipolygons as array elements for multipolygon constructor.
-* Calculate area more properly by using PolyTree result from Clipper.
-* Factor out polygon validity code into its own file.
+- Generate more valid polygons and multipolygons using [pyclipper](https://pypi.python.org/pypi/pyclipper) library for v2 MVT compliance (but we're still not fully v2 compliant for [other](https://github.com/tilezen/mapbox-vector-tile/issues/42) reasons).
+- Handle edge cases where polygon buffer makes a multi-polygon, ensuring inner rings are dropped when subtracting them from the polygon would make it invalid, and not adding multipolygons as array elements for multipolygon constructor.
+- Calculate area more properly by using PolyTree result from Clipper.
+- Factor out polygon validity code into its own file.
 
-Version 0.5.0
--------------
+## Version 0.5.0
 
-* Improved results from `on_invalid_geometry_make_valid` when the geometry is self-crossing. It was possible for large parts of the geometry to be discarded, and it is now less likely. See [PR 66](https://github.com/tilezen/mapbox-vector-tile/pull/66) for more information.
+- Improved results from `on_invalid_geometry_make_valid` when the geometry is self-crossing. It was possible for large parts of the geometry to be discarded, and it is now less likely. See [PR 66](https://github.com/tilezen/mapbox-vector-tile/pull/66) for more information.
 
-Version 0.4.0
--------------
+## Version 0.4.0
 
-* Custom rounding functions: a `round_fn` parameter was added to the `encode` function, which allows control over how floating point coordinates are transformed to integer ones. See [PR 55](https://github.com/tilezen/mapbox-vector-tile/pull/55).
-* Custom validity functions: an `on_invalid_geometry` parameter was added to the `encode` function, which is called when invalid geometry is found, or created through coordinate rounding. See [PR 46](https://github.com/tilezen/mapbox-vector-tile/pull/46).
-* Winding order bug fix: See [issue 57](https://github.com/tilezen/mapbox-vector-tile/issues/57) and [PR 59](https://github.com/tilezen/mapbox-vector-tile/pull/59).
-* Performance improvements: including a 2x speedup from using `tuple`s instead of `dict`s for coordinates, see [PR 56](https://github.com/tilezen/mapbox-vector-tile/pull/56).
-* Improvements to PY3 compatibility: See [PR 52](https://github.com/tilezen/mapbox-vector-tile/pull/52).
+- Custom rounding functions: a `round_fn` parameter was added to the `encode` function, which allows control over how floating point coordinates are transformed to integer ones. See [PR 55](https://github.com/tilezen/mapbox-vector-tile/pull/55).
+- Custom validity functions: an `on_invalid_geometry` parameter was added to the `encode` function, which is called when invalid geometry is found, or created through coordinate rounding. See [PR 46](https://github.com/tilezen/mapbox-vector-tile/pull/46).
+- Winding order bug fix: See [issue 57](https://github.com/tilezen/mapbox-vector-tile/issues/57) and [PR 59](https://github.com/tilezen/mapbox-vector-tile/pull/59).
+- Performance improvements: including a 2x speedup from using `tuple`s instead of `dict`s for coordinates, see [PR 56](https://github.com/tilezen/mapbox-vector-tile/pull/56).
+- Improvements to PY3 compatibility: See [PR 52](https://github.com/tilezen/mapbox-vector-tile/pull/52).
 
-Version 0.3.0
--------------
+## Version 0.3.0
 
-* python3 compatability improvements
-* travis integration
-* documentation updates
-* insert CMD_SEG_END for MultiPolygons
-* decode multipolygons correctly
-* encode tiles using version 1
+- python3 compatability improvements
+- travis integration
+- documentation updates
+- insert CMD_SEG_END for MultiPolygons
+- decode multipolygons correctly
+- encode tiles using version 1
 
-Version 0.2.1
--------------
+## Version 0.2.1
 
-* include README.md in distribution to fix install
+- include README.md in distribution to fix install
 
-Version 0.2.0
--------------
+## Version 0.2.0
 
-* python3 updates
-* enforce winding order on multipolygons
-* update key/val handling
-* round floating point values instead of truncating
-* add option to quantize bounds
-* add option to flip y coord system
-* add ability to pass custom extents
+- python3 updates
+- enforce winding order on multipolygons
+- update key/val handling
+- round floating point values instead of truncating
+- add option to quantize bounds
+- add option to flip y coord system
+- add ability to pass custom extents
 
-Version 0.1.0
--------------
+## Version 0.1.0
 
-* Add compatibility with python 3
-* Handle multipolygons as single features
-* Use winding order from mapbox vector tile 2.0 spec
-* Support custom extents when decoding
+- Add compatibility with python 3
+- Handle multipolygons as single features
+- Use winding order from mapbox vector tile 2.0 spec
+- Support custom extents when decoding
 
-Version 0.0.11
---------------
+## Version 0.0.11
 
-* Decode string keys to utf-8
+- Decode string keys to utf-8
 
-Version 0.0.10
---------------
+## Version 0.0.10
 
-* Allow encoder to accept shapely objects directly
+- Allow encoder to accept shapely objects directly
 
-Version 0.0.9
--------------
+## Version 0.0.9
 
-* Handle tiles from java-vector-tile (zero pad binary integers)
-* Update README
+- Handle tiles from java-vector-tile (zero pad binary integers)
+- Update README
 
-Version 0.0.8
--------------
+## Version 0.0.8
 
-* Handle unicode properties
+- Handle unicode properties
 
-Version 0.0.7
--------------
+## Version 0.0.7
 
-* Update id handling behavior
+- Update id handling behavior
 
-Version 0.0.6
--------------
+## Version 0.0.6
 
-* Explode multipolygons into several features
-* https://github.com/tilezen/mapbox-vector-tile/issues/4
-* Resolve issue when id is passed in
-* More tests
+- Explode multipolygons into several features
+- https://github.com/tilezen/mapbox-vector-tile/issues/4
+- Resolve issue when id is passed in
+- More tests
 
-Version 0.0.5
--------------
+## Version 0.0.5
 
-* Removing the option of encoding floats in big endian
-* Updated tests
+- Removing the option of encoding floats in big endian
+- Updated tests
 
-Version 0.0.4
--------------
+## Version 0.0.4
 
-* Bug fix - does not try to load wkt geom if wkb succeeds
+- Bug fix - does not try to load wkt geom if wkb succeeds
 
-Version 0.0.3
--------------
+## Version 0.0.3
 
-* Option to encode floats in little endian
+- Option to encode floats in little endian
 
-Version 0.0.2
--------------
+## Version 0.0.2
 
-* WKT Support
-* Better Documentation
-* More tests
+- WKT Support
+- Better Documentation
+- More tests
 
-Version 0.0.1
--------------
+## Version 0.0.1
 
-* Initial release
+- Initial release
```

### Comparing `mapbox_vector_tile-2.0.1/LICENSE` & `mapbox_vector_tile-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapbox_vector_tile-2.0.1/README.md` & `mapbox_vector_tile-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-Mapbox Vector Tile
-==================
+# Mapbox Vector Tile
 
 [![CI](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml)
 [![pre-commit](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml)
 [![Coverage Status](https://coveralls.io/repos/github/tilezen/mapbox-vector-tile/badge.svg?branch=master)](https://coveralls.io/github/tilezen/mapbox-vector-tile?branch=master)
 
-Installation
-------------
+## Installation
 
-mapbox-vector-tile is compatible with Python 3.8 or newer. It is listed on PyPi as `mapbox-vector-tile`. The
+mapbox-vector-tile is compatible with Python 3.9 or newer. It is listed on PyPi as `mapbox-vector-tile`. The
 recommended way to install is via `pip`:
 
 ```shell
 pip install mapbox-vector-tile
 ```
 
 An extra dependency has been defined to install [`pyproj`](https://pyproj4.github.io/pyproj/stable/). This is useful
 when changing the Coordinate Reference System when encoding or decoding tiles.
 
 ```shell
 pip install mapbox-vector-tile[proj]
 ```
 
-Encoding
---------
+## Encoding
 
 Encode method expects an array of layers or at least a single valid layer. A valid layer is a dictionary with the
 following keys
 
-* `name`: layer name
-* `features`: an array of features. A feature is a dictionary with the following keys:
+- `name`: layer name
+- `features`: an array of features. A feature is a dictionary with the following keys:
 
-  * `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. *Note* that `GeometryCollection` types are not supported, and will trigger a `ValueError`.
-  * `properties`: a dictionary with a few keys and their corresponding values.
+  - `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. _Note_ that `GeometryCollection` types are not supported, and will trigger a `ValueError`.
+  - `properties`: a dictionary with a few keys and their corresponding values.
 
 The encoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If
 there is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are
 taken into account. Finally, global default values are used. See the docstring of the `encode` method for more
 details about the available options and their global default values.
 
-
 ```python
 
   >>> import mapbox_vector_tile
 
   # Using WKT
   >>> mapbox_vector_tile.encode([
       {
@@ -271,16 +267,15 @@
             }
           }
         ]
       }
     ], default_options={"quantize_bounds": (0.0, 0.0, 10.0, 10.0), "extents":50})
 ```
 
-Decoding
---------
+## Decoding
 
 Decode method takes in a valid google.protobuf.message Tile and returns decoded string in the following format:
 
 ```python
   {
     layername: {
         'extent': 'integer layer extent'
@@ -364,17 +359,15 @@
   >>> with open('out.txt', 'w') as f:
   >>>     f.write(repr(decoded_data))
 ```
 
 The `decode` function has a `geojson` option which enforces a GeoJson RFC7946 compatible result. Its default value
 is `True`. To enforce the behaviour of versions <2.0.0, please use `geojson=False`.
 
-
-Use native protobuf library for performance
-------------------------------------------
+## Use native protobuf library for performance
 
 The c++ implementation of the underlying protobuf library is more performant than the pure python one. Depending on your operating system, you might need to [compile the C++ library](https://github.com/google/protobuf/tree/master/python#c-implementation) or install it.
 
 Since May 6, 2022, the Python `profobuf` library is based on the udp library and thus, the generated Python code
 requires `protoc` 3.19.0 or newer. Cf. [here](https://developers.google.com/protocol-buffers/docs/news/2022-05-06). On
 debian Bullseye, the version of `protoc` available in the package registry is too old. Please install it from [protobuf
 +GitHub repository](https://github.com/protocolbuffers/protobuf/releases).
@@ -388,11 +381,10 @@
      $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=cpp
      $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION_VERSION=2
 
 and then:
 
     $ protoc -I=mapbox_vector_tile/Mapbox/ --python_out=mapbox_vector_tile/Mapbox/ mapbox_vector_tile/Mapbox/vector_tile.proto
 
-Changelog
----------
+## Changelog
 
 Click [here](https://github.com/tilezen/mapbox-vector-tile/blob/master/CHANGELOG.md) to see what changed over time in various versions.
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/Mapbox/vector_tile.proto` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/Mapbox/vector_tile.proto`

 * *Files identical despite different names*

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/Mapbox/vector_tile_pb2.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/Mapbox/vector_tile_pb2.py`

 * *Files identical despite different names*

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/__init__.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             * `transformer`: a function transforming the coordinates of geometry object. It takes two floats (`x`
             and `y`) as arguments and retrieves the transformed coordinates `x_transformed`, `y_transformed`. Default to
             `None`.
             * `geojson`: when set to `False`, the behaviour of mapbox-vector-tile version 1.* is used. When set
             to `False`, the retrieved dictionary is a valid geojson file. Default to `True`.
     """
     if kwargs:
-        warnings.warn("`decode` signature has changed, use `default_options` instead", DeprecationWarning)
+        warnings.warn("`decode` signature has changed, use `default_options` instead", DeprecationWarning, stacklevel=2)
         default_options = {**kwargs, **(default_options or {})}
     vector_tile = decoder.TileData(pbf_data=tile, per_layer_options=per_layer_options, default_options=default_options)
     message = vector_tile.get_message()
     return message
 
 
 def encode(layers, per_layer_options=None, default_options=None, **kwargs):
@@ -76,19 +76,19 @@
                 * `on_invalid_geometry_ignore`: it ignores the invalid geometry and replaces it with a `None`.
                 * `on_invalid_geometry_make_valid`: it tries to make the geometry valid. If it fails, retrieves `None`.
             * `check_winding_order`: it forces the check of the winding order for polygons. Default to True.
             * `max_geometry_validate_tries`: the number of tries when trying to enforce the good winding order. Default
             to 5.
     """
     if kwargs:
-        warnings.warn("`encode` signature has changed, use `default_options` instead", DeprecationWarning)
+        warnings.warn("`encode` signature has changed, use `default_options` instead", DeprecationWarning, stacklevel=2)
         default_options = {**kwargs, **(default_options or {})}
     vector_tile = encoder.VectorTile(default_options=default_options)
     if per_layer_options is None:
-        per_layer_options = dict()
+        per_layer_options = {}
     if isinstance(layers, list):
         for layer in layers:
             layer_name = layer["name"]
             layer_options = per_layer_options.get(layer_name, None)
             vector_tile.add_layer(features=layer["features"], name=layer_name, options=layer_options)
     else:
         layer_name = layers["name"]
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/decoder.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from mapbox_vector_tile.Mapbox import vector_tile_pb2 as vector_tile
 from mapbox_vector_tile.utils import (
     CMD_BITS,
     CMD_LINE_TO,
     CMD_MOVE_TO,
     CMD_SEG_END,
-    get_decode_options,
     LINESTRING,
     POINT,
     POLYGON,
+    get_decode_options,
     zig_zag_decode,
 )
 
 
 class TileData:
     def __init__(self, pbf_data, per_layer_options=None, default_options=None):
         self.tile = vector_tile.tile()
         self.tile.ParseFromString(pbf_data)
         self.default_options = default_options
-        self.per_layer_options = per_layer_options if per_layer_options is not None else dict()
+        self.per_layer_options = per_layer_options if per_layer_options is not None else {}
 
     def get_message(self):
         tile = {}
         for layer in self.tile.layers:
             layer_name = layer.name
             layer_options = self.per_layer_options.get(layer_name, None)
             layer_options = get_decode_options(layer_options=layer_options, default_options=self.default_options)
@@ -77,15 +77,15 @@
         ):
             if val.HasField(candidate):
                 return getattr(val, candidate)
         raise ValueError(f"{val} is an unknown value")
 
     @staticmethod
     def _area_sign(ring):
-        a = sum(ring[i][0] * ring[i + 1][1] - ring[i + 1][0] * ring[i][1] for i in range(0, len(ring) - 1))
+        a = sum(ring[i][0] * ring[i + 1][1] - ring[i + 1][0] * ring[i][1] for i in range(len(ring) - 1))
         return -1 if a < 0 else 1 if a > 0 else 0
 
     @staticmethod
     def _ensure_polygon_closed(coords):
         if coords and coords[0] != coords[-1]:
             coords.append(coords[0])
 
@@ -108,27 +108,26 @@
             if cmd == CMD_SEG_END:
                 if ftype == POLYGON:
                     self._ensure_polygon_closed(coords)
                 parts.append(coords)
                 coords = []
 
             elif cmd in (CMD_MOVE_TO, CMD_LINE_TO):
-                if coords and cmd == CMD_MOVE_TO:
-                    if ftype in (LINESTRING, POLYGON):
-                        # multi line string or polygon our encoder includes CMD_SEG_END to denote the end of a
-                        # polygon ring, but this path would also handle the case where we receive a move without a
-                        # previous close on polygons
-
-                        # for polygons, we want to ensure that it is closed
-                        if ftype == POLYGON:
-                            self._ensure_polygon_closed(coords)
-                        parts.append(coords)
-                        coords = []
+                if coords and cmd == CMD_MOVE_TO and ftype in (LINESTRING, POLYGON):
+                    # multi line string or polygon our encoder includes CMD_SEG_END to denote the end of a
+                    # polygon ring, but this path would also handle the case where we receive a move without a
+                    # previous close on polygons
+
+                    # for polygons, we want to ensure that it is closed
+                    if ftype == POLYGON:
+                        self._ensure_polygon_closed(coords)
+                    parts.append(coords)
+                    coords = []
 
-                for point in range(0, cmd_len):
+                for _ in range(cmd_len):
                     x = geom[i]
                     i = i + 1
 
                     y = geom[i]
                     i = i + 1
 
                     # zigzag decode
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/encoder.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from numbers import Number
 
 from shapely.geometry import shape as shapely_shape
 from shapely.geometry.base import BaseGeometry
 from shapely.geometry.multipolygon import MultiPolygon
-from shapely.geometry.polygon import orient, Polygon
+from shapely.geometry.polygon import Polygon, orient
 from shapely.ops import transform
 from shapely.wkb import loads as load_wkb
 from shapely.wkt import loads as load_wkt
 
-from mapbox_vector_tile.Mapbox import vector_tile_pb2 as vector_tile
 from mapbox_vector_tile.geom_encoder import GeometryEncoder
+from mapbox_vector_tile.Mapbox import vector_tile_pb2 as vector_tile
 from mapbox_vector_tile.polygon import make_it_valid
 from mapbox_vector_tile.utils import get_encode_options
 
 
 def on_invalid_geometry_raise(shape):
     raise ValueError(f"Invalid geometry: {shape.wkt}")
 
@@ -139,19 +139,15 @@
                     parts.extend(part.geoms)
                 else:
                     parts.append(part)
 
         if not parts:
             return None
 
-        if len(parts) == 1:
-            oriented_shape = parts[0]
-        else:
-            oriented_shape = MultiPolygon(parts)
-
+        oriented_shape = parts[0] if len(parts) == 1 else MultiPolygon(parts)
         oriented_shape = self.handle_shape_validity(oriented_shape, n_try)
         return oriented_shape
 
     def enforce_polygon_winding_order(self, shape, n_try):
         assert shape.geom_type == "Polygon"
 
         def fn(point):
@@ -199,17 +195,16 @@
         feature_type = self._get_feature_type(shape)
         if len(geometry) == 0:
             # Don't add geometry if it's too small
             return
         f = self.layer.features.add()
 
         fid = feature.get("id")
-        if fid is not None:
-            if isinstance(fid, Number) and fid >= 0:
-                f.id = fid
+        if fid is not None and isinstance(fid, Number) and fid >= 0:
+            f.id = fid
 
         # properties
         properties = feature.get("properties")
         if properties is not None:
             self._handle_attr(self.layer, f, properties)
 
         f.type = feature_type
@@ -249,19 +244,15 @@
                 if k not in self.seen_keys_idx:
                     layer.keys.append(k)
                     self.seen_keys_idx[k] = self.key_idx
                     self.key_idx += 1
 
                 feature.tags.append(self.seen_keys_idx[k])
 
-                if isinstance(v, bool):
-                    values_idx = self.seen_values_bool_idx
-                else:
-                    values_idx = self.seen_values_idx
-
+                values_idx = self.seen_values_bool_idx if isinstance(v, bool) else self.seen_values_idx
                 if v not in values_idx:
                     values_idx[v] = self.val_idx
                     self.val_idx += 1
 
                     val = layer.values.add()
                     if isinstance(v, bool):
                         val.bool_value = v
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/geom_encoder.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/geom_encoder.py`

 * *Files identical despite different names*

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/optimise.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/optimise.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
             self.val_counts[v] = self.val_counts.get(v, 0) + 1
 
     @staticmethod
     def _update_table(counts, table):
         # Sort string table by usage, so most commonly-used values are
         # assigned the smallest indices. Since indices are encoded as
         # varints, this should make best use of the space.
-        sort = list(sorted(((c, k) for k, c in counts.items()), reverse=True))
+        sort = sorted(((c, k) for k, c in counts.items()), reverse=True)
 
         # construct the re-ordered string table
         new_table = []
         for _, x in sort:
             new_table.append(table[x])
         assert len(new_table) == len(table)
 
         # delete table in place and replace with the new table
         del table[:]
         table.extend(new_table)
 
         # construct a lookup table from the old to the new indices.
         new_indexes = {}
-        for i, (c, k) in enumerate(sort):
+        for i, (_, k) in enumerate(sort):
             new_indexes[k] = i
 
         return new_indexes
 
     def update_string_table(self, layer):
         new_key = self._update_table(self.key_counts, layer.keys)
         new_val = self._update_table(self.val_counts, layer.values)
@@ -108,15 +108,15 @@
             assert current_moveto
 
             # we just copy this run, since it's encoding isn't going to change
             next_i = i + 1 + run_length * 2
             current_line.extend(geom[i:next_i])
 
             # but we still need to decode it to figure out where each move-to command is in absolute space.
-            for j in range(0, run_length):
+            for j in range(run_length):
                 dx = zig_zag_decode(geom[i + 1 + 2 * j])
                 dy = zig_zag_decode(geom[i + 2 + 2 * j])
                 x += dx
                 y += dy
 
             i = next_i
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/polygon.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,31 +89,25 @@
         polygons.extend(p)
         children.extend(c)
 
     if node.IsHole:
         # Check expectations: a node should be a hole, _or_ return children. This is because children of holes must
         # be outers, and should be on the polygons list.
         assert len(children) == 0
-        if node.Contour:
-            children = [node.Contour]
-        else:
-            children = []
+        children = [node.Contour] if node.Contour else []
 
     elif node.Contour:
         poly = _contour_to_poly(node.Contour)
 
         # We add each inner one-by-one so that we can reject them individually if they cause the polygon to become
         # invalid. If the shape has lots of inners, then this can mean a proportional amount of work, and may take
         # 1,000s of seconds. Instead, we can group inners together, which reduces the number of times we call the
         # expensive 'difference' method.
         block_size = 200
-        if len(children) > block_size:
-            inners = _union_in_blocks(children, block_size)
-        else:
-            inners = _generate_polys(children)
+        inners = _union_in_blocks(children, block_size) if len(children) > block_size else _generate_polys(children)
 
         for inner in inners:
             # The difference of two valid polygons may fail, and in this  situation we'd like to be able to display
             # the polygon anyway. So we discard the bad inner and continue.
             #
             # See test_polygon_inners_crossing_outer for a test case.
             try:
```

### Comparing `mapbox_vector_tile-2.0.1/mapbox_vector_tile/utils.py` & `mapbox_vector_tile-2.1.0/mapbox_vector_tile/utils.py`

 * *Files identical despite different names*

### Comparing `mapbox_vector_tile-2.0.1/setup.py` & `mapbox_vector_tile-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['mapbox_vector_tile', 'mapbox_vector_tile.Mapbox']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['protobuf>=4.21,<5.0', 'pyclipper>=1.3.0,<2.0.0', 'shapely>=2.0.0,<3.0.0']
+['protobuf>=5.26.1,<6.0.0', 'pyclipper>=1.3.0,<2.0.0', 'shapely>=2.0.0,<3.0.0']
 
 extras_require = \
 {'proj': ['pyproj>=3.4.1,<4.0.0']}
 
 setup_kwargs = {
     'name': 'mapbox-vector-tile',
-    'version': '2.0.1',
+    'version': '2.1.0',
     'description': 'Mapbox Vector Tile encoding and decoding.',
-    'long_description': 'Mapbox Vector Tile\n==================\n\n[![CI](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml)\n[![pre-commit](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml)\n[![Coverage Status](https://coveralls.io/repos/github/tilezen/mapbox-vector-tile/badge.svg?branch=master)](https://coveralls.io/github/tilezen/mapbox-vector-tile?branch=master)\n\nInstallation\n------------\n\nmapbox-vector-tile is compatible with Python 3.8 or newer. It is listed on PyPi as `mapbox-vector-tile`. The\nrecommended way to install is via `pip`:\n\n```shell\npip install mapbox-vector-tile\n```\n\nAn extra dependency has been defined to install [`pyproj`](https://pyproj4.github.io/pyproj/stable/). This is useful\nwhen changing the Coordinate Reference System when encoding or decoding tiles.\n\n```shell\npip install mapbox-vector-tile[proj]\n```\n\nEncoding\n--------\n\nEncode method expects an array of layers or at least a single valid layer. A valid layer is a dictionary with the\nfollowing keys\n\n* `name`: layer name\n* `features`: an array of features. A feature is a dictionary with the following keys:\n\n  * `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. *Note* that `GeometryCollection` types are not supported, and will trigger a `ValueError`.\n  * `properties`: a dictionary with a few keys and their corresponding values.\n\nThe encoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If\nthere is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are\ntaken into account. Finally, global default values are used. See the docstring of the `encode` method for more\ndetails about the available options and their global default values.\n\n\n```python\n\n  >>> import mapbox_vector_tile\n\n  # Using WKT\n  >>> mapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POLYGON ((0 0, 0 1, 1 1, 1 0, 0 0))",\n            "properties":{\n              "uid":123,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      },\n      {\n        "name": "air",\n        "features": [\n          {\n            "geometry":"LINESTRING(159 3877, -1570 3877)",\n            "properties":{\n              "uid":1234,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      }\n    ])\n\n  b\'\\x1aH\\n\\x05water\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x02 {"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aD\\n\\x03air\\x12\\x15\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x02"\\t\\t\\xbe\\x02\\xb6\\x03\\n\\x81\\x1b\\x00\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x03 \\xd2\\t"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\'\n\n\n  # Using WKB\n  >>> mapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":b"\\x01\\x03\\x00\\x00\\x00\\x01\\x00\\x00\\x00\\x05\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00",\n            "properties":{\n              "uid":123,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      },\n      {\n        "name": "air",\n        "features": [\n          {\n            "geometry":b"\\x01\\x03\\x00\\x00\\x00\\x01\\x00\\x00\\x00\\x05\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00",\n            "properties":{\n              "uid":1234,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      }\n      ])\n\n    b\'\\x1aH\\n\\x05water\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x02 {"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aG\\n\\x03air\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x03 \\xd2\\t"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\'\n```\n\n### Coordinate transformations for encoding\n\nThe encoder expects geometries either:\n\n1. In tile-relative coordinates, where the lower left corner is origin and values grow up and to the right, and the tile is 4096 pixels square. For example, `POINT(0 0)` is the lower left corner of the tile and `POINT(4096, 4096)` is the upper right corner of the tile. In this case, the library does no projection, and coordinates are encoded as-is.\n2. In another coordinate system, with the tile bounds given by the `quantize_bounds` parameter. In this case, the library will scale coordinates so that the `quantize_bounds` fit within the range (0, 4096) in both `x` and `y` directions. Aside than the affine transformation, the library does no other projection.\n\nIt is possible to control whether the tile is in a "y down" coordinate system by setting the parameter `y_coord_down=True` on the call to `encode()`. The default is "y up".\n\nIt is possible to control the tile extents (by default, 4096 as used in the examples above), by setting the `extents` parameter on the call to `encode()`. The default is 4096.\n\nIf you have geometries in longitude and latitude (EPSG:4326), you can convert to tile-based coordinates by first projecting to Spherical Mercator (EPSG:3857) and then computing the pixel location within the tile. This example code uses Django\'s included GEOS library to do the transformation for `LineString` objects:\n\n```python\n  SRID_SPHERICAL_MERCATOR = 3857\n\n  def linestring_in_tile(tile_bounds, line):\n      # `mapbox-vector-tile` has a hardcoded tile extent of 4096 units.\n      MVT_EXTENT = 4096\n      from django.contrib.gis.geos import LineString\n\n      # We need tile bounds in spherical mercator\n      assert tile_bounds.srid == SRID_SPHERICAL_MERCATOR\n\n      # And we need the line to be in a known projection so we can re-project\n      assert line.srid is not None\n      line.transform(SRID_SPHERICAL_MERCATOR)\n\n      (x0, y0, x_max, y_max) = tile_bounds.extent\n      x_span = x_max - x0\n      y_span = y_max - y0\n\n      tile_based_coords = []\n      for x_merc, y_merc in line:\n          tile_based_coord = (int((x_merc - x0) * MVT_EXTENT / x_span),\n                              int((y_merc - y0) * MVT_EXTENT / y_span))\n          tile_based_coords.append(tile_based_coord)\n      return LineString(*tile_based_coords)\n```\n\nThe tile bounds can be found with `mercantile`, so a complete usage example might look like this:\n\n```python\n  from django.contrib.gis.geos import LineString, Polygon\n  import mercantile\n  import mapbox_vector_tile\n\n  SRID_LNGLAT = 4326\n  SRID_SPHERICAL_MERCATOR = 3857\n\n  tile_xyz = (2452, 3422, 18)\n  tile_bounds = Polygon.from_bbox(mercantile.bounds(*tile_xyz))\n  tile_bounds.srid = SRID_LNGLAT\n  tile_bounds.transform(SRID_SPHERICAL_MERCATOR)\n\n  lnglat_line = LineString(((-122.1, 45.1), (-122.2, 45.2)), srid=SRID_LNGLAT)\n  tile_line = linestring_in_tile(tile_bounds, lnglat_line)\n  tile_pbf = mapbox_vector_tile.encode({\n    "name": "my-layer",\n    "features": [ {\n      "geometry": tile_line.wkt,\n      "properties": { "stuff": "things" },\n    } ]\n  })\n```\n\nNote that this example may not have anything visible within the tile when rendered. It\'s up to you to make sure you put the right data in the tile!\n\nAlso note that the spec allows the extents to be modified, even though they are often set to 4096 by convention. `mapbox-vector-tile` assumes an extent of 4096.\n\n```python\n  import mapbox_vector_tile\n  from pyproj import Transformer\n  from shapely.geometry import LineString\n\n  SRID_LNGLAT = 4326\n  SRID_SPHERICAL_MERCATOR = 3857\n  direct_transformer = Transformer.from_crs(crs_from=SRID_LNGLAT, crs_to=SRID_SPHERICAL_MERCATOR, always_xy=True)\n\n  lnglat_line = LineString(((-122.1, 45.1), (-122.2, 45.2)))\n\n  # Encode the tile\n  tile_pbf = mapbox_vector_tile.encode({\n    "name": "my-layer",\n    "features": [{\n      "geometry": lnglat_line.wkt,\n      "properties": {"stuff": "things"},\n    }]\n  },\n    default_options={"transformer": direct_transformer.transform})\n\n  # Decode the tile\n  reverse_transformer = Transformer.from_crs(crs_from=SRID_SPHERICAL_MERCATOR, crs_to=SRID_LNGLAT, always_xy=True)\n  mapbox_vector_tile.decode(tile=tile_pbf, default_options={"transformer": reverse_transformer.transform})\n\n  {\n      "my-layer": {\n          "extent": 4096,\n          "version": 1,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "LineString",\n                      "coordinates": [\n                          [-122.10000156433787, 45.09999871982179],\n                          [-122.20000202176608, 45.20000292038091]\n                      ]\n                  },\n                  "properties": {\n                      "stuff": "things"\n                  },\n                  "id": 0,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      }\n  }\n```\n\n### Quantization\n\nThe encoder also has options to quantize the data for you via the `quantize_bounds` option. When encoding, pass in the bounds in the form (minx, miny, maxx, maxy) and the coordinates will be scaled appropriately during encoding.\n\n```python\nmapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POINT(15 15)",\n            "properties":{\n              "foo":"bar",\n            }\n          }\n        ]\n      }\n    ], default_options={"quantize_bounds": (10.0, 10.0, 20.0, 20.0)})\n```\n\nIn this example, the coordinate that would get encoded would be (2048, 2048)\n\nAdditionally, if the data is already in a coordinate system with y values going down, the encoder supports an\noption, `y_coord_down`, that can be set to True. This will suppress flipping the y coordinate values during encoding.\n\n### Custom extents\n\nThe encoder also supports passing in custom extents. These will be passed through to the layer in the pbf, and honored during any quantization or y coordinate flipping.\n\n```python\nmapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POINT(15 15)",\n            "properties":{\n              "foo":"bar",\n            }\n          }\n        ]\n      }\n    ], default_options={"quantize_bounds": (0.0, 0.0, 10.0, 10.0), "extents":50})\n```\n\nDecoding\n--------\n\nDecode method takes in a valid google.protobuf.message Tile and returns decoded string in the following format:\n\n```python\n  {\n    layername: {\n        \'extent\': \'integer layer extent\'\n        \'version\': \'integer\'\n        \'features\': [{\n          \'geometry\': \'list of points\',\n          \'properties\': \'dictionary of key/value pairs\',\n          \'id\': \'unique id for the given feature within the layer \'\n          }, ...\n        ]\n    },\n    layername2: {\n      # ...\n    }\n  }\n```\n\nThe decoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If\nthere is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are\ntaken into account. Finally, global default values are used. See the docstring of the `decode` method for more\ndetails about the available options and their global default values.\n\n```python\n  >>> import mapbox_vector_tile\n\n  >>> mapbox_vector_tile.decode(b\'\\x1aJ\\n\\x05water\\x12\\x1a\\x08\\x01\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03foo\\x1a\\x03uid\\x1a\\x03cat"\\x05\\n\\x03bar"\\x02 {"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aY\\n\\x03air\\x12\\x1c\\x08\\x01\\x12\\x08\\x00\\x00\\x01\\x01\\x02\\x02\\x03\\x03\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03foo\\x1a\\x03uid\\x1a\\x05balls\\x1a\\x03cat"\\x05\\n\\x03bar"\\x03 \\xd2\\t"\\x05\\n\\x03foo"\\x06\\n\\x04flew(\\x80 x\\x02\')\n\n  {\n      "water": {\n          "extent": 4096,\n          "version": 2,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "Polygon",\n                      "coordinates": [[[0,0],[0,1],[1,1],[1,0],[0,0]]]\n                  },\n                  "properties": {\n                      "foo": "bar",\n                      "uid": 123,\n                      "cat": "flew"\n                  },\n                  "id": 1,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      },\n      "air": {\n          "extent": 4096,\n          "version": 2,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "Polygon",\n                      "coordinates": [[[0,0],[0,1],[1,1],[1,0],[0,0]]]\n                  },\n                  "properties": {\n                      "foo": "bar",\n                      "uid": 1234,\n                      "balls": "foo",\n                      "cat": "flew"\n                  },\n                  "id": 1,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      }\n  }\n\n```\n\nHere\'s how you might decode a tile from a file.\n\n```python\n  >>> import mapbox_vector_tile\n  >>> with open(\'tile.mvt\', \'rb\') as f:\n  >>>     data = f.read()\n  >>> decoded_data = mapbox_vector_tile.decode(data)\n  >>> with open(\'out.txt\', \'w\') as f:\n  >>>     f.write(repr(decoded_data))\n```\n\nThe `decode` function has a `geojson` option which enforces a GeoJson RFC7946 compatible result. Its default value\nis `True`. To enforce the behaviour of versions <2.0.0, please use `geojson=False`.\n\n\nUse native protobuf library for performance\n------------------------------------------\n\nThe c++ implementation of the underlying protobuf library is more performant than the pure python one. Depending on your operating system, you might need to [compile the C++ library](https://github.com/google/protobuf/tree/master/python#c-implementation) or install it.\n\nSince May 6, 2022, the Python `profobuf` library is based on the udp library and thus, the generated Python code\nrequires `protoc` 3.19.0 or newer. Cf. [here](https://developers.google.com/protocol-buffers/docs/news/2022-05-06). On\ndebian Bullseye, the version of `protoc` available in the package registry is too old. Please install it from [protobuf\n+GitHub repository](https://github.com/protocolbuffers/protobuf/releases).\n\nTo compile the `proto` file, you have to enable two environnement variables BEFORE running your python program :\n\n    $  sudo apt-get install libprotoc9 libprotobuf9 protobuf-compiler python-protobuf\n\nThen, you\'ll have to enable two environnement variable BEFORE runing your python program :\n\n     $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=cpp\n     $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION_VERSION=2\n\nand then:\n\n    $ protoc -I=mapbox_vector_tile/Mapbox/ --python_out=mapbox_vector_tile/Mapbox/ mapbox_vector_tile/Mapbox/vector_tile.proto\n\nChangelog\n---------\n\nClick [here](https://github.com/tilezen/mapbox-vector-tile/blob/master/CHANGELOG.md) to see what changed over time in various versions.\n',
+    'long_description': '# Mapbox Vector Tile\n\n[![CI](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml)\n[![pre-commit](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml)\n[![Coverage Status](https://coveralls.io/repos/github/tilezen/mapbox-vector-tile/badge.svg?branch=master)](https://coveralls.io/github/tilezen/mapbox-vector-tile?branch=master)\n\n## Installation\n\nmapbox-vector-tile is compatible with Python 3.9 or newer. It is listed on PyPi as `mapbox-vector-tile`. The\nrecommended way to install is via `pip`:\n\n```shell\npip install mapbox-vector-tile\n```\n\nAn extra dependency has been defined to install [`pyproj`](https://pyproj4.github.io/pyproj/stable/). This is useful\nwhen changing the Coordinate Reference System when encoding or decoding tiles.\n\n```shell\npip install mapbox-vector-tile[proj]\n```\n\n## Encoding\n\nEncode method expects an array of layers or at least a single valid layer. A valid layer is a dictionary with the\nfollowing keys\n\n- `name`: layer name\n- `features`: an array of features. A feature is a dictionary with the following keys:\n\n  - `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. _Note_ that `GeometryCollection` types are not supported, and will trigger a `ValueError`.\n  - `properties`: a dictionary with a few keys and their corresponding values.\n\nThe encoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If\nthere is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are\ntaken into account. Finally, global default values are used. See the docstring of the `encode` method for more\ndetails about the available options and their global default values.\n\n```python\n\n  >>> import mapbox_vector_tile\n\n  # Using WKT\n  >>> mapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POLYGON ((0 0, 0 1, 1 1, 1 0, 0 0))",\n            "properties":{\n              "uid":123,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      },\n      {\n        "name": "air",\n        "features": [\n          {\n            "geometry":"LINESTRING(159 3877, -1570 3877)",\n            "properties":{\n              "uid":1234,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      }\n    ])\n\n  b\'\\x1aH\\n\\x05water\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x02 {"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aD\\n\\x03air\\x12\\x15\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x02"\\t\\t\\xbe\\x02\\xb6\\x03\\n\\x81\\x1b\\x00\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x03 \\xd2\\t"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\'\n\n\n  # Using WKB\n  >>> mapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":b"\\x01\\x03\\x00\\x00\\x00\\x01\\x00\\x00\\x00\\x05\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00",\n            "properties":{\n              "uid":123,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      },\n      {\n        "name": "air",\n        "features": [\n          {\n            "geometry":b"\\x01\\x03\\x00\\x00\\x00\\x01\\x00\\x00\\x00\\x05\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\xf0?\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00\\x00",\n            "properties":{\n              "uid":1234,\n              "foo":"bar",\n              "cat":"flew"\n            }\n          }\n        ]\n      }\n      ])\n\n    b\'\\x1aH\\n\\x05water\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x02 {"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aG\\n\\x03air\\x12\\x18\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03uid\\x1a\\x03foo\\x1a\\x03cat"\\x03 \\xd2\\t"\\x05\\n\\x03bar"\\x06\\n\\x04flew(\\x80 x\\x02\'\n```\n\n### Coordinate transformations for encoding\n\nThe encoder expects geometries either:\n\n1. In tile-relative coordinates, where the lower left corner is origin and values grow up and to the right, and the tile is 4096 pixels square. For example, `POINT(0 0)` is the lower left corner of the tile and `POINT(4096, 4096)` is the upper right corner of the tile. In this case, the library does no projection, and coordinates are encoded as-is.\n2. In another coordinate system, with the tile bounds given by the `quantize_bounds` parameter. In this case, the library will scale coordinates so that the `quantize_bounds` fit within the range (0, 4096) in both `x` and `y` directions. Aside than the affine transformation, the library does no other projection.\n\nIt is possible to control whether the tile is in a "y down" coordinate system by setting the parameter `y_coord_down=True` on the call to `encode()`. The default is "y up".\n\nIt is possible to control the tile extents (by default, 4096 as used in the examples above), by setting the `extents` parameter on the call to `encode()`. The default is 4096.\n\nIf you have geometries in longitude and latitude (EPSG:4326), you can convert to tile-based coordinates by first projecting to Spherical Mercator (EPSG:3857) and then computing the pixel location within the tile. This example code uses Django\'s included GEOS library to do the transformation for `LineString` objects:\n\n```python\n  SRID_SPHERICAL_MERCATOR = 3857\n\n  def linestring_in_tile(tile_bounds, line):\n      # `mapbox-vector-tile` has a hardcoded tile extent of 4096 units.\n      MVT_EXTENT = 4096\n      from django.contrib.gis.geos import LineString\n\n      # We need tile bounds in spherical mercator\n      assert tile_bounds.srid == SRID_SPHERICAL_MERCATOR\n\n      # And we need the line to be in a known projection so we can re-project\n      assert line.srid is not None\n      line.transform(SRID_SPHERICAL_MERCATOR)\n\n      (x0, y0, x_max, y_max) = tile_bounds.extent\n      x_span = x_max - x0\n      y_span = y_max - y0\n\n      tile_based_coords = []\n      for x_merc, y_merc in line:\n          tile_based_coord = (int((x_merc - x0) * MVT_EXTENT / x_span),\n                              int((y_merc - y0) * MVT_EXTENT / y_span))\n          tile_based_coords.append(tile_based_coord)\n      return LineString(*tile_based_coords)\n```\n\nThe tile bounds can be found with `mercantile`, so a complete usage example might look like this:\n\n```python\n  from django.contrib.gis.geos import LineString, Polygon\n  import mercantile\n  import mapbox_vector_tile\n\n  SRID_LNGLAT = 4326\n  SRID_SPHERICAL_MERCATOR = 3857\n\n  tile_xyz = (2452, 3422, 18)\n  tile_bounds = Polygon.from_bbox(mercantile.bounds(*tile_xyz))\n  tile_bounds.srid = SRID_LNGLAT\n  tile_bounds.transform(SRID_SPHERICAL_MERCATOR)\n\n  lnglat_line = LineString(((-122.1, 45.1), (-122.2, 45.2)), srid=SRID_LNGLAT)\n  tile_line = linestring_in_tile(tile_bounds, lnglat_line)\n  tile_pbf = mapbox_vector_tile.encode({\n    "name": "my-layer",\n    "features": [ {\n      "geometry": tile_line.wkt,\n      "properties": { "stuff": "things" },\n    } ]\n  })\n```\n\nNote that this example may not have anything visible within the tile when rendered. It\'s up to you to make sure you put the right data in the tile!\n\nAlso note that the spec allows the extents to be modified, even though they are often set to 4096 by convention. `mapbox-vector-tile` assumes an extent of 4096.\n\n```python\n  import mapbox_vector_tile\n  from pyproj import Transformer\n  from shapely.geometry import LineString\n\n  SRID_LNGLAT = 4326\n  SRID_SPHERICAL_MERCATOR = 3857\n  direct_transformer = Transformer.from_crs(crs_from=SRID_LNGLAT, crs_to=SRID_SPHERICAL_MERCATOR, always_xy=True)\n\n  lnglat_line = LineString(((-122.1, 45.1), (-122.2, 45.2)))\n\n  # Encode the tile\n  tile_pbf = mapbox_vector_tile.encode({\n    "name": "my-layer",\n    "features": [{\n      "geometry": lnglat_line.wkt,\n      "properties": {"stuff": "things"},\n    }]\n  },\n    default_options={"transformer": direct_transformer.transform})\n\n  # Decode the tile\n  reverse_transformer = Transformer.from_crs(crs_from=SRID_SPHERICAL_MERCATOR, crs_to=SRID_LNGLAT, always_xy=True)\n  mapbox_vector_tile.decode(tile=tile_pbf, default_options={"transformer": reverse_transformer.transform})\n\n  {\n      "my-layer": {\n          "extent": 4096,\n          "version": 1,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "LineString",\n                      "coordinates": [\n                          [-122.10000156433787, 45.09999871982179],\n                          [-122.20000202176608, 45.20000292038091]\n                      ]\n                  },\n                  "properties": {\n                      "stuff": "things"\n                  },\n                  "id": 0,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      }\n  }\n```\n\n### Quantization\n\nThe encoder also has options to quantize the data for you via the `quantize_bounds` option. When encoding, pass in the bounds in the form (minx, miny, maxx, maxy) and the coordinates will be scaled appropriately during encoding.\n\n```python\nmapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POINT(15 15)",\n            "properties":{\n              "foo":"bar",\n            }\n          }\n        ]\n      }\n    ], default_options={"quantize_bounds": (10.0, 10.0, 20.0, 20.0)})\n```\n\nIn this example, the coordinate that would get encoded would be (2048, 2048)\n\nAdditionally, if the data is already in a coordinate system with y values going down, the encoder supports an\noption, `y_coord_down`, that can be set to True. This will suppress flipping the y coordinate values during encoding.\n\n### Custom extents\n\nThe encoder also supports passing in custom extents. These will be passed through to the layer in the pbf, and honored during any quantization or y coordinate flipping.\n\n```python\nmapbox_vector_tile.encode([\n      {\n        "name": "water",\n        "features": [\n          {\n            "geometry":"POINT(15 15)",\n            "properties":{\n              "foo":"bar",\n            }\n          }\n        ]\n      }\n    ], default_options={"quantize_bounds": (0.0, 0.0, 10.0, 10.0), "extents":50})\n```\n\n## Decoding\n\nDecode method takes in a valid google.protobuf.message Tile and returns decoded string in the following format:\n\n```python\n  {\n    layername: {\n        \'extent\': \'integer layer extent\'\n        \'version\': \'integer\'\n        \'features\': [{\n          \'geometry\': \'list of points\',\n          \'properties\': \'dictionary of key/value pairs\',\n          \'id\': \'unique id for the given feature within the layer \'\n          }, ...\n        ]\n    },\n    layername2: {\n      # ...\n    }\n  }\n```\n\nThe decoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If\nthere is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are\ntaken into account. Finally, global default values are used. See the docstring of the `decode` method for more\ndetails about the available options and their global default values.\n\n```python\n  >>> import mapbox_vector_tile\n\n  >>> mapbox_vector_tile.decode(b\'\\x1aJ\\n\\x05water\\x12\\x1a\\x08\\x01\\x12\\x06\\x00\\x00\\x01\\x01\\x02\\x02\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03foo\\x1a\\x03uid\\x1a\\x03cat"\\x05\\n\\x03bar"\\x02 {"\\x06\\n\\x04flew(\\x80 x\\x02\\x1aY\\n\\x03air\\x12\\x1c\\x08\\x01\\x12\\x08\\x00\\x00\\x01\\x01\\x02\\x02\\x03\\x03\\x18\\x03"\\x0c\\t\\x00\\x80@\\x1a\\x00\\x01\\x02\\x00\\x00\\x02\\x0f\\x1a\\x03foo\\x1a\\x03uid\\x1a\\x05balls\\x1a\\x03cat"\\x05\\n\\x03bar"\\x03 \\xd2\\t"\\x05\\n\\x03foo"\\x06\\n\\x04flew(\\x80 x\\x02\')\n\n  {\n      "water": {\n          "extent": 4096,\n          "version": 2,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "Polygon",\n                      "coordinates": [[[0,0],[0,1],[1,1],[1,0],[0,0]]]\n                  },\n                  "properties": {\n                      "foo": "bar",\n                      "uid": 123,\n                      "cat": "flew"\n                  },\n                  "id": 1,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      },\n      "air": {\n          "extent": 4096,\n          "version": 2,\n          "features": [\n              {\n                  "geometry": {\n                      "type": "Polygon",\n                      "coordinates": [[[0,0],[0,1],[1,1],[1,0],[0,0]]]\n                  },\n                  "properties": {\n                      "foo": "bar",\n                      "uid": 1234,\n                      "balls": "foo",\n                      "cat": "flew"\n                  },\n                  "id": 1,\n                  "type": "Feature"\n              }\n          ],\n          "type": "FeatureCollection"\n      }\n  }\n\n```\n\nHere\'s how you might decode a tile from a file.\n\n```python\n  >>> import mapbox_vector_tile\n  >>> with open(\'tile.mvt\', \'rb\') as f:\n  >>>     data = f.read()\n  >>> decoded_data = mapbox_vector_tile.decode(data)\n  >>> with open(\'out.txt\', \'w\') as f:\n  >>>     f.write(repr(decoded_data))\n```\n\nThe `decode` function has a `geojson` option which enforces a GeoJson RFC7946 compatible result. Its default value\nis `True`. To enforce the behaviour of versions <2.0.0, please use `geojson=False`.\n\n## Use native protobuf library for performance\n\nThe c++ implementation of the underlying protobuf library is more performant than the pure python one. Depending on your operating system, you might need to [compile the C++ library](https://github.com/google/protobuf/tree/master/python#c-implementation) or install it.\n\nSince May 6, 2022, the Python `profobuf` library is based on the udp library and thus, the generated Python code\nrequires `protoc` 3.19.0 or newer. Cf. [here](https://developers.google.com/protocol-buffers/docs/news/2022-05-06). On\ndebian Bullseye, the version of `protoc` available in the package registry is too old. Please install it from [protobuf\n+GitHub repository](https://github.com/protocolbuffers/protobuf/releases).\n\nTo compile the `proto` file, you have to enable two environnement variables BEFORE running your python program :\n\n    $  sudo apt-get install libprotoc9 libprotobuf9 protobuf-compiler python-protobuf\n\nThen, you\'ll have to enable two environnement variable BEFORE runing your python program :\n\n     $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=cpp\n     $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION_VERSION=2\n\nand then:\n\n    $ protoc -I=mapbox_vector_tile/Mapbox/ --python_out=mapbox_vector_tile/Mapbox/ mapbox_vector_tile/Mapbox/vector_tile.proto\n\n## Changelog\n\nClick [here](https://github.com/tilezen/mapbox-vector-tile/blob/master/CHANGELOG.md) to see what changed over time in various versions.\n',
     'author': 'Rob Marianski',
     'author_email': 'rob@marianski.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tilezen/mapbox-vector-tile',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mapbox_vector_tile-2.0.1/PKG-INFO` & `mapbox_vector_tile-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 Metadata-Version: 2.1
 Name: mapbox-vector-tile
-Version: 2.0.1
+Version: 2.1.0
 Summary: Mapbox Vector Tile encoding and decoding.
 Home-page: https://github.com/tilezen/mapbox-vector-tile
 License: MIT
 Author: Rob Marianski
 Author-email: rob@marianski.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: proj
-Requires-Dist: protobuf (>=4.21,<5.0)
+Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: pyclipper (>=1.3.0,<2.0.0)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0) ; extra == "proj"
 Requires-Dist: shapely (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/tilezen/mapbox-vector-tile
 Description-Content-Type: text/markdown
 
-Mapbox Vector Tile
-==================
+# Mapbox Vector Tile
 
 [![CI](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/ci.yml)
 [![pre-commit](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/tilezen/mapbox-vector-tile/actions/workflows/pre-commit.yml)
 [![Coverage Status](https://coveralls.io/repos/github/tilezen/mapbox-vector-tile/badge.svg?branch=master)](https://coveralls.io/github/tilezen/mapbox-vector-tile?branch=master)
 
-Installation
-------------
+## Installation
 
-mapbox-vector-tile is compatible with Python 3.8 or newer. It is listed on PyPi as `mapbox-vector-tile`. The
+mapbox-vector-tile is compatible with Python 3.9 or newer. It is listed on PyPi as `mapbox-vector-tile`. The
 recommended way to install is via `pip`:
 
 ```shell
 pip install mapbox-vector-tile
 ```
 
 An extra dependency has been defined to install [`pyproj`](https://pyproj4.github.io/pyproj/stable/). This is useful
 when changing the Coordinate Reference System when encoding or decoding tiles.
 
 ```shell
 pip install mapbox-vector-tile[proj]
 ```
 
-Encoding
---------
+## Encoding
 
 Encode method expects an array of layers or at least a single valid layer. A valid layer is a dictionary with the
 following keys
 
-* `name`: layer name
-* `features`: an array of features. A feature is a dictionary with the following keys:
+- `name`: layer name
+- `features`: an array of features. A feature is a dictionary with the following keys:
 
-  * `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. *Note* that `GeometryCollection` types are not supported, and will trigger a `ValueError`.
-  * `properties`: a dictionary with a few keys and their corresponding values.
+  - `geometry`: representation of the feature geometry in WKT, WKB, or a shapely geometry. Coordinates are relative to the tile, scaled in the range `[0, 4096)`. See below for example code to perform the necessary transformation. _Note_ that `GeometryCollection` types are not supported, and will trigger a `ValueError`.
+  - `properties`: a dictionary with a few keys and their corresponding values.
 
 The encoding operation accepts options which can be defined per layer using the `per_layer_options` argument. If
 there is missing layer or missing options values in the `per_layer_options`, the options of `default_options` are
 taken into account. Finally, global default values are used. See the docstring of the `encode` method for more
 details about the available options and their global default values.
 
-
 ```python
 
   >>> import mapbox_vector_tile
 
   # Using WKT
   >>> mapbox_vector_tile.encode([
       {
@@ -298,16 +293,15 @@
             }
           }
         ]
       }
     ], default_options={"quantize_bounds": (0.0, 0.0, 10.0, 10.0), "extents":50})
 ```
 
-Decoding
---------
+## Decoding
 
 Decode method takes in a valid google.protobuf.message Tile and returns decoded string in the following format:
 
 ```python
   {
     layername: {
         'extent': 'integer layer extent'
@@ -391,17 +385,15 @@
   >>> with open('out.txt', 'w') as f:
   >>>     f.write(repr(decoded_data))
 ```
 
 The `decode` function has a `geojson` option which enforces a GeoJson RFC7946 compatible result. Its default value
 is `True`. To enforce the behaviour of versions <2.0.0, please use `geojson=False`.
 
-
-Use native protobuf library for performance
-------------------------------------------
+## Use native protobuf library for performance
 
 The c++ implementation of the underlying protobuf library is more performant than the pure python one. Depending on your operating system, you might need to [compile the C++ library](https://github.com/google/protobuf/tree/master/python#c-implementation) or install it.
 
 Since May 6, 2022, the Python `profobuf` library is based on the udp library and thus, the generated Python code
 requires `protoc` 3.19.0 or newer. Cf. [here](https://developers.google.com/protocol-buffers/docs/news/2022-05-06). On
 debian Bullseye, the version of `protoc` available in the package registry is too old. Please install it from [protobuf
 +GitHub repository](https://github.com/protocolbuffers/protobuf/releases).
@@ -415,12 +407,11 @@
      $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=cpp
      $ export PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION_VERSION=2
 
 and then:
 
     $ protoc -I=mapbox_vector_tile/Mapbox/ --python_out=mapbox_vector_tile/Mapbox/ mapbox_vector_tile/Mapbox/vector_tile.proto
 
-Changelog
----------
+## Changelog
 
 Click [here](https://github.com/tilezen/mapbox-vector-tile/blob/master/CHANGELOG.md) to see what changed over time in various versions.
```

