# Comparing `tmp/py_alpaca_daily_losers-0.3.0.tar.gz` & `tmp/py_alpaca_daily_losers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.3.0.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-0.3.1.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.3.0.tar` & `py_alpaca_daily_losers-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.0/LICENSE
--rw-r--r--   0        0        0    13887 2024-05-27 04:08:54.588515 py_alpaca_daily_losers-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    20680 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-27 03:42:55.091127 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/article_extractor.py
--rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/marketaux.py
--rw-r--r--   0        0        0     2527 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1927 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0      906 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/yahoo.py
--rw-r--r--   0        0        0      713 2024-05-27 16:16:51.833013 py_alpaca_daily_losers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/LICENSE
+-rw-r--r--   0        0        0    13887 2024-05-27 04:08:54.588515 py_alpaca_daily_losers-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0    21144 2024-05-28 23:12:37.168330 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-27 03:42:55.091127 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/article_extractor.py
+-rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/global_fuctions.py
+-rw-r--r--   0        0        0      936 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/marketaux.py
+-rw-r--r--   0        0        0     2527 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/openai.py
+-rw-r--r--   0        0        0     1927 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/slack.py
+-rw-r--r--   0        0        0      906 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/yahoo.py
+-rw-r--r--   0        0        0      713 2024-05-28 23:12:37.168330 py_alpaca_daily_losers-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    14591 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.3.1/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.3.0/LICENSE` & `py_alpaca_daily_losers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/README.md` & `py_alpaca_daily_losers-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/daily_losers.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,26 +86,27 @@
             send_message("No sell opportunities found.")
             return
 
         current_positions = self.alpaca.position.get_all()
         sold_positions = []
 
         for symbol in sell_opportunities:
-            if self.alpaca.market.clock().is_open:
-                try:
-                    qty = current_positions[current_positions["symbol"] == symbol]["qty"].values[0]
+            try:
+                qty = current_positions[
+                    current_positions["symbol"] == symbol
+                ]["qty"].values[0]
 
-                    self.alpaca.position.close(
-                        symbol_or_id=symbol, percentage=100
-                    )
-                except Exception as e:
-                    send_message(f"Error selling {symbol}: {e}")
-                    continue
-                else:
-                    sold_positions.append({"symbol": symbol, "qty": qty})
+                self.alpaca.position.close(
+                    symbol_or_id=symbol, percentage=100
+                )
+            except Exception as e:
+                send_message(f"Error selling {symbol}: {e}")
+                continue
+            else:
+                sold_positions.append({"symbol": symbol, "qty": qty})
 
         self._send_position_messages(sold_positions, "sell")
 
     ########################################################
     # Define the get_sell_opportunities method
     ########################################################
     def get_sell_opportunities(self) -> list:
@@ -115,25 +116,36 @@
         Returns:
             sell_list (list): A list of symbols representing potential sell opportunities.
         """
         current_positions = self.alpaca.position.get_all()
         if current_positions[current_positions["symbol"] != "Cash"].empty:
             return []
 
-        current_positions_symbols = current_positions[current_positions["symbol"] != "Cash"]["symbol"].tolist()
+        current_positions_symbols = current_positions[
+            current_positions["symbol"] != "Cash"
+        ]["symbol"].tolist()
 
         assets_history = self.get_ticker_data(current_positions_symbols)
 
-        sell_criteria = (((assets_history[["rsi14", "rsi30", "rsi50", "rsi200"]] >= 70).any(axis=1)) |
-                         ((assets_history[["bbhi14", "bbhi30", "bbhi50", "bbhi200"]] == 1).any(axis=1)))
+        sell_criteria = (
+            (assets_history[["rsi14", "rsi30", "rsi50", "rsi200"]] >= 70).any(
+                axis=1
+            )
+        ) | (
+            (
+                assets_history[["bbhi14", "bbhi30", "bbhi50", "bbhi200"]] == 1
+            ).any(axis=1)
+        )
 
         sell_filtered_df = assets_history[sell_criteria]
         sell_list = sell_filtered_df["symbol"].tolist()
 
-        percentage_change_list = current_positions[current_positions["profit_pct"] > 0.1]["symbol"].tolist()
+        percentage_change_list = current_positions[
+            current_positions["profit_pct"] > 0.1
+        ]["symbol"].tolist()
 
         for symbol in percentage_change_list:
             if symbol not in sell_list:
                 sell_list.append(symbol)
 
         return sell_list
 
@@ -160,34 +172,52 @@
 
         cash_row = current_positions[current_positions["symbol"] == "Cash"]
 
         total_holdings = current_positions["market_value"].sum()
         sold_positions = []
 
         if cash_row["market_value"][0] / total_holdings < 0.1:
-            current_positions = (current_positions[current_positions["symbol"] != "Cash"]
-                                 .sort_values(by="profit_pct", ascending=False))
-
-            top_performers = current_positions.iloc[:int(len(current_positions) // 2)]
+            current_positions = current_positions[
+                current_positions["symbol"] != "Cash"
+            ].sort_values(by="profit_pct", ascending=False)
+
+            top_performers = current_positions.iloc[
+                : int(len(current_positions) // 2)
+            ]
             top_performers_market_value = top_performers["market_value"].sum()
-            cash_needed = (total_holdings * 0.1 - cash_row["market_value"][0]) + 5.00
+            cash_needed = (
+                total_holdings * 0.1 - cash_row["market_value"][0]
+            ) + 5.00
 
             for index, row in top_performers.iterrows():
-                print(f"Selling {row['symbol']} to make cash 10% portfolio cash requirement")
-                amount_to_sell = int((row["market_value"] / top_performers_market_value) * cash_needed)
+                print(
+                    f"Selling {row['symbol']} to make cash 10% portfolio cash requirement"
+                )
+                amount_to_sell = int(
+                    (row["market_value"] / top_performers_market_value)
+                    * cash_needed
+                )
                 if amount_to_sell == 0:
                     continue
-                if self.alpaca.market.clock().is_open:
-                    try:
-                        self.alpaca.order.market(symbol=row["symbol"], notional=amount_to_sell, side="sell")
-                    except Exception as e:
-                        send_message(f"Error selling {row['symbol']}: {e}")
-                        continue
-                    else:
-                        sold_positions.append({"symbol": row["symbol"], "notional": round(amount_to_sell, 2)})
+                try:
+                    self.alpaca.order.market(
+                        symbol=row["symbol"],
+                        notional=amount_to_sell,
+                        side="sell",
+                    )
+                except Exception as e:
+                    send_message(f"Error selling {row['symbol']}: {e}")
+                    continue
+                else:
+                    sold_positions.append(
+                        {
+                            "symbol": row["symbol"],
+                            "notional": round(amount_to_sell, 2),
+                        }
+                    )
 
         self._send_position_messages(sold_positions, "liquidate")
 
     ########################################################
     # Define the check_for_buy_opportunities method
     ########################################################
     def check_for_buy_opportunities(self):
@@ -206,23 +236,25 @@
         class or its dependencies.
 
         """
         losers = self.get_daily_losers()
         tickers = self.filter_tickers_with_news(losers)
 
         if len(tickers) > 0:
-            print(f"{len(tickers)} buy opportunities found. Opening positions...")
+            print(
+                f"{len(tickers)} buy opportunities found. Opening positions..."
+            )
             self.open_positions(tickers=tickers)
         else:
             print("No buy opportunities found")
 
     ########################################################
     # Define the open_positions method
     ########################################################
-    def open_positions(self, tickers: list,  ticker_limit=8):
+    def open_positions(self, tickers: list, ticker_limit=8):
         """
         This method is used to open buying positions based on buy opportunities and openai sentiment.
         By default, it limits the number of stocks to 8.
 
         Parameters:
         - tickers: A list of ticker symbols for the stocks to be considered for opening positions.
         - ticker_limit: An optional parameter to limit the number of stocks to be considered. Default value is 8.
@@ -240,35 +272,38 @@
           - If the market is open, attempts to buy the stock using
           `self.alpaca.order.market(symbol=ticker, notional=notional)`.
           - If an exception occurs, sends an error message indicating the issue.
           - If the buy order is successful, adds the details of the bought position to `bought_positions`.
         - Calls `self._send_position_messages(bought_positions, "buy")` to send messages related to the
             bought positions.
         """
-        print("Buying orders based on buy opportunities and openai sentiment. Limit to 8 stocks by default")
+        print(
+            "Buying orders based on buy opportunities and openai sentiment. Limit to 8 stocks by default"
+        )
 
         available_cash = self.alpaca.account.get().cash
 
         if len(tickers) == 0:
             send_message("No tickers to buy.")
             return
         else:
             notional = (available_cash / len(tickers[:ticker_limit])) - 1
 
         bought_positions = []
 
         for ticker in tickers[:ticker_limit]:
-            if self.alpaca.market.clock().is_open:
-                try:
-                    self.alpaca.order.market(symbol=ticker, notional=notional)
-                except Exception as e:
-                    send_message(f"Error buying {ticker}: {e}")
-                    continue
-                else:
-                    bought_positions.append({"symbol": ticker, "notional": round(notional, 2)})
+            try:
+                self.alpaca.order.market(symbol=ticker, notional=notional)
+            except Exception as e:
+                send_message(f"Error buying {ticker}: {e}")
+                continue
+            else:
+                bought_positions.append(
+                    {"symbol": ticker, "notional": round(notional, 2)}
+                )
 
         self._send_position_messages(bought_positions, "buy")
 
     ########################################################
     # Define the update_or_create_watchlist method
     ########################################################
     def update_or_create_watchlist(self, name, symbols):
@@ -281,17 +316,18 @@
 
         Returns:
         None
 
         Raises:
         ValueError: If an error occurs while updating the watchlist, a new watchlist will be created instead.
         """
+        symbols = ','.join(symbols)
         try:
             self.alpaca.watchlist.update(watchlist_name=name, symbols=symbols)
-        except ValueError:
+        except Exception:
             self.alpaca.watchlist.create(name=name, symbols=symbols)
 
     ########################################################
     # Define the filter_tickers_with_news method
     ########################################################
     def filter_tickers_with_news(self, tickers) -> list:
         """
@@ -314,16 +350,16 @@
         """
         news = MarketAux()
         article = ArticleExtractor()
         openai = OpenAIAPI()
         filtered_tickers = []
 
         for i, ticker in tqdm(
-                enumerate(tickers),
-                desc=f"• Analyzing news for {len(tickers)} tickers, using OpenAI & MarketAux: ",
+            enumerate(tickers),
+            desc=f"• Analyzing news for {len(tickers)} tickers, using OpenAI & MarketAux: ",
         ):
             m_news = news.get_symbol_news(symbol=ticker)
             articles = article.extract_articles(m_news)
 
             if len(articles) > 0:
                 bullish = 0
                 bearish = 0
@@ -341,15 +377,17 @@
                 if bullish > bearish:
                     filtered_tickers.append(ticker)
 
         if len(filtered_tickers) == 0:
             print("No tickers with news found")
             return []
 
-        self.update_or_create_watchlist(name="DailyLosers", symbols=filtered_tickers)
+        self.update_or_create_watchlist(
+            name="DailyLosers", symbols=filtered_tickers
+        )
 
         return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
 
     ########################################################
     # Define the get_daily_losers method
     ########################################################
     def get_daily_losers(self) -> list:
@@ -370,16 +408,16 @@
         losers = self.buy_criteria(losers)
 
         if len(losers) == 0:
             send_message("No daily losers found.")
             return []
 
         for i, ticker in tqdm(
-                enumerate(losers),
-                desc=f"• Getting recommendations for {len(losers)} tickers, from Yahoo Finance: ",
+            enumerate(losers),
+            desc=f"• Getting recommendations for {len(losers)} tickers, from Yahoo Finance: ",
         ):
             sentiment = yahoo.get_sentiment(ticker)
             if sentiment == "NEUTRAL" or sentiment == "BEARISH":
                 losers.remove(ticker)
 
         self.update_or_create_watchlist(name="DailyLosers", symbols=losers)
 
@@ -401,26 +439,29 @@
         - A list of stock assets that meet the buy criteria.
 
         Example Usage:
         buy_criteria(data)
 
         """
 
-        buy_criteria = (((data[["bblo14", "bblo30", "bblo50", "bblo200"]] == 1).any(axis=1)) |
-                        ((data[["rsi14", "rsi30", "rsi50", "rsi200"]] <= 30).any(axis=1)))
+        buy_criteria = (
+            (data[["bblo14", "bblo30", "bblo50", "bblo200"]] == 1).any(axis=1)
+        ) | ((data[["rsi14", "rsi30", "rsi50", "rsi200"]] <= 30).any(axis=1))
 
         buy_filtered_data = data[buy_criteria]
 
         filtered_data = list(buy_filtered_data["symbol"])
 
         if len(filtered_data) == 0:
             print("No tickers meet the buy criteria")
             return []
 
-        self.update_or_create_watchlist(name="DailyLosers", symbols=filtered_data)
+        self.update_or_create_watchlist(
+            name="DailyLosers", symbols=filtered_data
+        )
 
         return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
 
     ########################################################
     # Define the get_ticker_data method
     ########################################################
     def get_ticker_data(self, tickers) -> pd.DataFrame:
@@ -433,18 +474,18 @@
         Returns:
             pd.DataFrame: DataFrame containing technical data for the tickers.
 
         """
         df_tech = []
 
         for i, ticker in tqdm(
-                enumerate(tickers),
-                desc="• Analyzing ticker data for "
-                     + str(len(tickers))
-                     + " symbols from Alpaca API",
+            enumerate(tickers),
+            desc="• Analyzing ticker data for "
+            + str(len(tickers))
+            + " symbols from Alpaca API",
         ):
             try:
                 history = self.alpaca.history.get_stock_data(
                     symbol=ticker, start=year_ago, end=previous_day
                 )
             except ValueError:
                 continue
@@ -473,15 +514,14 @@
 
         return df_tech
 
     ########################################################
     # Define the _send_position_messages method
     ########################################################
     def _send_position_messages(self, positions: list, pos_type: str):
-
         """
         Sends position messages based on the type of position.
         Args:
             positions (list): List of position dictionaries.
             pos_type (str): Type of position ("buy", "sell", or "liquidate").
         Returns:
             bool: True if message was sent successfully, False otherwise.
@@ -491,20 +531,24 @@
             "buy": "bought",
             "liquidate": "liquidated",
         }
 
         try:
             position_name = position_names[pos_type]
         except KeyError:
-            raise ValueError('Invalid type. Must be "sell", "buy", or "liquidate".')
+            raise ValueError(
+                'Invalid type. Must be "sell", "buy", or "liquidate".'
+            )
 
         if not positions:
             position_message = f"No positions to {pos_type}"
         else:
-            is_market_open = "" if self.alpaca.market.clock().is_open else " pretend"
+            is_market_open = (
+                "" if self.alpaca.market.clock().is_open else " pretend"
+            )
             position_message = f"Successfully{is_market_open} {position_name} the following positions:\n"
 
             for position in positions:
 
                 if position_name == "liquidated":
                     qty_key = "notional"
                 elif position_name == "sold":
```

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/article_extractor.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/article_extractor.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/marketaux.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/marketaux.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/py_alpaca_daily_losers/src/yahoo.py` & `py_alpaca_daily_losers-0.3.1/py_alpaca_daily_losers/src/yahoo.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.3.0/pyproject.toml` & `py_alpaca_daily_losers-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "0.3.0"
+version = "0.3.1"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1.0.1"
```

### Comparing `py_alpaca_daily_losers-0.3.0/PKG-INFO` & `py_alpaca_daily_losers-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 0.3.0
+Version: 0.3.1
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.30.1,<2.0.0)
```

