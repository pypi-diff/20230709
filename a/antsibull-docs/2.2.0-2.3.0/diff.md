# Comparing `tmp/antsibull_docs-2.2.0.tar.gz` & `tmp/antsibull_docs-2.3.0.tar.gz`

## Comparing `antsibull_docs-2.2.0.tar` & `antsibull_docs-2.3.0.tar`

### file list

```diff
@@ -1,522 +1,618 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.flake8
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.pylintrc.automated
--rw-r--r--   0        0        0    26378 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/LICENSE
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/antsibull-docs.cfg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/codecov.yml
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/noxfile.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.github/patchback.yml
--rw-r--r--   0        0        0     8888 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.github/workflows/build-css.yml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.reuse/dep5
--rw-r--r--   0        0        0    32066 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/docs/schemas.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/app_context.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/augment_docs.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/collection_config.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/collection_links.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/constants.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/env_variables.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/extra_docs.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/lint_extra_docs.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/lint_helpers.py
--rw-r--r--   0        0        0    29883 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/lint_plugin_docs.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/plugin_docs.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/process_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/py.typed
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/rstcheck.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/__init__.py
--rw-r--r--   0        0        0    26939 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/antsibull_docs.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/__init__.py
--rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/_build.py
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/collection.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/current.py
--rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/devel.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/lint_collection_docs.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/plugin.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
--rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/stable.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/__init__.py
--rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/ansible_2_10_routing.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/__init__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    17353 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
--rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/build_sh.j2
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/conf_py.j2
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/__init__.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/ansible_doc.py
--rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/fqcn.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/parsing.py
--rw-r--r--   0        0        0    17280 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/routing.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/jinja2/__init__.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/jinja2/environment.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/jinja2/filters.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/jinja2/tests.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/markup/__init__.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/markup/_counter.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/markup/htmlify.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/markup/rstify.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/markup/semantic_helper.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/ansible_doc.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/app_context.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/collection_config.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/collection_links.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/ansible_doc.py
--rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/base.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/callback.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/module.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/plugin.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/positional.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/role.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/utils/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/utils/collection_name_transformer.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/utils/get_pkg_data.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/utils/rst.py
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/vendored/ansible.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/__init__.py
--rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/collections.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/hierarchy.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/indexes.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/plugin_stubs.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/antsibull_docs/write_docs/plugins.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/__init__.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/antsibull-minimal.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/assets.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/roles.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/browserslistrc
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/build.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/cssnano.config.js
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/argcomplete.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/rstcheck.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/__init__.pyi
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/constants.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/release.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/cli/__init__.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/cli/arguments.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/collections/list.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/galaxy/collection.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/module_utils/_text.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/module_utils/common/json.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/plugins/loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/utils/collection_loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/ansible/utils/plugin_docs.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/jinja2/utils.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/rstcheck_core/__init__.pyi
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/rstcheck_core/checker.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/rstcheck_core/config.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/stubs/rstcheck_core/types.pyi
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/validate-html.py
--rw-r--r--   0        0        0  1043077 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all-others.json.license
--rw-r--r--   0        0        0  1041231 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all.json.license
--rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col1.json.license
--rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col2.json.license
--rw-r--r--   0        0        0    40997 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.col.json.license
--rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-all-others.json.license
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-all.json.license
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns.col1.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-version.output
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible-version.output.license
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/ansible_doc_caching.py
--rwxr-xr-x   0        0        0     3141 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/build-docs-baseline.sh
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/build-sphinx-init-baseline.sh
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/sanitize-ansible-doc-dump.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/sanitize-ansible-galaxy-list.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/test.rst
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/test_docs_baseline.py
--rw-r--r--   0        0        0   101015 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/test_docs_linting.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/test_sphinx_init_baseline.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/environment_variables.rst
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_connection.rst
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_lookup.rst
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_module.rst
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_strategy.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/index_vars.rst
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/index.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/index.rst
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/.gitignore
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      809 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/build.sh
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/conf.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/requirements.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/build.sh
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/conf.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
--rw-r--r--   0        0        0     9572 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/test_schema.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become.json.license
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become_results.json.license
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache.json.license
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache_results.json.license
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback.json.license
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback_results.json.license
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf.json.license
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf_results.json.license
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection.json.license
--rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection_results.json.license
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter.json.license
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter_results.json.license
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi.json.license
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi_results.json.license
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory.json.license
--rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory_results.json.license
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup.json.license
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup_results.json.license
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module.json.license
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf.json.license
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf_results.json.license
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role.json.license
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role_results.json.license
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell.json.license
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy.json.license
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy_results.json.license
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test.json.license
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test_results.json.license
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars.json.license
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars_results.json.license
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection.json.license
--rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection_results.json.license
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/units/test_jinja2.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/units/markup/test_counter.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/units/markup/test_markup.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/tests/units/markup/test_semantic_helper.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/.gitignore
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/README.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 antsibull_docs-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.flake8
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.pylintrc.automated
+-rw-r--r--   0        0        0    28723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/antsibull-docs.cfg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/codecov.yml
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.github/patchback.yml
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.github/workflows/build-css.yml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.reuse/dep5
+-rw-r--r--   0        0        0    34810 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/changelogs/fragments/.keep
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/docs/schemas.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/app_context.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/augment_docs.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/collection_config.py
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/collection_links.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/constants.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/env_variables.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/extra_docs.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/lint_extra_docs.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/lint_helpers.py
+-rw-r--r--   0        0        0    33046 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/lint_plugin_docs.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/plugin_docs.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/process_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/py.typed
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/rstcheck.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/__init__.py
+-rw-r--r--   0        0        0    29884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/antsibull_docs.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/__init__.py
+-rw-r--r--   0        0        0    13667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/_build.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/collection.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/collection_plugins.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/current.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/devel.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/lint_docs.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/plugin.py
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/stable.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/__init__.py
+-rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/ansible_2_10_routing.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    13316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/build_sh.j2
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/conf_py.j2
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/__init__.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/ansible_doc.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/fqcn.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/parsing.py
+-rw-r--r--   0        0        0    19449 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/routing.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/jinja2/__init__.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/jinja2/environment.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/jinja2/filters.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/jinja2/tests.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/markup/__init__.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/markup/_counter.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/markup/htmlify.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/markup/rstify.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/markup/semantic_helper.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/ansible_doc.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/app_context.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/collection_config.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/collection_links.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/ansible_doc.py
+-rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/base.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/callback.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/module.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/plugin.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/positional.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/role.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/utils/collection_name_transformer.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/utils/get_pkg_data.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/utils/rst.py
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/vendored/ansible.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/__init__.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/collections.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/hierarchy.py
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/indexes.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/plugin_stubs.py
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/antsibull_docs/write_docs/plugins.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/__init__.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/antsibull-minimal.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/assets.py
+-rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/roles.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/sphinx_helper.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/browserslistrc
+-rwxr-xr-x   0        0        0     1085 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/build.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/cssnano.config.js
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/argcomplete.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/rstcheck.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/__init__.pyi
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/constants.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/release.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/cli/__init__.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/cli/arguments.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/collections/list.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/galaxy/collection.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/module_utils/_text.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/module_utils/common/json.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/plugins/loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/utils/collection_loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/ansible/utils/plugin_docs.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/jinja2/utils.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/rstcheck_core/__init__.pyi
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/rstcheck_core/checker.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/rstcheck_core/config.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/stubs/rstcheck_core/types.pyi
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/validate-html.py
+-rw-r--r--   0        0        0  1043185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all-others.json.license
+-rw-r--r--   0        0        0  1041339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all.json.license
+-rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col1.json.license
+-rw-r--r--   0        0        0    28792 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col2.json.license
+-rw-r--r--   0        0        0    41105 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.col.json.license
+-rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-all-others.json.license
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-all.json.license
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns.col1.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-version.output
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible-version.output.license
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/ansible_doc_caching.py
+-rwxr-xr-x   0        0        0     3401 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/build-docs-baseline.sh
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/build-sphinx-init-baseline.sh
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/sanitize-ansible-doc-dump.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/sanitize-ansible-galaxy-list.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/test.rst
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/test_docs_baseline.py
+-rw-r--r--   0        0        0   101030 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/test_docs_linting.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/test_sphinx_init_baseline.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/environment_variables.rst
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_lookup.rst
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_module.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/index_vars.rst
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/index.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_become.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_cache.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_callback.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_connection.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_filter.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_inventory.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_lookup.rst
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_module.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_role.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_shell.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_strategy.rst
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_test.rst
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/index_vars.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/index.rst
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/index.rst
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/.gitignore
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/build.sh
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/conf.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/requirements.txt
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/build.sh
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/test_schema.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become.json.license
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become_results.json.license
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache.json.license
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache_results.json.license
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback.json.license
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback_results.json.license
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf.json.license
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf_results.json.license
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection.json.license
+-rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection_results.json.license
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter.json.license
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter_results.json.license
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi.json.license
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi_results.json.license
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory.json.license
+-rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory_results.json.license
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup.json.license
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup_results.json.license
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module.json.license
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf.json.license
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf_results.json.license
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role.json.license
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role_results.json.license
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell.json.license
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy.json.license
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy_results.json.license
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test.json.license
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test_results.json.license
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars.json.license
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars_results.json.license
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection.json.license
+-rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection_results.json.license
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/units/test_jinja2.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/units/markup/test_counter.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/units/markup/test_markup.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/tests/units/markup/test_semantic_helper.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/.gitignore
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/README.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 antsibull_docs-2.3.0/PKG-INFO
```

### Comparing `antsibull_docs-2.2.0/.pylintrc.automated` & `antsibull_docs-2.3.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/CHANGELOG.rst` & `antsibull_docs-2.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,39 @@
 ===================================================================
 antsibull-docs -- Ansible Documentation Build Scripts Release Notes
 ===================================================================
 
 .. contents:: Topics
 
 
+v2.3.0
+======
+
+Release Summary
+---------------
+
+Bugfix and feature release.
+
+Minor Changes
+-------------
+
+- Add a ``:ansplugin:`` role to the Sphinx extension. This allows to reference a module, plugin, or role with the ``fqcn#type`` syntax from semantic markup instead of having to manually compose a ``ansible_collections.{fqcn}_{type}`` label. An explicit reference title can also be provided with the ``title <fqcn#type>`` syntax similar to the ``:ref:`` role (https://github.com/ansible-community/antsibull-docs/pull/180).
+- Add a new subcommand ``lint-core-docs`` which lints the ansible-core documentation (https://github.com/ansible-community/antsibull-docs/pull/182).
+- Add a new subcommand, ``collection-plugins``, for rendering files for all plugins and roles in a collection without any indexes (https://github.com/ansible-community/antsibull-docs/pull/177).
+- Add support for different output formats. Next to the default format, ``ansible-docsite``, a new **experimental** format ``simplified-rst`` is supported. Experimental means that it will likely change considerably in the next few releases until it stabilizes. Such changes will not be considered breaking changes, and could potentially even be bugfixes (https://github.com/ansible-community/antsibull-docs/pull/177).
+- Use Dart sass compiler instead of sassc to compile CSS for Sphinx extension (https://github.com/ansible-community/antsibull-docs/issues/185, https://github.com/ansible-community/antsibull-docs/pull/186).
+- When parsing errors happen in the Sphinx extension, the extension now emits error messages during the build process in addition to error markup (https://github.com/ansible-community/antsibull-docs/pull/187).
+
+Bugfixes
+--------
+
+- Consider module/plugin aliases when linting references to other modules and plugins (https://github.com/ansible-community/antsibull-docs/pull/184).
+- Make sure that all aliases are actually listed for plugins (https://github.com/ansible-community/antsibull-docs/pull/183).
+- When looking for redirects, the ``aliases`` field and filesystem redirects in ansible-core were not properly considered. This ensures that all redirect stubs are created, and that no duplicates show up, not depending on whether ansible-core is installed in editable mode or not (https://github.com/ansible-community/antsibull-docs/pull/183).
+
 v2.2.0
 ======
 
 Release Summary
 ---------------
 
 Bugfix and feature release improving rendering and linting.
```

### Comparing `antsibull_docs-2.2.0/LICENSE` & `antsibull_docs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/antsibull-docs.cfg` & `antsibull_docs-2.3.0/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/noxfile.py` & `antsibull_docs-2.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/.github/workflows/antsibull-docs.yml` & `antsibull_docs-2.3.0/.github/workflows/antsibull-docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         antsibull_core_ref:
           - main
         antsibull_docs_parser_ref:
           - main
         include:
           - options: '--use-current --use-html-blobs --no-breadcrumbs community.crypto community.docker'
             python: '3.9'
+          - options: '--use-current --output-format simplified-rst community.crypto community.docker'
+            python: '3.10'
 
     steps:
       - name: Check out antsibull-docs
         uses: actions/checkout@v3
         with:
           path: antsibull-docs
```

### Comparing `antsibull_docs-2.2.0/.github/workflows/build-css.yml` & `antsibull_docs-2.3.0/.github/workflows/build-css.yml`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,13 @@
       - name: Use Node.js
         uses: actions/setup-node@v3
         with:
           node-version: 16.x
 
       - name: Install dependencies
         run: |
-          sudo apt-get install sassc
-          npm install -g autoprefixer cssnano postcss postcss-cli
+          npm install -g sass autoprefixer cssnano postcss postcss-cli
 
       - name: Build CSS
         run: |
           ./build.sh
         working-directory: ./src/sphinx_antsibull_ext/css
```

### Comparing `antsibull_docs-2.2.0/.github/workflows/nox.yml` & `antsibull_docs-2.3.0/.github/workflows/nox.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/changelogs/changelog.yaml` & `antsibull_docs-2.3.0/changelogs/changelog.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -549,7 +549,47 @@
     - 169-seealso-desc-copying.yml
     - 171-lint.yml
     - 172-ref-casing.yml
     - 173-lint-array-stubs.yml
     - 175-sphinx-ext-nodes.yml
     - 2.2.0.yml
     release_date: '2023-06-27'
+  2.3.0:
+    changes:
+      bugfixes:
+      - Consider module/plugin aliases when linting references to other modules and
+        plugins (https://github.com/ansible-community/antsibull-docs/pull/184).
+      - Make sure that all aliases are actually listed for plugins (https://github.com/ansible-community/antsibull-docs/pull/183).
+      - When looking for redirects, the ``aliases`` field and filesystem redirects
+        in ansible-core were not properly considered. This ensures that all redirect
+        stubs are created, and that no duplicates show up, not depending on whether
+        ansible-core is installed in editable mode or not (https://github.com/ansible-community/antsibull-docs/pull/183).
+      minor_changes:
+      - Add a ``:ansplugin:`` role to the Sphinx extension. This allows to reference
+        a module, plugin, or role with the ``fqcn#type`` syntax from semantic markup
+        instead of having to manually compose a ``ansible_collections.{fqcn}_{type}``
+        label. An explicit reference title can also be provided with the ``title <fqcn#type>``
+        syntax similar to the ``:ref:`` role (https://github.com/ansible-community/antsibull-docs/pull/180).
+      - Add a new subcommand ``lint-core-docs`` which lints the ansible-core documentation
+        (https://github.com/ansible-community/antsibull-docs/pull/182).
+      - Add a new subcommand, ``collection-plugins``, for rendering files for all
+        plugins and roles in a collection without any indexes (https://github.com/ansible-community/antsibull-docs/pull/177).
+      - Add support for different output formats. Next to the default format, ``ansible-docsite``,
+        a new **experimental** format ``simplified-rst`` is supported. Experimental
+        means that it will likely change considerably in the next few releases until
+        it stabilizes. Such changes will not be considered breaking changes, and could
+        potentially even be bugfixes (https://github.com/ansible-community/antsibull-docs/pull/177).
+      - Use Dart sass compiler instead of sassc to compile CSS for Sphinx extension
+        (https://github.com/ansible-community/antsibull-docs/issues/185, https://github.com/ansible-community/antsibull-docs/pull/186).
+      - When parsing errors happen in the Sphinx extension, the extension now emits
+        error messages during the build process in addition to error markup (https://github.com/ansible-community/antsibull-docs/pull/187).
+      release_summary: Bugfix and feature release.
+    fragments:
+    - 177-output-format.yml
+    - 180-plugin-role.yml
+    - 182-core-lint.yml
+    - 183-routing.yml
+    - 184-lint-routing.yml
+    - 186-sass.yml
+    - 187-role-errors.yml
+    - 2.3.0.yml
+    release_date: '2023-07-09'
```

### Comparing `antsibull_docs-2.2.0/changelogs/config.yaml` & `antsibull_docs-2.3.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/docs/schemas.rst` & `antsibull_docs-2.3.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/app_context.py` & `antsibull_docs-2.3.0/src/antsibull_docs/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/augment_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/augment_docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2020, Ansible Project
 """Augment data from plugin documenation with additional values."""
 
 from __future__ import annotations
 
 import typing as t
+from collections import defaultdict
 from collections.abc import Mapping, MutableMapping
 
-from antsibull_docs.utils.rst import massage_rst_label
+from .docs_parsing.routing import CollectionRoutingT
+from .utils.rst import massage_rst_label
 
 
 def add_full_key(
     options_data: Mapping[str, t.Any],
     suboption_entry: str,
     _full_key: list[str] | None = None,
     _full_keys: list[list[str]] | None = None,
@@ -95,15 +97,33 @@
             desc = None
         if desc:
             if not desc.endswith((".", "!", "?")):
                 desc += "."
             entry["description"] = desc
 
 
-def augment_docs(plugin_info: MutableMapping[str, MutableMapping[str, t.Any]]) -> None:
+def _add_aliases(
+    plugin_name: str,
+    plugin_record: MutableMapping[str, t.Any],
+    routing_sources: list[str],
+) -> None:
+    collection_prefix = ".".join(plugin_name.split(".", 2)[:2]) + "."
+    for redirect in routing_sources:
+        if redirect.startswith(collection_prefix):
+            alias = redirect[len(collection_prefix) :]
+            if "aliases" not in plugin_record:
+                plugin_record["aliases"] = []
+            if alias not in plugin_record["aliases"]:
+                plugin_record["aliases"].append(alias)
+
+
+def augment_docs(
+    plugin_info: MutableMapping[str, MutableMapping[str, t.Any]],
+    collection_routing: CollectionRoutingT,
+) -> None:
     """
     Add additional data to the data extracted from the plugins.
 
     The additional data is calculated from the existing data and then added to the data.
     Current Augmentations:
 
     * ``full_key`` allows displaying nested suboptions and return dicts.
@@ -111,18 +131,28 @@
       automatically insert the destination's short_description (if available)
 
     :arg plugin_info: The plugin_info that will be analyzed and augmented.
 
     .. warning:: This function operates by side-effect.  The plugin_info dictionay is modified
         directly.
     """
-    for _, plugin_map in plugin_info.items():
-        for _, plugin_record in plugin_map.items():
+    for plugin_type, plugin_map in plugin_info.items():
+        # First collect all routing targets
+        routing_sources: defaultdict[str, list[str]] = defaultdict(list)
+        for plugin_name, plugin_meta in collection_routing.get(plugin_type, {}).items():
+            redirect = plugin_meta.get("redirect")
+            if isinstance(redirect, str):
+                routing_sources[redirect].append(plugin_name)
+        # Now augment all plugin records
+        for plugin_name, plugin_record in plugin_map.items():
             if plugin_record.get("return"):
                 add_full_key(plugin_record["return"], "contains")
             if plugin_record.get("doc"):
                 add_full_key(plugin_record["doc"]["options"], "suboptions")
                 if plugin_record["doc"].get("seealso"):
                     _add_seealso(plugin_record["doc"]["seealso"], plugin_info)
+                _add_aliases(
+                    plugin_name, plugin_record["doc"], routing_sources[plugin_name]
+                )
             if plugin_record.get("entry_points"):
                 for entry_point in plugin_record["entry_points"].values():
                     add_full_key(entry_point["options"], "options")
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/collection_config.py` & `antsibull_docs-2.3.0/src/antsibull_docs/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/collection_links.py` & `antsibull_docs-2.3.0/src/antsibull_docs/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/constants.py` & `antsibull_docs-2.3.0/src/antsibull_docs/constants.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/env_variables.py` & `antsibull_docs-2.3.0/src/antsibull_docs/env_variables.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/extra_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/lint_extra_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/lint_extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/lint_helpers.py` & `antsibull_docs-2.3.0/src/antsibull_docs/lint_helpers.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/lint_plugin_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/lint_plugin_docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,37 +17,41 @@
 
 from antsibull_core.subprocess_util import log_run
 from antsibull_core.vendored.json_utils import _filter_non_json_lines
 from antsibull_core.venv import FakeVenvRunner
 from antsibull_docs_parser import dom
 from antsibull_docs_parser.parser import Context as ParserContext
 from antsibull_docs_parser.parser import parse as parse_markup
+from jinja2 import Template
 
 from sphinx_antsibull_ext import roles as antsibull_roles
 
 from .augment_docs import augment_docs
 from .collection_links import load_collections_links
 from .docs_parsing import AnsibleCollectionMetadata
 from .docs_parsing.ansible_doc import parse_ansible_galaxy_collection_list
 from .docs_parsing.parsing import get_ansible_plugin_info
 from .docs_parsing.routing import (
+    CollectionRoutingT,
     load_all_collection_routing,
     remove_redirect_duplicates,
 )
 from .jinja2.environment import OutputFormat, doc_environment
 from .lint_helpers import load_collection_info
 from .markup.semantic_helper import split_option_like_name
 from .plugin_docs import walk_plugin_docs_texts
 from .process_docs import (
     get_collection_contents,
     get_plugin_contents,
     normalize_all_plugin_info,
 )
 from .rstcheck import check_rst_content
+from .schemas.collection_links import CollectionLinks
 from .utils.collection_name_transformer import CollectionNameTransformer
+from .write_docs import PluginErrorsT
 from .write_docs.plugins import (
     create_plugin_rst,
     guess_relative_filename,
     has_broken_docs,
 )
 
 ValidCollectionRefs = t.Literal["self", "dependent", "all"]
@@ -132,14 +136,16 @@
 
 
 class _NameCollector:
     _plugins: set[tuple[str, str]]
     _option_names: dict[tuple[str, str, str], str]
     _return_value_names: dict[tuple[str, str, str], str]
     _collection_prefixes: set[str]
+    _collection_routing: CollectionRoutingT
+    _routing_table: dict[tuple[str, str], str]
 
     def _collect_role_option_names(
         self,
         plugin: tuple[str, str],
         options: dict[str, t.Any],
         entrypoint: str,
         path_prefixes: list[str],
@@ -196,19 +202,21 @@
             path = f"{path_prefix}{rv}"
             self._return_value_names[(*plugin, path)] = data["type"]
             if "contains" in data:
                 self._collect_return_value_names(
                     plugin, data["contains"], f"{path}{_NAME_SEPARATOR}"
                 )
 
-    def __init__(self):
+    def __init__(self, collection_routing: CollectionRoutingT):
         self._plugins = set()
         self._collection_prefixes = set()
         self._option_names = {}
         self._return_value_names = {}
+        self._collection_routing = collection_routing
+        self._routing_table = {}
 
     def collect_collection(self, collection_name_or_fqcn: str):
         self._collection_prefixes.add(
             _get_fqcn_collection_prefix(collection_name_or_fqcn)
         )
 
     def collect_plugin(
@@ -224,33 +232,64 @@
         if "entry_points" in plugin_record:
             for entry_point, data in sorted(plugin_record["entry_points"].items()):
                 if "options" in data:
                     self._collect_role_option_names(
                         plugin, data["options"], entry_point, [""]
                     )
 
+    def _resolve_plugin_fqcn(self, plugin_fqcn: str, plugin_type: str) -> str:
+        try:
+            return self._routing_table[(plugin_fqcn, plugin_type)]
+        except KeyError:
+            pass
+        tried_names = {plugin_fqcn}
+        new_fqcn = plugin_fqcn
+        while True:
+            try:
+                new_fqcn = self._collection_routing[plugin_type][new_fqcn]["redirect"]
+            except KeyError:
+                break
+            if new_fqcn in tried_names:
+                # Found infinite loop! Do not resolve name.
+                new_fqcn = plugin_fqcn
+                break
+            tried_names.add(new_fqcn)
+        self._routing_table[(plugin_fqcn, plugin_type)] = new_fqcn
+        return new_fqcn
+
     def get_option_type(
         self, plugin_fqcn: str, plugin_type: str, option_name: str
     ) -> str | None:
-        key = (plugin_fqcn, plugin_type, option_name)
+        key = (
+            self._resolve_plugin_fqcn(plugin_fqcn, plugin_type),
+            plugin_type,
+            option_name,
+        )
         return self._option_names.get(key)
 
     def get_return_value_type(
         self, plugin_fqcn: str, plugin_type: str, return_value_name: str
     ) -> str | None:
-        key = (plugin_fqcn, plugin_type, return_value_name)
+        key = (
+            self._resolve_plugin_fqcn(plugin_fqcn, plugin_type),
+            plugin_type,
+            return_value_name,
+        )
         return self._return_value_names.get(key)
 
     def is_valid_collection(self, plugin_fqcn: str) -> bool:
         return any(
             plugin_fqcn.startswith(prefix) for prefix in self._collection_prefixes
         )
 
     def is_valid_plugin(self, plugin_fqcn: str, plugin_type: str) -> bool:
-        return (plugin_fqcn, plugin_type) in self._plugins
+        return (
+            self._resolve_plugin_fqcn(plugin_fqcn, plugin_type),
+            plugin_type,
+        ) in self._plugins
 
     def is_valid_option(
         self, plugin_fqcn: str, plugin_type: str, option_name: str
     ) -> bool:
         return self.get_option_type(plugin_fqcn, plugin_type, option_name) is not None
 
     def is_valid_return_value(
@@ -519,16 +558,17 @@
 def _collect_names(
     new_plugin_info: Mapping[str, Mapping[str, t.Any]],
     collection_to_plugin_info: Mapping[str, Mapping[str, Mapping[str, str]]],
     collection_name: str,
     collections: list[str],
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     validate_collections_refs: ValidCollectionRefs,
+    collection_routing: CollectionRoutingT,
 ) -> _NameCollector:
-    name_collector = _NameCollector()
+    name_collector = _NameCollector(collection_routing)
     name_collector.collect_collection(collection_name)
     for other_collection in collection_metadata.keys():
         if validate_collections_refs != "all" and other_collection not in collections:
             continue
     for collection_name_, plugins_by_type in collection_to_plugin_info.items():
         if validate_collections_refs != "all" and collection_name_ not in collections:
             continue
@@ -539,19 +579,87 @@
                 if not has_broken_docs(plugin_record, plugin_type):
                     name_collector.collect_plugin(
                         plugin_record, plugin_name, plugin_type
                     )
     return name_collector
 
 
+def _lint_plugin_docs(
+    result: list[tuple[str, int, int, str]],
+    original_path_to_collection: str,
+    name_collector: _NameCollector,
+    collection_name: str,
+    collection_metadata: Mapping[str, AnsibleCollectionMetadata],
+    link_data: Mapping[str, CollectionLinks],
+    plugin_name: str,
+    plugin_type: str,
+    plugin_short_name: str,
+    filename: str,
+    plugin_record: dict[str, t.Any],
+    nonfatal_errors: PluginErrorsT,
+    plugin_type_tmpl: Template,
+    error_tmpl: Template,
+    disallow_unknown_collection_refs: bool,
+    disallow_semantic_markup: bool,
+    skip_rstcheck: bool,
+    validate_collections_refs: ValidCollectionRefs,
+):
+    if has_broken_docs(plugin_record, plugin_type):
+        result.append((filename, 0, 0, "Did not return correct DOCUMENTATION"))
+    else:
+        result.extend(
+            _validate_markup(
+                name_collector,
+                plugin_record,
+                plugin_name,
+                plugin_type,
+                filename,
+                validate_collections_refs,
+                disallow_unknown_collection_refs,
+                disallow_semantic_markup,
+            )
+        )
+    for error in nonfatal_errors[plugin_type][plugin_name]:
+        result.append((filename, 0, 0, error))
+    rst_content = create_plugin_rst(
+        collection_name,
+        collection_metadata[collection_name],
+        link_data[collection_name],
+        plugin_short_name,
+        plugin_type,
+        plugin_record,
+        nonfatal_errors[plugin_type][plugin_name],
+        plugin_type_tmpl,
+        error_tmpl,
+        use_html_blobs=False,
+        log_errors=False,
+    )
+    if not skip_rstcheck:
+        path = os.path.join(
+            original_path_to_collection,
+            "plugins",
+            plugin_type,
+            f"{plugin_short_name}.rst",
+        )
+        rst_results = check_rst_content(
+            rst_content,
+            filename=path,
+            ignore_directives=["rst-class"],
+            ignore_roles=list(antsibull_roles.ROLES),
+        )
+        result.extend(
+            [(path, result[0], result[1], result[2]) for result in rst_results]
+        )
+
+
 def _lint_collection_plugin_docs(
-    collections_dir: str,
+    collections_dir: str | None,
     dependencies: list[str],
     collection_name: str,
-    original_path_to_collection: str,
+    original_path_to_collection: str | None,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     validate_collections_refs: ValidCollectionRefs,
     disallow_unknown_collection_refs: bool,
     skip_rstcheck: bool,
     disallow_semantic_markup: bool,
     output_format: OutputFormat,
@@ -573,22 +681,25 @@
             if validate_collections_refs == "self"
             else collections
             if validate_collections_refs == "dependent"
             else None,
             fetch_all_installed=validate_collections_refs == "all",
         )
     )
+    if original_path_to_collection is None:
+        original_path_to_collection = collection_metadata[collection_name].path
+
     # Load routing information
     collection_routing = asyncio.run(load_all_collection_routing(collection_metadata))
     # Process data
     remove_redirect_duplicates(plugin_info, collection_routing)
     new_plugin_info, nonfatal_errors = asyncio.run(
         normalize_all_plugin_info(plugin_info)
     )
-    augment_docs(new_plugin_info)
+    augment_docs(new_plugin_info, collection_routing)
     # Load link data
     link_data = asyncio.run(
         load_collections_links(
             {name: data.path for name, data in collection_metadata.items()}
         )
     )
     # More processing
@@ -612,17 +723,18 @@
     name_collector = _collect_names(
         new_plugin_info,
         collection_to_plugin_info,
         collection_name,
         collections,
         collection_metadata,
         validate_collections_refs,
+        collection_routing,
     )
 
-    result = []
+    result: list[tuple[str, int, int, str]] = []
     for collection_name_, plugins_by_type in collection_to_plugin_info.items():
         if collection_name_ != collection_name:
             continue
         for plugin_type, plugins_dict in plugins_by_type.items():
             plugin_type_tmpl = plugin_tmpl
             if plugin_type == "role":
                 plugin_type_tmpl = role_tmpl
@@ -635,76 +747,46 @@
                         plugin_record,
                         plugin_short_name,
                         plugin_type,
                         collection_name_,
                         collection_metadata[collection_name_],
                     ),
                 )
-                if has_broken_docs(plugin_record, plugin_type):
-                    result.append(
-                        (filename, 0, 0, "Did not return correct DOCUMENTATION")
-                    )
-                else:
-                    result.extend(
-                        _validate_markup(
-                            name_collector,
-                            plugin_record,
-                            plugin_name,
-                            plugin_type,
-                            filename,
-                            validate_collections_refs,
-                            disallow_unknown_collection_refs,
-                            disallow_semantic_markup,
-                        )
-                    )
-                for error in nonfatal_errors[plugin_type][plugin_name]:
-                    result.append((filename, 0, 0, error))
-                rst_content = create_plugin_rst(
+                _lint_plugin_docs(
+                    result,
+                    original_path_to_collection,
+                    name_collector,
                     collection_name_,
-                    collection_metadata[collection_name_],
-                    link_data[collection_name_],
-                    plugin_short_name,
+                    collection_metadata,
+                    link_data,
+                    plugin_name,
                     plugin_type,
+                    plugin_short_name,
+                    filename,
                     plugin_record,
-                    nonfatal_errors[plugin_type][plugin_name],
+                    nonfatal_errors,
                     plugin_type_tmpl,
                     error_tmpl,
-                    use_html_blobs=False,
-                    log_errors=False,
+                    disallow_unknown_collection_refs,
+                    disallow_semantic_markup,
+                    skip_rstcheck,
+                    validate_collections_refs,
                 )
-                if not skip_rstcheck:
-                    path = os.path.join(
-                        original_path_to_collection,
-                        "plugins",
-                        plugin_type,
-                        f"{plugin_short_name}.rst",
-                    )
-                    rst_results = check_rst_content(
-                        rst_content,
-                        filename=path,
-                        ignore_directives=["rst-class"],
-                        ignore_roles=list(antsibull_roles.ROLES),
-                    )
-                    result.extend(
-                        [
-                            (path, result[0], result[1], result[2])
-                            for result in rst_results
-                        ]
-                    )
     return result
 
 
 def lint_collection_plugin_docs(
     path_to_collection: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     validate_collections_refs: ValidCollectionRefs = "self",
     disallow_unknown_collection_refs: bool = False,
     skip_rstcheck: bool = False,
     disallow_semantic_markup: bool = False,
+    output_format: OutputFormat = OutputFormat.ANSIBLE_DOCSITE,
 ) -> list[tuple[str, int, int, str]]:
     try:
         info = load_collection_info(path_to_collection)
         namespace = info["namespace"]
         name = info["name"]
         dependencies = info.get("dependencies") or {}
     except Exception:  # pylint:disable=broad-except
@@ -757,11 +839,33 @@
                 path_to_collection,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 validate_collections_refs=validate_collections_refs,
                 disallow_unknown_collection_refs=disallow_unknown_collection_refs,
                 skip_rstcheck=skip_rstcheck,
                 disallow_semantic_markup=disallow_semantic_markup,
-                output_format=OutputFormat.ANSIBLE_DOCSITE,
+                output_format=output_format,
             )
         )
     return result
+
+
+def lint_core_plugin_docs(
+    collection_url: CollectionNameTransformer,
+    collection_install: CollectionNameTransformer,
+    validate_collections_refs: ValidCollectionRefs = "self",
+    disallow_unknown_collection_refs: bool = False,
+) -> list[tuple[str, int, int, str]]:
+    result = _lint_collection_plugin_docs(
+        None,
+        ["ansible.builtin"],
+        "ansible.builtin",
+        None,
+        collection_url=collection_url,
+        collection_install=collection_install,
+        validate_collections_refs=validate_collections_refs,
+        disallow_unknown_collection_refs=disallow_unknown_collection_refs,
+        skip_rstcheck=True,
+        disallow_semantic_markup=False,
+        output_format=OutputFormat.ANSIBLE_DOCSITE,
+    )
+    return result
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/plugin_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/plugin_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/process_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/process_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/rstcheck.py` & `antsibull_docs-2.3.0/src/antsibull_docs/rstcheck.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/antsibull_docs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/antsibull_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 from antsibull_core.filesystem import UnableToCheck, writable_via_acls  # noqa: E402
 
 from ..constants import DOCUMENTABLE_PLUGINS  # noqa: E402
 from ..docs_parsing.fqcn import is_fqcn  # noqa: E402
 from ..schemas.app_context import DocsAppContext  # noqa: E402
 from .doc_commands import (  # noqa: E402
     collection,
+    collection_plugins,
     current,
     devel,
-    lint_collection_docs,
+    lint_docs,
     plugin,
     sphinx_init,
     stable,
 )
 
 # pylint: enable=wrong-import-position
 
@@ -53,25 +54,27 @@
 #: Mapping from command line subcommand names to functions which implement those
 #: The functions need to take a single argument, the processed list of args.
 ARGS_MAP: dict[str, Callable] = {
     "devel": devel.generate_docs,
     "stable": stable.generate_docs,
     "current": current.generate_docs,
     "collection": collection.generate_docs,
+    "collection-plugins": collection_plugins.generate_docs,
     "plugin": plugin.generate_docs,
     "sphinx-init": sphinx_init.site_init,
-    "lint-collection-docs": lint_collection_docs.lint_collection_docs,
+    "lint-collection-docs": lint_docs.lint_collection_docs,
+    "lint-core-docs": lint_docs.lint_core_docs,
 }
 
 #: The filename for the file which lists raw collection names
 DEFAULT_PIECES_FILE: str = "ansible.in"
 
 
 def _normalize_docs_options(args: argparse.Namespace) -> None:
-    if args.command == "lint-collection-docs":
+    if args.command in ("lint-collection-docs", "lint-core-docs"):
         return
 
     args.dest_dir = os.path.abspath(os.path.realpath(args.dest_dir))
 
     # We're going to be writing a deep hierarchy of files into this directory so we need to make
     # sure that the user understands that this needs to be a directory which has been secured
     # against malicious usage:
@@ -275,14 +278,25 @@
         "--collection-cache",
         default=argparse.SUPPRESS,
         help="Directory of collection tarballs.  These will be used instead"
         " of downloading fresh versions provided that they meet the criteria"
         " (Latest version of the collections known to galaxy).",
     )
 
+    output_format_parser = argparse.ArgumentParser(add_help=False)
+    output_format_parser.add_argument(
+        "--output-format",
+        default="ansible-docsite",
+        choices=["ansible-docsite", "simplified-rst"],
+        help="What kind of output format to use. Note that simplified-rst is"
+        " *EXPERIMENTAL*; the output format will likely change considerably"
+        " over the next few versions, and these changes will not be considered"
+        " breaking changes.",
+    )
+
     whole_site_parser = argparse.ArgumentParser(add_help=False)
     whole_site_parser.add_argument(
         "--breadcrumbs",
         "--gretel",
         dest="breadcrumbs",
         action=BooleanOptionalAction,
         default=argparse.SUPPRESS,
@@ -366,15 +380,15 @@
     )
 
     #
     # Document the currently installed version of ansible
     #
     current_parser = subparsers.add_parser(
         "current",
-        parents=[docs_parser, whole_site_parser, template_parser],
+        parents=[docs_parser, whole_site_parser, template_parser, output_format_parser],
         description="Generate documentation for the current"
         " installed version of ansible and the current installed"
         " collections",
     )
     current_parser.add_argument(
         "--collection-dir",
         help="Path to the directory containing ansible_collections. If not"
@@ -383,15 +397,15 @@
     )
 
     #
     # Document one or more specified collections
     #
     collection_parser = subparsers.add_parser(
         "collection",
-        parents=[docs_parser, whole_site_parser, template_parser],
+        parents=[docs_parser, whole_site_parser, template_parser, output_format_parser],
         description="Generate documentation for specified collections",
     )
     collection_parser.add_argument(
         "--collection-version",
         default="@latest",
         help="The version of the collection to document.  The special"
         ' version, "@latest" can be used to download and document the'
@@ -422,15 +436,15 @@
     )
 
     #
     # Document a specifically named plugin
     #
     file_parser = subparsers.add_parser(
         "plugin",
-        parents=[docs_parser, template_parser],
+        parents=[docs_parser, template_parser, output_format_parser],
         description="Generate documentation for a single plugin",
     )
     file_parser.add_argument(
         nargs=1,
         dest="plugin",
         action="store",
         help="A single file to document. Either a path to a file, or a FQCN."
@@ -442,19 +456,57 @@
         action="store",
         default="module",
         choices=DOCUMENTABLE_PLUGINS,
         help="The type of the plugin",
     )
 
     #
+    # Document one or more specified collections
+    #
+    collection_plugins_parser = subparsers.add_parser(
+        "collection-plugins",
+        parents=[docs_parser, template_parser, output_format_parser],
+        description="Generate documentation for all plugins of a specified collection",
+    )
+    collection_plugins_parser.add_argument(
+        "--collection-version",
+        default="@latest",
+        help="The version of the collection to document.  The special"
+        ' version, "@latest" can be used to download and document the'
+        " latest version from galaxy.",
+    )
+    collection_plugins_parser.add_argument(
+        "--use-current",
+        action="store_true",
+        default=False,
+        help="Assumes that the argument is a collection name, and"
+        " that collection has been installed with the current"
+        " version of ansible. Specified --collection-version will be"
+        " ignored.",
+    )
+    collection_plugins_parser.add_argument(
+        "--fqcn-plugin-names",
+        action="store_true",
+        default=False,
+        help="Include the collection name in the plugin file names.",
+    )
+    collection_plugins_parser.add_argument(
+        nargs=1,
+        dest="collection",
+        help="A collection whose plugins to document.  It will be"
+        " downloaded from Galaxy or is assumed to be installed,"
+        " depending on whether --use-current is specified.",
+    )
+
+    #
     # Create a Sphinx site template
     #
     sphinx_init_parser = subparsers.add_parser(
         "sphinx-init",
-        parents=[docs_parser, template_parser, whole_site_parser],
+        parents=[docs_parser, template_parser, whole_site_parser, output_format_parser],
         description="Generate a Sphinx site template for a collection docsite",
     )
 
     sphinx_init_parser.add_argument(
         "--collection-version",
         default="@latest",
         help="The version of the collection to document.  The special"
@@ -554,14 +606,15 @@
     )
 
     #
     # Lint collection docs
     #
     lint_collection_docs_parser = subparsers.add_parser(
         "lint-collection-docs",
+        parents=[output_format_parser],
         description="Collection extra docs linter for inclusion in docsite",
     )
 
     lint_collection_docs_parser.add_argument(
         "collection_root_path",
         metavar="/path/to/collection",
         help="path to collection (directory that includes galaxy.yml)",
@@ -588,19 +641,17 @@
         " to all collections the linter can find.",
     )
     lint_collection_docs_parser.add_argument(
         "--disallow-unknown-collection-refs",
         dest="disallow_unknown_collection_refs",
         action=BooleanOptionalAction,
         default=False,
-        help="When --plugin-docs is specified, determine references to which"
-        " collections to validate.  'self' means only validate references to"
-        " this collection.  'dependent' means validating references to"
-        " collections this collection (transitively) depends on.  'all' means"
-        " validating references to all collections the linter can find.",
+        help="When --plugin-docs is specified, determine whether to accept"
+        " references to unknown collections that are not covered by "
+        "--validate-collection-refs.",
     )
     lint_collection_docs_parser.add_argument(
         "--skip-rstcheck",
         dest="skip_rstcheck",
         action=BooleanOptionalAction,
         default=False,
         help="When --plugin-docs is specified, do not run"
@@ -614,14 +665,40 @@
         default=False,
         help="When --plugin-docs is specified, check that"
         " there is no semantic markup used. This can be used"
         " by collections to ensure that semantic markup is"
         " not yet used.",
     )
 
+    #
+    # Lint core docs
+    #
+    lint_core_docs_parser = subparsers.add_parser(
+        "lint-core-docs",
+        description="Collection extra docs linter for inclusion in docsite",
+    )
+
+    lint_core_docs_parser.add_argument(
+        "--validate-collection-refs",
+        dest="validate_collections_refs",
+        choices=["self", "all"],
+        default="self",
+        help="Determine references to which collections to validate.  'self'"
+        " means only validate references to ansible.builtin.  'all' means"
+        " validating references to all collections the linter can find.",
+    )
+    lint_core_docs_parser.add_argument(
+        "--disallow-unknown-collection-refs",
+        dest="disallow_unknown_collection_refs",
+        action=BooleanOptionalAction,
+        default=False,
+        help="Determine whether to accept references to unknown collections"
+        " that are not covered by --validate-collection-refs.",
+    )
+
     flog.debug("Argument parser setup")
 
     if "--ansible-base-cache" in args:
         flog.warning(
             "The CLI parameter, `--ansible-base-cache` has been renamed to"
             " `--ansible-core-source`.  Please use that instead"
         )
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/_build.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/_build.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 from ...env_variables import (
     collect_referable_envvars,
     collect_referenced_environment_variables,
     load_ansible_config,
 )
 from ...extra_docs import load_collections_extra_docs
-from ...jinja2.environment import OutputFormat
+from ...jinja2 import FilenameGenerator, OutputFormat
 from ...process_docs import (
     get_callback_plugin_contents,
     get_collection_contents,
     get_collection_namespaces,
     get_plugin_contents,
     normalize_all_plugin_info,
 )
@@ -49,52 +49,61 @@
 )
 from ...write_docs.plugin_stubs import output_all_plugin_stub_rst
 from ...write_docs.plugins import output_all_plugin_rst
 
 mlog = log.fields(mod=__name__)
 
 
-def generate_docs_for_all_collections(
+def generate_docs_for_all_collections(  # noqa: C901
     venv: VenvRunner | FakeVenvRunner,
     collection_dir: str | None,
     dest_dir: str,
     output_format: OutputFormat,
     *,
     collection_names: list[str] | None = None,
     create_indexes: bool = True,
+    create_collection_indexes: bool = True,
+    add_extra_docs: bool = True,
+    add_redirect_stubs: bool = True,
     squash_hierarchy: bool = False,
     breadcrumbs: bool = True,
     use_html_blobs: bool = False,
     fail_on_error: bool = False,
     for_official_docsite: bool = False,
+    include_collection_name_in_plugins: bool = False,
 ) -> int:
     """
     Create documentation for a set of installed collections.
 
     :arg venv: The venv in which ansible-core is installed.
     :arg collection_dir: The directory in which the collections have been installed.
                          If ``None``, the collections are assumed to be in the current
                          search path for Ansible.
     :arg dest_dir: The directory into which the documentation is written.
     :arg output_format: The output format.
     :kwarg collection_names: Optional list of collection names. If specified, only documentation
                              for these collections will be collected and generated.
     :kwarg create_indexes: Whether to create the collection, namespace, and plugin indexes. By
                            default, they are created.
+    :kwarg create_collection_indexes: Whether to create the per-collection plugin index.
+    :kwarg add_extra_docs: Whether to add extra docs.
+    :kwarg add_redirect_stubs: Whether to create redirect stub files.
     :kwarg squash_hierarchy: If set to ``True``, no directory hierarchy will be used.
                              Undefined behavior if documentation for multiple collections are
                              created.
     :kwarg breadcrumbs: Default True.  Set to False if breadcrumbs for collections should be
         disabled.  This will disable breadcrumbs but save on memory usage.
     :kwarg use_html_blobs: Default False.  Set to True if HTML blobs should be used instead of
         RST tables for parameter and return value tables.
     :kwarg fail_on_error: Default False.  Set to True to fail on loading or schema validation
         errors, instead of generating error pages.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg include_collection_name_in_plugins: Default False.  Set to True to use the FQCN for
+        plugin files instead of only the part without the collection name.
     :returns: A return code for the program.  See :func:`antsibull.cli.antsibull_docs.main` for
         details on what each code means.
     """
     flog = mlog.fields(func="generate_docs_for_all_collections")
     flog.notice("Begin")
 
     app_ctx = app_context.app_ctx.get()
@@ -115,21 +124,23 @@
     # Load collection routing information
     collection_routing = asyncio.run(load_all_collection_routing(collection_metadata))
     flog.notice("Finished loading collection routing information")
     # flog.fields(collection_routing=collection_routing).debug('Collection routing infos')
 
     remove_redirect_duplicates(plugin_info, collection_routing)
     stubs_info = find_stubs(plugin_info, collection_routing)
+    if collection_names is not None and "ansible.builtin" not in collection_names:
+        stubs_info.pop("ansible.builtin", None)
     # flog.fields(stubs_info=stubs_info).debug('Stubs info')
 
     new_plugin_info, nonfatal_errors = asyncio.run(
         normalize_all_plugin_info(plugin_info)
     )
     flog.fields(errors=len(nonfatal_errors)).notice("Finished data validation")
-    augment_docs(new_plugin_info)
+    augment_docs(new_plugin_info, collection_routing)
     flog.notice("Finished calculating new data")
 
     # Load collection extra docs data
     extra_docs_data = asyncio.run(
         load_collections_extra_docs(
             {name: data.path for name, data in collection_metadata.items()}
         )
@@ -178,131 +189,150 @@
         app_ctx.collection_url, "https://galaxy.ansible.com/{namespace}/{name}"
     )
     collection_install = CollectionNameTransformer(
         app_ctx.collection_install,
         "ansible-galaxy collection install {namespace}.{name}",
     )
 
+    filename_generator = FilenameGenerator(
+        include_collection_name_in_plugins=include_collection_name_in_plugins
+    )
+
     # Only build top-level index if requested
     if create_indexes:
         asyncio.run(
             output_collection_index(
                 collection_to_plugin_info,
                 collection_namespaces,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 output_format=output_format,
+                filename_generator=filename_generator,
                 breadcrumbs=breadcrumbs,
                 for_official_docsite=for_official_docsite,
                 referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing collection index")
         asyncio.run(
             output_collection_namespace_indexes(
                 collection_namespaces,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 output_format=output_format,
+                filename_generator=filename_generator,
                 breadcrumbs=breadcrumbs,
                 for_official_docsite=for_official_docsite,
                 referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing collection namespace index")
         asyncio.run(
             output_plugin_indexes(
                 plugin_contents,
                 collection_metadata,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 output_format=output_format,
+                filename_generator=filename_generator,
                 for_official_docsite=for_official_docsite,
                 referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing plugin indexes")
         asyncio.run(
             output_callback_indexes(
                 callback_plugin_contents,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 output_format=output_format,
+                filename_generator=filename_generator,
                 for_official_docsite=for_official_docsite,
                 referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing callback plugin indexes")
 
-    asyncio.run(
-        output_indexes(
-            collection_to_plugin_info,
-            dest_dir,
-            collection_url=collection_url,
-            collection_install=collection_install,
-            collection_metadata=collection_metadata,
-            squash_hierarchy=squash_hierarchy,
-            extra_docs_data=extra_docs_data,
-            link_data=link_data,
-            output_format=output_format,
-            breadcrumbs=breadcrumbs,
-            for_official_docsite=for_official_docsite,
-            referable_envvars=referable_envvars,
+    if create_collection_indexes:
+        asyncio.run(
+            output_indexes(
+                collection_to_plugin_info,
+                dest_dir,
+                collection_url=collection_url,
+                collection_install=collection_install,
+                collection_metadata=collection_metadata,
+                squash_hierarchy=squash_hierarchy,
+                extra_docs_data=extra_docs_data,
+                link_data=link_data,
+                output_format=output_format,
+                filename_generator=filename_generator,
+                breadcrumbs=breadcrumbs,
+                for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
+            )
         )
-    )
-    flog.notice("Finished writing indexes")
+        flog.notice("Finished writing indexes")
 
-    asyncio.run(
-        output_all_plugin_stub_rst(
-            stubs_info,
-            dest_dir,
-            collection_url=collection_url,
-            collection_install=collection_install,
-            collection_metadata=collection_metadata,
-            link_data=link_data,
-            output_format=output_format,
-            squash_hierarchy=squash_hierarchy,
-            for_official_docsite=for_official_docsite,
-            referable_envvars=referable_envvars,
+    if add_redirect_stubs:
+        asyncio.run(
+            output_all_plugin_stub_rst(
+                stubs_info,
+                dest_dir,
+                collection_url=collection_url,
+                collection_install=collection_install,
+                collection_metadata=collection_metadata,
+                link_data=link_data,
+                output_format=output_format,
+                filename_generator=filename_generator,
+                squash_hierarchy=squash_hierarchy,
+                for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
+            )
         )
-    )
-    flog.debug("Finished writing plugin stubs")
+        flog.debug("Finished writing plugin stubs")
 
     asyncio.run(
         output_all_plugin_rst(
             collection_to_plugin_info,
             new_plugin_info,
             nonfatal_errors,
             dest_dir,
             collection_url=collection_url,
             collection_install=collection_install,
             collection_metadata=collection_metadata,
             link_data=link_data,
             output_format=output_format,
+            filename_generator=filename_generator,
             squash_hierarchy=squash_hierarchy,
             use_html_blobs=use_html_blobs,
             for_official_docsite=for_official_docsite,
             referable_envvars=referable_envvars,
         )
     )
     flog.debug("Finished writing plugin docs")
 
-    asyncio.run(
-        output_extra_docs(dest_dir, extra_docs_data, squash_hierarchy=squash_hierarchy)
-    )
-    flog.debug("Finished writing extra docs")
+    if add_extra_docs:
+        asyncio.run(
+            output_extra_docs(
+                dest_dir, extra_docs_data, squash_hierarchy=squash_hierarchy
+            )
+        )
+        flog.debug("Finished writing extra docs")
 
-    asyncio.run(
-        output_environment_variables(
-            dest_dir,
-            referenced_env_vars,
-            output_format=output_format,
-            squash_hierarchy=squash_hierarchy,
-            referable_envvars=referable_envvars,
+    if output_format == OutputFormat.ANSIBLE_DOCSITE:
+        asyncio.run(
+            output_environment_variables(
+                dest_dir,
+                referenced_env_vars,
+                output_format=output_format,
+                filename_generator=filename_generator,
+                squash_hierarchy=squash_hierarchy,
+                referable_envvars=referable_envvars,
+            )
         )
-    )
-    flog.debug("Finished writing environment variables")
+        flog.debug("Finished writing environment variables")
+
     return 0
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/collection.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 from ... import app_context
 from ...jinja2.environment import OutputFormat
 from ._build import generate_docs_for_all_collections
 
 mlog = log.fields(mod=__name__)
 
 
-def generate_collection_docs(collection_dir: str | None, squash_hierarchy: bool) -> int:
-    flog = mlog.fields(func="generate_current_docs")
+def generate_collection_docs(
+    collection_dir: str | None, output_format: OutputFormat, squash_hierarchy: bool
+) -> int:
+    flog = mlog.fields(func="generate_collection_docs")
     flog.debug("Begin generating docs")
 
     app_ctx = app_context.app_ctx.get()
 
     venv = FakeVenvRunner()
 
     return generate_docs_for_all_collections(
         venv,
         collection_dir,
         app_ctx.extra["dest_dir"],
-        OutputFormat.ANSIBLE_DOCSITE,
+        output_format,
         collection_names=app_ctx.extra["collections"],
         create_indexes=app_ctx.indexes and not squash_hierarchy,
         squash_hierarchy=squash_hierarchy,
         breadcrumbs=app_ctx.breadcrumbs,
         use_html_blobs=app_ctx.use_html_blobs,
         fail_on_error=app_ctx.extra["fail_on_error"],
     )
@@ -113,17 +115,18 @@
     """
     flog = mlog.fields(func="generate_docs")
     flog.debug("Begin processing docs")
 
     app_ctx = app_context.app_ctx.get()
 
     squash_hierarchy: bool = app_ctx.extra["squash_hierarchy"]
+    output_format = OutputFormat.parse(app_ctx.extra["output_format"])
 
     if app_ctx.extra["use_current"]:
-        return generate_collection_docs(None, squash_hierarchy)
+        return generate_collection_docs(None, output_format, squash_hierarchy)
 
     collection_version = app_ctx.extra["collection_version"]
     if collection_version == "@latest":
         collection_version = None
 
     with tempfile.TemporaryDirectory() as tmp_dir:
         # Retrieve the collections
@@ -133,15 +136,15 @@
                 app_ctx.extra["collections"],
                 collection_version,
                 tmp_dir,
                 galaxy_server=app_ctx.galaxy_url,
                 collection_cache=app_ctx.collection_cache,
             )
         )
-        # flog.fields(tarballs=collection_tarballs).debug('Download complete')
+        flog.fields(tarballs=collection_tarballs).debug("Download complete")
         flog.notice("Finished retrieving tarballs")
 
         # Install the collections to a directory
 
         # Directory that ansible needs to see
         collection_dir = os.path.join(tmp_dir, "installed")
         # Directory that the collections will be untarred inside of
@@ -154,8 +157,8 @@
 
         # Install the collections
         asyncio.run(
             install_together(list(collection_tarballs.values()), collection_install_dir)
         )
         flog.notice("Finished installing collections")
 
-        return generate_collection_docs(collection_dir, squash_hierarchy)
+        return generate_collection_docs(collection_dir, output_format, squash_hierarchy)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/current.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/current.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,20 @@
         details on what each code means.
     """
     flog = mlog.fields(func="generate_docs")
     flog.debug("Begin processing docs")
 
     app_ctx = app_context.app_ctx.get()
 
+    output_format = OutputFormat.parse(app_ctx.extra["output_format"])
+
     venv = FakeVenvRunner()
 
     return generate_docs_for_all_collections(
         venv,
         app_ctx.extra["collection_dir"],
         app_ctx.extra["dest_dir"],
-        OutputFormat.ANSIBLE_DOCSITE,
+        output_format,
         breadcrumbs=app_ctx.breadcrumbs,
         use_html_blobs=app_ctx.use_html_blobs,
         fail_on_error=app_ctx.extra["fail_on_error"],
     )
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/devel.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/devel.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 tmp_dir,
                 galaxy_server=app_ctx.galaxy_url,
                 ansible_core_source=app_ctx.extra["ansible_core_source"],
                 collection_cache=app_ctx.collection_cache,
                 use_installed_ansible_core=use_installed_ansible_core,
             )
         )
-        # flog.fields(tarballs=collection_tarballs).debug('Download complete')
+        flog.fields(tarballs=collection_tarballs).debug("Download complete")
         flog.notice("Finished retrieving tarballs")
 
         # Get the ansible-core location
         if use_installed_ansible_core:
             ansible_core_path = None
         else:
             try:
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/plugin.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 from antsibull_core.venv import FakeVenvRunner
 
 from ... import app_context
 from ...augment_docs import augment_docs
 from ...collection_links import CollectionLinks
 from ...docs_parsing import AnsibleCollectionMetadata
 from ...docs_parsing.fqcn import get_fqcn_parts, is_fqcn
-from ...jinja2.environment import OutputFormat, doc_environment
+from ...jinja2 import FilenameGenerator, OutputFormat
+from ...jinja2.environment import doc_environment
 from ...process_docs import normalize_plugin_info
 from ...utils.collection_name_transformer import CollectionNameTransformer
 from ...write_docs.plugins import write_plugin_rst
 
 mlog = log.fields(mod=__name__)
 
 
 def generate_plugin_docs(
     plugin_type: str,
     plugin_name: str,
     collection_name: str,
     plugin: str,
     output_path: str,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
 ) -> int:
     """
     Render documentation for a locally installed plugin.
     """
     flog = mlog.fields(func="generate_plugin_docs")
     flog.debug("Begin generating plugin docs")
 
@@ -99,15 +101,16 @@
     #     dict[str, dict[str, dict[str, typing.Any]]]
     # is acceptable for
     #     MutableMapping[str, MutableMapping[str, typing.Any]].
     augment_docs(
         t.cast(
             MutableMapping[str, MutableMapping[str, t.Any]],
             {plugin_type: {plugin_name: plugin_info}},
-        )
+        ),
+        {},
     )
 
     # Setup the jinja environment
     collection_url = CollectionNameTransformer(
         app_ctx.collection_url, "https://galaxy.ansible.com/{namespace}/{name}"
     )
     collection_install = CollectionNameTransformer(
@@ -131,14 +134,16 @@
             plugin,
             plugin_type,
             plugin_info,
             errors,
             plugin_tmpl,
             error_tmpl,
             "",
+            output_format,
+            filename_generator,
             path_override=output_path,
             use_html_blobs=app_ctx.use_html_blobs,
         )
     )
     flog.debug("Finished writing plugin docs")
 
     return 0
@@ -155,14 +160,15 @@
     """
     flog = mlog.fields(func="generate_docs")
     flog.debug("Begin processing docs")
 
     app_ctx = app_context.app_ctx.get()
     plugin_type: str = app_ctx.extra["plugin_type"]
     plugin_name: str = app_ctx.extra["plugin"][0]
+    output_format = OutputFormat.parse(app_ctx.extra["output_format"])
 
     if not is_fqcn(plugin_name):
         raise NotImplementedError(
             "Priority to implement subcommands is stable, devel, plugin, and"
             " then collection commands. Only the FQCN form is implemented"
             " for the plugin subcommand right now."
         )
@@ -175,15 +181,18 @@
         namespace, collection, plugin = get_fqcn_parts(plugin_name)
     except ValueError:
         namespace, collection = "ansible", "builtin"
         plugin = plugin_name
     collection_name = ".".join([namespace, collection])
     plugin_name = ".".join([namespace, collection, plugin])
 
+    filename_generator = FilenameGenerator()
+
     return generate_plugin_docs(
         plugin_type,
         plugin_name,
         collection_name,
         plugin,
         output_path,
-        OutputFormat.ANSIBLE_DOCSITE,
+        output_format,
+        filename_generator,
     )
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     title: str = app_ctx.extra["title"]
     html_short_title: str | None = app_ctx.extra["html_short_title"]
     if html_short_title is None:
         html_short_title = title
     extra_conf = split_kv(app_ctx.extra["extra_conf"])
     extra_html_context = split_kv(app_ctx.extra["extra_html_context"])
     extra_html_theme_options = split_kv(app_ctx.extra["extra_html_theme_options"])
+    output_format = app_ctx.extra["output_format"]
 
     sphinx_theme = "sphinx_ansible_theme"
     sphinx_theme_package = "sphinx-ansible-theme >= 0.9.0"
     if app_ctx.extra["sphinx_theme"] != "sphinx-ansible-theme":
         sphinx_theme = app_ctx.extra["sphinx_theme"]
         sphinx_theme_package = app_ctx.extra["sphinx_theme"]
 
@@ -170,14 +171,15 @@
                 project=project,
                 conf_copyright=conf_copyright,
                 title=title,
                 html_short_title=html_short_title,
                 extra_conf=extra_conf,
                 extra_html_context=extra_html_context,
                 extra_html_theme_options=extra_html_theme_options,
+                output_format=output_format,
             )
             + "\n"
         )
 
         destination = os.path.join(dest_dir, filename)
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         write_file(destination, content)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/cli/doc_commands/stable.py` & `antsibull_docs-2.3.0/src/antsibull_docs/cli/doc_commands/stable.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 tmp_dir,
                 galaxy_server=app_ctx.galaxy_url,
                 ansible_core_source=app_ctx.extra["ansible_core_source"],
                 collection_cache=app_ctx.collection_cache,
                 use_installed_ansible_core=use_installed_ansible_core,
             )
         )
-        # flog.fields(tarballs=collection_tarballs).debug('Download complete')
+        flog.fields(tarballs=collection_tarballs).debug("Download complete")
         flog.notice("Finished retrieving tarballs")
 
         # Get the ansible-core location
         if use_installed_ansible_core:
             ansible_core_path = None
         else:
             try:
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/ansible_2_10_routing.yml` & `antsibull_docs-2.3.0/src/antsibull_docs/data/ansible_2_10_routing.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2`

 * *Files 16% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 See :ref:`list_of_callback_plugins` for the list of *all* callback plugins.
 
 {% for collection_name, plugins in per_collection_plugins.items() | sort %}
 @{ collection_name }@
 @{ '-' * (collection_name | length) }@
 
 {%   for plugin_name, plugin_desc in plugins.items() | sort %}
-* :ref:`@{ collection_name }@.@{ plugin_name }@ <ansible_collections.@{ collection_name }@.@{ plugin_name }@_callback>` -- @{ plugin_desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ plugin_name, plugin_type='callback') }@
+* :ansplugin:`@{ collection_name }@.@{ plugin_name }@#callback` -- @{ plugin_desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ plugin_name, plugin_type='callback') }@
 {%   endfor %}
 
 {% else %}
 No public @{ callback_type }@ callback plugin found.
 {% endfor %}
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 {% set plugins_ = [] %}
 {%   for plugin_type, plugins in env_var.plugins.items() %}
 {%     for plugin_name in plugins %}
 {%       set _ = plugins_.append((plugin_name, plugin_type)) %}
 {%     endfor %}
 {%   endfor %}
 {%   for plugin_name, plugin_type in plugins_ | unique | sort %}
-    :ref:`@{ plugin_name | rst_escape }@ {% if plugin_type == 'module' %}module{% else %}@{ plugin_type }@ plugin{% endif %} <ansible_collections.@{ plugin_name }@_@{ plugin_type }@>`
+    :ansplugin:`@{ plugin_name | rst_escape }@ {% if plugin_type == 'module' %}module{% else %}@{ plugin_type }@ plugin{% endif %} <@{ plugin_name }@#@{ plugin_type }@>`
 {%-    if not loop.last -%}
 ,
 {%     endif -%}
 {%-  endfor %}
 
 {% else %}
 No environment variables have been defined.
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2`

 * *Files 10% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 {% endif %}
 
 {% for collection_name, plugins in per_collection_plugins.items() | sort %}
 @{ collection_name }@
 @{ '-' * (collection_name | length) }@
 
 {%   for plugin_name, plugin_desc in plugins.items() | sort %}
-* :ref:`@{ collection_name }@.@{ plugin_name }@ <ansible_collections.@{ collection_name }@.@{ plugin_name }@_@{ plugin_type }@>` -- @{ plugin_desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ plugin_name, plugin_type=plugin_type) }@
+* :ansplugin:`@{ collection_name }@.@{ plugin_name }@#@{ plugin_type }@` -- @{ plugin_desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ plugin_name, plugin_type=plugin_type) }@
 {%   endfor %}
 
 {% else %}
 No {% if plugin_type == 'module' %}module{% elif plugin_type == 'role' %}role{% else %}@{ plugin_type }@ plugin{% endif %} found.
 {% endfor %}
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   It will be removed in version @{ deprecation.removal_version | rst_ify }@ of @{ collection }@.
 {%   elif deprecation.removal_date is defined %}
   It will be removed in a major release after @{ deprecation.removal_date | rst_ify }@ of @{ collection }@.
 {%   else %}
   It will eventually be removed from @{ collection_name }@.
 {%   endif %}
 {% endif %}
-- This is a redirect to the :ref:`@{ redirect }@ {% if plugin_type == 'module' %}module{% else %}@{ plugin_type }@ plugin{% endif %} <ansible_collections.@{ redirect }@_@{ plugin_type }@>`.
+- This is a redirect to the :ansplugin:`@{ redirect }@ {% if plugin_type == 'module' %}module{% else %}@{ plugin_type }@ plugin{% endif %} <@{ redirect }@#@{ plugin_type }@>`.
 {% if collection != 'ansible.builtin' -%}
 {%   if redirect_is_symlink %}
 - This redirect also works with Ansible 2.9.
 {%   else %}
 - This redirect does **not** work with Ansible 2.9.
 {%   endif %}
 {% endif %}
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,14 @@
 .. Anchors: short name for ansible.builtin
 
 {% if collection == 'ansible.builtin' -%}
 {# ansible.builtins get shortname anchors as well #}
 .. _@{ doc['name'] }@_@{ plugin_type }@:
 {% endif -%}
 
-.. Anchors: aliases
-
-{# TODO: This assumes that aliases will be short names.
-   If they're FQCN, then we need to change this
-#}
-
-{% for alias in doc['aliases'] -%}
-.. _ansible_collections.@{collection}@.@{ alias }@_@{ plugin_type }@:
-{% endfor %}
-
 .. Title
 
 {% if doc['short_description'] -%}
 {%   set title = plugin_name ~ ' ' ~ plugin_type ~ ' -- ' ~ doc['short_description'] | rst_ify -%}
 {% else -%}
 {%   set title = plugin_name ~ ' ' ~ plugin_type -%}
 {% endif -%}
@@ -168,15 +158,15 @@
 .. note::
     This module has a corresponding :ref:`action plugin <action_plugins>`.
 {% endif %}
 
 .. Aliases
 
 {% if doc['aliases'] -%}
-Aliases: @{ ','.join(aliases) }@
+Aliases: @{ ', '.join(doc['aliases'] | sort) }@
 {% endif %}
 
 .. Requirements
 
 {% if doc['requirements'] -%}
 .. _ansible_collections.@{plugin_name}@_@{plugin_type}@_requirements:
 
@@ -329,30 +319,30 @@
 --------
 
 .. seealso::
 
 {% for item in doc['seealso'] %}
 {%   if item.module is defined and item.description %}
    @{ reference_plugin_rst(item['module'], 'module') }@
-       @{ item['description'] | rst_ify }@
+       @{ item['description'] | rst_ify | indent(7) }@
 {%   elif item.module is defined %}
    @{ reference_plugin_rst(item['module'], 'module') }@
        The official documentation on the **@{ item['module'] }@** module.
 {%   elif item.plugin is defined and item.plugin_type is defined and item.description %}
    @{ reference_plugin_rst(item['plugin'], item['plugin_type']) }@ @{ item['plugin_type'] }@ plugin
-       @{ item['description'] | rst_ify }@
+       @{ item['description'] | rst_ify | indent(7) }@
 {%   elif item.plugin is defined and item.plugin_type is defined %}
    @{ reference_plugin_rst(item['plugin'], item['plugin_type']) }@ @{ item['plugin_type'] }@ plugin
        The official documentation on the **@{ item['plugin'] }@** @{ item['plugin_type'] }@ plugin.
 {%   elif item.name is defined and item.link is defined and item.description %}
    `@{ item['name'] }@ <@{ item['link'] }@>`_
-       @{ item['description'] | rst_ify }@
+       @{ item['description'] | rst_ify | indent(7) }@
 {%   elif item.ref is defined and item.description %}
    :ref:`@{ item['ref'] }@`
-       @{ item['description'] | rst_ify }@
+       @{ item['description'] | rst_ify | indent(7) }@
 {%   endif %}
 {% endfor %}
 {% endif %}
 
 .. Examples
 
 {% if examples -%}
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 {% if not breadcrumbs %}
 :orphan:
 {% endif %}
 
 {% macro list_plugins(plugin_type) %}
 {%   for name, desc in plugin_maps[plugin_type].items() | sort %}
-* :ref:`@{ name }@ @{ plugin_type }@ <ansible_collections.@{ collection_name }@.@{ name }@_@{ plugin_type }@>` -- @{ desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ name, plugin_type=plugin_type) | indent(width=2) }@
+* :ansplugin:`@{ name }@ @{ plugin_type }@ <@{ collection_name }@.@{ name }@#@{ plugin_type }@>` -- @{ desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ name, plugin_type=plugin_type) | indent(width=2) }@
 {%   endfor %}
 {%   if breadcrumbs %}
 
 .. toctree::
     :maxdepth: 1
     :hidden:
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
 {# Copyright (c) Ansible Project GNU General Public License v3.0+ (see
 LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later #} {% if not breadcrumbs %} :orphan:
 {% endif %} {% macro list_plugins(plugin_type) %} {% for name, desc in
-plugin_maps[plugin_type].items() | sort %} * :ref:`@{ name }@ @{ plugin_type }@
-@{ collection_name }@.@{ name }@_@{ plugin_type }@>` -- @{ desc | rst_ify
-(plugin_fqcn=collection_name ~ '.' ~ name, plugin_type=plugin_type) | indent
-(width=2) }@ {% endfor %} {% if breadcrumbs %} .. toctree:: :maxdepth: 1 :
-hidden: {% for name in plugin_maps[plugin_type] | sort %} @{ name }@_@
-{ plugin_type }@ {% endfor %} {% endif %} {% endmacro %} .. _plugins_in_@
-{collection_name}@: @{collection_name.title()}@ @{ '=' * (collection_name |
-length) }@ {% if collection_version %} Collection version @{ collection_version
-}@ {% endif %} .. contents:: :local: :depth: 1 {% if collection_description or
-collection_authors or collection_links or requires_ansible %} Description -----
------- {% if collection_description %} @{ link_data.description | rst_ify }@ {%
-endif %} {% if collection_authors %} **Author@{ 's' if (collection_authors |
-length) > 1 else '' }@:** {% for author in collection_authors %} * @{ author |
-indent(2) }@ {% endfor %} {% endif %} {% if requires_ansible %} **Supported
-ansible-core versions:** {% for part in requires_ansible %} * @{ part |
-rst_escape }@ {% endfor %} {% endif %} {% if collection_links %} .. raw:: html
+plugin_maps[plugin_type].items() | sort %} * :ansplugin:`@{ name }@ @
+{ plugin_type }@ <@{ collection_name }@.@{ name }@#@{ plugin_type }@>` -- @
+{ desc | rst_ify(plugin_fqcn=collection_name ~ '.' ~ name,
+plugin_type=plugin_type) | indent(width=2) }@ {% endfor %} {% if breadcrumbs %}
+.. toctree:: :maxdepth: 1 :hidden: {% for name in plugin_maps[plugin_type] |
+sort %} @{ name }@_@{ plugin_type }@ {% endfor %} {% endif %} {% endmacro %} ..
+_plugins_in_@{collection_name}@: @{collection_name.title()}@ @{ '=' *
+(collection_name | length) }@ {% if collection_version %} Collection version @
+{ collection_version }@ {% endif %} .. contents:: :local: :depth: 1 {% if
+collection_description or collection_authors or collection_links or
+requires_ansible %} Description ----------- {% if collection_description %} @
+{ link_data.description | rst_ify }@ {% endif %} {% if collection_authors %}
+**Author@{ 's' if (collection_authors | length) > 1 else '' }@:** {% for author
+in collection_authors %} * @{ author | indent(2) }@ {% endfor %} {% endif %} {%
+if requires_ansible %} **Supported ansible-core versions:** {% for part in
+requires_ansible %} * @{ part | rst_escape }@ {% endfor %} {% endif %} {% if
+collection_links %} .. raw:: html
 {% for link in collection_links %} @{_link.description_|_escape_}@ {% endfor %}
 {% endif %} {% endif %} {% if not collection_communication.empty %} ..
 Communication .. _communication_for_@{collection_name}@: Communication --------
 ----- {% for matrix_room in collection_communication.matrix_rooms %} - Matrix
 room :literal:`@{ matrix_room.room | rst_escape(escape_ending_whitespace=true)
 }@`: `@{ matrix_room.topic | rst_escape }@
 matrix.to/#/@{ matrix_room.room | rst_escape }@>`__. {% endfor %} {% for
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 :source: @{ source }@
 -#}
 
 .. Anchors
 
 .. _ansible_collections.@{plugin_name}@_@{plugin_type}@:
 
-.. Anchors: aliases
-
-{# TODO: This assumes that aliases will be short names.
-   If they're FQCN, then we need to change this
-#}
-
 .. Title
 
 {% if entry_points.main and entry_points.main.short_description -%}
 {%   set title = plugin_name ~ ' ' ~ plugin_type ~ ' -- ' ~ entry_points.main.short_description | rst_ify(role_entrypoint='main') -%}
 {% else -%}
 {%   set title = plugin_name ~ ' ' ~ plugin_type -%}
 {% endif -%}
@@ -184,30 +178,30 @@
 ^^^^^^^^
 
 .. seealso::
 
 {%     for item in ep_doc['seealso'] %}
 {%       if item.module is defined and item.description %}
    @{ reference_plugin_rst(item['module'], 'module') }@
-       @{ item['description'] | rst_ify(role_entrypoint=entry_point) }@
+       @{ item['description'] | rst_ify(role_entrypoint=entry_point) | indent(7) }@
 {%       elif item.module is defined %}
    @{ reference_plugin_rst(item['module'], 'module') }@
        The official documentation on the **@{ item['module'] }@** module.
 {%       elif item.plugin is defined and item.plugin_type is defined and item.description %}
    @{ reference_plugin_rst(item['plugin'], item['plugin_type']) }@ @{ item['plugin_type'] }@ plugin
-       @{ item['description'] | rst_ify(role_entrypoint=entry_point) }@
+       @{ item['description'] | rst_ify(role_entrypoint=entry_point) | indent(7) }@
 {%       elif item.plugin is defined and item.plugin_type is defined %}
    @{ reference_plugin_rst(item['plugin'], item['plugin_type']) }@ @{ item['plugin_type'] }@ plugin
        The official documentation on the **@{ item['plugin'] }@** @{ item['plugin_type'] }@ plugin.
 {%       elif item.name is defined and item.link is defined and item.description %}
    `@{ item['name'] }@ <@{ item['link'] }@>`_
-       @{ item['description'] | rst_ify(role_entrypoint=entry_point) }@
+       @{ item['description'] | rst_ify(role_entrypoint=entry_point) | indent(7) }@
 {%       elif item.ref is defined and item.description %}
    :ref:`@{ item['ref'] }@`
-       @{ item['description'] | rst_ify(role_entrypoint=entry_point) }@
+       @{ item['description'] | rst_ify(role_entrypoint=entry_point) | indent(7) }@
 {%       endif %}
 {%     endfor %}
 {%   endif %}
 
 {%   if ep_doc['author'] -%}
 Authors
 ^^^^^^^
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/build_sh.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/build_sh.j2`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 {%     endif %}
 {%     if collection_version != '@latest' %}
     --collection-version @{ collection_version }@ \
 {%     endif %}
 {%     if squash_hierarchy %}
     --squash-hierarchy \
 {%     endif %}
+    --output-format @{ output_format }@ \
     --dest-dir temp-rst \
     @{ ' '.join(collections) }@
 {% endif %}
 
 # Copy collection documentation into source directory
 {% if squash_hierarchy %}
 rsync -cprv --delete-after temp-rst/ rst/
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/conf_py.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/conf_py.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2` & `antsibull_docs-2.3.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/__init__.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/ansible_doc.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/fqcn.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/fqcn.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/parsing.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/parsing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/docs_parsing/routing.py` & `antsibull_docs-2.3.0/src/antsibull_docs/docs_parsing/routing.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from __future__ import annotations
 
 import asyncio
 import datetime
 import os
 import typing as t
 from collections import defaultdict
-from collections.abc import Mapping, MutableMapping
+from collections.abc import Mapping, MutableMapping, Sequence
 
 import asyncio_pool  # type: ignore[import]
 from antsibull_core import app_context, yaml
 from antsibull_core.utils.collections import compare_all_but
 
 from ..constants import DOCUMENTABLE_PLUGINS
 from ..utils.get_pkg_data import get_antsibull_data
@@ -256,14 +256,37 @@
                 plugin_type_routing[redirect_name] = {}
             if "redirect" not in plugin_type_routing[redirect_name]:
                 plugin_type_routing[redirect_name]["redirect"] = redirect_dst
             if plugin_type_routing[redirect_name]["redirect"] == redirect_dst:
                 plugin_type_routing[redirect_name]["redirect_is_symlink"] = True
 
 
+def _add_core_symlink_redirects(
+    collection_metadata: AnsibleCollectionMetadata,
+    plugin_routing_out: dict[str, dict[str, dict[str, t.Any]]],
+) -> None:
+    for plugin_type in DOCUMENTABLE_PLUGINS:
+        directory_name = (
+            "modules"
+            if plugin_type == "module"
+            else os.path.join("plugins", plugin_type)
+        )
+        directory_path = os.path.join(collection_metadata.path, directory_name)
+        plugin_type_routing = plugin_routing_out[plugin_type]
+
+        symlink_redirects = find_symlink_redirects(
+            "ansible.builtin", plugin_type, directory_path
+        )
+        for redirect_name, redirect_dst in symlink_redirects.items():
+            if redirect_name not in plugin_type_routing:
+                plugin_type_routing[redirect_name] = {}
+            if "redirect" not in plugin_type_routing[redirect_name]:
+                plugin_type_routing[redirect_name]["redirect"] = redirect_dst
+
+
 async def load_collection_routing(
     collection_name: str, collection_metadata: AnsibleCollectionMetadata
 ) -> dict[str, dict[str, dict[str, t.Any]]]:
     """
     Load plugin routing for a collection.
     """
     meta_runtime = load_meta_runtime(collection_name, collection_metadata)
@@ -276,14 +299,15 @@
             f"{collection_name}.{plugin_name}": process_dates(plugin_record)
             for plugin_name, plugin_record in plugin_type_routing.items()
         }
 
     if collection_name == "ansible.builtin":
         # ansible-core has a special directory structure we currently do not want
         # (or need) to handle
+        _add_core_symlink_redirects(collection_metadata, plugin_routing_out)
         return plugin_routing_out
 
     _add_symlink_redirects(collection_name, collection_metadata, plugin_routing_out)
 
     if collection_name in COLLECTIONS_WITH_FLATMAPPING:
         remove_flatmapping_artifacts(plugin_routing_out)
 
@@ -312,55 +336,83 @@
             global_plugin_routing[plugin_type].update(
                 collection_plugin_routing[plugin_type]
             )
 
     return global_plugin_routing
 
 
+def _add_meta_redirect_for_aliases(
+    plugin_map: MutableMapping[str, t.Any],
+    plugin_routing: MutableMapping[str, MutableMapping[str, t.Any]],
+) -> None:
+    for plugin_name, plugin_record in plugin_map.items():
+        if isinstance(plugin_record.get("doc"), Mapping) and isinstance(
+            plugin_record["doc"].get("aliases"), Sequence
+        ):
+            for alias in plugin_record["doc"]["aliases"]:
+                alias_fqcn = f"ansible.builtin.{alias}"
+                if alias_fqcn not in plugin_routing:
+                    plugin_routing[alias_fqcn] = {}
+                if "redirect" not in plugin_routing[alias_fqcn]:
+                    plugin_routing[alias_fqcn]["redirect"] = plugin_name
+
+
+def _remove_redirect_duplicates(
+    plugin_map: MutableMapping[str, t.Any],
+    plugin_routing: MutableMapping[str, MutableMapping[str, t.Any]],
+) -> None:
+    for plugin_name, plugin_record in list(plugin_map.items()):
+        if plugin_name in plugin_routing and "redirect" in plugin_routing[plugin_name]:
+            destination = plugin_routing[plugin_name]["redirect"]
+            if destination in plugin_map and destination != plugin_name:
+                # Heuristic: if we have a redirect, and docs for both this plugin and the
+                # redirected one are generated from the same plugin filename, then we can
+                # remove this plugin's docs and generate a redirect stub instead.
+                a = plugin_record.get("doc")
+                b = plugin_map[destination].get("doc")
+                if a and b and compare_all_but(a, b, ["filename"]):
+                    del plugin_map[plugin_name]
+
+
+def _remove_other_duplicates(
+    plugin_type: str,
+    plugin_map: MutableMapping[str, t.Any],
+    plugin_routing: MutableMapping[str, MutableMapping[str, t.Any]],
+) -> None:
+    # In some cases, both the plugin and its aliases will be listed.
+    # Basically look for plugins whose name is wrong, a plugin with that
+    # name exists, and whose docs are identical.
+    for plugin_name, plugin_record in list(plugin_map.items()):
+        doc = plugin_record.get("doc") or {}
+        name = doc.get("module" if plugin_type == "module" else "name")
+        collection_name = ".".join(plugin_name.split(".")[:2])
+        full_name = f"{collection_name}.{name}"
+        if full_name and full_name != plugin_name and full_name in plugin_map:
+            a = plugin_record.get("doc")
+            b = plugin_map[full_name].get("doc")
+            if a and b and compare_all_but(a, b, ["name", "filename"]):
+                del plugin_map[plugin_name]
+                if plugin_name not in plugin_routing:
+                    plugin_routing[plugin_name] = {}
+                plugin_routing[plugin_name]["redirect"] = full_name
+
+
 def remove_redirect_duplicates(
     plugin_info: MutableMapping[str, MutableMapping[str, t.Any]],
     collection_routing: MutableCollectionRoutingT,
 ) -> None:
     """
     Remove duplicate plugin docs that come from symlinks (or once ansible-docs supports them,
     other plugin routing redirects).
     """
     for plugin_type, plugin_map in plugin_info.items():
         plugin_routing = collection_routing[plugin_type]
-        for plugin_name, plugin_record in list(plugin_map.items()):
-            # Check redirect
-            if (
-                plugin_name in plugin_routing
-                and "redirect" in plugin_routing[plugin_name]
-            ):
-                destination = plugin_routing[plugin_name]["redirect"]
-                if destination in plugin_map and destination != plugin_name:
-                    # Heuristic: if we have a redirect, and docs for both this plugin and the
-                    # redirected one are generated from the same plugin filename, then we can
-                    # remove this plugin's docs and generate a redirect stub instead.
-                    a = plugin_record.get("doc")
-                    b = plugin_map[destination].get("doc")
-                    if a and b and compare_all_but(a, b, ["filename"]):
-                        del plugin_map[plugin_name]
-
-        # For filters and tests, both the plugin and its aliases will be listed. Basically
-        # look for plugins whose name is wrong, a plugin with that name exists, and whose
-        # docs are identical
-        for plugin_name, plugin_record in list(plugin_map.items()):
-            name = (plugin_record.get("doc") or {}).get("name")
-            collection_name = ".".join(plugin_name.split(".")[:2])
-            full_name = f"{collection_name}.{name}"
-            if full_name and full_name != plugin_name and full_name in plugin_map:
-                a = plugin_record.get("doc")
-                b = plugin_map[full_name].get("doc")
-                if a and b and compare_all_but(a, b, ["name", "filename"]):
-                    del plugin_map[plugin_name]
-                    if plugin_name not in plugin_routing:
-                        plugin_routing[plugin_name] = {}
-                    plugin_routing[plugin_name]["redirect"] = full_name
+        _add_meta_redirect_for_aliases(plugin_map, plugin_routing)
+        _remove_redirect_duplicates(plugin_map, plugin_routing)
+        _remove_other_duplicates(plugin_type, plugin_map, plugin_routing)
 
 
 def find_stubs(
     plugin_info: MutableMapping[str, MutableMapping[str, t.Any]],
     collection_routing: CollectionRoutingT,
 ) -> defaultdict[str, defaultdict[str, dict[str, t.Any]]]:
     """
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/jinja2/environment.py` & `antsibull_docs-2.3.0/src/antsibull_docs/jinja2/environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,74 +2,72 @@
 # https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2019-2020, Ansible Project
 """Create Jinja2 environment for rendering Ansible documentation."""
 
 from __future__ import annotations
 
-import json
 import os.path
 import typing as t
 from collections.abc import Mapping
 
 from jinja2 import BaseLoader, Environment, FileSystemLoader, PackageLoader
 
 from ..markup.rstify import rst_code, rst_escape
 from ..utils.collection_name_transformer import CollectionNameTransformer
-from . import OutputFormat
+from . import FilenameGenerator, OutputFormat
 from .filters import (
-    do_max,
+    collection_name,
     documented_type,
     extract_options_from_list,
     html_ify,
     make_rst_ify,
     massage_author_name,
     move_first,
+    plugin_shortname,
     remove_options_from_list,
     rst_fmt,
     rst_xline,
+    suboption_depth,
     to_ini_value,
     to_json,
 )
 from .tests import still_relevant, test_list
 
-# kludge_ns gives us a kludgey way to set variables inside of loops that need to be visible outside
-# the loop.  We can get rid of this when we no longer need to build docs with less than Jinja-2.10
-# http://jinja.pocoo.org/docs/2.10/templates/#assignments
-# With Jinja-2.10 we can use jinja2's namespace feature, restoring the namespace template portion
-# of: fa5c0282a4816c4dd48e80b983ffc1e14506a1f5
-NS_MAP = {}
 
-
-def to_kludge_ns(key, value):
-    NS_MAP[key] = value
-    return ""
+def reference_plugin_rst(plugin_name: str, plugin_type: str) -> str:
+    fqcn = f"{plugin_name}"
+    return f"\\ :ref:`{rst_escape(fqcn)} <ansible_collections.{fqcn}_{plugin_type}>`\\ "
 
 
-def from_kludge_ns(key):
-    return NS_MAP[key]
+def reference_plugin_rst_simplified(plugin_name: str, plugin_type: str) -> str:
+    fqcn = f"{plugin_name}"
+    # TODO: return f"\\ {fqcn}\\ " for other collections
+    name = plugin_name.split(".", 2)[2]
+    return f"\\ `{rst_escape(fqcn)} <{name}_{plugin_type}.rst>`__\\ "
 
 
-def reference_plugin_rst(plugin_name: str, plugin_type: str) -> str:
-    fqcn = f"{plugin_name}"
-    return f"\\ :ref:`{rst_escape(fqcn)} <ansible_collections.{fqcn}_{plugin_type}>`\\ "
+def make_reference_plugin_rst(output_format: OutputFormat):
+    if output_format == OutputFormat.SIMPLIFIED_RST:
+        return reference_plugin_rst_simplified
+    return reference_plugin_rst
 
 
 def get_template_location(output_format: OutputFormat) -> tuple[str, str]:
     """
     Return template location given the output format.
     """
-    return ("antsibull_docs.data", f"docsite/{output_format.value}")
+    return ("antsibull_docs.data", f"docsite/{output_format.output_format}")
 
 
 def get_template_filename(filename_base: str, output_format: OutputFormat) -> str:
     """
     Return template filename given the filename base and the output format.
     """
-    return f"{filename_base}{output_format.extension}"
+    return f"{filename_base}{output_format.template_extension}"
 
 
 def _get_loader(
     template_location: str | tuple[str, str] | None, output_format: OutputFormat | None
 ) -> BaseLoader:
     if template_location is None:
         if output_format is None:
@@ -87,63 +85,78 @@
     else:
         template_pkg = template_location[0]
         template_path = template_location[1]
 
     return PackageLoader(template_pkg, template_path)
 
 
+def _create_filename_functions(
+    filename_generator: FilenameGenerator,
+    output_format: OutputFormat,
+) -> Mapping[str, t.Callable]:
+    def get_plugin_basename(plugin_fqcn: str, plugin_type: str) -> str:
+        return filename_generator.plugin_basename(plugin_fqcn, plugin_type)
+
+    def get_plugin_filename(plugin_fqcn: str, plugin_type: str) -> str:
+        return filename_generator.plugin_filename(
+            plugin_fqcn, plugin_type, output_format
+        )
+
+    return {
+        "get_plugin_basename": get_plugin_basename,
+        "get_plugin_filename": get_plugin_filename,
+    }
+
+
 def doc_environment(
     template_location: str | tuple[str, str] | None = None,
     *,
     extra_filters: Mapping[str, t.Callable] | None = None,
     extra_tests: Mapping[str, t.Callable] | None = None,
     collection_url: CollectionNameTransformer | None = None,
     collection_install: CollectionNameTransformer | None = None,
     referable_envvars: set[str] | None = None,
     output_format: OutputFormat | None = None,
+    filename_generator: FilenameGenerator | None = None,
 ) -> Environment:
     loader = _get_loader(template_location, output_format)
     if output_format is None:
         output_format = OutputFormat.ANSIBLE_DOCSITE
 
     env = Environment(
         loader=loader,
         variable_start_string="@{",
         variable_end_string="}@",
         trim_blocks=True,
     )
     env.globals["xline"] = rst_xline
 
-    # Can be removed (and template switched to use namespace) when we no longer need to build
-    # with <Jinja-2.10
-    env.globals["to_kludge_ns"] = to_kludge_ns
-    env.globals["from_kludge_ns"] = from_kludge_ns
-    if "max" not in env.filters:
-        # Jinja < 2.10
-        env.filters["max"] = do_max
-
-    if "tojson" not in env.filters:
-        # Jinja < 2.9
-        env.filters["tojson"] = json.dumps
+    if filename_generator:
+        env.globals.update(
+            _create_filename_functions(filename_generator, output_format)
+        )
 
-    env.globals["reference_plugin_rst"] = reference_plugin_rst
+    env.globals["reference_plugin_rst"] = make_reference_plugin_rst(output_format)
     env.globals["referable_envvars"] = referable_envvars
     env.filters["rst_ify"] = make_rst_ify(output_format)
     env.filters["html_ify"] = html_ify
     env.filters["fmt"] = rst_fmt
     env.filters["rst_code"] = rst_code
     env.filters["rst_escape"] = rst_escape
     env.filters["xline"] = rst_xline
     env.filters["documented_type"] = documented_type
     env.filters["move_first"] = move_first
     env.filters["massage_author_name"] = massage_author_name
     env.filters["extract_options_from_list"] = extract_options_from_list
     env.filters["remove_options_from_list"] = remove_options_from_list
     env.filters["antsibull_to_json"] = to_json
     env.filters["antsibull_to_ini_value"] = to_ini_value
+    env.filters["collection_name"] = collection_name
+    env.filters["plugin_shortname"] = plugin_shortname
+    env.filters["suboption_depth"] = suboption_depth
     if collection_url is not None:
         env.filters["collection_url"] = collection_url
     if collection_install is not None:
         env.filters["collection_install"] = collection_install
     if extra_filters:
         env.filters.update(extra_filters)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/jinja2/filters.py` & `antsibull_docs-2.3.0/src/antsibull_docs/jinja2/filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,36 +14,42 @@
 from collections.abc import Mapping, Sequence
 
 from antsibull_core.logging import log
 from jinja2.runtime import Context, Undefined
 from jinja2.utils import pass_context
 
 from ..markup.htmlify import html_ify as html_ify_impl
-from ..markup.rstify import get_rst_formatter
+from ..markup.rstify import get_rst_formatter_link_provider
 from ..markup.rstify import rst_ify as rst_ify_impl
 from . import OutputFormat
 
 mlog = log.fields(mod=__name__)
 
 _EMAIL_ADDRESS = re.compile(
     r"(?:<{mail}>|\({mail}\)|{mail})".format(mail=r"[\w.+-]+@[\w.-]+\.\w+")
 )
 
 
 def extract_plugin_data(
     context: Context, plugin_fqcn: str | None = None, plugin_type: str | None = None
-) -> tuple[str | None, str | None]:
-    plugin_fqcn = context.get("plugin_name") if plugin_fqcn is None else plugin_fqcn
-    plugin_type = context.get("plugin_type") if plugin_type is None else plugin_type
+) -> tuple[str | None, str | None, str | None, str | None]:
+    # The doc plugin is determined by the current page
+    doc_plugin_fqcn = context.get("plugin_name")
+    doc_plugin_type = context.get("plugin_type")
+    if doc_plugin_fqcn is None or doc_plugin_type is None:
+        doc_plugin_fqcn = doc_plugin_type = None
+
+    # The current plugin for this markup is determined by the parameters,
+    # with fallback to the doc plugin
+    plugin_fqcn = doc_plugin_fqcn if plugin_fqcn is None else plugin_fqcn
+    plugin_type = doc_plugin_type if plugin_type is None else plugin_type
     if plugin_fqcn is None or plugin_type is None:
-        return None, None
-    # if plugin_type == 'role':
-    #     entry_point = context.get('entry_point', 'main')
-    #     # FIXME: use entry_point
-    return plugin_fqcn, plugin_type
+        plugin_fqcn = plugin_type = None
+
+    return doc_plugin_fqcn, doc_plugin_type, plugin_fqcn, plugin_type
 
 
 def documented_type(text) -> str:
     """Convert any python type to a type for documentation"""
 
     if isinstance(text, Undefined):
         return "-"
@@ -54,19 +60,14 @@
     if text == "int":
         return "integer"
     if text == "dict":
         return "dictionary"
     return text
 
 
-# The max filter was added in Jinja2-2.10.  Until we can require that version, use this
-def do_max(seq):
-    return max(seq)
-
-
 def rst_fmt(text, fmt):
     """helper for Jinja2 to do format strings"""
 
     return fmt % (text)
 
 
 def rst_xline(width, char="="):
@@ -151,25 +152,37 @@
         plugin_type: str | None = None,
         role_entrypoint: str | None = None,
     ) -> str:
         """convert symbols like I(this is in italics) to valid restructured text"""
         flog = mlog.fields(func="rst_ify")
         flog.fields(text=text).debug("Enter")
 
-        plugin_fqcn, plugin_type = extract_plugin_data(
-            context, plugin_fqcn=plugin_fqcn, plugin_type=plugin_type
+        (
+            doc_plugin_fqcn,
+            doc_plugin_type,
+            plugin_fqcn,
+            plugin_type,
+        ) = extract_plugin_data(
+            context,
+            plugin_fqcn=plugin_fqcn,
+            plugin_type=plugin_type,
         )
 
-        formatter = get_rst_formatter(output_format, context.get("referable_envvars"))
+        formatter, link_provider = get_rst_formatter_link_provider(
+            output_format, context.get("referable_envvars")
+        )
         text, counts = rst_ify_impl(
             text,
             plugin_fqcn=plugin_fqcn,
             plugin_type=plugin_type,
             role_entrypoint=role_entrypoint,
+            doc_plugin_fqcn=doc_plugin_fqcn,
+            doc_plugin_type=doc_plugin_type,
             formatter=formatter,
+            link_provider=link_provider,
         )
 
         flog.fields(counts=counts).info("Number of macros converted to rst equivalents")
         flog.debug("Leave")
         return text
 
     return rst_ify
@@ -184,21 +197,44 @@
     plugin_type: str | None = None,
     role_entrypoint: str | None = None,
 ) -> str:
     """convert symbols like I(this is in italics) to valid HTML"""
     flog = mlog.fields(func="html_ify")
     flog.fields(text=text).debug("Enter")
 
-    plugin_fqcn, plugin_type = extract_plugin_data(
-        context, plugin_fqcn=plugin_fqcn, plugin_type=plugin_type
+    doc_plugin_fqcn, doc_plugin_type, plugin_fqcn, plugin_type = extract_plugin_data(
+        context,
+        plugin_fqcn=plugin_fqcn,
+        plugin_type=plugin_type,
     )
 
     text, counts = html_ify_impl(
         text,
         plugin_fqcn=plugin_fqcn,
         plugin_type=plugin_type,
         role_entrypoint=role_entrypoint,
+        doc_plugin_fqcn=doc_plugin_fqcn,
+        doc_plugin_type=doc_plugin_type,
     )
 
     flog.fields(counts=counts).info("Number of macros converted to html equivalents")
     flog.debug("Leave")
     return text
+
+
+def collection_name(fqcn: str) -> str:
+    return ".".join(fqcn.split(".", 2)[:2])
+
+
+def plugin_shortname(fqcn: str) -> str:
+    return fqcn.split(".", 2)[2]
+
+
+def suboption_depth(
+    data: Sequence[tuple[t.Any, t.Any]] | t.ItemsView[t.Any, t.Any], subkey: str
+) -> int:
+    subdepth = 0
+    for _, option in data:
+        subdata = option.get(subkey)
+        if subdata and isinstance(subdata, Mapping):
+            subdepth = max(subdepth, suboption_depth(subdata.items(), subkey))
+    return subdepth + 1
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/jinja2/tests.py` & `antsibull_docs-2.3.0/src/antsibull_docs/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/markup/_counter.py` & `antsibull_docs-2.3.0/src/antsibull_docs/markup/_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/markup/htmlify.py` & `antsibull_docs-2.3.0/src/antsibull_docs/markup/htmlify.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,24 +43,31 @@
 
 def html_ify(
     text: str,
     *,
     plugin_fqcn: str | None = None,
     plugin_type: str | None = None,
     role_entrypoint: str | None = None,
+    doc_plugin_fqcn: str | None = None,
+    doc_plugin_type: str | None = None,
 ) -> tuple[str, Mapping[str, int]]:
     """convert symbols like I(this is in italics) to valid HTML"""
     current_plugin: dom.PluginIdentifier | None = None
     if plugin_fqcn and plugin_type:
         current_plugin = dom.PluginIdentifier(fqcn=plugin_fqcn, type=plugin_type)
+    doc_current_plugin: dom.PluginIdentifier | None = None
+    if doc_plugin_fqcn and doc_plugin_type:
+        doc_current_plugin = dom.PluginIdentifier(
+            fqcn=doc_plugin_fqcn, type=doc_plugin_type
+        )
     context = Context(current_plugin=current_plugin, role_entrypoint=role_entrypoint)
     paragraphs = parse(text, context, errors="message")
     link_provider = _HTMLLinkProvider()
     text = to_html(
         paragraphs,
         link_provider=link_provider,
-        current_plugin=current_plugin,
+        current_plugin=doc_current_plugin,
         par_start="",
         par_end="",
     )
     counts = _count(paragraphs)
     return text, counts
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/markup/semantic_helper.py` & `antsibull_docs-2.3.0/src/antsibull_docs/markup/semantic_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from __future__ import annotations
 
 import re
 
 _ARRAY_STUB_RE = re.compile(r"\[([^\]]*)\]")
 _ARRAY_STUB_SEP_START_RE = re.compile(r"[\[.]")
+_FQCN_TYPE_RE = re.compile(r"^([^.]+\.[^.]+\.[^#]+)#([a-z]+)$")
 _FQCN_TYPE_PREFIX_RE = re.compile(r"^([^.]+\.[^.]+\.[^#]+)#([a-z]+):(.*)$")
 _IGNORE_MARKER = "ignore:"
 
 
 def _remove_array_stubs(text: str) -> str:
     return _ARRAY_STUB_RE.sub("", text)
 
@@ -119,7 +120,14 @@
             index += 1
             continue
         raise ValueError(
             f'Expecting separator ".", but got "{name[index]!r}"'
             f" at position {index + 1} of {name!r}"
         )
     return result
+
+
+def parse_plugin_name(text: str) -> tuple[str, str]:
+    m = _FQCN_TYPE_RE.match(text)
+    if not m:
+        raise ValueError("Cannot extract plugin name and type")
+    return m.group(1), m.group(2)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/ansible_doc.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/app_context.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/collection_config.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/collection_links.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/__init__.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/ansible_doc.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/base.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/base.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/callback.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/callback.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/module.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/module.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/plugin.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/positional.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/positional.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/schemas/docs/role.py` & `antsibull_docs-2.3.0/src/antsibull_docs/schemas/docs/role.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/utils/collection_name_transformer.py` & `antsibull_docs-2.3.0/src/antsibull_docs/utils/collection_name_transformer.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/utils/get_pkg_data.py` & `antsibull_docs-2.3.0/src/antsibull_docs/utils/get_pkg_data.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/vendored/ansible.py` & `antsibull_docs-2.3.0/src/antsibull_docs/vendored/ansible.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/__init__.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/collections.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from antsibull_core.utils.io import copy_file, write_file
 from jinja2 import Template
 from packaging.specifiers import SpecifierSet
 
 from ..collection_links import CollectionLinks
 from ..docs_parsing import AnsibleCollectionMetadata
 from ..extra_docs import CollectionExtraDocsInfoT
-from ..jinja2.environment import OutputFormat, doc_environment, get_template_filename
+from ..jinja2 import FilenameGenerator, OutputFormat
+from ..jinja2.environment import doc_environment, get_template_filename
 from ..utils.collection_name_transformer import CollectionNameTransformer
 from . import CollectionInfoT, _render_template
 
 mlog = log.fields(mod=__name__)
 
 
 def _parse_required_ansible(requires_ansible: str) -> list[str]:
@@ -57,14 +58,16 @@
     collection_name: str,
     plugin_maps: Mapping[str, Mapping[str, str]],
     template: Template,
     dest_dir: str,
     collection_meta: AnsibleCollectionMetadata,
     extra_docs_data: CollectionExtraDocsInfoT,
     link_data: CollectionLinks,
+    output_format: OutputFormat,
+    filename_generator: FilenameGenerator,  # pylint: disable=unused-argument
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
     squash_hierarchy: bool = False,
 ) -> None:
     """
     Write an index page for each collection.
 
@@ -115,15 +118,15 @@
         for_official_docsite=for_official_docsite,
         squash_hierarchy=squash_hierarchy,
     )
 
     # This is only safe because we made sure that the top of the directory tree we're writing to
     # (docs/docsite/rst) is only writable by us.
     os.makedirs(dest_dir, mode=0o755, exist_ok=True)
-    index_file = os.path.join(dest_dir, "index.rst")
+    index_file = os.path.join(dest_dir, f"index{output_format.output_extension}")
 
     await write_file(index_file, index_contents)
 
     flog.debug("Leave")
 
 
 async def output_indexes(
@@ -131,14 +134,15 @@
     dest_dir: str,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     extra_docs_data: Mapping[str, CollectionExtraDocsInfoT],
     link_data: Mapping[str, CollectionLinks],
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     squash_hierarchy: bool = False,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate collection-level index pages for the collections.
@@ -165,14 +169,15 @@
         collection_metadata = {}
 
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     collection_plugins_tmpl = env.get_template(
         get_template_filename("plugins_by_collection", output_format)
     )
 
     writers = []
@@ -203,14 +208,16 @@
                         collection_name,
                         plugin_maps,
                         collection_plugins_tmpl,
                         collection_dir,
                         collection_metadata[collection_name],
                         extra_docs_data[collection_name],
                         link_data[collection_name],
+                        output_format,
+                        filename_generator,
                         breadcrumbs=breadcrumbs,
                         for_official_docsite=for_official_docsite,
                         squash_hierarchy=squash_hierarchy,
                     )
                 )
             )
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/hierarchy.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 
 import asyncio_pool  # type: ignore[import]
 from antsibull_core import app_context
 from antsibull_core.logging import log
 from antsibull_core.utils.io import write_file
 from jinja2 import Template
 
-from ..jinja2.environment import OutputFormat, doc_environment, get_template_filename
+from ..jinja2 import FilenameGenerator, OutputFormat
+from ..jinja2.environment import doc_environment, get_template_filename
 from ..utils.collection_name_transformer import CollectionNameTransformer
 from . import CollectionInfoT, _render_template
 
 mlog = log.fields(mod=__name__)
 
 
 async def write_collection_list(
     collections: Iterable[str],
     namespaces: Iterable[str],
     template: Template,
     dest_dir: str,
+    output_format: OutputFormat,
+    filename_generator: FilenameGenerator,  # pylint: disable=unused-argument
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
 ) -> None:
     """
     Write an index page listing all of the collections.
 
     Each collection will link to an index page listing all content in the collection.
@@ -51,24 +54,26 @@
         template,
         dest_dir,
         collections=collections,
         namespaces=namespaces,
         breadcrumbs=breadcrumbs,
         for_official_docsite=for_official_docsite,
     )
-    index_file = os.path.join(dest_dir, "index.rst")
+    index_file = os.path.join(dest_dir, f"index{output_format.output_extension}")
 
     await write_file(index_file, index_contents)
 
 
 async def write_collection_namespace_index(
     namespace: str,
     collections: Iterable[str],
     template: Template,
     dest_dir: str,
+    output_format: OutputFormat,
+    filename_generator: FilenameGenerator,  # pylint: disable=unused-argument
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
 ) -> None:
     """
     Write an index page listing all of the collections for this namespace.
 
     Each collection will link to an index page listing all content in the collection.
@@ -86,26 +91,27 @@
         template,
         dest_dir,
         namespace=namespace,
         collections=collections,
         breadcrumbs=breadcrumbs,
         for_official_docsite=for_official_docsite,
     )
-    index_file = os.path.join(dest_dir, "index.rst")
+    index_file = os.path.join(dest_dir, f"index{output_format.output_extension}")
 
     await write_file(index_file, index_contents)
 
 
 async def output_collection_index(
     collection_to_plugin_info: CollectionInfoT,
     collection_namespaces: Mapping[str, list[str]],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level collection index page for the collections.
 
@@ -124,14 +130,15 @@
     flog.debug("Enter")
 
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     collection_list_tmpl = env.get_template(
         get_template_filename("list_of_collections", output_format)
     )
 
     collection_toplevel = os.path.join(dest_dir, "collections")
@@ -143,27 +150,30 @@
     os.makedirs(collection_toplevel, mode=0o755, exist_ok=True)
 
     await write_collection_list(
         collection_to_plugin_info.keys(),
         collection_namespaces.keys(),
         collection_list_tmpl,
         collection_toplevel,
+        output_format,
+        filename_generator,
         breadcrumbs=breadcrumbs,
         for_official_docsite=for_official_docsite,
     )
 
     flog.debug("Leave")
 
 
 async def output_collection_namespace_indexes(
     collection_namespaces: Mapping[str, list[str]],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate collection namespace index pages for the collections.
 
@@ -180,14 +190,15 @@
     flog.debug("Enter")
 
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     collection_list_tmpl = env.get_template(
         get_template_filename("list_of_collections_by_namespace", output_format)
     )
 
     writers = []
@@ -202,14 +213,16 @@
             writers.append(
                 await pool.spawn(
                     write_collection_namespace_index(
                         namespace,
                         collection_names,
                         collection_list_tmpl,
                         namespace_dir,
+                        output_format,
+                        filename_generator,
                         breadcrumbs=breadcrumbs,
                         for_official_docsite=for_official_docsite,
                     )
                 )
             )
 
         await asyncio.gather(*writers)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/indexes.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/indexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from antsibull_core import app_context
 from antsibull_core.logging import log
 from antsibull_core.utils.io import write_file
 from jinja2 import Template
 
 from ..docs_parsing import AnsibleCollectionMetadata
 from ..env_variables import EnvironmentVariableInfo
-from ..jinja2.environment import OutputFormat, doc_environment, get_template_filename
+from ..jinja2 import FilenameGenerator, OutputFormat
+from ..jinja2.environment import doc_environment, get_template_filename
 from ..utils.collection_name_transformer import CollectionNameTransformer
 from . import PluginCollectionInfoT, _render_template
 
 mlog = log.fields(mod=__name__)
 
 
 async def write_callback_type_index(
@@ -90,14 +91,15 @@
 
 async def output_callback_indexes(
     plugin_info: PluginCollectionInfoT,
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level callback plugin index pages for all callback plugins of a type in all
     collections.
 
@@ -113,14 +115,15 @@
     flog.debug("Enter")
 
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     plugin_list_tmpl = env.get_template(
         get_template_filename("list_of_callback_plugins", output_format)
     )
 
     collection_toplevel = os.path.join(dest_dir, "collections")
@@ -132,15 +135,16 @@
     os.makedirs(collection_toplevel, mode=0o755, exist_ok=True)
 
     writers = []
     lib_ctx = app_context.lib_ctx.get()
     async with asyncio_pool.AioPool(size=lib_ctx.thread_max) as pool:
         for callback_type, per_collection_data in plugin_info.items():
             filename = os.path.join(
-                collection_toplevel, f"callback_index_{callback_type}.rst"
+                collection_toplevel,
+                f"callback_index_{callback_type}{output_format.output_extension}",
             )
             writers.append(
                 await pool.spawn(
                     write_callback_type_index(
                         callback_type,
                         per_collection_data,
                         plugin_list_tmpl,
@@ -158,14 +162,15 @@
 async def output_plugin_indexes(
     plugin_info: PluginCollectionInfoT,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level plugin index pages for all plugins of a type in all collections.
 
     :arg plugin_info: Mapping of plugin_type to Mapping of collection_name to Mapping of
@@ -181,14 +186,15 @@
     flog.debug("Enter")
 
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     plugin_list_tmpl = env.get_template(
         get_template_filename("list_of_plugins", output_format)
     )
 
     collection_toplevel = os.path.join(dest_dir, "collections")
@@ -199,15 +205,18 @@
     # (docs/docsite/rst) is only writable by us.
     os.makedirs(collection_toplevel, mode=0o755, exist_ok=True)
 
     writers = []
     lib_ctx = app_context.lib_ctx.get()
     async with asyncio_pool.AioPool(size=lib_ctx.thread_max) as pool:
         for plugin_type, per_collection_data in plugin_info.items():
-            filename = os.path.join(collection_toplevel, f"index_{plugin_type}.rst")
+            filename = os.path.join(
+                collection_toplevel,
+                f"index_{plugin_type}{output_format.output_extension}",
+            )
             writers.append(
                 await pool.spawn(
                     write_plugin_type_index(
                         plugin_type,
                         per_collection_data,
                         collection_metadata,
                         plugin_list_tmpl,
@@ -222,14 +231,15 @@
     flog.debug("Leave")
 
 
 async def output_environment_variables(
     dest_dir: str,
     env_variables: Mapping[str, EnvironmentVariableInfo],
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     squash_hierarchy: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Write environment variable Generate collection-level index pages for the collections.
 
     :arg dest_dir: The directory to place the documentation in.
@@ -247,28 +257,31 @@
         collection_toplevel = os.path.join(dest_dir, "collections")
     else:
         collection_toplevel = dest_dir
 
     env = doc_environment(
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     env_var_list_tmpl = env.get_template(
         get_template_filename("list_of_env_variables", output_format)
     )
 
     flog.fields(
         toplevel=collection_toplevel, exists=os.path.isdir(collection_toplevel)
     ).debug("collection_toplevel exists?")
     # This is only safe because we made sure that the top of the directory tree we're writing to
     # (docs/docsite/rst) is only writable by us.
     os.makedirs(collection_toplevel, mode=0o755, exist_ok=True)
 
-    index_file = os.path.join(collection_toplevel, "environment_variables.rst")
+    index_file = os.path.join(
+        collection_toplevel, f"environment_variables{output_format.output_extension}"
+    )
     index_contents = _render_template(
         env_var_list_tmpl,
         index_file,
         env_variables=env_variables,
     )
 
     await write_file(index_file, index_contents)
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/plugin_stubs.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/plugin_stubs.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from antsibull_core import app_context
 from antsibull_core.logging import log
 from antsibull_core.utils.io import write_file
 from jinja2 import Template
 
 from ..collection_links import CollectionLinks
 from ..docs_parsing import AnsibleCollectionMetadata
-from ..jinja2.environment import OutputFormat, doc_environment, get_template_filename
+from ..jinja2 import FilenameGenerator, OutputFormat
+from ..jinja2.environment import doc_environment, get_template_filename
 from ..utils.collection_name_transformer import CollectionNameTransformer
 from . import _render_template
 
 mlog = log.fields(mod=__name__)
 
 
 async def write_stub_rst(
@@ -34,14 +35,16 @@
     collection_links: CollectionLinks,
     plugin_short_name: str,
     plugin_type: str,
     routing_data: Mapping[str, t.Any],
     redirect_tmpl: Template,
     tombstone_tmpl: Template,
     dest_dir: str,
+    output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     path_override: str | None = None,
     squash_hierarchy: bool = False,
     for_official_docsite: bool = False,
 ) -> None:
     """
     Write the rst page for one plugin stub.
 
@@ -108,15 +111,16 @@
                 dest_dir, "collections", namespace, collection
             )
             # This is dangerous but the code that takes dest_dir from the user checks
             # permissions on it to make it as safe as possible.
             os.makedirs(collection_dir, mode=0o755, exist_ok=True)
 
         plugin_file = os.path.join(
-            collection_dir, f"{plugin_short_name}_{plugin_type}.rst"
+            collection_dir,
+            filename_generator.plugin_filename(plugin_name, plugin_type, output_format),
         )
 
     await write_file(plugin_file, plugin_contents)
 
     flog.debug("Leave")
 
 
@@ -124,14 +128,15 @@
     stubs_info: Mapping[str, Mapping[str, Mapping[str, t.Any]]],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     link_data: Mapping[str, CollectionLinks],
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     squash_hierarchy: bool = False,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Output rst files for each plugin stub.
 
@@ -150,14 +155,15 @@
     """
     # Setup the jinja environment
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     redirect_tmpl = env.get_template(
         get_template_filename("plugin-redirect", output_format)
     )
     tombstone_tmpl = env.get_template(
         get_template_filename("plugin-tombstone", output_format)
@@ -177,14 +183,16 @@
                                 link_data[collection_name],
                                 plugin_short_name,
                                 plugin_type,
                                 routing_data,
                                 redirect_tmpl,
                                 tombstone_tmpl,
                                 dest_dir,
+                                output_format,
+                                filename_generator,
                                 squash_hierarchy=squash_hierarchy,
                                 for_official_docsite=for_official_docsite,
                             )
                         )
                     )
 
         # Write docs for each plugin
```

### Comparing `antsibull_docs-2.2.0/src/antsibull_docs/write_docs/plugins.py` & `antsibull_docs-2.3.0/src/antsibull_docs/write_docs/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from antsibull_core import app_context
 from antsibull_core.logging import log
 from antsibull_core.utils.io import write_file
 from jinja2 import Template
 
 from ..collection_links import CollectionLinks
 from ..docs_parsing import AnsibleCollectionMetadata
-from ..jinja2.environment import OutputFormat, doc_environment, get_template_filename
+from ..jinja2 import FilenameGenerator, OutputFormat
+from ..jinja2.environment import doc_environment, get_template_filename
 from ..utils.collection_name_transformer import CollectionNameTransformer
 from . import CollectionInfoT, PluginErrorsT, _render_template
 
 mlog = log.fields(mod=__name__)
 
 
 def follow_relative_links(path: str) -> str:
@@ -255,14 +256,16 @@
     plugin_short_name: str,
     plugin_type: str,
     plugin_record: dict[str, t.Any],
     nonfatal_errors: Sequence[str],
     plugin_tmpl: Template,
     error_tmpl: Template,
     dest_dir: str,
+    output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     path_override: str | None = None,
     squash_hierarchy: bool = False,
     use_html_blobs: bool = False,
     for_official_docsite: bool = False,
 ) -> None:
     """
     Write the rst page for one plugin.
@@ -318,15 +321,18 @@
                 dest_dir, "collections", namespace, collection
             )
             # This is dangerous but the code that takes dest_dir from the user checks
             # permissions on it to make it as safe as possible.
             os.makedirs(collection_dir, mode=0o755, exist_ok=True)
 
         plugin_file = os.path.join(
-            collection_dir, f"{plugin_short_name}_{plugin_type}.rst"
+            collection_dir,
+            filename_generator.plugin_filename(
+                f"{collection_name}.{plugin_short_name}", plugin_type, output_format
+            ),
         )
 
     await write_file(plugin_file, plugin_contents)
 
     flog.debug("Leave")
 
 
@@ -336,14 +342,15 @@
     nonfatal_errors: PluginErrorsT,
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     link_data: Mapping[str, CollectionLinks],
     output_format: OutputFormat,
+    filename_generator: FilenameGenerator,
     squash_hierarchy: bool = False,
     use_html_blobs: bool = False,
     for_official_docsite: bool = False,
     referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Output rst files for each plugin.
@@ -368,14 +375,15 @@
     """
     # Setup the jinja environment
     env = doc_environment(
         collection_url=collection_url,
         collection_install=collection_install,
         referable_envvars=referable_envvars,
         output_format=output_format,
+        filename_generator=filename_generator,
     )
     # Get the templates
     plugin_tmpl = env.get_template(get_template_filename("plugin", output_format))
     role_tmpl = env.get_template(get_template_filename("role", output_format))
     error_tmpl = env.get_template(get_template_filename("plugin-error", output_format))
 
     writers = []
@@ -397,14 +405,16 @@
                                 plugin_short_name,
                                 plugin_type,
                                 plugin_info[plugin_type].get(plugin_name),
                                 nonfatal_errors[plugin_type][plugin_name],
                                 plugin_type_tmpl,
                                 error_tmpl,
                                 dest_dir,
+                                output_format,
+                                filename_generator,
                                 squash_hierarchy=squash_hierarchy,
                                 use_html_blobs=use_html_blobs,
                                 for_official_docsite=for_official_docsite,
                             )
                         )
                     )
```

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/__init__.py` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/antsibull-minimal.css` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/antsibull-minimal.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/assets.py` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/assets.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/roles.py` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/roles.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,33 @@
 """
 
 from __future__ import annotations
 
 import typing as t
 
 from docutils import nodes
+from docutils.utils import unescape  # pyre-ignore[21]
 from sphinx import addnodes
+from sphinx.util import logging
 
-from antsibull_docs.markup.semantic_helper import parse_option, parse_return_value
+from antsibull_docs.markup.semantic_helper import (
+    parse_option,
+    parse_plugin_name,
+    parse_return_value,
+)
 from antsibull_docs.utils.rst import massage_rst_label
 
+from .sphinx_helper import extract_explicit_title
+
+logger = logging.getLogger(__name__)
+
+
+def _plugin_ref(plugin_fqcn: str, plugin_type: str) -> str:
+    return f"ansible_collections.{plugin_fqcn}_{plugin_type}"
+
 
 # pylint:disable-next=unused-argument,dangerous-default-value
 def option_choice(name, rawtext, text, lineno, inliner, options={}, content=[]):
     """Format Ansible option choice entry.
 
     Returns 2 part tuple containing list of nodes to insert into the
     document and a list of system messages.  Both are allowed to be
@@ -100,28 +114,28 @@
     entrypoint: str | None,
     option: str,
 ) -> str | None:
     if not plugin_fqcn or not plugin_type:
         return None
     ref = massage_rst_label(option.replace(".", "/"))
     ep = f"{entrypoint}__" if entrypoint is not None else ""
-    return f"ansible_collections.{plugin_fqcn}_{plugin_type}__parameter-{ep}{ref}"
+    return f"{_plugin_ref(plugin_fqcn, plugin_type)}__parameter-{ep}{ref}"
 
 
 def _create_return_value_reference(
     plugin_fqcn: str | None,
     plugin_type: str | None,
     entrypoint: str | None,
     return_value: str,
 ) -> str | None:
     if not plugin_fqcn or not plugin_type:
         return None
     ref = massage_rst_label(return_value.replace(".", "/"))
     ep = f"{entrypoint}__" if entrypoint is not None else ""
-    return f"ansible_collections.{plugin_fqcn}_{plugin_type}__return-{ep}{ref}"
+    return f"{_plugin_ref(plugin_fqcn, plugin_type)}__return-{ep}{ref}"
 
 
 def _create_ref_or_not(
     create_ref: t.Callable[[str | None, str | None, str | None, str], str | None],
     plugin_fqcn: str | None,
     plugin_type: str | None,
     entrypoint: str | None,
@@ -145,17 +159,19 @@
         "refwarn": True,
     }
     refnode = addnodes.pending_xref(text, content, **options)
     refnode["reftarget"] = ref
     return refnode
 
 
-# pylint:disable-next=unused-argument
 def _create_error(rawtext: str, text: str, error: str) -> tuple[list[t.Any], list[str]]:
     content = nodes.strong(text, error, classes=["error"])
+    logger.error(
+        f"while processing {rawtext}: {error}", location=content, type="semantic-markup"
+    )
     return [content], []
 
 
 # pylint:disable-next=unused-argument,dangerous-default-value
 def option_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
     """Format Ansible option key, or option key-value.
 
@@ -170,15 +186,15 @@
     :param inliner: The inliner instance that called us.
     :param options: Directive options for customization.
     :param content: The directive content for customization.
     """
     classes = []
     try:
         plugin_fqcn, plugin_type, entrypoint, option_link, option, value = parse_option(
-            text.replace("\x00", ""), "", "", require_plugin=False
+            unescape(text), "", "", require_plugin=False
         )
     except ValueError as exc:
         return _create_error(rawtext, text, str(exc))
     if value is None:
         text = f"{option}"
         classes.append("ansible-option")
     else:
@@ -231,15 +247,15 @@
     :param inliner: The inliner instance that called us.
     :param options: Directive options for customization.
     :param content: The directive content for customization.
     """
     classes = ["ansible-return-value"]
     try:
         plugin_fqcn, plugin_type, entrypoint, rv_link, rv, value = parse_return_value(
-            text.replace("\x00", ""), "", "", require_plugin=False
+            unescape(text), "", "", require_plugin=False
         )
     except ValueError as exc:
         return _create_error(rawtext, text, str(exc))
     if value is None:
         text = f"{rv}"
     else:
         text = f"{rv}={value}"
@@ -281,15 +297,15 @@
     text,
     lineno,  # pylint:disable=unused-argument
     inliner,  # pylint:disable=unused-argument
     options={},
     content=[],
 ):
     # Extract the name of the environment variable
-    ref = text.replace("\x00", "").split("=", 1)[0].strip()
+    ref = unescape(text).split("=", 1)[0].strip()
 
     classes = ["xref", "std", "std-envvar"]
     content = nodes.literal(rawtext, text, classes=classes)
 
     options = {
         "reftype": "envvar",
         "refdomain": "std",
@@ -298,24 +314,65 @@
     }
     refnode = addnodes.pending_xref(text, content, **options)
     refnode["reftarget"] = ref
 
     return [refnode], []
 
 
+# pylint:disable-next=unused-argument,dangerous-default-value
+def plugin_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
+    """Format Ansible plugin.
+
+    Returns 2 part tuple containing list of nodes to insert into the
+    document and a list of system messages.  Both are allowed to be
+    empty.
+
+    :param name: The role name used in the document.
+    :param rawtext: The entire markup snippet, with role.
+    :param text: The text marked with the role.
+    :param lineno: The line number where rawtext appears in the input.
+    :param inliner: The inliner instance that called us.
+    :param options: Directive options for customization.
+    :param content: The directive content for customization.
+    """
+    target, title = extract_explicit_title(text)
+
+    try:
+        plugin_fqcn, plugin_type = parse_plugin_name(target)
+    except ValueError as exc:
+        return _create_error(rawtext, text, str(exc))
+
+    if title is None:
+        title = plugin_fqcn
+
+    options = {
+        "reftype": "ref",
+        "refdomain": "std",
+        "refexplicit": True,
+        "refwarn": True,
+    }
+    refnode = addnodes.pending_xref(
+        plugin_fqcn, nodes.inline(rawtext, title), **options
+    )
+    refnode["reftarget"] = _plugin_ref(plugin_fqcn, plugin_type)
+
+    return [refnode], []
+
+
 ROLES = {
     "ansible-option-choices-entry": option_choice,
     "ansible-option-choices-entry-default": option_choice_default,
     "ansible-option-default": option_default,
     "ansible-rv-sample-value": return_value_sample,
     "ansopt": option_role,
     "ansval": value_role,
     "ansretval": return_value_role,
     "ansenvvar": environment_variable,
     "ansenvvarref": environment_variable_reference,
+    "ansplugin": plugin_role,
 }
 
 
 def setup_roles(app):
     """
     Setup roles for a Sphinx app object.
     """
```

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/src/sphinx_antsibull_ext/css/build.sh` & `antsibull_docs-2.3.0/src/sphinx_antsibull_ext/css/build.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/bin/bash
 # Copyright (c) Ansible Project
 # GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-SASSC=${SASS_COMPILER:-$(which sassc)}
+SASS=${SASS_COMPILER:-$(which sass)}
 POSTCSS=${POSTCSS:-$(which postcss)}
 
-if [ "${SASSC}" == "" ]; then
-    echo "Need 'sassc' on path. You can install sassc with 'apt-get install sassc'."
+if [ "${SASS}" == "" ]; then
+    echo "Need 'sass' on path. You can install sass with 'npm install sass'."
     exit -1
 fi
 
 if [ "${POSTCSS}" == "" ]; then
     echo "Need 'postcss' on path. You can install postcss and the required plugins with 'npm install autoprefixer cssnano postcss postcss-cli'."
     exit -1
 fi
@@ -24,13 +24,13 @@
 
 set -e
 
 build_css() {
     SOURCE="$1.scss"
     DEST="../$1.css"
     set -x
-    ${SASSC} "${SOURCE}" "${DEST}"
+    ${SASS} --no-source-map "${SOURCE}" "${DEST}"
     ${POSTCSS} --use autoprefixer --use cssnano --no-map -r "${DEST}"
     { set +x; } 2>/dev/null  # https://stackoverflow.com/a/19226038
 }
 
 build_css antsibull-minimal
```

### Comparing `antsibull_docs-2.2.0/stubs/rstcheck.pyi` & `antsibull_docs-2.3.0/stubs/rstcheck.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/stubs/rstcheck_core/config.pyi` & `antsibull_docs-2.3.0/stubs/rstcheck_core/config.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/validate-html.py` & `antsibull_docs-2.3.0/tests/validate-html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all-others.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all-others.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997872412854%*

 * *Differences: {"'all'": "{'module': {'ns2.col.foo2': {'doc': {'description': {insert: [(2, 'Reference using "*

 * *          'alias - O(ns2.col.foo_redirect#module:bar) and '*

 * *          "O(ns2.col.foo_redirect#module:baz).')]}}}}}"}*

```diff
@@ -23078,15 +23078,16 @@
                     },
                     "author": [
                         "Another one (@ansible-community)"
                     ],
                     "collection": "ns2.col",
                     "description": [
                         "Foo bar.",
-                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value."
+                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value.",
+                        "Reference using alias - O(ns2.col.foo_redirect#module:bar) and O(ns2.col.foo_redirect#module:baz)."
                     ],
                     "filename": "ansible_collections/ns2/col/plugins/modules/foo2.py",
                     "has_action": false,
                     "module": "foo2",
                     "options": {
                         "bar": {
                             "description": [
```

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-all.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997845481371%*

 * *Differences: {"'all'": "{'module': {'ns2.col.foo2': {'doc': {'description': {insert: [(2, 'Reference using "*

 * *          'alias - O(ns2.col.foo_redirect#module:bar) and '*

 * *          "O(ns2.col.foo_redirect#module:baz).')]}}}}}"}*

```diff
@@ -22997,15 +22997,16 @@
                     },
                     "author": [
                         "Another one (@ansible-community)"
                     ],
                     "collection": "ns2.col",
                     "description": [
                         "Foo bar.",
-                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value."
+                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value.",
+                        "Reference using alias - O(ns2.col.foo_redirect#module:bar) and O(ns2.col.foo_redirect#module:baz)."
                     ],
                     "filename": "ansible_collections/ns2/col/plugins/modules/foo2.py",
                     "has_action": false,
                     "module": "foo2",
                     "options": {
                         "bar": {
                             "description": [
```

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col1.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col1.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns.col2.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns.col2.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.col.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.col.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999943264342774%*

 * *Differences: {"'all'": "{'module': {'ns2.col.foo2': {'doc': {'description': {insert: [(2, 'Reference using "*

 * *          'alias - O(ns2.col.foo_redirect#module:bar) and '*

 * *          "O(ns2.col.foo_redirect#module:baz).')]}}}}}"}*

```diff
@@ -1210,15 +1210,16 @@
                     },
                     "author": [
                         "Another one (@ansible-community)"
                     ],
                     "collection": "ns2.col",
                     "description": [
                         "Foo bar.",
-                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value."
+                        "See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.col.foo#role:main:foo_param_2=42) for one with a value.",
+                        "Reference using alias - O(ns2.col.foo_redirect#module:bar) and O(ns2.col.foo_redirect#module:baz)."
                     ],
                     "filename": "ansible_collections/ns2/col/plugins/modules/foo2.py",
                     "has_action": false,
                     "module": "foo2",
                     "options": {
                         "bar": {
                             "description": [
```

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-doc-cache-ns2.flatcol.json` & `antsibull_docs-2.3.0/tests/functional/ansible-doc-cache-ns2.flatcol.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible-version.output` & `antsibull_docs-2.3.0/tests/functional/ansible-version.output`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/ansible_doc_caching.py` & `antsibull_docs-2.3.0/tests/functional/ansible_doc_caching.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/build-docs-baseline.sh` & `antsibull_docs-2.3.0/tests/functional/build-docs-baseline.sh`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     mkdir -p "${DEST}"
     ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/ antsibull-docs collection --dest-dir "${DEST}" --use-current "$@" 2>&1 | (
         set +e
         grep -v "ERROR:antsibull:func=create_plugin_rst:mod=antsibull_docs.write_docs.plugins:nonfatal_errors="
         set -e
     )
 
-    rstcheck --report-level warning --ignore-roles ansible-option-default,ansible-rv-sample-value,ansopt,ansval,ansretval,ansible-option-choices-entry-default,ansible-option-choices-entry,ansenvvar,ansenvvarref -r "${DEST}" 2>&1 | (
+    rstcheck --report-level warning --ignore-roles ansible-option-default,ansible-rv-sample-value,ansopt,ansval,ansretval,ansplugin,ansible-option-choices-entry-default,ansible-option-choices-entry,ansenvvar,ansenvvarref -r "${DEST}" 2>&1 | (
         set +e
         grep -v "CRITICAL:rstcheck_core.checker:An \`AttributeError\` error occured."
         set -e
     )
 }
 
 
@@ -40,14 +40,16 @@
 
 
 make_docsite_baseline baseline-default ns.col1 ns.col2 ns2.col ns2.flatcol
 make_docsite_baseline baseline-no-breadcrumbs ns.col1 ns.col2 ns2.col ns2.flatcol --no-breadcrumbs
 make_docsite_baseline baseline-no-indexes ns.col1 ns2.col ns2.flatcol --fail-on-error --no-indexes
 make_docsite_baseline baseline-use-html-blobs ns2.col --fail-on-error --use-html-blobs
 make_docsite_baseline baseline-squash-hierarchy ns2.col --fail-on-error --squash-hierarchy
+make_docsite_baseline baseline-simplified-rst ns.col1 ns.col2 ns2.col ns2.flatcol --output-format simplified-rst
+make_docsite_baseline baseline-simplified-rst-squash-hierarchy ns2.col --fail-on-error --squash-hierarchy --output-format simplified-rst
 
 echo "Build ansible --version output cache"
 ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/ ansible --version | sed -e "s|${PWD}/collections|<<<<<COLLECTIONS>>>>>|g" | sed -e "s|${HOME}|<<<<<HOME>>>>>|g" | sed -E "s|(ansible python module location = ).*|\\1<<<<<ANSIBLE>>>>>|g" > ansible-version.output
 
 make_ansible_doc_extract all
 make_ansible_doc_extract ns.col1 ns.col1
 make_ansible_doc_extract ns.col2 ns.col2
```

### Comparing `antsibull_docs-2.2.0/tests/functional/build-sphinx-init-baseline.sh` & `antsibull_docs-2.3.0/tests/functional/build-sphinx-init-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/sanitize-ansible-doc-dump.py` & `antsibull_docs-2.3.0/tests/functional/sanitize-ansible-doc-dump.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/sanitize-ansible-galaxy-list.py` & `antsibull_docs-2.3.0/tests/functional/sanitize-ansible-galaxy-list.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/test_docs_baseline.py` & `antsibull_docs-2.3.0/tests/functional/test_docs_baseline.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,39 @@
             "--use-current",
             "ns2.col",
             "--fail-on-error",
             "--squash-hierarchy",
         ],
         "baseline-squash-hierarchy",
     ),
+    (
+        [
+            "collection",
+            "--use-current",
+            "ns.col1",
+            "ns.col2",
+            "ns2.col",
+            "ns2.flatcol",
+            "--output-format",
+            "simplified-rst",
+        ],
+        "baseline-simplified-rst",
+    ),
+    (
+        [
+            "collection",
+            "--use-current",
+            "ns2.col",
+            "--fail-on-error",
+            "--squash-hierarchy",
+            "--output-format",
+            "simplified-rst",
+        ],
+        "baseline-simplified-rst-squash-hierarchy",
+    ),
 ]
 
 
 def _scan_directories(root: str):
     result = {}
     for path, dirs, files in os.walk(root):
         result[os.path.relpath(path, root)] = (path, files)
```

### Comparing `antsibull_docs-2.2.0/tests/functional/test_docs_linting.py` & `antsibull_docs-2.3.0/tests/functional/test_docs_linting.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[5]: RV(ext.col.foo#module:baz): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[6]: RV(ext.col.foo#module:baz[ ]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[10]: P(ns2.col.foo#lookup): a reference to the collection ns2.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[11]: O(ns2.col.bar#filter:foo[-1]): a reference to the collection ns2.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[12]: RV(ns2.col.bar#test:_value): a reference to the collection ns2.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[17]: M(ext.col.foo): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[18]: P(ext.col.bar#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[1]: M(ansible.builtin.service): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[20]: RV(ext.col.foo#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[2]: P(ansible.builtin.pipe#lookup): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[3]: O(ansible.builtin.file#module:state): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[4]: RV(ansible.builtin.stat#module:stat.exists): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[5]: M(ns2.flatcol.foo): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[6]: P(ns2.flatcol.sub.foo2#module): a reference to the collection ns2.flatcol is not allowed",
@@ -518,19 +518,19 @@
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[20]: P(ns.col2.foobarbam#filter): there is no filter plugin ns.col2.foobarbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[21]: O(ns.col2.foo2#module:barbazbam.foo): option name does not reference to an existing option of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[22]: RV(ns.col2.foo2#module:bambazbar): return value name does not reference to an existing return value of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[23]: O(ns.col2.foofoo#test:subfoo.foo): there is no test plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[24]: RV(ns.col2.foofoo#lookup:baz): there is no lookup plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[25]: M(ext.col.notthere): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[26]: P(ext.col.notthere#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\)].notthere): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\\)].notthere): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[29]: RV(ext.col.foo#module:notthere[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[2]: P(ansible.builtin.bazbam#lookup): a reference to the collection ansible.builtin is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[31]: RV(ext.col.notthere#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[3]: O(ansible.builtin.file#module:foobarbaz): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[4]: RV(ansible.builtin.stat#module:baz.bam[]): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[5]: O(ansible.builtin.foobar#module:state): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[6]: RV(ansible.builtin.bazbam#module:stat.exists): a reference to the collection ansible.builtin is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[7]: M(ns2.flatcol.foobarbaz): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[8]: P(ns2.flatcol.sub.bazbam#module): a reference to the collection ns2.flatcol is not allowed",
@@ -598,15 +598,15 @@
             "                             return -> baz",
             "                               value is not a valid dict (type=type_error.dict)",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[4]: O(ext.col.foo#module:foo[baz].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[5]: RV(ext.col.foo#module:baz): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[6]: RV(ext.col.foo#module:baz[ ]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[17]: M(ext.col.foo): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[18]: P(ext.col.bar#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[20]: RV(ext.col.foo#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[5]: M(ns2.flatcol.foo): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[6]: P(ns2.flatcol.sub.foo2#module): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[7]: O(ns2.flatcol.foo#module:subbaz.bam): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[8]: RV(ns2.flatcol.sub.foo2#module:bar): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[1]: O(ansible.builtin.file#module:state[]): option name 'state[]' refers to state - which is neither list nor dictionary - with `[]`",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[2]: RV(ansible.builtin.stat#module:stat[foo.bar].exists): return value name 'stat[foo.bar].exists' refers to stat - which is neither list nor dictionary - with `[]`",
@@ -629,19 +629,19 @@
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[20]: P(ns.col2.foobarbam#filter): there is no filter plugin ns.col2.foobarbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[21]: O(ns.col2.foo2#module:barbazbam.foo): option name does not reference to an existing option of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[22]: RV(ns.col2.foo2#module:bambazbar): return value name does not reference to an existing return value of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[23]: O(ns.col2.foofoo#test:subfoo.foo): there is no test plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[24]: RV(ns.col2.foofoo#lookup:baz): there is no lookup plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[25]: M(ext.col.notthere): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[26]: P(ext.col.notthere#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\)].notthere): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\\)].notthere): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[29]: RV(ext.col.foo#module:notthere[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[2]: P(ansible.builtin.bazbam#lookup): there is no lookup plugin ansible.builtin.bazbam",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[31]: RV(ext.col.notthere#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[3]: O(ansible.builtin.file#module:foobarbaz): option name does not reference to an existing option of the module ansible.builtin.file",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[4]: RV(ansible.builtin.stat#module:baz.bam[]): return value name does not reference to an existing return value of the module ansible.builtin.stat",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[5]: O(ansible.builtin.foobar#module:state): there is no module ansible.builtin.foobar",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[6]: RV(ansible.builtin.bazbam#module:stat.exists): there is no module ansible.builtin.bazbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[7]: M(ns2.flatcol.foobarbaz): a reference to the collection ns2.flatcol is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[8]: P(ns2.flatcol.sub.bazbam#module): a reference to the collection ns2.flatcol is not allowed",
@@ -706,15 +706,15 @@
             "                             return -> baz",
             "                               value is not a valid dict (type=type_error.dict)",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[4]: O(ext.col.foo#module:foo[baz].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[5]: RV(ext.col.foo#module:baz): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> correct_array_stubs -> description[6]: RV(ext.col.foo#module:baz[ ]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[17]: M(ext.col.foo): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[18]: P(ext.col.bar#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[19]: O(ext.col.foo#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> existing -> description[20]: RV(ext.col.foo#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[1]: O(ansible.builtin.file#module:state[]): option name 'state[]' refers to state - which is neither list nor dictionary - with `[]`",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[2]: RV(ansible.builtin.stat#module:stat[foo.bar].exists): return value name 'stat[foo.bar].exists' refers to stat - which is neither list nor dictionary - with `[]`",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[3]: RV(ansible.builtin.stat#module:stat.exists[]): return value name 'stat.exists[]' refers to stat.exists - which is neither list nor dictionary - with `[]`",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[4]: O(ns.col2.foo2#module:subfoo[): option name 'subfoo[' cannot be parsed: Found \"[\" without closing \"]\" at position 7 of 'subfoo['",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[4]: O(ns.col2.foo2#module:subfoo[): option name does not reference to an existing option of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> incorrect_array_stubs -> description[5]: RV(ns.col2.foo2#module:bar[]): return value name 'bar[]' refers to bar - which is neither list nor dictionary - with `[]`",
@@ -733,19 +733,19 @@
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[20]: P(ns.col2.foobarbam#filter): there is no filter plugin ns.col2.foobarbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[21]: O(ns.col2.foo2#module:barbazbam.foo): option name does not reference to an existing option of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[22]: RV(ns.col2.foo2#module:bambazbar): return value name does not reference to an existing return value of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[23]: O(ns.col2.foofoo#test:subfoo.foo): there is no test plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[24]: RV(ns.col2.foofoo#lookup:baz): there is no lookup plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[25]: M(ext.col.notthere): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[26]: P(ext.col.notthere#lookup): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\)].notthere): a reference to the collection ext.col is not allowed",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\\)].notthere): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[29]: RV(ext.col.foo#module:notthere[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[2]: P(ansible.builtin.bazbam#lookup): there is no lookup plugin ansible.builtin.bazbam",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\)].bar): a reference to the collection ext.col is not allowed",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\\)].bar): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[31]: RV(ext.col.notthere#module:baz[]): a reference to the collection ext.col is not allowed",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[3]: O(ansible.builtin.file#module:foobarbaz): option name does not reference to an existing option of the module ansible.builtin.file",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[4]: RV(ansible.builtin.stat#module:baz.bam[]): return value name does not reference to an existing return value of the module ansible.builtin.stat",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[5]: O(ansible.builtin.foobar#module:state): there is no module ansible.builtin.foobar",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[6]: RV(ansible.builtin.bazbam#module:stat.exists): there is no module ansible.builtin.bazbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[7]: M(ns2.flatcol.foobarbaz): there is no module ns2.flatcol.foobarbaz",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[8]: P(ns2.flatcol.sub.bazbam#module): there is no module ns2.flatcol.sub.bazbam",
@@ -832,19 +832,19 @@
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[20]: P(ns.col2.foobarbam#filter): there is no filter plugin ns.col2.foobarbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[21]: O(ns.col2.foo2#module:barbazbam.foo): option name does not reference to an existing option of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[22]: RV(ns.col2.foo2#module:bambazbar): return value name does not reference to an existing return value of the module ns.col2.foo2",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[23]: O(ns.col2.foofoo#test:subfoo.foo): there is no test plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[24]: RV(ns.col2.foofoo#lookup:baz): there is no lookup plugin ns.col2.foofoo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[25]: M(ext.col.notthere): there is no module ext.col.notthere",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[26]: P(ext.col.notthere#lookup): there is no lookup plugin ext.col.notthere",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\)].notthere): option name does not reference to an existing option of the module ext.col.foo",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\)].bar): option name does not reference to an existing option of the module ext.col.foo",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[27]: O(ext.col.foo#module:foo[len(foo\\)].notthere): option name does not reference to an existing option of the module ext.col.foo",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[28]: O(ext.col.foo#module:notthere[len(notthere\\)].bar): option name does not reference to an existing option of the module ext.col.foo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[29]: RV(ext.col.foo#module:notthere[]): return value name does not reference to an existing return value of the module ext.col.foo",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[2]: P(ansible.builtin.bazbam#lookup): there is no lookup plugin ansible.builtin.bazbam",
-            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\)].bar): there is no module ext.col.notthere",
+            "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[30]: O(ext.col.notthere#module:foo[len(foo\\)].bar): there is no module ext.col.notthere",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[31]: RV(ext.col.notthere#module:baz[]): there is no module ext.col.notthere",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[3]: O(ansible.builtin.file#module:foobarbaz): option name does not reference to an existing option of the module ansible.builtin.file",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[4]: RV(ansible.builtin.stat#module:baz.bam[]): return value name does not reference to an existing return value of the module ansible.builtin.stat",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[5]: O(ansible.builtin.foobar#module:state): there is no module ansible.builtin.foobar",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[6]: RV(ansible.builtin.bazbam#module:stat.exists): there is no module ansible.builtin.bazbam",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[7]: M(ns2.flatcol.foobarbaz): there is no module ns2.flatcol.foobarbaz",
             "plugins/modules/foo4.py:0:0: DOCUMENTATION -> options -> not_existing -> description[8]: P(ns2.flatcol.sub.bazbam#module): there is no module ns2.flatcol.sub.bazbam",
```

### Comparing `antsibull_docs-2.2.0/tests/functional/test_sphinx_init_baseline.py` & `antsibull_docs-2.3.0/tests/functional/test_sphinx_init_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/environment_variables.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/environment_variables.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 Environment variables used by the ansible-core configuration are documented in :ref:`ansible_configuration_settings`.
 
 .. envvar:: ANSIBLE_FOO_EXE
 
     Foo executable.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_FOO_FILENAME_EXT
 
     All extensions to check.
 
     *Used by:*
-    :ref:`ns2.col.foo vars plugin <ansible_collections.ns2.col.foo_vars>`
+    :ansplugin:`ns2.col.foo vars plugin <ns2.col.foo#vars>`
 .. envvar:: ANSIBLE_FOO_USER
 
     User you 'become' to execute the task.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_REMOTE_TEMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
 .. envvar:: ANSIBLE_REMOTE_TMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.bar_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns.col2.bar role -- Bar role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo2 module -- Foo two
 ++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo3 module -- Foo III
 ++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo4_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo4 module -- Markup reference linting test
 ++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns/col2/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns/col2/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 These are the plugins in the ns.col2 collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns.col2.foo_module>` -- 
-* :ref:`foo2 module <ansible_collections.ns.col2.foo2_module>` -- Foo two
-* :ref:`foo3 module <ansible_collections.ns.col2.foo3_module>` -- Foo III
-* :ref:`foo4 module <ansible_collections.ns.col2.foo4_module>` -- Markup reference linting test
+* :ansplugin:`foo module <ns.col2.foo#module>` -- 
+* :ansplugin:`foo2 module <ns.col2.foo2#module>` -- Foo two
+* :ansplugin:`foo3 module <ns.col2.foo3#module>` -- Foo III
+* :ansplugin:`foo4 module <ns.col2.foo4#module>` -- Markup reference linting test
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
@@ -56,15 +56,15 @@
 
 
 Role Index
 ----------
 
 These are the roles in the ns.col2 collection:
 
-* :ref:`bar role <ansible_collections.ns.col2.bar_role>` -- Bar role
+* :ansplugin:`bar role <ns.col2.bar#role>` -- Bar role
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_role
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.bar filter -- The bar filter
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-.. _ansible_collections.ns2.col.is_bar_test:
-
 .. Title
 
 ns2.col.bar test -- Is something a bar
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -66,15 +61,15 @@
 .. Description
 
 - Check whether a path is a bar.
 
 
 .. Aliases
 
-Aliases: 
+Aliases: is_bar
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -62,14 +58,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Foo bar.
 - See \ :ansopt:`ns2.col.foo#role:main:foo\_param\_1`\  for a random role parameter reference. And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\  for one with a value.
+- Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\  and \ :ansopt:`ns2.col.foo\_redirect#module:baz`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_become:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo become -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cache:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cache -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cache: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cache -- Foo files \ :
-ansopt:`ns2.col.foo#cache:bar`\
+ansible.builtin .. Title ns2.col.foo cache -- Foo files \ :ansopt:
+`ns2.col.foo#cache:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This cache plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.9.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Cache foo files. .. Aliases .. Requirements .. Options
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_callback:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo callback -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_callback: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo callback -- Foo output
-\ :ansopt:`ns2.col.foo#callback:bar`\
+ansible.builtin .. Title ns2.col.foo callback -- Foo output \ :ansopt:
+`ns2.col.foo#callback:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This callback plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.0.1 .. contents:: :local: :depth: 1 .. Deprecated Callback plugin
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cliconf:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cliconf -- Foo router CLI config
 ++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cliconf: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cliconf -- Foo router
-CLI config ++++++++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This cliconf plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo cliconf -- Foo router CLI config
+++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+cliconf plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - This is a CLI config for foo
 routers. Whatever these are. .. Aliases .. Requirements .. Options ..
 Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values .. Status
 (Presently only deprecated) .. Authors Authors ~~~~~~~ - Felix Fontein
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_connection:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo connection -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo filter -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_inventory:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo inventory -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_inventory: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo inventory -- The foo
-inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+ansible.builtin .. Title ns2.col.foo inventory -- The foo inventory \ :ansopt:
+`ns2.col.foo#inventory:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This inventory plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.5.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_lookup:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo lookup -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo module -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -72,14 +68,15 @@
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
 - \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
+Aliases: foo_redirect
 
 .. Requirements
 
 .. _ansible_collections.ns2.col.foo_module_requirements:
 
 Requirements
 ------------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns2.col.foo role -- Foo role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_shell:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo shell -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_strategy:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo strategy -- Executes tasks in foo
 +++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_strategy: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo strategy -- Executes
-tasks in foo +++++++++++++++++++++++++++++++++++++++++++++ .. Collection note
-.. note:: This strategy plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo strategy -- Executes tasks in foo
++++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+strategy plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.1.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is something funny. Or at least I think so from its
 name. .. Aliases .. Requirements .. Options .. Attributes .. Notes .. Seealso
 .. Examples .. Facts .. Return values .. Status (Presently only deprecated) ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo test -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_vars:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo vars -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -70,181 +70,181 @@
 
 These are the plugins in the ns2.col collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.col.foo2_module>` -- Another foo
-* :ref:`sub.foo3 module <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
+* :ansplugin:`foo module <ns2.col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.col.foo2#module>` -- Another foo
+* :ansplugin:`sub.foo3 module <ns2.col.sub.foo3#module>` -- A sub-foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
     sub.foo3_module
 
 
 Become Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo become <ansible_collections.ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
+* :ansplugin:`foo become <ns2.col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_become
 
 
 Cache Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo cache <ansible_collections.ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
+* :ansplugin:`foo cache <ns2.col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cache
 
 
 Callback Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo callback <ansible_collections.ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
+* :ansplugin:`foo callback <ns2.col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_callback
 
 
 Cliconf Plugins
 ~~~~~~~~~~~~~~~
 
-* :ref:`foo cliconf <ansible_collections.ns2.col.foo_cliconf>` -- Foo router CLI config
+* :ansplugin:`foo cliconf <ns2.col.foo#cliconf>` -- Foo router CLI config
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cliconf
 
 
 Connection Plugins
 ~~~~~~~~~~~~~~~~~~
 
-* :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
+* :ansplugin:`foo connection <ns2.col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
-* :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
+* :ansplugin:`bar filter <ns2.col.bar#filter>` -- The bar filter
+* :ansplugin:`foo filter <ns2.col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
-* :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
+* :ansplugin:`foo inventory <ns2.col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_inventory
 
 
 Lookup Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo lookup <ansible_collections.ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
+* :ansplugin:`foo lookup <ns2.col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_lookup
 
 
 Shell Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo shell <ansible_collections.ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
+* :ansplugin:`foo shell <ns2.col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_shell
 
 
 Strategy Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
+* :ansplugin:`foo strategy <ns2.col.foo#strategy>` -- Executes tasks in foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
-* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
-* :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
+* :ansplugin:`bar test <ns2.col.bar#test>` -- Is something a bar
+* :ansplugin:`foo test <ns2.col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
-* :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
+* :ansplugin:`foo vars <ns2.col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_vars
 
 
 Role Index
 ----------
 
 These are the roles in the ns2.col collection:
 
-* :ref:`foo role <ansible_collections.ns2.col.foo_role>` -- Foo role
+* :ansplugin:`foo role <ns2.col.foo#role>` -- Foo role
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_role
```

#### html2text {}

```diff
@@ -9,53 +9,52 @@
 matrix.to/#/#users:ansible.im>`__. - IRC channel :literal:`#ansible` (Libera
 network): `General usage and support questions
 web.libera.chat/?channel=#ansible>`__. - Mailing list: `Ansible Project List
 groups.google.com/g/ansible-project>`__. (`Subscribe
 subscribe@googlegroups.com?subject=subscribe>`__) .. toctree:: :maxdepth: 1
 Guides ------ .. toctree:: :maxdepth: 1 docsite/filter_guide Plugin Index -----
 ------- These are the plugins in the ns2.col collection: Modules ~~~~~~~ * :
-ref:`foo module
-ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :ref:
-`foo2 module
-ns2.col.foo2_module>` -- Another foo * :ref:`sub.foo3 module
-ns2.col.sub.foo3_module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
-foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :ref:
-`foo become
-ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ref:
-`foo cache
-ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo callback
-ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
+ansplugin:`foo module
+col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :
+ansplugin:`foo2 module
+col.foo2#module>` -- Another foo * :ansplugin:`sub.foo3 module
+col.sub.foo3#module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
+foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :
+ansplugin:`foo become
+col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ansplugin:`foo
+cache
+col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo callback
+col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
-:ref:`foo cliconf
-ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
-hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
-connection
-ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`bar filter
-ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
-ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
+:ansplugin:`foo cliconf
+col.foo#cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :hidden:
+foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ansplugin:`foo connection
+col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`bar filter
+col.bar#filter>` -- The bar filter * :ansplugin:`foo filter
+col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
-~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
-ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
-~~~~~~~~~~~~~~ * :ref:`foo lookup
-ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
-`foo shell
-ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo strategy
-ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
-ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
-ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
+~~~~~~~~~~~~~~~~~ * :ansplugin:`foo inventory
+col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`foo lookup
+col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
+toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :
+ansplugin:`foo shell
+col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo strategy
+col.foo#strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :hidden:
+foo_strategy Test Plugins ~~~~~~~~~~~~ * :ansplugin:`bar test
+col.bar#test>` -- Is something a bar * :ansplugin:`foo test
+col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
-ref:`foo vars
-ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
+ansplugin:`foo vars
+col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
-ns2.col collection: * :ref:`foo role
-ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
+ns2.col collection: * :ansplugin:`foo role
+col.foo#role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
 seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.sub.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.sub.foo3 module -- A sub-foo
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo module -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 These are the plugins in the ns2.flatcol collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.flatcol.foo_module>` -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.flatcol.foo2_module>` -- Another foo
+* :ansplugin:`foo module <ns2.flatcol.foo#module>` -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.flatcol.foo2#module>` -- Another foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 Environment variables used by the ansible-core configuration are documented in :ref:`ansible_configuration_settings`.
 
 .. envvar:: ANSIBLE_FOO_EXE
 
     Foo executable.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_FOO_FILENAME_EXT
 
     All extensions to check.
 
     *Used by:*
-    :ref:`ns2.col.foo vars plugin <ansible_collections.ns2.col.foo_vars>`
+    :ansplugin:`ns2.col.foo vars plugin <ns2.col.foo#vars>`
 .. envvar:: ANSIBLE_FOO_USER
 
     User you 'become' to execute the task.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_REMOTE_TEMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
 .. envvar:: ANSIBLE_REMOTE_TMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.bar_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns.col2.bar role -- Bar role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo2 module -- Foo two
 ++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo3 module -- Foo III
 ++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns.col2.foo4_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns.col2.foo4 module -- Markup reference linting test
 ++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -37,24 +37,24 @@
 
 These are the plugins in the ns.col2 collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns.col2.foo_module>` -- 
-* :ref:`foo2 module <ansible_collections.ns.col2.foo2_module>` -- Foo two
-* :ref:`foo3 module <ansible_collections.ns.col2.foo3_module>` -- Foo III
-* :ref:`foo4 module <ansible_collections.ns.col2.foo4_module>` -- Markup reference linting test
+* :ansplugin:`foo module <ns.col2.foo#module>` -- 
+* :ansplugin:`foo2 module <ns.col2.foo2#module>` -- Foo two
+* :ansplugin:`foo3 module <ns.col2.foo3#module>` -- Foo III
+* :ansplugin:`foo4 module <ns.col2.foo4#module>` -- Markup reference linting test
 
 
 Role Index
 ----------
 
 These are the roles in the ns.col2 collection:
 
-* :ref:`bar role <ansible_collections.ns.col2.bar_role>` -- Bar role
+* :ansplugin:`bar role <ns.col2.bar#role>` -- Bar role
 
 
 .. seealso::
 
     List of :ref:`collections <list_of_collections>` with docs hosted here.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.bar filter -- The bar filter
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-.. _ansible_collections.ns2.col.is_bar_test:
-
 .. Title
 
 ns2.col.bar test -- Is something a bar
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -66,15 +61,15 @@
 .. Description
 
 - Check whether a path is a bar.
 
 
 .. Aliases
 
-Aliases: 
+Aliases: is_bar
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -62,14 +58,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Foo bar.
 - See \ :ansopt:`ns2.col.foo#role:main:foo\_param\_1`\  for a random role parameter reference. And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\  for one with a value.
+- Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\  and \ :ansopt:`ns2.col.foo\_redirect#module:baz`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_become:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo become -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cache:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cache -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cache: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cache -- Foo files \ :
-ansopt:`ns2.col.foo#cache:bar`\
+ansible.builtin .. Title ns2.col.foo cache -- Foo files \ :ansopt:
+`ns2.col.foo#cache:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This cache plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.9.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Cache foo files. .. Aliases .. Requirements .. Options
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_callback:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo callback -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_callback: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo callback -- Foo output
-\ :ansopt:`ns2.col.foo#callback:bar`\
+ansible.builtin .. Title ns2.col.foo callback -- Foo output \ :ansopt:
+`ns2.col.foo#callback:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This callback plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.0.1 .. contents:: :local: :depth: 1 .. Deprecated Callback plugin
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cliconf:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cliconf -- Foo router CLI config
 ++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cliconf: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cliconf -- Foo router
-CLI config ++++++++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This cliconf plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo cliconf -- Foo router CLI config
+++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+cliconf plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - This is a CLI config for foo
 routers. Whatever these are. .. Aliases .. Requirements .. Options ..
 Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values .. Status
 (Presently only deprecated) .. Authors Authors ~~~~~~~ - Felix Fontein
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_connection:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo connection -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo filter -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_inventory:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo inventory -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_inventory: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo inventory -- The foo
-inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+ansible.builtin .. Title ns2.col.foo inventory -- The foo inventory \ :ansopt:
+`ns2.col.foo#inventory:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This inventory plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.5.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_lookup:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo lookup -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo module -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -72,14 +68,15 @@
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
 - \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
+Aliases: foo_redirect
 
 .. Requirements
 
 .. _ansible_collections.ns2.col.foo_module_requirements:
 
 Requirements
 ------------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns2.col.foo role -- Foo role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_shell:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo shell -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_strategy:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo strategy -- Executes tasks in foo
 +++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_strategy: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo strategy -- Executes
-tasks in foo +++++++++++++++++++++++++++++++++++++++++++++ .. Collection note
-.. note:: This strategy plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo strategy -- Executes tasks in foo
++++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+strategy plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.1.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is something funny. Or at least I think so from its
 name. .. Aliases .. Requirements .. Options .. Attributes .. Notes .. Seealso
 .. Examples .. Facts .. Return values .. Status (Presently only deprecated) ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo test -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_vars:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo vars -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -71,97 +71,97 @@
 
 These are the plugins in the ns2.col collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.col.foo2_module>` -- Another foo
-* :ref:`sub.foo3 module <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
+* :ansplugin:`foo module <ns2.col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.col.foo2#module>` -- Another foo
+* :ansplugin:`sub.foo3 module <ns2.col.sub.foo3#module>` -- A sub-foo
 
 
 Become Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo become <ansible_collections.ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
+* :ansplugin:`foo become <ns2.col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 
 
 Cache Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo cache <ansible_collections.ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
+* :ansplugin:`foo cache <ns2.col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 
 
 Callback Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo callback <ansible_collections.ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
+* :ansplugin:`foo callback <ns2.col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 
 
 Cliconf Plugins
 ~~~~~~~~~~~~~~~
 
-* :ref:`foo cliconf <ansible_collections.ns2.col.foo_cliconf>` -- Foo router CLI config
+* :ansplugin:`foo cliconf <ns2.col.foo#cliconf>` -- Foo router CLI config
 
 
 Connection Plugins
 ~~~~~~~~~~~~~~~~~~
 
-* :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
+* :ansplugin:`foo connection <ns2.col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
-* :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
+* :ansplugin:`bar filter <ns2.col.bar#filter>` -- The bar filter
+* :ansplugin:`foo filter <ns2.col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
-* :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
+* :ansplugin:`foo inventory <ns2.col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 
 
 Lookup Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo lookup <ansible_collections.ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
+* :ansplugin:`foo lookup <ns2.col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 
 
 Shell Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo shell <ansible_collections.ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
+* :ansplugin:`foo shell <ns2.col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 
 
 Strategy Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
+* :ansplugin:`foo strategy <ns2.col.foo#strategy>` -- Executes tasks in foo
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
-* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
-* :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
+* :ansplugin:`bar test <ns2.col.bar#test>` -- Is something a bar
+* :ansplugin:`foo test <ns2.col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
-* :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
+* :ansplugin:`foo vars <ns2.col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 
 
 Role Index
 ----------
 
 These are the roles in the ns2.col collection:
 
-* :ref:`foo role <ansible_collections.ns2.col.foo_role>` -- Foo role
+* :ansplugin:`foo role <ns2.col.foo#role>` -- Foo role
 
 
 .. seealso::
 
     List of :ref:`collections <list_of_collections>` with docs hosted here.
```

#### html2text {}

```diff
@@ -9,41 +9,41 @@
 matrix.to/#/#users:ansible.im>`__. - IRC channel :literal:`#ansible` (Libera
 network): `General usage and support questions
 web.libera.chat/?channel=#ansible>`__. - Mailing list: `Ansible Project List
 groups.google.com/g/ansible-project>`__. (`Subscribe
 subscribe@googlegroups.com?subject=subscribe>`__) .. toctree:: :maxdepth: 1
 Guides ------ .. toctree:: :maxdepth: 1 docsite/filter_guide Plugin Index -----
 ------- These are the plugins in the ns2.col collection: Modules ~~~~~~~ * :
-ref:`foo module
-ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :ref:
-`foo2 module
-ns2.col.foo2_module>` -- Another foo * :ref:`sub.foo3 module
-ns2.col.sub.foo3_module>` -- A sub-foo Become Plugins ~~~~~~~~~~~~~~ * :ref:
+ansplugin:`foo module
+col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :
+ansplugin:`foo2 module
+col.foo2#module>` -- Another foo * :ansplugin:`sub.foo3 module
+col.sub.foo3#module>` -- A sub-foo Become Plugins ~~~~~~~~~~~~~~ * :ansplugin:
 `foo become
-ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ Cache
-Plugins ~~~~~~~~~~~~~ * :ref:`foo cache
-ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ Callback
-Plugins ~~~~~~~~~~~~~~~~ * :ref:`foo callback
-ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\
-Cliconf Plugins ~~~~~~~~~~~~~~~ * :ref:`foo cliconf
-ns2.col.foo_cliconf>` -- Foo router CLI config Connection Plugins
-~~~~~~~~~~~~~~~~~~ * :ref:`foo connection
-ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ Filter Plugins ~~~~~~~~~~~~~~ * :ref:`bar filter
-ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
-ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\
-Inventory Plugins ~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
-ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
-bar`\ Lookup Plugins ~~~~~~~~~~~~~~ * :ref:`foo lookup
-ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\
-Shell Plugins ~~~~~~~~~~~~~ * :ref:`foo shell
-ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ Strategy
-Plugins ~~~~~~~~~~~~~~~~ * :ref:`foo strategy
-ns2.col.foo_strategy>` -- Executes tasks in foo Test Plugins ~~~~~~~~~~~~ * :
-ref:`bar test
-ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
-ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ Vars
-Plugins ~~~~~~~~~~~~ * :ref:`foo vars
-ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ Role Index ---
-------- These are the roles in the ns2.col collection: * :ref:`foo role
-ns2.col.foo_role>` -- Foo role .. seealso:: List of :ref:`collections ` with
-docs hosted here.
+col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ Cache Plugins
+~~~~~~~~~~~~~ * :ansplugin:`foo cache
+col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ Callback
+Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:`foo callback
+col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ Cliconf
+Plugins ~~~~~~~~~~~~~~~ * :ansplugin:`foo cliconf
+col.foo#cliconf>` -- Foo router CLI config Connection Plugins
+~~~~~~~~~~~~~~~~~~ * :ansplugin:`foo connection
+col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\
+Filter Plugins ~~~~~~~~~~~~~~ * :ansplugin:`bar filter
+col.bar#filter>` -- The bar filter * :ansplugin:`foo filter
+col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\
+Inventory Plugins ~~~~~~~~~~~~~~~~~ * :ansplugin:`foo inventory
+col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+Lookup Plugins ~~~~~~~~~~~~~~ * :ansplugin:`foo lookup
+col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ Shell
+Plugins ~~~~~~~~~~~~~ * :ansplugin:`foo shell
+col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ Strategy
+Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:`foo strategy
+col.foo#strategy>` -- Executes tasks in foo Test Plugins ~~~~~~~~~~~~ * :
+ansplugin:`bar test
+col.bar#test>` -- Is something a bar * :ansplugin:`foo test
+col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ Vars
+Plugins ~~~~~~~~~~~~ * :ansplugin:`foo vars
+col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ Role Index -------
+--- These are the roles in the ns2.col collection: * :ansplugin:`foo role
+col.foo#role>` -- Foo role .. seealso:: List of :ref:`collections ` with docs
+hosted here.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.sub.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.sub.foo3 module -- A sub-foo
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo module -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 Environment variables used by the ansible-core configuration are documented in :ref:`ansible_configuration_settings`.
 
 .. envvar:: ANSIBLE_FOO_EXE
 
     Foo executable.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_FOO_FILENAME_EXT
 
     All extensions to check.
 
     *Used by:*
-    :ref:`ns2.col.foo vars plugin <ansible_collections.ns2.col.foo_vars>`
+    :ansplugin:`ns2.col.foo vars plugin <ns2.col.foo#vars>`
 .. envvar:: ANSIBLE_FOO_USER
 
     User you 'become' to execute the task.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_REMOTE_TEMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
 .. envvar:: ANSIBLE_REMOTE_TMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.bar filter -- The bar filter
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-.. _ansible_collections.ns2.col.is_bar_test:
-
 .. Title
 
 ns2.col.bar test -- Is something a bar
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -66,15 +61,15 @@
 .. Description
 
 - Check whether a path is a bar.
 
 
 .. Aliases
 
-Aliases: 
+Aliases: is_bar
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -62,14 +58,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Foo bar.
 - See \ :ansopt:`ns2.col.foo#role:main:foo\_param\_1`\  for a random role parameter reference. And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\  for one with a value.
+- Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\  and \ :ansopt:`ns2.col.foo\_redirect#module:baz`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_become:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo become -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cache:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cache -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cache: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cache -- Foo files \ :
-ansopt:`ns2.col.foo#cache:bar`\
+ansible.builtin .. Title ns2.col.foo cache -- Foo files \ :ansopt:
+`ns2.col.foo#cache:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This cache plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.9.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Cache foo files. .. Aliases .. Requirements .. Options
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_callback:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo callback -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_callback: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo callback -- Foo output
-\ :ansopt:`ns2.col.foo#callback:bar`\
+ansible.builtin .. Title ns2.col.foo callback -- Foo output \ :ansopt:
+`ns2.col.foo#callback:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This callback plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.0.1 .. contents:: :local: :depth: 1 .. Deprecated Callback plugin
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cliconf:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cliconf -- Foo router CLI config
 ++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cliconf: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cliconf -- Foo router
-CLI config ++++++++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This cliconf plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo cliconf -- Foo router CLI config
+++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+cliconf plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - This is a CLI config for foo
 routers. Whatever these are. .. Aliases .. Requirements .. Options ..
 Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values .. Status
 (Presently only deprecated) .. Authors Authors ~~~~~~~ - Felix Fontein
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_connection:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo connection -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo filter -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_inventory:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo inventory -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_inventory: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo inventory -- The foo
-inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+ansible.builtin .. Title ns2.col.foo inventory -- The foo inventory \ :ansopt:
+`ns2.col.foo#inventory:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This inventory plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.5.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_lookup:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo lookup -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo module -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -72,14 +68,15 @@
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
 - \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
+Aliases: foo_redirect
 
 .. Requirements
 
 .. _ansible_collections.ns2.col.foo_module_requirements:
 
 Requirements
 ------------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns2.col.foo role -- Foo role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_shell:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo shell -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_strategy:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo strategy -- Executes tasks in foo
 +++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_strategy: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo strategy -- Executes
-tasks in foo +++++++++++++++++++++++++++++++++++++++++++++ .. Collection note
-.. note:: This strategy plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo strategy -- Executes tasks in foo
++++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+strategy plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.1.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is something funny. Or at least I think so from its
 name. .. Aliases .. Requirements .. Options .. Attributes .. Notes .. Seealso
 .. Examples .. Facts .. Return values .. Status (Presently only deprecated) ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo test -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_vars:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo vars -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -70,181 +70,181 @@
 
 These are the plugins in the ns2.col collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.col.foo2_module>` -- Another foo
-* :ref:`sub.foo3 module <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
+* :ansplugin:`foo module <ns2.col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.col.foo2#module>` -- Another foo
+* :ansplugin:`sub.foo3 module <ns2.col.sub.foo3#module>` -- A sub-foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
     sub.foo3_module
 
 
 Become Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo become <ansible_collections.ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
+* :ansplugin:`foo become <ns2.col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_become
 
 
 Cache Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo cache <ansible_collections.ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
+* :ansplugin:`foo cache <ns2.col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cache
 
 
 Callback Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo callback <ansible_collections.ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
+* :ansplugin:`foo callback <ns2.col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_callback
 
 
 Cliconf Plugins
 ~~~~~~~~~~~~~~~
 
-* :ref:`foo cliconf <ansible_collections.ns2.col.foo_cliconf>` -- Foo router CLI config
+* :ansplugin:`foo cliconf <ns2.col.foo#cliconf>` -- Foo router CLI config
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cliconf
 
 
 Connection Plugins
 ~~~~~~~~~~~~~~~~~~
 
-* :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
+* :ansplugin:`foo connection <ns2.col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
-* :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
+* :ansplugin:`bar filter <ns2.col.bar#filter>` -- The bar filter
+* :ansplugin:`foo filter <ns2.col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
-* :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
+* :ansplugin:`foo inventory <ns2.col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_inventory
 
 
 Lookup Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo lookup <ansible_collections.ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
+* :ansplugin:`foo lookup <ns2.col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_lookup
 
 
 Shell Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo shell <ansible_collections.ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
+* :ansplugin:`foo shell <ns2.col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_shell
 
 
 Strategy Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
+* :ansplugin:`foo strategy <ns2.col.foo#strategy>` -- Executes tasks in foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
-* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
-* :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
+* :ansplugin:`bar test <ns2.col.bar#test>` -- Is something a bar
+* :ansplugin:`foo test <ns2.col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
-* :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
+* :ansplugin:`foo vars <ns2.col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_vars
 
 
 Role Index
 ----------
 
 These are the roles in the ns2.col collection:
 
-* :ref:`foo role <ansible_collections.ns2.col.foo_role>` -- Foo role
+* :ansplugin:`foo role <ns2.col.foo#role>` -- Foo role
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_role
```

#### html2text {}

```diff
@@ -9,53 +9,52 @@
 matrix.to/#/#users:ansible.im>`__. - IRC channel :literal:`#ansible` (Libera
 network): `General usage and support questions
 web.libera.chat/?channel=#ansible>`__. - Mailing list: `Ansible Project List
 groups.google.com/g/ansible-project>`__. (`Subscribe
 subscribe@googlegroups.com?subject=subscribe>`__) .. toctree:: :maxdepth: 1
 Guides ------ .. toctree:: :maxdepth: 1 docsite/filter_guide Plugin Index -----
 ------- These are the plugins in the ns2.col collection: Modules ~~~~~~~ * :
-ref:`foo module
-ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :ref:
-`foo2 module
-ns2.col.foo2_module>` -- Another foo * :ref:`sub.foo3 module
-ns2.col.sub.foo3_module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
-foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :ref:
-`foo become
-ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ref:
-`foo cache
-ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo callback
-ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
+ansplugin:`foo module
+col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :
+ansplugin:`foo2 module
+col.foo2#module>` -- Another foo * :ansplugin:`sub.foo3 module
+col.sub.foo3#module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
+foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :
+ansplugin:`foo become
+col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ansplugin:`foo
+cache
+col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo callback
+col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
-:ref:`foo cliconf
-ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
-hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
-connection
-ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`bar filter
-ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
-ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
+:ansplugin:`foo cliconf
+col.foo#cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :hidden:
+foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ansplugin:`foo connection
+col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`bar filter
+col.bar#filter>` -- The bar filter * :ansplugin:`foo filter
+col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
-~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
-ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
-~~~~~~~~~~~~~~ * :ref:`foo lookup
-ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
-`foo shell
-ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo strategy
-ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
-ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
-ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
+~~~~~~~~~~~~~~~~~ * :ansplugin:`foo inventory
+col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`foo lookup
+col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
+toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :
+ansplugin:`foo shell
+col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo strategy
+col.foo#strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :hidden:
+foo_strategy Test Plugins ~~~~~~~~~~~~ * :ansplugin:`bar test
+col.bar#test>` -- Is something a bar * :ansplugin:`foo test
+col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
-ref:`foo vars
-ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
+ansplugin:`foo vars
+col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
-ns2.col collection: * :ref:`foo role
-ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
+ns2.col collection: * :ansplugin:`foo role
+col.foo#role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
 seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.sub.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.sub.foo3 module -- A sub-foo
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.flatcol.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.flatcol.foo module -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 These are the plugins in the ns2.flatcol collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.flatcol.foo_module>` -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.flatcol.foo2_module>` -- Another foo
+* :ansplugin:`foo module <ns2.flatcol.foo#module>` -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.flatcol.foo2#module>` -- Another foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/build.sh` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/build.sh`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Create collection documentation into temporary directory
 rm -rf temp-rst
 mkdir -p temp-rst
 chmod og-w temp-rst  # antsibull-docs wants that directory only readable by itself
 antsibull-docs \
     --config-file antsibull-docs.cfg \
     collection \
+    --output-format ansible-docsite \
     --dest-dir temp-rst \
     ns.col1 ns.col2 ns2.col
 
 # Copy collection documentation into source directory
 rsync -cprv --delete-after temp-rst/collections/ rst/collections/
 
 # Build Sphinx site
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-collections/conf.py` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-collections/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/build.sh` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/build.sh`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 mkdir -p temp-rst
 chmod og-w temp-rst  # antsibull-docs wants that directory only readable by itself
 antsibull-docs \
     --config-file antsibull-docs.cfg \
     collection \
     --fail-on-error \
     --squash-hierarchy \
+    --output-format ansible-docsite \
     --dest-dir temp-rst \
     ns.col1
 
 # Copy collection documentation into source directory
 rsync -cprv --delete-after temp-rst/ rst/
 
 # Build Sphinx site
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-config/conf.py` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-config/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/build.sh` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-current/conf.py` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-current/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-sphinx-init-extra/conf.py` & `antsibull_docs-2.3.0/tests/functional/baseline-sphinx-init-extra/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.bar filter -- The bar filter
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/bar_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/bar_test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-.. _ansible_collections.ns2.col.is_bar_test:
-
 .. Title
 
 ns2.col.bar test -- Is something a bar
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -66,15 +61,15 @@
 .. Description
 
 - Check whether a path is a bar.
 
 
 .. Aliases
 
-Aliases: 
+Aliases: is_bar
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 Environment variables used by the ansible-core configuration are documented in :ref:`ansible_configuration_settings`.
 
 .. envvar:: ANSIBLE_FOO_EXE
 
     Foo executable.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_FOO_FILENAME_EXT
 
     All extensions to check.
 
     *Used by:*
-    :ref:`ns2.col.foo vars plugin <ansible_collections.ns2.col.foo_vars>`
+    :ansplugin:`ns2.col.foo vars plugin <ns2.col.foo#vars>`
 .. envvar:: ANSIBLE_FOO_USER
 
     User you 'become' to execute the task.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_REMOTE_TEMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
 .. envvar:: ANSIBLE_REMOTE_TMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -62,14 +58,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Foo bar.
 - See \ :ansopt:`ns2.col.foo#role:main:foo\_param\_1`\  for a random role parameter reference. And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\  for one with a value.
+- Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\  and \ :ansopt:`ns2.col.foo\_redirect#module:baz`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_become.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_become:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo become -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cache:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cache -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cache: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cache -- Foo files \ :
-ansopt:`ns2.col.foo#cache:bar`\
+ansible.builtin .. Title ns2.col.foo cache -- Foo files \ :ansopt:
+`ns2.col.foo#cache:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This cache plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.9.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Cache foo files. .. Aliases .. Requirements .. Options
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_callback:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo callback -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_callback: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo callback -- Foo output
-\ :ansopt:`ns2.col.foo#callback:bar`\
+ansible.builtin .. Title ns2.col.foo callback -- Foo output \ :ansopt:
+`ns2.col.foo#callback:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This callback plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.0.1 .. contents:: :local: :depth: 1 .. Deprecated Callback plugin
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cliconf:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cliconf -- Foo router CLI config
 ++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cliconf: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cliconf -- Foo router
-CLI config ++++++++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This cliconf plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo cliconf -- Foo router CLI config
+++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+cliconf plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - This is a CLI config for foo
 routers. Whatever these are. .. Aliases .. Requirements .. Options ..
 Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values .. Status
 (Presently only deprecated) .. Authors Authors ~~~~~~~ - Felix Fontein
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_connection:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo connection -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo filter -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_inventory:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo inventory -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_inventory: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo inventory -- The foo
-inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+ansible.builtin .. Title ns2.col.foo inventory -- The foo inventory \ :ansopt:
+`ns2.col.foo#inventory:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This inventory plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.5.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_lookup:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo lookup -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo module -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -72,14 +68,15 @@
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
 - \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
+Aliases: foo_redirect
 
 .. Requirements
 
 .. _ansible_collections.ns2.col.foo_module_requirements:
 
 Requirements
 ------------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns2.col.foo role -- Foo role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_shell:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo shell -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_strategy:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo strategy -- Executes tasks in foo
 +++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_strategy: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo strategy -- Executes
-tasks in foo +++++++++++++++++++++++++++++++++++++++++++++ .. Collection note
-.. note:: This strategy plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo strategy -- Executes tasks in foo
++++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+strategy plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.1.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is something funny. Or at least I think so from its
 name. .. Aliases .. Requirements .. Options .. Attributes .. Notes .. Seealso
 .. Examples .. Facts .. Return values .. Status (Presently only deprecated) ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_test.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo test -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_vars:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo vars -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -70,181 +70,185 @@
 
 These are the plugins in the ns2.col collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.col.foo2_module>` -- Another foo
-* :ref:`sub.foo3 module <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
+* :ansplugin:`foo module <ns2.col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.col.foo2#module>` -- Another foo
+* :ansplugin:`sub.foo3 module <ns2.col.sub.foo3#module>` -- A sub-foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
     sub.foo3_module
 
 
 Become Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo become <ansible_collections.ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
+* :ansplugin:`foo become <ns2.col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_become
 
 
 Cache Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo cache <ansible_collections.ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
+* :ansplugin:`foo cache <ns2.col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cache
 
 
 Callback Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo callback <ansible_collections.ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
+* :ansplugin:`foo callback <ns2.col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_callback
 
 
 Cliconf Plugins
 ~~~~~~~~~~~~~~~
 
-* :ref:`foo cliconf <ansible_collections.ns2.col.foo_cliconf>` -- Foo router CLI config
+* :ansplugin:`foo cliconf <ns2.col.foo#cliconf>` -- Foo router CLI config
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cliconf
 
 
 Connection Plugins
 ~~~~~~~~~~~~~~~~~~
 
-* :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
+* :ansplugin:`foo connection <ns2.col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
-* :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
+* :ansplugin:`bar filter <ns2.col.bar#filter>` -- The bar filter
+* :ansplugin:`foo filter <ns2.col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
-* :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
+* :ansplugin:`foo inventory <ns2.col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_inventory
 
 
 Lookup Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo lookup <ansible_collections.ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
+* :ansplugin:`foo lookup <ns2.col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_lookup
 
 
 Shell Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo shell <ansible_collections.ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
+* :ansplugin:`foo shell <ns2.col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_shell
 
 
 Strategy Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
+* :ansplugin:`foo strategy <ns2.col.foo#strategy>` -- Executes tasks in foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
-* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
-* :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
+* :ansplugin:`bar test <ns2.col.bar#test>` -- Is something a bar
+* :ansplugin:`foo test <ns2.col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
-* :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
+* :ansplugin:`foo vars <ns2.col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_vars
 
 
 Role Index
 ----------
 
 These are the roles in the ns2.col collection:
 
-* :ref:`foo role <ansible_collections.ns2.col.foo_role>` -- Foo role
+* :ansplugin:`foo role <ns2.col.foo#role>` -- Foo role
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_role
 
+
+.. seealso::
+
+    List of :ref:`collections <list_of_collections>` with docs hosted here.
```

#### html2text {}

```diff
@@ -9,52 +9,52 @@
 matrix.to/#/#users:ansible.im>`__. - IRC channel :literal:`#ansible` (Libera
 network): `General usage and support questions
 web.libera.chat/?channel=#ansible>`__. - Mailing list: `Ansible Project List
 groups.google.com/g/ansible-project>`__. (`Subscribe
 subscribe@googlegroups.com?subject=subscribe>`__) .. toctree:: :maxdepth: 1
 Guides ------ .. toctree:: :maxdepth: 1 docsite/filter_guide Plugin Index -----
 ------- These are the plugins in the ns2.col collection: Modules ~~~~~~~ * :
-ref:`foo module
-ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :ref:
-`foo2 module
-ns2.col.foo2_module>` -- Another foo * :ref:`sub.foo3 module
-ns2.col.sub.foo3_module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
-foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :ref:
-`foo become
-ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ref:
-`foo cache
-ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo callback
-ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
+ansplugin:`foo module
+col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :
+ansplugin:`foo2 module
+col.foo2#module>` -- Another foo * :ansplugin:`sub.foo3 module
+col.sub.foo3#module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
+foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :
+ansplugin:`foo become
+col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ansplugin:`foo
+cache
+col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo callback
+col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
-:ref:`foo cliconf
-ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
-hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
-connection
-ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`bar filter
-ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
-ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
+:ansplugin:`foo cliconf
+col.foo#cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :hidden:
+foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ansplugin:`foo connection
+col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`bar filter
+col.bar#filter>` -- The bar filter * :ansplugin:`foo filter
+col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
-~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
-ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
-~~~~~~~~~~~~~~ * :ref:`foo lookup
-ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
-`foo shell
-ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo strategy
-ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
-ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
-ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
+~~~~~~~~~~~~~~~~~ * :ansplugin:`foo inventory
+col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`foo lookup
+col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
+toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :
+ansplugin:`foo shell
+col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo strategy
+col.foo#strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :hidden:
+foo_strategy Test Plugins ~~~~~~~~~~~~ * :ansplugin:`bar test
+col.bar#test>` -- Is something a bar * :ansplugin:`foo test
+col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
-ref:`foo vars
-ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
+ansplugin:`foo vars
+col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
-ns2.col collection: * :ref:`foo role
-ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role
+ns2.col collection: * :ansplugin:`foo role
+col.foo#role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
+seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.sub.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.sub.foo3 module -- A sub-foo
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 Environment variables used by the ansible-core configuration are documented in :ref:`ansible_configuration_settings`.
 
 .. envvar:: ANSIBLE_FOO_EXE
 
     Foo executable.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_FOO_FILENAME_EXT
 
     All extensions to check.
 
     *Used by:*
-    :ref:`ns2.col.foo vars plugin <ansible_collections.ns2.col.foo_vars>`
+    :ansplugin:`ns2.col.foo vars plugin <ns2.col.foo#vars>`
 .. envvar:: ANSIBLE_FOO_USER
 
     User you 'become' to execute the task.
 
     *Used by:*
-    :ref:`ns2.col.foo become plugin <ansible_collections.ns2.col.foo_become>`
+    :ansplugin:`ns2.col.foo become plugin <ns2.col.foo#become>`
 .. envvar:: ANSIBLE_REMOTE_TEMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
 .. envvar:: ANSIBLE_REMOTE_TMP
 
     Temporary directory to use on targets when executing tasks.
 
     *Used by:*
-    :ref:`ns2.col.foo shell plugin <ansible_collections.ns2.col.foo_shell>`
+    :ansplugin:`ns2.col.foo shell plugin <ns2.col.foo#shell>`
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.bar filter -- The bar filter
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.bar_filter: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.bar filter -- The bar
-filter ++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
-filter plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.bar filter -- The bar filter
+++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This filter
+plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.bar`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 2.0.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Do some barring. .. Aliases .. Requirements .. Input Input -
 ---- This describes the input of the filter, the value before ``|
 ns2.col.bar``. .. raw:: html
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.bar_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-.. _ansible_collections.ns2.col.is_bar_test:
-
 .. Title
 
 ns2.col.bar test -- Is something a bar
 ++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -66,15 +61,15 @@
 .. Description
 
 - Check whether a path is a bar.
 
 
 .. Aliases
 
-Aliases: 
+Aliases: is_bar
 
 .. Requirements
```

#### html2text {}

```diff
@@ -9,25 +9,24 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.bar_test: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases ..
-_ansible_collections.ns2.col.is_bar_test: .. Title ns2.col.bar test -- Is
-something a bar ++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This test plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.bar test -- Is something a bar
+++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This test
+plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.bar`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - Check whether a path is a bar. ..
-Aliases Aliases: .. Requirements .. Input Input ----- This describes the input
-of the test, the value before ``is ns2.col.bar`` or ``is not ns2.col.bar``. ..
-raw:: html
+Aliases Aliases: is_bar .. Requirements .. Input Input ----- This describes the
+input of the test, the value before ``is ns2.col.bar`` or ``is not
+ns2.col.bar``. .. raw:: html
 Parameter Comments
 Input     A path.
 path
 .. Options .. Attributes .. Notes .. Seealso .. Examples Examples -------- ..
 code-block:: yaml+jinja is_path_bar: "{{ '/etc/hosts' is ns2.col.bar }}}" ..
 Facts .. Return values Return Value ------------ .. raw:: html
 Key          Description
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo2_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -62,14 +58,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Foo bar.
 - See \ :ansopt:`ns2.col.foo#role:main:foo\_param\_1`\  for a random role parameter reference. And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\  for one with a value.
+- Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\  and \ :ansopt:`ns2.col.foo\_redirect#module:baz`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

#### html2text {}

```diff
@@ -9,24 +9,26 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo2_module: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo2 module -- Another foo
+ansible.builtin .. Title ns2.col.foo2 module -- Another foo
 ++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This module is
 part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo2`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - Foo bar. - See \ :ansopt:
 `ns2.col.foo#role:main:foo\_param\_1`\ for a random role parameter reference.
-And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\ for one with a value.
-.. Aliases .. Requirements .. Options Parameters ---------- .. raw:: html
+And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\ for one with a value. -
+Reference using alias - \ :ansopt:`ns2.col.foo\_redirect#module:bar`\ and \ :
+ansopt:`ns2.col.foo\_redirect#module:baz`\ . .. Aliases .. Requirements ..
+Options Parameters ---------- .. raw:: html
 Parameter Comments
 bar       Some bar.
 string    See foo_param_1 for a random role parameter reference. And
           foo_param_2=42 for one with a value.
 .. Attributes Attributes ---------- .. rst-class:: ansible-option-table ..
 list-table:: :width: 100% :widths: auto :header-rows: 1 * - Attribute - Support
 - Description * - .. raw:: html
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_become:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo become -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_become: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo become -- Use foo \ :
-ansopt:`ns2.col.foo#become:bar`\
+ansible.builtin .. Title ns2.col.foo become -- Use foo \ :ansopt:
+`ns2.col.foo#become:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This become plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated DEPRECATED ---------- :Removed in: version 5.0.0 :Why: Just some
 text. This one has more than one line. And one more. :Alternative: I don't know
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cache:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cache -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cache: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cache -- Foo files \ :
-ansopt:`ns2.col.foo#cache:bar`\
+ansible.builtin .. Title ns2.col.foo cache -- Foo files \ :ansopt:
+`ns2.col.foo#cache:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This cache plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.9.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Cache foo files. .. Aliases .. Requirements .. Options
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_callback:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo callback -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_callback: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo callback -- Foo output
-\ :ansopt:`ns2.col.foo#callback:bar`\
+ansible.builtin .. Title ns2.col.foo callback -- Foo output \ :ansopt:
+`ns2.col.foo#callback:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This callback plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.0.1 .. contents:: :local: :depth: 1 .. Deprecated Callback plugin
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_cliconf:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo cliconf -- Foo router CLI config
 ++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_cliconf: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo cliconf -- Foo router
-CLI config ++++++++++++++++++++++++++++++++++++++++++++ .. Collection note ..
-note:: This cliconf plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo cliconf -- Foo router CLI config
+++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+cliconf plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - This is a CLI config for foo
 routers. Whatever these are. .. Aliases .. Requirements .. Options ..
 Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values .. Status
 (Presently only deprecated) .. Authors Authors ~~~~~~~ - Felix Fontein
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_connection:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo connection -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_connection: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo connection -- Foo
-connection \ :ansopt:`ns2.col.foo#connection:bar`\
+ansible.builtin .. Title ns2.col.foo connection -- Foo connection \ :ansopt:
+`ns2.col.foo#connection:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This connection plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.2.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_filter:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo filter -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_filter: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo filter -- The foo
-filter \ :ansopt:`ns2.col.foo#filter:bar`\
+ansible.builtin .. Title ns2.col.foo filter -- The foo filter \ :ansopt:
+`ns2.col.foo#filter:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This filter plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.3.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - Do some fooing. .. Aliases .. Requirements .. Input Input --
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_inventory:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo inventory -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_inventory: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo inventory -- The foo
-inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+ansible.builtin .. Title ns2.col.foo inventory -- The foo inventory \ :ansopt:
+`ns2.col.foo#inventory:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 .. Collection note .. note:: This inventory plugin is part of the `ns2.col
 collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 0.5.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_lookup:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo lookup -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_lookup: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo lookup -- Look up some
-foo \ :ansopt:`ns2.col.foo#lookup:bar`\
+ansible.builtin .. Title ns2.col.foo lookup -- Look up some foo \ :ansopt:
+`ns2.col.foo#lookup:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This lookup plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.0.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This looks up some foo. - Whatever that is. .. Aliases ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo module -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
 
@@ -72,14 +68,15 @@
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
 - \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
+Aliases: foo_redirect
 
 .. Requirements
 
 .. _ansible_collections.ns2.col.foo_module_requirements:
 
 Requirements
 ------------
```

#### html2text {}

```diff
@@ -9,28 +9,28 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_module: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo module -- Do some foo
-\ :ansopt:`ns2.col.foo#module:bar`\
+ansible.builtin .. Title ns2.col.foo module -- Do some foo \ :ansopt:
+`ns2.col.foo#module:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This module is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. You need further requirements to
 be able to use this module, see :ref:`Requirements
 ns2.col.foo_module_requirements>` for details. To use it in a playbook,
 specify: :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-
 added New in ns2.col 2.0.0 .. contents:: :local: :depth: 1 .. Deprecated
 Synopsis -------- .. Description - Does some foo on the remote host. - Whether
 foo is magic or not has not yet been determined. - \ :ansenvvarref:`FOOBAR1`\ ,
 \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\
-. .. Aliases .. Requirements ..
+. .. Aliases Aliases: foo_redirect .. Requirements ..
 _ansible_collections.ns2.col.foo_module_requirements: Requirements -----------
 - The below requirements are needed on the host that executes this module. -
 Foo on remote. .. Options Parameters ---------- .. raw:: html
 Parameter               Comments
 bar                     A bar.
 aliases: baz            Independent from foo.
 list / elements=integer Do not confuse with bar.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 .. role:: ansible-option-choices-default-mark
 .. role:: ansible-option-default-bold
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_role:
 
-.. Anchors: aliases
-
-
 .. Title
 
 ns2.col.foo role -- Foo role
 ++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -7,17 +7,17 @@
 attribute-support-label .. role:: ansible-attribute-support-property .. role::
 ansible-attribute-support-full .. role:: ansible-attribute-support-partial ..
 role:: ansible-attribute-support-none .. role:: ansible-attribute-support-na ..
 role:: ansible-option-type .. role:: ansible-option-elements .. role:: ansible-
 option-required .. role:: ansible-option-versionadded .. role:: ansible-option-
 aliases .. role:: ansible-option-choices .. role:: ansible-option-choices-
 default-mark .. role:: ansible-option-default-bold .. Anchors ..
-_ansible_collections.ns2.col.foo_role: .. Anchors: aliases .. Title ns2.col.foo
-role -- Foo role ++++++++++++++++++++++++++++ .. Collection note .. note:: This
-role is part of the `ns2.col collection
+_ansible_collections.ns2.col.foo_role: .. Title ns2.col.foo role -- Foo role
+++++++++++++++++++++++++++++ .. Collection note .. note:: This role is part of
+the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. contents:: :local: :depth: 2 .. Entry point title Entry
 point ``main`` -- Foo role -------------------------------- .. version_added ..
 rst-class:: ansible-version-added New in ns2.col 0.2.0 .. Deprecated DEPRECATED
 ^^^^^^^^^^ :Removed in: version 5.0.0 :Why: Just some text. This one has more
 than one line. And one more. :Alternative: I don't know of any alternative.
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_shell:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo shell -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_shell: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo shell -- Foo shell \ :
-ansopt:`ns2.col.foo#shell:bar`\
+ansible.builtin .. Title ns2.col.foo shell -- Foo shell \ :ansopt:
+`ns2.col.foo#shell:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This shell plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.0.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is for the foo shell. .. Aliases .. Requirements ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_strategy:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo strategy -- Executes tasks in foo
 +++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_strategy: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo strategy -- Executes
-tasks in foo +++++++++++++++++++++++++++++++++++++++++++++ .. Collection note
-.. note:: This strategy plugin is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.foo strategy -- Executes tasks in foo
++++++++++++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
+strategy plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
 in ns2.col 1.1.0 .. contents:: :local: :depth: 1 .. Deprecated Synopsis -------
 - .. Description - This is something funny. Or at least I think so from its
 name. .. Aliases .. Requirements .. Options .. Attributes .. Notes .. Seealso
 .. Examples .. Facts .. Return values .. Status (Presently only deprecated) ..
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_test:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo test -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_test: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo test -- Is something a
-foo \ :ansopt:`ns2.col.foo#test:bar`\
+ansible.builtin .. Title ns2.col.foo test -- Is something a foo \ :ansopt:
+`ns2.col.foo#test:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This test plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - Check whether the input
 dictionary is a foo. .. Aliases .. Requirements .. Input Input ----- This
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.foo_vars:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.foo vars -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.foo_vars: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.foo vars -- Load foo \ :
-ansopt:`ns2.col.foo#vars:bar`\
+ansible.builtin .. Title ns2.col.foo vars -- Load foo \ :ansopt:
+`ns2.col.foo#vars:bar`\
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ .. Collection
 note .. note:: This vars plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. You need further requirements to
 be able to use this vars plugin, see :ref:`Requirements
 ns2.col.foo_vars_requirements>` for details. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-added New
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/index.rst`

 * *Files 25% similar despite different names*

```diff
@@ -70,185 +70,181 @@
 
 These are the plugins in the ns2.col collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
-* :ref:`foo2 module <ansible_collections.ns2.col.foo2_module>` -- Another foo
-* :ref:`sub.foo3 module <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
+* :ansplugin:`foo module <ns2.col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
+* :ansplugin:`foo2 module <ns2.col.foo2#module>` -- Another foo
+* :ansplugin:`sub.foo3 module <ns2.col.sub.foo3#module>` -- A sub-foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_module
     foo2_module
     sub.foo3_module
 
 
 Become Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo become <ansible_collections.ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
+* :ansplugin:`foo become <ns2.col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_become
 
 
 Cache Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo cache <ansible_collections.ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
+* :ansplugin:`foo cache <ns2.col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cache
 
 
 Callback Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo callback <ansible_collections.ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
+* :ansplugin:`foo callback <ns2.col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_callback
 
 
 Cliconf Plugins
 ~~~~~~~~~~~~~~~
 
-* :ref:`foo cliconf <ansible_collections.ns2.col.foo_cliconf>` -- Foo router CLI config
+* :ansplugin:`foo cliconf <ns2.col.foo#cliconf>` -- Foo router CLI config
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_cliconf
 
 
 Connection Plugins
 ~~~~~~~~~~~~~~~~~~
 
-* :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
+* :ansplugin:`foo connection <ns2.col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
-* :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
+* :ansplugin:`bar filter <ns2.col.bar#filter>` -- The bar filter
+* :ansplugin:`foo filter <ns2.col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
-* :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
+* :ansplugin:`foo inventory <ns2.col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_inventory
 
 
 Lookup Plugins
 ~~~~~~~~~~~~~~
 
-* :ref:`foo lookup <ansible_collections.ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
+* :ansplugin:`foo lookup <ns2.col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_lookup
 
 
 Shell Plugins
 ~~~~~~~~~~~~~
 
-* :ref:`foo shell <ansible_collections.ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
+* :ansplugin:`foo shell <ns2.col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_shell
 
 
 Strategy Plugins
 ~~~~~~~~~~~~~~~~
 
-* :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
+* :ansplugin:`foo strategy <ns2.col.foo#strategy>` -- Executes tasks in foo
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
-* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
-* :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
+* :ansplugin:`bar test <ns2.col.bar#test>` -- Is something a bar
+* :ansplugin:`foo test <ns2.col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
-* :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
+* :ansplugin:`foo vars <ns2.col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_vars
 
 
 Role Index
 ----------
 
 These are the roles in the ns2.col collection:
 
-* :ref:`foo role <ansible_collections.ns2.col.foo_role>` -- Foo role
+* :ansplugin:`foo role <ns2.col.foo#role>` -- Foo role
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
     foo_role
 
-
-.. seealso::
-
-    List of :ref:`collections <list_of_collections>` with docs hosted here.
```

#### html2text {}

```diff
@@ -9,53 +9,51 @@
 matrix.to/#/#users:ansible.im>`__. - IRC channel :literal:`#ansible` (Libera
 network): `General usage and support questions
 web.libera.chat/?channel=#ansible>`__. - Mailing list: `Ansible Project List
 groups.google.com/g/ansible-project>`__. (`Subscribe
 subscribe@googlegroups.com?subject=subscribe>`__) .. toctree:: :maxdepth: 1
 Guides ------ .. toctree:: :maxdepth: 1 docsite/filter_guide Plugin Index -----
 ------- These are the plugins in the ns2.col collection: Modules ~~~~~~~ * :
-ref:`foo module
-ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :ref:
-`foo2 module
-ns2.col.foo2_module>` -- Another foo * :ref:`sub.foo3 module
-ns2.col.sub.foo3_module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
-foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :ref:
-`foo become
-ns2.col.foo_become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ref:
-`foo cache
-ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo callback
-ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
+ansplugin:`foo module
+col.foo#module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ * :
+ansplugin:`foo2 module
+col.foo2#module>` -- Another foo * :ansplugin:`sub.foo3 module
+col.sub.foo3#module>` -- A sub-foo .. toctree:: :maxdepth: 1 :hidden:
+foo_module foo2_module sub.foo3_module Become Plugins ~~~~~~~~~~~~~~ * :
+ansplugin:`foo become
+col.foo#become>` -- Use foo \ :ansopt:`ns2.col.foo#become:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_become Cache Plugins ~~~~~~~~~~~~~ * :ansplugin:`foo
+cache
+col.foo#cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_cache Callback Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo callback
+col.foo#callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
-:ref:`foo cliconf
-ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
-hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
-connection
-ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`bar filter
-ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
-ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
+:ansplugin:`foo cliconf
+col.foo#cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :hidden:
+foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ansplugin:`foo connection
+col.foo#connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`bar filter
+col.bar#filter>` -- The bar filter * :ansplugin:`foo filter
+col.foo#filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
-~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
-ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
-bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
-~~~~~~~~~~~~~~ * :ref:`foo lookup
-ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
-`foo shell
-ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
-ref:`foo strategy
-ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
-ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
-ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
+~~~~~~~~~~~~~~~~~ * :ansplugin:`foo inventory
+col.foo#inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\
+.. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins ~~~~~~~~~~~~~~
+* :ansplugin:`foo lookup
+col.foo#lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
+toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :
+ansplugin:`foo shell
+col.foo#shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ .. toctree:: :
+maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :ansplugin:
+`foo strategy
+col.foo#strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :hidden:
+foo_strategy Test Plugins ~~~~~~~~~~~~ * :ansplugin:`bar test
+col.bar#test>` -- Is something a bar * :ansplugin:`foo test
+col.foo#test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
-ref:`foo vars
-ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
+ansplugin:`foo vars
+col.foo#vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
-ns2.col collection: * :ref:`foo role
-ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
-seealso:: List of :ref:`collections ` with docs hosted here.
+ns2.col collection: * :ansplugin:`foo role
+col.foo#role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 .. Anchors
 
 .. _ansible_collections.ns2.col.sub.foo3_module:
 
 .. Anchors: short name for ansible.builtin
 
-.. Anchors: aliases
-
-
-
 .. Title
 
 ns2.col.sub.foo3 module -- A sub-foo
 ++++++++++++++++++++++++++++++++++++
 
 .. Collection note
```

#### html2text {}

```diff
@@ -9,17 +9,17 @@
 none .. role:: ansible-attribute-support-na .. role:: ansible-option-type ..
 role:: ansible-option-elements .. role:: ansible-option-required .. role::
 ansible-option-versionadded .. role:: ansible-option-aliases .. role:: ansible-
 option-choices .. role:: ansible-option-choices-default-mark .. role:: ansible-
 option-default-bold .. role:: ansible-option-configuration .. role:: ansible-
 option-returned-bold .. role:: ansible-option-sample-bold .. Anchors ..
 _ansible_collections.ns2.col.sub.foo3_module: .. Anchors: short name for
-ansible.builtin .. Anchors: aliases .. Title ns2.col.sub.foo3 module -- A sub-
-foo ++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This
-module is part of the `ns2.col collection
+ansible.builtin .. Title ns2.col.sub.foo3 module -- A sub-foo
+++++++++++++++++++++++++++++++++++++ .. Collection note .. note:: This module
+is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.sub.foo3`. .. version_added .. contents:: :local: :depth: 1 ..
 Deprecated Synopsis -------- .. Description - Foo sub bar. - See \ :ansopt:
 `ns2.col.foo#role:main:foo\_param\_1`\ for a random role parameter reference.
 And \ :ansopt:`ns2.col.foo#role:main:foo\_param\_2=42`\ for one with a value.
 .. Aliases .. Requirements .. Options Parameters ---------- .. raw:: html
```

### Comparing `antsibull_docs-2.2.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst` & `antsibull_docs-2.3.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 author:
     - "Another one (@ansible-community)"
 short_description: Another foo
 description:
     - Foo bar.
     - See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And
       O(ns2.col.foo#role:main:foo_param_2=42) for one with a value.
+    - Reference using alias - O(ns2.col.foo_redirect#module:bar) and O(ns2.col.foo_redirect#module:baz).
 options:
     bar:
         description:
           - Some bar.
           - See O(ns2.col.foo#role:main:foo_param_1) for a random role parameter reference. And
             O(ns2.col.foo#role:main:foo_param_2=42) for one with a value.
         type: str
```

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py` & `antsibull_docs-2.3.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py` & `antsibull_docs-2.3.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py` & `antsibull_docs-2.3.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/test_schema.py` & `antsibull_docs-2.3.0/tests/functional/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_become_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_become_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cache_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cache_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_callback_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_callback_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_cliconf_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_cliconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_connection_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_filter_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_filter_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_httpapi_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_httpapi_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_inventory_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_inventory_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_lookup_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_lookup_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_module_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_module_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_netconf_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_netconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_role_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_role_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_shell_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_shell_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_strategy_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_strategy_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_test_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_test_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/one_vars_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/one_vars_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/functional/schema/good_data/ssh_connection_results.json` & `antsibull_docs-2.3.0/tests/functional/schema/good_data/ssh_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/units/test_jinja2.py` & `antsibull_docs-2.3.0/tests/units/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/units/markup/test_counter.py` & `antsibull_docs-2.3.0/tests/units/markup/test_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/tests/units/markup/test_markup.py` & `antsibull_docs-2.3.0/tests/units/markup/test_markup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 # SPDX-FileCopyrightText: 2020, Ansible Project
 
 from __future__ import annotations
 
 import pytest
 
 from antsibull_docs.jinja2 import OutputFormat
-from antsibull_docs.markup.rstify import get_rst_formatter, rst_escape, rst_ify
+from antsibull_docs.markup.rstify import (
+    get_rst_formatter_link_provider,
+    rst_escape,
+    rst_ify,
+)
 
 RST_IFY_DATA = {
     # No substitutions
     "no-op": "no-op",
     "no-op Z(test)": "no-op Z(test)",
     # Simple cases of all substitutions
     "I(italic)": r"\ :emphasis:`italic`\ ",
@@ -31,17 +35,25 @@
     "L(the user guide, https://docs.ansible.com/)": r"\ `the user guide <https://docs.ansible.com/>`__\ ",
     "R(the user guide, user-guide)": r"\ :ref:`the user guide <user-guide>`\ ",
 }
 
 
 @pytest.mark.parametrize("text, expected", RST_IFY_DATA.items())
 def test_rst_ify(text, expected):
-    formatter = get_rst_formatter(OutputFormat.ANSIBLE_DOCSITE)
+    formatter, link_provider = get_rst_formatter_link_provider(
+        OutputFormat.ANSIBLE_DOCSITE
+    )
     assert (
-        rst_ify(text, formatter, plugin_fqcn="foo.bar.baz", plugin_type="module")[0]
+        rst_ify(
+            text,
+            formatter,
+            plugin_fqcn="foo.bar.baz",
+            plugin_type="module",
+            link_provider=link_provider,
+        )[0]
         == expected
     )
 
 
 RST_ESCAPE_DATA = {
     "": "",
     "no-op": "no-op",
```

### Comparing `antsibull_docs-2.2.0/tests/units/markup/test_semantic_helper.py` & `antsibull_docs-2.3.0/tests/units/markup/test_semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/.gitignore` & `antsibull_docs-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/README.md` & `antsibull_docs-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/pyproject.toml` & `antsibull_docs-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs"
-version = "2.2.0"
+version = "2.3.0"
 description = "Tools for building Ansible documentation"
 license = "GPL-3.0-or-later"
 license-files = {globs=["LICENSES/*.txt"]}
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Ansible",
```

### Comparing `antsibull_docs-2.2.0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs-2.3.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.2.0/PKG-INFO` & `antsibull_docs-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs
-Version: 2.2.0
+Version: 2.3.0
 Summary: Tools for building Ansible documentation
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-docs/issues
 Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later
```

