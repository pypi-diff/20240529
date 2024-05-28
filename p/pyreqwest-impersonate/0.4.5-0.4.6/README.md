# Comparing `tmp/pyreqwest_impersonate-0.4.5.tar.gz` & `tmp/pyreqwest_impersonate-0.4.6.tar.gz`

## Comparing `pyreqwest_impersonate-0.4.5.tar` & `pyreqwest_impersonate-0.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.5/Cargo.toml
--rw-r--r--   0     1001      127     8780 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      766 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/.gitignore
--rw-r--r--   0     1001      127     8546 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/README.md
--rw-r--r--   0     1001      127      343 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/README.md
--rw-r--r--   0     1001      127     3484 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3719 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/generate_image.py
--rw-r--r--   0     1001      127      144 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/requirements.txt
--rw-r--r--   0     1001      127      990 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/server.py
--rw-r--r--   0     1001      127   112327 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark.jpg
--rw-r--r--   0     1001      127    29872 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/src/response.rs
--rw-r--r--   0     1001      127     6232 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/tests/test_client.py
--rw-r--r--   0     1001      127     8287 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/tests/test_defs.py
--rw-r--r--   0     1001      127    41306 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     9615 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.6/Cargo.toml
+-rw-r--r--   0     1001      127     8719 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/.gitignore
+-rw-r--r--   0     1001      127     8566 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/README.md
+-rw-r--r--   0     1001      127      343 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3748 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark/generate_image.py
+-rw-r--r--   0     1001      127      144 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark/server.py
+-rw-r--r--   0     1001      127   112288 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/benchmark.jpg
+-rw-r--r--   0     1001      127    29872 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/src/response.rs
+-rw-r--r--   0     1001      127     6232 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/tests/test_client.py
+-rw-r--r--   0     1001      127     8287 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/tests/test_defs.py
+-rw-r--r--   0     1001      127    41502 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-28 23:50:30.000000 pyreqwest_impersonate-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     9635 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.6/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.4.5/Cargo.toml` & `pyreqwest_impersonate-0.4.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.4.5"
+version = "0.4.6"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `pyreqwest_impersonate-0.4.5/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.6/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             target: x86_64
           - runner: ubuntu-latest
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.12'
+          python-version: '3.8'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist --zig
           sccache: 'true'
@@ -81,15 +81,15 @@
             target: x86_64
           - runner: ubuntu-latest
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.12'
+          python-version: '3.8'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist --zig
           sccache: 'true'
@@ -134,15 +134,15 @@
         platform:
           - runner: windows-latest
             target: x64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.12'
+          python-version: '3.8'
           architecture: ${{ matrix.platform.target }}
       - name: Install nasm
         run: choco install nasm
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           rust-toolchain: stable
@@ -164,43 +164,42 @@
           pytest
 
   macos:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
-          - runner: macos-latest
+          - runner: macos-12
             target: x86_64
           - runner: macos-14
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.12'
+          python-version: '3.8'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
-      #- name: pytest
-      #  if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
-      #  shell: bash
-      #  run: |
-      #    set -e
-      #    pip install pyreqwest_impersonate --find-links dist --force-reinstall
-      #    pip install pytest
-      #    pytest
+      - name: pytest
+        shell: bash
+        run: |
+          set -e
+          pip install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
+          pip install pytest
+          pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
@@ -213,15 +212,15 @@
           name: wheels-sdist
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
+    needs: [linux, musllinux, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
@@ -235,15 +234,15 @@
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [release]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
-          python-version: '3.12'
+          python-version: '3.8'
       - name: Install dependencies
         run: |
           sleep 30  # Wait for the package to be available on PyPI
           python -m pip install --upgrade pip
           pip install -r benchmark/requirements.txt
       - name: Start Uvicorn server
         run: |
```

### Comparing `pyreqwest_impersonate-0.4.5/.gitignore` & `pyreqwest_impersonate-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/README.md` & `pyreqwest_impersonate-0.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_ios_16.5","safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16",
-                "safari_16.5","safari_17.2.1","safari_17.4.1"
+            Safari: "safari_ios_16.5","safari_ios_17.2","safari_ios_17.4.1","safari_15.3","safari_15.5","safari_15.6.1",
+                "safari_16","safari_16.5","safari_17.2.1","safari_17.4.1"
             OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
             Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
```

### Comparing `pyreqwest_impersonate-0.4.5/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.6/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/benchmark/generate_image.py` & `pyreqwest_impersonate-0.4.6/benchmark/generate_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,8 +92,8 @@
 ax3.set_ylabel('Time (s)')
 ax3.set_title('Performance comparison. Threads: 32. Requests: 2000. Response: gzip, utf-8, size 5Kb|50Kb|200Kb')
 ax3.set_xticks(x3 + 3*width - width/2) # Adjust the x-ticks to be after the 3rd bar, moved 0.5 bar width to the left
 ax3.set_xticklabels(names)
 ax3.legend(loc='upper left', ncols=6, prop={'size': 8})
 
 # Save the plot to a file
-plt.savefig('benchmark.jpg', format='jpg')
+plt.savefig('benchmark.jpg', format='jpg', dpi=80, bbox_inches='tight')
```

### Comparing `pyreqwest_impersonate-0.4.5/benchmark/server.py` & `pyreqwest_impersonate-0.4.6/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/benchmark.jpg` & `pyreqwest_impersonate-0.4.6/benchmark.jpg`

 * *Files 13% similar despite different names*

#### Image content

```diff
@@ -1,21 +1,21 @@
    ;:;;@88888X88888S8888X%X888@8@88@88@S88@88X888@@X8@@8;;::
- ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %: .8:% %
+ ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %: .8;% %
 S:;t      .           ..     .  .          .      S8 : X%8 t
-8.:%  . .    .    .S8   ;; .     .  .  .S .  %t . S8   @8S %
-S ;%  .:S;8  .S ;;%8@  t8 . .t 8  .t S8S8X.%X @ t8SX :8 8X.t
-  :% XX t8 8SS;S S:88..S: @:.8@ @8. %88 %8@88:SSX8 @8 .888.t
-  ;;;:;SX@8X8X%:tt%SX88X%888X88X8888XX@8X888XSt.;88888@ttt;:
-   ;:;;@88888@88888S88@88@S@88X8@88@888%8@@88@8888@S8@X@t:;:
- ..88;XS:S8tXS%tXtS%X;88@%SSS:@SS%SXt;8tS%X@X...   .. .8XS %
-S;tt  .. .            ::     .   .  .   .       .   . .%8% t
-8t%%      .  .          :..    .     .      .8S   .    S8X.%
-S t%  .  : . SX.   ;t..;S; .     ..% ..t8X.t% 8. .;:8 8 8t.t
-  :% tX8@X%8%XtX@%;88X S8S;8@@:8S8:8Xt;8888@@:S;@:@8XS88 X t
- .;;;;tS8X8@8Xt;:%S88888S888888888@8@XX8@@8@XS;;;88@8S8%;;;:
-   ;:;X88888888@8@8%88%8888X@88S88@@@88X8@X8@S88X8S8@8@X%;;:
- ;%88;SX.:8.XSSt8;%%X:88@SXS%:8SS%XStt@%X%X@S.......   8%S t
-S.:t   .              .:    . .      .        .    .  .S8S %
-8;;%   .     :t       . .8:  .  .  .   . .  .%:   . .  %8S.%
-S %%   . ;. %t8%. :;%888.@.       .t .:%% :%@.8. .: 8 St8t.t
-  :t.tXXSX:8.88X;.888X888%;8@@%8X8  t;t;%888@88:8.88X 88.X %
-  ;;;;tSX88@@X;::tX8@@XS:88888888888@XX8@@888@%;t88X8X@%;;;:
+8.:%  . .    .    .t%   ::.       .   . S .  tt . S8   @8%.t
+S ;%  .:S;8  :X .:S88  t@.  .t.@  :t.%8S8@.;X @ ;8X8 .8 8X.%
+  :% X@ t8 8SX;S S:88;.S. @:.8@ @8. t8@ %8@88:8X%X88%:@88@ t
+  ;;;:;XX@8X8Xt:tt%%X88X%888@88@8888XX@8X888XSt:.@X88X8S:;;;
+   ;:;;@88888@88888%88@88XS@88X8@88X888%8@888888@@@X88@Xt;::
+ . 88tX%:S8tXS%tS%%%@;88@%SSS:@SSSXS;;8tS%S@X.:   .  . 8@S.t
+S;%t  .. .            .:  .  .     .            .  .  .%8% %
+8t%%     .  .         . :.     . .    .  .  .X%    .   %8S.%
+S t%  .  ..  XX.   ;t..;t; .      .t...t88:;% @.. ::8 8.8% t
+  :% tX8SXS8%XtX8%;88% %8S;8@@:@%8:8Xt;888XX@8@;8t88@X@@ X.t
+ .;;;;tS8X8X8@t;;tS88888S8888@8888@8@XS8888@8tt:t88@8S8S;;;:
+   :;:X88888888@8@8%88S8888X@88S8@@@@88X8@S@@S88X8X888@X%;::
+ ;%88tSX.:8.XS%t8;%%X.88@SXS%:8SS%XStt@%X%%XS......    8SS.t
+S..t   .      .       .:    . .      .      . .   .  . %8S %
+8;t%   .     :;      .  %8.  .  .  .   . .  ..% .  .  .%8S.t
+S %%    .:. %t8% ..;%888. t      ..% .:SX :;@.@.  : 8 X 8%.t
+  :t.tXSXS:@.88X; 888X888X;88X%8X8 %%;;@8888@.S;8:88@ 88.@ t
+  ;;:;tS@88@@X;::tX8X@XS;888X@8888@8@XX8X@88@S;;t88X8X@S;;;:
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 100
 Y resolution: 100
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 18791
+Number of unique colors: 18891
 Comment: 
 EXIF data:
```

### Comparing `pyreqwest_impersonate-0.4.5/src/lib.rs` & `pyreqwest_impersonate-0.4.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/src/response.rs` & `pyreqwest_impersonate-0.4.6/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/tests/test_client.py` & `pyreqwest_impersonate-0.4.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/tests/test_defs.py` & `pyreqwest_impersonate-0.4.6/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/Cargo.lock` & `pyreqwest_impersonate-0.4.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+checksum = "6e4503c46a5c0c7844e948c9a4d6acd9f50cccb4de1c48eb9e291ea17470c678"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -58,24 +58,30 @@
  "futures-core",
  "memchr",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
+name = "atomic-waker"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
+
+[[package]]
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.71"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -160,32 +166,32 @@
 name = "brotli"
 version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74f7971dbd9326d58187408ab83117d8ac1bb9c17b085fdacd1cf2f598719b6b"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
- "brotli-decompressor 4.0.0",
+ "brotli-decompressor 4.0.1",
 ]
 
 [[package]]
 name = "brotli-decompressor"
 version = "2.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "4.0.0"
+version = "4.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6221fe77a248b9117d431ad93761222e1cf8ff282d9d1d5d9f53d6299a1cf76"
+checksum = "9a45bd2e4095a8b518033b128020dd4a55aab1c0a381ba4404a472630f4bc362"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
@@ -197,17 +203,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.97"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -218,17 +224,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clang-sys"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
+checksum = "a483f3cbf7cec2e153d424d0e92329d816becc6421389bd494375c6065921b9b"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
@@ -282,17 +288,17 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
@@ -300,17 +306,17 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
@@ -412,35 +418,35 @@
  "futures-task",
  "pin-project-lite",
  "pin-utils",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2_imp"
-version = "0.4.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "733220cab3b696d7089c92685e883eeac4d217ce4e6026ed36bece698ea06efe"
+checksum = "0b6449767c80c16a3c6c5c6bddb20fb64637ab7b77c9c7e0e0d78d496021af43"
 dependencies = [
+ "atomic-waker",
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
- "futures-util",
  "http",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
@@ -609,17 +615,17 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
@@ -693,17 +699,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -729,32 +735,32 @@
 name = "num-conv"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
 
 [[package]]
 name = "object"
-version = "0.32.2"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "b8ec7ab813848ba4522158d5517a6093db1ded27575b070f4177b8d12b41db5e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -797,17 +803,17 @@
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.82"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psl-types"
 version = "2.0.11"
@@ -886,15 +892,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.4.5"
+version = "0.4.6"
 dependencies = [
  "encoding_rs",
  "indexmap",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
@@ -1026,26 +1032,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1100,17 +1106,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.63"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1138,26 +1144,26 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `pyreqwest_impersonate-0.4.5/pyproject.toml` & `pyreqwest_impersonate-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.5/PKG-INFO` & `pyreqwest_impersonate-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.4.5
+Version: 0.4.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -83,16 +83,16 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_ios_16.5","safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16",
-                "safari_16.5","safari_17.2.1","safari_17.4.1"
+            Safari: "safari_ios_16.5","safari_ios_17.2","safari_ios_17.4.1","safari_15.3","safari_15.5","safari_15.6.1",
+                "safari_16","safari_16.5","safari_17.2.1","safari_17.4.1"
             OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
             Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
```

