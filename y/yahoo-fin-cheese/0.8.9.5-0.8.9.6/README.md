# Comparing `tmp/yahoo_fin_cheese-0.8.9.5.tar.gz` & `tmp/yahoo_fin_cheese-0.8.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yahoo_fin_cheese-0.8.9.5.tar", last modified: Sun May 26 17:00:35 2024, max compression
+gzip compressed data, was "yahoo_fin_cheese-0.8.9.6.tar", last modified: Thu May 30 08:48:56 2024, max compression
```

## Comparing `yahoo_fin_cheese-0.8.9.5.tar` & `yahoo_fin_cheese-0.8.9.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-26 17:00:35.960398 yahoo_fin_cheese-0.8.9.5/
--rw-r--r--   0 cheese     (501) staff       (20)     1095 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.5/LICENSE.txt
--rw-r--r--   0 cheese     (501) staff       (20)      466 2024-05-26 17:00:35.960062 yahoo_fin_cheese-0.8.9.5/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     2220 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.5/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2024-05-26 17:00:35.960441 yahoo_fin_cheese-0.8.9.5/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      895 2024-05-26 17:00:32.000000 yahoo_fin_cheese-0.8.9.5/setup.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-26 17:00:35.956695 yahoo_fin_cheese-0.8.9.5/yahoo_fin/
--rw-r--r--   0 cheese     (501) staff       (20)      170 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)      218 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin/news.py
--rw-r--r--   0 cheese     (501) staff       (20)     3218 2024-05-26 16:27:12.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin/options.py
--rw-r--r--   0 cheese     (501) staff       (20)      410 2024-05-26 16:27:12.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin/options_test.py
--rw-r--r--   0 cheese     (501) staff       (20)    33894 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin/stock_info.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-26 17:00:35.959700 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)      466 2024-05-26 17:00:35.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      379 2024-05-26 17:00:35.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2024-05-26 17:00:35.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2024-05-26 16:44:12.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/not-zip-safe
--rw-r--r--   0 cheese     (501) staff       (20)       54 2024-05-26 17:00:35.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2024-05-26 17:00:35.000000 yahoo_fin_cheese-0.8.9.5/yahoo_fin_cheese.egg-info/top_level.txt
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-30 08:48:56.148936 yahoo_fin_cheese-0.8.9.6/
+-rw-r--r--   0 cheese     (501) staff       (20)     1095 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.6/LICENSE.txt
+-rw-r--r--   0 cheese     (501) staff       (20)      531 2024-05-30 08:48:56.148546 yahoo_fin_cheese-0.8.9.6/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     2411 2024-05-30 08:42:12.000000 yahoo_fin_cheese-0.8.9.6/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2024-05-30 08:48:56.148991 yahoo_fin_cheese-0.8.9.6/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)     1024 2024-05-30 08:39:19.000000 yahoo_fin_cheese-0.8.9.6/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-30 08:48:56.143059 yahoo_fin_cheese-0.8.9.6/yahoo_fin/
+-rw-r--r--   0 cheese     (501) staff       (20)      170 2024-05-26 15:21:51.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)      209 2024-05-30 08:38:28.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/news.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2984 2024-05-30 08:28:19.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/options.py
+-rw-r--r--   0 cheese     (501) staff       (20)      410 2024-05-26 16:27:12.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/options_test.py
+-rw-r--r--   0 cheese     (501) staff       (20)    32142 2024-05-30 08:37:43.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/stock_info.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2651 2024-05-30 08:37:53.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin/stock_info_test.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2024-05-30 08:48:56.148078 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)      531 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      408 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/not-zip-safe
+-rw-r--r--   0 cheese     (501) staff       (20)       88 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2024-05-30 08:48:56.000000 yahoo_fin_cheese-0.8.9.6/yahoo_fin_cheese.egg-info/top_level.txt
```

### Comparing `yahoo_fin_cheese-0.8.9.5/LICENSE.txt` & `yahoo_fin_cheese-0.8.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yahoo_fin_cheese-0.8.9.5/README.md` & `yahoo_fin_cheese-0.8.9.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-# yahoo_fin
+# yahoo_fin_cheese
+
+> *Note:*
+>
+> Forked from [yahoo_fin](https://github.com/atreadw1492/yahoo_fin) to:
+>
+> - Update some outdated functions.
+> - Add some unit tests.
+> - Remove egg package way.
+
 Scrape stock price history from new (Spring 2017) Yahoo Finance layout
 
 Full documentation is available on my website, here: http://theautomatic.net/yahoo_fin-documentation/.
 
 If you're familiar with the "get_data_yahoo" method in pandas.io.data, this package's initial purpose was to serve as an updated replacement
 based off Yahoo Finance's change in layout and its API (Spring 2017).  Since then, the package has been developed to scrape stock fundamentals data, ticker symbols from popular exchanges, (including S&P 500, NASDAQ, Dow Jones, and NYSE), balance sheets, income statements, cash flows, data on holders and analysts, and additional data such as beta / dividend information / 1 yr est. etc.  Additionally, it contains a module for scraping options data.
 
 The package contains two modules: stock_info and options.
 
 Download using pip:
 
 ```batch
-pip install yahoo_fin
+pip install yahoo_fin_cheese
 ```
 
 Examples:
 
 ```python
 from yahoo_fin.stock_info import get_data, tickers_sp500, tickers_nasdaq, tickers_other, get_quote_table
```

### Comparing `yahoo_fin_cheese-0.8.9.5/setup.py` & `yahoo_fin_cheese-0.8.9.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from setuptools import setup
 
 setup(name='yahoo_fin_cheese',
-      version='0.8.9.5',
+      version='0.8.9.6',
       description="""Forked from yahoo_fin to update some outdated functions.
                      Download historical stock prices (daily / weekly / monthly),
                      realtime-prices, fundamentals data, income statements, 
                      cash flows, analyst info, current cryptocurrency prices,
                      option chains, earnings history, and more with yahoo_fin.
                     """,
-      url='http://theautomatic.net/yahoo_fin-documentation/',
+      url='https://theautomatic.net/yahoo_fin-documentation/',
       author='Cheese Wong',
       author_email='cheese.javaee@gmail.com',
       license='MIT',
       packages=['yahoo_fin'],
-      install_requires = ["requests_html", "feedparser", "requests", "pandas", "pycryptodome"],
-      keywords = ["yahoo finance", "stocks", "options", "fundamentals"],
-zip_safe=False)
+      install_requires=[
+          "requests_html",
+          "feedparser",
+          "requests",
+          "pandas",
+          "pycryptodome",
+          "beautifulsoup4==4.11.1",
+          "bs4==0.0.2"
+      ],
+      keywords=["yahoo finance", "stocks", "options", "fundamentals"],
+      zip_safe=False)
```

### Comparing `yahoo_fin_cheese-0.8.9.5/yahoo_fin/options.py` & `yahoo_fin_cheese-0.8.9.6/yahoo_fin/options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,100 @@
-
-
 import pandas as pd
 import numpy as np
 import requests
 
 try:
     from requests_html import HTMLSession
 except Exception:
     pass
 
 
 def force_float(elt):
-    
     try:
         return float(elt)
     except:
         return elt
 
-def build_options_url(ticker, date = None):
-    
+
+def build_options_url(ticker, date=None):
     """Constructs the URL pointing to options chain"""
-       
+
     url = "https://finance.yahoo.com/quote/" + ticker + "/options?p=" + ticker
 
     if date is not None:
         url = url + "&date=" + str(int(pd.Timestamp(date).timestamp()))
 
     return url
 
-def get_options_chain(ticker, date = None, raw = True, headers = {'User-agent': 'Mozilla/5.0'}):
-    
+
+def get_options_chain(ticker, date=None, raw=True, headers={'User-agent': 'Mozilla/5.0'}):
     """Extracts call / put option tables for input ticker and expiration date.  If
        no date is input, the default result will be the earliest expiring
        option chain from the current date.
     
        @param: ticker
-       @param: date"""    
-    
+       @param: date"""
+
     site = build_options_url(ticker, date)
-    
+
     tables = pd.read_html(requests.get(site, headers=headers).text)
-    
+
     if len(tables) == 1:
         calls = tables[0].copy()
-        puts = pd.DataFrame(columns = calls.columns)
+        puts = pd.DataFrame(columns=calls.columns)
     else:
         calls = tables[0].copy()
         puts = tables[1].copy()
-    
+
     if not raw:
         calls["% Change"] = calls["% Change"].str.strip("%").map(force_float)
         calls["% Change"] = calls["% Change"].map(lambda num: num / 100 if isinstance(num, float) else 0)
         calls["Volume"] = calls["Volume"].str.replace("-", "0").map(force_float)
         calls["Open Interest"] = calls["Open Interest"].str.replace("-", "0").map(force_float)
-        
-        
+
         puts["% Change"] = puts["% Change"].str.strip("%").map(force_float)
         puts["% Change"] = puts["% Change"].map(lambda num: num / 100 if isinstance(num, float) else 0)
-        puts["Volume"] =puts["Volume"].str.replace("-", "0").map(force_float)
+        puts["Volume"] = puts["Volume"].str.replace("-", "0").map(force_float)
         puts["Open Interest"] = puts["Open Interest"].str.replace("-", "0").map(force_float)
-        
-    
-    
-    return {"calls": calls, "puts":puts}    
-    
-    
-def get_calls(ticker, date = None):
 
+    return {"calls": calls, "puts": puts}
+
+
+def get_calls(ticker, date=None):
     """Extracts call option table for input ticker and expiration date
     
        @param: ticker
        @param: date"""
-       
+
     options_chain = get_options_chain(ticker, date)
-    
+
     return options_chain["calls"]
-    
-    
 
-def get_puts(ticker, date = None):
 
+def get_puts(ticker, date=None):
     """Extracts put option table for input ticker and expiration date
     
        @param: ticker
        @param: date"""
-    
+
     options_chain = get_options_chain(ticker, date)
-    
-    return options_chain["puts"]    
 
-    
-def get_expiration_dates(ticker):
+    return options_chain["puts"]
+
 
+def get_expiration_dates(ticker):
     """Scrapes the expiration dates from each option chain for input ticker
     
        @param: ticker"""
-    
+
     site = build_options_url(ticker)
-    
+
     session = HTMLSession()
     resp = session.get(site)
-    
+
     query = "//button[@aria-haspopup='listbox' and @data-type='date']/../div[@role='listbox']/div[@role='option']"
     nodes = resp.html.xpath(query)
     dates = [node.text for node in nodes]
 
     session.close()
-    
-    return dates
-    
-
-
-
-    
-    
-    
-    
-    
-    
-    
-    
 
-    
+    return dates
```

### Comparing `yahoo_fin_cheese-0.8.9.5/yahoo_fin/stock_info.py` & `yahoo_fin_cheese-0.8.9.6/yahoo_fin/stock_info.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,378 +9,352 @@
 import base64
 import hashlib
 # Need to install pycryptodome package
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import unpad
 # For pretty print
 from pprint import pp
-
+from bs4 import BeautifulSoup
 
 try:
     from requests_html import HTMLSession
 except Exception:
     print("""Warning - Certain functionality 
              requires requests_html, which is not installed.
-             
+
              Install using:
              pip install requests_html
 
              After installation, you may have to restart your Python session.""")
 
-
 base_url = "https://query1.finance.yahoo.com/v8/finance/chart/"
-default_headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
+default_headers = {
+    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
+
 
-def build_url(ticker, start_date = None, end_date = None, interval = "1d"):
-    
-    if end_date is None:  
+def build_url(ticker, start_date=None, end_date=None, interval="1d"):
+    if end_date is None:
         end_seconds = int(pd.Timestamp("now").timestamp())
-        
+
     else:
         end_seconds = int(pd.Timestamp(end_date).timestamp())
-        
+
     if start_date is None:
-        start_seconds = 7223400    
-        
+        start_seconds = 7223400
+
     else:
         start_seconds = int(pd.Timestamp(start_date).timestamp())
-    
+
     site = base_url + ticker
-    
+
     params = {"period1": start_seconds, "period2": end_seconds,
               "interval": interval.lower(), "events": "div,splits"}
-    
-    
+
     return site, params
 
 
 def force_float(elt):
-    
     try:
         return float(elt)
     except:
         return elt
-    
-def _convert_to_numeric(s):
 
+
+def _convert_to_numeric(s):
     if "M" in s:
         s = s.strip("M")
         return force_float(s) * 1_000_000
 
     if "B" in s:
         s = s.strip("B")
         return force_float(s) * 1_000_000_000
 
     return force_float(s)
 
 
-def get_data(ticker, start_date = None, end_date = None, index_as_date = True,
-             interval = "1d", headers = default_headers
-):
-    '''Downloads historical stock price data into a pandas data frame.  Interval
+def get_data(ticker, start_date=None, end_date=None, index_as_date=True,
+             interval="1d", headers=default_headers
+             ):
+    """Downloads historical stock price data into a pandas data frame.  Interval
        must be "1d", "1wk", "1mo", or "1m" for daily, weekly, monthly, or minute data.
        Intraday minute data is limited to 7 days.
-    
+
        @param: ticker
        @param: start_date = None
        @param: end_date = None
        @param: index_as_date = True
        @param: interval = "1d"
-    '''
-    
+    """
+
     if interval not in ("1d", "1wk", "1mo", "1m"):
         raise AssertionError("interval must be of of '1d', '1wk', '1mo', or '1m'")
-    
-    
+
     # build and connect to URL
     site, params = build_url(ticker, start_date, end_date, interval)
-    resp = requests.get(site, params = params, headers = headers)
-    
-    
+    resp = requests.get(site, params=params, headers=headers)
+
     if not resp.ok:
         raise AssertionError(resp.json())
-        
-    
+
     # get JSON response
     data = resp.json()
-    
+
     # get open / high / low / close data
     frame = pd.DataFrame(data["chart"]["result"][0]["indicators"]["quote"][0])
 
     # get the date info
     temp_time = data["chart"]["result"][0]["timestamp"]
 
     if interval != "1m":
-    
+
         # add in adjclose
-        frame["adjclose"] = data["chart"]["result"][0]["indicators"]["adjclose"][0]["adjclose"]   
-        frame.index = pd.to_datetime(temp_time, unit = "s")
+        frame["adjclose"] = data["chart"]["result"][0]["indicators"]["adjclose"][0]["adjclose"]
+        frame.index = pd.to_datetime(temp_time, unit="s")
         frame.index = frame.index.map(lambda dt: dt.floor("d"))
         frame = frame[["open", "high", "low", "close", "adjclose", "volume"]]
-            
+
     else:
 
-        frame.index = pd.to_datetime(temp_time, unit = "s")
+        frame.index = pd.to_datetime(temp_time, unit="s")
         frame = frame[["open", "high", "low", "close", "volume"]]
-        
-        
+
     frame['ticker'] = ticker.upper()
-    
-    if not index_as_date:  
+
+    if not index_as_date:
         frame = frame.reset_index()
-        frame.rename(columns = {"index": "date"}, inplace = True)
-        
-    return frame
+        frame.rename(columns={"index": "date"}, inplace=True)
 
+    return frame
 
 
-def tickers_sp500(include_company_data = False):
-    '''Downloads list of tickers currently listed in the S&P 500 '''
+def tickers_sp500(include_company_data=False):
+    """Downloads list of tickers currently listed in the S&P 500 """
     # get list of all S&P 500 stocks
     sp500 = pd.read_html("https://en.wikipedia.org/wiki/List_of_S%26P_500_companies")[0]
     sp500["Symbol"] = sp500["Symbol"].str.replace(".", "-")
 
     if include_company_data:
         return sp500
 
     sp_tickers = sp500.Symbol.tolist()
     sp_tickers = sorted(sp_tickers)
-    
+
     return sp_tickers
 
 
-def tickers_nasdaq(include_company_data = False):
-    
-    '''Downloads list of tickers currently listed in the NASDAQ'''
-    
+def tickers_nasdaq(include_company_data=False):
+    """Downloads list of tickers currently listed in the NASDAQ"""
+
     ftp = ftplib.FTP("ftp.nasdaqtrader.com")
     ftp.login()
     ftp.cwd("SymbolDirectory")
-    
+
     r = io.BytesIO()
     ftp.retrbinary('RETR nasdaqlisted.txt', r.write)
-    
+
     if include_company_data:
         r.seek(0)
-        data = pd.read_csv(r, sep = "|")
+        data = pd.read_csv(r, sep="|")
         return data
-    
+
     info = r.getvalue().decode()
     splits = info.split("|")
-    
-    
+
     tickers = [x for x in splits if "\r\n" in x]
     tickers = [x.split("\r\n")[1] for x in tickers if "NASDAQ" not in x != "\r\n"]
-    tickers = [ticker for ticker in tickers if "File" not in ticker]    
-    
-    ftp.close()    
+    tickers = [ticker for ticker in tickers if "File" not in ticker]
+
+    ftp.close()
 
     return tickers
-    
-    
 
-def tickers_other(include_company_data = False):
-    '''Downloads list of tickers currently listed in the "otherlisted.txt"
-       file on "ftp.nasdaqtrader.com" '''
+
+def tickers_other(include_company_data=False):
+    """Downloads list of tickers currently listed in the "otherlisted.txt"
+       file on "ftp.nasdaqtrader.com" """
     ftp = ftplib.FTP("ftp.nasdaqtrader.com")
     ftp.login()
     ftp.cwd("SymbolDirectory")
-    
+
     r = io.BytesIO()
     ftp.retrbinary('RETR otherlisted.txt', r.write)
-    
+
     if include_company_data:
         r.seek(0)
-        data = pd.read_csv(r, sep = "|")
+        data = pd.read_csv(r, sep="|")
         return data
-    
+
     info = r.getvalue().decode()
-    splits = info.split("|")    
-    
+    splits = info.split("|")
+
     tickers = [x for x in splits if "\r\n" in x]
     tickers = [x.split("\r\n")[1] for x in tickers]
-    tickers = [ticker for ticker in tickers if "File" not in ticker]        
-    
-    ftp.close()    
+    tickers = [ticker for ticker in tickers if "File" not in ticker]
+
+    ftp.close()
 
     return tickers
-    
-    
-def tickers_dow(include_company_data = False):
-    
-    '''Downloads list of currently traded tickers on the Dow'''
+
+
+def tickers_dow(include_company_data=False):
+    """Downloads list of currently traded tickers on the Dow"""
 
     site = "https://en.wikipedia.org/wiki/Dow_Jones_Industrial_Average"
-    
-    table = pd.read_html(site, attrs = {"id":"constituents"})[0]
-    
+
+    table = pd.read_html(site, attrs={"id": "constituents"})[0]
+
     if include_company_data:
         return table
 
     dow_tickers = sorted(table['Symbol'].tolist())
-    
-    return dow_tickers    
-    
-
-def tickers_ibovespa(include_company_data = False):
-    
-    '''Downloads list of currently traded tickers on the Ibovespa, Brazil'''
+
+    return dow_tickers
+
+
+def tickers_ibovespa(include_company_data=False):
+    """Downloads list of currently traded tickers on the Ibovespa, Brazil"""
 
     table = pd.read_html("https://pt.wikipedia.org/wiki/Lista_de_companhias_citadas_no_Ibovespa")[0]
     table.columns = ["Symbol", "Share", "Sector", "Type", "Site"]
-    
+
     if include_company_data:
         return table
-    
-    ibovespa_tickers = sorted(table.Symbol.tolist())
-    
-    return ibovespa_tickers 
 
+    ibovespa_tickers = sorted(table.Symbol.tolist())
 
+    return ibovespa_tickers
 
-def tickers_nifty50(include_company_data = False, headers = {'User-agent': 'Mozilla/5.0'}):
 
-    '''Downloads list of currently traded tickers on the NIFTY 50, India'''
+def tickers_nifty50(include_company_data=False, headers={'User-agent': 'Mozilla/5.0'}):
+    """Downloads list of currently traded tickers on the NIFTY 50, India"""
 
     site = "https://finance.yahoo.com/quote/%5ENSEI/components?p=%5ENSEI"
     table = pd.read_html(requests.get(site, headers=headers).text)[0]
-    
+
     if include_company_data:
         return table
-    
+
     nifty50 = sorted(table['Symbol'].tolist())
 
     return nifty50
 
+
 def tickers_niftybank():
-    ''' Currently traded tickers on the NIFTY BANK, India '''
-    
-    niftybank = ['AXISBANK', 'KOTAKBANK', 'HDFCBANK', 'SBIN', 'BANKBARODA', 'INDUSINDBK', 'PNB', 'IDFCFIRSTB', 'ICICIBANK', 'RBLBANK', 'FEDERALBNK', 'BANDHANBNK']
-    
+    """ Currently traded tickers on the NIFTY BANK, India """
+
+    niftybank = ['AXISBANK', 'KOTAKBANK', 'HDFCBANK', 'SBIN', 'BANKBARODA', 'INDUSINDBK', 'PNB', 'IDFCFIRSTB',
+                 'ICICIBANK', 'AUBANK', 'FEDERALBNK', 'BANDHANBNK']
+
     return niftybank
 
 
+def tickers_ftse100(include_company_data=False):
+    """Downloads a list of the tickers traded on the FTSE 100 index"""
+
+    table = pd.read_html("https://en.wikipedia.org/wiki/FTSE_100_Index", attrs={"id": "constituents"})[0]
 
-def tickers_ftse100(include_company_data = False):
-    
-    '''Downloads a list of the tickers traded on the FTSE 100 index'''
-    
-    table = pd.read_html("https://en.wikipedia.org/wiki/FTSE_100_Index", attrs = {"id": "constituents"})[0]
-    
     if include_company_data:
         return table
-    
+
     return sorted(table.EPIC.tolist())
-    
 
-def tickers_ftse250(include_company_data = False):
-    
-    
-    '''Downloads a list of the tickers traded on the FTSE 250 index'''
-    
-    table = pd.read_html("https://en.wikipedia.org/wiki/FTSE_250_Index", attrs = {"id": "constituents"})[0]
-    
+
+def tickers_ftse250(include_company_data=False):
+    """Downloads a list of the tickers traded on the FTSE 250 index"""
+
+    table = pd.read_html("https://en.wikipedia.org/wiki/FTSE_250_Index", attrs={"id": "constituents"})[0]
+
     table.columns = ["Company", "Ticker"]
-    
+
     if include_company_data:
         return table
-    
-    return sorted(table.Ticker.tolist())
-    
 
+    return sorted(table.Ticker.tolist())
 
 
-def get_quote_table(ticker , dict_result = True, headers = {'User-agent': 'Mozilla/5.0'}): 
-    
-    '''Scrapes data elements found on Yahoo Finance's quote page 
+def get_quote_table(ticker, dict_result=True, headers={'User-agent': 'Mozilla/5.0'}):
+    """Scrapes data elements found on Yahoo Finance's quote page 
        of input ticker
-    
+
        @param: ticker
        @param: dict_result = True
-    '''
+    """
 
     site = "https://finance.yahoo.com/quote/" + ticker + "?p=" + ticker
-    
+
     tables = pd.read_html(requests.get(site, headers=headers).text)
-    
+
     data = pd.concat([tables[0], tables[1]])
-    
 
-    data.columns = ["attribute" , "value"]
-    
+    data.columns = ["attribute", "value"]
+
     quote_price = pd.DataFrame(["Quote Price", get_live_price(ticker)]).transpose()
     quote_price.columns = data.columns.copy()
-    
+
     data = pd.concat([data, quote_price])
-    
+
     data = data.sort_values("attribute")
-    
-    data = data.drop_duplicates().reset_index(drop = True)
-    
+
+    data = data.drop_duplicates().reset_index(drop=True)
+
     data["value"] = data.value.map(force_float)
 
     if dict_result:
-        
-        result = {key : val for key,val in zip(data.attribute , data.value)}
+        result = {key: val for key, val in zip(data.attribute, data.value)}
         return result
-        
-    return data    
-    
-    
-def get_stats(ticker, headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Scrapes information from the statistics tab on Yahoo Finance 
+
+    return data
+
+
+def get_stats(ticker, headers={'User-agent': 'Mozilla/5.0'}):
+    """Scrapes information from the statistics tab on Yahoo Finance 
        for an input ticker 
-    
+
        @param: ticker
-    '''
+    """
 
     stats_site = "https://finance.yahoo.com/quote/" + ticker + \
                  "/key-statistics?p=" + ticker
-    
 
     tables = pd.read_html(requests.get(stats_site, headers=headers).text)
-    
+
     tables = [table for table in tables[1:] if table.shape[1] == 2]
-    
+
     table = tables[0]
     for elt in tables[1:]:
         table = pd.concat([table, elt])
 
-    table.columns = ["Attribute" , "Value"]
-    
-    table = table.reset_index(drop = True)
-    
+    table.columns = ["Attribute", "Value"]
+
+    table = table.reset_index(drop=True)
+
     return table
 
 
-def get_stats_valuation(ticker, headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Scrapes Valuation Measures table from the statistics tab on Yahoo Finance 
+def get_stats_valuation(ticker, headers={'User-agent': 'Mozilla/5.0'}):
+    """Scrapes Valuation Measures table from the statistics tab on Yahoo Finance 
        for an input ticker 
-    
+
        @param: ticker
-    '''
+    """
 
     stats_site = "https://finance.yahoo.com/quote/" + ticker + \
                  "/key-statistics?p=" + ticker
-    
-    
+
     tables = pd.read_html(requests.get(stats_site, headers=headers).text)
-    
-    tables = [table for table in tables if "Trailing P/E" in table.iloc[:,0].tolist()]
-    
-    
-    table = tables[0].reset_index(drop = True)
-    
+
+    tables = [table for table in tables if "Trailing P/E" in table.iloc[:, 0].tolist()]
+
+    table = tables[0].reset_index(drop=True)
+
     return table
 
 
 def _decrypt_yblob_aes(data):
-    '''From pydata/pandas-datareader PR#953 - https://github.com/pydata/pandas-datareader/pull/953/commits/ea66d6b981554f9d0262038aef2106dda7138316 '''
+    """From pydata/pandas-datareader PR#953 - https://github.com/pydata/pandas-datareader/pull/953/commits/ea66d6b981554f9d0262038aef2106dda7138316 """
     encrypted_stores = data['context']['dispatcher']['stores']
     _cs = data["_cs"]
     _cr = data["_cr"]
 
     _cr = b"".join(int.to_bytes(i, length=4, byteorder="big", signed=True) for i in json.loads(_cr)["words"])
     password = hashlib.pbkdf2_hmac("sha1", _cs.encode("utf8"), _cr, 1, dklen=32).hex()
 
@@ -438,689 +412,650 @@
 
     cipher = AES.new(key, AES.MODE_CBC, iv=iv)
     plaintext = cipher.decrypt(encrypted_stores)
     plaintext = unpad(plaintext, 16, style="pkcs7")
     decoded_stores = json.loads(plaintext)
     return decoded_stores
 
-def _parse_json(url, headers = {'User-agent': 'Mozilla/5.0'}):
 
-    html = requests.get(url=url, headers = headers).text
+def _parse_json(url, headers={'User-agent': 'Mozilla/5.0'}):
+    html = requests.get(url=url, headers=headers).text
 
-    json_str = html.split('root.App.main =')[1].split('(this)')[0].split(';\n}')[0].strip()
+    json_str = '{}'
+
+    soup = BeautifulSoup(html, "html.parser")
+    script_tags = soup.find_all('script')
+    for script_tag in script_tags:
+        data_url = script_tag.get('data-url')
+        if data_url and "quoteSummary" in data_url:
+            if script_tag.contents is not None and len(script_tag.contents):
+                json_str = script_tag.contents[0]
 
     try:
         data = json.loads(json_str)
-        #print("type of json_str :", type(data))
-        unencrypted_stores = _decrypt_yblob_aes(data)
-        json_info = unencrypted_stores['QuoteSummaryStore']
-        #print("json_info :", json_info)
+        json_info = data
+        body_json = json.loads(json_info["body"])
+        result = body_json["quoteSummary"]["result"][0]
     except:
         return '{}'
-    #else:
-        # return data
-        #new_data = json.dumps(data).replace('{}', 'null')
-        #new_data = re.sub(r'\{[\'|\"]raw[\'|\"]:(.*?),(.*?)\}', r'\1', new_data)
-        #json_info = json.loads(new_data)
-        #print("json info :", json_info)
-    return json_info
+
+    return result
 
 
 def _parse_table(json_info):
-
     df = pd.DataFrame(json_info)
-    
     if df.empty:
         return df
-    
+
     del df["maxAge"]
 
-    df.set_index("endDate", inplace=True)
+    df["rawEndDate"] = df["endDate"][0]["raw"]
+
+    df.set_index("rawEndDate", inplace=True)
     df.index = pd.to_datetime(df.index, unit="s")
- 
+
     df = df.transpose()
     df.index.name = "Breakdown"
 
     return df
 
 
-def get_income_statement(ticker, yearly = True):
-    
-    '''Scrape income statement from Yahoo Finance for a given ticker
-    
+def get_income_statement(ticker, yearly=True):
+    """Scrape income statement from Yahoo Finance for a given ticker
+
        @param: ticker
-    '''
-    
+    """
+
     income_site = "https://finance.yahoo.com/quote/" + ticker + \
-            "/financials?p=" + ticker
+                  "/financials?p=" + ticker
 
     json_info = _parse_json(income_site)
     try:
         if yearly:
             temp = json_info["incomeStatementHistory"]["incomeStatementHistory"]
         else:
             temp = json_info["incomeStatementHistoryQuarterly"]["incomeStatementHistory"]
     except:
         temp = []
-    
-    return _parse_table(temp)      
-        
-
-def get_balance_sheet(ticker, yearly = True):
-    
-    '''Scrapes balance sheet from Yahoo Finance for an input ticker 
-    
+
+    return _parse_table(temp)
+
+
+def get_balance_sheet(ticker, yearly=True):
+    """Scrapes balance sheet from Yahoo Finance for an input ticker 
+
        @param: ticker
-    '''    
-    
+    """
+
     balance_sheet_site = "https://finance.yahoo.com/quote/" + ticker + \
                          "/balance-sheet?p=" + ticker
-    
 
     json_info = _parse_json(balance_sheet_site)
-    
+
     try:
         if yearly:
             temp = json_info["balanceSheetHistory"]["balanceSheetStatements"]
         else:
             temp = json_info["balanceSheetHistoryQuarterly"]["balanceSheetStatements"]
     except:
         temp = []
-        
-    return _parse_table(temp)      
 
+    return _parse_table(temp)
+
+
+def get_cash_flow(ticker, yearly=True):
+    """Scrapes the cash flow statement from Yahoo Finance for an input ticker 
 
-def get_cash_flow(ticker, yearly = True):
-    
-    '''Scrapes the cash flow statement from Yahoo Finance for an input ticker 
-    
        @param: ticker
-    '''
-    
+    """
+
     cash_flow_site = "https://finance.yahoo.com/quote/" + \
-            ticker + "/cash-flow?p=" + ticker
-    
-    
+                     ticker + "/cash-flow?p=" + ticker
+
     json_info = _parse_json(cash_flow_site)
-    
+
     if yearly:
         temp = json_info["cashflowStatementHistory"]["cashflowStatements"]
     else:
         temp = json_info["cashflowStatementHistoryQuarterly"]["cashflowStatements"]
-        
-    return _parse_table(temp)      
 
+    return _parse_table(temp)
 
-def get_financials(ticker, yearly = True, quarterly = True):
 
-    '''Scrapes financials data from Yahoo Finance for an input ticker, including
+def get_financials(ticker, yearly=True, quarterly=True):
+    """Scrapes financials data from Yahoo Finance for an input ticker, including
        balance sheet, cash flow statement, and income statement.  Returns dictionary
        of results.
-    
+
        @param: ticker
        @param: yearly = True
        @param: quarterly = True
-    '''
+    """
 
     if not yearly and not quarterly:
         raise AssertionError("yearly or quarterly must be True")
-    
+
     financials_site = "https://finance.yahoo.com/quote/" + ticker + \
-            "/financials?p=" + ticker
-            
+                      "/financials?p=" + ticker
+
     json_info = _parse_json(financials_site)
-    
+
     result = {}
-    
-    if yearly:
 
+    if yearly:
         temp = json_info["incomeStatementHistory"]["incomeStatementHistory"]
         table = _parse_table(temp)
         result["yearly_income_statement"] = table
-    
+
         temp = json_info["balanceSheetHistory"]["balanceSheetStatements"]
         table = _parse_table(temp)
         result["yearly_balance_sheet"] = table
-        
+
         temp = json_info["cashflowStatementHistory"]["cashflowStatements"]
         table = _parse_table(temp)
         result["yearly_cash_flow"] = table
 
     if quarterly:
         temp = json_info["incomeStatementHistoryQuarterly"]["incomeStatementHistory"]
         table = _parse_table(temp)
         result["quarterly_income_statement"] = table
-    
+
         temp = json_info["balanceSheetHistoryQuarterly"]["balanceSheetStatements"]
         table = _parse_table(temp)
         result["quarterly_balance_sheet"] = table
-        
+
         temp = json_info["cashflowStatementHistoryQuarterly"]["cashflowStatements"]
         table = _parse_table(temp)
         result["quarterly_cash_flow"] = table
 
-        
     return result
 
 
-def get_holders(ticker, headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Scrapes the Holders page from Yahoo Finance for an input ticker 
-    
+def get_holders(ticker, headers={'User-agent': 'Mozilla/5.0'}):
+    """Scrapes the Holders page from Yahoo Finance for an input ticker 
+
        @param: ticker
-    '''    
-    
+    """
+
     holders_site = "https://finance.yahoo.com/quote/" + \
-                    ticker + "/holders?p=" + ticker
-    
-        
+                   ticker + "/holders?p=" + ticker
+
     tables = pd.read_html(requests.get(holders_site, headers=headers).text)
-    
-       
-    table_names = ["Major Holders" , "Direct Holders (Forms 3 and 4)" ,
-                   "Top Institutional Holders" , "Top Mutual Fund Holders"]
-     
-    
-    table_mapper = {key : val for key,val in zip(table_names , tables)}
-                   
-                   
-    return table_mapper       
-
-def get_analysts_info(ticker, headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Scrapes the Analysts page from Yahoo Finance for an input ticker 
-    
+
+    table_names = ["Major Holders", "Direct Holders (Forms 3 and 4)",
+                   "Top Institutional Holders", "Top Mutual Fund Holders"]
+
+    table_mapper = {key: val for key, val in zip(table_names, tables)}
+
+    return table_mapper
+
+
+def get_analysts_info(ticker, headers={'User-agent': 'Mozilla/5.0'}):
+    """Scrapes the Analysts page from Yahoo Finance for an input ticker 
+
        @param: ticker
-    '''    
-    
-    
+    """
+
     analysts_site = "https://finance.yahoo.com/quote/" + ticker + \
-                     "/analysts?p=" + ticker
-    
+                    "/analysts?p=" + ticker
+
     tables = pd.read_html(requests.get(analysts_site, headers=headers).text)
-    
+
     table_names = [table.columns[0] for table in tables]
 
-    table_mapper = {key : val for key , val in zip(table_names , tables)}
-    
+    table_mapper = {key: val for key, val in zip(table_names, tables)}
 
     return table_mapper
-        
+
 
 def get_live_price(ticker):
-    
-    '''Gets the live price of input ticker
-    
+    """Gets the live price of input ticker
+
        @param: ticker
-    '''    
-    
-    df = get_data(ticker, end_date = pd.Timestamp.today() + pd.DateOffset(10))
-    
-    
-    return df.close[-1]
+    """
+
+    df = get_data(ticker, end_date=pd.Timestamp.today() + pd.DateOffset(10))
+
+    return df.close.iloc[-1]
+
 
 def get_live_prices(ticker_list):
     base_quotes_url = 'https://query1.finance.yahoo.com/v7/finance/quote?symbols='
     new_url = base_quotes_url + ','.join(ticker_list)
     resp = requests.get(new_url, headers=default_headers)
     # get JSON response
     data = resp.json()
-    results = {result['symbol'] : result['regularMarketPrice'] 
+    results = {result['symbol']: result['regularMarketPrice']
                for result in data['quoteResponse']['result']}
     return results
 
+
 def _raw_get_daily_info(site):
-       
     session = HTMLSession()
-    
+
     resp = session.get(site)
-    
-    tables = pd.read_html(resp.html.raw_html)  
-    
+
+    tables = pd.read_html(resp.html.raw_html)
+
     df = tables[0].copy()
-    
+
     df.columns = tables[0].columns
-    
+
     del df["52 Week Range"]
-    
+
     df["% Change"] = df["% Change"].map(lambda x: float(x.strip("%+").replace(",", "")))
-     
 
     fields_to_change = [x for x in df.columns.tolist() if "Vol" in x \
                         or x == "Market Cap"]
-    
+
     for field in fields_to_change:
-        
+
         if type(df[field][0]) == str:
             df[field] = df[field].map(_convert_to_numeric)
-            
+
     session.close()
-    
+
     return df
-    
 
-def get_day_most_active(count: int = 100):
 
+def get_day_most_active(count: int = 100):
     return _raw_get_daily_info(f"https://finance.yahoo.com/most-active?offset=0&count={count}")
 
 
 def get_day_gainers(count: int = 100):
-
     return _raw_get_daily_info(f"https://finance.yahoo.com/gainers?offset=0&count={count}")
 
 
 def get_day_losers(count: int = 100):
-
     return _raw_get_daily_info(f"https://finance.yahoo.com/losers?offset=0&count={count}")
 
 
 def get_top_crypto():
-    
-    '''Gets the top 100 Cryptocurrencies by Market Cap'''      
+    """Gets the top 100 Cryptocurrencies by Market Cap"""
 
     session = HTMLSession()
-    
+
     resp = session.get("https://finance.yahoo.com/cryptocurrencies?offset=0&count=100")
-    
-    tables = pd.read_html(resp.html.raw_html)               
-                    
+
+    tables = pd.read_html(resp.html.raw_html)
+
     df = tables[0].copy()
 
-    
-    df["% Change"] = df["% Change"].map(lambda x: float(str(x).strip("%").\
-                                                               strip("+").\
-                                                               replace(",", "")))
+    df["% Change"] = df["% Change"].map(lambda x: float(str(x).strip("%"). \
+                                                        strip("+"). \
+                                                        replace(",", "")))
     del df["52 Week Range"]
     del df["Day Chart"]
-    
+
     fields_to_change = [x for x in df.columns.tolist() if "Volume" in x \
                         or x == "Market Cap" or x == "Circulating Supply"]
-    
+
     for field in fields_to_change:
-        
+
         if type(df[field][0]) == str:
             df[field] = df[field].map(lambda x: _convert_to_numeric(str(x)))
-            
-            
-    session.close()        
-                
+
+    session.close()
+
     return df
-                    
-        
-def get_dividends(ticker, start_date = None, end_date = None, index_as_date = True, 
-                  headers = default_headers
-):
-    '''Downloads historical dividend data into a pandas data frame.
-    
+
+
+def get_dividends(ticker, start_date=None, end_date=None, index_as_date=True,
+                  headers=default_headers
+                  ):
+    """Downloads historical dividend data into a pandas data frame.
+
        @param: ticker
        @param: start_date = None
        @param: end_date = None
        @param: index_as_date = True
-    '''
-    
+    """
+
     # build and connect to URL
     site, params = build_url(ticker, start_date, end_date, "1d")
-    resp = requests.get(site, params = params, headers = headers)
-    
-    
+    resp = requests.get(site, params=params, headers=headers)
+
     if not resp.ok:
         return pd.DataFrame()
-        
-    
+
     # get JSON response
     data = resp.json()
-    
+
     # check if there is data available for dividends
     if "events" not in data["chart"]["result"][0] or "dividends" not in data["chart"]["result"][0]['events']:
         return pd.DataFrame()
-    
+
     # get the dividend data
     frame = pd.DataFrame(data["chart"]["result"][0]['events']['dividends'])
-    
+
     frame = frame.transpose()
-        
-    frame.index = pd.to_datetime(frame.index, unit = "s")
+
+    frame.index = pd.to_datetime(frame.index, unit="s")
     frame.index = frame.index.map(lambda dt: dt.floor("d"))
-    
+
     # sort in chronological order
     frame = frame.sort_index()
-        
+
     frame['ticker'] = ticker.upper()
-    
+
     # remove old date column
     frame = frame.drop(columns='date')
-    
-    frame = frame.rename({'amount': 'dividend'}, axis = 'columns')
-    
-    if not index_as_date:  
+
+    frame = frame.rename({'amount': 'dividend'}, axis='columns')
+
+    if not index_as_date:
         frame = frame.reset_index()
-        frame.rename(columns = {"index": "date"}, inplace = True)
-        
+        frame.rename(columns={"index": "date"}, inplace=True)
+
     return frame
 
 
+def get_splits(ticker, start_date=None, end_date=None, index_as_date=True,
+               headers=default_headers
+               ):
+    """Downloads historical stock split data into a pandas data frame.
 
-def get_splits(ticker, start_date = None, end_date = None, index_as_date = True,
-               headers = default_headers
-):
-    '''Downloads historical stock split data into a pandas data frame.
-    
        @param: ticker
        @param: start_date = None
        @param: end_date = None
        @param: index_as_date = True
-    '''
-    
+    """
+
     # build and connect to URL
     site, params = build_url(ticker, start_date, end_date, "1d")
-    resp = requests.get(site, params = params, headers = headers)
-    
-    
+    resp = requests.get(site, params=params, headers=headers)
+
     if not resp.ok:
         raise AssertionError(resp.json())
-        
-    
+
     # get JSON response
     data = resp.json()
-    
+
     # check if there is data available for events
     if "events" not in data["chart"]["result"][0]:
-        raise AssertionError("There is no data available on stock events, or none have occured") 
+        raise AssertionError("There is no data available on stock events, or none have occured")
 
-    # check if there is data available for splits
+        # check if there is data available for splits
     if "splits" not in data["chart"]["result"][0]['events']:
         raise AssertionError("There is no data available on stock splits, or none have occured")
-    
+
     # get the split data
     frame = pd.DataFrame(data["chart"]["result"][0]['events']['splits'])
-    
+
     frame = frame.transpose()
-        
-    frame.index = pd.to_datetime(frame.index, unit = "s")
+
+    frame.index = pd.to_datetime(frame.index, unit="s")
     frame.index = frame.index.map(lambda dt: dt.floor("d"))
-    
+
     # sort in to chronological order
     frame = frame.sort_index()
-        
+
     frame['ticker'] = ticker.upper()
-    
+
     # remove unnecessary columns
     frame = frame.drop(columns=['date', 'denominator', 'numerator'])
-    
-    if not index_as_date:  
+
+    if not index_as_date:
         frame = frame.reset_index()
-        frame.rename(columns = {"index": "date"}, inplace = True)
-        
+        frame.rename(columns={"index": "date"}, inplace=True)
+
     return frame
-        
-        
 
 
 def get_earnings(ticker):
-    
-    '''Scrapes earnings data from Yahoo Finance for an input ticker 
-    
+    """Scrapes earnings data from Yahoo Finance for an input ticker 
+
        @param: ticker
-    '''
+    """
 
     result = {
         "quarterly_results": pd.DataFrame(),
         "yearly_revenue_earnings": pd.DataFrame(),
         "quarterly_revenue_earnings": pd.DataFrame()
     }
 
     financials_site = "https://finance.yahoo.com/quote/" + ticker + \
-        "/financials?p=" + ticker
+                      "/financials?p=" + ticker
 
     json_info = _parse_json(financials_site)
 
     if "earnings" not in json_info:
         return result
 
     temp = json_info["earnings"]
 
     if temp == None:
         return result
-    
+
     result["quarterly_results"] = pd.DataFrame.from_dict(temp["earningsChart"]["quarterly"])
-    
+
     result["yearly_revenue_earnings"] = pd.DataFrame.from_dict(temp["financialsChart"]["yearly"])
-    
+
     result["quarterly_revenue_earnings"] = pd.DataFrame.from_dict(temp["financialsChart"]["quarterly"])
-    
-    return (pp(result))
 
+    return result
 
 
 ### Earnings functions
-def _parse_earnings_json(url, headers = default_headers
-):
-        resp = requests.get(url, headers = headers)
-        
-        content = resp.content.decode(encoding='utf-8', errors='strict')
-        
-        page_data = [row for row in content.split(
-            '\n') if row.startswith('root.App.main = ')][0][:-1]
-        
-        page_data = page_data.split('root.App.main = ', 1)[1]
-        
-        return json.loads(page_data)
+def _parse_earnings_json(url, headers=default_headers
+                         ):
+    resp = requests.get(url, headers=headers)
+
+    content = resp.content.decode(encoding='utf-8', errors='strict')
+
+    page_data = [row for row in content.split(
+        '\n') if row.startswith('root.App.main = ')][0][:-1]
+
+    page_data = page_data.split('root.App.main = ', 1)[1]
+
+    return json.loads(page_data)
+
 
 def get_next_earnings_date(ticker):
-        
     base_earnings_url = 'https://finance.yahoo.com/quote'
     new_url = base_earnings_url + "/" + ticker
 
     parsed_result = _parse_earnings_json(new_url)
-    
-    temp = parsed_result['context']['dispatcher']['stores']['QuoteSummaryStore']['calendarEvents']['earnings']['earningsDate'][0]['raw']
+
+    temp = \
+    parsed_result['context']['dispatcher']['stores']['QuoteSummaryStore']['calendarEvents']['earnings']['earningsDate'][
+        0]['raw']
 
     return datetime.datetime.fromtimestamp(temp)
 
 
 def get_earnings_history(ticker):
-    
-        '''Inputs: @ticker
-           Returns the earnings calendar history of the input ticker with 
-           EPS actual vs. expected data.'''
+    """Inputs: @ticker
+       Returns the earnings calendar history of the input ticker with 
+       EPS actual vs. expected data."""
 
-        url = 'https://finance.yahoo.com/calendar/earnings?symbol=' + ticker
-         
-        result = _parse_earnings_json(url)
-        
-        return result["context"]["dispatcher"]["stores"]["ScreenerResultsStore"]["results"]["rows"]
+    url = 'https://finance.yahoo.com/calendar/earnings?symbol=' + ticker
 
+    result = _parse_earnings_json(url)
 
+    return result["context"]["dispatcher"]["stores"]["ScreenerResultsStore"]["results"]["rows"]
 
-def get_earnings_for_date(date, offset = 0, count = 1):
 
-    '''Inputs: @date
+def get_earnings_for_date(date, offset=0, count=1):
+    """Inputs: @date
        Returns a dictionary of stock tickers with earnings expected on the
        input date.  The dictionary contains the expected EPS values for each
-       stock if available.'''
-    
+       stock if available."""
+
     base_earnings_url = 'https://finance.yahoo.com/calendar/earnings'
-    
+
     if offset >= count:
         return []
-    
+
     temp = pd.Timestamp(date)
     date = temp.strftime("%Y-%m-%d")
 
     dated_url = '{0}?day={1}&offset={2}&size={3}'.format(
         base_earnings_url, date, offset, 100)
-    
+
     result = _parse_earnings_json(dated_url)
-    
+
     stores = result['context']['dispatcher']['stores']
-    
+
     earnings_count = stores['ScreenerCriteriaStore']['meta']['total']
 
     new_offset = offset + 100
-    
+
     more_earnings = get_earnings_for_date(date, new_offset, earnings_count)
-    
+
     current_earnings = stores['ScreenerResultsStore']['results']['rows']
 
     total_earnings = current_earnings + more_earnings
 
     return total_earnings
 
 
 def get_earnings_in_date_range(start_date, end_date):
+    """Inputs: @start_date
+               @end_date
+
+       Returns the stock tickers with expected EPS data for all dates in the
+       input range (inclusive of the start_date and end_date."""
+
+    earnings_data = []
+
+    days_diff = pd.Timestamp(end_date) - pd.Timestamp(start_date)
+    days_diff = days_diff.days
+
+    current_date = pd.Timestamp(start_date)
+
+    dates = [current_date + datetime.timedelta(diff) for diff in range(days_diff + 1)]
+    dates = [d.strftime("%Y-%m-%d") for d in dates]
+
+    i = 0
+    while i < len(dates):
+        try:
+            earnings_data += get_earnings_for_date(dates[i])
+        except Exception:
+            pass
+
+        i += 1
+
+    return earnings_data
+
+
+def get_currencies(headers={'User-agent': 'Mozilla/5.0'}):
+    """Returns the currencies table from Yahoo Finance"""
 
-        '''Inputs: @start_date
-                   @end_date
-                   
-           Returns the stock tickers with expected EPS data for all dates in the
-           input range (inclusive of the start_date and end_date.'''
-    
-        earnings_data = []
-
-        days_diff = pd.Timestamp(end_date) - pd.Timestamp(start_date)
-        days_diff = days_diff.days
-
-        
-        current_date = pd.Timestamp(start_date)
-        
-        dates = [current_date + datetime.timedelta(diff) for diff in range(days_diff + 1)]
-        dates = [d.strftime("%Y-%m-%d") for d in dates]
- 
-        i = 0
-        while i < len(dates):
-            try:
-                earnings_data += get_earnings_for_date(dates[i])
-            except Exception:
-                pass
-            
-            i += 1
-            
-        return earnings_data
-
-
-def get_currencies(headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Returns the currencies table from Yahoo Finance'''
-    
     site = "https://finance.yahoo.com/currencies"
     tables = pd.read_html(requests.get(site, headers=headers).text)
-    
+
     result = tables[0]
-    
+
     return result
 
 
-def get_futures(headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Returns the futures table from Yahoo Finance'''
-    
+def get_futures(headers={'User-agent': 'Mozilla/5.0'}):
+    """Returns the futures table from Yahoo Finance"""
+
     site = "https://finance.yahoo.com/commodities"
     tables = pd.read_html(requests.get(site, headers=headers).text)
-    
+
     result = tables[0]
-    
+
     return result
 
 
-def get_undervalued_large_caps(headers = {'User-agent': 'Mozilla/5.0'}):
-    
-    '''Returns the undervalued large caps table from Yahoo Finance'''
-    
+def get_undervalued_large_caps(headers={'User-agent': 'Mozilla/5.0'}):
+    """Returns the undervalued large caps table from Yahoo Finance"""
+
     site = "https://finance.yahoo.com/screener/predefined/undervalued_large_caps?offset=0&count=100"
-    
+
     tables = pd.read_html(requests.get(site, headers=headers).text)
-    
+
     result = tables[0]
-    
+
     return result
 
 
-def get_quote_data(ticker, headers = default_headers
-):
-    
-    '''Inputs: @ticker
-    
+def get_quote_data(ticker, headers=default_headers
+                   ):
+    """Inputs: @ticker
+
        Returns a dictionary containing over 70 elements corresponding to the 
        input ticker, including company name, book value, moving average data,
-       pre-market / post-market price (when applicable), and more.'''
-    
+       pre-market / post-market price (when applicable), and more."""
+
     site = "https://query1.finance.yahoo.com/v7/finance/quote?symbols=" + ticker
-    
-    resp = requests.get(site, headers = default_headers
-)
-    
+
+    resp = requests.get(site, headers=default_headers
+                        )
+
     if not resp.ok:
         raise AssertionError("""Invalid response from server.  Check if ticker is
                               valid.""")
-    
-    
+
     json_result = resp.json()
     info = json_result["quoteResponse"]["result"]
-    
+
     return info[0]
-    
+
 
 def get_market_status():
-    
-    '''Returns the current state of the market - PRE, POST, OPEN, or CLOSED'''
-    
+    """Returns the current state of the market - PRE, POST, OPEN, or CLOSED"""
+
     quote_data = get_quote_data("^dji")
 
     return quote_data["marketState"]
 
+
 def get_premarket_price(ticker):
+    """Inputs: @ticker
 
-    '''Inputs: @ticker
-    
        Returns the current pre-market price of the input ticker
-       (returns value if pre-market price is available.'''
-    
+       (returns value if pre-market price is available."""
+
     quote_data = get_quote_data(ticker)
-    
+
     if "preMarketPrice" in quote_data:
         return quote_data["preMarketPrice"]
-        
+
     raise AssertionError("Premarket price not currently available.")
 
+
 def get_postmarket_price(ticker):
+    """Inputs: @ticker
 
-    '''Inputs: @ticker
-    
        Returns the current post-market price of the input ticker
-       (returns value if pre-market price is available.'''
-    
+       (returns value if pre-market price is available."""
+
     quote_data = get_quote_data(ticker)
-    
+
     if "postMarketPrice" in quote_data:
         return quote_data["postMarketPrice"]
-    
+
     raise AssertionError("Postmarket price not currently available.")
-    
+
 
 # Company Information Functions
 def get_company_info(ticker):
-    '''Scrape the company information for a ticker
+    """Scrape the company information for a ticker
 
        @param: ticker
-    '''
+    """
     site = f"https://finance.yahoo.com/quote/{ticker}/profile?p={ticker}"
     json_info = _parse_json(site)
     json_info = json_info["assetProfile"]
     info_frame = pd.DataFrame.from_dict(json_info,
                                         orient="index",
                                         columns=["Value"])
     info_frame = info_frame.drop("companyOfficers", axis="index")
     info_frame.index.name = "Breakdown"
     return info_frame
 
 
 def get_company_officers(ticker):
-    '''Scrape the company information and return a table of the officers
+    """Scrape the company information and return a table of the officers
 
        @param: ticker
-    '''
+    """
     site = f"https://finance.yahoo.com/quote/{ticker}/profile?p={ticker}"
     json_info = _parse_json(site)
     json_info = json_info["assetProfile"]["companyOfficers"]
     info_frame = pd.DataFrame.from_dict(json_info)
     info_frame = info_frame.set_index("name")
     return info_frame
```

