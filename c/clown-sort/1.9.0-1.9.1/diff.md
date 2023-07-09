# Comparing `tmp/clown_sort-1.9.0.tar.gz` & `tmp/clown_sort-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.9.0.tar", max compression
+gzip compressed data, was "clown_sort-1.9.1.tar", max compression
```

## Comparing `clown_sort-1.9.0.tar` & `clown_sort-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3534 2023-06-25 02:58:48.184419 clown_sort-1.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.9.0/LICENSE
--rw-r--r--   0        0        0     9287 2023-06-25 02:54:41.522424 clown_sort-1.9.0/README.md
--rw-r--r--   0        0        0     4431 2023-06-25 02:54:41.522832 clown_sort-1.9.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     8073 2023-06-25 02:54:41.523241 clown_sort-1.9.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.9.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4832 2023-06-25 02:54:41.523569 clown_sort-1.9.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0      392 2023-06-24 02:14:02.169664 clown_sort-1.9.0/clown_sort/files/import pdfplumber.py
--rw-r--r--   0        0        0     3766 2023-06-25 02:56:51.220186 clown_sort-1.9.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.9.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.9.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    11873 2023-06-25 02:54:41.524264 clown_sort-1.9.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     4181 2023-06-25 02:54:44.150613 clown_sort-1.9.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.9.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.9.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.9.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.9.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.9.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.9.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1712 2023-06-25 02:58:48.188486 clown_sort-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 clown_sort-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4098 2023-07-09 08:22:00.390857 clown_sort-1.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.9.1/LICENSE
+-rw-r--r--   0        0        0     9287 2023-06-25 02:54:41.522424 clown_sort-1.9.1/README.md
+-rw-r--r--   0        0        0     4502 2023-07-09 08:21:26.854406 clown_sort-1.9.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     8167 2023-07-09 08:21:26.854847 clown_sort-1.9.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.9.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4832 2023-06-25 02:54:41.523569 clown_sort-1.9.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0      392 2023-06-24 02:14:02.169664 clown_sort-1.9.1/clown_sort/files/import pdfplumber.py
+-rw-r--r--   0        0        0     4914 2023-07-09 08:21:26.855255 clown_sort-1.9.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    12130 2023-07-09 08:21:26.855827 clown_sort-1.9.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.9.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    12478 2023-07-06 21:33:53.445844 clown_sort-1.9.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     4416 2023-07-09 08:21:26.856147 clown_sort-1.9.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.9.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.9.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.9.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.9.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3527 2023-07-09 08:21:26.856578 clown_sort-1.9.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.9.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1713 2023-07-09 08:22:00.396643 clown_sort-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10710 1970-01-01 00:00:00.000000 clown_sort-1.9.1/PKG-INFO
```

### Comparing `clown_sort-1.9.0/CHANGELOG.md` & `clown_sort-1.9.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # NEXT RELEASE
 
+### 1.9.1
+* Output progress notifications to STDERR when parsing text from very large PDFs
+* Fix issue that caused explosive memory growth when parsing large PDFs
+* `--print-when-parsed` command line option for `extract_text_from_files`
+* Upgrade `pypdf` to `3.12.0` to resolve various PDF parsing failures
+* PDFs: Handle various exceptions when enumerating embedded images:
+   * `OSError: cannot write mode CMYK as PNG`
+   * `ValueError: not enough image data`
+   * `TypeError: unhashable type: 'ArrayObject'`
+   * `TypeError: unhashable type: 'IndirectObject'`
+
 # 1.9.0
 * Parse text from images in PDFs (some PDFs have no text only images)
 * Improve `extract_text_from_files` functionality
 
 ### 1.8.1
 * Actually make `extract_text_from_files` executable
```

### Comparing `clown_sort-1.9.0/LICENSE` & `clown_sort-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/README.md` & `clown_sort-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/__init__.py` & `clown_sort-1.9.1/clown_sort/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     """
     args: Namespace = extraction_parser.parse_args()
     console.line()
     files_to_process = []
 
     if args.debug:
         Config.enable_debug_mode()
+    if args.print_when_parsed:
+        Config.print_when_parsed = True
 
     for file_or_dir in args.file_or_dir:
         file_path = Path(file_or_dir)
 
         if not file_path.exists():
             console.print(f"File '{file_path}' doesn't exist!")
             sys.exit()
```

### Comparing `clown_sort-1.9.0/clown_sort/config.py` & `clown_sort-1.9.1/clown_sort/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from clown_sort.util.constants import CRYPTO_RULES_CSV_PATH, PACKAGE_NAME
 from clown_sort.util.filesystem_helper import subdirs_of_dir
 from clown_sort.util.logging import log, set_log_level
 
 StringOrPath = Union[str, Path]
 SortRule = namedtuple('SortRule', ['folder', 'regex'])
 
+MIN_PDF_SIZE_TO_LOG_PROGRESS_TO_STDERR = 1024 * 1024 * 20
 RULES_CSV_PATHS = 'RULES_CSV_PATHS'
 
 if RULES_CSV_PATHS in environ:
     DEFAULT_RULES_CSV_PATHS = str(environ.get(RULES_CSV_PATHS)).split(':')
 else:
     DEFAULT_RULES_CSV_PATHS = [CRYPTO_RULES_CSV_PATH]
 
@@ -39,14 +40,15 @@
     manual_fallback: bool = False
     only_if_match: bool = False
     leave_in_place: bool = False
     screenshots_only: bool = True
     delete_originals: bool = False
     rescan_sorted: bool = False
     yes_overwrite: bool = False
+    print_when_parsed: bool = False
     sort_rules: List[SortRule] = []
     filename_regex: re.Pattern
 
     @classmethod
     def configure(cls):
         """Parse arguments and configure."""
         if '--version' in sys.argv:
```

### Comparing `clown_sort-1.9.0/clown_sort/filename_extractor.py` & `clown_sort-1.9.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/files/image_file.py` & `clown_sort-1.9.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/files/pdf_file.py` & `clown_sort-1.9.1/clown_sort/files/pdf_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,60 +7,74 @@
 
 from PIL import Image
 from pypdf import PdfReader
 from pypdf.errors import DependencyError, EmptyFileError
 from rich.console import Console
 from rich.panel import Panel
 
-from clown_sort.config import check_for_pymupdf, log_optional_module_warning
+from clown_sort.config import (MIN_PDF_SIZE_TO_LOG_PROGRESS_TO_STDERR, Config, check_for_pymupdf,
+     log_optional_module_warning)
 from clown_sort.files.image_file import ImageFile
 from clown_sort.files.sortable_file import SortableFile
 from clown_sort.util.logging import log
-from clown_sort.util.rich_helper import WARNING, console
+from clown_sort.util.rich_helper import WARNING, console, stderr_console
 
 MAX_DISPLAY_HEIGHT = 600
 SCALE_FACTOR = 0.4
 
 
 class PdfFile(SortableFile):
     is_presentable_in_popup = None
 
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
             return self._extracted_text
 
         log.debug(f"Extracting text from '{self.file_path}'...")
-        console_buffer = Console(file=io.StringIO())
         extracted_pages = []
 
         try:
             pdf_reader = PdfReader(self.file_path)
+            page_count = len(pdf_reader.pages)
+            log.debug(f"PDF Page count: {page_count}")
 
-            for page_number, page in enumerate(pdf_reader.pages):
-                console_buffer.print(Panel(f"PAGE {page_number + 1}", padding=(0, 15), expand=False))
-                console_buffer.print(page.extract_text().strip())
-
-                for image_number, image in enumerate(page.images, start=1):
-                    image_name = f"Page {page_number + 1}, Image {image_number}"
-                    console_buffer.print(Panel(image_name, expand=False))
-                    image_obj = Image.open(io.BytesIO(image.data))
-                    image_text = ImageFile.extract_text(image_obj, f"{self.file_path} ({image_name})")
-                    console_buffer.print((image_text or '').strip())
+            for page_number, page in enumerate(pdf_reader.pages, start=1):
+                self._log_to_stderr(f"Parsing page {page_number}...")
+                page_buffer = Console(file=io.StringIO())
+                page_buffer.print(Panel(f"PAGE {page_number}", padding=(0, 15), expand=False))
+                page_buffer.print(page.extract_text().strip())
+                image_number = 1
+
+                # Extracting images is a bit fraught (lots of PIL and pypdf exceptions have come from here)
+                try:
+                    for image_number, image in enumerate(page.images, start=1):
+                        image_name = f"Page {page_number}, Image {image_number}"
+                        self._log_to_stderr(f"   Processing {image_name}...")
+                        page_buffer.print(Panel(image_name, expand=False))
+                        image_obj = Image.open(io.BytesIO(image.data))
+                        image_text = ImageFile.extract_text(image_obj, f"{self.file_path} ({image_name})")
+                        page_buffer.print((image_text or '').strip())
+                except (NotImplementedError, OSError, TypeError, ValueError) as e:
+                    stderr_console.print(f"WARNING: {type(e).__name__}: {e} while parsing embedded image {image_number} on page {page_number}...")
+                    stderr_console.print_exception()
 
-                page_text = console_buffer.file.getvalue()
-                log.debug(page_text)
+                page_text = page_buffer.file.getvalue()
                 extracted_pages.append(page_text)
+                log.debug(page_text)
+
+                if Config.print_when_parsed:
+                    print(f"{page_text}")
         except DependencyError:
             log_optional_module_warning('pdf')
         except EmptyFileError:
             log.warn("Skipping empty file!")
 
-        self.text_extraction_attempted = True
         self._extracted_text = "\n\n".join(extracted_pages).strip()
+        self.text_extraction_attempted = True
         return self._extracted_text
 
     def thumbnail_bytes(self) -> Optional[bytes]:
         """Return bytes for a thumbnail."""
         import fitz  # TODO: Can we do this without PyMuPDF dependency?
         log.debug(f"Getting bytes for '{self.file_path}'...")
 
@@ -91,9 +105,16 @@
         if not type(self).is_presentable_in_popup:
             console.line()
             msg = WARNING.append(f"File '{self.basename}' is not displayable without pymupdf...\n")
             console.print(msg)
 
         return type(self).is_presentable_in_popup
 
+    def _log_to_stderr(self, msg: str) -> None:
+        """When parsing very large PDFs it can be useful to log progress and other messages to STDERR."""
+        if self.file_size() < MIN_PDF_SIZE_TO_LOG_PROGRESS_TO_STDERR:
+            return
+
+        stderr_console.print(msg)
+
     def __repr__(self) -> str:
         return f"PdfFile('{self.file_path}')"
```

### Comparing `clown_sort-1.9.0/clown_sort/files/sortable_file.py` & `clown_sort-1.9.1/clown_sort/files/sortable_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,17 @@
         else:
             run(['open', self.file_path])
 
     def print_extracted_text(self, max_chars: Optional[int] = None) -> None:
         console.print(self._filename_panel())
         console.print(self._extracted_str())
 
+    def file_size(self) -> int:
+        return self.file_path.stat().st_size
+
     def _extracted_str(self, max_chars: Optional[int] = None) -> str:
         """Raw string version of extracted text but truncated to max_chars if provided."""
         txt = self.extracted_text()
 
         if txt is None:
             txt = "<No extracted text>"
         else:
```

### Comparing `clown_sort-1.9.0/clown_sort/sort_selector.py` & `clown_sort-1.9.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.9.1/clown_sort/sorting_rules/crypto.csv`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 ConsenSys,ConsenSys
 Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b|\bMomnt
+Crypto Capital,Global[-_\s.]*Transaction[-_\s.]*Services|Crypto[-_\s.]*Capital\b
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s|Doug(las)?[-_\s.]*Ching\b|Bobby[-_\s.]*Bao\b|Gary[-_\s.]*Or\b|Marszalek|Rafael[-_\s.]*Melo\b
 CUBI,\bCUBI\b|Customers[-_\s.]*Ban(k|corp)
 Cumberland,cumberland
 Custodia,custodia\b|caitlin[-_\s.]*long
 dalle,craiyon|midjourney|\bdall[-_\s.]*e\b
 DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b|hq[-_\s.]*digital|Alana[-_\s.]*Ackerson|Jennifer[-_\s.]*Mitrenga|Emily[-_\s.]*(Heather[-_\s.]*)?Goodman|Founders[-_\s.]*Liquidity[-_\s.]*Fund
 DeFi,\bdefi\b|decentralized[-_\s.]*finance
@@ -59,50 +60,51 @@
 Effective Altruism,\bE\.?A\.?\b|effective[-_\s.]*altruism
 El Salvador,El[-_\s.]*Salvador|Bukele|Max[-_\s.]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Evertas,\bEvertas\b|Ryan[-_\s.]*Lackey
 Euler Finance,\bEuler\b
 FalconX,falconx
-First Digital,First[-_\s.]*Digital\b
-Flip Filipkowski,filipkowski
+First Digital,First[-_\s.]*Digital\b|Legacy[-_\s.]*Trust\b
 Finblox,finblox
+Fintech,Mercury\b(Azibo|\bChime(bank)|Nibiru|Brex|Checkout\.com|Holyheld|Pinwheel|Lithic|Unit21|Unlimin?t|Synapse|LendingClub|Piermont|Burling|Bangor|Klarna|Afterpay|Zeta|FirstDollar|Alto|Marqeta|Grasshopper|CheckOut|Allpoint|ArrowEye|C2Fo|Wagestream)\b|Treasury[-_\s.]*Prime|Chris[-_\s.]*Dean\b|Jim[-_\s.]*Brusstar|(Bangor|Third[-_\s.]*Coast|First[-_\s.]*Internet|Emprise)[-_\s.]*Bank
 Fireblocks,fireblocks
+Flip Filipkowski,filipkowski
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker|Yecheskel|Swift[-_\s.]*Staffing
-FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism[-_\s.]*capital|\bryne\b|clifton[-_\s.]*bay|\bZUBR\b
+FTX,FTX|\b(Bankman|FTT|SBF|Trabucco|Ellison|Nishad|Redline|Ryne|Tackett|ZUBR)\b|Moonstone|Friedberg|autism[-_\s.]*capital|clifton[-_\s.]*bay|Alameda
 Galaxy Digital,novogratz|Alex[-_\s.]*Thorn
 Gate.io,Gate[_.]?IO
 Gelato Network,Gelato[-_\s.]*Network|\bSorbet[-_\s.]*Finance|@gitpusha|hilmar[-_\s.]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s.]*Finance|Dave[-_\s.]*Leibowitz|Hilmar[-_\s.]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hamas,\bHamas\b|Al[-_\s.]*Qassam
 Haru Invest,\bHaru(invest)?\b|\b(happy)?Delio\b
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard[-_\s.]*Heart|Hexican
 Hoo,Hoo[-_\s.]*(Research|Exchange)|[#$]Hoo\b|Rexy[-_\s.]*(Hoo|Wang)|\bhoo\b
 Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s.]*Li\b|\b(GoPlus|Walken)\b
 Iran,\bIran\b|\bIranian\b|Nobitex|\bCoinNik|\bWallex\b|Sarmayex|\bRabex\b
 Jump Trading,Jump[-_\s.]*Trading|@jump_
-Justin Sun,justin[-_\s.]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina|\bR(ebo|ible)\b|Love[-_\s.]*Letters[-_\s.]*Limited|Objectivists[-_\s.]*Limited
+Justin Sun,justin[-_\s.]*sun|USDD|USDJ|pgala|sunswap|sunyuchentron|poloniex|web3nina|\bR(ebo|ible)\b|Love[-_\s.]*Letters[-_\s.]*Limited|Objectivists[-_\s.]*Limited
 Kazakhstan,\bkazakh|Freedom[-_\s.]*Holding|\balmaty|Timor[-_\s.]*Turlov|\bFFIN[-_\s.]*brokerage
 Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
 Kraken,kraken|payward|\bjespow\b|Jesse[-_\s.]*Powell
 KuCoin,kucoin
 Lead Bank,\bLead[-_\s.]*Bank\b|Finzly
 LBRY,LBRY|\bLBC\b
 Lexpunk Army,lexpunk|gabriel[-_\s.]*shapiro|_gabrielShapir0|\blex_node\b
 Lifeboat Foundation,Lifeboat[-_\s.]*Foundation
 North Korea,lazarus|North[-_\s.]*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
 Paul LeRoux,leroux
 Polygon Labs,polygon[-_\s.]*labs|ryan[-_\s.]*watt\b|@Fwiz|Rebecca[-_\s.]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
-Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s.]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners|\bGarzik\b
 Mario Nawfal,mario[-_\s.]*nawfal
+Matthew Roszak,\b(Beauregard|Bloq|Garzik|GoCoin)\b|(matthew)?[-_\s.]*roszak|Calvin[-_\s.]*Cheng|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners
 Messari,Ryan[-_\s.]*Selkis|twobitidiot|messari|@robustus|Dan[-_\s.]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s.]*Stewart|\bHayner\b
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s.]*(Bank|Commercial)|Mission[-_\s.]*Gateway|Aryeh[-_\s.]*Realty
 Multichain,Multichain\b
 Founders Bank,Michael[-_\s.]*Bianchi|Founders[-_\s.]*Bank
 Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s.]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s.]*seven|kin[-_\s.]*ming[-_\s.]*je|william[-_\s.]*je\b|\bHaoyun\b|\bLi[-_\s.]*You\b
@@ -119,18 +121,18 @@
 OneCoin,\bOne(Coin|Life)\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea\b
 PAG,\bpag\b|Weijian[-_\s.]*Shan
 Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s.]*(Youssef|Savant)|Artur[-_\s.]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
-Payrnet,Payrnet|Rails(r|bank)\b
+Payrnet,Rails(r|bank)\b|\b(Wirex|Cryptopay|Payrnet)\b
 Pi,\$PI[^\w]|Pi[-_\s.]*Network
 Politics,\bted[-_\s.]*cruz
-Prime Trust,Prime[-\s_]*Trust|\b(Banq|PrimeX|Sroge|anonalyx)\b|Scott[-\s_]*Purcell|(Planet|Fortress)[-\s_]*(Xyz|Trust|NFT)|George[-\s_]*Georgiades|Kevin[-\s_]*Lehtiniitty
+Prime Trust,\bPrime[-\s_]*(Trust|Core|IRA|Digital)\b|\b(Banq|PrimeX|Sroge|anonalyx|Kasidie)\b|Scott[-\s_]*Purcell|(Planet|Fortress)[-\s_]*(Xyz|Trust|NFT)|George[-\s_]*Georgiades|Kevin[-\s_]*Lehtiniitty
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s.]*Cotten|0xsifu\b|michael[-_\s.]*patryn|wonderland|daniele[-_\s.]*sesta\b
 Revolut,\bRevolut\b
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
@@ -142,19 +144,19 @@
 Skrill,\bSkrill\b
 Solana,(Solana|Serum)\b
 Stellar,\bStellar\b|[$#]?XLM
 Stifel Bank,\bStifel\b|[#$]SF\b
 Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
 Synapse,Synapse(fi|labs|protocol)?\b
 TerraLuna,\bluna\b|do[-_\s.]*kwon|stablekwon|\bTerra(form|Luna)?\b|Macedo|\bLuna[-_\s.]*Foundation\b|Mirror[-_\s.]*Protocol
-Tether,\b(BFXNA|BFXWW|Chesham|Coinapult|D10e|Devasini|GoCoin|Evertune|Friedberg|GamesTV|Hoegner|IGEL|Infomatec|Ludovicus|(Master|Real)coin|Mallers|Noblex|Paolo(Ardoino)?|Playsino|Renrenbee|SFP|Sinopec|SJMBT|Stablehouse|Sunlot|Tether|Tuxia|urwhatyouknow|USDT|XBTO|Xfire)\b|Noble[-_\s.]*Bank|\bDeltec[^\']|\b(B[ei]t|i|Digi?|Eth)finex[^e']|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|[$#]LEO\b|Phil[-_\s.]*Potter|Samson[-_\s.]*Mow|Gabor[-_\s.]*Gurbacs|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|Reeve[-_\s.]*Collins|phil(ip)?[-_\s.]*potter\b|Van[-_\s.]*der[-_\s.]*Velde|Perpetual[-_\s.]*Action[-_\s.]*Group|Global[-_\s.]*Trade[-_\s.]*Solutions|reginald[-_\s.]*fowler|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Blade[-_\s.]*payments|Five[-_\s.]*Delta|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|Mainstreet[-_\s.]*Partners|Far[-_\s.]*Eastern[-_\s.]*International|White[-_\s.]*Plains[-_\s.]*Capital|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS
+Tether,\b(BFXNA|BFXWW|Chesham|Coinapult|D10e|Devasini|Eqonex|GoCoin|Evertune|Friedberg|GamesTV|Hoegner|Huashun|IGEL|Infomatec|Ludovicus|(Master|Real)coin|Mallers|Noblex|Paolo(Ardoino)?|Playsino|Renrenbee|SFP|Sinopec|SJMBT|Stablehouse|Sunlot|Tether|Tuxia|urwhatyouknow|USDT|XBTO|Xfire|Yantis)\b|Noble[-_\s.]*Bank|\bDeltec[^\']|\b(B[ei]t|i|Digi?|Eth)f?inex[^e']|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|[$#]LEO\b|Phil[-_\s.]*Potter|Samson[-_\s.]*Mow|Gabor[-_\s.]*Gurbacs|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|Reeve[-_\s.]*Collins|phil(ip)?[-_\s.]*potter\b|Van[-_\s.]*der[-_\s.]*Velde|Perpetual[-_\s.]*Action[-_\s.]*Group|Global[-_\s.]*Trade[-_\s.]*Solutions|reginald[-_\s.]*fowler|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Blade[-_\s.]*payments|Five[-_\s.]*Delta|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|Mainstreet[-_\s.]*Partners|Far[-_\s.]*Eastern[-_\s.]*International|White[-_\s.]*Plains[-_\s.]*Capital|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS|Tackett
 Tornado Cash,tornado[-_\s.]*cash
 Transactive Systems UAB,Transactive[-_\s.]*Systems
 Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
-TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
+TrueUSD,\b(TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx|Jaiyong|TrustLabs)\b
 Vauld,Vauld
 VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
 Voyager,Voyager\b
 Wanxiang Group,wanxiang|\bFeng[-_\s.]*Xiao
 Wallet Addresses BCH,bitcoincash:q.*\b
 Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39}\b
@@ -163,12 +165,12 @@
 Wallet Addresses Dash,\bX[1-9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\bD[a-zA-Z0-9_.-]{33}
 Wallet Addresses Ethereum,0x[a-fA-F0-9]{40}
 Wallet Addresses Monero,\b[48][0-9AB][1-9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,\b1[0-9a-zA-Z]{47}
 Wallet Addresses Ripple,\br[0-9a-zA-Z]{33}
 Wallet Addresses Stellar,\bG[0-9A-Z]{40,60}\b
-Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s.]*ivanov|boris[-_\s.]*titov|[$#]waves\b
+Waves,sasha[-_\s.]*(35625|ivanov|\.waves)|\bVires\b|boris[-_\s.]*titov|[$#]WAVES\b|USDN
 Wintermute,Wintermute|\b(Bebop|Evgeny)\b
 Wirecard,\b(Bafin|Marsalek|Wirecard)\b|Markus[-_\s.]*Braun
 Worldcoin,Worldcoin|\borb\b
 Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b|Steven[-_\s.]*Huynh
```

### Comparing `clown_sort-1.9.0/clown_sort/util/argument_parser.py` & `clown_sort-1.9.1/clown_sort/util/argument_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,7 +84,11 @@
     formatter_class=RichHelpFormatterPlus,
     description="Extract the text from one or more files or directories.",
     epilog="If any of the FILE_OR_DIRs is a directory all files in that directory will be extracted."
 )
 
 extraction_parser.add_argument('file_or_dir', nargs='+', metavar='FILE_OR_DIR')
 extraction_parser.add_argument('--debug', action='store_true', help='turn on debug level logging')
+
+extraction_parser.add_argument('--print-when-parsed', '-p',
+                                action='store_true',
+                                help='print pages as they are parsed instead of waiting until document is fully parsed')
```

### Comparing `clown_sort-1.9.0/clown_sort/util/constants.py` & `clown_sort-1.9.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.9.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/clown_sort/util/rich_helper.py` & `clown_sort-1.9.1/clown_sort/util/rich_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from sys import stderr
 from typing import List, Optional, Union
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.text import Text
 from rich.theme import Theme
 
@@ -43,14 +44,15 @@
 }
 
 COLOR_THEME = Theme(COLOR_THEME_DICT)
 INDENT_SPACES = 4
 
 # Main rich text output object.
 console = Console(theme=COLOR_THEME, color_system='256')
+stderr_console = Console(theme=COLOR_THEME, color_system='256', file=stderr)
 
 
 def indented_bullet(msg: Union[str, Text], style: Optional[str] = None) -> Text:
     return Text('  ') + bullet_text(msg, style)
 
 
 def bullet_text(msg: Union[str, Text], style: Optional[str] = None) -> Text:
```

### Comparing `clown_sort-1.9.0/clown_sort/util/string_helper.py` & `clown_sort-1.9.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.9.0/pyproject.toml` & `clown_sort-1.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.9.0"
+version = "1.9.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -33,22 +33,22 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 exif = "^1.5.0"
 PySimpleGUI = {version = "^4.60.4", optional = true}
 pytesseract = "^0.3.10"
 rich = "^13.0.1"
 piexif = "^1.1.3"
-pillow = "^9.4.0"
+pillow = "^9.5.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
-pyexiftool = "^0.5.5"
-pypdf = "^3.8.0"
 pycryptodome = {version = "^3.17", optional = true}
+pyexiftool = "^0.5.5"
 PyMuPDF = {version = "^1.22.3", optional = true}
+pypdf = "^3.12.0"
 
 [tool.poetry.extras]
 pdf = ['pycryptodome', 'PyMuPDF']
 gui = ['PySimpleGUI']
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
```

### Comparing `clown_sort-1.9.0/PKG-INFO` & `clown_sort-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.9.0
+Version: 1.9.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,18 @@
 Provides-Extra: gui
 Provides-Extra: pdf
 Requires-Dist: PyMuPDF (>=1.22.3,<2.0.0) ; extra == "pdf"
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
-Requires-Dist: pypdf (>=3.8.0,<4.0.0)
+Requires-Dist: pypdf (>=3.12.0,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
 
 ![Python Version](https://img.shields.io/pypi/pyversions/clown_sort)
```

