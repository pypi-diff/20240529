# Comparing `tmp/kaizen_cloudcode-0.1.8.tar.gz` & `tmp/kaizen_cloudcode-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.8.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.9.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.8.tar` & `kaizen_cloudcode-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-19 03:39:17.325799 kaizen_cloudcode-0.1.8/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-19 03:39:17.325799 kaizen_cloudcode-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1463 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3631 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     2526 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     4067 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1528 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     2248 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-19 03:39:17.329799 kaizen_cloudcode-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4089 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3594 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7039 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     2526 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     4195 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1528 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.9/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.8/LICENSE` & `kaizen_cloudcode-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/README.md` & `kaizen_cloudcode-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,26 +39,21 @@
 - `docs`: Contains Nextra-powered documentation for the project.
 - `examples`: Contains sample code for various use cases.
 
 ## Getting Started
 
 To get started with Kaizen, follow these steps:
 
-1. Clone the repository:
+1. Install Kaizen package:
 
-   ```bash
-   git clone https://github.com/Cloud-Code-AI/kaizen.git
-   ```
-
-2. Install dependencies:
-
-   ```bash
-   cd kaizen
-   poetry install
-   ```
+    ```bash
+      pip install kaizen-cloudcode
+    ```
+
+2. Copy the example code from `examples/basic`
 
 3. Generate tests for your website:
 
     First, you need to update the URL in the `examples/basic/generate.py`
     ```bash
       PYTHONPATH=. poetry run python examples/basic/generate.py
     ```
```

#### html2text {}

```diff
@@ -18,30 +18,30 @@
 Contains the main logic for interaction with LLMs and data processing. -
 `actors`: Contains classes used to process various different actions like Code
 Review and Test execution. - `generators`: Contains the main logic for
 generative use cases like test case generation, description generation, etc. -
 `llms`: Contains LLM integrations. - `docs`: Contains Nextra-powered
 documentation for the project. - `examples`: Contains sample code for various
 use cases. ## Getting Started To get started with Kaizen, follow these steps:
-1. Clone the repository: ```bash git clone https://github.com/Cloud-Code-AI/
-kaizen.git ``` 2. Install dependencies: ```bash cd kaizen poetry install ``` 3.
-Generate tests for your website: First, you need to update the URL in the
-`examples/basic/generate.py` ```bash PYTHONPATH=. poetry run python examples/
-basic/generate.py ``` Kaizen will generate all the tests and store them inside
-`.kaizen/tests/` 4. Execute tests: Once you have generated all the necessary
-tests, you can run all the tests in two ways: ```bash PYTHONPATH=. poetry run
-python examples/basic/execute.py ``` Or using the default pytest module: ```
-pytest -v .kaizen/tests/ ``` Kaizen will generate all the tests and store them
-inside `.kaizen/tests/` ### Running API Server for GitHub App Kaizen utilizes a
-GitHub app to perform actions like PR review and description updates. Here is a
-quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/
-pages/github_app.md) Deploy the API using Docker Compose: ``` docker-compose up
-``` You can also configure features by tweaking the config.json file. **NOTE:**
-You need to create a `.env` file by copying `.env.example` and also store the
-PEM file for the GitHub app as `GITHUB_APP_KEY.pem`. ## Contributing We welcome
-contributions from the community! If you'd like to contribute to Kaizen, please
-follow these steps: 1. Fork the repository 2. Create a new branch (`git
-checkout -b feature/my-feature`) 3. Commit your changes (`git commit -m 'Add
-some feature'`) 4. Push to the branch (`git push origin feature/my-feature`) 5.
-Open a Pull Request ## License Kaizen is released under the [AGPL License]
-(LICENSE). ## Contact If you have any questions or need further assistance,
-please feel free to contact us at support@cloudcode.ai.
+1. Install Kaizen package: ```bash pip install kaizen-cloudcode ``` 2. Copy the
+example code from `examples/basic` 3. Generate tests for your website: First,
+you need to update the URL in the `examples/basic/generate.py` ```bash
+PYTHONPATH=. poetry run python examples/basic/generate.py ``` Kaizen will
+generate all the tests and store them inside `.kaizen/tests/` 4. Execute tests:
+Once you have generated all the necessary tests, you can run all the tests in
+two ways: ```bash PYTHONPATH=. poetry run python examples/basic/execute.py ```
+Or using the default pytest module: ``` pytest -v .kaizen/tests/ ``` Kaizen
+will generate all the tests and store them inside `.kaizen/tests/` ### Running
+API Server for GitHub App Kaizen utilizes a GitHub app to perform actions like
+PR review and description updates. Here is a quick link to set up your own
+GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md) Deploy the API
+using Docker Compose: ``` docker-compose up ``` You can also configure features
+by tweaking the config.json file. **NOTE:** You need to create a `.env` file by
+copying `.env.example` and also store the PEM file for the GitHub app as
+`GITHUB_APP_KEY.pem`. ## Contributing We welcome contributions from the
+community! If you'd like to contribute to Kaizen, please follow these steps: 1.
+Fork the repository 2. Create a new branch (`git checkout -b feature/my-
+feature`) 3. Commit your changes (`git commit -m 'Add some feature'`) 4. Push
+to the branch (`git push origin feature/my-feature`) 5. Open a Pull Request ##
+License Kaizen is released under the [AGPL License](LICENSE). ## Contact If you
+have any questions or need further assistance, please feel free to contact us
+at support@cloudcode.ai.
```

### Comparing `kaizen_cloudcode-0.1.8/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.9/kaizen/generator/ui.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.9/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.9/kaizen/helpers/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 from kaizen.helpers import general
 
 logger = logging.getLogger(__name__)
 
 
 PR_COLLAPSIBLE_TEMPLATE = """
 <details>
-<summary>{comment}</summary>
-
-##### Reason
-{reasoning}
-
-##### Confidence
-{confidence}
+<summary>[{confidence}] -> {reasoning}</summary>
 </details>
 """
 
 DESC_COLLAPSIBLE_TEMPLATE = """
 <details>
 <summary>Original Description</summary>
 {desc}
```

### Comparing `kaizen_cloudcode-0.1.8/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.9/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.9/kaizen/llms/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Provide constructive feedback and suggestions for improvements, considering best practices, error handling, performance, readability, and maintainability. 
 Be thorough, objective, and respectful in your reviews, focusing on helping developers improve their skills and code quality. 
 Ask clarifying questions if needed.
 """
 
 CODE_REVIEW_PROMPT = """
 You are an experienced software engineer tasked with reviewing a pull request.
-Your goal is to provide a comprehensive code review that evaluates the code changes, identifies potential issues or areas for improvement,
+Your goal is to provide a comprehensive code review that evaluates the code changes, identifies potential issues,
 and provides constructive feedback to the developer.
 
 Using the provided information, generate a detailed code review with feedback organized as a JSON object. Only include sections with relevant feedback, omitting sections without feedback. Follow this structure:
 {{
   "review": [
     {{
       "topic": "<SECTION_TOPIC>",
@@ -32,16 +32,14 @@
   "low",
   "trivial"
 ]
 
 Potential section topics:
 - "Code Quality"
 - "Performance" 
-- "Testing"
-- "Documentation"
 - "Potential Issues"
 - "Improvements"
 
 Generate all possible feedbacks.
 For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed. Use markdown code blocks to quote relevant snippets of code when necessary.
 Keep comments short but make sure it has actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
 
@@ -79,16 +77,14 @@
   "low",
   "trivial"
 ]
 
 Potential section topics:
 - "Code Quality"
 - "Performance" 
-- "Testing"
-- "Documentation"
 - "Potential Issues"
 - "Improvements"
 
 Generate all possible feedbacks.
 For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed. Use markdown code blocks to quote relevant snippets of code when necessary.
 Keep comments short but make sure it has actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
 
@@ -103,15 +99,14 @@
 PR_DESCRIPTION_PROMPT = """
 You are a skilled developer reviewing a pull request.
 
 Using the provided information, generate a comprehensive description for this pull request. Cover the following points:
 
 1. Summarize the main purpose and scope of the changes.
 2. Highlight any significant modifications, refactoring, or new features introduced.
-3. Explain the motivation or rationale behind the changes.
 
 Provide output in following format:
 {{"desc": "<PR_DESCRIPTION_IN_MARKDOWN>"}}
 
 Your description should be clear, concise, and tailored to help reviewers understand the pull request's impact and make an informed decision.
 
 INFORMATION:
@@ -121,15 +116,15 @@
 Code Diff:
 ```{CODE_DIFF}```
 
 """
 # TODO: Rephrase prompt to make it more clear and accurate.
 UI_MODULES_PROMPT = """
 Assign yourself as a quality assurance engineer. Read this code and design comprehensive tests to test the UI
-of this html. Break it down into 5-10 seperate modules and return the output as JSON with the following keys:
+of this html. Break it down into 5-10 separate modules and return the output as JSON with the following keys:
 id - serial number to identify
 module_title - title of the identified module
 tests - JSON containing list of tests steps to carry out for that module with keys - id, test_description, test_name.
 folder_name - relevant name for the module
 importance - level of importance of this test out of ['critical', 'good_to_have', 'non_essential']
 Share the JSON output ONLY. No other text.
```

### Comparing `kaizen_cloudcode-0.1.8/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.9/kaizen/llms/provider.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.9/kaizen/reviewer/code_review.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class ReviewOutput:
     review: str
     usage: dict
+    model_name: str
     cost: dict
 
 
 @dataclass
 class DescOutput:
     desc: str
     usage: dict
+    model_name: str
     cost: dict
 
 
 class CodeReviewer:
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self.provider = LLMProvider(system_prompt=CODE_REVIEW_SYSTEM_PROMPT)
@@ -75,14 +77,15 @@
         prompt_cost, completion_cost = self.provider.get_usage_cost(
             total_usage=total_usage
         )
 
         return ReviewOutput(
             review=review,
             usage=total_usage,
+            model_name=self.provider.model,
             cost={"prompt_cost": prompt_cost, "completion_cost": completion_cost},
         )
 
     def generate_pull_request_desc(
         self,
         diff_text: str,
         pull_request_title: str,
@@ -108,9 +111,10 @@
         total_usage = self.provider.update_usage(total_usage, usage)
         prompt_cost, completion_cost = self.provider.get_usage_cost(
             total_usage=total_usage
         )
         return DescOutput(
             desc=body,
             usage=total_usage,
+            model_name=self.provider.model,
             cost={"prompt_cost": prompt_cost, "completion_cost": completion_cost},
         )
```

### Comparing `kaizen_cloudcode-0.1.8/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.9/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.9/kaizen/utils/config.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.8/pyproject.toml` & `kaizen_cloudcode-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.8"
+version = "0.1.9"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.8/PKG-INFO` & `kaizen_cloudcode-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.8
+Version: 0.1.9
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -68,26 +68,21 @@
 - `docs`: Contains Nextra-powered documentation for the project.
 - `examples`: Contains sample code for various use cases.
 
 ## Getting Started
 
 To get started with Kaizen, follow these steps:
 
-1. Clone the repository:
+1. Install Kaizen package:
 
-   ```bash
-   git clone https://github.com/Cloud-Code-AI/kaizen.git
-   ```
-
-2. Install dependencies:
-
-   ```bash
-   cd kaizen
-   poetry install
-   ```
+    ```bash
+      pip install kaizen-cloudcode
+    ```
+
+2. Copy the example code from `examples/basic`
 
 3. Generate tests for your website:
 
     First, you need to update the URL in the `examples/basic/generate.py`
     ```bash
       PYTHONPATH=. poetry run python examples/basic/generate.py
     ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.8 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.9 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -35,30 +35,30 @@
 Contains the main logic for interaction with LLMs and data processing. -
 `actors`: Contains classes used to process various different actions like Code
 Review and Test execution. - `generators`: Contains the main logic for
 generative use cases like test case generation, description generation, etc. -
 `llms`: Contains LLM integrations. - `docs`: Contains Nextra-powered
 documentation for the project. - `examples`: Contains sample code for various
 use cases. ## Getting Started To get started with Kaizen, follow these steps:
-1. Clone the repository: ```bash git clone https://github.com/Cloud-Code-AI/
-kaizen.git ``` 2. Install dependencies: ```bash cd kaizen poetry install ``` 3.
-Generate tests for your website: First, you need to update the URL in the
-`examples/basic/generate.py` ```bash PYTHONPATH=. poetry run python examples/
-basic/generate.py ``` Kaizen will generate all the tests and store them inside
-`.kaizen/tests/` 4. Execute tests: Once you have generated all the necessary
-tests, you can run all the tests in two ways: ```bash PYTHONPATH=. poetry run
-python examples/basic/execute.py ``` Or using the default pytest module: ```
-pytest -v .kaizen/tests/ ``` Kaizen will generate all the tests and store them
-inside `.kaizen/tests/` ### Running API Server for GitHub App Kaizen utilizes a
-GitHub app to perform actions like PR review and description updates. Here is a
-quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/
-pages/github_app.md) Deploy the API using Docker Compose: ``` docker-compose up
-``` You can also configure features by tweaking the config.json file. **NOTE:**
-You need to create a `.env` file by copying `.env.example` and also store the
-PEM file for the GitHub app as `GITHUB_APP_KEY.pem`. ## Contributing We welcome
-contributions from the community! If you'd like to contribute to Kaizen, please
-follow these steps: 1. Fork the repository 2. Create a new branch (`git
-checkout -b feature/my-feature`) 3. Commit your changes (`git commit -m 'Add
-some feature'`) 4. Push to the branch (`git push origin feature/my-feature`) 5.
-Open a Pull Request ## License Kaizen is released under the [AGPL License]
-(LICENSE). ## Contact If you have any questions or need further assistance,
-please feel free to contact us at support@cloudcode.ai.
+1. Install Kaizen package: ```bash pip install kaizen-cloudcode ``` 2. Copy the
+example code from `examples/basic` 3. Generate tests for your website: First,
+you need to update the URL in the `examples/basic/generate.py` ```bash
+PYTHONPATH=. poetry run python examples/basic/generate.py ``` Kaizen will
+generate all the tests and store them inside `.kaizen/tests/` 4. Execute tests:
+Once you have generated all the necessary tests, you can run all the tests in
+two ways: ```bash PYTHONPATH=. poetry run python examples/basic/execute.py ```
+Or using the default pytest module: ``` pytest -v .kaizen/tests/ ``` Kaizen
+will generate all the tests and store them inside `.kaizen/tests/` ### Running
+API Server for GitHub App Kaizen utilizes a GitHub app to perform actions like
+PR review and description updates. Here is a quick link to set up your own
+GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md) Deploy the API
+using Docker Compose: ``` docker-compose up ``` You can also configure features
+by tweaking the config.json file. **NOTE:** You need to create a `.env` file by
+copying `.env.example` and also store the PEM file for the GitHub app as
+`GITHUB_APP_KEY.pem`. ## Contributing We welcome contributions from the
+community! If you'd like to contribute to Kaizen, please follow these steps: 1.
+Fork the repository 2. Create a new branch (`git checkout -b feature/my-
+feature`) 3. Commit your changes (`git commit -m 'Add some feature'`) 4. Push
+to the branch (`git push origin feature/my-feature`) 5. Open a Pull Request ##
+License Kaizen is released under the [AGPL License](LICENSE). ## Contact If you
+have any questions or need further assistance, please feel free to contact us
+at support@cloudcode.ai.
```

