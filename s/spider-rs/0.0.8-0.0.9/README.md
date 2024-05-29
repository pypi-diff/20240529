# Comparing `tmp/spider_rs-0.0.8.tar.gz` & `tmp/spider_rs-0.0.9.tar.gz`

## Comparing `spider_rs-0.0.8.tar` & `spider_rs-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 spider_rs-0.0.8/Cargo.toml
--rw-r--r--   0      501       20      118 2023-11-26 15:09:47.000000 spider_rs-0.0.8/.cargo/config.toml
--rw-r--r--   0      501       20      608 2023-11-28 15:02:16.000000 spider_rs-0.0.8/.github/workflows/book.yml
--rw-r--r--   0      501       20     3309 2023-12-03 23:07:06.000000 spider_rs-0.0.8/.gitignore
--rw-r--r--   0      501       20     1076 2023-12-08 15:00:23.000000 spider_rs-0.0.8/LICENSE.txt
--rw-r--r--   0      501       20     1658 2023-12-09 14:47:36.000000 spider_rs-0.0.8/README.md
--rw-r--r--   0      501       20      460 2023-12-09 04:56:24.000000 spider_rs-0.0.8/bench/README.md
--rw-r--r--   0      501       20      883 2023-12-09 05:03:00.000000 spider_rs-0.0.8/bench/scrappy.py
--rw-r--r--   0      501       20      382 2023-12-09 04:50:17.000000 spider_rs-0.0.8/bench/spider.py
--rw-r--r--   0      501       20        5 2023-11-28 14:28:08.000000 spider_rs-0.0.8/book/.gitignore
--rw-r--r--   0      501       20      278 2023-12-08 13:57:40.000000 spider_rs-0.0.8/book/book.toml
--rw-r--r--   0      501       20      567 2023-12-09 15:06:25.000000 spider_rs-0.0.8/book/src/README.md
--rw-r--r--   0      501       20      201 2023-12-09 14:40:47.000000 spider_rs-0.0.8/book/src/SUMMARY.md
--rw-r--r--   0      501       20      160 2023-11-29 17:33:27.000000 spider_rs-0.0.8/book/src/env.md
--rw-r--r--   0      501       20       88 2023-12-08 16:00:47.000000 spider_rs-0.0.8/book/src/getting-started.md
--rw-r--r--   0      501       20      219 2023-12-08 16:01:20.000000 spider_rs-0.0.8/book/src/simple.md
--rw-r--r--   0      501       20     5338 2023-12-09 16:52:43.000000 spider_rs-0.0.8/book/src/website.md
--rw-r--r--   0      501       20      160 2023-12-08 15:02:34.000000 spider_rs-0.0.8/examples/basic.py
--rw-r--r--   0      501       20      263 2023-12-09 15:02:20.000000 spider_rs-0.0.8/examples/builder.py
--rw-r--r--   0      501       20      454 2023-12-09 16:51:49.000000 spider_rs-0.0.8/examples/stop.py
--rw-r--r--   0      501       20      361 2023-12-09 14:45:55.000000 spider_rs-0.0.8/examples/subscription.py
--rw-r--r--   0      501       20      195 2023-12-09 14:39:19.000000 spider_rs-0.0.8/examples/website.py
--rw-r--r--   0      501       20       32 2023-11-26 15:09:47.000000 spider_rs-0.0.8/rustfmt.toml
--rw-r--r--   0      501       20      784 2023-12-09 14:13:00.000000 spider_rs-0.0.8/src/lib.rs
--rw-r--r--   0      501       20     1323 2023-12-09 14:05:46.000000 spider_rs-0.0.8/src/npage.rs
--rw-r--r--   0      501       20      254 2023-12-08 14:38:37.000000 spider_rs-0.0.8/src/nwebsite.rs
--rw-r--r--   0      501       20     2333 2023-12-09 02:55:15.000000 spider_rs-0.0.8/src/page.rs
--rw-r--r--   0      501       20      929 2023-12-09 13:57:44.000000 spider_rs-0.0.8/src/shortcut.rs
--rw-r--r--   0      501       20    20374 2023-12-09 16:53:16.000000 spider_rs-0.0.8/src/website.rs
--rw-r--r--   0      501       20    62102 2023-12-09 16:53:04.000000 spider_rs-0.0.8/Cargo.lock
--rw-r--r--   0      501       20      310 2023-12-08 14:48:13.000000 spider_rs-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 spider_rs-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 spider_rs-0.0.9/Cargo.toml
+-rw-r--r--   0      501       20      118 2023-11-26 15:09:47.000000 spider_rs-0.0.9/.cargo/config.toml
+-rw-r--r--   0      501       20      608 2023-11-28 15:02:16.000000 spider_rs-0.0.9/.github/workflows/book.yml
+-rw-r--r--   0      501       20     3309 2023-12-03 23:07:06.000000 spider_rs-0.0.9/.gitignore
+-rw-r--r--   0      501       20     1076 2023-12-08 15:00:23.000000 spider_rs-0.0.9/LICENSE.txt
+-rw-r--r--   0      501       20     1535 2023-12-10 07:58:14.000000 spider_rs-0.0.9/README.md
+-rw-r--r--   0      501       20      460 2023-12-09 04:56:24.000000 spider_rs-0.0.9/bench/README.md
+-rw-r--r--   0      501       20      883 2023-12-09 05:03:00.000000 spider_rs-0.0.9/bench/scrappy.py
+-rw-r--r--   0      501       20      382 2023-12-09 04:50:17.000000 spider_rs-0.0.9/bench/spider.py
+-rw-r--r--   0      501       20        5 2023-11-28 14:28:08.000000 spider_rs-0.0.9/book/.gitignore
+-rw-r--r--   0      501       20      278 2023-12-08 13:57:40.000000 spider_rs-0.0.9/book/book.toml
+-rw-r--r--   0      501       20      567 2023-12-09 15:06:25.000000 spider_rs-0.0.9/book/src/README.md
+-rw-r--r--   0      501       20      201 2023-12-09 14:40:47.000000 spider_rs-0.0.9/book/src/SUMMARY.md
+-rw-r--r--   0      501       20      160 2023-11-29 17:33:27.000000 spider_rs-0.0.9/book/src/env.md
+-rw-r--r--   0      501       20       88 2023-12-08 16:00:47.000000 spider_rs-0.0.9/book/src/getting-started.md
+-rw-r--r--   0      501       20      219 2023-12-08 16:01:20.000000 spider_rs-0.0.9/book/src/simple.md
+-rw-r--r--   0      501       20     5338 2023-12-09 16:52:43.000000 spider_rs-0.0.9/book/src/website.md
+-rw-r--r--   0      501       20      160 2023-12-08 15:02:34.000000 spider_rs-0.0.9/examples/basic.py
+-rw-r--r--   0      501       20      263 2023-12-09 15:02:20.000000 spider_rs-0.0.9/examples/builder.py
+-rw-r--r--   0      501       20      454 2023-12-09 16:51:49.000000 spider_rs-0.0.9/examples/stop.py
+-rw-r--r--   0      501       20      451 2023-12-09 17:22:06.000000 spider_rs-0.0.9/examples/subscription.py
+-rw-r--r--   0      501       20      270 2023-12-09 17:20:39.000000 spider_rs-0.0.9/examples/website.py
+-rw-r--r--   0      501       20       32 2023-11-26 15:09:47.000000 spider_rs-0.0.9/rustfmt.toml
+-rw-r--r--   0      501       20      784 2023-12-09 14:13:00.000000 spider_rs-0.0.9/src/lib.rs
+-rw-r--r--   0      501       20     1323 2023-12-09 14:05:46.000000 spider_rs-0.0.9/src/npage.rs
+-rw-r--r--   0      501       20      254 2023-12-08 14:38:37.000000 spider_rs-0.0.9/src/nwebsite.rs
+-rw-r--r--   0      501       20     2333 2023-12-09 02:55:15.000000 spider_rs-0.0.9/src/page.rs
+-rw-r--r--   0      501       20      929 2023-12-09 13:57:44.000000 spider_rs-0.0.9/src/shortcut.rs
+-rw-r--r--   0      501       20    23712 2023-12-15 17:20:51.000000 spider_rs-0.0.9/src/website.rs
+-rw-r--r--   0      501       20    62101 2023-12-15 17:21:04.000000 spider_rs-0.0.9/Cargo.lock
+-rw-r--r--   0      501       20      310 2023-12-08 14:48:13.000000 spider_rs-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 spider_rs-0.0.9/PKG-INFO
```

### Comparing `spider_rs-0.0.8/Cargo.toml` & `spider_rs-0.0.9/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 edition = "2021"
 name = "spider_rs"
-version = "0.0.8"
+version = "0.0.9"
 description = "The fastest web crawler written in Rust ported to nodejs."
 repository = "https://github.com/spider-rs/spider-nodejs"
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 compact_str = "0.7.1"
 indexmap = "2.1.0"
 num_cpus = "1.16.0"
 serde = "1.0.193"
 serde_json = "1.0.108"
-spider = { version = "1.50.20", features = ["budget", "cron", "regex", "cookies", "socks", "chrome", "control" ] }
+spider = { version = "1.70.4", features = ["budget", "cron", "regex", "cookies", "socks", "chrome", "control", "smart", "chrome_intercept" ] }
 pyo3 = { version = "0.20.0", features = ["extension-module"] }
 pyo3-asyncio = { version = "0.20", features = ["attributes", "tokio-runtime"] }
 
 [target.x86_64-unknown-linux-gnu.dependencies]
 openssl-sys = { version = "0.9.96", features = ["vendored"] }
 openssl = { version = "0.10.60", features = ["vendored"] }
```

### Comparing `spider_rs-0.0.8/.github/workflows/book.yml` & `spider_rs-0.0.9/.github/workflows/book.yml`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/.gitignore` & `spider_rs-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/LICENSE.txt` & `spider_rs-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/README.md` & `spider_rs-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -62,14 +62,14 @@
 1. `maturin develop`
 
 ## Benchmarks
 
 View [bench](./bench/) to see the results. The library should run faster than scrappy by at least 2x for normal workflows and up to 100,000x for large websites.
 The speed increases drastically as we harness isolated concurrency from Rust.
 
-## Todo
+## TODO
 
-1. Fix http headers custom assign.
-1. Add better docs.
-1. Fix benchmarks.
+1. Fix stop concurrent crawl.
 
-Once these items are done the base of the module should be complete. Most of the code comes from the initial port to Node.js that was done.
+## Issues
+
+Please submit a Github issue for any issues found.
```

### Comparing `spider_rs-0.0.8/bench/scrappy.py` & `spider_rs-0.0.9/bench/scrappy.py`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/book/src/README.md` & `spider_rs-0.0.9/book/src/README.md`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/book/src/website.md` & `spider_rs-0.0.9/book/src/website.md`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/src/lib.rs` & `spider_rs-0.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/src/npage.rs` & `spider_rs-0.0.9/src/npage.rs`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/src/page.rs` & `spider_rs-0.0.9/src/page.rs`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/src/shortcut.rs` & `spider_rs-0.0.9/src/shortcut.rs`

 * *Files identical despite different names*

### Comparing `spider_rs-0.0.8/src/website.rs` & `spider_rs-0.0.9/src/website.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::{new_page, NPage, BUFFER};
 use compact_str::CompactString;
 use indexmap::IndexMap;
 use pyo3::prelude::*;
-use spider::tokio::task::JoinHandle;
 use spider::tokio::select;
+use spider::tokio::task::JoinHandle;
 use spider::utils::shutdown;
 use std::time::Duration;
 
 /// a website holding the inner spider::website::Website from Rust fit for python.
 #[pyclass]
 pub struct Website {
   /// the website from spider.
@@ -268,15 +268,14 @@
                   // println!("Sync receiver droped");
               }
               _ = f2 => {
                   // println!("operation completed");
               }
             }
           });
-          
         }
       }
       _ => {
         if background {
           let mut website = slf.inner.clone();
 
           let crawl_id = match slf.crawl_handles.last() {
@@ -303,14 +302,117 @@
             Ok::<(), ()>(())
           });
         }
       }
     };
   }
 
+  /// crawl a website smart mode
+  pub fn crawl_smart(
+    mut slf: PyRefMut<'_, Self>,
+    on_page_event: Option<PyObject>,
+    background: Option<bool>,
+  ) {
+    // only run in background if on_page_event is handled for streaming.
+    let background = background.is_some() && background.unwrap_or_default();
+    let raw_content = slf.raw_content;
+
+    if background {
+      slf.running_in_background = background;
+    }
+
+    match on_page_event {
+      Some(callback) => {
+        if background {
+          let mut website = slf.inner.clone();
+          let mut rx2 = website
+            .subscribe(*BUFFER / 2)
+            .expect("sync feature should be enabled");
+
+          let handle = spider::tokio::spawn(async move {
+            while let Ok(res) = rx2.recv().await {
+              let page = new_page(&res, raw_content);
+              Python::with_gil(|py| {
+                let _ = callback.call(py, (page,), None);
+              });
+            }
+          });
+
+          let crawl_id = match slf.crawl_handles.last() {
+            Some(handle) => handle.0 + 1,
+            _ => 0,
+          };
+
+          let crawl_handle = spider::tokio::spawn(async move {
+            website.crawl_smart().await;
+          });
+
+          let id = match slf.subscription_handles.last() {
+            Some(handle) => handle.0 + 1,
+            _ => 0,
+          };
+
+          slf.crawl_handles.insert(crawl_id, crawl_handle);
+          slf.subscription_handles.insert(id, handle);
+        } else {
+          let mut rx2 = slf
+            .inner
+            .subscribe(*BUFFER / 2)
+            .expect("sync feature should be enabled");
+
+          let py: Python<'_> = slf.py();
+          let rt = pyo3_asyncio::tokio::get_runtime();
+
+          let f1 = async {
+            while let Ok(res) = rx2.recv().await {
+              let page = new_page(&res, raw_content);
+              let _ = callback.call(py, (page,), None);
+            }
+          };
+
+          let f2 = async {
+            slf.inner.crawl_smart().await;
+          };
+
+          rt.block_on(async move {
+            select! {
+              _ = f1 => {
+                  // println!("Sync receiver droped");
+              }
+              _ = f2 => {
+                  // println!("operation completed");
+              }
+            }
+          });
+        }
+      }
+      _ => {
+        if background {
+          let mut website = slf.inner.clone();
+
+          let crawl_id = match slf.crawl_handles.last() {
+            Some(handle) => handle.0 + 1,
+            _ => 0,
+          };
+
+          let crawl_handle = spider::tokio::spawn(async move {
+            website.crawl_smart().await;
+          });
+
+          slf.crawl_handles.insert(crawl_id, crawl_handle);
+        } else {
+          let _ = pyo3_asyncio::tokio::get_runtime().block_on(async move {
+            slf.inner.crawl_smart().await;
+            Ok::<(), ()>(())
+          });
+        }
+      }
+    };
+  }
+
   /// scrape a website
   pub fn scrape(
     mut slf: PyRefMut<'_, Self>,
     on_page_event: Option<PyObject>,
     background: Option<bool>,
     headless: Option<bool>,
   ) {
@@ -384,18 +486,18 @@
               slf.inner.scrape_raw().await;
             }
           };
 
           rt.block_on(async move {
             select! {
               _ = f1 => {
-                  println!("Sync receiver droped");
+                  // println!("Sync receiver droped");
               }
               _ = f2 => {
-                  println!("operation completed");
+                  // println!("operation completed");
               }
             }
           });
         }
       }
       _ => {
         if background {
@@ -702,14 +804,26 @@
         }
         _ => None,
       });
 
     slf
   }
 
+  /// Use network interception for the request to only allow content that matches the host. If the content is from a 3rd party it needs to be part of our include list.
+  pub fn with_chrome_intercept(
+    mut slf: PyRefMut<'_, Self>,
+    chrome_intercept: bool,
+    block_images: bool,
+  ) -> PyRefMut<'_, Self> {
+    slf
+      .inner
+      .with_chrome_intercept(chrome_intercept, block_images);
+    slf
+  }
+
   /// Setup cron jobs to run
   pub fn with_cron(
     mut slf: PyRefMut<'_, Self>,
     cron_str: String,
     cron_type: Option<String>,
   ) -> PyRefMut<'_, Self> {
     slf.inner.with_cron(
```

### Comparing `spider_rs-0.0.8/Cargo.lock` & `spider_rs-0.0.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1774,17 +1774,17 @@
 dependencies = [
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "spider"
-version = "1.50.20"
+version = "1.70.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6d5d6c16bb91eb4dcf5f5f0d6a1c89bc66261732ac31a18df9c566d22cd0f85"
+checksum = "bc7e744e6b1fd4b524bfb4f4b3406871e07fcd066cf5a12b3c3f795ae442fe7a"
 dependencies = [
  "ahash",
  "async-trait",
  "async_job",
  "bytes",
  "case_insensitive_string",
  "chromiumoxide",
@@ -1809,15 +1809,15 @@
  "tokio",
  "tokio-stream",
  "url",
 ]
 
 [[package]]
 name = "spider_rs"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "compact_str",
  "indexmap",
  "num_cpus",
  "openssl",
  "openssl-sys",
  "pyo3",
@@ -2028,17 +2028,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.34.0"
+version = "1.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0c014766411e834f7af5b8f4cf46257aab4036ca95e9d2c144a10f59ad6f5b9"
+checksum = "841d45b238a16291a4e1584e61820b8ae57d696cc5015c459c229ccc6990cc1c"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
```

### Comparing `spider_rs-0.0.8/PKG-INFO` & `spider_rs-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider_rs
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.txt
 Summary: The fastest web crawler written in Rust ported to nodejs.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -74,15 +74,14 @@
 1. `maturin develop`
 
 ## Benchmarks
 
 View [bench](./bench/) to see the results. The library should run faster than scrappy by at least 2x for normal workflows and up to 100,000x for large websites.
 The speed increases drastically as we harness isolated concurrency from Rust.
 
-## Todo
+## TODO
 
-1. Fix http headers custom assign.
-1. Add better docs.
-1. Fix benchmarks.
+1. Fix stop concurrent crawl.
 
-Once these items are done the base of the module should be complete. Most of the code comes from the initial port to Node.js that was done.
+## Issues
 
+Please submit a Github issue for any issues found.
```

