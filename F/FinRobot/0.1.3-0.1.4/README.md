# Comparing `tmp/finrobot-0.1.3.tar.gz` & `tmp/finrobot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finrobot-0.1.3.tar", last modified: Thu May 23 14:53:41 2024, max compression
+gzip compressed data, was "finrobot-0.1.4.tar", last modified: Wed May 29 10:16:57 2024, max compression
```

## Comparing `finrobot-0.1.3.tar` & `finrobot-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.264455 finrobot-0.1.3/
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.263994 finrobot-0.1.3/FinRobot.egg-info/
--rw-r--r--   0 wangneng   (501) staff       (20)     1400 2024-05-23 14:53:41.000000 finrobot-0.1.3/FinRobot.egg-info/PKG-INFO
--rw-r--r--   0 wangneng   (501) staff       (20)      797 2024-05-23 14:53:41.000000 finrobot-0.1.3/FinRobot.egg-info/SOURCES.txt
--rw-r--r--   0 wangneng   (501) staff       (20)        1 2024-05-23 14:53:41.000000 finrobot-0.1.3/FinRobot.egg-info/dependency_links.txt
--rw-r--r--   0 wangneng   (501) staff       (20)      178 2024-05-23 14:53:41.000000 finrobot-0.1.3/FinRobot.egg-info/requires.txt
--rw-r--r--   0 wangneng   (501) staff       (20)        9 2024-05-23 14:53:41.000000 finrobot-0.1.3/FinRobot.egg-info/top_level.txt
--rw-r--r--   0 wangneng   (501) staff       (20)    11380 2024-05-23 06:34:32.000000 finrobot-0.1.3/LICENSE
--rw-r--r--   0 wangneng   (501) staff       (20)     1400 2024-05-23 14:53:41.264260 finrobot-0.1.3/PKG-INFO
--rw-r--r--   0 wangneng   (501) staff       (20)    15552 2024-05-23 14:51:01.000000 finrobot-0.1.3/README.md
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.259712 finrobot-0.1.3/finrobot/
--rw-r--r--   0 wangneng   (501) staff       (20)        0 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/__init__.py
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.260525 finrobot-0.1.3/finrobot/agents/
--rw-r--r--   0 wangneng   (501) staff       (20)        1 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/agents/__init__.py
--rw-r--r--   0 wangneng   (501) staff       (20)     6649 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/agents/agent_library.py
--rw-r--r--   0 wangneng   (501) staff       (20)      621 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/agents/utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)     3967 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/agents/workflow.py
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.261886 finrobot-0.1.3/finrobot/data_source/
--rw-r--r--   0 wangneng   (501) staff       (20)      429 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/data_source/__init__.py
--rw-r--r--   0 wangneng   (501) staff       (20)    10324 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/data_source/finnhub_utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)    14297 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/data_source/finnlp_utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)     7867 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/data_source/fmp_utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)     3054 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/data_source/sec_utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)     4246 2024-05-23 14:51:01.000000 finrobot-0.1.3/finrobot/data_source/yfinance_utils.py
-drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 14:53:41.263786 finrobot-0.1.3/finrobot/functional/
--rw-r--r--   0 wangneng   (501) staff       (20)      251 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/__init__.py
--rw-r--r--   0 wangneng   (501) staff       (20)    18299 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/analyzer.py
--rw-r--r--   0 wangneng   (501) staff       (20)     8790 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/charting.py
--rw-r--r--   0 wangneng   (501) staff       (20)     3107 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/coding.py
--rw-r--r--   0 wangneng   (501) staff       (20)     7357 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/quantitative.py
--rw-r--r--   0 wangneng   (501) staff       (20)    15099 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/reportlab.py
--rw-r--r--   0 wangneng   (501) staff       (20)      780 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/functional/text.py
--rw-r--r--   0 wangneng   (501) staff       (20)     3133 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/toolkits.py
--rw-r--r--   0 wangneng   (501) staff       (20)     2537 2024-05-23 02:46:09.000000 finrobot-0.1.3/finrobot/utils.py
--rw-r--r--   0 wangneng   (501) staff       (20)       38 2024-05-23 14:53:41.264489 finrobot-0.1.3/setup.cfg
--rw-r--r--   0 wangneng   (501) staff       (20)     1553 2024-05-23 14:53:33.000000 finrobot-0.1.3/setup.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.453399 finrobot-0.1.4/
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.452791 finrobot-0.1.4/FinRobot.egg-info/
+-rw-r--r--   0 wangneng   (501) staff       (20)     1487 2024-05-29 10:16:57.000000 finrobot-0.1.4/FinRobot.egg-info/PKG-INFO
+-rw-r--r--   0 wangneng   (501) staff       (20)      797 2024-05-29 10:16:57.000000 finrobot-0.1.4/FinRobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)        1 2024-05-29 10:16:57.000000 finrobot-0.1.4/FinRobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)      220 2024-05-29 10:16:57.000000 finrobot-0.1.4/FinRobot.egg-info/requires.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)        9 2024-05-29 10:16:57.000000 finrobot-0.1.4/FinRobot.egg-info/top_level.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)    11380 2024-05-23 06:34:32.000000 finrobot-0.1.4/LICENSE
+-rw-r--r--   0 wangneng   (501) staff       (20)     1487 2024-05-29 10:16:57.453173 finrobot-0.1.4/PKG-INFO
+-rw-r--r--   0 wangneng   (501) staff       (20)    17641 2024-05-29 06:07:03.000000 finrobot-0.1.4/README.md
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.447684 finrobot-0.1.4/finrobot/
+-rw-r--r--   0 wangneng   (501) staff       (20)        0 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/__init__.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.448936 finrobot-0.1.4/finrobot/agents/
+-rw-r--r--   0 wangneng   (501) staff       (20)        1 2024-05-23 14:51:01.000000 finrobot-0.1.4/finrobot/agents/__init__.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     6692 2024-05-29 10:15:12.000000 finrobot-0.1.4/finrobot/agents/agent_library.py
+-rw-r--r--   0 wangneng   (501) staff       (20)      621 2024-05-23 14:51:01.000000 finrobot-0.1.4/finrobot/agents/utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     5486 2024-05-29 10:15:12.000000 finrobot-0.1.4/finrobot/agents/workflow.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.450204 finrobot-0.1.4/finrobot/data_source/
+-rw-r--r--   0 wangneng   (501) staff       (20)      429 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/data_source/__init__.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    10324 2024-05-23 14:51:01.000000 finrobot-0.1.4/finrobot/data_source/finnhub_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    14297 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/data_source/finnlp_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     7867 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/data_source/fmp_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3054 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/data_source/sec_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     4246 2024-05-23 14:51:01.000000 finrobot-0.1.4/finrobot/data_source/yfinance_utils.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-29 10:16:57.452477 finrobot-0.1.4/finrobot/functional/
+-rw-r--r--   0 wangneng   (501) staff       (20)      251 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/__init__.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    18299 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/analyzer.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     8790 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/charting.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3107 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/coding.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     7357 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/quantitative.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    15099 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/reportlab.py
+-rw-r--r--   0 wangneng   (501) staff       (20)      780 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/functional/text.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3133 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/toolkits.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     2537 2024-05-23 02:46:09.000000 finrobot-0.1.4/finrobot/utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)       38 2024-05-29 10:16:57.453443 finrobot-0.1.4/setup.cfg
+-rw-r--r--   0 wangneng   (501) staff       (20)     1553 2024-05-29 10:16:46.000000 finrobot-0.1.4/setup.py
```

### Comparing `finrobot-0.1.3/FinRobot.egg-info/PKG-INFO` & `finrobot-0.1.4/FinRobot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinRobot
-Version: 0.1.3
+Version: 0.1.4
 Summary: FinRobot: An Open-Source AI Agent Platform for Financial Applications using LLMs
 Home-page: https://github.com/AI4Finance-Foundation/FinRobot
 Author: AI4Finance Foundation
 Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Financial Large Language Models,AI Agents
 Platform: any
@@ -25,16 +25,19 @@
 Requires-Dist: ipython
 Requires-Dist: huggingface_hub
 Requires-Dist: matplotlib
 Requires-Dist: finnhub-python
 Requires-Dist: yfinance
 Requires-Dist: mplfinance
 Requires-Dist: backtrader
+Requires-Dist: sec_api
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyPDF2
+Requires-Dist: reportlab
+Requires-Dist: pyautogen[retrievechat]
 Requires-Dist: setuptools>=41.4.0
 Requires-Dist: wheel>=0.33.6
 Requires-Dist: tushare
 Requires-Dist: pandas_datareader
 
 FinRobot
```

### Comparing `finrobot-0.1.3/FinRobot.egg-info/SOURCES.txt` & `finrobot-0.1.4/FinRobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/LICENSE` & `finrobot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/PKG-INFO` & `finrobot-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinRobot
-Version: 0.1.3
+Version: 0.1.4
 Summary: FinRobot: An Open-Source AI Agent Platform for Financial Applications using LLMs
 Home-page: https://github.com/AI4Finance-Foundation/FinRobot
 Author: AI4Finance Foundation
 Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Financial Large Language Models,AI Agents
 Platform: any
@@ -25,16 +25,19 @@
 Requires-Dist: ipython
 Requires-Dist: huggingface_hub
 Requires-Dist: matplotlib
 Requires-Dist: finnhub-python
 Requires-Dist: yfinance
 Requires-Dist: mplfinance
 Requires-Dist: backtrader
+Requires-Dist: sec_api
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyPDF2
+Requires-Dist: reportlab
+Requires-Dist: pyautogen[retrievechat]
 Requires-Dist: setuptools>=41.4.0
 Requires-Dist: wheel>=0.33.6
 Requires-Dist: tushare
 Requires-Dist: pandas_datareader
 
 FinRobot
```

### Comparing `finrobot-0.1.3/README.md` & `finrobot-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 <img align="center" src=figs/logo_white_background.jpg width="40%"/>
 </div>
 
 **FinRobot** is an AI Agent Platform that transcends the scope of FinGPT, representing a comprehensive solution meticulously designed for financial applications. It integrates **a diverse array of AI technologies**, extending beyond mere language models. This expansive vision highlights the platform's versatility and adaptability, addressing the multifaceted needs of the financial industry.
 
 **Concept of AI Agent**: an AI Agent is an intelligent entity that uses large language models as its brain to perceive its environment, make decisions, and execute actions. Unlike traditional artificial intelligence, AI Agents possess the ability to independently think and utilize tools to progressively achieve given objectives.
 
+[Whitepaper of FinRobot](https://arxiv.org/abs/2405.14767)
+
 [![](https://dcbadge.vercel.app/api/server/trsr8SXpW5)](https://discord.gg/trsr8SXpW5)
 
 ## FinRobot Ecosystem
 <div align="center">
 <img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/6b30d9c1-35e5-4d36-a138-7e2769718f62" width="90%"/>
 </div>
 
@@ -58,15 +60,15 @@
 The main folder **finrobot** has three subfolders **agents, data_source, functional**. 
 
 ```
 FinRobot
 ├── finrobot (main folder)
 │   ├── agents
 │   	├── agent_library.py
-│   	└── data_agents.py
+│   	└── workflow.py
 │   ├── data_source
 │   	├── finnhub_utils.py
 │   	├── finnlp_utils.py
 │   	├── fmp_utils.py
 │   	├── sec_utils.py
 │   	└── yfinance_utils.py
 │   ├── functional
@@ -79,61 +81,77 @@
 │   ├── toolkits.py
 │   └── utils.py
 │
 ├── configs
 ├── experiments
 ├── tutorials_beginner (hands-on tutorial)
 │   ├── agent_fingpt_forecaster.ipynb
-├── tutorials_advanced (hands-on tutorial)
-│   ├── agent_annual_report.ipynb 
+│   └── agent_annual_report.ipynb 
+├── tutorials_advanced (advanced tutorials for potential finrobot developers)
 │   ├── agent_trade_strategist.ipynb
+│   ├── agent_fingpt_forecaster.ipynb
+│   ├── agent_annual_report.ipynb 
 │   ├── lmm_agent_mplfinance.ipynb
 │   └── lmm_agent_opt_smacross.ipynb
 ├── setup.py
 ├── OAI_CONFIG_LIST_sample
 ├── config_api_keys_sample
 ├── requirements.txt
 └── README.md
 ```
 
 ## Installation:
-1. download the FinRobot repo use terminal or download it manually 
+
+**1. (Recommended) Create a new virtual environment**
+```shell
+conda create --name finrobot python=3.10
+conda activate finrobot
+```
+**2. download the FinRobot repo use terminal or download it manually**
 ```shell
 git clone https://github.com/AI4Finance-Foundation/FinRobot.git
+cd FinRobot
 ```
-2. install dependencies
-cd into this repository
+**3. install finrobot & dependencies from source or pypi**
+
+get our latest release from pypi
 ```bash
-cd FinRobot
-pip install FinRobot
+pip install -U finrobot
+```
+or install from this repo directly
+```
+pip install -e .
 ```
-3. modify OAI_CONFIG_LIST_sample file
+**4. modify OAI_CONFIG_LIST_sample file**
 ```shell
 1) rename OAI_CONFIG_LIST_sample to OAI_CONFIG_LIST
 2) remove the four lines of comment within the OAI_CONFIG_LIST file
 3) add your own openai api-key <your OpenAI API key here>
 ```
-4. modify config_api_keys_sample file
+**5. modify config_api_keys_sample file**
 ```shell
 1) rename config_api_keys_sample to config_api_keys
 2) remove the comment within the config_api_keys file
 3) add your own finnhub-api "YOUR_FINNHUB_API_KEY"
 4) add your own financialmodelingprep and sec-api keys "YOUR_FMP_API_KEY" and "YOUR_SEC_API_KEY" (for financial report generation)
 ```
-5. Run tutorials, use jupyter notebook navigate to the tutorials folder
-```shell
-#run these notebooks
+**6. start navigating the tutorials or the demos below:**
+```
+# find these notebooks in tutorials
 1) agent_annual_report.ipynb
 2) agent_fingpt_forecaster.ipynb
 3) agent_trade_strategist.ipynb
 4) lmm_agent_mplfinance.ipynb
 5) lmm_agent_opt_smacross.ipynb
 ```
 
-### Example:
+## Demos
+### 1. Market Forecaster Agent (Predict Stock Movements Direction)
+Takes a company's ticker symbol, recent basic financials, and market news as input and predicts its stock movements.
+
 1. Import 
 ```python
 import autogen
 from finrobot.utils import get_current_date, register_keys_from_json
 from finrobot.agents.workflow import SingleAssistant
 ```
 2. Config
@@ -149,56 +167,107 @@
 }
 
 # Register FINNHUB API keys
 register_keys_from_json("../config_api_keys")
 ```
 3. Run
 ```python
-company = "AAPL"
+company = "NVDA"
 
 assitant = SingleAssistant(
     "Market_Analyst",
     llm_config,
     # set to "ALWAYS" if you want to chat instead of simply receiving the prediciton
     human_input_mode="NEVER",
 )
 assitant.chat(
     f"Use all the tools provided to retrieve information available for {company} upon {get_current_date()}. Analyze the positive developments and potential concerns of {company} "
     "with 2-4 most important factors respectively and keep them concise. Most factors should be inferred from company related news. "
     f"Then make a rough prediction (e.g. up/down by 2-3%) of the {company} stock price movement for next week. Provide a summary analysis to support your prediction."
 )
 ```
+4. Result
+<div align="center">
+<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/812ec23a-9cb3-4fad-b716-78533ddcd9dc" width="40%"/>
+<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/9a2f9f48-b0e1-489c-8679-9a4c530f313c" width="41%"/>
+</div>
 
-## Demos
-### 1. Financial Analyst Agent for Report Writing (Equity Research Report)
-Take a company's 10-k form, financial data as input and output an equity research report
-1. **Gather Preliminary Data**: 10-K report
-2. **Analyze Financial Statements**: balance sheet, income statement, cash flow
-3. **Company Overview and Performance**: company description, business highlights, segment analysis
-4. **Risk Assessment**: assess risks
-5. **Financial Performance Visualization**:  plot PE ratio and EPS
-6. **Synthesize Findings into Paragraphs**: combine all parts into a coherent summary
-7. **Generate PDF Report**: use tools to generate PDF automatically
-8. **Quality Assurance**: check word counts
+### 2. Financial Analyst Agent for Report Writing (Equity Research Report)
+Take a company's 10-k form, financial data, and market data as input and output an equity research report
 
-check out the report folder for more examples
+1. Import 
+```python
+import os
+import autogen
+from textwrap import dedent
+from finrobot.utils import register_keys_from_json
+from finrobot.agents.workflow import SingleAssistantShadow
+```
+2. Config
+```python
+llm_config = {
+    "config_list": autogen.config_list_from_json(
+        "../OAI_CONFIG_LIST",
+        filter_dict={
+            "model": ["gpt-4-0125-preview"],
+        },
+    ),
+    "timeout": 120,
+    "temperature": 0.5,
+}
+register_keys_from_json("../config_api_keys")
 
-<div align="center">
-<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/d2d999e0-dc0e-4196-aca1-218f5fadcc5b" width="60%"/>
-</div>
+# Intermediate strategy modules will be saved in this directory
+work_dir = "../report"
+os.makedirs(work_dir, exist_ok=True)
 
+assistant = SingleAssistantShadow(
+    "Expert_Investor",
+    llm_config,
+    max_consecutive_auto_reply=None,
+    human_input_mode="TERMINATE",
+)
 
-### 2. Market Forecaster Agent (Predict Stock Movements Direction)
-Takes a company's ticker symbol, recent basic financials and market news as input and predict its stock movements.
+```
+3. Run
+```python
+company = "Microsoft"
+fyear = "2023"
+
+message = dedent(
+    f"""
+    With the tools you've been provided, write an annual report based on {company}'s {fyear} 10-k report, format it into a pdf.
+    Pay attention to the followings:
+    - Explicitly explain your working plan before you kick off.
+    - Use tools one by one for clarity, especially when asking for instructions. 
+    - All your file operations should be done in "{work_dir}". 
+    - Display any image in the chat once generated.
+    - All the paragraphs should combine between 400 and 450 words, don't generate the pdf until this is explicitly fulfilled.
+"""
+)
 
+assistant.chat(message, use_cache=True, max_turns=50,
+               summary_method="last_msg")
+```
+4. Result
 <div align="center">
-<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/812ec23a-9cb3-4fad-b716-78533ddcd9dc" width="40%"/>
-<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/9a2f9f48-b0e1-489c-8679-9a4c530f313c" width="41%"/>
+<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/d2d999e0-dc0e-4196-aca1-218f5fadcc5b" width="60%"/>
+<img align="center" src="https://github.com/AI4Finance-Foundation/FinRobot/assets/31713746/3a21873f-9498-4d73-896b-3740bf6d116d" width="60%"/>
 </div>
 
+**Financial CoT**:
+1. **Gather Preliminary Data**: 10-K report, market data, financial ratios
+2. **Analyze Financial Statements**: balance sheet, income statement, cash flow
+3. **Company Overview and Performance**: company description, business highlights, segment analysis
+4. **Risk Assessment**: assess risks
+5. **Financial Performance Visualization**:  plot PE ratio and EPS
+6. **Synthesize Findings into Paragraphs**: combine all parts into a coherent summary
+7. **Generate PDF Report**: use tools to generate PDF automatically
+8. **Quality Assurance**: check word counts
+
 ### 3. Trade Strategist Agent with multimodal capabilities
 
 
 ## AI Agent Papers
 
 + [Stanford University + Microsoft Research] [Agent AI: Surveying the Horizons of Multimodal Interaction](https://arxiv.org/abs/2401.03568)
 + [Stanford University] [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442)
@@ -229,10 +298,10 @@
 + [CrewAI (12.1k stars)](https://github.com/joaomdmoura/crewAI) is a framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks.
 + [XAgent (7.5k stars)](https://github.com/OpenBMB/XAgent) is an open-source experimental Large Language Model (LLM) driven autonomous agent that can automatically solve various tasks.
 + [Bisheng (5.5k stars)](https://github.com/dataelement/bisheng) is a leading open-source platform for developing LLM applications.
 + [Voyager (5.1k stars)](https://github.com/OpenBMB/XAgent) An Open-Ended Embodied Agent with Large Language Models.
 + [CAMEL (4.4k stars)](https://github.com/camel-ai/camel) is a framework that offers a comprehensive set of tools and algorithms for building multimodal AI Agents, enabling them to handle various data forms such as text, images, and speech.
 + [Langfuse (2.9k stars)](https://github.com/langfuse/langfuse) is a language fusion framework that can integrate the language abilities of multiple AI Agents, enabling them to simultaneously possess multilingual understanding and generation capabilities.
 
-**Disclaimer**: The codes provided herein are released for academic purposes under the MIT education license. They should not be construed as financial counsel or recommendations for live trading. It is imperative to exercise caution and consult with qualified financial professionals prior to any trading or investment actions.
+**Disclaimer**: The codes and documents provided herein are released under the Apache-2.0 license. They should not be construed as financial counsel or recommendations for live trading. It is imperative to exercise caution and consult with qualified financial professionals prior to any trading or investment actions.
```

### Comparing `finrobot-0.1.3/finrobot/agents/agent_library.py` & `finrobot-0.1.4/finrobot/agents/agent_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 library = [
     {
         "name": "Software_Developer",
         "profile": "As a Software Developer for this position, you must be able to work collaboratively in a group chat environment to complete tasks assigned by a leader or colleague, primarily using Python programming expertise, excluding the need for code interpretation skills.",
     },
     {
         "name": "Data_Analyst",
-        "profile": "As a Data Analyst for this position, you must be adept at analyzing data using Python, completing tasks assigned by leaders or colleagues, and collaboratively solving problems in a group chat setting with professionals of various roles.",
+        "profile": "As a Data Analyst for this position, you must be adept at analyzing data using Python, completing tasks assigned by leaders or colleagues, and collaboratively solving problems in a group chat setting with professionals of various roles. Reply 'TERMINATE' when everything is done.",
     },
     {
         "name": "Programmer",
         "profile": "As a Programmer for this position, you should be proficient in Python, able to effectively collaborate and solve problems within a group chat environment, and complete tasks assigned by leaders or colleagues without requiring expertise in code interpretation.",
     },
     {
         "name": "Accountant",
```

### Comparing `finrobot-0.1.3/finrobot/agents/utils.py` & `finrobot-0.1.4/finrobot/agents/utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/agents/workflow.py` & `finrobot-0.1.4/finrobot/agents/workflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .agent_library import library
 from typing import Any, Callable, Dict, List, Literal
 import autogen
 from autogen.cache import Cache
+from autogen.agentchat.contrib.retrieve_user_proxy_agent import RetrieveUserProxyAgent
 
 from ..toolkits import register_toolkits
 from .utils import *
 
 
 class FinRobot(autogen.AssistantAgent):
 
@@ -30,14 +31,17 @@
         assert bool(system_message), f"System message is required for {name}."
 
         super().__init__(orig_name, system_message, **kwargs)
         if proxy is not None:
             register_toolkits(self.toolkits, self, proxy)
 
 
+from autogen.agentchat.contrib.retrieve_assistant_agent import RetrieveAssistantAgent
+
+
 class SingleAssistant:
 
     def __init__(
         self,
         name: str,
         llm_config: Dict[str, Any] = {},
         is_termination_msg=lambda x: x.get("content", "")
@@ -46,14 +50,15 @@
         max_consecutive_auto_reply=10,
         code_execution_config={
             "work_dir": "coding",
             "use_docker": False,
         },
         **kwargs,
     ):
+
         self.user_proxy = autogen.UserProxyAgent(
             name="User_Proxy",
             is_termination_msg=is_termination_msg,
             human_input_mode=human_input_mode,
             max_consecutive_auto_reply=max_consecutive_auto_reply,
             code_execution_config=code_execution_config,
             **kwargs,
@@ -70,14 +75,57 @@
                 self.assistant,
                 message=message,
                 cache=cache if use_cache else None,
                 **kwargs,
             )
 
 
+class SingleAssistantRAG:
+
+    def __init__(
+        self,
+        name: str,
+        llm_config: Dict[str, Any] = {},
+        is_termination_msg=lambda x: x.get("content", "")
+        and x.get("content", "").endswith("TERMINATE"),
+        human_input_mode="NEVER",
+        max_consecutive_auto_reply=10,
+        code_execution_config={
+            "work_dir": "coding",
+            "use_docker": False,
+        },
+        retrieve_config=None,
+        **kwargs,
+    ):
+        self.user_proxy = RetrieveUserProxyAgent(
+            name="User_Proxy",
+            is_termination_msg=is_termination_msg,
+            human_input_mode=human_input_mode,
+            max_consecutive_auto_reply=max_consecutive_auto_reply,
+            code_execution_config=code_execution_config,
+            retrieve_config=retrieve_config,
+            **kwargs,
+        )
+        self.assistant = FinRobot(
+            name,
+            llm_config=llm_config,
+            proxy=self.user_proxy,
+        )
+
+    def chat(self, message: str, use_cache=False, **kwargs):
+        with Cache.disk() as cache:
+            self.user_proxy.initiate_chat(
+                self.assistant,
+                message=self.user_proxy.message_generator,
+                problem=message,
+                cache=cache if use_cache else None,
+                **kwargs,
+            )
+
+
 class SingleAssistantShadow(SingleAssistant):
 
     def __init__(
         self,
         name: str,
         llm_config: Dict[str, Any] = {},
         is_termination_msg=lambda x: x.get("content", "")
```

### Comparing `finrobot-0.1.3/finrobot/data_source/finnhub_utils.py` & `finrobot-0.1.4/finrobot/data_source/finnhub_utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/data_source/finnlp_utils.py` & `finrobot-0.1.4/finrobot/data_source/finnlp_utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/data_source/fmp_utils.py` & `finrobot-0.1.4/finrobot/data_source/fmp_utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/data_source/sec_utils.py` & `finrobot-0.1.4/finrobot/data_source/sec_utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/data_source/yfinance_utils.py` & `finrobot-0.1.4/finrobot/data_source/yfinance_utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/analyzer.py` & `finrobot-0.1.4/finrobot/functional/analyzer.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/charting.py` & `finrobot-0.1.4/finrobot/functional/charting.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/coding.py` & `finrobot-0.1.4/finrobot/functional/coding.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/quantitative.py` & `finrobot-0.1.4/finrobot/functional/quantitative.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/reportlab.py` & `finrobot-0.1.4/finrobot/functional/reportlab.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/functional/text.py` & `finrobot-0.1.4/finrobot/functional/text.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/toolkits.py` & `finrobot-0.1.4/finrobot/toolkits.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/finrobot/utils.py` & `finrobot-0.1.4/finrobot/utils.py`

 * *Files identical despite different names*

### Comparing `finrobot-0.1.3/setup.py` & `finrobot-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         REQUIRES = [line.split("#", 1)[0].strip() for line in f if line.strip()]
 except:
     print("'requirements.txt' not found!")
     REQUIRES = list()
 
 setup(
     name="FinRobot",
-    version="0.1.3",
+    version="0.1.4",
     include_package_data=True,
     author="AI4Finance Foundation",
     author_email="contact@ai4finance.org",
     url="https://github.com/AI4Finance-Foundation/FinRobot",
     license="MIT",
     packages=find_packages(),
     install_requires=REQUIRES,
```

