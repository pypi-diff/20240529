# Comparing `tmp/fieldenum-0.0.1.tar.gz` & `tmp/fieldenum-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fieldenum-0.0.1.tar", max compression
+gzip compressed data, was "fieldenum-0.1.0.tar", max compression
```

## Comparing `fieldenum-0.0.1.tar` & `fieldenum-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0      411 2024-05-21 13:14:28.643224 fieldenum-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      814 2024-05-21 13:20:58.119251 fieldenum-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-21 13:14:18.785108 fieldenum-0.0.1/src/fieldenum/__init__.py
--rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 fieldenum-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1169 2024-05-29 13:40:58.552524 fieldenum-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2024-05-29 12:53:12.406371 fieldenum-0.1.0/README.md
+-rw-r--r--   0        0        0       85 2024-05-25 05:33:16.009348 fieldenum-0.1.0/src/fieldenum/__init__.py
+-rw-r--r--   0        0        0    13882 2024-05-29 13:32:42.148368 fieldenum-0.1.0/src/fieldenum/_fieldenum.py
+-rw-r--r--   0        0        0     1973 2024-05-27 15:40:55.050130 fieldenum-0.1.0/src/fieldenum/_utils.py
+-rw-r--r--   0        0        0     8144 2024-05-29 13:17:23.700130 fieldenum-0.1.0/src/fieldenum/enums.py
+-rw-r--r--   0        0        0      552 2024-05-29 12:17:55.706204 fieldenum-0.1.0/src/fieldenum/exceptions.py
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 fieldenum-0.1.0/PKG-INFO
```

### Comparing `fieldenum-0.0.1/README.md` & `fieldenum-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # fieldenum
 
-Rust-like fielded Enum in Python
+Rust-like fielded Enums in Python
+
+**[한국어로 보기](docs/README-ko.md)**
 
 ## Examples
 
 ```python
-from fieldenum import fieldenum, Item
+from fieldenum import fieldenum, Unit, Variant
 
-# define
 @fieldenum
 class Message:
-    Quit = Item()
-    Move = Item(x=int, y=int)
-    Write = Item(str)
-    ChangeColor = Item(int, int, int)
+    Quit = Unit
+    Move = Variant(x=int, y=int)
+    Write = Variant(str)
+    ChangeColor = Variant(int, int, int)
 
 # Corresponding code in Rust:
 # enum Message {
 #     Quit,
 #     Move { x: i32, y: i32 },
 #     Write(String),
 #     ChangeColor(i32, i32, i32),
 # }
 
 
 # usage
-message = Message.Quit()
+message = Message.Quit
 message = Message.Move(x=1, y=2)
 message = Message.Write("hello, world!")
 message = Message.ChangeColor(256, 256, 0)
 ```
 
 ## Credits
 
 This project is heavily influenced by [Rust's `Enum`](https://doc.rust-lang.org/reference/items/enumerations.html), and also borrows some of its design from [rust_enum](https://github.com/girvel/rust_enum).
+
+## Releases
+
+* 0.1.0: initial release
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

