# Comparing `tmp/piou-0.9.7.tar.gz` & `tmp/piou-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piou-0.9.7.tar", max compression
+gzip compressed data, was "piou-0.9.8.tar", max compression
```

## Comparing `piou-0.9.7.tar` & `piou-0.9.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1081 2022-04-23 14:47:10.962634 piou-0.9.7/LICENSE
--rw-r--r--   0        0        0     8822 2022-04-23 14:47:10.962634 piou-0.9.7/README.md
--rw-r--r--   0        0        0      148 2022-04-23 14:47:10.962634 piou-0.9.7/piou/__init__.py
--rw-r--r--   0        0        0     4427 2022-04-23 14:47:10.966634 piou-0.9.7/piou/cli.py
--rw-r--r--   0        0        0     9758 2022-04-23 14:47:10.966634 piou-0.9.7/piou/command.py
--rw-r--r--   0        0        0     1591 2022-04-23 14:47:10.966634 piou-0.9.7/piou/exceptions.py
--rw-r--r--   0        0        0       70 2022-04-23 14:47:10.966634 piou-0.9.7/piou/formatter/__init__.py
--rw-r--r--   0        0        0     3902 2022-04-23 14:47:10.966634 piou-0.9.7/piou/formatter/base.py
--rw-r--r--   0        0        0     9505 2022-04-23 14:47:10.966634 piou-0.9.7/piou/formatter/rich_formatter.py
--rw-r--r--   0        0        0        0 2022-04-23 14:47:10.966634 piou-0.9.7/piou/test/__init__.py
--rw-r--r--   0        0        0     2282 2022-04-23 14:47:10.966634 piou-0.9.7/piou/test/__main__.py
--rw-r--r--   0        0        0      781 2022-04-23 14:47:10.966634 piou-0.9.7/piou/test/derived.py
--rw-r--r--   0        0        0      619 2022-04-23 14:47:10.966634 piou-0.9.7/piou/test/simple.py
--rw-r--r--   0        0        0    11644 2022-04-23 14:47:10.966634 piou-0.9.7/piou/utils.py
--rw-r--r--   0        0        0      865 2022-04-23 14:47:10.966634 piou-0.9.7/pyproject.toml
--rw-r--r--   0        0        0    10008 2022-04-23 14:47:11.782739 piou-0.9.7/setup.py
--rw-r--r--   0        0        0     9474 2022-04-23 14:47:11.783281 piou-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-05-17 13:33:25.014959 piou-0.9.8/LICENSE
+-rw-r--r--   0        0        0     8822 2022-05-17 13:33:25.014959 piou-0.9.8/README.md
+-rw-r--r--   0        0        0      148 2022-05-17 13:33:25.018959 piou-0.9.8/piou/__init__.py
+-rw-r--r--   0        0        0     4426 2022-05-17 13:33:25.018959 piou-0.9.8/piou/cli.py
+-rw-r--r--   0        0        0     9758 2022-05-17 13:33:25.018959 piou-0.9.8/piou/command.py
+-rw-r--r--   0        0        0     1591 2022-05-17 13:33:25.018959 piou-0.9.8/piou/exceptions.py
+-rw-r--r--   0        0        0       70 2022-05-17 13:33:25.018959 piou-0.9.8/piou/formatter/__init__.py
+-rw-r--r--   0        0        0     3902 2022-05-17 13:33:25.018959 piou-0.9.8/piou/formatter/base.py
+-rw-r--r--   0        0        0     9505 2022-05-17 13:33:25.018959 piou-0.9.8/piou/formatter/rich_formatter.py
+-rw-r--r--   0        0        0        0 2022-05-17 13:33:25.018959 piou-0.9.8/piou/test/__init__.py
+-rw-r--r--   0        0        0     2282 2022-05-17 13:33:25.018959 piou-0.9.8/piou/test/__main__.py
+-rw-r--r--   0        0        0      781 2022-05-17 13:33:25.018959 piou-0.9.8/piou/test/derived.py
+-rw-r--r--   0        0        0      619 2022-05-17 13:33:25.018959 piou-0.9.8/piou/test/simple.py
+-rw-r--r--   0        0        0    11661 2022-05-17 13:33:25.018959 piou-0.9.8/piou/utils.py
+-rw-r--r--   0        0        0      865 2022-05-17 13:33:25.018959 piou-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    10008 2022-05-17 13:33:26.039449 piou-0.9.8/setup.py
+-rw-r--r--   0        0        0     9474 2022-05-17 13:33:26.040114 piou-0.9.8/PKG-INFO
```

### Comparing `piou-0.9.7/LICENSE` & `piou-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/README.md` & `piou-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/cli.py` & `piou-0.9.8/piou/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     follows the boolean
     """
     on_cmd_run: Optional[OnCommandRun] = None
     """ Function called before running the actual function.
     For instance, you can use this to get the arguments passed
     for monitoring
     """
-
     _group: CommandGroup = field(init=False, default_factory=CommandGroup)
 
     _loop: asyncio.AbstractEventLoop = field(init=False, default_factory=get_loop)
 
     def __post_init__(self):
         self._group.description = clean_multiline(self.description) if self.description else None
         self._group.propagate_options = self.propagate_options
```

### Comparing `piou-0.9.7/piou/command.py` & `piou-0.9.8/piou/command.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/exceptions.py` & `piou-0.9.8/piou/exceptions.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/formatter/base.py` & `piou-0.9.8/piou/formatter/base.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/formatter/rich_formatter.py` & `piou-0.9.8/piou/formatter/rich_formatter.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/test/__main__.py` & `piou-0.9.8/piou/test/__main__.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/test/derived.py` & `piou-0.9.8/piou/test/derived.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/test/simple.py` & `piou-0.9.8/piou/test/simple.py`

 * *Files identical despite different names*

### Comparing `piou-0.9.7/piou/utils.py` & `piou-0.9.8/piou/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,19 +242,18 @@
 
 
 KeywordParam = namedtuple('KeywordParam', ['name', 'validate'])
 
 
 def convert_args_to_dict(input_args: list[str],
                          options: list[CommandOption]) -> dict:
-    _input_pos_args, _input_keyword_args = get_cmd_args(' '.join(input_args),
+    _input_pos_args, _input_keyword_args = get_cmd_args(' '.join(f'"{x}"' for x in input_args),
                                                         {name: opt.data_type
                                                          for opt in options
                                                          for name in opt.names})
-
     positional_args, keyword_args = [], {}
     for _arg in options:
         if _arg.is_positional_arg:
             positional_args.append(_arg)
         for _keyword_arg in _arg.keyword_args:
             keyword_args[_keyword_arg] = KeywordParam(_arg.name, _arg.validate)
```

### Comparing `piou-0.9.7/pyproject.toml` & `piou-0.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "piou"
-version = "0.9.7"
+version = "0.9.8"
 description = "A CLI toolkit"
 authors = ["Julien Brayere <julien.brayere@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andarius/piou"
 repository = "https://github.com/andarius/piou"
 keywords = ["cli"]
```

### Comparing `piou-0.9.7/setup.py` & `piou-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['rich>=10.11.0,<13.0']
 
 setup_kwargs = {
     'name': 'piou',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'A CLI toolkit',
     'long_description': '[<img src="https://github.com/Andarius/piou/raw/dev/docs/piou.jpg" width="250"/>](docs/piou.png)\n\n# Piou\n\n[![Python versions](https://img.shields.io/pypi/pyversions/piou)](https://pypi.python.org/pypi/piou)\n[![Latest PyPI version](https://img.shields.io/pypi/v/piou?logo=pypi)](https://pypi.python.org/pypi/piou)\n[![CircleCI](https://circleci.com/gh/Andarius/piou/tree/master.svg?style=shield)](https://app.circleci.com/pipelines/github/Andarius/piou?branch=master)\n[![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/piou?logo=conda-forge)](https://anaconda.org/conda-forge/piou)\n\nA CLI tool to build beautiful command-line interfaces with type validation.\n\nIt is as simple as\n\n```python\nfrom piou import Cli, Option\n\ncli = Cli(description=\'A CLI tool\')\n\n\n@cli.command(cmd=\'foo\', help=\'Run foo command\')\ndef foo_main(\n        bar: int = Option(..., help=\'Bar positional argument (required)\'),\n        baz: str = Option(..., \'-b\', \'--baz\', help=\'Baz keyword argument (required)\'),\n        foo: str = Option(None, \'--foo\', help=\'Foo keyword argument\'),\n):\n    """\n    A longer description on what the function is doing.\n    You can run it with:\n    ```bash\n     poetry run python -m piou.test.simple foo 1 -b baz\n    ```\n    And you are good to go!\n    """\n    pass\n\n\nif __name__ == \'__main__\':\n    cli.run()\n```\n\nThe output will look like this:\n\n- `python -m piou.test.simple -h`\n\n![example](https://github.com/Andarius/piou/raw/master/docs/simple-output.png)\n\n- `python -m piou.test.simple foo -h`\n\n![example](https://github.com/Andarius/piou/raw/master/docs/simple-output-foo.png)\n\n# Why ?\n\nI could not find a library that provided:\n\n- the same developer experience than [FastAPI](https://fastapi.tiangolo.com/)\n- customization of the interface (to build a CLI similar to the one of [Poetry](https://python-poetry.org/))\n- type validation / casting\n\n[Typer](https://github.com/tiangolo/typer) is the closest alternative in terms of experience but lacks the possibility\nto format the output is a custom way using external libraries (like [Rich](https://github.com/Textualize/rich)).\n\n**Piou** provides all these possibilities and lets you define your own [Formatter](#custom-formatter).\n\n# Install\n\nYou can install `piou` with either:\n\n- `pip install piou`\n- `conda install piou -c conda-forge`\n\n# Features\n\n## Commands\n\n```python\nfrom piou import Cli, Option\n\ncli = Cli(description=\'A CLI tool\')\n\n\n@cli.command(cmd=\'foo\',\n             help=\'Run foo command\')\ndef foo_main(\n        foo1: int = Option(..., help=\'Foo arguments\'),\n        foo2: str = Option(..., \'-f\', \'--foo2\', help=\'Foo2 arguments\'),\n        foo3: str = Option(None, \'-g\', \'--foo3\', help=\'Foo3 arguments\'),\n):\n    pass\n\n\n@cli.command(cmd=\'bar\',\n             help=\'Run bar command\')\ndef bar_main(\n        foo1: int = Option(..., help=\'Foo arguments\'),\n        foo2: str = Option(..., \'-f\', \'--foo2\', help=\'Foo2 arguments\'),\n        foo3: str = Option(None, \'-g\', \'--foo3\', help=\'Foo3 arguments\'),\n):\n    pass\n\n\nif __name__ == \'__main__\':\n    cli.run()\n```\n\nIn this case, `foo1` is a positional argument while `foo2` and `foo3` are keyword arguments.\n\nYou can optionally specify global options that will be passed to all commands:\n\n```python\ncli = Cli(description=\'A CLI tool\')\n\ncli.add_option(\'-q\', \'--quiet\', help=\'Do not output any message\')\n```\n\nThe **description** can also be extracted from the function docstring. Both functions here return the same description.\n\n```python\n@cli.command(cmd=\'bar\', description=\'Run foo command\')\ndef bar_main():\n    pass\n\n\n@cli.command(cmd=\'bar2\')\ndef bar_2_main():\n    """\n    Run foo command\n    """\n    pass\n```\n\nA command can also be asynchronous, it will be run automatically using `asyncio.run`.\n\n```python\n@cli.command(cmd=\'bar\', help=\'Run foo command\')\nasync def bar_main():\n    pass\n```\n\n## Command Groups / Sub-commands\n\nYou can group commands into sub-commands:\n\n```python\nfrom piou import Cli, Option\n\ncli = Cli(description=\'A CLI tool\')\n\n\n@cli.command(cmd=\'foo\', help=\'Run foo command\')\ndef foo_main():\n    pass\n\n\nsub_cmd = cli.add_sub_parser(cmd=\'sub\', help=\'A sub command\')\nsub_cmd.add_option(\'--test\', help=\'Test mode\')\n\n\n@sub_cmd.command(cmd=\'bar\', help=\'Run bar command\')\ndef sub_bar_main(**kwargs):\n    pass\n\n\n@sub_cmd.command(cmd=\'foo\', help=\'Run foo command\')\ndef sub_foo_main(\n        test: bool,\n        foo1: int = Option(..., help=\'Foo argument\'),\n        foo2: str = Option(..., \'-f\', \'--foo2\', help=\'Foo2 argument\'),\n):\n    pass\n\n\nif __name__ == \'__main__\':\n    cli.run()\n```\n\nSo when running `python run.py sub -h` it will output the following:\n\n![example](https://github.com/Andarius/piou/raw/master/docs/sub-cmd-output.png)\n\n## Options processor\n\nSometimes, you want to run a function using the global arguments before running the actual command (for instance\ninitialize a logger based on the `verbose` level).\n\nTo do so, you use `set_options_processor` that will receive all the current global options of the CLI.\n\n```python\nfrom piou import Cli\n\ncli = Cli(description=\'A CLI tool\')\n\ncli.add_option(\'--verbose\', help=\'Increase verbosity\')\n\n\ndef processor(verbose: bool):\n    print(f\'Processing {verbose=}\')\n\n\ncli.set_options_processor(processor)\n```\n\nYou can also use the decorator syntax:\n\n```python\nfrom piou import Cli, Option\n\ncli = Cli(description=\'A CLI tool\')\n\n\n@cli.processor()\ndef processor(verbose: bool = Option(False, \'--verbose\', help=\'Increase verbosity\')):\n    print(f\'Processing {verbose=}\')\n```\n\nBy default, when a processor is set, the global arguments will not be passed downstream.\nIf you still want them to be passed to the functions by setting\n\n```python\ncli = Cli(description=\'A CLI tool\', propagate_options=True)\n```\n\nor in the case of a **sub-command**\n\n```python\ncli.add_sub_parser(cmd=\'sub\', help=\'A sub command\', propagate_options=True)\n```\n\n## Derived Options\n\nSometimes, you want to reuse the options in multiple command and group them into a single output to pass to\nthe command. For instance, you might want to group a connection string parameter to connect to a database. Here is a\nfull example:\n\n```python\nfrom piou import Cli, Option, Derived\nimport psycopg2\n\ncli = Cli(description=\'A CLI tool\')\n\n\ndef get_pg_conn(\n        pg_user: str = Option(\'postgres\', \'--pg-user\'),\n        pg_pwd: str = Option(\'postgres\', \'--pg-pwd\'),\n        pg_host: str = Option(\'localhost\', \'--pg-host\'),\n        pg_port: int = Option(5432, \'--pg-port\'),\n        pg_db: str = Option(\'postgres\', \'--pg-db\')\n\n):\n    conn = psycopg2.connect(dbname=pg_db, user=pg_user, password=pg_pwd,\n                            host=pg_host, port=pg_port)\n    return conn\n\n\n@cli.command(help=\'Run foo command\')\ndef foo(pg_conn: str = Derived(get_pg_conn)):\n    ...\n\n\n@cli.command(help=\'Run bar command\')\ndef bar(pg_conn: str = Derived(get_pg_conn)):\n    ...\n```\n\n## On Command Run\n\nIf you want to get the command name and arguments information that are passed to it (in case of general purpose\ndebugging for instance), you can pass `on_cmd_run` to the CLI.\n\n```python\nfrom piou import Cli, Option, CommandMeta, Derived\n\n\ndef on_cmd_run(meta: CommandMeta):\n    pass\n\n\ncli = Cli(description=\'A CLI tool\',\n          on_cmd_run=on_cmd_run)\n\n\ndef processor(a: int = Option(1, \'-a\'),\n              b: int = Option(2, \'-b\')):\n    return a + b\n\n\n@cli.command()\ndef test(\n        value: int = Derived(processor),\n        bar: str = Option(None, \'--bar\')\n):\n    pass\n```\n\nIn this case, `meta` will be equal to:\n\n```python\nCommandMeta(cmd_name=\'test\',\n            fn_args={\'bar\': \'bar\', \'value\': 5},\n            cmd_args={\'a\': 3, \'b\': 2, \'bar\': \'bar\'})\n```\n\n## Help / Errors Formatter\n\nYou can customize the help and the different errors displayed by the CLI by passing a Formatter.\nThe default one is the **Rich formatter** based on the [Rich](https://github.com/Textualize/rich) package:\n\n- `cmd_color`: set the color of the command in the help\n- `option_color`: set the color of the positional / keyword arguments in the help\n- `show_default`: show the default values if the keyword arguments (if available)\n\nYou can create your own Formatter by subclassing the `Formatter` class (see\nthe [Rich formatter](https://github.com/Andarius/piou/blob/master/piou/formatter/rich_formatter.py)\nfor example).\n\n## Complete example\n\nYou can try a more complete example by running `python -m piou.test -h`\n\n## Moving from `argparse`\n\nIf you are migrating code from `argparse` to `piou` here are some differences:\n\n**choices**:\n`add_argument(\'--pick\', choices=[\'foo\', \'bar\'])` can be replaced by\n`pick: Literal[\'foo\', \'bar\'] = Option(None, \'--pick\')`.\n\nYou can also disable the case sensitivity by passing `Option(None, \'--pick\', case_sentitive=False)`\n\n**action=store_true**\n`add_argument(\'--verbose\', action=\'store_true\')` can be replaced by\n`verbose: bool = Option(False, \'--verbose\')`\n',
     'author': 'Julien Brayere',
     'author_email': 'julien.brayere@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/andarius/piou',
```

### Comparing `piou-0.9.7/PKG-INFO` & `piou-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piou
-Version: 0.9.7
+Version: 0.9.8
 Summary: A CLI toolkit
 Home-page: https://github.com/andarius/piou
 License: MIT
 Keywords: cli
 Author: Julien Brayere
 Author-email: julien.brayere@gmail.com
 Requires-Python: >=3.9,<4.0
```

