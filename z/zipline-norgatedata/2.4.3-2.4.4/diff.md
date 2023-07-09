# Comparing `tmp/zipline_norgatedata-2.4.3-py3-none-any.whl.zip` & `tmp/zipline_norgatedata-2.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 37179 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     9650 b- defN 23-Jun-06 03:29 zipline_norgatedata/CHANGES.txt
+Zip file size: 38384 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     9796 b- defN 23-Jul-09 02:10 zipline_norgatedata/CHANGES.txt
 -rw-rw-rw-  2.0 fat    16020 b- defN 20-Sep-09 09:35 zipline_norgatedata/LICENSE.txt
 -rw-rw-rw-  2.0 fat       62 b- defN 19-Aug-27 04:23 zipline_norgatedata/__init__.py
 -rw-rw-rw-  2.0 fat    10981 b- defN 23-May-01 11:22 zipline_norgatedata/pipelines.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-06 03:28 zipline_norgatedata/version.py
--rw-rw-rw-  2.0 fat    43449 b- defN 23-Jun-06 04:52 zipline_norgatedata/zipline_norgatedata.py
--rw-rw-rw-  2.0 fat    16020 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    29504 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      990 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/RECORD
-11 files, 126811 bytes uncompressed, 35481 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-09 02:11 zipline_norgatedata/version.py
+-rw-rw-rw-  2.0 fat    43637 b- defN 23-Jul-09 02:25 zipline_norgatedata/zipline_norgatedata.py
+-rw-rw-rw-  2.0 fat    16020 b- defN 23-Jul-09 02:27 zipline_norgatedata-2.4.4.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    34322 b- defN 23-Jul-09 02:27 zipline_norgatedata-2.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 02:27 zipline_norgatedata-2.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-09 02:27 zipline_norgatedata-2.4.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      990 b- defN 23-Jul-09 02:27 zipline_norgatedata-2.4.4.dist-info/RECORD
+11 files, 131963 bytes uncompressed, 36686 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: zipline_norgatedata/version.py
 Comment: 
 
 Filename: zipline_norgatedata/zipline_norgatedata.py
 Comment: 
 
-Filename: zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT
+Filename: zipline_norgatedata-2.4.4.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: zipline_norgatedata-2.4.3.dist-info/METADATA
+Filename: zipline_norgatedata-2.4.4.dist-info/METADATA
 Comment: 
 
-Filename: zipline_norgatedata-2.4.3.dist-info/WHEEL
+Filename: zipline_norgatedata-2.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: zipline_norgatedata-2.4.3.dist-info/top_level.txt
+Filename: zipline_norgatedata-2.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: zipline_norgatedata-2.4.3.dist-info/RECORD
+Filename: zipline_norgatedata-2.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zipline_norgatedata/CHANGES.txt

```diff
@@ -113,7 +113,8 @@
 v2.3.3 20230122 Notes on TSXFailures patch
 v2.3.4 20230222 Update documentation to specify sqlalchemy<2
 v2.4.0 20230506 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
 v2.4.1 20230507 Minor documentation fixes on installation method
 v2.4.1 20230507 Documentation fixes
 v2.4.2 20230507 Documentation fixes, revised Clenow scripts
 v2.4.3 20230606 Revised information on extending backtests to 1970 by patching Zipline, better start/end session handling so that you don't have to be on an actual trading date
+v2.4.4 20230709 Prevent TypeError: Cannot compare tz-naive and tz-aware timestamps on bundle ingest when normalizing start and end session dates
```

## zipline_norgatedata/version.py

```diff
@@ -1 +1 @@
-__version__ = '2.4.3'
+__version__ = '2.4.4'
```

## zipline_norgatedata/zipline_norgatedata.py

```diff
@@ -116,14 +116,17 @@
         start_session = cal.first_session
         if start_session.weekday() == 6: # Don't start on Sundays, this helps with futures testing...
             start_session = cal.next_close(start_session).floor(freq="D")
         #logger.info("  Realigning start to " + start_session.strftime("%Y-%m-%d"))
     if not (cal.is_session(end_session)):
         end_session = cal.previous_close(end_session).floor(freq="D")
         #logger.info("  Realigning end to " + end_session.strftime("%Y-%m-%d"))
+    # Take out TZ now just in case cal inserts it, since sessions should be TZ-naive
+    start_session = start_session.tz_localize(None)
+    end_session = end_session.tz_localize(None)
     return start_session, end_session
 
 def define_non_US_country_code(exchanges):
     aulist = ('ASX','AU IDX')
     for exchange in aulist:
         #if exchanges.index.contains(exchange):
         if exchange in exchanges.index:
```

## Comparing `zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT` & `zipline_norgatedata-2.4.4.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

## Comparing `zipline_norgatedata-2.4.3.dist-info/METADATA` & `zipline_norgatedata-2.4.4.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-norgatedata
-Version: 2.4.3
+Version: 2.4.4
 Summary: Zipline extension to provide bundles of data from Norgate Data into the Zipline algorithmic trading library for the Python programming language
 Home-page: https://norgatedata.com
 Author: NorgateData Pty Ltd
 Author-email: support@norgatedata.com
 License: EULA
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,32 +28,67 @@
 
 Key features of this extension
  * Simple bundle creation
  * Survivorship bias-free bundles
  * Incorporates time series data such as historical index membership and dividend yield into Zipline's Pipeline mechanism
  * No modifications to the Zipline code base (except to fix problems with installation and obsolete calls that crash Zipline)
 
+# Table of Contents
+
+- [Requirements](#requirements)
+- [How to install Zipline using Anaconda/Miniconda](#how-to-install-zipline-using-anaconda-miniconda)
+  * [How to install Zipline Reloaded and PyFolio, and Zipline-NorgateData](#how-to-install-zipline-reloaded-and-pyfolio--and-zipline-norgatedata)
+  * [Upgrades of Zipline-NorgateData](#upgrades-of-zipline-norgatedata)
+- [Exchange Calendar Issues that require patching](#exchange-calendar-issues-that-require-patching)
+  * [Patch to allow backtesting before 20 years ago](#patch-to-allow-backtesting-before-20-years-ago)
+  * [Additional patch to allow backtesting before 1990](#additional-patch-to-allow-backtesting-before-1990)
+  * [Patch to allow calendars other than US calendars for backtesting](#patch-to-allow-calendars-other-than-us-calendars-for-backtesting)
+  * [Patches for Canadian equities](#patches-for-canadian-equities)
+- [Backtest Assumptions](#backtest-assumptions)
+- [Bundle Creation](#bundle-creation)
+- [Benchmark against a symbol](#benchmark-against-a-symbol)
+- [Pipelines - accessing timeseries data](#pipelines---accessing-timeseries-data)
+- [Worked example backtesting S&P 500 Constituents back to 1990](#worked-example-backtesting-s-p-500-constituents-back-to-1990)
+- [Worked example backtesting E-Mini S&P 500 futures](#worked-example-backtesting-e-mini-s-p-500-futures)
+- [Metadata](#metadata)
+- [Norgate Data Futures Market Session symbols](#norgate-data-futures-market-session-symbols)
+- [Zipline Limitations/Quirks](#zipline-limitations-quirks)
+- [Testing on Australian ASX data](#testing-on-australian-asx-data)
+- [Testing on Canadian TSX data](#testing-on-canadian-tsx-data)
+- [Books/publications that use Zipline, adapted for Norgate Data use](#books-publications-that-use-zipline--adapted-for-norgate-data-use)
+- [FAQs](#faqs)
+    + [During a backtest I receive an error ValueError: 'Time Period' is not in list.  How do I fix this?](#during-a-backtest-i-receive-an-error-valueerror---time-period--is-not-in-list--how-do-i-fix-this-)
+    + [During a backtest, an error message is shown for index_constituent_timeseries](#during-a-backtest--an-error-message-is-shown-for-index-constituent-timeseries)
+- [Change log](#change-log)
+- [Installing older versions](#installing-older-versions)
+- [Support](#support)
+- [Thanks](#thanks)
+- [Recent Version History](#recent-version-history)
+
+<a id="requirements"></a>
 # Requirements
 
 * Zipline 2.4 and above (based upon the [Zipline Reloaded fork](https://zipline.ml4trading.io/) led by Stefan Jansen, which originates from the Quantopian-developed Zipline (which became become abandonware).  We recommend the latest release of Zipline Reloaded (currently v2.4) and associated packages (such as exchange-calendars) - there are too many quirks and workarounds for issues with older versions of Zipline to continue to maintain backwards compatibility.
 * Python 3.8+ (Python 3.10 recommended)
 * Microsoft Windows
 * An active [Norgate Data](https://norgatedata.com/) subscription
 * Norgate Data Updater software installed and running
 * Writable local user folder named .norgatedata (or defined in environment variable NORGATEDATA_ROOT) - defaults to C:\\Users\\Your username\\.norgatedata
 * Python packages: Pandas, Numpy, Logbook
 
 Note: The "Norgate Data Updater" application (NDU) is a Windows-only application. NDU must be running for this Python package to work.
 
+<a id="how-to-install-zipline-using-anaconda-miniconda"></a>
 # How to install Zipline using Anaconda/Miniconda
 
 Most people have problems installing Zipline because they attempt to install it into their base environment.  The solution is simple:  Create a separate virtual environment that only has the necessary Python pacakges you require.  If you want to experiment then just create a new environment.
 
 Firstly, install either Anaconda (graphical environment) or Miniconda (cut-down command-line-based).  These instructions relate to Windows only.
 
+<a id="how-to-install-zipline-reloaded-and-pyfolio--and-zipline-norgatedata"></a>
 ## How to install Zipline Reloaded and PyFolio, and Zipline-NorgateData
 
 Here's how we installed it here at Norgate:  
 Note:  We use Mamba instead of conda for the majority of the install, as it seems to be much quicker in resolving everything (ie seconds instead of minutes) and parallelizing the downlodas/install.
 
 Install the latest 64 bit [MiniConda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda Distribution](https://www.anaconda.com/distribution/).
 
@@ -71,26 +106,29 @@
 pip install norgatedata zipline-norgatedata
 if not exist %HOMEPATH%\.zipline mkdir %HOMEPATH%\.zipline
 if not exist %HOMEPATH%\.zipline\extension.py copy /b NUL %HOMEPATH%\.zipline\extension.py
 ````
 
 Note:  Mamba is used to install zipline-reloaded, because the Conda package manager becomes confused with so many dependencies required.  Mamba is also about 10 times quicker than Conda.
 
+<a id="upgrades-of-zipline-norgatedata"></a>
 ## Upgrades of Zipline-NorgateData
 
 To receive upgrades/updates
 
 ```sh
 pip install zipline-norgatedata --upgrade
 ```
 
+<a id="exchange-calendar-issues-that-require-patching"></a>
 # Exchange Calendar Issues that require patching
 
 Norgate Data has developed the following patches.  Please make sure you implement the ones applicable to you.
 
+<a id="patch-to-allow-backtesting-before-20-years-ago"></a>
 ## Patch to allow backtesting before 20 years ago
 
 Unfortunately this is hardcoded into exchange_calendars for some reason.  To extend backtesting beyond more than 20 years from today:
 
 Navigate to the exchange_calendars folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\exchange_calendars**
 
 Edit exchange_calendars.py
@@ -101,14 +139,15 @@
 ```
 to the following:
 ```
 GLOBAL_DEFAULT_START = pd.Timestamp('1970-01-01')
 ```
 
 
+<a id="additional-patch-to-allow-backtesting-before-1990"></a>
 ## Additional patch to allow backtesting before 1990
 
 In addition to the "20 year" patch above if you want to do backtesting prior to 1990 you will need to patch Zipline to handle that too.
 
 Navigate to the zipline folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\ziplines**
 
 Navigate to the subfolder utils.
@@ -121,14 +160,15 @@
 ```
 to the following:
 ```
         return ec_get_calendar(*args, side="right", start=pd.Timestamp("1970-01-01"))
 ```
 
 
+<a id="patch-to-allow-calendars-other-than-us-calendars-for-backtesting"></a>
 ## Patch to allow calendars other than US calendars for backtesting
 
 If you see the message "AssertionError: All readers must share target trading_calendar." then you probably need this patch.  Our testing shows that AU and CA stocks users need this.
 
 Navigate to the zipline folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\zipline**
 
 Navigate to the data subfolder and edit the file dipatch_bar_reader.py
@@ -152,14 +192,15 @@
 	        "match the desired shared calendar={3} ".format(
 	            r, t, r.trading_calendar, trading_calendar)
 ```
 
 (For further details, see https://github.com/quantopian/zipline/issues/2684 - this has been an issue for some time and the original solution doesn't address the issue since there are actually two instances of the calendar - one from run_algorithm and one from the register_bundle within extension.py)
 
 
+<a id="patches-for-canadian-equities"></a>
 ## Patches for Canadian equities
 
 Of you are a Canadian Stocks user, you probably want to add this as a holiday:
 
 On 17 Dec 2008, TSX had a major outage and was halted not long after the open, and never reopened.  In general, the financial industry has written off this day as a bust for the purposes of data analysis.
 
 The New Years observance shift to Monday only started in 2000.
@@ -188,18 +229,20 @@
         return list(chain(September11ClosingsCanada),TSXFailure20081217,)
 
 ```
 
 
 
 
+<a id="backtest-assumptions"></a>
 # Backtest Assumptions
 - Stocks are automatically set an auto_close_date of the last quoted date 
 - Futures are automatically set an auto_close_date to the earlier of following: 2 days prior to last trading date (for cash settled futures, and physically delivered futures that only allow delivery after the last trading date), or 2 trading days prior to first notice date for futures that have a first notice date prior to the last trading date.
 
+<a id="bundle-creation"></a>
 # Bundle Creation 
 
 Navigate to your Zipline local settings folder.  This is typically located at **c:\\users\\<your username>\\.zipline**
 
 Add the following lines at the top of your Zipline local settings file - extension.py (:
 **Note:  This is _NOT_ the extension.py file inside the Anaconda3\\envs\\<your environment>\\lib\\site-packages\\zipline**
 
@@ -301,24 +344,26 @@
 
 To ingest a bundle:
 
 ```sh
 zipline ingest -b <bundlename>
 ```
 
+<a id="benchmark-against-a-symbol"></a>
 # Benchmark against a symbol
 
 To benchmark against an index, you should use add set_benchmark within the intialize function.
 
 ```py
  def initialize(context):
     set_benchmark(symbol('$SPXTR')) # Note: $SPXTR must be included in the bundle
     # ...
 ```
 
+<a id="pipelines---accessing-timeseries-data"></a>
 # Pipelines - accessing timeseries data
 
 Timeseries data has been exposed into Zipline's Pipeline interface.   During a backtest, the Pipelines will be calculated against all securities in the bundle.
 
 The following Filter (i.e. boolean) pipelines are available:
  - [NorgateDataIndexConstituent](https://norgatedata.com/data-content-tables.php#ushics)
  - [NorgateDataMajorExchangeListed](https://norgatedata.com/data-content-tables.php#usmajorexchangelisted)
@@ -382,14 +427,15 @@
             order_target_percent(asset,0.0)
 
     # ... your code here ...
 ```
 
 Note: Access to historical index constituents requires a Norgate Data Stocks subscription at the Platinum or Diamond level.
 
+<a id="worked-example-backtesting-s-p-500-constituents-back-to-1990"></a>
 # Worked example backtesting S&P 500 Constituents back to 1990
 
 This example comprises a backtest on the S&P 500, with a basic trend filter that is applied on the S&P 500 index ($SPX).  The total return version of the index is also ingested ($SPXTR) for comparison purposes.
 
 Note: This requires a Norgate Data US Stocks subscription at the Platinum or Diamond level.
 
 Create a bundle definition in extensions.py as follows:
@@ -449,14 +495,15 @@
         if asset not in context.assets:
             order_target_percent(asset,0.0)
 
     # ...
 ```
 
 
+<a id="worked-example-backtesting-e-mini-s-p-500-futures"></a>
 # Worked example backtesting E-Mini S&P 500 futures
 
 This example created a continuous contract of the E-Mini S&P 500 futures that trade on CME on volume.
 
 Create a bundle definition in extensions.py as follows:
 
 ```py
@@ -531,38 +578,42 @@
 
     # Finally, if there are open positions check for rolls
     if len(open_pos) > 0:   
         roll_futures(context, data)           
 
 ```
 
+<a id="metadata"></a>
 # Metadata
 
 The following fields are available in the metadata dataframe: start_date, end_date, ac_date, symbol, asset_name, exchange, exchange_full, asset_type, norgate_data_symbol, norgate_data_assetid.  
 
+<a id="norgate-data-futures-market-session-symbols"></a>
 # Norgate Data Futures Market Session symbols
 
 To obtain just the futures market sessions symbols, you can use the norgatedata package and adapt the following code:
 ```py
 import norgatedata
 for session_symbol in norgatedata.futures_market_session_symbols():
     print (session_symbol + " " + norgatedata.futures_market_session_name(session_symbol)) 
 ```
 
+<a id="zipline-limitations-quirks"></a>
 # Zipline Limitations/Quirks
 
 - Zipline 2.4.2 is hardcoded ignore dates prior to 1990-01-01.  It can be patched to 1970-01-01, but no cannot go any further since it uses the Unix Epoch (1970-01-01) as the underlying time storage mechanism.
 - Zipline doesn't define all futures markets and doesn't provide any runtime extensibility in this area - you will need to add them to <your_environment>\lib\site-packages\zipline\finance\constants.py if they are not defined.  Be sure to backup this file as it will be overwritten any time you update zipline.
 - Zipline assumes that there are bars for every day of trading.  If a security doesn't trade for a given day (e.g. it was halted/suspended, or simply nobody wanted to trade it), it will be padded with the previous close repeated in the OHLC fields, with volume set to zero.  Consider how this might affect your trading calculations.  
 - Index volumes cannot be accurately ingested due to Zipline trying to convert large volumes to UINTs which are out-of-bounds for UINT32.  Index volumes will be divided by 1000.
 - Any stock whose adjusted volume exceeds the upper bound of UINT32 will be set to the maximum UINT32 value (4294967295).  This only occurs for stocks with a lot of splits and/or very large special dsitributions.
 - Some stocks have adjusted volume values that fall below the boundaries used by winsorize_uint32 (e.g. volume of 8.225255e-05).  You'll see a warning when those stocks are ingested "UserWarning: Ignoring 12911 values because they are out of bounds for uint32".   These are  There's not much we can do here.  For now, just ignore those warnings.
 - Ingestion times could be improved significantly with multiprocessing (this would require Zipline enhancements)
 - Zipline cannot handle negative prices (eg. Crude Oil in 2020) - any such prices will be set to zero.  Most systems would have rolled prior to this strange event anyway.
 
+<a id="testing-on-australian-asx-data"></a>
 # Testing on Australian ASX data
 
 By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.  For the ASX, the calendar name is XASX.    
 
 At the top of your algorithm:
 ```py
 from exchange_calendars import get_calendar
@@ -578,14 +629,15 @@
     capital_base=10000, 
     trading_calendar=get_calendar('XASX',start="1990-01-01"),
     data_frequency = 'daily', 
     bundle='norgatedata-spasx200',
 )
 ```
 
+<a id="testing-on-canadian-tsx-data"></a>
 # Testing on Canadian TSX data
 
 By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.  For the TSX, the calendar name is XTSE.  
 
 At the top of your algorithm:
 ```py
 from trading_calendars import get_calendar
@@ -603,36 +655,39 @@
     data_frequency = 'daily', 
     bundle='norgatedata-sptsx60',
 )
 ```
 
 Be sure to implement the trading_calendars patch mentioned above too.
 
+<a id="books-publications-that-use-zipline--adapted-for-norgate-data-use"></a>
 # Books/publications that use Zipline, adapted for Norgate Data use
 
 We have adapted the Python code in the following books to use Norgate Data.  
 [Trading Evoled:  Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  
 
 Source code compatible with Zipline (Reloaded) v2.4 in Jupyter notebook format, can be downloaded here:
 https://norgatedata.com/book-examples/trading-evolved/NorgateDataTradingEvolvedExamples.zipline240.2.zip
 
 If there are other book/publications that use Zipline and worth adding here, let us know.
 
+<a id="faqs"></a>
 # FAQs
 
+<a id="during-a-backtest-i-receive-an-error-valueerror---time-period--is-not-in-list--how-do-i-fix-this-"></a>
 ### During a backtest I receive an error ValueError: 'Time Period' is not in list.  How do I fix this?
 
 This can occur when the items in the bundle do not match the latest data in the Norgate Data database.  For stocks, if there are symbol changes within the database then the bundle will have the old symbol but the Norgate database will have the new symbol.    For Futures, there may have been additional futures contracts listed since your previous ingestion and the roll-over algorithm is trying to roll into them.  
 
 The solution is simple:  Ingest the bundle with fresh data.
 
 Also consider putting Norgate Data Updater into manual mode for updating and using the NDU Trigger app to explicitly start NDU and obtain updates.  More information on this can be found here:
 https://norgatedata.com/ndu-usage.php
 
-
+<a id="during-a-backtest--an-error-message-is-shown-for-index-constituent-timeseries"></a>
 ### During a backtest, an error message is shown for index_constituent_timeseries
 
 For example, an error such as this is shown:
 
 ```
 [2023-06-05 07:39:25.720989] INFO: Norgate Data: Populating NorgateDataIndexConstituent pipeline populating with $DJI on 3638 securities from 2000-01-03 to 2023-06-02....
 [2023-06-05 07:39:34.734116] ERROR: Norgate Data: index_constituent_timeseries: DBD not found
@@ -645,46 +700,67 @@
 
 The solution is simple:  Ingest the bundle with fresh data.
 
 Also consider putting Norgate Data Updater into manual mode for updating and using the NDU Trigger app to explicitly start NDU and obtain updates.  More information on this can be found here:
 https://norgatedata.com/ndu-usage.php
 
 
+<a id="change-log"></a>
 # Change log
 
 Released versions and release dates can be seen here:
 https://pypi.org/project/zipline-norgatedata/#history
 
-The CHANGES.TXT within the package details the changes.
+The CHANGES.TXT within the package details the changes  A summary is also shown below.
 
+<a id="installing-older-versions"></a>
 # Installing older versions
 
 Older versions of Zipline-NorgateData can be installed easily using pip.  For example, to install v2.0.17.
 
 
 ````
 pip install zipline-norgatedata==2.0.17
 ````
 
 Note that prior versions may be only suited to older versions of Zipline.  However, due to the constantly evolving nature of Zipline, we can only really support the current version.
 
+<a id="support"></a>
 # Support
 
 For support on Norgate Data or usage of the zipline-norgatedata extension:
 [Norgate Data support](https://norgatedata.com/contact.php)
 
 Please put separate issues in separate emails, as this ensures each issue is separately ticketed and tracked.
 
 For bug reports on Zipline Reloaded, report them on Stefan Jansen's [Zipline Reloaded Github](https://github.com/stefan-jansen/zipline-reloaded/issues)
 
 There is also a Google Group, which isn't used much these days: [Zipline Google Group](https://groups.google.com/forum/#!forum/zipline).  
 
-
+<a id="thanks"></a>
 # Thanks
 
 Thanks to:
 
 * [Andreas Clenow](https://www.followingthetrend.com) for his pioneering work in documenting Zipline bundles in his latest book [Trading Evolved: Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  We used many of the techniques described in the book to build our bundle code.  There are many excellent examples of how to implement various trading systems including trend following, counter trend following, momentum, curve trading and combining multiple trading systems together.
 * Norgate Data alpha and beta testers.  Without your persistence we wouldn't have implemented half of the features.
 * The team that were formerly employed by Quantopian for developing and open sourcing Zipline
-* Continued development efforts on Zipline and associated packages since Quantopian ceased, by Stefan Jansen, Mehdi Bounouar, Allan Coppola and Shlomi Kushchi and many more.
+* Continued development efforts on Zipline and associated packages since Quantopian ceased, by [Stefan Jansen](https://ml4trading.io/), Mehdi Bounouar, Allan Coppola and Shlomi Kushchi and many more.
+
+<a id="recent-version-history"></a>
+# Recent Version History
+
+```
+v2.3.0 20220728 Bump to v2.3.0 due to version checking issue
+v2.3.1 20221027 Added Mac M1/M2 workaround to docs
+v2.3.2 20221114 Notes on Juneteenth holiday patch
+v2.3.3 20230122 Notes on TSXFailures patch
+v2.3.4 20230222 Update documentation to specify sqlalchemy<2
+v2.4.0 20230506 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
+v2.4.1 20230507 Minor documentation fixes on installation method
+v2.4.1 20230507 Documentation fixes
+v2.4.2 20230507 Documentation fixes, revised Clenow scripts
+v2.4.3 20230606 Revised information on extending backtests to 1970 by patching Zipline, better start/end session handling so that you don't have to be on an actual trading date
+v2.4.4 20230709 Prevent TypeError: Cannot compare tz-naive and tz-aware timestamps on bundle ingest when normalizing start and end session dates
+```
+
```

## Comparing `zipline_norgatedata-2.4.3.dist-info/RECORD` & `zipline_norgatedata-2.4.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-zipline_norgatedata/CHANGES.txt,sha256=B4K4F0UpgJAbSK2fQO_W_CDD7lnUymwSV8XXd4-cIFo,9650
+zipline_norgatedata/CHANGES.txt,sha256=PxUR6_zUNEHFqrrpqNYsrZkAMgGlmWSqLJScSVEFVi0,9796
 zipline_norgatedata/LICENSE.txt,sha256=6MW6JFLECMi-sugOZe7rA9yWqgm5caDNktT3JeQ1tDg,16020
 zipline_norgatedata/__init__.py,sha256=aXR_wp3lXNQD_L3LDXvl1kyVAtUfO7QCqvGxO2PexNA,62
 zipline_norgatedata/pipelines.py,sha256=XTtkyWnA0j0FkAsINJOTvEgnYMhnVTZva86ITk749Y8,10981
-zipline_norgatedata/version.py,sha256=G3ulfv4PF3ByvRJkX4W2UlKkB75b9xoCAR-byvYMmvM,23
-zipline_norgatedata/zipline_norgatedata.py,sha256=JMezU-udusYNISJ49Bkl5YguKSK7ialFoCWr1PK53DM,43449
-zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT,sha256=6MW6JFLECMi-sugOZe7rA9yWqgm5caDNktT3JeQ1tDg,16020
-zipline_norgatedata-2.4.3.dist-info/METADATA,sha256=G7YNAHFZoUz3PQeP2i1JaHXnhrSdKrM97evhxmj7r1Q,29504
-zipline_norgatedata-2.4.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-zipline_norgatedata-2.4.3.dist-info/top_level.txt,sha256=qBcvLFeVd6HtMgLdZ1Lemg-vrIP3TOnR2jWn2IH1SwM,20
-zipline_norgatedata-2.4.3.dist-info/RECORD,,
+zipline_norgatedata/version.py,sha256=wgKuFn1DcC8ugW7Ao_jyi0E1-qGLR9mw2vdASd5b76k,23
+zipline_norgatedata/zipline_norgatedata.py,sha256=EE6zvWMWJ8DTWfBjz3uErWTNnJUz4DP_hZWGY04xuTg,43637
+zipline_norgatedata-2.4.4.dist-info/LICENSE.TXT,sha256=6MW6JFLECMi-sugOZe7rA9yWqgm5caDNktT3JeQ1tDg,16020
+zipline_norgatedata-2.4.4.dist-info/METADATA,sha256=pKrKmv27KYh2O01WWsh7QnflIsTcIPKd1oyvhR_Z_Ek,34322
+zipline_norgatedata-2.4.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+zipline_norgatedata-2.4.4.dist-info/top_level.txt,sha256=qBcvLFeVd6HtMgLdZ1Lemg-vrIP3TOnR2jWn2IH1SwM,20
+zipline_norgatedata-2.4.4.dist-info/RECORD,,
```

