# Comparing `tmp/py_alpaca_api-0.6.0.tar.gz` & `tmp/py_alpaca_api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.6.0.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.6.1.tar", max compression
```

## Comparing `py_alpaca_api-0.6.0.tar` & `py_alpaca_api-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.0/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.0/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2213 2024-05-26 23:53:22.916017 py_alpaca_api-0.6.0/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.0/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6791 2024-05-26 00:47:40.736842 py_alpaca_api-0.6.0/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3324 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.0/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    15970 2024-05-26 15:45:30.270707 py_alpaca_api-0.6.0/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     8341 2024-05-26 00:47:40.736842 py_alpaca_api-0.6.0/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2985 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.0/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    17430 2024-05-26 15:45:30.270707 py_alpaca_api-0.6.0/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0     9323 2024-05-26 15:45:30.270707 py_alpaca_api-0.6.0/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     8633 2024-05-26 23:53:22.916017 py_alpaca_api-0.6.0/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14951 2024-05-26 13:07:04.489420 py_alpaca_api-0.6.0/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-26 23:53:22.916017 py_alpaca_api-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.1/LICENSE
+-rw-r--r--   0        0        0    17780 2024-05-28 01:41:42.529974 py_alpaca_api-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.1/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.1/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.1/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6777 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.1/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     2898 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.1/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    11730 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7469 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2984 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    20152 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0     9323 2024-05-28 01:32:55.543711 py_alpaca_api-0.6.1/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     9587 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14852 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.1/PKG-INFO
```

### Comparing `py_alpaca_api-0.6.0/LICENSE` & `py_alpaca_api-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.0/README.md` & `py_alpaca_api-0.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,48 @@
+Metadata-Version: 2.1
+Name: py-alpaca-api
+Version: 0.6.1
+Summary: Python package, for communicating with Alpaca Markets REST API.
+Home-page: https://github.com/TexasCoding/py-alpaca-api
+License: MIT
+Keywords: alpaca,python
+Author: TexasCoding
+Author-email: jeff10278@me.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">PY-ALPACA-API</h1>
 </p>
 <p align="center">
-    <em>Empowering Alpaca Trading API with Python</em>
+    <em>Empower Trading with Seamless Alpaca API Integration</em>
 </p>
 <p align="center">
-<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
+   <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
 	<img src="https://img.shields.io/github/license/TexasCoding/py-alpaca-api?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
 	<img src="https://img.shields.io/github/last-commit/TexasCoding/py-alpaca-api?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 	<img src="https://img.shields.io/github/languages/top/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-top-language">
 	<img src="https://img.shields.io/github/languages/count/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-language-count">
 <p>
 <p align="center">
 	<!-- default option, no dependency badges. -->
    <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
    <img alt="Poetry" src="https://img.shields.io/badge/Poetry-%233B82F6.svg?style=for-the-badge&logo=poetry&logoColor=0B3D8D">
-
 </p>
 
 <br><!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary><br>
 
 - [ Overview](#-overview)
@@ -38,80 +58,100 @@
 - [ License](#-license)
 - [ Acknowledgments](#-acknowledgments)
 </details>
 <hr>
 
 ##  Overview
 
-The py-alpaca-api project facilitates seamless interaction with the Alpaca Markets REST API, offering a comprehensive suite of functionalities for trading and investment purposes. Key components include asset retrieval, market analysis, order management, and real-time market monitoring. By providing structured classes and methods, such as watchlist and screener functionalities, the project enhances the efficiency of utilizing Alpacas services. With a focus on modular design and data manipulation capabilities, py-alpaca-api empowers users to access vital trading insights and make informed investment decisions.
+The py-alpaca-api project provides a comprehensive Python interface for seamless interaction with the Alpaca API, offering functionalities such as accessing account information, retrieving asset data, managing market details, executing orders, and analyzing stock performance. By encapsulating key components like account, asset, order, and market classes, this project facilitates efficient data retrieval, trading operations, and market analysis within the Alpaca ecosystem. Integrated with GitHub Actions for testing integrity, py-alpaca-api enhances developers capabilities in integrating Alpacas features into diverse projects, emphasizing simplicity and reliability in financial data processing and trading activities.
 
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
-| ⚙️  | **Architecture**  | The project follows a structured architecture using classes like PyAlpacaApi, Watchlist, Screener, Position, Order, Market, and others for specific API interactions. This modular design enhances functionality and maintainability. |
-| 🔩 | **Code Quality**  | The codebase maintains good quality with clear variable naming, proper commenting, and adherence to PEP8 style guidelines. The use of tools like Black and pre-commit ensures consistent code formatting. |
-| 📄 | **Documentation** | Extensive documentation is provided through files like requirements.txt, pyproject.toml, and inline comments. Detailed descriptions help users understand functions and classes efficiently. Proper metadata and dependencies are also outlined. |
-| 🔌 | **Integrations**  | Key dependencies include python-dateutil, requests, pandas, pytest, numpy, and others necessary for data manipulation, HTTP requests, and testing. GitHub Actions are used for CI/CD processes. |
-| 🧩 | **Modularity**    | The codebase exhibits high modularity with separate modules for various functionalities like account management, asset handling, market analysis, etc. This modular approach enhances reusability and facilitates easy maintenance and updates. |
-| 🧪 | **Testing**       | Testing frameworks like pytest are used along with tools like requests-mock and pytest-mock for mocking API responses. Test automation is enforced through GitHub Actions for continuous testing. |
-| ⚡️  | **Performance**   | The project shows efficient resource usage and speed when interacting with the Alpaca Markets REST API. Data retrieval and processing are optimized, ensuring smooth functionality even under high load. |
-| 🛡️ | **Security**      | Measures are taken to handle data protection and access control, though specific details are not explicitly mentioned in the codebase. Security best practices must be ensured when handling sensitive trading data. |
-| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy, and others crucial for data manipulation and API interactions. Poetry is used for dependency management. |
+| ⚙️  | **Architecture**  | The project follows a modular architecture, with key components like `account.py`, `asset.py`, `market.py`, etc., encapsulating specific functionalities. This design enhances code organization and maintainability. |
+| 🔩 | **Code Quality**  | The codebase maintains high quality and follows PEP8 style conventions. It leverages tools like `black`, `flake8`, and `isort` for consistent formatting and clean code practices. |
+| 📄 | **Documentation** | The project includes detailed documentation in `pyproject.toml`, outlining metadata, dependencies, and structure. Inline code comments and docstrings enhance readability and understanding for developers. |
+| 🔌 | **Integrations**  | Key integrations include `requests`, `pandas`, `numpy`, etc., for data processing, HTTP requests, and financial analysis. External services like Alpaca API are seamlessly integrated for trading operations. |
+| 🧩 | **Modularity**    | The codebase exhibits high modularity, allowing for code reuse and easy maintenance. Each module focuses on specific tasks, promoting separation of concerns and enhancing scalability. |
+| 🧪 | **Testing**       | Testing frameworks such as `pytest` and `pytest-mock` are employed for unit testing. `pre-commit` ensures code quality checks before commits, maintaining robust test coverage. |
+| ⚡️  | **Performance**   | The project emphasizes efficiency and resource optimization, ensuring swift data retrieval and processing. Performance tuning techniques are implemented to enhance speed and responsiveness. |
+| 🛡️ | **Security**      | Security measures are in place for data protection and access control. Proper handling of API credentials and secure HTTP communication safeguard sensitive information. |
+| 📦 | **Dependencies**  | Key dependencies include `certifi`, `requests`, `pytz`, etc., facilitating API interaction, data manipulation, and time zone handling. These libraries enhance the project's functionality. |
 
 ---
 
 ##  Repository Structure
 
 ```sh
-   py_alpaca_api
-   ├── alpaca.py
-   └── src
-       ├── __init__.py
-       ├── account.py
-       ├── asset.py
-       ├── data_classes.py
-       ├── history.py
-       ├── market.py
-       ├── order.py
-       ├── position.py
-       ├── screener.py
-       └── watchlist.py
+py_alpaca_api 
+├── __init__.py
+├── alpaca.py
+└── src
+   ├── __init__.py
+   ├── account.py
+   ├── asset.py
+   ├── data_classes.py
+   ├── history.py
+   ├── market.py
+   ├── order.py
+   ├── position.py
+   ├── screener.py
+   └── watchlist.py
 ```
 
 ---
 
 ##  Modules
 
+<details closed><summary>.</summary>
+
+| File                                                                                          | Summary                                                                                                                                                                                                                                      |
+| ---                                                                                           | ---                                                                                                                                                                                                                                          |
+| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml)     | Defines dependencies and metadata for Python Alpaca API package.-Specifies version, description, authors, license, homepage, and repository.-Lists development, testing, and documentation dependencies.                                     |
+| [requirements.txt](https://github.com/TexasCoding/py-alpaca-api/blob/master/requirements.txt) | Specifies Python package dependencies for the repository based on version compatibility. Essential libraries for API integration and data processing are outlined, ensuring proper functioning and alignment with specified Python versions. |
+
+</details>
+
 <details closed><summary>py_alpaca_api</summary>
 
-| File                                                                                          | Summary                                                                                                                                                                                                                              |
-| ---                                                                                           | ---                                                                                                                                                                                                                                  |
-| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class initializing with API credentials for Alpaca trading. Sets URL based on trading type. Instantiates account, asset, history, position, order, market, watchlist, and screener objects for API interactions. |
+| File                                                                                          | Summary                                                                                                                                                                                                                                               |
+| ---                                                                                           | ---                                                                                                                                                                                                                                                   |
+| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class central to Alpaca API interaction. Initializes key components like account, asset, history, position, order, market, watchlist, and screener with API credentials and URLs for seamless data access and trading operations. |
+
+</details>
+
+<details closed><summary>.github.workflows</summary>
+
+| File                                                                                                            | Summary                                                                                                                           |
+| ---                                                                                                             | ---                                                                                                                               |
+| [test-package.yml](https://github.com/TexasCoding/py-alpaca-api/blob/master/.github/workflows/test-package.yml) | Verifies Python package build and tests integrity using GitHub Actions workflow test-package.yml in the py-alpaca-api repository. |
 
 </details>
 
 <details closed><summary>py_alpaca_api.src</summary>
 
-| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | This code file within the `py-alpaca-api` repository serves the critical purpose of providing a comprehensive set of classes and functions to interact with the Alpaca API effectively. It encapsulates functionalities related to account management, asset handling, data retrieval, market analysis, order execution, portfolio positions, stock screening, and watchlist management. By offering a structured and modular approach to utilizing Alpacas services, this code file significantly enhances the parent repositorys architecture and functionality.                          |
-| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Defines methods to retrieve top gainers and losers in the stock market by analyzing price, volume, and trade count. Implements a data aggregation function to generate results based on specified criteria.                                                                                                                                                                                                                                                                                                                                                                                 |
-| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, formats, and manages position data from the Alpaca Trade API, enabling actions like fetching all positions, getting specific positions, closing all positions, and closing a specific position. Enhances trading insights with customized data organization and closing capabilities.                                                                                                                                                                                                                                                                                            |
-| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | This code file, `screener.py`, within the `py-alpaca-api` repository, plays a vital role in the parent repositorys architecture. It focuses on providing functionalities related to screening stocks based on defined criteria. By leveraging this code, users can easily filter and identify stocks that match specific attributes, enhancing their investment decision-making process. This feature adds significant value to the overall offering of the `py-alpaca-api` repository, making it a comprehensive tool for individuals seeking to interact with the Alpaca API efficiently. |
-| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Defines Market class with clock method to retrieve market status from Alpaca API. Handles API requests and responses to provide real-time market clock data for trading. Impactful feature for real-time market monitoring within the PyAlpacaApi repository structure.                                                                                                                                                                                                                                                                                                                     |
-| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data from Alpaca API based on specified parameters. Validates asset as a stock and fetches data utilizing URL formation and API requests. Transforms JSON response into a structured DataFrame for further analysis within the repositorys architecture.                                                                                                                                                                                                                                                                                                         |
-| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file in the py-alpaca-api repository serves as a comprehensive interface for interacting with Alpacas API services. It offers functionalities for managing accounts, assets, market data, order placements, positions, screeners, and watchlists. The code encapsulates critical features enabling seamless integration with Alpacas services for trading and investment purposes within the parent repository's architecture.                                                                                                                                                    |
-| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using provided trade URL and headers. Supports fetching all assets based on status, asset class, and exchange. Implements error handling for unsuccessful requests.                                                                                                                                                                                                                                                                                                                                                                             |
-| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API using provided URL and headers. Implements a method to return account details as an object. Handles successful and unsuccessful responses appropriately.                                                                                                                                                                                                                                                                                                                                                                                      |
+| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account activities for a specific type, ensuring valid date usage. Fetches account information from Alpaca API and portfolio history data, transforming timestamps. Maintains DataFrame consistency and raises exceptions for failed requests.                                                                                                                                                                                                                        |
+| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using given parameters. Utilizes requests to fetch data, then processes and returns it in a structured format. Maps API responses to custom AssetClass objects for ease of use.                                                                                                                                                                                                                                                     |
+| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file, `alpaca.py`, serves as a crucial component within the `py-alpaca-api` repository. It encapsulates functionalities related to interacting with the Alpaca API, including handling account information, managing assets, and executing orders. By providing a streamlined interface for accessing Alpacas services, this module enhances the overall capability of the repository, enabling seamless integration of Alpacas features into broader projects.       |
+| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data, validates if an asset is a stock, and preprocesses data. Supports fetching data based on symbol, timeframe, and date range. Ensures data integrity and format consistency for analysis within the parent repositorys Alpaca API integration.                                                                                                                                                                                                   |
+| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Implements Market class with methods for retrieving calendar data and market clock status from Alpaca API. Provides functionalities to fetch, process, and return market-related information in a structured format.                                                                                                                                                                                                                                                            |
+| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | Watchlist.py`The `watchlist.py` file in the `py-alpaca-api` repository is crucial for managing and tracking user-defined watchlists of assets within the Alpaca trading platform. It enables users to create, update, and retrieve custom watchlists, providing a streamlined approach to monitor specific assets of interest. By utilizing this module, users can easily curate and monitor their preferred assets, enhancing their trading experience on the Alpaca platform. |
+| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, processes, and manages Alpaca account positions, providing data in DataFrame format, individual position details, and options to close positions individually or all at once. Maintains accuracy and consistency in position-related actions within the Alpaca API ecosystem.                                                                                                                                                                                        |
+| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Analyzes stock winners and losers by filtering data based on preset criteria. Retrieves and ranks stock performances for the previous day, with options to customize filter thresholds. Requires asset and market context for accurate analysis.                                                                                                                                                                                                                                |
+| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | Retrieval, creation, updating, deletion, and asset management. Encapsulates request handling, response processing, and error management. conforms to the parent repositorys architecture by structuring functionality into distinct modules.                                                                                                                                                                                                                                    |
 
 </details>
 
+---
+
 ##  Getting Started
 
 **System Requirements:**
 
 * **Python**: `version x.y.z`
 
 ###  Installation
@@ -127,15 +167,15 @@
 > 2. Change to the project directory:
 > ```console
 > $ cd py-alpaca-api
 > ```
 >
 > 3. Install the dependencies:
 > ```console
-> $ poetry install
+> $ pip install -r requirements.txt
 > ```
 
 ###  Usage
 
 <h4>From <code>source</code></h4>
 
 > Run py-alpaca-api using the command below:
@@ -193,18 +233,19 @@
 </p>
 </details>
 
 ---
 
 ##  License
 
-This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.
+This project is protected under the [MIT]() License. For more details, refer to the [LICENSE](https://github.com/TexasCoding/py-alpaca-api/blob/master/LICENSE) file.
 
 ---
 
 ##  Acknowledgments
 
 - List any resources, contributors, inspiration, etc. here.
 
 [**Return**](#-overview)
 
 ---
+
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.6.1/py_alpaca_api/alpaca.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             api_key (str): The API key for accessing the Alpaca API.
             api_secret (str): The API secret for accessing the Alpaca API.
             api_paper (bool, optional): Specifies whether to use the Alpaca paper trading API.
                 Defaults to True.
 
         Raises:
             ValueError: If the API key or API secret is not provided.
-
         """
         if not api_key:
             raise ValueError("API Key is required")
         if not api_secret:
             raise ValueError("API Secret is required")
 
         # Set the API Key and Secret
@@ -50,8 +49,13 @@
             trade_url=self.trade_url,
             headers=self.headers,
             account=self.account,
         )
         self.order = Order(trade_url=self.trade_url, headers=self.headers)
         self.market = Market(trade_url=self.trade_url, headers=self.headers)
         self.watchlist = Watchlist(trade_url=self.trade_url, headers=self.headers)
-        self.screener = Screener(data_url=self.data_url, headers=self.headers, asset=self.asset, market=self.market)
+        self.screener = Screener(
+            data_url=self.data_url,
+            headers=self.headers,
+            asset=self.asset,
+            market=self.market,
+        )
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/account.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if request.status_code != 200:
             raise Exception(f"Failed to get account activities. Response: {request.text}")
 
         response = json.loads(request.text)
 
         activity_df = pd.DataFrame()
-        activity_df = activity_df.assign(
+        activity_df.assign(
             symbol="NAN",
             activity_type="NAN",
             id="NAN",
             cum_qty="NAN",
             leaves_qty="NAN",
             price="NAN",
             qty="NAN",
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/history.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/history.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,37 @@
 
         """
         self.data_url = data_url
         self.headers = headers
         self.asset = asset
 
     ###########################################
+    # /////// Check if Asset is Stock \\\\\\\ #
+    ###########################################
+    def check_if_stock(self, symbol: str) -> AssetClass:
+        """Check if asset is stock
+        Args:
+            symbol: The symbol of the asset to be checked.
+
+        Returns:
+            AssetClass: The asset information for the given symbol.
+
+        Raises:
+            ValueError: If there is an error getting the asset information or if the asset is not a stock.
+        """
+
+        try:
+            asset = self.asset.get(symbol)
+        except Exception as e:
+            raise ValueError(e)
+        if asset.asset_class != "us_equity":
+            raise ValueError(f"{symbol} is not a stock.")
+        return asset
+
+    ###########################################
     # ////// Get Stock Historical Data \\\\\\ #
     ###########################################
     def get_stock_data(
         self,
         symbol: str,
         start: str,
         end: str,
@@ -51,22 +74,19 @@
             adjustment: The adjustment for historical data. Default is "raw".
 
         Returns:
             A pandas DataFrame containing the historical stock data for the given symbol and time range.
 
         Raises:
             ValueError: If the given timeframe is not one of the allowed values.
-
         """
-
         self.check_if_stock(symbol)
 
-        # URL for historical stock data request
         url = f"{self.data_url}/stocks/{symbol}/bars"
-        # Set timeframe
+
         timeframe_mapping: dict = {
             "1m": "1Min",
             "5m": "5Min",
             "15m": "15Min",
             "30m": "30Min",
             "1h": "1Hour",
             "4h": "4Hour",
@@ -74,15 +94,14 @@
             "1w": "1Week",
             "1M": "1Month",
         }
 
         if timeframe not in timeframe_mapping:
             raise ValueError('Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"')
 
-        # Parameters for historical stock data request
         params = {
             "timeframe": timeframe_mapping[timeframe],  # Timeframe for historical data, default: 1d
             "start": start,  # Start date for historical data
             "end": end,  # End date for historical data
             "currency": currency,  # Currency for historical data, default: USD
             "limit": limit,  # Limit number of data points, default: 1000
             "adjustment": adjustment,  # Adjustment for historical data, default: raw
@@ -90,93 +109,63 @@
             "sort": sort,  # Sort order, default: asc
         }
         symbol_data = self.get_historical_data(symbol, url, params)
         bar_data_df = self.preprocess_data(symbol_data, symbol)
         return bar_data_df
 
     ###########################################
-    # /////// Check if Asset is Stock \\\\\\\ #
-    ###########################################
-    def check_if_stock(self, symbol: str) -> AssetClass:
-        """Check if asset is stock
-        Args:
-            symbol: The symbol of the asset to be checked.
-
-        Returns:
-            AssetClass: The asset information for the given symbol.
-
-        Raises:
-            ValueError: If there is an error getting the asset information or if the asset is not a stock.
-        """
-        # Get asset information for the symbol
-        try:
-            asset = self.asset.get(symbol)
-        # Raise exception if failed to get asset information
-        except Exception as e:
-            raise ValueError(e)
-        else:
-            # Check if asset is a stock
-            if asset.asset_class != "us_equity":
-                # Raise exception if asset is not a stock
-                raise ValueError(f"{symbol} is not a stock.")
-        return asset
-
-    ###########################################
     # /////////// PreProcess Data \\\\\\\\\\\ #
     ###########################################
     @staticmethod
     def preprocess_data(symbol_data: list[defaultdict], symbol: str) -> pd.DataFrame:
         """Prepross data
         Preprocesses the given symbol data by converting it to a pandas DataFrame and performing various
         data transformations.
 
         Args:
             symbol_data: A list of defaultdict objects representing the JSON response data.
             symbol: A string representing the symbol or ticker for the stock data.
 
         Returns:
             A pandas DataFrame containing the preprocessed historical stock data.
-
         """
-        # Convert JSON response to dictionary
+
         bar_data_df = pd.DataFrame(symbol_data)
 
-        # Add symbol column to DataFrame
         bar_data_df.insert(0, "symbol", symbol)
-        # Reformat date column
         bar_data_df["t"] = pd.to_datetime(bar_data_df["t"].replace("[A-Za-z]", " ", regex=True))
-        # Rename columns for consistency
+
         bar_data_df.rename(
             columns={
                 "t": "date",
                 "o": "open",
                 "h": "high",
                 "l": "low",
                 "c": "close",
                 "v": "volume",
                 "n": "trade_count",
                 "vw": "vwap",
             },
             inplace=True,
         )
-        # Convert columns to appropriate data types
+
         bar_data_df = bar_data_df.astype(
             {
                 "open": "float",
                 "high": "float",
                 "low": "float",
                 "close": "float",
                 "symbol": "str",
                 "date": "datetime64[ns]",
                 "vwap": "float",
                 "trade_count": "int",
                 "volume": "int",
             }
         )
-        # Return historical stock data as a DataFrame
+
         return bar_data_df
 
     ###########################################
     # ///////// Get Historical Data \\\\\\\\\ #
     ###########################################
     def get_historical_data(self, symbol: str, url: str, params: dict) -> list[defaultdict]:
         """Get historical stock data
@@ -190,21 +179,14 @@
 
         Raises:
             Exception: If the API response status code is not 200, an exception is raised with the error message.
 
 
         This function fetches historical data for a given symbol by making requests to the specified API endpoint.
         It uses a page token to paginate through the response data and retrieves all available historical bars.
-
-        Example usage:
-            symbol = "AAPL"
-            url = "https://api.example.com/historical"
-            params = {"start_date": "2021-01-01", "end_date": "2021-01-31"}
-
-            historical_data = get_historical_data(symbol, url, params)
         """
         page_token = None
         symbols_data = defaultdict(list)
         while True:
             params["page_token"] = page_token
             response = requests.get(url, headers=self.headers, params=params)
             if response.status_code != 200:
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/market.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
         Args:
             start_date (str): The start date of the calendar range in the format 'yyyy-mm-dd'.
             end_date (str): The end date of the calendar range in the format 'yyyy-mm-dd'.
 
         Returns:
             pd.DataFrame: A pandas DataFrame object containing the calendar data for the specified date range.
-
         """
         url = f"{self.trade_url}/calendar"
         params = {
             "start": start_date,
             "end": end_date,
         }
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/order.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/order.py`

 * *Files 15% similar despite different names*

```diff
@@ -109,162 +109,208 @@
             res = json.loads(response.text)
             return f"{len(res)} orders have been cancelled"
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
             raise Exception(f'Failed to cancel orders. Response: {res["message"]}')
 
+    @staticmethod
+    def check_for_order_errors(
+        symbol: str,
+        qty: float = None,
+        notional: float = None,
+        take_profit: float = None,
+        stop_loss: float = None,
+    ) -> None:
+        """
+        Checks for order errors based on the given parameters.
+
+        Args:
+            symbol (str): The symbol for trading.
+            qty (float, optional): The quantity of the order. Defaults to None.
+            notional (float, optional): The notional value of the order. Defaults to None.
+            take_profit (float, optional): The take profit value for the order. Defaults to None.
+            stop_loss (float, optional): The stop loss value for the order. Defaults to None.
+
+        Raises:
+            ValueError: If symbol is not provided.
+            ValueError: If both qty and notional are provided or if neither is provided.
+            ValueError: If either take_profit or stop_loss is not provided.
+            ValueError: If both take_profit and stop_loss are not provided.
+            ValueError: If notional is provided or if qty is not an integer when both take_profit and
+            stop_loss are provided.
+
+        Returns:
+            None
+        """
+        if not symbol:
+            raise ValueError("Must provide symbol for trading.")
+
+        if not (qty or notional) or (qty and notional):
+            raise ValueError("Qty or Notional are required, not both.")
+
+        if take_profit and not stop_loss or stop_loss and not take_profit:
+            raise ValueError("Both take profit and stop loss are required for bracket orders.")
+
+        if take_profit and stop_loss:
+            if notional or not qty.is_integer():
+                raise ValueError("Bracket orders can not be fractionable.")
+
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Market Order ////////////////#
     ########################################################
     def market(
         self,
         symbol: str,
         qty: float = None,
         notional: float = None,
+        take_profit: float = None,
+        stop_loss: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
         """
-        Submits a market order for the specified symbol.
+        Submits a market order for a specified symbol.
 
         Args:
-            symbol (str): The symbol to trade.
-            qty (float, optional): The quantity to trade. Either `qty` or `notional` must be provided, not both.
-            Defaults to None.
-            notional (float, optional): The notional value of the trade. Either `qty` or `notional` must be provided, not both.
-            Defaults to None.
-            side (str, optional): The side of the trade. Defaults to "buy".
-            time_in_force (str, optional): The time in force for the order. Defaults to "day".
-            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+            symbol (str): The symbol of the asset to trade.
+            qty (float, optional): The quantity of the asset to trade. Either qty or notional must be provided,
+            but not both. Defaults to None.
+            notional (float, optional): The notional value of the asset to trade. Either qty or notional must be
+            provided, but not both. Defaults to None.
+            take_profit (float, optional): The take profit price for the order. Defaults to None.
+            stop_loss (float, optional): The stop loss price for the order. Defaults to None.
+            side (str, optional): The side of the order (buy/sell). Defaults to "buy".
+            time_in_force (str, optional): The time in force for the order (day/gtc/opg/ioc/fok). Defaults to "day".
+            extended_hours (bool, optional): Whether to trade during extended hours. Defaults to False.
 
         Returns:
-            OrderClass: The submitted market order.
-
-        Raises:
-            ValueError: If `symbol` is not provided.
-            ValueError: If both `qty` and `notional` are not provided, or if both are provided.
+            OrderClass: An instance of the OrderClass representing the submitted order.
         """
+        self.check_for_order_errors(
+            symbol=symbol,
+            qty=qty,
+            notional=notional,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
+        )
 
-        if not symbol:
-            raise ValueError("Must provide symbol for trading.")
-
-        if not (qty or notional) or (qty and notional):
-            raise ValueError("Qty or Notional are required, not both.")
-
-        return self.__submit_order(
+        return self._submit_order(
             symbol=symbol,
             side=side,
             qty=qty,
             notional=notional,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
             entry_type="market",
             time_in_force=time_in_force,
             extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Limit Order /////////////////#
     ########################################################
     def limit(
         self,
         symbol: str,
         limit_price: float,
         qty: float = None,
         notional: float = None,
+        take_profit: float = None,
+        stop_loss: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
         """
-        Submits a limit order for trading.
+        Limit order function that submits an order to buy or sell a specified symbol at a specified limit price.
 
         Args:
-            symbol (str): The symbol of the security to trade.
-            limit_price (float): The limit price for the order.
-            qty (float, optional): The quantity of shares to trade. Either `qty` or `notional` must be provided, not both.
-            Defaults to None.
-            notional (float, optional): The notional value of the trade. Either `qty` or `notional` must be provided, not both.
-            Defaults to None.
-            side (str, optional): The side of the order, either 'buy' or 'sell'. Defaults to 'buy'.
-            time_in_force (str, optional): The time in force for the order. Defaults to 'day'.
-            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+            symbol (str): The symbol of the asset to trade.
+            limit_price (float): The limit price at which to execute the order.
+            qty (float, optional): The quantity of the asset to trade. Default is None.
+            notional (float, optional): The amount of money to spend on the asset. Default is None.
+            take_profit (float, optional): The price at which to set a take profit order. Default is None.
+            stop_loss (float, optional): The price at which to set a stop loss order. Default is None.
+            side (str, optional): The side of the order. Must be either "buy" or "sell". Default is "buy".
+            time_in_force (str, optional): The duration of the order. Must be either "day" or "gtc"
+            (good till canceled). Default is "day".
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Default is False.
 
         Returns:
-            OrderClass: The submitted limit order.
-
-        Raises:
-            ValueError: If `symbol` or `limit_price` is not provided, or if both `qty` and `notional` are provided or not provided.
-
+            OrderClass: The submitted order.
         """
+        self.check_for_order_errors(
+            symbol=symbol,
+            qty=qty,
+            notional=notional,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
+        )
 
-        if not symbol:
-            raise ValueError("Must provide symbol for trading.")
-
-        if not limit_price:
-            raise ValueError("Must provide limit price for trading.")
-
-        if not (qty or notional) or (qty and notional):
-            raise ValueError("Qty or Notional are required, not both.")
-
-        return self.__submit_order(
+        return self._submit_order(
             symbol=symbol,
             side=side,
             limit_price=limit_price,
             qty=qty,
             notional=notional,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
             entry_type="limit",
             time_in_force=time_in_force,
             extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
     ########################################################
     def stop(
         self,
         symbol: str,
         stop_price: float,
         qty: float,
         side: str = "buy",
+        take_profit: float = None,
+        stop_loss: float = None,
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
         """
-        Submits a stop order for trading.
-
         Args:
-            symbol (str): The symbol of the security to trade.
-            stop_price (float): The stop price for the order.
-            qty (float): The quantity of shares to trade.
-            side (str, optional): The side of the order. Defaults to "buy".
-            time_in_force (str, optional): The time in force for the order. Defaults to "day".
-            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+            symbol: The symbol of the security to trade.
+            stop_price: The stop price at which the trade should be triggered.
+            qty: The quantity of shares to trade.
+            side: The side of the trade. Defaults to 'buy'.
+            take_profit: The price at which to take profit on the trade. Defaults to None.
+            stop_loss: The price at which to set the stop loss on the trade. Defaults to None.
+            time_in_force: The duration for which the order will be in effect. Defaults to 'day'.
+            extended_hours: A boolean value indicating whether to place the order during extended hours.
+            Defaults to False.
 
         Returns:
-            OrderClass: The submitted stop order.
+            An instance of the OrderClass representing the submitted order.
 
         Raises:
-            ValueError: If symbol, stop_price, or qty is not provided.
+            OrderError: If there are any errors with the order parameters.
         """
+        self.check_for_order_errors(
+            symbol=symbol,
+            qty=qty,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
+        )
 
-        if not symbol:
-            raise ValueError("Must provide symbol for trading.")
-
-        if not stop_price:
-            raise ValueError("Must provide stop price for trading.")
-
-        if not qty:
-            raise ValueError("Qty is required.")
-
-        return self.__submit_order(
+        return self._submit_order(
             symbol=symbol,
             side=side,
             stop_price=stop_price,
             qty=qty,
+            take_profit=take_profit,
+            stop_loss=stop_loss,
             entry_type="stop",
             time_in_force=time_in_force,
             extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
@@ -305,15 +351,15 @@
 
         if not (limit_price or stop_price):
             raise ValueError("Must provide limit and stop price for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
 
-        return self.__submit_order(
+        return self._submit_order(
             symbol=symbol,
             side=side,
             stop_price=stop_price,
             limit_price=limit_price,
             qty=qty,
             entry_type="stop_limit",
             time_in_force=time_in_force,
@@ -366,73 +412,79 @@
         if trail_percent is None and trail_price is None or trail_percent and trail_price:
             raise ValueError("Either trail_percent or trail_price must be provided, not both.")
 
         if trail_percent:
             if trail_percent < 0:
                 raise ValueError("Trail percent must be greater than 0.")
 
-        return self.__submit_order(
+        return self._submit_order(
             symbol=symbol,
             side=side,
             trail_price=trail_price,
             trail_percent=trail_percent,
             qty=qty,
             entry_type="trailing_stop",
             time_in_force=time_in_force,
             extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Order //////////////////////#
     ########################################################
-    def __submit_order(
+    def _submit_order(
         self,
         symbol: str,
         entry_type: str,
         qty: float = None,
         notional: float = None,
         stop_price: float = None,
         limit_price: float = None,
         trail_percent: float = None,
         trail_price: float = None,
+        take_profit: Dict[str, float] = None,
+        stop_loss: Dict[str, float] = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
         """
         Submits an order to the Alpaca API.
 
         Args:
             symbol (str): The symbol of the security to trade.
-            entry_type (str): The type of order to submit (e.g., 'market', 'limit', 'stop').
+            entry_type (str): The type of order to submit.
             qty (float, optional): The quantity of shares to trade. Defaults to None.
-            notional (float, optional): The desired notional value of the trade. Defaults to None.
+            notional (float, optional): The notional value of the trade. Defaults to None.
             stop_price (float, optional): The stop price for a stop order. Defaults to None.
             limit_price (float, optional): The limit price for a limit order. Defaults to None.
             trail_percent (float, optional): The trailing stop percentage for a trailing stop order. Defaults to None.
             trail_price (float, optional): The trailing stop price for a trailing stop order. Defaults to None.
-            side (str, optional): The side of the trade ('buy' or 'sell'). Defaults to 'buy'.
-            time_in_force (str, optional): The time in force for the order ('day', 'gtc', 'opg', 'ioc', 'fok'). Defaults to 'day'.
+            take_profit (Dict[str, float], optional): The take profit parameters for the order. Defaults to None.
+            stop_loss (Dict[str, float], optional): The stop loss parameters for the order. Defaults to None.
+            side (str, optional): The side of the trade (buy or sell). Defaults to "buy".
+            time_in_force (str, optional): The time in force for the order. Defaults to "day".
             extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
 
         Returns:
-            OrderClass: An object representing the submitted order.
+            OrderClass: The submitted order.
 
         Raises:
-            Exception: If the order submission fails, an exception is raised with the error message.
+            Exception: If the order submission fails.
         """
-
         payload = {
             "symbol": symbol,
             "qty": qty if qty else None,
             "notional": round(notional, 2) if notional else None,
             "stop_price": stop_price if stop_price else None,
             "limit_price": limit_price if limit_price else None,
             "trail_percent": trail_percent if trail_percent else None,
             "trail_price": trail_price if trail_price else None,
+            "order_class": "bracket" if take_profit or stop_loss else "simple",
+            "take_profit": ({"limit_price": take_profit} if take_profit else None),
+            "stop_loss": {"stop_price": stop_loss} if stop_loss else None,
             "side": side if side == "buy" else "sell",
             "type": entry_type,
             "time_in_force": time_in_force,
             "extended_hours": extended_hours,
         }
 
         url = f"{self.trade_url}/orders"
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/position.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/screener.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         ___________
         data_url: str
                 Alpaca Data API URL required
 
         headers: object
                 API request headers required
 
-        asset: Asset
-                Asset object required
+        asset: Asset                 object required
 
         Raises:
         _______
         ValueError: If data URL is not provided
 
         ValueError: If headers are not provided
 
@@ -42,85 +41,118 @@
         self.headers = headers
         self.asset = asset
         self.market = market
 
         self.yesterday = ""
         self.day_before_yesterday = ""
 
+    ##################################################
+    # /////////////// Filter Stocks \\\\\\\\\\\\\\\\ #
+    ##################################################
+    def filter_stocks(
+        self,
+        price_greater_than: float,
+        change_condition: callable,
+        volume_greater_than: int,
+        trade_count_greater_than: int,
+        total_returned: int,
+        ascending_order: bool,
+    ) -> pd.DataFrame:
+        """
+        Filter stocks based on given parameters.
+
+        Args:
+            price_greater_than: The minimum price threshold for the stocks.
+            change_condition: A callable function that takes in a DataFrame and returns a boolean value.
+                This function is used to filter the stocks based on a specific change condition.
+            volume_greater_than: The minimum volume threshold for the stocks.
+            trade_count_greater_than: The minimum trade count threshold for the stocks.
+            total_returned: The number of stocks to return.
+            ascending_order: A boolean value indicating whether to sort the stocks in ascending order by change value.
+
+        Returns:
+            A pandas DataFrame containing the filtered stocks.
+        """
+        self.set_dates()
+        df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
+        df = df[df["price"] > price_greater_than]
+        df = df[change_condition(df)]
+        df = df[df["volume"] > volume_greater_than]
+        df = df[df["trades"] > trade_count_greater_than]
+        return df.sort_values(by="change", ascending=ascending_order).reset_index(drop=True).head(total_returned)
+
+    ##################################################
+    # //////////////// Get Losers \\\\\\\\\\\\\\\\\\ #
+    ##################################################
     def losers(
         self,
         price_greater_than: float = 5.0,
         change_less_than: float = -2.0,
         volume_greater_than: int = 20000,
         trade_count_greater_than: int = 2000,
         total_losers_returned: int = 100,
     ) -> pd.DataFrame:
         """
-        This method filters and returns a DataFrame of stock losers based on specific criteria.
+        Returns a filtered DataFrame of stocks that meet the specified conditions for losers.
 
         Args:
-            price_greater_than (float): The minimum price of the losers. Defaults to 5.0.
-            change_less_than (float): The maximum change percentage of the losers. Defaults to -2.0.
-            volume_greater_than (int): The minimum trading volume of the losers. Defaults to 20000.
-            trade_count_greater_than (int): The minimum trade count of the losers. Defaults to 2000.
-            total_losers_returned (int): The number of losers to be returned. Defaults to 100.
+            price_greater_than (float): The minimum price threshold for stocks to be considered losers. Default is 5.0.
+            change_less_than (float): The maximum change threshold for stocks to be considered losers. Default is -2.0.
+            volume_greater_than (int): The minimum volume threshold for stocks to be considered losers. Default is 20000.
+            trade_count_greater_than (int): The minimum trade count threshold for stocks to be considered losers. Default is 2000.
+            total_losers_returned (int): The maximum number of losers to be returned. Default is 100.
 
         Returns:
-            pd.DataFrame: DataFrame containing the filtered stock losers sorted by change percentage in ascending order.
-
-        Example:
-            losers_df = losers(price_greater_than=10.0, change_less_than=-5.0, volume_greater_than=50000,
-            trade_count_greater_than=3000, total_losers_returned=50)
+            pd.DataFrame: A filtered DataFrame containing stocks that meet the specified conditions for losers.
         """
-        self.set_dates()
-
-        losers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
-
-        losers_df = losers_df[losers_df["price"] > price_greater_than]
-        losers_df = losers_df[losers_df["change"] < change_less_than]
-        losers_df = losers_df[losers_df["volume"] > volume_greater_than]
-        losers_df = losers_df[losers_df["trades"] > trade_count_greater_than]
-        return losers_df.sort_values(by="change", ascending=True).reset_index(drop=True).head(total_losers_returned)
+        return self.filter_stocks(
+            price_greater_than,
+            lambda df: df["change"] < change_less_than,
+            volume_greater_than,
+            trade_count_greater_than,
+            total_losers_returned,
+            ascending_order=True,
+        )
 
+    ##################################################
+    # //////////////// Get Gainers \\\\\\\\\\\\\\\\\ #
+    ##################################################
     def gainers(
         self,
         price_greater_than: float = 5.0,
         change_greater_than: float = 2.0,
         volume_greater_than: int = 20000,
         trade_count_greater_than: int = 2000,
         total_gainers_returned: int = 100,
     ) -> pd.DataFrame:
         """
         Args:
-            price_greater_than: The minimum price threshold for filtering gainers. Only gainers with prices greater
-            than this value will be included. Default is 5.0.
-            change_greater_than: The minimum change threshold for filtering gainers. Only gainers with changes greater
-            than this value will be included. Default is 2.0.
-            volume_greater_than: The minimum volume threshold for filtering gainers. Only gainers with volumes greater
-            than this value will be included. Default is 20000.
-            trade_count_greater_than: The minimum trade count threshold for filtering gainers. Only gainers with trade
-            counts greater than this value will be included. Default is 2000.
-            total_gainers_returned: The total number of gainers to be returned. Only the top gainers based on their
-            change will be included. Default is 100.
+            price_greater_than (float): The minimum price threshold for the stocks to be included in the gainers list. Default is 5.0.
+            change_greater_than (float): The minimum change (in percentage) threshold for the stocks to be included in the gainers list.
+            Default is 2.0.
+            volume_greater_than (int): The minimum volume threshold for the stocks to be included in the gainers list. Default is 20000.
+            trade_count_greater_than (int): The minimum trade count threshold for the stocks to be included in the gainers list. Default is 2000.
+            total_gainers_returned (int): The maximum number of gainers to be returned. Default is 100.
 
         Returns:
-            pd.DataFrame: A DataFrame that contains the filtered gainers that satisfy the given thresholds.
-            The DataFrame is sorted by the "change" column in descending order and is limited to the specified
-            number of gainers.
-        """
-        self.set_dates()
-
-        gainers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
+            pd.DataFrame: A Pandas DataFrame containing the stocks that satisfy the criteria for being gainers.
 
-        gainers_df = gainers_df[gainers_df["price"] > price_greater_than]
-        gainers_df = gainers_df[gainers_df["change"] > change_greater_than]
-        gainers_df = gainers_df[gainers_df["volume"] > volume_greater_than]
-        gainers_df = gainers_df[gainers_df["trades"] > trade_count_greater_than]
-        return gainers_df.sort_values(by="change", ascending=False).reset_index(drop=True).head(total_gainers_returned)
+        """
+        return self.filter_stocks(
+            price_greater_than,
+            lambda df: df["change"] > change_greater_than,
+            volume_greater_than,
+            trade_count_greater_than,
+            total_gainers_returned,
+            ascending_order=False,
+        )
 
+    ##################################################
+    # /////////// Calculate Percentages \\\\\\\\\\\\ #
+    ##################################################
     def _get_percentages(
         self,
         start: str,
         end: str,
         timeframe: str = "1Day",
     ) -> pd.DataFrame:
         """Get percentage changes for the previous day
@@ -195,28 +227,24 @@
                         "change": change,
                         "price": bar[1][1]["c"],
                         "volume": bar[1][1]["v"],
                         "trades": bar[1][1]["n"],
                     }
                     all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
 
-                except Exception:
+                except KeyError:
                     pass
             all_bars_df.reset_index(drop=True, inplace=True)
             return all_bars_df
         else:
             raise ValueError(f"Failed to get assets. Response: {response.text}")
 
-    @staticmethod
-    def get_previous_date(current_date, day_to_look):
-        """
-        Get the previous date based on the day_to_look from the current_date.
-        """
-        return current_date.previous(day_to_look).strftime("%Y-%m-%d")
-
+    ##################################################
+    # ///////////////// Set Dates \\\\\\\\\\\\\\\\\\ #
+    ##################################################
     def set_dates(self):
         """
         Sets the dates for the screener.
 
         This method retrieves the last two trading dates from the market calendar
         and assigns them to the `yesterday` and `day_before_yesterday` attributes.
 
@@ -232,10 +260,7 @@
             )
             .tail(2)
             .reset_index(drop=True)
         )
 
         self.yesterday = calender.iloc[1]["date"].strftime("%Y-%m-%d")
         self.day_before_yesterday = calender.iloc[0]["date"].strftime("%Y-%m-%d")
-
-        print(f"Yesterday: {self.yesterday}")
-        print(f"Day Before Yesterday: {self.day_before_yesterday}")
```

### Comparing `py_alpaca_api-0.6.0/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.6.1/py_alpaca_api/src/watchlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         Returns:
             WatchlistClass: The updated watchlist.
 
         Raises:
             ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor `watchlist_name` are provided.
 
         """
-        # Check if both watchlist_id and watchlist_name are provided and raise an error if they are
+
         if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
         # Check if watchlist_id is provided
         if watchlist_id:
             watchlist = self.get(watchlist_id=watchlist_id)
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
```

### Comparing `py_alpaca_api-0.6.0/pyproject.toml` & `py_alpaca_api-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.6.0/PKG-INFO` & `py_alpaca_api-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,27 @@
-Metadata-Version: 2.1
-Name: py-alpaca-api
-Version: 0.6.0
-Summary: Python package, for communicating with Alpaca Markets REST API.
-Home-page: https://github.com/TexasCoding/py-alpaca-api
-License: MIT
-Keywords: alpaca,python
-Author: TexasCoding
-Author-email: jeff10278@me.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: pendulum (>=3.0.0,<4.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">PY-ALPACA-API</h1>
 </p>
 <p align="center">
-    <em>Empowering Alpaca Trading API with Python</em>
+    <em>Empower Trading with Seamless Alpaca API Integration</em>
 </p>
 <p align="center">
-<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
+   <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
 	<img src="https://img.shields.io/github/license/TexasCoding/py-alpaca-api?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
 	<img src="https://img.shields.io/github/last-commit/TexasCoding/py-alpaca-api?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 	<img src="https://img.shields.io/github/languages/top/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-top-language">
 	<img src="https://img.shields.io/github/languages/count/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-language-count">
 <p>
 <p align="center">
 	<!-- default option, no dependency badges. -->
    <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
    <img alt="Poetry" src="https://img.shields.io/badge/Poetry-%233B82F6.svg?style=for-the-badge&logo=poetry&logoColor=0B3D8D">
-
 </p>
 
 <br><!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary><br>
 
 - [ Overview](#-overview)
@@ -59,80 +37,100 @@
 - [ License](#-license)
 - [ Acknowledgments](#-acknowledgments)
 </details>
 <hr>
 
 ##  Overview
 
-The py-alpaca-api project facilitates seamless interaction with the Alpaca Markets REST API, offering a comprehensive suite of functionalities for trading and investment purposes. Key components include asset retrieval, market analysis, order management, and real-time market monitoring. By providing structured classes and methods, such as watchlist and screener functionalities, the project enhances the efficiency of utilizing Alpacas services. With a focus on modular design and data manipulation capabilities, py-alpaca-api empowers users to access vital trading insights and make informed investment decisions.
+The py-alpaca-api project provides a comprehensive Python interface for seamless interaction with the Alpaca API, offering functionalities such as accessing account information, retrieving asset data, managing market details, executing orders, and analyzing stock performance. By encapsulating key components like account, asset, order, and market classes, this project facilitates efficient data retrieval, trading operations, and market analysis within the Alpaca ecosystem. Integrated with GitHub Actions for testing integrity, py-alpaca-api enhances developers capabilities in integrating Alpacas features into diverse projects, emphasizing simplicity and reliability in financial data processing and trading activities.
 
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
-| ⚙️  | **Architecture**  | The project follows a structured architecture using classes like PyAlpacaApi, Watchlist, Screener, Position, Order, Market, and others for specific API interactions. This modular design enhances functionality and maintainability. |
-| 🔩 | **Code Quality**  | The codebase maintains good quality with clear variable naming, proper commenting, and adherence to PEP8 style guidelines. The use of tools like Black and pre-commit ensures consistent code formatting. |
-| 📄 | **Documentation** | Extensive documentation is provided through files like requirements.txt, pyproject.toml, and inline comments. Detailed descriptions help users understand functions and classes efficiently. Proper metadata and dependencies are also outlined. |
-| 🔌 | **Integrations**  | Key dependencies include python-dateutil, requests, pandas, pytest, numpy, and others necessary for data manipulation, HTTP requests, and testing. GitHub Actions are used for CI/CD processes. |
-| 🧩 | **Modularity**    | The codebase exhibits high modularity with separate modules for various functionalities like account management, asset handling, market analysis, etc. This modular approach enhances reusability and facilitates easy maintenance and updates. |
-| 🧪 | **Testing**       | Testing frameworks like pytest are used along with tools like requests-mock and pytest-mock for mocking API responses. Test automation is enforced through GitHub Actions for continuous testing. |
-| ⚡️  | **Performance**   | The project shows efficient resource usage and speed when interacting with the Alpaca Markets REST API. Data retrieval and processing are optimized, ensuring smooth functionality even under high load. |
-| 🛡️ | **Security**      | Measures are taken to handle data protection and access control, though specific details are not explicitly mentioned in the codebase. Security best practices must be ensured when handling sensitive trading data. |
-| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy, and others crucial for data manipulation and API interactions. Poetry is used for dependency management. |
+| ⚙️  | **Architecture**  | The project follows a modular architecture, with key components like `account.py`, `asset.py`, `market.py`, etc., encapsulating specific functionalities. This design enhances code organization and maintainability. |
+| 🔩 | **Code Quality**  | The codebase maintains high quality and follows PEP8 style conventions. It leverages tools like `black`, `flake8`, and `isort` for consistent formatting and clean code practices. |
+| 📄 | **Documentation** | The project includes detailed documentation in `pyproject.toml`, outlining metadata, dependencies, and structure. Inline code comments and docstrings enhance readability and understanding for developers. |
+| 🔌 | **Integrations**  | Key integrations include `requests`, `pandas`, `numpy`, etc., for data processing, HTTP requests, and financial analysis. External services like Alpaca API are seamlessly integrated for trading operations. |
+| 🧩 | **Modularity**    | The codebase exhibits high modularity, allowing for code reuse and easy maintenance. Each module focuses on specific tasks, promoting separation of concerns and enhancing scalability. |
+| 🧪 | **Testing**       | Testing frameworks such as `pytest` and `pytest-mock` are employed for unit testing. `pre-commit` ensures code quality checks before commits, maintaining robust test coverage. |
+| ⚡️  | **Performance**   | The project emphasizes efficiency and resource optimization, ensuring swift data retrieval and processing. Performance tuning techniques are implemented to enhance speed and responsiveness. |
+| 🛡️ | **Security**      | Security measures are in place for data protection and access control. Proper handling of API credentials and secure HTTP communication safeguard sensitive information. |
+| 📦 | **Dependencies**  | Key dependencies include `certifi`, `requests`, `pytz`, etc., facilitating API interaction, data manipulation, and time zone handling. These libraries enhance the project's functionality. |
 
 ---
 
 ##  Repository Structure
 
 ```sh
-   py_alpaca_api
-   ├── alpaca.py
-   └── src
-       ├── __init__.py
-       ├── account.py
-       ├── asset.py
-       ├── data_classes.py
-       ├── history.py
-       ├── market.py
-       ├── order.py
-       ├── position.py
-       ├── screener.py
-       └── watchlist.py
+py_alpaca_api 
+├── __init__.py
+├── alpaca.py
+└── src
+   ├── __init__.py
+   ├── account.py
+   ├── asset.py
+   ├── data_classes.py
+   ├── history.py
+   ├── market.py
+   ├── order.py
+   ├── position.py
+   ├── screener.py
+   └── watchlist.py
 ```
 
 ---
 
 ##  Modules
 
+<details closed><summary>.</summary>
+
+| File                                                                                          | Summary                                                                                                                                                                                                                                      |
+| ---                                                                                           | ---                                                                                                                                                                                                                                          |
+| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml)     | Defines dependencies and metadata for Python Alpaca API package.-Specifies version, description, authors, license, homepage, and repository.-Lists development, testing, and documentation dependencies.                                     |
+| [requirements.txt](https://github.com/TexasCoding/py-alpaca-api/blob/master/requirements.txt) | Specifies Python package dependencies for the repository based on version compatibility. Essential libraries for API integration and data processing are outlined, ensuring proper functioning and alignment with specified Python versions. |
+
+</details>
+
 <details closed><summary>py_alpaca_api</summary>
 
-| File                                                                                          | Summary                                                                                                                                                                                                                              |
-| ---                                                                                           | ---                                                                                                                                                                                                                                  |
-| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class initializing with API credentials for Alpaca trading. Sets URL based on trading type. Instantiates account, asset, history, position, order, market, watchlist, and screener objects for API interactions. |
+| File                                                                                          | Summary                                                                                                                                                                                                                                               |
+| ---                                                                                           | ---                                                                                                                                                                                                                                                   |
+| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class central to Alpaca API interaction. Initializes key components like account, asset, history, position, order, market, watchlist, and screener with API credentials and URLs for seamless data access and trading operations. |
+
+</details>
+
+<details closed><summary>.github.workflows</summary>
+
+| File                                                                                                            | Summary                                                                                                                           |
+| ---                                                                                                             | ---                                                                                                                               |
+| [test-package.yml](https://github.com/TexasCoding/py-alpaca-api/blob/master/.github/workflows/test-package.yml) | Verifies Python package build and tests integrity using GitHub Actions workflow test-package.yml in the py-alpaca-api repository. |
 
 </details>
 
 <details closed><summary>py_alpaca_api.src</summary>
 
-| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | This code file within the `py-alpaca-api` repository serves the critical purpose of providing a comprehensive set of classes and functions to interact with the Alpaca API effectively. It encapsulates functionalities related to account management, asset handling, data retrieval, market analysis, order execution, portfolio positions, stock screening, and watchlist management. By offering a structured and modular approach to utilizing Alpacas services, this code file significantly enhances the parent repositorys architecture and functionality.                          |
-| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Defines methods to retrieve top gainers and losers in the stock market by analyzing price, volume, and trade count. Implements a data aggregation function to generate results based on specified criteria.                                                                                                                                                                                                                                                                                                                                                                                 |
-| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, formats, and manages position data from the Alpaca Trade API, enabling actions like fetching all positions, getting specific positions, closing all positions, and closing a specific position. Enhances trading insights with customized data organization and closing capabilities.                                                                                                                                                                                                                                                                                            |
-| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | This code file, `screener.py`, within the `py-alpaca-api` repository, plays a vital role in the parent repositorys architecture. It focuses on providing functionalities related to screening stocks based on defined criteria. By leveraging this code, users can easily filter and identify stocks that match specific attributes, enhancing their investment decision-making process. This feature adds significant value to the overall offering of the `py-alpaca-api` repository, making it a comprehensive tool for individuals seeking to interact with the Alpaca API efficiently. |
-| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Defines Market class with clock method to retrieve market status from Alpaca API. Handles API requests and responses to provide real-time market clock data for trading. Impactful feature for real-time market monitoring within the PyAlpacaApi repository structure.                                                                                                                                                                                                                                                                                                                     |
-| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data from Alpaca API based on specified parameters. Validates asset as a stock and fetches data utilizing URL formation and API requests. Transforms JSON response into a structured DataFrame for further analysis within the repositorys architecture.                                                                                                                                                                                                                                                                                                         |
-| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file in the py-alpaca-api repository serves as a comprehensive interface for interacting with Alpacas API services. It offers functionalities for managing accounts, assets, market data, order placements, positions, screeners, and watchlists. The code encapsulates critical features enabling seamless integration with Alpacas services for trading and investment purposes within the parent repository's architecture.                                                                                                                                                    |
-| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using provided trade URL and headers. Supports fetching all assets based on status, asset class, and exchange. Implements error handling for unsuccessful requests.                                                                                                                                                                                                                                                                                                                                                                             |
-| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API using provided URL and headers. Implements a method to return account details as an object. Handles successful and unsuccessful responses appropriately.                                                                                                                                                                                                                                                                                                                                                                                      |
+| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account activities for a specific type, ensuring valid date usage. Fetches account information from Alpaca API and portfolio history data, transforming timestamps. Maintains DataFrame consistency and raises exceptions for failed requests.                                                                                                                                                                                                                        |
+| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from Alpaca API using given parameters. Utilizes requests to fetch data, then processes and returns it in a structured format. Maps API responses to custom AssetClass objects for ease of use.                                                                                                                                                                                                                                                     |
+| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file, `alpaca.py`, serves as a crucial component within the `py-alpaca-api` repository. It encapsulates functionalities related to interacting with the Alpaca API, including handling account information, managing assets, and executing orders. By providing a streamlined interface for accessing Alpacas services, this module enhances the overall capability of the repository, enabling seamless integration of Alpacas features into broader projects.       |
+| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieves historical stock data, validates if an asset is a stock, and preprocesses data. Supports fetching data based on symbol, timeframe, and date range. Ensures data integrity and format consistency for analysis within the parent repositorys Alpaca API integration.                                                                                                                                                                                                   |
+| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Implements Market class with methods for retrieving calendar data and market clock status from Alpaca API. Provides functionalities to fetch, process, and return market-related information in a structured format.                                                                                                                                                                                                                                                            |
+| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | Watchlist.py`The `watchlist.py` file in the `py-alpaca-api` repository is crucial for managing and tracking user-defined watchlists of assets within the Alpaca trading platform. It enables users to create, update, and retrieve custom watchlists, providing a streamlined approach to monitor specific assets of interest. By utilizing this module, users can easily curate and monitor their preferred assets, enhancing their trading experience on the Alpaca platform. |
+| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves, processes, and manages Alpaca account positions, providing data in DataFrame format, individual position details, and options to close positions individually or all at once. Maintains accuracy and consistency in position-related actions within the Alpaca API ecosystem.                                                                                                                                                                                        |
+| [screener.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/screener.py)         | Analyzes stock winners and losers by filtering data based on preset criteria. Retrieves and ranks stock performances for the previous day, with options to customize filter thresholds. Requires asset and market context for accurate analysis.                                                                                                                                                                                                                                |
+| [watchlist.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/watchlist.py)       | Retrieval, creation, updating, deletion, and asset management. Encapsulates request handling, response processing, and error management. conforms to the parent repositorys architecture by structuring functionality into distinct modules.                                                                                                                                                                                                                                    |
 
 </details>
 
+---
+
 ##  Getting Started
 
 **System Requirements:**
 
 * **Python**: `version x.y.z`
 
 ###  Installation
@@ -148,15 +146,15 @@
 > 2. Change to the project directory:
 > ```console
 > $ cd py-alpaca-api
 > ```
 >
 > 3. Install the dependencies:
 > ```console
-> $ poetry install
+> $ pip install -r requirements.txt
 > ```
 
 ###  Usage
 
 <h4>From <code>source</code></h4>
 
 > Run py-alpaca-api using the command below:
@@ -214,19 +212,18 @@
 </p>
 </details>
 
 ---
 
 ##  License
 
-This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.
+This project is protected under the [MIT]() License. For more details, refer to the [LICENSE](https://github.com/TexasCoding/py-alpaca-api/blob/master/LICENSE) file.
 
 ---
 
 ##  Acknowledgments
 
 - List any resources, contributors, inspiration, etc. here.
 
 [**Return**](#-overview)
 
 ---
-
```

