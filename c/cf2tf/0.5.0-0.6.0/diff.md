# Comparing `tmp/cf2tf-0.5.0.tar.gz` & `tmp/cf2tf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.5.0.tar", max compression
+gzip compressed data, was "cf2tf-0.6.0.tar", max compression
```

## Comparing `cf2tf-0.5.0.tar` & `cf2tf-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-03-23 23:06:21.406725 cf2tf-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     7382 2023-03-23 23:06:21.406725 cf2tf-0.5.0/README.md
--rw-r--r--   0        0        0     1145 2023-03-23 23:06:33.502714 cf2tf-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1419 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2605 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    31091 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     1543 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    19587 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2629 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2200 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3653 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     2610 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2170 2023-03-23 23:06:21.410725 cf2tf-0.5.0/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8524 1970-01-01 00:00:00.000000 cf2tf-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 21:10:05.191587 cf2tf-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     7382 2023-07-09 21:10:05.191587 cf2tf-0.6.0/README.md
+-rw-r--r--   0        0        0     1087 2023-07-09 21:10:19.743600 cf2tf-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:10:05.191587 cf2tf-0.6.0/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2605 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    31201 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    20221 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2629 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2200 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     3995 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     2865 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2171 2023-07-09 21:10:05.195587 cf2tf-0.6.0/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 cf2tf-0.6.0/PKG-INFO
```

### Comparing `cf2tf-0.5.0/LICENSE.txt` & `cf2tf-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/README.md` & `cf2tf-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/pyproject.toml` & `cf2tf-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.5.0"
+version = "0.6.0"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
 
 [tool.poetry.scripts]
 cf2tf = "cf2tf.app:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 cfn-flip = "^1.3.0"
 PyYAML = "^6.0"
 click = "^8.1.2"
 GitPython = "^3.1.27"
 thefuzz = {extras = ["speedup"], version = "^0.19.0"}
 click-log = "^0.4.0"
 requests = "^2.27.1"
 pytest = "^7.1.2"
 
 [tool.poetry.dev-dependencies]
 black = "^23.0.0"
-flake8 = "^5.0.4"
+flake8 = "^6.0.0"
 flake8-black = "^0.3.3"
 coverage = {extras = ["toml"], version = "^7.0.0"}
 pytest-cov = "^4.0.0"
 mypy = "^1.1"
-typing-extensions = { version = "^4.3.0", python = "~3.7" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `cf2tf-0.5.0/src/cf2tf/app.py` & `cf2tf-0.6.0/src/cf2tf/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cf2tf.convert import TemplateConverter
 from cf2tf.terraform import code
 
 log = logging.getLogger("cf2tf")
 click_log.basic_config(log)
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.version_option()
 @click.option("--output", "-o", type=click.Path(exists=False))
 @click_log.simple_verbosity_option(log)
 @click.argument("template_path", type=click.Path(exists=True))
 def cli(output: Optional[str], template_path: str):
     """Convert Cloudformation template into Terraform.
 
@@ -44,8 +44,8 @@
     config = TemplateConverter(tmpl_path.stem, cf_template, search_manger).convert()
 
     # Save this configuration to disc
     config.save(output_writer)
 
 
 if __name__ == "__main__":
-    cli()
+    cli()  # type: ignore
```

### Comparing `cf2tf-0.5.0/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.6.0/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/conversion/expressions.py` & `cf2tf-0.6.0/src/cf2tf/conversion/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -756,15 +756,15 @@
         source_string = values[0]
         local_vars = values[1]
     else:
         raise TypeError(
             "Fn::Sub - The first value must be a String and the second a Map."
         )
 
-    def replace_var(m):
+    def replace_var(m) -> str:
         var: str = m.group(1)
 
         if var in local_vars:
             result = local_vars[var]
             return wrap_in_curlys(result)
 
         if "." in var:
@@ -824,18 +824,19 @@
         return LiteralType(f"var.{tf_name}")
 
     cf_resource = template.resource_lookup(var_name, ["Resources"])
 
     if cf_resource:
         cf_resource_type = cf_resource.get("Type", "")
         docs_path = template.search_manager.find(cf_resource_type)
-        _, valid_attributes = doc_file.parse_attributes(docs_path)
+        valid_arguments, valid_attributes = doc_file.parse_attributes(docs_path)
         tf_name = cf2tf.convert.pascal_to_snake(var_name)
         tf_type = cf2tf.convert.create_resource_type(docs_path)
-        first_attr = next(iter(valid_attributes))
+
+        first_attr = valid_attributes[0] if valid_attributes else valid_arguments[0]
         conditional = cf_resource.get("Condition")
 
         if conditional is not None:
             tf_name = f"{tf_name}[0]"
 
         return LiteralType(f"{tf_type}.{tf_name}.{first_attr}")
 
@@ -972,15 +973,19 @@
 }
 
 # Cloudformation only allows certain functions to be called from inside
 # other functions. The keys are the function name and the values are the
 # functions that are allowed to be nested inside it.
 ALLOWED_FUNCTIONS: Dict[str, Dispatch] = {
     "Fn::And": ALLOWED_NESTED_CONDITIONS,
-    "Fn::Equals": {**ALLOWED_NESTED_CONDITIONS, "Fn::Join": join},
+    "Fn::Equals": {
+        **ALLOWED_NESTED_CONDITIONS,
+        "Fn::Join": join,
+        "Fn::Select": select,
+    },
     "Fn::If": {
         "Fn::Base64": base64,
         "Fn::FindInMap": find_in_map,
         "Fn::GetAtt": get_att,
         "Fn::GetAZs": get_azs,
         "Fn::If": if_,
         "Fn::Join": join,
```

### Comparing `cf2tf-0.5.0/src/cf2tf/conversion/overrides.py` & `cf2tf-0.6.0/src/cf2tf/conversion/overrides.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import TYPE_CHECKING, Callable, Dict
 
 from cf2tf.terraform.hcl2.custom import LiteralType
 from cf2tf.terraform.hcl2.primitive import NullType, StringType, TerraformType
+from cf2tf.terraform.hcl2.complex import ListType, MapType
 
 if TYPE_CHECKING:
     from cf2tf.convert import TemplateConverter
 
 CFParams = Dict[str, TerraformType]
 
 Override = Callable[["TemplateConverter", CFParams], CFParams]
@@ -41,11 +42,27 @@
     policy_value = params["PolicyDocument"]
 
     params["PolicyDocument"] = LiteralType(f"jsonencode({policy_value.render(4)}\n  )")
 
     return params
 
 
+def tag_conversion(_tc: "TemplateConverter", params: CFParams) -> CFParams:
+    if isinstance(params["Tags"], dict):
+        return params
+
+    orginal_tags: ListType = params["Tags"]  # type: ignore
+
+    new_tags = {LiteralType(tag["Key"]): tag["Value"] for tag in orginal_tags}
+
+    del params["Tags"]
+    params["tags"] = MapType(new_tags)
+
+    return params
+
+
 OVERRIDE_DISPATCH: ResourceOverride = {
     "aws_s3_bucket": {"AccessControl": s3_bucket_acl},
     "aws_s3_bucket_policy": {"PolicyDocument": s3_bucket_policy},
 }
+
+GLOBAL_OVERRIDES: ParamOverride = {"Tags": tag_conversion}
```

### Comparing `cf2tf-0.5.0/src/cf2tf/convert.py` & `cf2tf-0.6.0/src/cf2tf/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type
 
 from thefuzz import process  # type: ignore
 
 import cf2tf.conversion.expressions as functions
 import cf2tf.terraform._configuration as config
 import cf2tf.terraform.doc_file as doc_file
-from cf2tf.conversion.overrides import OVERRIDE_DISPATCH
+from cf2tf.conversion.overrides import OVERRIDE_DISPATCH, GLOBAL_OVERRIDES
 from cf2tf.terraform.blocks import Block, Locals, Output, Resource, Variable
 from cf2tf.terraform.hcl2 import AllTypes
 from cf2tf.terraform.hcl2.complex import ListType, MapType
 from cf2tf.terraform.hcl2.custom import CommentType, LiteralType
 from cf2tf.terraform.hcl2.primitive import NumberType, StringType, TerraformType
 
 if TYPE_CHECKING:
@@ -136,15 +136,15 @@
 
             converter = get_converter(self, section)
 
             tf_resources.extend(converter(resources))
 
         return tf_resources
 
-    def resolve_values(
+    def resolve_values(  # noqa: max-complexity=13
         self,
         data: Any,
         allowed_func: functions.Dispatch,
         prev_func: Optional[str] = None,
         inside_function=False,
     ):
         """Recurses through a Cloudformation template. Solving all
@@ -177,15 +177,18 @@
                 if key not in allowed_func:
                     raise ValueError(f"{key} not allowed to be nested in {prev_func}.")
 
                 value = self.resolve_values(
                     value, functions.ALLOWED_FUNCTIONS[key], key, inside_function=True
                 )
 
-                return allowed_func[key](self, value)
+                try:
+                    return allowed_func[key](self, value)
+                except Exception:
+                    return CommentType(f"Unable to resolve {key} with value: {value}")
 
             return MapType(data)
         elif isinstance(data, list):
             resolved_list_values = [
                 self.resolve_values(
                     item, allowed_func, prev_func, inside_function=inside_function
                 )
@@ -319,14 +322,18 @@
 
                 log.debug("Overiding Properties")
 
                 overrided_values = perform_resource_overrides(
                     tf_type, resolved_values, self
                 )
 
+                overrided_values = perform_global_overrides(
+                    tf_type, overrided_values, self
+                )
+
                 log.debug("Converting property names to argument names...")
 
                 arguments = props_to_args(overrided_values, valid_arguments, docs_path)
 
                 log.debug(f"Converted properties to {arguments}")
 
             conditional = resource_values.get("Condition")
@@ -599,7 +606,19 @@
     param_overrides = OVERRIDE_DISPATCH[tf_type]
 
     for param, override in param_overrides.items():
         if param in params:
             params = override(tc, params)
 
     return params
+
+
+def perform_global_overrides(
+    tf_type: str, params: Dict[str, TerraformType], tc: TemplateConverter
+):
+    log.debug("Performing global overrides for {tf_type}")
+
+    for param, override in GLOBAL_OVERRIDES.items():
+        if param in params:
+            params = override(tc, params)
+
+    return params
```

### Comparing `cf2tf-0.5.0/src/cf2tf/save.py` & `cf2tf-0.6.0/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/blocks.py` & `cf2tf-0.6.0/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/code.py` & `cf2tf-0.6.0/src/cf2tf/terraform/code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import re
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Optional
+from shutil import rmtree
 
 import click
 from click._termui_impl import ProgressBar
 from git import RemoteProgress
-from git.repo.base import Repo
+from git.repo.base import Repo, InvalidGitRepositoryError
 from thefuzz import fuzz, process  # type: ignore
 
 import cf2tf.convert
 
 log = logging.getLogger("cf2tf")
 
 
@@ -30,15 +31,15 @@
             doc_file: transform_file_name(doc_file.name) for doc_file in self.resources
         }
 
         resource_name: str
         ranking: int
         doc_path: Path
         resource_name, ranking, doc_path = process.extractOne(
-            name.lower(), files, scorer=fuzz.UWRatio
+            name.lower(), files, scorer=fuzz.token_sort_ratio
         )
 
         log.debug(
             f"Best match was {resource_name} at {doc_path} with score of {ranking}."
         )
 
         return doc_path
@@ -53,40 +54,53 @@
 
     if not docs_path.exists():
         print("The docs path does not exist")
 
     return SearchManager(docs_path)
 
 
-def get_code():
+def get_code() -> Repo:
     temp_dir = Path(gettempdir())
     repo_path = temp_dir.joinpath("terraform_src")
 
-    if repo_path.exists():
-        if repo_path.joinpath(".git").exists():
-            # todo Need to check to make sure the remote is correct
-            click.echo(" existing repo found.")
-            repo = Repo(repo_path)
-            return repo
+    try:
+        existing_repo = repo_from_existing(repo_path)
+
+        if existing_repo:
+            return existing_repo
+
+    except InvalidGitRepositoryError:
+        rmtree(repo_path)
+        repo_path.rmdir()
 
     print(f"// Cloning Terraform src code to {repo_path}...", end="")
 
     repo_path.mkdir(exist_ok=True)
 
     repo = Repo.clone_from(
         "https://github.com/hashicorp/terraform-provider-aws.git",
         repo_path,
         depth=1,
-        progress=CloneProgress(),
+        progress=CloneProgress(),  # type: ignore
     )
     click.echo(" code has been checked out.")
 
     return repo
 
 
+def repo_from_existing(repo_path: Path) -> Optional[Repo]:
+    if repo_path.exists():
+        if repo_path.joinpath(".git").exists():
+            repo = Repo(repo_path)
+            click.echo(f"// Existing Terraform src code found at {repo_path}.")
+            return repo
+
+    return None
+
+
 def resource_type_to_name(resource_type: str) -> str:
     """Converts a Cloudformation Resource Type into something more search friendly.
 
     Args:
         resource_type (str): The Cloudformation resource type.
 
     Returns:
```

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.6.0/src/cf2tf/terraform/doc_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 import logging
 
 log = logging.getLogger("cf2tf")
 
 
 def parse_attributes(docs_path: Path):
     with open(docs_path) as file:
-        arguments = parse_section("Argument Reference", file)
-
-        attributes = parse_section("Attributes Reference", file)
+        try:
+            arguments = parse_section("Argument Reference", file)
+        except Exception as e:
+            raise Exception(f"Unable to find arguments in {file.name}") from e
+
+        try:
+            attributes = parse_section("Attributes Reference", file)
+        except Exception as e:
+            raise Exception(f"Unable to find attributes in {file.name}") from e
 
     return (arguments, attributes)
 
 
 def read_section(docs_path: Path, section_name: str):
     items: List[str]
     with open(docs_path) as file:
@@ -57,15 +63,15 @@
 
         # If line starts with whitespace its probably a multiline description
         if line.startswith((" ", "\t")):
             continue
 
         # These should be the attributes we are after
         if line[0] == "*":
-            regex = r"`([\w\.]+)`"
+            regex = r"`([\w.*]+)`"
 
             match = re.search(regex, line)
 
             if not match:
                 raise Exception(f"Did not find an item to parse in {line}")
 
             attribute = match.group(1)
```

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.5.0/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.6.0/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class TerraformType(Protocol):
     """A Terraform value of some type."""
 
     value: Any
 
     def __str__(self) -> str:
-        return self.render()
+        return self.render(0)
 
     @abstractclassmethod
     def render(self, indent: int) -> str:
         raise NotImplementedError
 
 
 class StringType(str, TerraformType):
```

### Comparing `cf2tf-0.5.0/PKG-INFO` & `cf2tf-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.5.0
+Version: 0.6.0
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cfn-flip (>=1.3.0,<2.0.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
```

#### html2text {}

```diff
@@ -1,26 +1,24 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.5.0 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.6.0 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
-Author-email: shadycuz@gmail.com Requires-Python: >=3.7,<4.0 Classifier:
+Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: GitPython (>=3.1.27,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-
-Dist: cfn-flip (>=1.3.0,<2.0.0) Requires-Dist: click (>=8.1.2,<9.0.0) Requires-
-Dist: click-log (>=0.4.0,<0.5.0) Requires-Dist: pytest (>=7.1.2,<8.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: thefuzz[speedup]
-(>=0.19.0,<0.20.0) Project-URL: Repository, https://github.com/DontShaveTheYak/
-cf2tf Description-Content-Type: text/markdown   [![Python][python-shield]]
-[pypi-url] [![Latest][version-shield]][pypi-url] [![Tests][test-shield]][test-
-url] [![Coverage][codecov-shield]][codecov-url] [![License][license-shield]]
-[license-url]
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: GitPython
+(>=3.1.27,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: cfn-flip
+(>=1.3.0,<2.0.0) Requires-Dist: click (>=8.1.2,<9.0.0) Requires-Dist: click-log
+(>=0.4.0,<0.5.0) Requires-Dist: pytest (>=7.1.2,<8.0.0) Requires-Dist: requests
+(>=2.27.1,<3.0.0) Requires-Dist: thefuzz[speedup] (>=0.19.0,<0.20.0) Project-
+URL: Repository, https://github.com/DontShaveTheYak/cf2tf Description-Content-
+Type: text/markdown   [![Python][python-shield]][pypi-url] [![Latest][version-
+shield]][pypi-url] [![Tests][test-shield]][test-url] [![Coverage][codecov-
+shield]][codecov-url] [![License][license-shield]][license-url]
                      **** Cloudformation 2 Terraform ****
              Convert your Cloudformation templates to Terraform.
                        Report_Bug Â· Request_Feature Â·
   Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
```

