# Comparing `tmp/QuikUI-0.1.0a2.tar.gz` & `tmp/QuikUI-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuikUI-0.1.0a2.tar", last modified: Mon May 27 16:14:00 2024, max compression
+gzip compressed data, was "QuikUI-0.1.0b0.tar", last modified: Tue May 28 21:17:08 2024, max compression
```

## Comparing `QuikUI-0.1.0a2.tar` & `QuikUI-0.1.0b0.tar`

### file list

```diff
@@ -1,41 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.830855 QuikUI-0.1.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.822855 QuikUI-0.1.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.822855 QuikUI-0.1.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/QuikUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 16:14:00.000000 QuikUI-0.1.0a2/QuikUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/quikui/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:14:00.826855 QuikUI-0.1.0a2/quikui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Anchor.html
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/AppBase.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Button.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/CheckboxInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Div.html
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Form.html
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/FormInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Image.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/List.html
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Page.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/RadioInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/SelectionInput.html
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/templates/Span.html
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/quikui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:14:00.830855 QuikUI-0.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:13:45.000000 QuikUI-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.388604 QuikUI-0.1.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.388604 QuikUI-0.1.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/QuikUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-28 21:17:08.000000 QuikUI-0.1.0b0/QuikUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-28 21:17:08.000000 QuikUI-0.1.0b0/QuikUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:17:08.000000 QuikUI-0.1.0b0/QuikUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 21:17:08.000000 QuikUI-0.1.0b0/QuikUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 21:17:08.000000 QuikUI-0.1.0b0/QuikUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/example/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/example/templates/AppBase.html
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/example/templates/CustomPage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/quikui/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17936 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/quikui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/Anchor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/CheckboxInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/FormInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/Heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/Image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/RadioInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/SelectionInput.html
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/_MultiItemComponent.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/templates/_SingleContentComponent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/quikui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:17:08.392604 QuikUI-0.1.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:16:54.000000 QuikUI-0.1.0b0/setup.py
```

### Comparing `QuikUI-0.1.0a2/.github/workflows/publish.yaml` & `QuikUI-0.1.0b0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a2/LICENSE` & `QuikUI-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a2/pyproject.toml` & `QuikUI-0.1.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `QuikUI-0.1.0a2/quikui/dependencies.py` & `QuikUI-0.1.0b0/quikui/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,11 +17,11 @@
         async with request.form() as form_data:
             model_data = unflatten(form_data)
 
         try:
             return Model.model_validate(model_data)
         except ValidationError as e:
             raise RequestValidationError(
-                e.errors(include_input=False, include_url=False, include_context=False)
+                e.errors(include_input=True, include_url=True, include_context=True)
             )
 
     return handle_request
```

### Comparing `QuikUI-0.1.0a2/quikui/templates/AppBase.html` & `QuikUI-0.1.0b0/example/templates/AppBase.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+{# This is recommended for structuring your application pages #}
 <!DOCTYPE html>
 <html lang="en">
 
   <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
 
+    {# You can use any design system you want #}
     <link
       href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css"
       rel="stylesheet"
       integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3"
       crossorigin="anonymous">
 
     {% block header %} {% endblock %}
@@ -18,20 +20,22 @@
   <body class="d-flex flex-column h-100">
     <main class="flex-shrink-0">
       <div class="container py-5">
         {% block content %} {% endblock content %}
       </div>
     </main>
 
+    {# You can use any design system you want #}
     <script
       src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
       integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
       crossorigin="anonymous">
     </script>
 
+    {# You can use any JS modules you want #}
     <script
       src="https://unpkg.com/htmx.org@1.9.10"
       integrity="sha384-D1Kt99CQMDuVetoL1lrYwg5t+9QdHe7NLX/SoJYkXDFfX37iInKRy5xLSi8nO7UC"
       crossorigin="anonymous">
     </script>
 
     {% block script %} {% endblock script %}
```

#### html2text {}

```diff
@@ -1,3 +1,7 @@
+{# This is recommended for structuring your application pages #}
+{# You can use any design system you want #}
 {% block header %} {% endblock %}
 {% block content %} {% endblock content %}
+{# You can use any design system you want #}
+{# You can use any JS modules you want #}
 {% block script %} {% endblock script %}
```

### Comparing `QuikUI-0.1.0a2/quikui/utils.py` & `QuikUI-0.1.0b0/quikui/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,40 @@
 from fastapi.concurrency import run_in_threadpool
 
 P = ParamSpec("P")
 T = TypeVar("T")
 MaybeAsyncFunc = Callable[P, T] | Callable[P, Coroutine[Any, Any, T]]
 
 
-def get_hx_request(
-    request: Request, hx_request: Annotated[str | None, Header()] = None
+def html_response_requested(
+    request: Request,
+    hx_request: Annotated[bool, Header()] = False,
+    content_type: Annotated[str | None, Header()] = None,
+    raw_accept_header: Annotated[str | None, Header(alias="accept")] = None,
 ) -> Request | None:
-    """
-    FastAPI dependency that returns the current request if it is an HTMX one,
-    i.e. it contains an `"HX-Request: true"` header.
-    """
-    return request if hx_request == "true" else None
+    if hx_request:
+        # We definitely know that HX-Request=true headers means return html
+        return request
+
+    elif content_type and content_type == "application/json":
+        # Assume that if the request is JSON, the response should be too
+        # NOTE: htmx never does this
+        return None
+
+    elif raw_accept_header and (
+        accepted_types := list(t.strip() for t in raw_accept_header.split(","))
+    ):
+        if any(t.startswith("text/html") for t in accepted_types):
+            return request  # We have determined this is expecting HTML back
+
+    # else: We haven't determined (according to above heuristics) that HTML is requested
+    return None
 
 
-DependsHXRequest = Annotated[Request | None, Depends(get_hx_request)]
+DependsHtmlResponse = Annotated[Request | None, Depends(html_response_requested)]
 
 
 def append_to_signature(func: Callable, *params: inspect.Parameter) -> Callable:
     """
     Appends the given parameters to the *end* of the signature of the given function.
 
     Notes:
```

