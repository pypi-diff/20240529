# Comparing `tmp/modular-ai-0.1.0.tar.gz` & `tmp/modular-ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular-ai-0.1.0.tar", last modified: Wed May 29 00:54:21 2024, max compression
+gzip compressed data, was "modular-ai-0.1.1.tar", last modified: Wed May 29 01:00:15 2024, max compression
```

## Comparing `modular-ai-0.1.0.tar` & `modular-ai-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 00:54:21.063014 modular-ai-0.1.0/
--rw-rw-r--   0 hx        (1000) hx        (1000)        0 2024-05-28 20:57:04.000000 modular-ai-0.1.0/LICENSE
--rw-rw-r--   0 hx        (1000) hx        (1000)       17 2024-05-28 22:02:16.000000 modular-ai-0.1.0/MANIFEST.in
--rw-rw-r--   0 hx        (1000) hx        (1000)     4144 2024-05-29 00:54:21.063014 modular-ai-0.1.0/PKG-INFO
--rw-rw-r--   0 hx        (1000) hx        (1000)     3664 2024-05-28 21:22:31.000000 modular-ai-0.1.0/README.md
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 00:54:21.063014 modular-ai-0.1.0/ailib/
--rw-rw-r--   0 hx        (1000) hx        (1000)       91 2024-05-28 21:47:33.000000 modular-ai-0.1.0/ailib/__init__.py
--rw-rw-r--   0 hx        (1000) hx        (1000)     3808 2024-05-28 21:59:49.000000 modular-ai-0.1.0/ailib/ai_models.py
--rw-rw-r--   0 hx        (1000) hx        (1000)     1032 2024-05-28 21:53:02.000000 modular-ai-0.1.0/ailib/models.py
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 00:54:21.063014 modular-ai-0.1.0/modular_ai.egg-info/
--rw-rw-r--   0 hx        (1000) hx        (1000)     4144 2024-05-29 00:54:21.000000 modular-ai-0.1.0/modular_ai.egg-info/PKG-INFO
--rw-rw-r--   0 hx        (1000) hx        (1000)      299 2024-05-29 00:54:21.000000 modular-ai-0.1.0/modular_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)        1 2024-05-29 00:54:21.000000 modular-ai-0.1.0/modular_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)       23 2024-05-29 00:54:21.000000 modular-ai-0.1.0/modular_ai.egg-info/requires.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)       12 2024-05-29 00:54:21.000000 modular-ai-0.1.0/modular_ai.egg-info/top_level.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)       38 2024-05-29 00:54:21.063014 modular-ai-0.1.0/setup.cfg
--rw-rw-r--   0 hx        (1000) hx        (1000)      735 2024-05-29 00:54:05.000000 modular-ai-0.1.0/setup.py
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 00:54:21.063014 modular-ai-0.1.0/tests/
--rw-rw-r--   0 hx        (1000) hx        (1000)        0 2024-05-28 20:57:22.000000 modular-ai-0.1.0/tests/__init__.py
--rw-rw-r--   0 hx        (1000) hx        (1000)     2370 2024-05-28 22:00:03.000000 modular-ai-0.1.0/tests/test_ai_lib.py
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 01:00:15.933721 modular-ai-0.1.1/
+-rw-rw-r--   0 hx        (1000) hx        (1000)        0 2024-05-28 20:57:04.000000 modular-ai-0.1.1/LICENSE
+-rw-rw-r--   0 hx        (1000) hx        (1000)       17 2024-05-28 22:02:16.000000 modular-ai-0.1.1/MANIFEST.in
+-rw-rw-r--   0 hx        (1000) hx        (1000)     4084 2024-05-29 01:00:15.933721 modular-ai-0.1.1/PKG-INFO
+-rw-rw-r--   0 hx        (1000) hx        (1000)     3597 2024-05-29 00:58:21.000000 modular-ai-0.1.1/README.md
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 01:00:15.933721 modular-ai-0.1.1/ailib/
+-rw-rw-r--   0 hx        (1000) hx        (1000)       91 2024-05-28 21:47:33.000000 modular-ai-0.1.1/ailib/__init__.py
+-rw-rw-r--   0 hx        (1000) hx        (1000)     3808 2024-05-28 21:59:49.000000 modular-ai-0.1.1/ailib/ai_models.py
+-rw-rw-r--   0 hx        (1000) hx        (1000)      960 2024-05-29 00:56:47.000000 modular-ai-0.1.1/ailib/models.py
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 01:00:15.933721 modular-ai-0.1.1/modular_ai.egg-info/
+-rw-rw-r--   0 hx        (1000) hx        (1000)     4084 2024-05-29 01:00:15.000000 modular-ai-0.1.1/modular_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 hx        (1000) hx        (1000)      299 2024-05-29 01:00:15.000000 modular-ai-0.1.1/modular_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)        1 2024-05-29 01:00:15.000000 modular-ai-0.1.1/modular_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       33 2024-05-29 01:00:15.000000 modular-ai-0.1.1/modular_ai.egg-info/requires.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       12 2024-05-29 01:00:15.000000 modular-ai-0.1.1/modular_ai.egg-info/top_level.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       38 2024-05-29 01:00:15.933721 modular-ai-0.1.1/setup.cfg
+-rw-rw-r--   0 hx        (1000) hx        (1000)      705 2024-05-29 00:59:45.000000 modular-ai-0.1.1/setup.py
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2024-05-29 01:00:15.933721 modular-ai-0.1.1/tests/
+-rw-rw-r--   0 hx        (1000) hx        (1000)        0 2024-05-28 20:57:22.000000 modular-ai-0.1.1/tests/__init__.py
+-rw-rw-r--   0 hx        (1000) hx        (1000)     2370 2024-05-28 22:00:03.000000 modular-ai-0.1.1/tests/test_ai_lib.py
```

### Comparing `modular-ai-0.1.0/PKG-INFO` & `modular-ai-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,30 @@
-Metadata-Version: 2.1
-Name: modular-ai
-Version: 0.1.0
-Summary: A library for interacting with various AI models
-Home-page: https://github.com/HarveyGW/AILib
-Author: HarveyGW
-Author-email: your_email@example.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AI Model Library
+# Modular AI Library
 
 A Python library that allows you to import and use various AI models easily. This library supports multiple AI model providers, making it straightforward to switch between different models without writing initialisation code each time.
 
 ## Features
 
 - **Easy Integration**: Quickly integrate with multiple AI providers.
 - **Flexibility**: Easily switch between different AI models.
 - **Convenience**: Avoid the hassle of writing repetitive initialisation code.
 
 ## Installation
 
 First, install the library using pip:
 
 ```bash
-pip install ai_model_library
+git clone https://github.com/harveygw/ailib
 ```
 
 ## Setup
 
-### 1. Environment Variables
+### Environment Variables
 
-This library requires a `.env` file for storing API keys and URLs for the different AI providers. Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
+This library requires a `.env` file for storing API keys and URLs for the different AI providers (You don't need to have all of them). Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
 
 ```
 OPENAI_API_KEY=your_openai_api_key
 OPENAI_API_URL=openai_api_url
 
 GEMINI_API_KEY=your_gemini_api_key
 GEMINI_API_URL=gemini_api_url
@@ -82,18 +66,22 @@
 
 ### Generating Text Using a Registered Model
 
 Once the models are registered, you can use them to generate text. Here's an example using OpenAI's GPT-3 model:
 
 ```python
 # Get the OpenAI model
-model = Models.get_model("openai", "text-davinci-003")
+model = Models.get_model("openai", "gpt-4o")
+
+# Generating text without token limit
+response = model.generate_text("Hello, world!")
+print(response)
 
-# Generate text
-response = model.generate_text("Hello, world!", max_tokens=5)
+# Generate text with token limit
+response = model.generate_text("Hello, world!", max_tokens=128000)
 print(response)
 ```
 
 ### Listing Available Models
 
 You can list all registered models for each provider:
 
@@ -114,33 +102,23 @@
 Models.fetch_and_register_models("openai", "openai")
 Models.fetch_and_register_models("gemini", "gemini")
 Models.fetch_and_register_models("anthropic", "anthropic")
 Models.fetch_and_register_models("cohere", "cohere")
 Models.fetch_and_register_models("google", "google")
 
 # Generate text using a registered model
-model = Models.get_model("openai", "text-davinci-003")
-response = model.generate_text("Hello, world!", max_tokens=5)
+model = Models.get_model("openai", "gpt-4o")
+response = model.generate_text("Hello, world!")
 print(response)
 
 # List all registered models
 all_models = Models.list_models()
 print(all_models)
 ```
 
 ## Running Tests
 
 To ensure everything is working correctly, you can run the provided test suite. This will verify the initialisation, model listing, and text generation for different APIs. Make sure you have your `.env` file properly set up with actual API keys to run these tests.
 
 ```bash
 python -m unittest discover -s tests
 ```
-
-## Contributing
-
-Contributions are welcome! Please open an issue or submit a pull request on GitHub.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-
```

### Comparing `modular-ai-0.1.0/README.md` & `modular-ai-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-# AI Model Library
+Metadata-Version: 2.1
+Name: modular-ai
+Version: 0.1.1
+Summary: A library for interacting with various AI models
+Home-page: https://github.com/HarveyGW/modular-ai
+Author: HarveyGW
+Author-email: harvey@hwfreelance.co.uk
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Modular AI Library
 
 A Python library that allows you to import and use various AI models easily. This library supports multiple AI model providers, making it straightforward to switch between different models without writing initialisation code each time.
 
 ## Features
 
 - **Easy Integration**: Quickly integrate with multiple AI providers.
 - **Flexibility**: Easily switch between different AI models.
 - **Convenience**: Avoid the hassle of writing repetitive initialisation code.
 
 ## Installation
 
 First, install the library using pip:
 
 ```bash
-pip install ai_model_library
+git clone https://github.com/harveygw/ailib
 ```
 
 ## Setup
 
-### 1. Environment Variables
+### Environment Variables
 
-This library requires a `.env` file for storing API keys and URLs for the different AI providers. Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
+This library requires a `.env` file for storing API keys and URLs for the different AI providers (You don't need to have all of them). Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
 
 ```
 OPENAI_API_KEY=your_openai_api_key
 OPENAI_API_URL=openai_api_url
 
 GEMINI_API_KEY=your_gemini_api_key
 GEMINI_API_URL=gemini_api_url
@@ -66,18 +82,22 @@
 
 ### Generating Text Using a Registered Model
 
 Once the models are registered, you can use them to generate text. Here's an example using OpenAI's GPT-3 model:
 
 ```python
 # Get the OpenAI model
-model = Models.get_model("openai", "text-davinci-003")
+model = Models.get_model("openai", "gpt-4o")
+
+# Generating text without token limit
+response = model.generate_text("Hello, world!")
+print(response)
 
-# Generate text
-response = model.generate_text("Hello, world!", max_tokens=5)
+# Generate text with token limit
+response = model.generate_text("Hello, world!", max_tokens=128000)
 print(response)
 ```
 
 ### Listing Available Models
 
 You can list all registered models for each provider:
 
@@ -98,16 +118,16 @@
 Models.fetch_and_register_models("openai", "openai")
 Models.fetch_and_register_models("gemini", "gemini")
 Models.fetch_and_register_models("anthropic", "anthropic")
 Models.fetch_and_register_models("cohere", "cohere")
 Models.fetch_and_register_models("google", "google")
 
 # Generate text using a registered model
-model = Models.get_model("openai", "text-davinci-003")
-response = model.generate_text("Hello, world!", max_tokens=5)
+model = Models.get_model("openai", "gpt-4o")
+response = model.generate_text("Hello, world!")
 print(response)
 
 # List all registered models
 all_models = Models.list_models()
 print(all_models)
 ```
 
@@ -115,14 +135,8 @@
 
 To ensure everything is working correctly, you can run the provided test suite. This will verify the initialisation, model listing, and text generation for different APIs. Make sure you have your `.env` file properly set up with actual API keys to run these tests.
 
 ```bash
 python -m unittest discover -s tests
 ```
 
-## Contributing
-
-Contributions are welcome! Please open an issue or submit a pull request on GitHub.
-
-## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `modular-ai-0.1.0/ailib/ai_models.py` & `modular-ai-0.1.1/ailib/ai_models.py`

 * *Files identical despite different names*

### Comparing `modular-ai-0.1.0/ailib/models.py` & `modular-ai-0.1.1/ailib/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,10 +25,9 @@
         api_key_env, api_url_env, _, _ = AIModel.API_CONFIG[api]
         if os.getenv(api_key_env) and os.getenv(api_url_env):
             models = AIModel.list_available_models(api)
             for model_name in models:
                 cls.register_model(provider, model_name, api)
 
 
-# Fetch and register models from each provider with configured API keys
 for api in AIModel.API_CONFIG:
     Models.fetch_and_register_models(api)
```

### Comparing `modular-ai-0.1.0/modular_ai.egg-info/PKG-INFO` & `modular-ai-0.1.1/modular_ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: modular-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for interacting with various AI models
-Home-page: https://github.com/HarveyGW/AILib
+Home-page: https://github.com/HarveyGW/modular-ai
 Author: HarveyGW
-Author-email: your_email@example.com
+Author-email: harvey@hwfreelance.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# AI Model Library
+# Modular AI Library
 
 A Python library that allows you to import and use various AI models easily. This library supports multiple AI model providers, making it straightforward to switch between different models without writing initialisation code each time.
 
 ## Features
 
 - **Easy Integration**: Quickly integrate with multiple AI providers.
 - **Flexibility**: Easily switch between different AI models.
 - **Convenience**: Avoid the hassle of writing repetitive initialisation code.
 
 ## Installation
 
 First, install the library using pip:
 
 ```bash
-pip install ai_model_library
+git clone https://github.com/harveygw/ailib
 ```
 
 ## Setup
 
-### 1. Environment Variables
+### Environment Variables
 
-This library requires a `.env` file for storing API keys and URLs for the different AI providers. Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
+This library requires a `.env` file for storing API keys and URLs for the different AI providers (You don't need to have all of them). Create a `.env` file in the root of your project and add the respective API keys and URLs like so:
 
 ```
 OPENAI_API_KEY=your_openai_api_key
 OPENAI_API_URL=openai_api_url
 
 GEMINI_API_KEY=your_gemini_api_key
 GEMINI_API_URL=gemini_api_url
@@ -82,18 +82,22 @@
 
 ### Generating Text Using a Registered Model
 
 Once the models are registered, you can use them to generate text. Here's an example using OpenAI's GPT-3 model:
 
 ```python
 # Get the OpenAI model
-model = Models.get_model("openai", "text-davinci-003")
+model = Models.get_model("openai", "gpt-4o")
 
-# Generate text
-response = model.generate_text("Hello, world!", max_tokens=5)
+# Generating text without token limit
+response = model.generate_text("Hello, world!")
+print(response)
+
+# Generate text with token limit
+response = model.generate_text("Hello, world!", max_tokens=128000)
 print(response)
 ```
 
 ### Listing Available Models
 
 You can list all registered models for each provider:
 
@@ -114,16 +118,16 @@
 Models.fetch_and_register_models("openai", "openai")
 Models.fetch_and_register_models("gemini", "gemini")
 Models.fetch_and_register_models("anthropic", "anthropic")
 Models.fetch_and_register_models("cohere", "cohere")
 Models.fetch_and_register_models("google", "google")
 
 # Generate text using a registered model
-model = Models.get_model("openai", "text-davinci-003")
-response = model.generate_text("Hello, world!", max_tokens=5)
+model = Models.get_model("openai", "gpt-4o")
+response = model.generate_text("Hello, world!")
 print(response)
 
 # List all registered models
 all_models = Models.list_models()
 print(all_models)
 ```
 
@@ -131,16 +135,8 @@
 
 To ensure everything is working correctly, you can run the provided test suite. This will verify the initialisation, model listing, and text generation for different APIs. Make sure you have your `.env` file properly set up with actual API keys to run these tests.
 
 ```bash
 python -m unittest discover -s tests
 ```
 
-## Contributing
-
-Contributions are welcome! Please open an issue or submit a pull request on GitHub.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
```

### Comparing `modular-ai-0.1.0/setup.py` & `modular-ai-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="modular-ai",  # New unique project name
-    version="0.1.0",
+    name="modular-ai",
+    version="0.1.1",
     packages=find_packages(),
-    install_requires=[
-        "requests",
-        "python-dotenv",
-    ],
+    install_requires=["requests", "python-dotenv", "anthropic"],
     include_package_data=True,
     description="A library for interacting with various AI models",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="HarveyGW",
-    author_email="your_email@example.com",
-    url="https://github.com/HarveyGW/AILib",
+    author_email="harvey@hwfreelance.co.uk",
+    url="https://github.com/HarveyGW/modular-ai",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `modular-ai-0.1.0/tests/test_ai_lib.py` & `modular-ai-0.1.1/tests/test_ai_lib.py`

 * *Files identical despite different names*

