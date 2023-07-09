# Comparing `tmp/conplex_dti-0.1.4.tar.gz` & `tmp/conplex_dti-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conplex_dti-0.1.4.tar", max compression
+gzip compressed data, was "conplex_dti-0.1.5.tar", max compression
```

## Comparing `conplex_dti-0.1.4.tar` & `conplex_dti-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.4/LICENSE
--rw-r--r--   0        0        0     4227 2023-06-14 20:00:03.673625 conplex_dti-0.1.4/README.md
--rw-r--r--   0        0        0     3510 2023-06-14 01:47:41.847038 conplex_dti-0.1.4/conplex_dti/MAIN_OLD.txt
--rw-r--r--   0        0        0      399 2023-06-14 01:47:41.848725 conplex_dti-0.1.4/conplex_dti/__init__.py
--rw-r--r--   0        0        0     1070 2023-06-14 01:47:41.850137 conplex_dti-0.1.4/conplex_dti/__main__.py
--rw-r--r--   0        0        0    23714 2023-06-14 01:47:41.852511 conplex_dti-0.1.4/conplex_dti/architectures.py
--rw-r--r--   0        0        0      166 2023-06-14 01:47:41.854260 conplex_dti-0.1.4/conplex_dti/cli/__init__.py
--rw-r--r--   0        0        0     3802 2023-06-14 20:00:03.676732 conplex_dti-0.1.4/conplex_dti/cli/download.py
--rw-r--r--   0        0        0    19563 2023-06-14 20:00:03.678325 conplex_dti-0.1.4/conplex_dti/cli/train.py
--rw-r--r--   0        0        0      171 2023-06-14 01:47:41.895917 conplex_dti-0.1.4/conplex_dti/dataset/__init__.py
--rw-r--r--   0        0        0    24300 2023-06-14 20:00:03.680200 conplex_dti-0.1.4/conplex_dti/dataset/datamodules.py
--rw-r--r--   0        0        0      421 2023-06-14 01:47:41.919180 conplex_dti-0.1.4/conplex_dti/featurizer/__init__.py
--rw-r--r--   0        0        0     7765 2023-06-14 20:00:03.681608 conplex_dti-0.1.4/conplex_dti/featurizer/base.py
--rw-r--r--   0        0        0    11422 2023-06-14 01:47:41.958730 conplex_dti-0.1.4/conplex_dti/featurizer/molecule.py
--rw-r--r--   0        0        0    11493 2023-06-14 01:47:41.996784 conplex_dti-0.1.4/conplex_dti/featurizer/protein.py
--rw-r--r--   0        0        0        0 2023-06-14 01:47:41.997856 conplex_dti-0.1.4/conplex_dti/model/__init__.py
--rw-r--r--   0        0        0    23789 2023-06-14 01:47:42.015759 conplex_dti-0.1.4/conplex_dti/model/architectures.py
--rw-r--r--   0        0        0     2125 2023-06-14 01:47:42.044312 conplex_dti-0.1.4/conplex_dti/model/margin.py
--rw-r--r--   0        0        0     4022 2023-06-14 01:47:42.059531 conplex_dti-0.1.4/conplex_dti/utils.py
--rw-r--r--   0        0        0     4177 2023-06-14 20:00:03.689428 conplex_dti-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 conplex_dti-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     4831 2023-07-09 05:21:18.075778 conplex_dti-0.1.5/README.md
+-rw-r--r--   0        0        0     3510 2023-06-14 01:47:41.847038 conplex_dti-0.1.5/conplex_dti/MAIN_OLD.txt
+-rw-r--r--   0        0        0      399 2023-06-14 01:47:41.848725 conplex_dti-0.1.5/conplex_dti/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-09 05:21:18.079836 conplex_dti-0.1.5/conplex_dti/__main__.py
+-rw-r--r--   0        0        0    23714 2023-06-14 01:47:41.852511 conplex_dti-0.1.5/conplex_dti/architectures.py
+-rw-r--r--   0        0        0      251 2023-07-09 05:21:18.081792 conplex_dti-0.1.5/conplex_dti/cli/__init__.py
+-rw-r--r--   0        0        0     3859 2023-07-09 05:21:15.929266 conplex_dti-0.1.5/conplex_dti/cli/download.py
+-rw-r--r--   0        0        0     4037 2023-07-09 05:21:18.083732 conplex_dti-0.1.5/conplex_dti/cli/predict.py
+-rw-r--r--   0        0        0    19588 2023-07-09 05:21:15.932012 conplex_dti-0.1.5/conplex_dti/cli/train.py
+-rw-r--r--   0        0        0      171 2023-07-09 05:21:15.934053 conplex_dti-0.1.5/conplex_dti/dataset/__init__.py
+-rw-r--r--   0        0        0    24300 2023-07-09 05:21:15.936761 conplex_dti-0.1.5/conplex_dti/dataset/datamodules.py
+-rw-r--r--   0        0        0      421 2023-06-14 01:47:41.919180 conplex_dti-0.1.5/conplex_dti/featurizer/__init__.py
+-rw-r--r--   0        0        0     7765 2023-06-14 20:00:03.681608 conplex_dti-0.1.5/conplex_dti/featurizer/base.py
+-rw-r--r--   0        0        0    11422 2023-06-14 01:47:41.958730 conplex_dti-0.1.5/conplex_dti/featurizer/molecule.py
+-rw-r--r--   0        0        0    11493 2023-06-14 01:47:41.996784 conplex_dti-0.1.5/conplex_dti/featurizer/protein.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:47:41.997856 conplex_dti-0.1.5/conplex_dti/model/__init__.py
+-rw-r--r--   0        0        0    23789 2023-06-14 01:47:42.015759 conplex_dti-0.1.5/conplex_dti/model/architectures.py
+-rw-r--r--   0        0        0     2125 2023-06-14 01:47:42.044312 conplex_dti-0.1.5/conplex_dti/model/margin.py
+-rw-r--r--   0        0        0     4022 2023-06-14 01:47:42.059531 conplex_dti-0.1.5/conplex_dti/utils.py
+-rw-r--r--   0        0        0     4195 2023-07-09 05:24:58.151833 conplex_dti-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6472 1970-01-01 00:00:00.000000 conplex_dti-0.1.5/PKG-INFO
```

### Comparing `conplex_dti-0.1.4/LICENSE` & `conplex_dti-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/README.md` & `conplex_dti-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 # ConPLex
 
 ![ConPLex Schematic](assets/images/Fig2_Schematic.png)
 
 [![ConPLex Releases](https://img.shields.io/github/v/release/samsledje/ConPLex?include_prereleases)](https://github.com/samsledje/ConPLex/releases)
 [![PyPI](https://img.shields.io/pypi/v/conplex-dti)](https://pypi.org/project/conplex-dti/)
-[![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=main)](https://conplex.readthedocs.io/en/main/?badge=main)
+[![Build](https://github.com/samsledje/ConPLex/actions/workflows/build.yml/badge.svg)](https://github.com/samsledje/ConPLex/actions/workflows/build.yml)
+[![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=latest)](https://conplex.readthedocs.io/en/main/?badge=main)
 [![License](https://img.shields.io/github/license/samsledje/ConPLex)](https://github.com/samsledje/ConPLex/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-🚧🚧 Please note that ConPLex v0.1.0 is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
+🚧🚧 Please note that ConPLex is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
 
  - [Homepage](http://conplex.csail.mit.edu)
  - [Documentation](https://d-script.readthedocs.io/en/main/)
 
 ## Abstract
 
 Sequence-based prediction of drug-target interactions has the potential to accelerate drug discovery by complementing experimental screens. Such computational prediction needs to be generalizable and scalable while remaining sensitive to subtle variations in the inputs. However, current computational techniques fail to simultaneously meet these goals, often sacrificing performance on one to achieve the others. We develop a deep learning model, ConPLex, successfully leveraging the advances in pre-trained protein language models ("PLex") and employing  a novel  protein-anchored contrastive co-embedding ("Con") to outperform state-of-the-art approaches. ConPLex achieves high accuracy, broad adaptivity to unseen data, and specificity against decoy compounds. It makes predictions of binding based on the distance between learned representations, enabling predictions at the scale of massive compound libraries and the human proteome. Experimental testing of 19 kinase-drug interaction predictions validated 12 interactions, including four with sub-nanomolar affinity, plus a novel strongly-binding EPHB1 inhibitor ($K_D = 1.3nM$). Furthermore, ConPLex embeddings are interpretable, which enables us to visualize the drug-target embedding space and use embeddings to characterize the function of human cell-surface proteins. We anticipate ConPLex will facilitate novel drug discovery by making highly sensitive in-silico drug screening feasible at genome scale.
 
 ## Installation
 
 ### Install from PyPI
 
+You should first have a version of [`cudatoolkit`](https://anaconda.org/nvidia/cudatoolkit) compatible with your system installed. Then run
+
 ```bash
 pip install conplex-dti
 conplex-dti --help
 ```
 
 ### Compile from Source
 
 ```bash
 git clone https://github.com/samsledje/ConPLex.git
 cd ConPLex
 conda create -n conplex-dti python=3.9
 conda activate conplex-dti
 make poetry-download
-export PATH=[poetry install location]:PATH
+export PATH="[poetry  install  location]:$PATH"
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 make install
 conplex-dti --help
 ```
 
 ## Usage
 
-### Download benchmark data sets
+### Download benchmark data sets and pre-trained models
+
+```bash
+conplex-dti download --to datasets --benchmarks davis bindingdb biosnap biosnap_prot biosnap_mol dude
+```
 
 ```bash
-conplex-dti download --to datasets --benchmarks davis bindingdb biosnap biosnap_prot biosnap_mol --models ConPLex_v1_BindingDB
+conplex-dti download --to models --models ConPLex_v1_BindingDB
 ```
 
 ### Run benchmark training
 
 ```bash
 conplex-dti train --run-id TestRun --config config/default_config.yaml
 ```
 
 ### Make predictions with a trained model
 
 ```bash
-...
+conplex-dti predict --data-file [pair predict file].tsv --model-path ./models/ConPLex_v1_BindingDB.pt --outfile ./results.tsv
 ```
 
+Format of `[pair predict file].tsv` should be `[protein ID]\t[molecule ID]\t[protein Sequence]\t[molecule SMILES]`
+
 ### Visualize co-embedding space
 
 ```bash
 ...
 ```
 
 ## Reference
 
-If you use ConPLex, please cite [Contrastive learning in protein language space predicts interactions between drugs and protein targets]("https://www.pnas.org/doi/10.1073/pnas.2220778120") by Rohit Singh*, Samuel Sledzieski*, Bryan Bryson, Lenore Cowen and Bonnie Berger, currently in press at PNAS.
+If you use ConPLex, please cite [Contrastive learning in protein language space predicts interactions between drugs and protein targets](https://www.pnas.org/doi/10.1073/pnas.2220778120) by Rohit Singh*, Samuel Sledzieski*, Bryan Bryson, Lenore Cowen and Bonnie Berger, currently in press at PNAS.
 
 ```bash
 @article{singh2023contrastive,
   title={Contrastive learning in protein language space predicts interactions between drugs and protein targets},
   author={Singh, Rohit and Sledzieski, Samuel and Bryson, Bryan and Cowen, Lenore and Berger, Bonnie},
   journal={Proceedings of the National Academy of Sciences},
   volume={120},
```

### Comparing `conplex_dti-0.1.4/conplex_dti/MAIN_OLD.txt` & `conplex_dti-0.1.5/conplex_dti/MAIN_OLD.txt`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/__main__.py` & `conplex_dti-0.1.5/conplex_dti/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     subparsers.required = True
 
     modules = {
         "train": (cli.train, cli.train_parser),
         "download": (cli.download, cli.download_parser),
         # "embed": embed,
         # "evaluate": evaluate,
-        # "predict": predict,
+        "predict": (cli.predict, cli.predict_parser),
     }
 
     for name, (main_func, args_func) in modules.items():
         sp = subparsers.add_parser(name, description=main_func.__doc__)
         args_func(sp)
         sp.set_defaults(main_func=main_func)
```

### Comparing `conplex_dti-0.1.4/conplex_dti/architectures.py` & `conplex_dti-0.1.5/conplex_dti/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/cli/download.py` & `conplex_dti-0.1.5/conplex_dti/cli/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
-import sys
 import shutil
+import sys
 import urllib.request
-from functools import wraps, partial
 from argparse import ArgumentParser
+from functools import partial, wraps
 from pathlib import Path
 
-from ..utils import config_logger, get_logger
 from ..dataset import get_task_dir
+from ..utils import config_logger, get_logger
 
 logg = config_logger(
     None, "%(asctime)s [%(levelname)s] %(message)s", level=2, use_stdout=True
 )
 
 
 def get_remote_path(bm: str):
@@ -42,15 +42,15 @@
         choices=[
             "davis",
             "bindingdb",
             "biosnap",
             "biosnap_prot",
             "biosnap_mol",
             "dude",
-#            "dti_dg",
+            #            "dti_dg",
         ],
         help="Benchmarks to download.",
     )
 
     parser.add_argument(
         "--models",
         type=str,
@@ -58,58 +58,66 @@
         choices=["ConPLex_v1_BindingDB"],
         help="Pre-trained ConPLex models to download.",
     )
 
     return parser
 
 
-def download_safe(remote_path: str, local_path: str, key: str = "file", verbose: bool = True) -> str:
+def download_safe(
+    remote_path: str, local_path: str, key: str = "file", verbose: bool = True
+) -> str:
     if not os.path.exists(local_path):
         try:
             if verbose:
                 logg.info(f"Downloading {key} from {remote_path} to {local_path}...")
             with urllib.request.urlopen(remote_path) as response, open(
                 local_path, "wb"
             ) as out_file:
                 shutil.copyfileobj(response, out_file)
         except Exception as e:
             logg.error(f"Unable to download {key} - {e}")
             sys.exit(1)
     return local_path
 
+
 def main(args):
     args.to = Path(args.to).absolute()
     logg.info(f"Download Location: {args.to}")
     logg.info("")
 
     logg.info("[BENCHMARKS]")
     benchmarks = args.benchmarks or []
     for bm in benchmarks:
         logg.info(f"Downloading {bm}...")
-        task_dir = Path(get_task_dir(bm, database_root = args.to))
-        os.makedirs(task_dir, exist_ok = True)
-        
+        task_dir = Path(get_task_dir(bm, database_root=args.to))
+        os.makedirs(task_dir, exist_ok=True)
+
         if bm == "dude":
-            fi_list = ["full.tsv", "dude_cross_type_train_test_split.csv", "dude_within_type_train_test_split.csv"]
+            fi_list = [
+                "full.tsv",
+                "dude_cross_type_train_test_split.csv",
+                "dude_within_type_train_test_split.csv",
+            ]
         else:
             fi_list = ["train.csv", "val.csv", "test.csv"]
-        
+
         for fi in fi_list:
             local_path = task_dir / fi
             remote_base = get_remote_path(bm)
             remote_path = f"{remote_base}/{fi}"
-            download_safe(remote_path, local_path, key = f"{bm}/{fi}")
+            download_safe(remote_path, local_path, key=f"{bm}/{fi}")
 
     logg.info("[MODELS]")
     models = args.models or []
     for mo in models:
         model_dir = args.to / "models"
-        os.makedirs(model_dir, exist_ok = True)
+        os.makedirs(model_dir, exist_ok=True)
         local_path = (model_dir / mo).with_suffix(".pt")
         remote_path = get_remote_path(mo)
-        download_safe(remote_path, local_path, key = mo)
+        download_safe(remote_path, local_path, key=mo)
+
 
 if __name__ == "__main__":
     parser = ArgumentParser()
     parser = add_args(parser)
     args = parser.parse_args()
     main(args)
```

### Comparing `conplex_dti-0.1.4/conplex_dti/cli/train.py` & `conplex_dti-0.1.5/conplex_dti/cli/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from pathlib import Path
 from time import time
 
 import numpy as np
 import pandas as pd
 import torch
 import torchmetrics
+import wandb
 from omegaconf import OmegaConf
 from torch import nn
 from torch.autograd import Variable
 from torch.utils import data
 from tqdm.auto import tqdm
 
-import wandb
-
 from ..dataset import (
     DTIDataModule,
     DUDEDataModule,
     EnzPredDataModule,
     TDCDataModule,
     get_task_dir,
 )
@@ -327,19 +326,21 @@
     training_generator = datamodule.train_dataloader()
     validation_generator = datamodule.val_dataloader()
     testing_generator = datamodule.test_dataloader()
 
     if config.contrastive:
         logg.info("Loading contrastive data (DUDE)")
         dude_drug_featurizer = get_featurizer(
-            config.drug_featurizer, save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir)
+            config.drug_featurizer,
+            save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir),
         )
 
         dude_target_featurizer = get_featurizer(
-            config.target_featurizer, save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir)
+            config.target_featurizer,
+            save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir),
         )
 
         contrastive_datamodule = DUDEDataModule(
             get_task_dir("DUDe", database_root=config.data_cache_dir),
             config.contrastive_split,
             dude_drug_featurizer,
             dude_target_featurizer,
```

### Comparing `conplex_dti-0.1.4/conplex_dti/dataset/datamodules.py` & `conplex_dti-0.1.5/conplex_dti/dataset/datamodules.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/featurizer/base.py` & `conplex_dti-0.1.5/conplex_dti/featurizer/base.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/featurizer/molecule.py` & `conplex_dti-0.1.5/conplex_dti/featurizer/molecule.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/featurizer/protein.py` & `conplex_dti-0.1.5/conplex_dti/featurizer/protein.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/model/architectures.py` & `conplex_dti-0.1.5/conplex_dti/model/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/model/margin.py` & `conplex_dti-0.1.5/conplex_dti/model/margin.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/conplex_dti/utils.py` & `conplex_dti-0.1.5/conplex_dti/utils.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.4/pyproject.toml` & `conplex_dti-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conplex-dti"
-version = "0.1.4"
+version = "0.1.5"
 description = "Adapting protein language models and contrastive learning for DTI prediction."
 readme = "README.md"
 authors = ["samsledje <samsl@mit.edu>"]
 license = "MIT"
 repository = "https://github.com/samsledje/ConPLex"
 homepage = "https://github.com/samsledje/ConPLex"
 
@@ -43,14 +43,15 @@
 omegaconf = "^2.3.0"
 rdkit = "^2022.9.5"
 fair-esm = "^0.1.0"
 transformers = "^4.26.1"
 PyTDC = "^0.3.9"
 typer = {extras = ["all"], version = "^0.4.0"}
 rich = "^13.3.2"
+numpy = "^1.25.1"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.1"
 black = {version = "^23.1", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^0.910"
```

### Comparing `conplex_dti-0.1.4/PKG-INFO` & `conplex_dti-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conplex-dti
-Version: 0.1.4
+Version: 0.1.5
 Summary: Adapting protein language models and contrastive learning for DTI prediction.
 Home-page: https://github.com/samsledje/ConPLex
 License: MIT
 Keywords: protein language models,contrastive learning,drug target interaction,DTI
 Author: samsledje
 Author-email: samsl@mit.edu
 Requires-Python: >=3.9,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyTDC (>=0.3.9,<0.4.0)
 Requires-Dist: fair-esm (>=0.1.0,<0.2.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: pytorch_lightning (>=1.9.3,<2.0.0)
 Requires-Dist: rdkit (>=2022.9.5,<2023.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: torchmetrics (>=0.11.3,<0.12.0)
@@ -38,79 +39,88 @@
 
 # ConPLex
 
 ![ConPLex Schematic](assets/images/Fig2_Schematic.png)
 
 [![ConPLex Releases](https://img.shields.io/github/v/release/samsledje/ConPLex?include_prereleases)](https://github.com/samsledje/ConPLex/releases)
 [![PyPI](https://img.shields.io/pypi/v/conplex-dti)](https://pypi.org/project/conplex-dti/)
-[![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=main)](https://conplex.readthedocs.io/en/main/?badge=main)
+[![Build](https://github.com/samsledje/ConPLex/actions/workflows/build.yml/badge.svg)](https://github.com/samsledje/ConPLex/actions/workflows/build.yml)
+[![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=latest)](https://conplex.readthedocs.io/en/main/?badge=main)
 [![License](https://img.shields.io/github/license/samsledje/ConPLex)](https://github.com/samsledje/ConPLex/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-🚧🚧 Please note that ConPLex v0.1.0 is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
+🚧🚧 Please note that ConPLex is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
 
  - [Homepage](http://conplex.csail.mit.edu)
  - [Documentation](https://d-script.readthedocs.io/en/main/)
 
 ## Abstract
 
 Sequence-based prediction of drug-target interactions has the potential to accelerate drug discovery by complementing experimental screens. Such computational prediction needs to be generalizable and scalable while remaining sensitive to subtle variations in the inputs. However, current computational techniques fail to simultaneously meet these goals, often sacrificing performance on one to achieve the others. We develop a deep learning model, ConPLex, successfully leveraging the advances in pre-trained protein language models ("PLex") and employing  a novel  protein-anchored contrastive co-embedding ("Con") to outperform state-of-the-art approaches. ConPLex achieves high accuracy, broad adaptivity to unseen data, and specificity against decoy compounds. It makes predictions of binding based on the distance between learned representations, enabling predictions at the scale of massive compound libraries and the human proteome. Experimental testing of 19 kinase-drug interaction predictions validated 12 interactions, including four with sub-nanomolar affinity, plus a novel strongly-binding EPHB1 inhibitor ($K_D = 1.3nM$). Furthermore, ConPLex embeddings are interpretable, which enables us to visualize the drug-target embedding space and use embeddings to characterize the function of human cell-surface proteins. We anticipate ConPLex will facilitate novel drug discovery by making highly sensitive in-silico drug screening feasible at genome scale.
 
 ## Installation
 
 ### Install from PyPI
 
+You should first have a version of [`cudatoolkit`](https://anaconda.org/nvidia/cudatoolkit) compatible with your system installed. Then run
+
 ```bash
 pip install conplex-dti
 conplex-dti --help
 ```
 
 ### Compile from Source
 
 ```bash
 git clone https://github.com/samsledje/ConPLex.git
 cd ConPLex
 conda create -n conplex-dti python=3.9
 conda activate conplex-dti
 make poetry-download
-export PATH=[poetry install location]:PATH
+export PATH="[poetry  install  location]:$PATH"
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 make install
 conplex-dti --help
 ```
 
 ## Usage
 
-### Download benchmark data sets
+### Download benchmark data sets and pre-trained models
+
+```bash
+conplex-dti download --to datasets --benchmarks davis bindingdb biosnap biosnap_prot biosnap_mol dude
+```
 
 ```bash
-conplex-dti download --to datasets --benchmarks davis bindingdb biosnap biosnap_prot biosnap_mol --models ConPLex_v1_BindingDB
+conplex-dti download --to models --models ConPLex_v1_BindingDB
 ```
 
 ### Run benchmark training
 
 ```bash
 conplex-dti train --run-id TestRun --config config/default_config.yaml
 ```
 
 ### Make predictions with a trained model
 
 ```bash
-...
+conplex-dti predict --data-file [pair predict file].tsv --model-path ./models/ConPLex_v1_BindingDB.pt --outfile ./results.tsv
 ```
 
+Format of `[pair predict file].tsv` should be `[protein ID]\t[molecule ID]\t[protein Sequence]\t[molecule SMILES]`
+
 ### Visualize co-embedding space
 
 ```bash
 ...
 ```
 
 ## Reference
 
-If you use ConPLex, please cite [Contrastive learning in protein language space predicts interactions between drugs and protein targets]("https://www.pnas.org/doi/10.1073/pnas.2220778120") by Rohit Singh*, Samuel Sledzieski*, Bryan Bryson, Lenore Cowen and Bonnie Berger, currently in press at PNAS.
+If you use ConPLex, please cite [Contrastive learning in protein language space predicts interactions between drugs and protein targets](https://www.pnas.org/doi/10.1073/pnas.2220778120) by Rohit Singh*, Samuel Sledzieski*, Bryan Bryson, Lenore Cowen and Bonnie Berger, currently in press at PNAS.
 
 ```bash
 @article{singh2023contrastive,
   title={Contrastive learning in protein language space predicts interactions between drugs and protein targets},
   author={Singh, Rohit and Sledzieski, Samuel and Bryson, Bryan and Cowen, Lenore and Berger, Bonnie},
   journal={Proceedings of the National Academy of Sciences},
   volume={120},
```

