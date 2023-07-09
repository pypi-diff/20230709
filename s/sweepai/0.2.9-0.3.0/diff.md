# Comparing `tmp/sweepai-0.2.9.tar.gz` & `tmp/sweepai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.9.tar", max compression
+gzip compressed data, was "sweepai-0.3.0.tar", max compression
```

## Comparing `sweepai-0.2.9.tar` & `sweepai-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.9/LICENSE
--rw-r--r--   0        0        0     5649 2023-07-07 17:07:48.766509 sweepai-0.2.9/README.md
--rw-r--r--   0        0        0     1395 2023-07-07 19:43:15.812873 sweepai-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/__init__.py
--rw-r--r--   0        0        0    10759 2023-07-06 22:37:11.532073 sweepai-0.2.9/sweepai/api.py
--rw-r--r--   0        0        0     5979 2023-07-07 19:36:37.902025 sweepai-0.2.9/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10163 2023-07-07 17:21:31.731293 sweepai-0.2.9/sweepai/app/backend.py
--rw-r--r--   0        0        0     1185 2023-07-06 22:37:11.532073 sweepai-0.2.9/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/app/config.py
--rw-r--r--   0        0        0    11493 2023-07-07 19:31:43.131206 sweepai-0.2.9/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.9/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17384 2023-07-07 17:07:48.766509 sweepai-0.2.9/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.9/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8121 2023-07-07 19:15:26.680881 sweepai-0.2.9/sweepai/core/entities.py
--rw-r--r--   0        0        0    13788 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/core/react.py
--rw-r--r--   0        0        0    16366 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12611 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3612 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    15807 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-04 07:56:27.370433 sweepai-0.2.9/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-06 22:37:11.535407 sweepai-0.2.9/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-07 18:46:43.059593 sweepai-0.2.9/sweepai/utils/constants.py
--rw-r--r--   0        0        0     5230 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-05 21:28:16.693961 sweepai-0.2.9/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8409 2023-07-07 19:15:26.680881 sweepai-0.2.9/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 17:07:48.769842 sweepai-0.2.9/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-05 21:28:16.697295 sweepai-0.2.9/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.9/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-05 21:28:16.697295 sweepai-0.2.9/sweepai/utils/utils.py
--rw-r--r--   0        0        0     6771 2023-07-07 19:43:18.987431 sweepai-0.2.9/setup.py
--rw-r--r--   0        0        0     6558 2023-07-07 19:43:18.987821 sweepai-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5649 2023-07-07 20:46:56.696885 sweepai-0.3.0/README.md
+-rw-r--r--   0        0        0     1395 2023-07-09 01:01:06.768373 sweepai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/__init__.py
+-rw-r--r--   0        0        0    10759 2023-07-07 20:47:46.586917 sweepai-0.3.0/sweepai/api.py
+-rw-r--r--   0        0        0     5979 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10268 2023-07-09 01:00:44.458338 sweepai-0.3.0/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1166 2023-07-09 01:00:31.551651 sweepai-0.3.0/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3546 2023-07-09 01:00:31.551651 sweepai-0.3.0/sweepai/app/config.py
+-rw-r--r--   0        0        0    12903 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8121 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/entities.py
+-rw-r--r--   0        0        0    15579 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/react.py
+-rw-r--r--   0        0        0    18185 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12695 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     6608 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.3.0/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    15025 2023-07-09 01:00:47.045009 sweepai-0.3.0/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0     1551 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-07-09 01:00:31.554984 sweepai-0.3.0/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     5831 2023-07-09 00:27:16.396539 sweepai-0.3.0/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8225 2023-07-09 01:00:44.465005 sweepai-0.3.0/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     6800 2023-07-09 01:01:42.819061 sweepai-0.3.0/setup.py
+-rw-r--r--   0        0        0     6601 2023-07-09 01:01:42.820184 sweepai-0.3.0/PKG-INFO
```

### Comparing `sweepai-0.2.9/LICENSE` & `sweepai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/README.md` & `sweepai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/pyproject.toml` & `sweepai-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.9"
+version = "0.3.0"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -20,14 +20,15 @@
 loguru = "^0.6.0"
 requests = "^2.28.2"
 urllib3 = "^2.0.3"
 gradio = "^3.35.2"
 config-path = "^1.0.3"
 typer = "^0.9.0"
 tabulate = "^0.9.0"
+GitPython = "^3.1.31"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 commit5 = "^0.1.1"
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 build = "^0.10.0"
@@ -44,15 +45,14 @@
 redis = "^4.5.5"
 google-search-results = "^2.4.2"
 slack-sdk = "^3.21.3"
 modal-client = "^0.49.2348"
 anthropic = "^0.2.8"
 tiktoken = "^0.3.2"
 PyJWT = "^2.6.0"
-GitPython = "^3.1.31"
 backoff = "^2.2.1"
 highlight-io = "0.5.0"
 posthog = "^3.0.1"
 tree-sitter = "^0.20.1"
 
 [mypy]
 check_untyped_defs = true
```

### Comparing `sweepai-0.2.9/sweepai/api.py` & `sweepai-0.3.0/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/app/api_client.py` & `sweepai-0.3.0/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/app/backend.py` & `sweepai-0.3.0/sweepai/app/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from fastapi.responses import StreamingResponse
 from pydantic import BaseModel
 
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
 from sweepai.core.sweep_bot import SweepBot
+from sweepai.utils.config import SweepConfig
 from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, PREFIX
 from sweepai.utils.github_utils import get_github_client, get_installation_id
 from sweepai.core.prompts import gradio_system_message_prompt
 from sweepai.utils.event_logger import posthog
 
 get_relevant_snippets = modal.Function.from_name(DB_NAME, "get_relevant_snippets")
 
@@ -129,15 +130,15 @@
                 n_results=request.n_results,
                 installation_id=request.config.installation_id
             )
             g = get_github_client(request.config.installation_id)
             repo = g.get_repo(request.config.repo_full_name)
             for snippet in snippets:
                 try:
-                    snippet.content = repo.get_contents(snippet.file_path).decoded_content.decode("utf-8")
+                    snippet.content = repo.get_contents(snippet.file_path, SweepConfig.get_branch(repo)).decoded_content.decode("utf-8")
                 except Exception:
                     logger.error(snippet)
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
 
         posthog.capture(request.config.github_username, "succeeded", properties=metadata)
@@ -178,15 +179,15 @@
                 snippets="\n".join([snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
                 repo_name=request.config.repo_full_name,
                 repo_description=repo.description
             )
 
             def file_exists(file_path: str) -> bool:
                 try:
-                    repo.get_contents(file_path)
+                    repo.get_contents(file_path, SweepConfig.get_branch(repo))
                     return True
                 except Exception:
                     return False
 
             results = create_pr_func.call(
                 [FileChangeRequest(
                     filename = item[0],
```

### Comparing `sweepai-0.2.9/sweepai/app/cli.py` & `sweepai-0.3.0/sweepai/app/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Launch Sweep Chat in the browser
     """
     SweepChatConfig.load()
     from sweepai.app.ui import demo
     print("\033[93m⭐ Remember to star our repo at https://github.com/sweepai/sweep! \033[0m")
     demo.queue()
-    demo.launch(enable_queue=True, inbrowser=True)
+    demo.launch(inbrowser=True)
     
 @typer_app.command()
 def auth():
     """
     Reauthenticate with Github API for Sweep to work (for token expiry)
     """
     SweepChatConfig.load(recreate=True)
```

### Comparing `sweepai-0.2.9/sweepai/app/config.py` & `sweepai-0.3.0/sweepai/app/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 from urllib.parse import parse_qs, unquote
 import webbrowser
 
 from config_path import ConfigPath
 from pydantic import BaseModel
 import yaml
 
+from sweepai.core.entities import Snippet
+
 CLIENT_ID = "Iv1.91fd31586a926a9f"
 
 DEVICE_CODE_ENDPOINT = "https://github.com/login/device/code"
 USER_LOGIN_ENDPOINT = "https://github.com/login/device"
 OAUTH_ACCESS_TOKEN_ENDPOINT = "https://github.com/login/oauth/access_token"
 
 config_path = ConfigPath( 'sweep_chat', 'sweep', '.yaml' )
 CONFIG_FILE = config_path.saveFilePath()
 
+class State(BaseModel):
+    file_paths: list[str] = []
+    chat_history: list[tuple[str | None, str | None]] = []
+    snippets_text: str = "### Relevant Snippets:"
+
 class SweepChatConfig(BaseModel):
     github_username: str
     github_pat: str # secret
     repo_full_name: str | None = None
     installation_id: int | None = None
-    version: str = "0.0.1"
+    state: State = State()
+    version: str = "0.0.2"
 
     @classmethod
     def create(cls):
         device_code_response = requests.post(DEVICE_CODE_ENDPOINT, json={"client_id": CLIENT_ID})
         parsed_device_code_response = parse_qs(unquote(device_code_response.text))
         print("\033[93m" + f"Open {USER_LOGIN_ENDPOINT} if it doesn't open automatically." + "\033[0m")
         print("\033[93m" + f"Paste the following code (copied to your clipboard) and click authorize:" + "\033[0m")
```

### Comparing `sweepai-0.2.9/sweepai/app/ui.py` & `sweepai-0.3.0/sweepai/app/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 import os
+import tempfile
 from git import Repo
 from github import Github
 import gradio as gr
 from loguru import logger
+import shutil
 
 from sweepai.app.api_client import APIClient, create_pr_function, create_pr_function_call
-from sweepai.app.config import SweepChatConfig
+from sweepai.app.config import State, SweepChatConfig
 from sweepai.core.entities import Snippet
+from sweepai.utils.config import SweepConfig
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
 pr_summary_template = '''⏳ I'm creating the following PR...
 
@@ -90,56 +93,72 @@
         # Make sure repo is added to Sweep before checking all recursive files
         try:
             installation_id = get_installation_id(repo_full_name)
             assert installation_id
         except:
             return []
         repo = github_client.get_repo(repo_full_name)
+        branch_name = SweepConfig.get_branch(repo)
         repo_url = f"https://x-access-token:{config.github_pat}@github.com/{repo_full_name}.git"
-        if os.path.exists("/tmp/" + repo_full_name):
-            git_repo = Repo("/tmp/" + repo_full_name)
+        try:
+            repo_dir = os.path.join(tempfile.gettempdir(), repo_full_name)
+            if os.path.exists(repo_dir):
+                git_repo = Repo(repo_dir)
+            else:
+                git_repo = Repo.clone_from(repo_url, repo_dir)
+            git_repo.git.checkout(branch_name)
             git_repo.remotes.origin.pull()
-        else:
-            Repo.clone_from(repo_url, "/tmp/" + repo_full_name)
-        all_files, path_to_contents = get_files_recursively("/tmp/" + repo_full_name)
+        except Exception as e:
+            logger.warning(f"Git pull failed with error {e}, deleting cache and recloning...")
+            shutil.rmtree(repo_dir)
+            git_repo = Repo.clone_from(repo_url, repo_dir)
+            git_repo.git.checkout(branch_name)
+            git_repo.remotes.origin.pull()
+        all_files, path_to_contents = get_files_recursively(repo_dir)
     return all_files
 
 def get_files_update(*args):
     global repo
     if len(args) > 0:
         repo = args[0]
     else:
         repo = config.repo_full_name
     return gr.Dropdown.update(choices=get_files(repo))
 
+global_state = config.state
 
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
     print("Launching gradio!")
     with gr.Row():
-        with gr.Column():
-            repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=config.repo_full_name or "")
-        print("Indexing files...")
         with gr.Column(scale=2):
-            file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files")
+            repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=lambda: config.repo_full_name or "")
+        print("Indexing files...")
+        with gr.Column(scale=4):
+            file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files", value=lambda: global_state.file_paths)
         print("Indexed files!")
         repo_full_name.change(get_files_update, repo_full_name, file_names)
+        with gr.Column(scale=1):
+            restart_button = gr.Button("Restart")
 
     with gr.Row():
         with gr.Column(scale=2):
-            chatbot = gr.Chatbot(height=750)
+            chatbot = gr.Chatbot(height=750, value=lambda: global_state.chat_history)
         with gr.Column():
-            snippets_text = gr.Markdown(value="### Relevant snippets", elem_id="snippets")
+            snippets_text = gr.Markdown(value=lambda: global_state.snippets_text, elem_id="snippets")
     
     with gr.Row():
         with gr.Column(scale=8):
             msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
         with gr.Column(scale=0.5):
             create_pr_button = gr.Button(value="Create PR", interactive=False)
 
-    # proposed_pr: str | None = None
+    restart_button.click(lambda: ([], []), [], [file_names, chatbot])
+
+    file_names.change(get_files_update, repo_full_name, chatbot)
+
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
         global installation_id
         try:
@@ -152,39 +171,39 @@
         except Exception as e:
             config.repo_full_name = None
             config.installation_id = None
             config.save()
             api_client.config = config
             raise e
 
-    repo_full_name.change(repo_name_change, [repo_full_name], [msg])
-
     def build_string():
         global selected_snippets
         global file_to_str
         for snippet in selected_snippets:
             file_name = snippet.file_path
             if file_name not in file_to_str:
                 add_file_to_dict(file_name)
         snippets_text = "### Relevant snippets:\n" + "\n\n".join([file_to_str[snippet.file_path] for snippet in selected_snippets])
         return snippets_text
 
+    repo_full_name.change(repo_name_change, [repo_full_name], [msg])
+
     def add_file_to_dict(file_name):
         global file_to_str
         global path_to_contents
         global repo
         if file_name in path_to_contents:
             file_contents = path_to_contents[file_name]
         else:
-            file_contents = repo.get_contents(file_name).decoded_content.decode('utf-8')
+            file_contents = repo.get_contents(file_name, ref=SweepConfig.get_branch(repo)).decoded_content.decode('utf-8')
         file_contents_split = file_contents.split("\n")
         length = len(file_contents_split)
         backtick, escaped_backtick = "`", "\\`"
         preview = "\n".join(file_contents_split[:3]).replace(backtick, escaped_backtick)
-        file_to_str[file_name] = f'{file_name}:0:{length}\n```python\n{preview}\n...\n```'
+        file_to_str[file_name] = f'{file_name}:0:{length}\n```\n{preview}\n...\n```'
     
     def file_names_change(file_names):
         global selected_snippets
         global file_to_str
         global path_to_contents
         selected_snippets = [Snippet(content=path_to_contents[file_name], start=0, end=path_to_contents[file_name].count('\n'), file_path=file_name) for file_name in file_names]
         return file_names, build_string()
@@ -192,15 +211,15 @@
     file_names.change(file_names_change, [file_names], [file_names, snippets_text])
     
     def handle_message_submit(repo_full_name: str, user_message: str, history: list[tuple[str | None, str | None]]):
         if not repo_full_name:
             raise Exception("Set the repository name first")
         return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(interactive=True)
 
-    def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names):
+    def _handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names):
         global selected_snippets
         global searched
         message = chat_history[-1][0]
         yield chat_history, snippets_text, file_names
         if not selected_snippets:
             searched = True
             # Searching for relevant snippets
@@ -235,15 +254,15 @@
             stream = api_client.stream_chat(chat_history, selected_snippets)
         function_name = ""
         raw_arguments = ""
         for chunk in stream:
             if chunk.get("content"):
                 token = chunk["content"]
                 chat_history[-1][1] += token
-                yield chat_history, snippets_text, file_names, "Create PR"
+                yield chat_history, snippets_text, file_names
             if chunk.get("function_call"):
                 function_call = chunk["function_call"]
                 function_name = function_name or function_call.get("name")
                 raw_arguments += function_call.get("arguments")
                 chat_history[-1][1] = f"Calling function: `{function_name}`\n```json\n{raw_arguments}\n```"
                 yield chat_history, snippets_text, file_names
         if function_name:
@@ -255,28 +274,40 @@
                 if "branch" not in arguments:
                     arguments["branch"] = arguments["title"].lower().replace(" ", "_").replace("-", "_")[:50]
                 chat_history[-1][1] = pr_summary_template.format(
                     title=arguments["title"],
                     summary=arguments["summary"],
                     plan="\n".join([f"* `{item['file_path']}`: {item['instructions']}" for item in arguments["plan"]])
                 )
-                yield chat_history, snippets_text, file_names, "Create PR"
+                yield chat_history, snippets_text, file_names
                 pull_request = api_client.create_pr(
                     file_change_requests=[(item["file_path"], item["instructions"]) for item in arguments["plan"]],
                     pull_request={
                         "title": arguments["title"],
                         "content": arguments["summary"],
                         "branch_name": arguments["branch"],
                     },
                     messages=chat_history,
                 )
                 chat_history.append((None, f"✅ PR created at {pull_request['html_url']}"))
-                yield chat_history, snippets_text, file_names, "Create PR"
+                yield chat_history, snippets_text, file_names
             else:
                 raise NotImplementedError
+    
+    def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_paths):
+        global global_state
+        for chat_history, snippets_text, file_paths in _handle_message_stream(chat_history, snippets_text, file_paths):
+            global_state = State(
+                chat_history=chat_history,
+                snippets_text=snippets_text,
+                file_paths=file_paths,
+            )
+            config.state = global_state
+            config.save()
+            yield chat_history, snippets_text, file_paths
 
     response = msg \
         .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False)\
         .then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
     response.then(lambda: gr.update(interactive=True), None, [msg], queue=False)
 
     def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], create_pr_button: str):
```

### Comparing `sweepai-0.2.9/sweepai/core/chat.py` & `sweepai-0.3.0/sweepai/core/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             return [
                 message
                 for message in self.messages
                 if message.key == message_key and message.role == message_role
             ][0]
         return [message for message in self.messages if message.key == message_key][0]
 
-    def delete_messages_from_chat(self, message_key: str):
+    def delete_messages_from_chat(self, key_to_delete: str):
         self.messages = [
-            message for message in self.messages if message.key != message_key
+            message for message in self.messages if key_to_delete not in (message.key or '')
         ]
 
     def delete_file_from_system_message(self, file_path: str):
         self.human_message.delete_file(file_path)
 
     def get_message_content_from_message_key(
         self, message_key: str, message_role: str = None
```

### Comparing `sweepai-0.2.9/sweepai/core/code_repair.py` & `sweepai-0.3.0/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/core/entities.py` & `sweepai-0.3.0/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/core/prompts.py` & `sweepai-0.3.0/sweepai/core/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -211,14 +211,15 @@
 
 Reply in the following format. DO NOT write "pass" or "Rest of code". Do not literally write "{{new_file}}". You must use the new_file XML tags, and all text inside these tags will be placed in the newly created file.
 
 Step-by-step thoughts with explanations: 
 * Thought 1 - Explanation 1
 * Thought 2 - Explanation 2
 ...
+
 Detailed plan of additions:
 * Addition 1
 * Addition 2
 ...
 Commit Message: {{commit_message}}
 <new_file>
 {{new_file}}
@@ -239,57 +240,122 @@
 Then create a plan of parts of the code to modify with detailed references to functions to modify.
 
 File Name: {filename}
 <old_file>
 {code}
 </old_file>
 
-Your instructions to modify the file are: "{instructions}".
+Your instructions to modify the file are: "{instructions}". Limit your changes to the instructions.
 
 Step-by-step thoughts with explanations: 
 * Thought 1 - Explanation 1
 * Thought 2 - Explanation 2
 ...
+
 Detailed plan of modifications:
 * Modification 1
 * Modification 2
 ...
-"""
 
+Lines to change in the file:
+* lines a-b
+...
+
+Only include the line numbers."""
+
+#<snippets>
+#{snippets}
+#</snippets>
 modify_file_prompt = """
+File contains lines {line_numbers}
+
 Generate a new_file based on the given plan, ensuring that you:
 1. Do not write "pass" statements.
 2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
 3. Do not write new "todo" comments.
 4. Do not write incomplete functions.
 5. Do not write the original line numbers with the new code.
 6. Make sure the new code follows the same programming language conventions as the old code.
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copied>0-25</copied>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copied>0-50</copied>".
 
-Example: New file:
-print("new file")
+Example: If you want to modify lines 51-52 and add line after line 75:
+<new_file>
+<copied>1-50</copied>
+def main():
+     print("hello world")
+<copied>53-75</copied>
+print("debug statement")
+<copied>76-100</copied>
 </new_file>
 
-Example: Insert at end:
-<copied>0-100</copied>
-print("inserted at end")
-</new_file>
+Do not rewrite entire file. Use <copied> XML tag when possible.
+"""
+
+
+modify_file_prompt_2 = """
+File Name: {filename}
+<old_file>
+{code}
+</old_file>
+
+---
+
+Code Planning:
+```
+Step-by-step thoughts with explanations: 
+* Thought 1 - Explanation 1
+* Thought 2 - Explanation 2
+...
 
-Example: If you want to insert code after lines 50 and 75:
+Detailed plan of modifications:
+* Modification 1
+* Modification 2
+...
+
+Lines to change in the file:
+* lines a-b
+...
+```
+
+Code Generation:
+```
+Generate a new_file based on the given plan, ensuring that you:
+1. Do not write "pass" statements.
+2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
+3. Do not write new "todo" comments.
+4. Do not write incomplete functions.
+5. Do not write the original line numbers with the new code.
+6. Make sure the new code follows the same programming language conventions as the old code.
+
+Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copy_lines A-B>"). Make sure to use this exact format.
+Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copy_lines 1-50>".
+
+Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
-<copied>0-50</copied>
+<copy_lines 1-50>
 def main():
      print("hello world")
-<copied>51-75</copied>
+<copy_lines 53-75>
 print("debug statement")
-<copied>76-100</copied>
+<copy_lines 76-100>
 </new_file>
-"""
+
+Do not rewrite entire file. Use <copy_lines A-B> XML tag when possible. Do not include the line numbers in the new file.
+```
+
+Context: "{instructions}". Limit your changes to the context.
+Instructions:
+- Complete Code Planning step
+- Complete Code Generation step"""
+
+
+
+
 
 pr_code_prompt = ""  # TODO: deprecate this
 
 
 pull_request_prompt = """
 Awesome! Could you also provide a PR message in the following format? Content should be in Github style markdown. Thanks!
```

### Comparing `sweepai-0.2.9/sweepai/core/react.py` & `sweepai-0.3.0/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/core/sweep_bot.py` & `sweepai-0.3.0/sweepai/core/sweep_bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from github.Repository import Repository
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
 import modal
 from pydantic import BaseModel
 from sweepai.core.code_repair import CodeRepairer
 from sweepai.utils.chat_logger import ChatLogger
+import re
 
 from sweepai.core.entities import (
     FileChange,
     FileChangeRequest,
     FilesToChange,
     PullRequest,
     RegexMatchError,
@@ -19,17 +20,18 @@
     Snippet
 )
 from sweepai.core.chat import ChatGPT
 from sweepai.core.prompts import (
     files_to_change_prompt,
     pull_request_prompt,
     create_file_prompt,
-    modify_file_prompt,
+    modify_file_prompt_2,
     modify_file_plan_prompt,
 )
+from sweepai.utils.config import SweepConfig
 from sweepai.utils.constants import DB_NAME
 from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown, revert_whitespace_changes
 
 
 class CodeGenBot(ChatGPT):
 
     def get_files_to_change(self):
@@ -76,17 +78,18 @@
 
     def generate_pull_request(self) -> PullRequest:
         pull_request = None
         for count in range(5):
             try:
                 logger.info(f"Generating for the {count}th time...")
                 pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
+                self.delete_messages_from_chat("pull_request")
             except Exception as e:
                 logger.warning(f"Exception {e}. Failed to parse! Retrying...")
-                self.undo()
+                self.delete_messages_from_chat("pull_request")
                 continue
             pull_request = PullRequest.from_string(pr_text_response)
             pull_request.branch_name = "sweep/" + pull_request.branch_name[:250]
             return pull_request
         raise Exception("Could not generate PR text")
 
 
@@ -94,15 +97,15 @@
     class Config:
         arbitrary_types_allowed = True  # for repo: Repository
 
     repo: Repository
 
     def get_contents(self, path: str, branch: str = ""):
         if not branch:
-            branch = self.repo.default_branch
+            branch = SweepConfig.get_branch(self.repo)
         try:
             return self.repo.get_contents(path, ref=branch)
         except Exception as e:
             logger.warning(path)
             raise e
 
     def get_file(self, file_path: str, branch: str = "") -> ContentFile:
@@ -135,15 +138,15 @@
                 except GithubException:
                     pass
             raise e
     
     def populate_snippets(self, snippets: list[Snippet]):
         for snippet in snippets:
             try:
-                snippet.content = self.repo.get_contents(snippet.file_path).decoded_content.decode("utf-8")
+                snippet.content = self.repo.get_contents(snippet.file_path, SweepConfig.get_branch(self.repo)).decoded_content.decode("utf-8")
             except Exception as e:
                 logger.error(snippet)
     
     def search_snippets(
         self, 
         query: str, 
         installation_id: str,
@@ -158,15 +161,15 @@
         )
         self.populate_snippets(snippets)
         return snippets
     
     def validate_file_change_requests(self, file_change_requests: list[FileChangeRequest]):
         for file_change_request in file_change_requests:
             try:
-                contents = self.repo.get_contents(file_change_request.filename)
+                contents = self.repo.get_contents(file_change_request.filename, SweepConfig.get_branch(self.repo))
                 if contents:
                     file_change_request.change_type = "modify"
                 else:
                     file_change_request.change_type = "create"
             except:
                 file_change_request.change_type = "create"
         return file_change_requests
@@ -234,32 +237,34 @@
         #                 functions=functions
         #             ) # update this constant
         return
 
     def create_file(self, file_change_request: FileChangeRequest) -> FileChange:
         file_change: FileChange | None = None
         for count in range(5):
+            key = f"file_change_created_{file_change_request.filename}"
             create_file_response = self.chat(
                 create_file_prompt.format(
                     filename=file_change_request.filename,
                     instructions=file_change_request.instructions,
                 ),
-                message_key=f"file_change_{file_change_request.filename}",
+                message_key=key,
             )
             # Add file to list of changed_files
             self.file_change_paths.append(file_change_request.filename)
             # self.delete_file_from_system_message(file_path=file_change_request.filename)
             try:
                 file_change = FileChange.from_string(create_file_response)
                 assert file_change is not None
                 file_change.commit_message = f"sweep: {file_change.commit_message[:50]}"
                 return file_change
             except Exception:
+                # Todo: should we undo appending to file_change_paths?
                 logger.warning(f"Failed to parse. Retrying for the {count}th time...")
-                self.undo()
+                self.delete_messages_from_chat(key)
                 continue
         raise Exception("Failed to parse response after 5 attempts.")
 
     def modify_file(
         self, file_change_request: FileChangeRequest, contents: str = ""
     ) -> tuple[str, str]:
         if not contents:
@@ -267,42 +272,73 @@
                 file_change_request.filename
             ).decoded_content.decode("utf-8")
         # Add line numbers to the contents; goes in prompts but not github
         contents_line_numbers = "\n".join([f"{i + 1}:{line}" for i, line in enumerate(contents.split("\n"))])
         contents_line_numbers = contents_line_numbers.replace('"""', "'''")
         for count in range(5):
             if "0613" in self.model:
-                _ = self.chat( # We don't use the plan in the next call
+                """
+                planning_response = self.chat( # We don't use the plan in the next call
                     modify_file_plan_prompt.format(
                         filename=file_change_request.filename,
                         instructions=file_change_request.instructions,
                         code=contents_line_numbers,
                     ),
                     message_key=f"file_change_{file_change_request.filename}",
                 )
+
+                snippet_string = ""
+                lines = []
+                for match in re.findall(r"(?:lines (\d+)-(\d+)|line (\d+))", planning_response):
+                    if len(match[2]) > 0:
+                        start_line = int(match[2])
+                        end_line = start_line
+                    else:
+                        start_line = int(match[0])
+                        end_line = int(match[1])
+                    lines.append('\n'.join(contents_line_numbers.splitlines()[start_line - 1:end_line]))
+
+                code_snippets = '\n...\n'.join(lines)
+
+                newline = '\n'
                 modify_file_response = self.chat(
-                    modify_file_prompt,
+                    modify_file_prompt.format(
+                        snippets=code_snippets,
+                        line_numbers=f'{1} to {1 + contents.count(newline)}'
+                    ),
                     message_key=f"file_change_{file_change_request.filename}",
                 )
+                """
+
+                # Todo: updated code is outdated by unified v2 prompt! remove?
+                key = f"file_change_modified_{file_change_request.filename}"
+                modify_file_response = self.chat(
+                    modify_file_prompt_2.format(
+                        filename=file_change_request.filename,
+                        instructions=file_change_request.instructions,
+                        code=contents_line_numbers,
+                        line_count=contents.count('\n') + 1
+                    ),
+                    message_key=key,
+                )
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
                         code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
                         new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
                         # new_file = revert_whitespace_changes(original_file_str=contents, modified_file_str=new_file)
                     return (new_file, file_change_request.filename)
                 except Exception as e:
                     logger.warning(f"Recieved error {e}")
                     logger.warning(
                         f"Failed to parse. Retrying for the {count}th time..."
                     )
-                    self.undo()
-                    self.undo()
+                    self.delete_messages_from_chat(key)
                     continue
         raise Exception("Failed to parse response after 5 attempts.")
  
     def change_file(self, file_change_request: FileChangeRequest):
         if file_change_request.change_type == "create":
             return self.create_file(file_change_request)
         elif file_change_request.change_type == "modify":
@@ -350,14 +386,15 @@
     def handle_modify_file(self, file_change_request: FileChangeRequest, branch: str, file_markdown: bool):
         try:
             contents = self.get_file(file_change_request.filename, branch=branch)
             new_file_contents, file_name = self.modify_file(
                 file_change_request, contents.decoded_content.decode("utf-8")
             )
             new_file_contents = format_contents(new_file_contents, file_markdown)
+            new_file_contents = new_file_contents.rstrip()
             if contents.decoded_content.decode("utf-8").endswith("\n"):
                 new_file_contents += "\n"
             logger.debug(
                 f"{file_name}, {f'Update {file_name}'}, {new_file_contents}, {branch}"
             )
             self.repo.update_file(
                 file_name,
```

### Comparing `sweepai-0.2.9/sweepai/core/vector_db.py` & `sweepai-0.3.0/sweepai/core/vector_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,27 +138,29 @@
             logger.info(f"Failed to get cache for {repo_name}")
     logger.info(f"Downloading repository and indexing for {repo_name}...")
     start = time.time()
     logger.info("Recursively getting list of files...")
 
     repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
     shutil.rmtree("repo", ignore_errors=True)
-    Repo.clone_from(repo_url, "repo")
+    
+    branch_name = SweepConfig.get_branch(repo)
+
+    git_repo = Repo.clone_from(repo_url, "repo")
+    git_repo.git.checkout(branch_name)
 
     file_list = glob.iglob("repo/**", recursive=True)
     file_list = [
         file
         for file in tqdm(file_list)
         if os.path.isfile(file)
         and all(not file.endswith(ext) for ext in sweep_config.exclude_exts)
         and all(not file[len("repo/"):].startswith(dir_name) for dir_name in sweep_config.exclude_dirs)
     ]
 
-    branch_name = repo.default_branch
-
     file_paths = []
     file_contents = []
     scores = []
 
     for file in tqdm(file_list):
         with open(file, "rb") as f:
             is_binary = False
@@ -215,15 +217,15 @@
     documents, metadatas, ids = zip(*chunked_results)
     documents = [item for sublist in documents for item in sublist]
     metadatas = [item for sublist in metadatas for item in sublist]
     ids = [item for sublist in ids for item in sublist]
     
     logger.info(f"Used {len(file_paths)} files...")
 
-    shutil.rmtree("repo")
+    shutil.rmtree("repo", ignore_errors=True)
     logger.info(f"Getting list of all files took {time.time() -start}")
     logger.info(f"Received {len(documents)} documents from repository {repo_name}")
     collection_name = parse_collection_name(repo_name)
     return compute_deeplake_vs(collection_name, documents, cache_success, cache, ids, metadatas, commit_hash)
     
 def compute_deeplake_vs(collection_name, 
                         documents,
```

### Comparing `sweepai-0.2.9/sweepai/events.py` & `sweepai-0.3.0/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/handlers/create_pr.py` & `sweepai-0.3.0/sweepai/handlers/create_pr.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from loguru import logger
 import modal
 
 from sweepai.core.entities import FileChangeRequest, PullRequest
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.handlers.on_review import review_pr
+from sweepai.utils.config import SweepConfig
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client
 from sweepai.utils.constants import DB_NAME, PREFIX
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
@@ -74,15 +75,15 @@
         else:
             pr_description = f"{pull_request.content}\n\nTo checkout this PR branch, run the following command in your terminal:\n```zsh\ngit checkout {pull_request.branch_name}\n```"
 
         pr = sweep_bot.repo.create_pull(
             title=pull_request.title,
             body=pr_description,
             head=pull_request.branch_name,
-            base=sweep_bot.repo.default_branch,
+            base=SweepConfig.get_branch(sweep_bot.repo),
         )
     except openai.error.InvalidRequestError as e:
         logger.error(e)
         posthog.capture(
             username,
             "failed",
             properties={
```

### Comparing `sweepai-0.2.9/sweepai/handlers/on_comment.py` & `sweepai-0.3.0/sweepai/handlers/on_comment.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import (
     get_github_client,
     search_snippets,
 )
 from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
 from sweepai.utils.constants import PREFIX
+from sweepai.utils.chat_logger import ChatLogger
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 
 def on_comment(
     repo_full_name: str,
@@ -91,17 +92,34 @@
             tree=tree,
             summary=pr_body,
             snippets=snippets,
             pr_file_path=pr_file_path, # may be None
             pr_line=pr_line, # may be None
         )
         logger.info(f"Human prompt{human_message.construct_prompt()}")
+
+        chat_logger = ChatLogger({
+            'repo_name': repo_name,
+            'title': '(Comment) ' + pr_title,
+            "issue_url": pr.html_url,
+            "pr_file_path": pr_file_path,  # may be None
+            "pr_line": pr_line,  # may be None
+            "repo_full_name": repo_full_name,
+            "repo_description": repo_description,
+            "comment": comment,
+            "pr_path": pr_path,
+            "pr_line_position": pr_line_position,
+            "username": username,
+            "installation_id": installation_id,
+            "pr_number": pr_number,
+            "type": "comment",
+        })
         sweep_bot = SweepBot.from_system_message_content(
             # human_message=human_message, model="claude-v1.3-100k", repo=repo
-            human_message=human_message, repo=repo, 
+            human_message=human_message, repo=repo, chat_logger=chat_logger
         )
     except Exception as e:
         posthog.capture(username, "failed", properties={
             "error": str(e),
             "reason": "Failed to get files",
             **metadata
         })
```

### Comparing `sweepai-0.2.9/sweepai/handlers/on_review.py` & `sweepai-0.3.0/sweepai/handlers/on_review.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from loguru import logger
 from sweepai.core.entities import DiffSummarization, PullRequestComment
 from sweepai.core.prompts import review_prompt
 from sweepai.core.sweep_bot import SweepBot
 
 from sweepai.utils.github_utils import get_file_contents
 from sweepai.utils.prompt_constructor import HumanMessageFinalPRComment, HumanMessagePromptReview, HumanMessageReviewFollowup
+from sweepai.utils.chat_logger import ChatLogger
 
 # Plan:
 # 1. Get PR
 # 2. Get files changed
 # 3. Come up with some comments for the PR
 # 4. Take comments and add them to the PR
 
@@ -50,17 +51,34 @@
         snippets=[],
         tree=tree,
         diffs=[diffs[0] if len(diffs) > 0 else ""],
         pr_title=pr.title,
         pr_message=pr.body or "",
     )
     summarization_replies = []
+
+    chat_logger = ChatLogger({
+        'repo_name': repo_name,
+        'title': '(Review) ' + title,
+        'summary': summary + replies_text,
+        "issue_url": issue_url,
+        "username": username,
+        "repo_description": repo_description,
+        "issue_url": issue_url,
+        "username": username,
+        "repo_description": repo_description,
+        "title": title,
+        "summary": summary,
+        "replies_text": replies_text,
+        "tree": tree,
+        "type": "review",
+    })
     sweep_bot = SweepBot.from_system_message_content(
         # human_message=human_message, model="claude-v1.3-100k", repo=repo, is_reply=False
-        human_message=human_message, repo=repo, is_reply=False
+        human_message=human_message, repo=repo, is_reply=False, chat_logger=chat_logger
     )
     summarization_reply = sweep_bot.chat(review_prompt, message_key="review")
     extracted_summary = DiffSummarization.from_string(summarization_reply)
     summarization_replies.append(extracted_summary.content)
     for diff in diffs[1:]:
         review_message = HumanMessageReviewFollowup(diff=diff)
         review_prompt_constructed = review_message.construct_prompt()
```

### Comparing `sweepai-0.2.9/sweepai/handlers/on_ticket.py` & `sweepai-0.3.0/sweepai/handlers/on_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,44 @@
   {body}
 </details>
 '''
 
 chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 num_of_snippets_to_query = 30
-max_num_of_snippets = 5
+# max_num_of_snippets = 5
+total_number_of_snippet_tokens = 15_000
+num_full_files = 2
+num_extended_snippets = 2
+
+def post_process_snippets(snippets: list[Snippet]):
+    for snippet in snippets[:num_full_files]:
+        snippet = snippet.expand()
+
+    # snippet fusing
+    i = 0
+    while i < len(snippets):
+        j = i + 1
+        while j < len(snippets):
+            if snippets[i] ^ snippets[j]:  # this checks for overlap
+                snippets[i] = snippets[i] | snippets[j]  # merging
+                snippets.pop(j)
+            else:
+                j += 1
+        i += 1
+
+    # truncating snippets based on character length
+    result_snippets = []
+    total_length = 0
+    for snippet in snippets:
+        total_length += len(snippet.get_snippet())
+        if total_length > total_number_of_snippet_tokens * 5:
+            break
+        result_snippets.append(snippet)
+    return result_snippets
 
 def on_ticket(
     title: str,
     summary: str,
     issue_number: int,
     issue_url: str,
     username: str,
@@ -74,17 +103,14 @@
     # 3. Get files to change
     # 4. Get file changes
     # 5. Create PR
 
     organization, repo_name = repo_full_name.split("/")
     metadata = {
         "issue_url": issue_url,
-        "issue_number": issue_number,
-        "repo_full_name": repo_full_name,
-        "organization": organization,
         "repo_name": repo_name,
         "repo_description": repo_description,
         "username": username,
         "installation_id": installation_id,
         "function": "on_ticket",
         "mode": PREFIX,
     }
@@ -196,58 +222,16 @@
         logger.error(e)
         comment_reply(
             "It looks like an issue has occured around fetching the files. Perhaps the repo has not been initialized: try removing this repo and adding it back. I'll try again in a minute. If this error persists contact team@sweep.dev.",
             -1
         )
         log_error("File Fetch", str(e))
         raise e
-
-    num_full_files = 2
-    num_extended_snippets = 2
-
-    most_relevant_snippets = snippets[:num_full_files]
-    snippets = snippets[:-num_full_files]
-    logger.info("Expanding snippets...")
-    for snippet in most_relevant_snippets:
-        current_snippet = snippet
-        _chunks, metadatas, _ids = chunker.call(
-            current_snippet.content,
-            current_snippet.file_path
-        )
-        segmented_snippets = [
-            Snippet(
-                content=current_snippet.content,
-                start=metadata["start"],
-                end=metadata["end"],
-                file_path=metadata["file_path"],
-            ) for metadata in metadatas
-        ]
-        index = 0
-        while index < len(segmented_snippets) and segmented_snippets[index].start <= current_snippet.start:
-            index += 1
-        index -= 1
-        for i in range(index + 1, min(index + num_extended_snippets + 1, len(segmented_snippets))):
-            current_snippet += segmented_snippets[i]
-        for i in range(index - 1, max(index - num_extended_snippets - 1, 0), -1):
-            current_snippet = segmented_snippets[i] + current_snippet
-        snippets.append(current_snippet)
-
-    # snippet fusing
-    i = 0
-    while i < len(snippets):
-        j = i + 1
-        while j < len(snippets):
-            if snippets[i] ^ snippets[j]:  # this checks for overlap
-                snippets[i] = snippets[i] | snippets[j]  # merging
-                snippets.pop(j)
-            else:
-                j += 1
-        i += 1
-
-    snippets = snippets[:min(len(snippets), max_num_of_snippets)]
+    
+    snippets = post_process_snippets(snippets)
 
     human_message = HumanMessagePrompt(
         repo_name=repo_name,
         issue_url=issue_url,
         username=username,
         repo_description=repo_description,
         title=title,
```

### Comparing `sweepai-0.2.9/sweepai/utils/chat_logger.py` & `sweepai-0.3.0/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/constants.py` & `sweepai-0.3.0/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/diff.py` & `sweepai-0.3.0/sweepai/utils/diff.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,21 +72,39 @@
 def generate_new_file(modify_file_response: str, old_file_content: str) -> str:
     import re
 
     result_file = ""
     old_file_lines = old_file_content.splitlines()
 
     # Extract content between <new_file> tags
-    new_file = re.search(r"<new_file>(.*?)<\/new_file>", modify_file_response, re.DOTALL).group(1).strip()
-    if "<copied>" not in new_file:
+    new_file = re.search(r".*?<new_file>(.*)<\/new_file>", modify_file_response, re.DOTALL).group(1).strip()
+    if "<copy_lines" not in new_file:
         return new_file
 
-    # Find all <copied> tags and their content
-    copied_sections = re.findall(r"<copied>(.*?)<\/copied>", new_file, re.DOTALL)
-    
+    # v5
+    result = []
+    lines = new_file.split('\n')
+    for line in lines:
+        # Todo: make it support 1 number only
+        matches = re.finditer(r"<copy_lines\s(\d+-\d+)>", line)
+        for match in matches:
+            start, end = match.group(1).split('-')
+            start, end = int(start)-1, int(end)-1
+
+            start = max(0, start)
+            end = min(len(old_file_lines) - 1, end)
+
+            replacements = old_file_lines[start:end + 1]
+            replacements_str = '\n'.join(replacements)
+            line = line.replace(match.group(0), replacements_str)
+        result.append(line)
+    result = '\n'.join(result)
+
+    # Todo: v4 is inefficient; deprecated
+    """
     first_section_idx = new_file.index("<copied>")
     if first_section_idx > 0:
         result_file += new_file[:first_section_idx]
         new_file = new_file[first_section_idx:] # remove the first section from new_file
     last_section_idx = new_file.rindex("</copied>")
     last_section = ""
     if last_section_idx < len(new_file) - 1:
@@ -108,15 +126,19 @@
         result_file = join_contents_k(result_file, "\n".join(old_file_lines[start_line:end_line]), k)
         # TODO: Use replace first instead of .replace, since duplicated <copied> sections might cause faulty copy
         new_file = new_file.replace(f"<copied>{copied_section}</copied>\n", "")
         next_section_idx = new_file.index("<copied>") if "<copied>" in new_file else len(new_file)
         # Check for duplicate lines
         result_file = join_contents_k(result_file, new_file[:next_section_idx], k)
         new_file = new_file[next_section_idx:] # remove the first section from new_file
+    
     return result_file + last_section
+    """
+
+    return result
     
 def join_contents_k(first, second, k):
     """
     Join contents together removing k duplicate lines
     """
     first_lines = first.splitlines()
     second_lines = second.splitlines()
```

### Comparing `sweepai-0.2.9/sweepai/utils/event_logger.py` & `sweepai-0.3.0/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/file_change_functions.py` & `sweepai-0.3.0/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/github_utils.py` & `sweepai-0.3.0/sweepai/utils/github_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,23 +120,24 @@
 #     token = get_token(installation_id)
 #     repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
 #     Repo.clone_from(repo_url, "repo")
 #     tree = display_directory_tree("repo")
 #     shutil.rmtree("repo")
 #     return tree
 def get_tree_and_file_list(
-    repo_name: str, 
+    repo: Repository, 
     installation_id: int, 
     snippet_paths: list[str]
 ) -> str:
     from git import Repo
     token = get_token(installation_id)
     shutil.rmtree("repo", ignore_errors=True)
-    repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
-    Repo.clone_from(repo_url, "repo")
+    repo_url = f"https://x-access-token:{token}@github.com/{repo.full_name}.git"
+    git_repo = Repo.clone_from(repo_url, "repo")
+    git_repo.git.checkout(SweepConfig.get_branch(repo))
 
     prefixes = []
     for snippet_path in snippet_paths:
         file_list = ""
         for directory in snippet_path.split("/")[:-1]:
             file_list += directory + "/"
             prefixes.append(file_list.rstrip("/"))
@@ -164,66 +165,57 @@
     repo: Repository,
     query: str,
     installation_id: int,
     num_files: int = 5,
     include_tree: bool = True,
     branch: str = None,
     sweep_config: SweepConfig = SweepConfig(),
-) -> tuple[Snippet, str]:
+) -> tuple[list[Snippet], str]:
     # Initialize the relevant directories string
     get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
     snippets: list[Snippet] = get_relevant_snippets.call(
         repo.full_name, query, num_files, installation_id=installation_id
     )
     logger.info(f"Snippets: {snippets}")
-    total_file_contents = 0
     # TODO: We should prioritize the mentioned files
     for snippet in snippets:
         try:
             file_contents = get_file_contents(repo, snippet.file_path, ref=branch)
-            if (
-                total_file_contents > sweep_config.max_file_limit
-            ):  # more than 10000 tokens
+            if len(file_contents) > sweep_config.max_file_limit:  # more than ~10000 tokens
                 logger.warning(f"Skipping {snippet.file_path}, too many tokens")
                 continue
-            else:
-                total_file_contents += len(file_contents)
         except github.UnknownObjectException as e:
             logger.warning(f"Error: {e}")
             logger.warning(f"Skipping {snippet.file_path}")
         else:
             snippet.content = file_contents
     tree, file_list = get_tree_and_file_list(
-        repo.full_name, 
+        repo, 
         installation_id, 
         snippet_paths=[snippet.file_path for snippet in snippets]
     )
     for file_path in tqdm(file_list):
         if file_path in query:
             try:
                 file_contents = get_file_contents(repo, file_path, ref=branch)
-                if (
-                    total_file_contents > sweep_config.max_file_limit
-                ):  # more than 10000 tokens
+                if len(file_contents) > sweep_config.max_file_limit:  # more than 10000 tokens
                     logger.warning(f"Skipping {file_path}, too many tokens")
                     continue
-                else:
-                    total_file_contents += len(file_contents)
             except github.UnknownObjectException as e:
                 logger.warning(f"Error: {e}")
                 logger.warning(f"Skipping {file_path}")
             else:
-                snippets.append(
+                snippets = [
                     Snippet(
                         content=file_contents,
                         start=0,
                         end=file_contents.count("\n") + 1,
                         file_path=file_path,
                     )
-                )
+                ] + snippets
     snippets = [snippet.expand() for snippet in snippets]
     if include_tree:
         return snippets, tree
     else:
         return snippets
```

### Comparing `sweepai-0.2.9/sweepai/utils/huggingface.py` & `sweepai-0.3.0/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/prompt_constructor.py` & `sweepai-0.3.0/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/scorer.py` & `sweepai-0.3.0/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/snippets.py` & `sweepai-0.3.0/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/sweepai/utils/utils.py` & `sweepai-0.3.0/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.9/setup.py` & `sweepai-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 packages = \
 ['sweepai', 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyGithub==1.58.2',
+['GitPython>=3.1.31,<4.0.0',
+ 'PyGithub==1.58.2',
  'config-path>=1.0.3,<2.0.0',
  'gradio>=3.35.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'requests>=2.28.2,<3.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'typer>=0.9.0,<0.10.0',
  'urllib3>=2.0.3,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.9',
+    'version': '0.3.0',
     'description': 'Sweep software chores',
     'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/week" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* Automatic interactive bug fixes & feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created using PR replies & code comments\n* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
-package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
-'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
-'urllib3>=2.0.3,<3.0.0'] entry_points = \ {'console_scripts': ['sweep =
-sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.2.9', 'description': 'Sweep software
-chores', 'long_description': '\n
+package_data = \ {'': ['*']} install_requires = \ ['GitPython>=3.1.31,<4.0.0',
+'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0',
+'loguru>=0.6.0,<0.7.0', 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0',
+'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0'] entry_points = \
+{'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai = sweepai.app.cli:
+app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.3.0', 'description':
+'Sweep software chores', 'long_description': '\n
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
   sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
```

### Comparing `sweepai-0.2.9/PKG-INFO` & `sweepai-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.9
+Version: 0.3.0
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.9 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.3.0 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyGithub
-(==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0) Requires-Dist: gradio
-(>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
-requests (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-
-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Project-
-URL: Bug Tracker, https://github.com/sweepai/sweep/issues Project-URL:
-Community, https://discord.gg/sweep-ai Project-URL: documentation, https://
-docs.sweep.dev Project-URL: homepage, https://sweep.dev Project-URL:
-repository, https://github.com/sweepai/sweep Description-Content-Type: text/
-markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
+(>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
+(>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
+(>=0.6.0,<0.7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
+tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
+Dist: urllib3 (>=2.0.3,<3.0.0) Project-URL: Bug Tracker, https://github.com/
+sweepai/sweep/issues Project-URL: Community, https://discord.gg/sweep-ai
+Project-URL: documentation, https://docs.sweep.dev Project-URL: homepage,
+https://sweep.dev Project-URL: repository, https://github.com/sweepai/sweep
+Description-Content-Type: text/markdown
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
  ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/week] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
```

