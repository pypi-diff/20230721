# Comparing `tmp/finance-scrapers-0.1.5.tar.gz` & `tmp/finance-scrapers-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finance-scrapers-0.1.5.tar", last modified: Wed Jul 19 04:01:01 2023, max compression
+gzip compressed data, was "finance-scrapers-1.1.5.tar", last modified: Fri Jul 21 16:11:23 2023, max compression
```

## Comparing `finance-scrapers-0.1.5.tar` & `finance-scrapers-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 04:01:01.937551 finance-scrapers-0.1.5/
--rw-rw-rw-   0        0        0     1089 2023-07-14 03:22:40.000000 finance-scrapers-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2147 2023-07-19 04:01:01.937551 finance-scrapers-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-07-19 03:40:29.000000 finance-scrapers-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 04:01:01.931551 finance-scrapers-0.1.5/finance_scrapers/
--rw-rw-rw-   0        0        0      158 2023-07-19 03:47:19.000000 finance-scrapers-0.1.5/finance_scrapers/__init__.py
--rw-rw-rw-   0        0        0     3728 2023-07-19 03:15:42.000000 finance-scrapers-0.1.5/finance_scrapers/downloader.py
--rw-rw-rw-   0        0        0     3403 2023-07-14 17:55:28.000000 finance-scrapers-0.1.5/finance_scrapers/stock_info.py
--rw-rw-rw-   0        0        0    11034 2023-07-19 03:47:34.000000 finance-scrapers-0.1.5/finance_scrapers/yahoo_finance.py
-drwxrwxrwx   0        0        0        0 2023-07-19 04:01:01.936552 finance-scrapers-0.1.5/finance_scrapers.egg-info/
--rw-rw-rw-   0        0        0     2147 2023-07-19 04:01:01.000000 finance-scrapers-0.1.5/finance_scrapers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-19 04:01:01.000000 finance-scrapers-0.1.5/finance_scrapers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 04:01:01.000000 finance-scrapers-0.1.5/finance_scrapers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-19 04:01:01.000000 finance-scrapers-0.1.5/finance_scrapers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-19 04:01:01.000000 finance-scrapers-0.1.5/finance_scrapers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-07-14 03:22:40.000000 finance-scrapers-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      766 2023-07-19 04:01:01.938551 finance-scrapers-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:23.269498 finance-scrapers-1.1.5/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 03:22:40.000000 finance-scrapers-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4054 2023-07-21 16:11:23.269498 finance-scrapers-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3489 2023-07-21 15:56:39.000000 finance-scrapers-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:23.262750 finance-scrapers-1.1.5/finance_scrapers/
+-rw-rw-rw-   0        0        0      158 2023-07-19 03:47:19.000000 finance-scrapers-1.1.5/finance_scrapers/__init__.py
+-rw-rw-rw-   0        0        0     3772 2023-07-19 23:06:09.000000 finance-scrapers-1.1.5/finance_scrapers/downloader.py
+-rw-rw-rw-   0        0        0     3403 2023-07-14 17:55:28.000000 finance-scrapers-1.1.5/finance_scrapers/stock_info.py
+-rw-rw-rw-   0        0        0    11967 2023-07-21 16:10:42.000000 finance-scrapers-1.1.5/finance_scrapers/yahoo_finance.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:11:23.268499 finance-scrapers-1.1.5/finance_scrapers.egg-info/
+-rw-rw-rw-   0        0        0     4054 2023-07-21 16:11:23.000000 finance-scrapers-1.1.5/finance_scrapers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-21 16:11:23.000000 finance-scrapers-1.1.5/finance_scrapers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:11:23.000000 finance-scrapers-1.1.5/finance_scrapers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-07-21 16:11:23.000000 finance-scrapers-1.1.5/finance_scrapers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 16:11:23.000000 finance-scrapers-1.1.5/finance_scrapers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-14 03:22:40.000000 finance-scrapers-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      777 2023-07-21 16:11:23.270499 finance-scrapers-1.1.5/setup.cfg
```

### Comparing `finance-scrapers-0.1.5/LICENSE` & `finance-scrapers-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finance-scrapers-0.1.5/finance_scrapers/downloader.py` & `finance-scrapers-1.1.5/finance_scrapers/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         Creates a .json file of this downloader's data
 
         Raises:
             ValueError: if the file cannot be written to due to invalid file extension
         """
         if self.file_path.endswith(".json"):
             df = pd.DataFrame(self.data_dict)
+            df.fillna("N/A", inplace=True)
             df.to_json(self.file_path)
         else:
             raise ValueError("File path must end in .json to download json file")
         
 
     def download_md(self) -> None:
         """
```

### Comparing `finance-scrapers-0.1.5/finance_scrapers/stock_info.py` & `finance-scrapers-1.1.5/finance_scrapers/stock_info.py`

 * *Files identical despite different names*

### Comparing `finance-scrapers-0.1.5/finance_scrapers/yahoo_finance.py` & `finance-scrapers-1.1.5/finance_scrapers/yahoo_finance.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,32 +20,39 @@
 
     Attrs:
         home_url (str): the url of the home page for Yahoo Finance
     """
     home_url: str = "https://www.finance.yahoo.com"
 
     def __init__(self, tickers: List[str], validate_tickers: bool = True, 
-                 show_progress: bool = False, info_to_find: set[StockInfo] = set(StockInfo)) -> None:
+                 show_progress: bool = False) -> None:
         """
-        Initializes a YahooFinance to scrape information about the given stocks
-        (identified by their tickers).
+        Initializes a YahooFinance to scrape information about the given stocks which
+        are identified by their ticker symbols. Found information is stored in self.stock_info
 
         Args
             tickers: the tickers of the stocks to be scraped
             validate_tickers: if the tickers should be validated before scraping
             show_progress: if the stock-scraping progress should be displayed in the terminal
         """
+        # general
+        tickers = map(lambda ticker: ticker.upper(), tickers)
+        self.browser = YahooFinance.__configure_browser()
+        self.info_to_find = set(StockInfo)
         self.show_progress = show_progress
-        self.tickers: List[str] = self.__validate_tickers(tickers) if validate_tickers else tickers
-        self.validate_tickers = validate_tickers
 
-        self.info_to_find = info_to_find
-        self.num_options = len(info_to_find)
+        # find stocks straight away if validation doesn't matter
+        self.stock_info: Dict[str, Dict[str, str]] = dict() if validate_tickers else self.find_stocks(tickers)
+
+        # validate stocks and then automatically find stock information as validation occurs
+        self.validate_tickers = validate_tickers
+        self.tickers: List[str] = self.check_tickers(tickers) if validate_tickers else tickers
 
-        self.browser = self.__configure_browser()
+        
+        
     
     @staticmethod
     def __create_progress_bar(progress_message: str, max_value: int) -> progressbar:
         """
         Creates an animated progress bar displaying the given message, and with a length of
         the given max.
 
@@ -62,15 +69,15 @@
             ' [', progressbar.ETA(), ']\n',
             ]
         
         progress_bar = progressbar.ProgressBar(max_value=max_value, widgets=widgets)
         return progress_bar
     
 
-    def __explicit_wait(self, search_method: By, element: str, max_wait_time: int = 2) -> str:
+    def _explicit_wait(self, search_method: By, element: str, max_wait_time: int = 2) -> str:
         """
         Explicitly waits for the given element to be located on the browser's page
         before proceeding to gather its value.
 
         Args
             element: the element whose presence is being awaited
             max_wait_time: the amount of time to wait before 'giving up' finding the element
@@ -85,82 +92,97 @@
                 EC.presence_of_element_located((search_method, element))
             ).text
         except:
             element_value = "N/A"
         return element_value
     
 
-    def __valid_ticker(self, ticker: str) -> bool:
+    def valid_ticker(self, ticker: str) -> bool:
         """
-        Determines if the given ticker is valid--i.e. 5 or fewer characters
+        Determines if the given ticker is valid--i.e. 5 or fewer characters and exists
+        on yahoo finance. Will scrape the information and store if valid.
 
-        Args
+        Args:
             ticker: the ticker to validate
         
-        Returns
+        Returns:
             True if valid, False if invalid
         """
         ticker_len = len(ticker)
-        return ticker_len <= 5 and ticker_len > 0
+        stock = self.get_stock_info(ticker)
+
+        valid = (ticker_len <= 5 and ticker_len > 0) and (stock != dict())
+        if valid:
+            self.stock_info[ticker] = stock
+
+        return valid
 
     
-    def __validate_tickers(self, tickers: List[str]) -> List[str]:
+    def check_tickers(self, tickers: List[str]) -> List[str]:
         """
         Determines if the given stock tickers are valid--i.e. 5 or fewer
-        characters.
+        characters and exists on yahoo finance.
 
         Args:
             tickers: the list of stock tickers to validate
 
         Returns:
             valid_tickers: the list of valid tickers, if any
         """
         valid_tickers: List[str] = []
 
-        for idx, ticker in enumerate(tickers):
-            ticker = ticker.upper()
-            valid_ticker = [ticker] if self.__valid_ticker(ticker) else self.__request_new_ticker(ticker)
+        for ticker in tickers:
+            valid_ticker = [ticker] if self.valid_ticker(ticker) else self.__request_new_ticker(ticker)
             valid_tickers.extend(valid_ticker)
 
         return valid_tickers
     
 
     def __request_new_ticker(self, invalid_ticker: str) -> List[str]:
         """
         Asks the user via the terminal for a new ticker to replace the
         invalid one.
 
-        Args
+        Args:
             invalid_ticker: the invalid ticker originally provided by the user
 
-        Returns
+        Returns:
             valid_ticker: empty if no replacement given, one-element list if
                           valid replacement provided
+
+        Raises:
+            ValueError: if an invalid response to the 'request new ticker' question
+                        is provided.
         """
-        request_new = input(f"The provided ticker {invalid_ticker} is invalid. Would you like to choose another (y/n)?:  ")
+        request_new = input(f"The provided ticker {invalid_ticker} is invalid/does not exist. Would you like to choose another (y/n)?:  ")
+        # dont choose new ticker
         if request_new.lower() == "n":
             return []
-        
+        elif request_new.lower() != "y":
+            raise ValueError("Invalid response provided. Expected either 'y' or 'n'")
+
+        # choose new ticker
         valid_ticker: List[str] = []
         valid_provided = False
 
         while not valid_provided:
             new_ticker = input(f"New ticker: ").upper()
             # valid provided
-            if self.__valid_ticker(new_ticker):
+            if self.valid_ticker(new_ticker):
                 valid_ticker.append(new_ticker)
                 break
             else:
                 # ask again
                 valid_ticker = self.__request_new_ticker(new_ticker)
             
         return valid_ticker
     
 
-    def __configure_browser(self) -> webdriver:
+    @staticmethod
+    def __configure_browser() -> webdriver:
         """
         Downloads (if one doesn't already exist) and configures a ChromeDriver with basic options.
 
         Returns:
             browser: the configured webdriver on finance.yahoo.com
         """
         get_driver = GetChromeDriver()
@@ -188,15 +210,15 @@
 
         Returns:
             True if the stock could be found, False otherwise
         """
         url = f"https://finance.yahoo.com/quote/{ticker}?p={ticker}&.tsrc=fin-srch"
         self.browser.get(url)
         if self.stock_exists(expected_url=url):
-            self.__explicit_wait(By.ID, "quote-header-info")
+            self._explicit_wait(By.ID, "quote-header-info")
             return True
         
         return False
 
 
     def stock_exists(self, expected_url: str) -> bool:
         """
@@ -210,67 +232,69 @@
         Returns:
             True if the stock exists, False otherwise
         """
         current_url = self.browser.current_url
         return current_url == expected_url
 
 
-    def __get_stock_info(self, ticker: str) -> Dict[str, str]:
+    def get_stock_info(self, ticker: str) -> Dict[str, str]:
         """
         Gathers all information, requested by the user, about the given stock,
         if it could be found.
 
         Args:
             ticker: the ticker of the stock whose info is being gathered
 
         Returns:
             stock_info: information about the stock
         """
         stock_info: Dict[str, str] = dict()
 
         if self.__find_stock(ticker):
-            for idx, info in enumerate(self.info_to_find):
+            for info in self.info_to_find:
+                # get information
                 info_val = info.value
-                info_name = self.__explicit_wait(By.XPATH, info_val['name_loc'])
-                info_text = self.__explicit_wait(By.XPATH, info_val['info_loc'])
+                info_name = self._explicit_wait(By.XPATH, info_val['name_loc'])
+                info_text = self._explicit_wait(By.XPATH, info_val['info_loc'])
+                # store information
                 stock_info[info_name] = info_text
-
+                
         return stock_info
     
 
-    def __find_stocks(self) -> Dict[str, Dict[str, str]]:
+    def find_stocks(self, tickers: List[str]) -> Dict[str, Dict[str, str]]:
         """
         Finds all the stocks, with their information, requested by the user
 
+        Args:
+            tickers: the tickers of the stocks to find
+        
         Returns:
             all_stocks_info: keys = the stock names  |  values = the stock information
         """
         all_stocks_info: Dict[str, Dict[str, str]] = dict()
 
-        for idx, ticker in enumerate(self.tickers): 
-            all_stocks_info[ticker] = self.__get_stock_info(ticker)
+        for ticker in tickers: 
+            all_stocks_info[ticker] = self.get_stock_info(ticker)
 
         return all_stocks_info
     
 
-    def scrape(self, display_info: bool = True) -> Dict[str, Dict[str, str]]:
+    def display_data(self, data: Dict = None) -> None:
         """
-        Runs the scraper to find all the stock information
+        Displays the given data in the terminal as 'pretty' json. Defaults
+        to displaying data about the stocks scraped.
 
         Args:
-            display_info: if the results of the search should be displayed in the
-                          terminal
-
-        Returns:
-            stock_info: the stocks' information
+            data: the data to be displayed in the terminal
         """
-        stock_info = self.__find_stocks()
-        formatted_info = json.dumps(stock_info, indent=4)
-        print(formatted_info)
-        return stock_info
+        if data:
+            print(json.dumps(data, indent=4))
+        else:
+            print(json.dumps(self.stock_info, indent=4))
     
 
     def download_data(self, file_type: str, file_path: str, overwrite: bool = True) -> None:
         """
         Download's the given stock information to a file of the given type.
 
         File Type options: 
@@ -286,15 +310,15 @@
 
         Raises:
             ValueError: if an invalid/unsupported file type is provided or if
                         attempting to download a file of one type using a different
                         method (e.g. markdown in sample.json)
         """
         downloader = Downloader(
-            self.scrape(), 
+            self.stock_info, 
             file_path=file_path,
             overwrite=overwrite
         )
 
         download_methods = {
             "json": downloader.download_json,
             "csv": downloader.download_csv,
@@ -302,11 +326,8 @@
             "markdown": downloader.download_md
         }
         supported_file_types = download_methods.keys()
         
         if file_type.lower() not in supported_file_types:
             raise ValueError("Invalid file type provided. Expected one of: %s" % supported_file_types)
         else:
-            download_methods[file_type]()
-        
-        
-    
+            download_methods[file_type]()
```

### Comparing `finance-scrapers-0.1.5/setup.cfg` & `finance-scrapers-1.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 696e 616e 6365 2d73 6372 6170   = finance-scrap
-00000020: 6572 730d 0a76 6572 7369 6f6e 203d 2030  ers..version = 0
+00000020: 6572 730d 0a76 6572 7369 6f6e 203d 2031  ers..version = 1
 00000030: 2e31 2e35 0d0a 6175 7468 6f72 203d 204d  .1.5..author = M
 00000040: 616e 6479 2d63 7962 6572 0d0a 6465 7363  andy-cyber..desc
 00000050: 7269 7074 696f 6e20 3d20 4120 746f 6f6c  ription = A tool
 00000060: 2074 6f20 7363 7261 7065 2061 6e64 2064   to scrape and d
 00000070: 6f77 6e6c 6f61 6420 7075 626c 6963 6c79  ownload publicly
 00000080: 2061 7661 696c 6162 6c65 2073 746f 636b   available stock
 00000090: 2069 6e66 6f72 6d61 7469 6f6e 2e20 4375   information. Cu
@@ -39,10 +39,11 @@
 00000260: 7320 3d20 0d0a 0973 656c 656e 6975 6d0d  s = ...selenium.
 00000270: 0a09 7265 7175 6573 7473 0d0a 0967 6574  ..requests...get
 00000280: 5f63 6872 6f6d 655f 6472 6976 6572 0d0a  _chrome_driver..
 00000290: 0970 726f 6772 6573 7362 6172 0d0a 0970  .progressbar...p
 000002a0: 726f 6772 6573 7362 6172 320d 0a09 7479  rogressbar2...ty
 000002b0: 7065 720d 0a09 7479 7069 6e67 5f65 7874  per...typing_ext
 000002c0: 656e 7369 6f6e 730d 0a09 7061 6e64 6173  ensions...pandas
-000002d0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000002e0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000002f0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000002d0: 0d0a 0974 6162 756c 6174 650d 0a0d 0a5b  ...tabulate....[
+000002e0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000002f0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000300: 6520 3d20 300d 0a0d 0a                   e = 0....
```

