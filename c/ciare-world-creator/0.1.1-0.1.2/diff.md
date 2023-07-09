# Comparing `tmp/ciare-world-creator-0.1.1.tar.gz` & `tmp/ciare-world-creator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciare-world-creator-0.1.1.tar", max compression
+gzip compressed data, was "ciare-world-creator-0.1.2.tar", max compression
```

## Comparing `ciare-world-creator-0.1.1.tar` & `ciare-world-creator-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11277 2023-07-05 22:17:52.097926 ciare-world-creator-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     6127 2023-07-06 22:05:39.671482 ciare-world-creator-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-05 22:17:52.433934 ciare-world-creator-0.1.1/ciare_world_creator/cli.py
--rw-r--r--   0        0        0     2390 2023-07-05 22:17:52.405933 ciare-world-creator-0.1.1/ciare_world_creator/collections/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/commands/__init__.py
--rw-r--r--   0        0        0     6791 2023-07-06 22:05:41.727349 ciare-world-creator-0.1.1/ciare_world_creator/commands/create.py
--rw-r--r--   0        0        0     2104 2023-07-05 22:17:52.245930 ciare-world-creator-0.1.1/ciare_world_creator/commands/fix.py
--rw-r--r--   0        0        0     1577 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/commands/list.py
--rw-r--r--   0        0        0      812 2023-07-05 22:17:52.429934 ciare-world-creator-0.1.1/ciare_world_creator/commands/purge.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/__init__.py
--rw-r--r--   0        0        0     4186 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/edit.py
--rw-r--r--   0        0        0     1295 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/model.py
--rw-r--r--   0        0        0     2397 2023-07-06 20:53:17.176457 ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/place.py
--rw-r--r--   0        0        0      837 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/world.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/llm/__init__.py
--rw-r--r--   0        0        0     2406 2023-07-06 21:28:00.517823 ciare-world-creator-0.1.1/ciare_world_creator/llm/model.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/model_databases/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/model_databases/fetch_models.py
--rw-r--r--   0        0        0     3618 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/model_databases/fetch_worlds.py
--rw-r--r--   0        0        0     1355 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/model_databases/gazebo.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/utils/__init__.py
--rw-r--r--   0        0        0     1358 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/utils/cache.py
--rw-r--r--   0        0        0      493 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/utils/json.py
--rw-r--r--   0        0        0      523 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.1/ciare_world_creator/utils/style.py
--rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.1/ciare_world_creator/xml/__init__.py
--rw-r--r--   0        0        0     1460 2023-07-05 22:17:52.177928 ciare-world-creator-0.1.1/ciare_world_creator/xml/empty_world.py
--rw-r--r--   0        0        0     1714 2023-07-05 22:17:52.425934 ciare-world-creator-0.1.1/ciare_world_creator/xml/worlds.py
--rw-r--r--   0        0        0      880 2023-07-06 22:05:41.727349 ciare-world-creator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7558 2023-07-06 22:05:45.962978 ciare-world-creator-0.1.1/setup.py
--rw-r--r--   0        0        0     7012 2023-07-06 22:05:45.963382 ciare-world-creator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11277 2023-07-05 22:17:52.097926 ciare-world-creator-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     6639 2023-07-09 11:05:53.438271 ciare-world-creator-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-05 22:17:52.433934 ciare-world-creator-0.1.2/ciare_world_creator/cli.py
+-rw-r--r--   0        0        0     2390 2023-07-07 21:07:46.256297 ciare-world-creator-0.1.2/ciare_world_creator/collections/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/commands/__init__.py
+-rw-r--r--   0        0        0     7511 2023-07-09 11:53:50.275788 ciare-world-creator-0.1.2/ciare_world_creator/commands/create.py
+-rw-r--r--   0        0        0     2104 2023-07-05 22:17:52.245930 ciare-world-creator-0.1.2/ciare_world_creator/commands/fix.py
+-rw-r--r--   0        0        0     1577 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/commands/list.py
+-rw-r--r--   0        0        0      812 2023-07-05 22:17:52.429934 ciare-world-creator-0.1.2/ciare_world_creator/commands/purge.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/__init__.py
+-rw-r--r--   0        0        0     4186 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/edit.py
+-rw-r--r--   0        0        0     1295 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/model.py
+-rw-r--r--   0        0        0     2397 2023-07-06 20:53:17.176457 ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/place.py
+-rw-r--r--   0        0        0      837 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/world.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/llm/__init__.py
+-rw-r--r--   0        0        0     2427 2023-07-07 22:27:11.300116 ciare-world-creator-0.1.2/ciare_world_creator/llm/model.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/model_databases/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/model_databases/fetch_models.py
+-rw-r--r--   0        0        0     3618 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/model_databases/fetch_worlds.py
+-rw-r--r--   0        0        0     1355 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/model_databases/gazebo.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/utils/__init__.py
+-rw-r--r--   0        0        0     1358 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/utils/cache.py
+-rw-r--r--   0        0        0      493 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/utils/json.py
+-rw-r--r--   0        0        0      523 2023-07-05 22:17:52.193928 ciare-world-creator-0.1.2/ciare_world_creator/utils/style.py
+-rw-r--r--   0        0        0        0 2023-07-05 22:17:52.169928 ciare-world-creator-0.1.2/ciare_world_creator/xml/__init__.py
+-rw-r--r--   0        0        0     1460 2023-07-05 22:17:52.177928 ciare-world-creator-0.1.2/ciare_world_creator/xml/empty_world.py
+-rw-r--r--   0        0        0     1714 2023-07-05 22:17:52.425934 ciare-world-creator-0.1.2/ciare_world_creator/xml/worlds.py
+-rw-r--r--   0        0        0      902 2023-07-09 18:26:13.370937 ciare-world-creator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8112 2023-07-09 18:26:16.655637 ciare-world-creator-0.1.2/setup.py
+-rw-r--r--   0        0        0     7567 2023-07-09 18:26:16.655938 ciare-world-creator-0.1.2/PKG-INFO
```

### Comparing `ciare-world-creator-0.1.1/LICENSE.md` & `ciare-world-creator-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/README.md` & `ciare-world-creator-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 <p align="center">
   <img width="800" src="https://cdn.jsdelivr.net/gh/ciare-robotics/world-creator@latest/docs/media/demo.svg">
 </p>
 
 # Features
 
+## Models
+
+Currently it uses gpt-3.5-16k by default, but if you have access to gpt-4, you will be prompted with a selection. Note that gpt-4 performs much better, but not everyone has the invitation from OpenAI to use it.
+
 ## Current limitations
 
 Currently it's Proof Of Concept solution. There will be a lot of future development. Right now it really does often hallucinate and it's spatial notion is not that great, but sometimes it generates something cool.
 
 Also complex models(like robots) currently is impossible to include. Work will be done on that in the future. Also complex textures of the models are not properly loading too.
 
 ## Integration with other simulators
@@ -38,27 +42,36 @@
 
 # Examples
 
 | Prompt  | Generated world |
 | ------------- | ------------- |
 | Healthcare worker and couple of medical items around them  | ![alt text](./docs/examples/medical.png)  |
 | Pile of fruits and other food in empty world | ![alt text](./docs/examples/pile.png)  |
-
+| Surgical room | ![alt text](./docs/examples/surgical_room.png) |
+| Warehouse shelves | ![alt text](./docs/examples/warehouse_shelves.png) |
+| Usual persons living room| ![alt text](./docs/examples/living_room.png) |
 
 
 # Getting Started
 
-## Installation(Using poetry)
+## Installation
 
+### From source using poetry
 ```
 git clone https://github.com/ciare-robotics/world-creator.git
 cd world-creator
 poetry install
 ```
 
+### Using pip
+```
+pip3 install ciare-world-creator
+```
+
+
 ## Token configuration
 
 Once you installed ciare, you need to save your OpenAI token by launching `ciare_world_creator create` command first time.
 
 ## OpenAI API usage
 
 I estimate that creating single world is only a matter of a few cents.
```

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/cli.py` & `ciare-world-creator-0.1.2/ciare_world_creator/cli.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/collections/utils.py` & `ciare-world-creator-0.1.2/ciare_world_creator/collections/utils.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/commands/create.py` & `ciare-world-creator-0.1.2/ciare_world_creator/commands/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "create",
     short_help="Create new simulation world",
 )
 @pass_context
 def cli(ctx):
     cache = Cache()
     db = TinyDB(os.path.join(cache.worlds_path, "world_db.json"))
-    
+
     from ciare_world_creator.llm.model import prompt_model
 
     # Only gazebo is supported
     loader = GazeboLoader()
     full_models = loader.get_models_full()
     full_worlds = loader.get_worlds_full()
 
@@ -53,14 +53,33 @@
 
     query = world_query.lower()
     query = query.replace("\n", "")
 
     World = Query()
     exists = db.search(World.prompt == query)
 
+    openai.api_key = os.getenv("OPENAI_API_KEY")
+    models = openai.Model.list()
+    allowed_models = ["gpt-3.5-turbo-16k"]
+    for model in models["data"]:
+        if model["id"] == "gpt-4":
+            allowed_models.append("gpt-4")
+
+    if len(allowed_models) > 1:
+        chosen_model = questionary.select(
+            message=(
+                "Choose model to generate with. GPT-4 is much better,"
+                " but also little-bit more expensive"
+            ),
+            choices=allowed_models,
+            style=STYLE,
+        ).ask()
+    else:
+        chosen_model = allowed_models[0]
+
     if exists:
         questionary.print(
             f"World already exists at {exists[0]['filepath']}... 🦄",
             style="bold italic fg:green",
         )
         return
 
@@ -69,39 +88,42 @@
         claim_query_result = model_collection.query(
             query_texts=[query],
             include=["documents", "distances", "metadatas"],
             n_results=100,
         )
     except openai.error.AuthenticationError:
         questionary.print(
-            f"OpenAI api key at {cache.cache_path}/openai_api_key incorrect. Regenerate it at https://platform.openai.com/account/api-keys at copy to {cache.cache_path}/openai_api_key",
+            f"OpenAI api key at {cache.cache_path}/openai_api_key incorrect. "
+            "Regenerate it at https://platform.openai.com/account/api-keys at copy "
+            f"to {cache.cache_path}/openai_api_key",
             style="bold italic fg:red",
         )
         sys.exit(os.EX_DATAERR)
 
     context = [
         {"name": name, "metadata": metadata}
         for name, metadata in zip(
             claim_query_result["documents"][0], claim_query_result["metadatas"][0]
         )
     ]
 
     generate_world = questionary.confirm(
-        "Do you want to also ask model to download pre-existing world?"
-        "Saying no will spawn models in empty world, it's more stable and predictable. Y/n",
+        "Do you want to spawn model in an empty world?"
+        " Saying no will download world from database, but it's very unstable. Y/n",
         style=STYLE,
     ).ask()
+
     if generate_world is None:
         sys.exit(os.EX_OK)
 
-    if generate_world:
+    if not generate_world:
         content = fmt_world_qa_tmpl.format(context_str=worlds)
 
         questionary.print("Generating world... 🌎", style="bold fg:yellow")
-        world = prompt_model(content, query)
+        world = prompt_model(content, query, chosen_model)
 
         questionary.print(
             f"World is {world['World']}, downloading it", style="bold italic fg:green"
         )
 
         full_world = find_world(world["World"], full_worlds)
         template_world_path = None
@@ -127,63 +149,66 @@
         )
         template_world_path = os.path.join(cache.worlds_path, "empty.sdf")
 
     questionary.print(
         "Spawning models in the world... 🫖", style="bold italic fg:yellow"
     )
     content = fmt_model_qa_tmpl.format(context_str=context)
-    models = prompt_model(content, query)
+    models = prompt_model(content, query, chosen_model)
 
     for model in models:
         if not find_model(model["Model"], full_models):
             models = prompt_model(
                 content,
-                f"{model} was not found in context list. Generate only the one that are in the context",
+                f"{model} was not found in context list. "
+                "Generate only the one that are in the context",
+                chosen_model,
             )
 
     questionary.print("Placing models in the world... 📍", style="bold italic fg:yellow")
     content = fmt_place_qa_tmpl.format(
         context_str=f"Arrange following models: {str(models)}",
         world_file=open(template_world_path, "r"),
     )
 
-    placement = prompt_model(content, query)
+    placement = prompt_model(content, query, chosen_model)
 
     # TODO handle ,.; etc
     cleaned_query = re.sub(r'[<>:;.,"/\\|?*]', "", query).strip()
     world_name = f'world_{cleaned_query.replace(" ", "_")}'
 
-    x, y = 0, 0
     include_elements = []
     i = 0
 
     # TODO add asserts on model fields
     non_existent_models = []
 
     for model in placement:
         # Example usage
         m = find_model(model["Model"], full_models)
         if not m:
             questionary.print(
-                f"Model {model} was not found in database. LLM hallucinated and made that up, skipping this model...",
+                f"Model {model} was not found in database. "
+                "LLM hallucinated and made that up, skipping this model...",
                 style="bold italic fg:red",
             )
             non_existent_models.append(model)
             i = i + 1
             continue
 
         include = add_model_to_xml(
             m["name"] + str(i),
             model["Pose"]["x"],
             model["Pose"]["y"],
             model["Pose"]["z"],
             0,
             0,
             0,
-            f"https://fuel.gazebosim.org/1.0/{m['owner']}/models/{m['name'].replace(' ', '%20')}",
+            "https://fuel.gazebosim.org/1.0/"
+            f"{m['owner']}/models/{m['name'].replace(' ', '%20')}",
         )
         include_elements.append(include)
         i = i + 1
 
     filtered_models = []
     for model in placement:
         if model not in non_existent_models:
```

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/commands/fix.py` & `ciare-world-creator-0.1.2/ciare_world_creator/commands/fix.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/commands/list.py` & `ciare-world-creator-0.1.2/ciare_world_creator/commands/list.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/commands/purge.py` & `ciare-world-creator-0.1.2/ciare_world_creator/commands/purge.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/edit.py` & `ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/edit.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/model.py` & `ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/model.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/place.py` & `ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/place.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/contexts_prompts/world.py` & `ciare-world-creator-0.1.2/ciare_world_creator/contexts_prompts/world.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/llm/model.py` & `ciare-world-creator-0.1.2/ciare_world_creator/llm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
                 text=chat_result.generations[0].message.content,
                 generation_info=chat_result.llm_output,
             )
             langchain.llm_cache.update(messages_prompt, self.model_name, [result])
         return chat_result
 
 
-def prompt_model(context: str, prompt: str):
+def prompt_model(context: str, prompt: str, model: str = "gpt-3.5-turbo-16k"):
     llm = CachedChatOpenAI(
-        model="gpt-3.5-turbo-16k", temperature=0, max_retries=0, request_timeout=59
+        model=model, temperature=0, max_retries=0, request_timeout=120
     )
     messages = [SystemMessage(content=context), HumanMessage(content=prompt)]
     try:
         ans = llm(messages)
     except openai.error.Timeout:
         print(
             "Timeout while waiting for model response."
```

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/model_databases/fetch_models.py` & `ciare-world-creator-0.1.2/ciare_world_creator/model_databases/fetch_models.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/model_databases/fetch_worlds.py` & `ciare-world-creator-0.1.2/ciare_world_creator/model_databases/fetch_worlds.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/model_databases/gazebo.py` & `ciare-world-creator-0.1.2/ciare_world_creator/model_databases/gazebo.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/utils/cache.py` & `ciare-world-creator-0.1.2/ciare_world_creator/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/utils/style.py` & `ciare-world-creator-0.1.2/ciare_world_creator/utils/style.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/xml/empty_world.py` & `ciare-world-creator-0.1.2/ciare_world_creator/xml/empty_world.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/ciare_world_creator/xml/worlds.py` & `ciare-world-creator-0.1.2/ciare_world_creator/xml/worlds.py`

 * *Files identical despite different names*

### Comparing `ciare-world-creator-0.1.1/pyproject.toml` & `ciare-world-creator-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciare-world-creator"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Alex Karavaev <alexkaravaev@alexkaravaev.xyz>"]
 readme = "README.md"
 packages = [{include = "ciare_world_creator"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
@@ -17,14 +17,15 @@
 click = "^8.1.3"
 tinydb = "^4.8.0"
 langchain = "^0.0.222"
 asyncio = "^3.4.3"
 aiohttp = "^3.8.4"
 tabulate = "^0.9.0"
 lark = "^1.1.5"
+pre-commit = "^3.3.3"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 pytest = "*"
 
 [tool.black]
```

### Comparing `ciare-world-creator-0.1.1/setup.py` & `ciare-world-creator-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,28 @@
  'chromadb>=0.3.26,<0.4.0',
  'click>=8.1.3,<9.0.0',
  'langchain>=0.0.222,<0.0.223',
  'lark>=1.1.5,<2.0.0',
  'lxml>=4.9.2,<5.0.0',
  'openai>=0.27.8,<0.28.0',
  'pandas>=2.0.3,<3.0.0',
+ 'pre-commit>=3.3.3,<4.0.0',
  'questionary>=1.10.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'tinydb>=4.8.0,<5.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['ciare_world_creator = ciare_world_creator.cli:cli']}
 
 setup_kwargs = {
     'name': 'ciare-world-creator',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
-    'long_description': '\n[![Ciare World Creator](/docs/media/logo.png)](https://ciare.dev)\n\n[![GitHub open issues](https://img.shields.io/github/issues-raw/ciare-robotics/world-creator.svg)](https://github.com/ciare/world-creator/issues)\n[![GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/ciare-robotics/world-creator.svg)](https://github.com/ciare/world-creator/pulls)\n[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nCiare World Creator is a CLI tool that reimagines the creation of simulation worlds for robotics. We have a vision that in the future you will not be obliged to painstakingly craft detailed SDF files. With Ciare, you will be able to effortlessly generate dynamic and realistic simulation environments by simply providing input text. Whether you\'re testing robot navigation or experimenting with new solutions, Ciare intelligently spawns models, freeing you from the complexities of precise object placement. By harnessing the power of Language Models (LLMs), Ciare empowers developers to rapidly prototype and explore their ideas, simplifying the simulation process and unlocking a world of possibilities for innovation.\n\nImagine a scenario where you want to test the navigation capabilities of a robot. With Ciare World Creator, you no longer have to spend hours meticulously positioning every object in the simulation. Instead, you simply provide input text to the Ciare pipeline, and it takes care of the rest. Ciare intelligently spawns models in a reasonable manner, allowing you to focus on testing your solution in a simulated environment that closely resembles real-world scenarios.\n\n<p align="center">\n  <img width="800" src="https://cdn.jsdelivr.net/gh/ciare-robotics/world-creator@latest/docs/media/demo.svg">\n</p>\n\n# Features\n\n## Current limitations\n\nCurrently it\'s Proof Of Concept solution. There will be a lot of future development. Right now it really does often hallucinate and it\'s spatial notion is not that great, but sometimes it generates something cool.\n\nAlso complex models(like robots) currently is impossible to include. Work will be done on that in the future. Also complex textures of the models are not properly loading too.\n\n## Integration with other simulators\nGenerate simulation worlds on the fly with LLMs.\n\nSupports selected simulators, with plans to expand support to all major simulators.\nSimulator | Supported\n-- | --\nGazebo | ![Static Badge](https://img.shields.io/badge/Yes-green)\nNvidia Isaac Sim | ![Static Badge](https://img.shields.io/badge/Planned-yellow) \nUnity   | ![Static Badge](https://img.shields.io/badge/Planned-yellow)\n\n## Model Database\nIn the future we want to collect a vast model database from which you can freely choose any model to incorporate into your simulations. It aims to become the largest robotics model database available.\n\nCurrently, we use https://app.gazebosim.org/dashboard as database of the models.\n\n# Examples\n\n| Prompt  | Generated world |\n| ------------- | ------------- |\n| Healthcare worker and couple of medical items around them  | ![alt text](./docs/examples/medical.png)  |\n| Pile of fruits and other food in empty world | ![alt text](./docs/examples/pile.png)  |\n\n\n\n# Getting Started\n\n## Installation(Using poetry)\n\n```\ngit clone https://github.com/ciare-robotics/world-creator.git\ncd world-creator\npoetry install\n```\n\n## Token configuration\n\nOnce you installed ciare, you need to save your OpenAI token by launching `ciare_world_creator create` command first time.\n\n## OpenAI API usage\n\nI estimate that creating single world is only a matter of a few cents.\n\n# How to use\n\nCiare has couple of commands\n\n```console\nUsage: ciare ciare_world_creator [OPTIONS] COMMAND [ARGS]...\n\n  World creator by Ciare\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  create            Create new simulation world\n  list              Lists all worlds created by you\n  purge             Delete database and all of the worlds you\'ve created\n  fix               Sometimes, world downloaded can be malformed, so we will\n                   take all objects from that world and respawn them in empty\n                     world\n\n```\n\n## Create simulation world\n\nYou can crate simulation worlds by using command `ciare_world_creator create`. You will need to prompt any query that will describe your simulation world as precise as possible. Model hallucinate pretty often.\n\n```console\nsim@sim:world-creator$ ±|main ✗|→ ciare_world_creator create\n? Enter query for world generation(E.g Two cars and person next to it) Multiple cars spawned 5 meters from each other in empty world. One bicycle besides them\n\nUsing embedded DuckDB with persistence: data will be stored in: /var/tmp/ciare/chromadb\n\nGenerating world... 🌎\nWorld is Test, downloading it\nFile downloaded successfully.\n\nSpawning models in the world... 🫖\n\nPlacing models in the world... 📍\n\nFinished! Output available at /var/tmp/ciare/worlds/world_multiple_cars_spawned_5_meters_from_each_other_in_empty_world_one_bicycle_besides_them.sdf 🦄\n```\n\n## List created worlds\nYou can run `ciare_world_creator list` to view already created worlds. We save every prompt from create command, so later you won\'t query LLM again.\n\n## Purge database\n\nWith `ciare_world_creator purge` you can delete created worlds from local storage and start from scratch.\n\n## Fix malformed world\nWe take database of worlds from https://app.gazebosim.org/, but sometimes someone puts a world there that doesn\'t work at all and breaks because of the missing tag or any other error...\n\nTo overcome this, you can fix already created world by running `ciare_world_creator fix` command and later typing the name of your world. All models will be spawned in the empty world after that.\n\n# Feedback and contributions\nWe welcome feedback and contributions from the community to make Ciare World Creator even better. If you encounter any issues, have ideas for improvements, or would like to contribute to the project, please visit the GitHub repository and open an issue or submit a pull request.\n\nLet\'s create stunning simulation worlds together!\n\n',
+    'long_description': '\n[![Ciare World Creator](/docs/media/logo.png)](https://ciare.dev)\n\n[![GitHub open issues](https://img.shields.io/github/issues-raw/ciare-robotics/world-creator.svg)](https://github.com/ciare/world-creator/issues)\n[![GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/ciare-robotics/world-creator.svg)](https://github.com/ciare/world-creator/pulls)\n[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nCiare World Creator is a CLI tool that reimagines the creation of simulation worlds for robotics. We have a vision that in the future you will not be obliged to painstakingly craft detailed SDF files. With Ciare, you will be able to effortlessly generate dynamic and realistic simulation environments by simply providing input text. Whether you\'re testing robot navigation or experimenting with new solutions, Ciare intelligently spawns models, freeing you from the complexities of precise object placement. By harnessing the power of Language Models (LLMs), Ciare empowers developers to rapidly prototype and explore their ideas, simplifying the simulation process and unlocking a world of possibilities for innovation.\n\nImagine a scenario where you want to test the navigation capabilities of a robot. With Ciare World Creator, you no longer have to spend hours meticulously positioning every object in the simulation. Instead, you simply provide input text to the Ciare pipeline, and it takes care of the rest. Ciare intelligently spawns models in a reasonable manner, allowing you to focus on testing your solution in a simulated environment that closely resembles real-world scenarios.\n\n<p align="center">\n  <img width="800" src="https://cdn.jsdelivr.net/gh/ciare-robotics/world-creator@latest/docs/media/demo.svg">\n</p>\n\n# Features\n\n## Models\n\nCurrently it uses gpt-3.5-16k by default, but if you have access to gpt-4, you will be prompted with a selection. Note that gpt-4 performs much better, but not everyone has the invitation from OpenAI to use it.\n\n## Current limitations\n\nCurrently it\'s Proof Of Concept solution. There will be a lot of future development. Right now it really does often hallucinate and it\'s spatial notion is not that great, but sometimes it generates something cool.\n\nAlso complex models(like robots) currently is impossible to include. Work will be done on that in the future. Also complex textures of the models are not properly loading too.\n\n## Integration with other simulators\nGenerate simulation worlds on the fly with LLMs.\n\nSupports selected simulators, with plans to expand support to all major simulators.\nSimulator | Supported\n-- | --\nGazebo | ![Static Badge](https://img.shields.io/badge/Yes-green)\nNvidia Isaac Sim | ![Static Badge](https://img.shields.io/badge/Planned-yellow) \nUnity   | ![Static Badge](https://img.shields.io/badge/Planned-yellow)\n\n## Model Database\nIn the future we want to collect a vast model database from which you can freely choose any model to incorporate into your simulations. It aims to become the largest robotics model database available.\n\nCurrently, we use https://app.gazebosim.org/dashboard as database of the models.\n\n# Examples\n\n| Prompt  | Generated world |\n| ------------- | ------------- |\n| Healthcare worker and couple of medical items around them  | ![alt text](./docs/examples/medical.png)  |\n| Pile of fruits and other food in empty world | ![alt text](./docs/examples/pile.png)  |\n| Surgical room | ![alt text](./docs/examples/surgical_room.png) |\n| Warehouse shelves | ![alt text](./docs/examples/warehouse_shelves.png) |\n| Usual persons living room| ![alt text](./docs/examples/living_room.png) |\n\n\n# Getting Started\n\n## Installation\n\n### From source using poetry\n```\ngit clone https://github.com/ciare-robotics/world-creator.git\ncd world-creator\npoetry install\n```\n\n### Using pip\n```\npip3 install ciare-world-creator\n```\n\n\n## Token configuration\n\nOnce you installed ciare, you need to save your OpenAI token by launching `ciare_world_creator create` command first time.\n\n## OpenAI API usage\n\nI estimate that creating single world is only a matter of a few cents.\n\n# How to use\n\nCiare has couple of commands\n\n```console\nUsage: ciare ciare_world_creator [OPTIONS] COMMAND [ARGS]...\n\n  World creator by Ciare\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  create            Create new simulation world\n  list              Lists all worlds created by you\n  purge             Delete database and all of the worlds you\'ve created\n  fix               Sometimes, world downloaded can be malformed, so we will\n                   take all objects from that world and respawn them in empty\n                     world\n\n```\n\n## Create simulation world\n\nYou can crate simulation worlds by using command `ciare_world_creator create`. You will need to prompt any query that will describe your simulation world as precise as possible. Model hallucinate pretty often.\n\n```console\nsim@sim:world-creator$ ±|main ✗|→ ciare_world_creator create\n? Enter query for world generation(E.g Two cars and person next to it) Multiple cars spawned 5 meters from each other in empty world. One bicycle besides them\n\nUsing embedded DuckDB with persistence: data will be stored in: /var/tmp/ciare/chromadb\n\nGenerating world... 🌎\nWorld is Test, downloading it\nFile downloaded successfully.\n\nSpawning models in the world... 🫖\n\nPlacing models in the world... 📍\n\nFinished! Output available at /var/tmp/ciare/worlds/world_multiple_cars_spawned_5_meters_from_each_other_in_empty_world_one_bicycle_besides_them.sdf 🦄\n```\n\n## List created worlds\nYou can run `ciare_world_creator list` to view already created worlds. We save every prompt from create command, so later you won\'t query LLM again.\n\n## Purge database\n\nWith `ciare_world_creator purge` you can delete created worlds from local storage and start from scratch.\n\n## Fix malformed world\nWe take database of worlds from https://app.gazebosim.org/, but sometimes someone puts a world there that doesn\'t work at all and breaks because of the missing tag or any other error...\n\nTo overcome this, you can fix already created world by running `ciare_world_creator fix` command and later typing the name of your world. All models will be spawned in the empty world after that.\n\n# Feedback and contributions\nWe welcome feedback and contributions from the community to make Ciare World Creator even better. If you encounter any issues, have ideas for improvements, or would like to contribute to the project, please visit the GitHub repository and open an issue or submit a pull request.\n\nLet\'s create stunning simulation worlds together!\n\n',
     'author': 'Alex Karavaev',
     'author_email': 'alexkaravaev@alexkaravaev.xyz',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ciare-world-creator-0.1.1/PKG-INFO` & `ciare-world-creator-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciare-world-creator
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Alex Karavaev
 Author-email: alexkaravaev@alexkaravaev.xyz
 Requires-Python: >=3.8.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: langchain (>=0.0.222,<0.0.223)
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 
@@ -36,14 +37,18 @@
 
 <p align="center">
   <img width="800" src="https://cdn.jsdelivr.net/gh/ciare-robotics/world-creator@latest/docs/media/demo.svg">
 </p>
 
 # Features
 
+## Models
+
+Currently it uses gpt-3.5-16k by default, but if you have access to gpt-4, you will be prompted with a selection. Note that gpt-4 performs much better, but not everyone has the invitation from OpenAI to use it.
+
 ## Current limitations
 
 Currently it's Proof Of Concept solution. There will be a lot of future development. Right now it really does often hallucinate and it's spatial notion is not that great, but sometimes it generates something cool.
 
 Also complex models(like robots) currently is impossible to include. Work will be done on that in the future. Also complex textures of the models are not properly loading too.
 
 ## Integration with other simulators
@@ -63,27 +68,36 @@
 
 # Examples
 
 | Prompt  | Generated world |
 | ------------- | ------------- |
 | Healthcare worker and couple of medical items around them  | ![alt text](./docs/examples/medical.png)  |
 | Pile of fruits and other food in empty world | ![alt text](./docs/examples/pile.png)  |
-
+| Surgical room | ![alt text](./docs/examples/surgical_room.png) |
+| Warehouse shelves | ![alt text](./docs/examples/warehouse_shelves.png) |
+| Usual persons living room| ![alt text](./docs/examples/living_room.png) |
 
 
 # Getting Started
 
-## Installation(Using poetry)
+## Installation
 
+### From source using poetry
 ```
 git clone https://github.com/ciare-robotics/world-creator.git
 cd world-creator
 poetry install
 ```
 
+### Using pip
+```
+pip3 install ciare-world-creator
+```
+
+
 ## Token configuration
 
 Once you installed ciare, you need to save your OpenAI token by launching `ciare_world_creator create` command first time.
 
 ## OpenAI API usage
 
 I estimate that creating single world is only a matter of a few cents.
```

