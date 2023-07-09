# Comparing `tmp/contact_magic-0.5.1.tar.gz` & `tmp/contact_magic-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.1.tar", max compression
+gzip compressed data, was "contact_magic-0.5.2.tar", max compression
```

## Comparing `contact_magic-0.5.1.tar` & `contact_magic-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.1/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.1/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.1/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.1/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.5.1/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.1/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.5.1/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.1/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2499 2023-06-14 21:27:06.608482 contact_magic-0.5.1/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1678 2023-06-14 21:25:23.127407 contact_magic-0.5.1/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1638 2023-06-13 07:39:32.822031 contact_magic-0.5.1/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.1/contact_magic/logger.py
--rw-r--r--   0        0        0    13609 2023-06-14 21:27:07.154508 contact_magic-0.5.1/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.1/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.1/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.5.1/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.1/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.1/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.5.1/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.1/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-06-27 14:36:30.970027 contact_magic-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.2/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.2/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.2/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.2/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.5.2/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.2/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.2/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.2/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-08 20:52:26.946536 contact_magic-0.5.2/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.2/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.2/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.2/contact_magic/logger.py
+-rw-r--r--   0        0        0    15182 2023-07-08 21:41:34.642770 contact_magic-0.5.2/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.2/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.2/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.2/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.2/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.2/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.2/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.2/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.2/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.2/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-09 10:38:49.448262 contact_magic-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.2/PKG-INFO
```

### Comparing `contact_magic-0.5.1/README.md` & `contact_magic-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/asyncio.py` & `contact_magic-0.5.2/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/conf/settings.py` & `contact_magic-0.5.2/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/dict_utils.py` & `contact_magic-0.5.2/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/helpers.py` & `contact_magic-0.5.2/contact_magic/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,26 +48,34 @@
     for i in range(0, len(df_settings_data.columns), 2):
         scraper_col_values = list(df_settings_data.iloc[:, i].values)
         if not scraper_col_values:
             continue
         new_entry = {"col_name": df_settings_data.columns[i], "sentence_wizards": []}
         scrapers_seen = set()
         for position, scraper in enumerate(scraper_col_values):
-            if (
+            if SETTINGS.ALLOWED_SCRAPER_NAMES and (
                 scraper not in SETTINGS.ALLOWED_SCRAPER_NAMES
                 or scraper in scrapers_seen
             ):
                 continue
             premise_url = df_settings_data.iloc[position, i + 1]
             if pd.isnull(premise_url):
                 continue
             if scraper == "FALLBACK":
                 new_entry["sentence_wizards"].append(
                     {"scraper_name": scraper, "fallback_template": premise_url}
                 )
+            elif scraper == "USE_HISTORIC_DATA":
+                new_entry["sentence_wizards"].append(
+                    {
+                        "scraper_name": None,
+                        "premise_url": premise_url,
+                        "restrict_to_scraped_data": False,
+                    }
+                )
             else:
                 new_entry["sentence_wizards"].append(
                     {"scraper_name": scraper, "premise_url": premise_url}
                 )
             scrapers_seen.add(scraper)
         if new_entry.get("sentence_wizards"):
             settings.append(new_entry)
```

### Comparing `contact_magic-0.5.1/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.2/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.2/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/integrations/sheets.py` & `contact_magic-0.5.2/contact_magic/integrations/sheets.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,7 +50,11 @@
 
 def bulk_update(sheet, data):
     return retry_req(sheet.update, data)
 
 
 def update_cell(sheet, row, col, value):
     return retry_req(sheet.update_cell, row, col, value)
+
+
+def clear_sheet(sheet):
+    return retry_req(sheet.clear)
```

### Comparing `contact_magic-0.5.1/contact_magic/models.py` & `contact_magic-0.5.2/contact_magic/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,20 +79,30 @@
     field_processors: dict = Field(
         description="A list of fields to validate before "
         "doing Copyfactory request."
         "If any of the fields fail validation "
         "Copyfactory will not be called.",
         default={},
     )
+    restrict_to_scraped_data: bool = Field(
+        description="A boolean to indicate what data the "
+        "wizard is allowed to look at before calling Copyfactory."
+        " defaults to only looking at the latest scrape attempt. If set to False will "
+        "look at all scraped data on the row.",
+        default=True,
+    )
+    added_key_names: set = Field(
+        description="A list of keys that were added during the scraping.", default=set()
+    )
 
     @validator("premise_url")
     def validate_premise_url(cls, url):
         if not isinstance(url, str):
             return url
-        return f"{url}/" if not url.endswith("/") else url
+        return url if url.endswith("/") else f"{url}/"
 
     @validator("scraper_name")
     def validate_scraper_name(cls, value):
         if value is None:
             return value
         if not SETTINGS.ALLOWED_SCRAPER_NAMES:
             return value
@@ -111,18 +121,18 @@
         """
         Fills in the template with row data.
         either returns the filled in template or an empty string.
         """
         list_pot_keys = re.findall(r"\{(.*?)\}", self.fallback_template)
         copy_of_template = self.fallback_template
         for key in list_pot_keys:
-            value = get_values_in_object_by_key(row.data, key)
-            if not value:
+            if value := get_values_in_object_by_key(row.data, key):
+                copy_of_template = copy_of_template.replace("{" + key + "}", value[0])
+            else:
                 return ""
-            copy_of_template = copy_of_template.replace("{" + key + "}", value[0])
         return copy_of_template
 
     async def run_sales_scraper(self, row: DataRow, col_prefix: str, overwrite=False):
         """
         Runs the scraping and extends the row by adding
         the column name + scraper as a prefix to ensure uniqueness.
         """
@@ -141,25 +151,31 @@
                 if key in row.data and not overwrite:
                     continue
                 # Remove output schema since don't want
                 # to pass schema values to Copyfactory
                 value = delete_key_in_object(value, "output_schema")
                 unique_key = f"{col_prefix}__{self.scraper_name}__{key}"
                 row.data[unique_key] = value
+                self.added_key_names.add(unique_key)
             return row
         return row
 
     async def run_copyfactory(
-        self, row: DataRow, content_col_name: str, source_col_name: str
+        self,
+        row: DataRow,
+        content_col_name: str,
+        source_col_name: str,
+        keys_to_delete: set = None,
     ):
         """
         Runs Copyfactory using the current row Data.
         If successfully called with Copyfactory returns True to stop iteration
         for that datapoint.
         """
+        keys_to_delete = keys_to_delete or set()
         if not self.premise_url and not self.premise_id:
             return row, False
         if self.premise_url and self.is_premise_url_valid:
             self.premise_id = get_id_from_url(self.premise_url)
         if not self.copyfactory_mapping and SETTINGS.COPYFACTORY_MAPPING:
             self.copyfactory_mapping = SETTINGS.COPYFACTORY_MAPPING
 
@@ -168,14 +184,23 @@
             return row, False
 
         data = (
             replace_keys_in_object(row.data, self.copyfactory_mapping)
             if self.copyfactory_mapping
             else row.data
         )
+        # Remove all other scraped data keys
+        # from the row from consideration in the event of
+        # multiple keys from scraped data having
+        # the same name to restrict the passed data to being from
+        # this sentence wizard scrape.
+        if self.restrict_to_scraped_data:
+            for key in keys_to_delete:
+                data = delete_key_in_object(data, key)
+
         if cf := await make_copyfactory_request(self.premise_id, variables=data):
             row.data[content_col_name] = cf["content"]
             source = row.data.get(
                 f"{content_col_name}__{self.scraper_name}__scraper_info", {}
             ).get("data_source", "-")
             row.data[source_col_name] = f"{self.scraper_name}, {source}"
             return row, True
@@ -208,69 +233,81 @@
                     except Exception:
                         is_value_valid = False
                     if not is_value_valid:
                         return row, False
         return row, True
 
     async def execute(
-        self, row: DataRow, content_col_name: str, source_col_name: str
+        self,
+        row: DataRow,
+        content_col_name: str,
+        source_col_name: str,
+        keys_to_delete: set = None,
     ) -> tuple[DataRow, bool]:
         """
         Executes the scraper and extends the DataRow as it moves along to
         allow for exploding the DF with more
         datapoints from the scraping + personalization.
         """
+        keys_to_delete = keys_to_delete or set()
         if self.scraper_name == "FALLBACK" and self.fallback_template:
             row.data[content_col_name] = self.fill_fallback(row)
             row.data[source_col_name] = "-"
             return row, row.data[content_col_name] != ""
         row = await self.run_sales_scraper(row, col_prefix=content_col_name)
         row, success = await self.run_copyfactory(
-            row, content_col_name, source_col_name
+            row, content_col_name, source_col_name, keys_to_delete=keys_to_delete
         )
         return row, success
 
     def __init__(self, **data: Any):
         if data.get("scraper_name", None):
             if default_options := SETTINGS.SENTENCE_WIZARD_OPTIONS.get(
                 data.get("scraper_name"), None
             ):
-                data = data | default_options
+                data |= default_options
         super().__init__(**data)
 
 
 class DataPoint(BaseModel):
     """
     A reference to a datapoint to create for a given contact
     targeting a column and a list of allowed scrapers.
     """
 
     col_name: str = Field(
         description="The column name you want for the datapoint.",
         example="Personalization1",
     )
     sentence_wizards: list[SentenceWizard]
+    keys_added: set = set()
 
     @property
     def get_col_name_as_source(self) -> str:
         return f"source__{self.col_name}"
 
-    async def build_datapoint(self, row: DataRow):
+    async def build_datapoint(self, row: DataRow, keys_to_delete: set = None):
+        keys_to_delete = keys_to_delete or set()
         for scraper in self.sentence_wizards:
             logger.info(
                 "processing_row",
                 row_number=row.index,
                 scraper_name=scraper.scraper_name,
                 premise_id=scraper.premise_id or get_id_from_url(scraper.premise_url),
                 column_name=self.col_name,
                 status="STARTING",
             )
             row, did_succeed = await scraper.execute(
-                row, self.col_name, self.get_col_name_as_source
+                row,
+                self.col_name,
+                self.get_col_name_as_source,
+                keys_to_delete=keys_to_delete,
             )
+            for key in scraper.added_key_names:
+                self.keys_added.add(key)
             if did_succeed:
                 logger.info(
                     "processing_row",
                     row_number=row.index,
                     scraper_name=scraper.scraper_name,
                     premise_id=scraper.premise_id
                     or get_id_from_url(scraper.premise_url),
@@ -372,10 +409,13 @@
 
     async def build_row(self, row: DataRow):
         """
         Iterate over all personalization datapoints and their
         allowed scrapers to extend a row of contact data
         with enrichment and personalized sentences.
         """
+        keys_to_delete = set()
         for datapoint in self.datapoints:
-            row = await datapoint.build_datapoint(row)
+            row = await datapoint.build_datapoint(row, keys_to_delete=keys_to_delete)
+            for key in datapoint.keys_added:
+                keys_to_delete.add(key)
         return row
```

### Comparing `contact_magic-0.5.1/contact_magic/preprocessors.py` & `contact_magic-0.5.2/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/scripts/agency.py` & `contact_magic-0.5.2/contact_magic/scripts/agency.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 from typing import List
 
 import typer
 from rich import print
 from typing_extensions import Annotated
 
 from contact_magic.scripts.run_workflows import run_sheets
+from contact_magic.scripts.sync_scraper_options_to_workersheets import (
+    sync_scraper_options,
+)
 from contact_magic.scripts.update_workflow_approval_metrics import (
     update_rows_approved_and_remaining,
 )
 
 app = typer.Typer()
 
 
 class ScriptOptions(Enum):
     run_sheets = "run_sheets"
     update_approved = "update_approved"
+    sync_scraper_options = "sync_scraper_options"
 
 
 @app.command()
 def pipeline(
     task: List[ScriptOptions] = None,
     run_all: Annotated[bool, typer.Option("--run-all")] = False,
     times_to_run: Annotated[int, typer.Option(min=1)] = 1,
@@ -37,14 +41,15 @@
     To run all of the scripts
 
     Ex: "python agency.py --run-all"
     """
     commands = {
         "run_sheets": run_sheets,
         "update_approved": update_rows_approved_and_remaining,
+        "sync_scraper_options": sync_scraper_options,
     }
     tasks = task or []
     for _ in range(times_to_run):
         if run_all:
             for name, command in commands.items():
                 print(f":robot_face: [green]Running[/green] {name}")
                 command()
```

### Comparing `contact_magic-0.5.1/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.2/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.2/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,18 @@
                 status="STARTING",
             )
             data = worksheet_to_dataframe(
                 get_spreadsheet_by_url(row["WorkflowUrl"]), "WorkingSheet"
             )
             total_rows = len(data.dropna(subset=["Website"]))
             total_approved_data = len(data.loc[data["is_approved"] == "TRUE"])
-            approved_percentage = round(total_approved_data / total_rows, 2)
+            if total_rows > 0:
+                approved_percentage = round(total_approved_data / total_rows, 2)
+            else:
+                approved_percentage = 0
             base = 5
             for num, metric in enumerate(
                 [total_rows, total_approved_data, approved_percentage], 1
             ):
                 cell = workflows_sheet.cell(row=i + 2, col=base + num)
                 cell.value = metric
                 update_cell(workflows_sheet, cell.row, cell.col, cell.value)
```

### Comparing `contact_magic-0.5.1/contact_magic/utils.py` & `contact_magic-0.5.2/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.1/pyproject.toml` & `contact_magic-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.1"
+version = "0.5.2"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.1/PKG-INFO` & `contact_magic-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.1
+Version: 0.5.2
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

