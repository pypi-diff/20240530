# Comparing `tmp/parcllabs-0.2.2.tar.gz` & `tmp/parcllabs-0.3.0.tar.gz`

## Comparing `parcllabs-0.2.2.tar` & `parcllabs-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/__version__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/common.py
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/parcllabs_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/__init__.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/metros.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/top_markets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/__init__.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/investor_metrics.py
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/market_metrics.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/parcllabs_service.py
--rw-r--r--   0        0        0    17702 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/portfolio_metrics.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/price_feed.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/rental_market_metrics.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/search.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 parcllabs-0.2.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 parcllabs-0.2.2/LICENSE
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 parcllabs-0.2.2/README.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 parcllabs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    16712 2020-02-02 00:00:00.000000 parcllabs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/__version__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/common.py
+-rw-r--r--   0        0        0     6899 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/parcllabs_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/search/__init__.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/search/metros.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/search/top_markets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/__init__.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/investor_metrics.py
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/market_metrics.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/parcllabs_service.py
+-rw-r--r--   0        0        0    17702 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/price_feed.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/rental_market_metrics.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 parcllabs-0.3.0/parcllabs/services/search.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 parcllabs-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 parcllabs-0.3.0/LICENSE
+-rw-r--r--   0        0        0    14835 2020-02-02 00:00:00.000000 parcllabs-0.3.0/README.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 parcllabs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16927 2020-02-02 00:00:00.000000 parcllabs-0.3.0/PKG-INFO
```

### Comparing `parcllabs-0.2.2/parcllabs/parcllabs_client.py` & `parcllabs-0.3.0/parcllabs/parcllabs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         self.price_feed = PriceFeedBase(
             url="/v1/price_feed/{parcl_id}/price_feed", client=self
         )
         self.price_feed_volatility = PriceFeedBase(
             url="/v1/price_feed/{parcl_id}/volatility", client=self
         )
 
+        self.rental_price_feed = PriceFeedBase(
+            url="/v1/price_feed/{parcl_id}/rental_price_feed", client=self
+        )
+
         # top-level services: The client is responsible for creating instances of these services
         self.investor_metrics_housing_stock_ownership = (
             InvestorMetricsHousingStockOwnership(client=self)
         )
         self.investor_metrics_new_listings_for_sale_rolling_counts = (
             InvesetorMetricsNewListingsForSaleRollingCounts(client=self)
         )
```

### Comparing `parcllabs-0.2.2/parcllabs/search/metros.py` & `parcllabs-0.3.0/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.3.0/parcllabs/services/for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/investor_metrics.py` & `parcllabs-0.3.0/parcllabs/services/investor_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/market_metrics.py` & `parcllabs-0.3.0/parcllabs/services/market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/parcllabs_service.py` & `parcllabs-0.3.0/parcllabs/services/parcllabs_service.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/portfolio_metrics.py` & `parcllabs-0.3.0/parcllabs/services/portfolio_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/price_feed.py` & `parcllabs-0.3.0/parcllabs/services/price_feed.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.3.0/parcllabs/services/rental_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/parcllabs/services/search.py` & `parcllabs-0.3.0/parcllabs/services/search.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/.gitignore` & `parcllabs-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/LICENSE` & `parcllabs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/README.md` & `parcllabs-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
 #### Price Feed
 Gets the daily price feed for a specified `parcl_id`.
 
 #### Price Feed Volatility
 Gets the daily price feed volatility for a specified `parcl_id`.
 
+#### Rental Price Feed
+Gets the daily updated Parcl Labs Rental Price Feed for a given `parcl_id`.
+
 ```python
 import os
 
 from parcllabs import ParclLabsClient
 
 api_key = os.getenv('PARCLLABS_API_KEY')
 client = ParclLabsClient(api_key)
@@ -89,14 +92,18 @@
         sort_order='DESC',
         params={'limit': 10},
         as_dataframe=True
 )
 pricefeed_ids = pricefeed_markets['parcl_id'].tolist()
 
 price_feeds = client.price_feed.retrieve_many(parcl_ids=pricefeed_ids, as_dataframe=True)
+rental_price_feeds = client.rental_price_feed.retrieve_many(
+    parcl_ids=pricefeed_ids, 
+    as_dataframe=True
+)
 price_feed_volatility = client.price_feed_volatility.retrieve_many(parcl_ids=pricefeed_ids, as_dataframe=True)
 
 # want to save to csv? 
 price_feeds.to_csv('price_feeds.csv', index=False)
 price_feed_volatility.to_csv('price_feed_volatility.csv', index=False)
 ```
```

### Comparing `parcllabs-0.2.2/pyproject.toml` & `parcllabs-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.2/PKG-INFO` & `parcllabs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: parcllabs
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python SDK for ParclLabs API
 Project-URL: Homepage, https://github.com/ParclLabs/parcllabs-python
 Author-email: ParclLabs <team@parcllabs.com>
 License: MIT License
         
         Copyright (c) [2024] [Parcl Labs]
         
@@ -116,14 +116,17 @@
 
 #### Price Feed
 Gets the daily price feed for a specified `parcl_id`.
 
 #### Price Feed Volatility
 Gets the daily price feed volatility for a specified `parcl_id`.
 
+#### Rental Price Feed
+Gets the daily updated Parcl Labs Rental Price Feed for a given `parcl_id`.
+
 ```python
 import os
 
 from parcllabs import ParclLabsClient
 
 api_key = os.getenv('PARCLLABS_API_KEY')
 client = ParclLabsClient(api_key)
@@ -134,14 +137,18 @@
         sort_order='DESC',
         params={'limit': 10},
         as_dataframe=True
 )
 pricefeed_ids = pricefeed_markets['parcl_id'].tolist()
 
 price_feeds = client.price_feed.retrieve_many(parcl_ids=pricefeed_ids, as_dataframe=True)
+rental_price_feeds = client.rental_price_feed.retrieve_many(
+    parcl_ids=pricefeed_ids, 
+    as_dataframe=True
+)
 price_feed_volatility = client.price_feed_volatility.retrieve_many(parcl_ids=pricefeed_ids, as_dataframe=True)
 
 # want to save to csv? 
 price_feeds.to_csv('price_feeds.csv', index=False)
 price_feed_volatility.to_csv('price_feed_volatility.csv', index=False)
 ```
```

