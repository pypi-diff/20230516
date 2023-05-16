# Comparing `tmp/robotcode_language_server-0.38.0.tar.gz` & `tmp/robotcode_language_server-0.39.0.tar.gz`

## Comparing `robotcode_language_server-0.38.0.tar` & `robotcode_language_server-0.39.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54596 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63744 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15233 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80441 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.38.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    56379 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63734 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80441 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19441 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40438 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11635 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.39.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from robotcode.core.dataclasses import CamelSnakeMixin, from_dict
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.core.lsp.types import InitializeError
 from robotcode.jsonrpc2.protocol import JsonRPCErrorException, JsonRPCErrors, ProtocolPartDescriptor
 from robotcode.language_server.common.parts.document_symbols import symbol_information_label
 from robotcode.language_server.common.protocol import LanguageDefinition, LanguageServerProtocol
+from robotcode.robot.config.model import RobotBaseProfile
 
 from ..__version__ import __version__
 from .configuration import RobotConfig
 from .parts.code_action_documentation import RobotCodeActionDocumentationProtocolPart
 from .parts.code_action_fixes import RobotCodeActionFixesProtocolPart
 from .parts.codelens import RobotCodeLensProtocolPart
 from .parts.completion import RobotCompletionProtocolPart
@@ -117,16 +118,17 @@
         #     id="feature",
         #     extensions=[".feature", ".md"],
         #     aliases=["feature", "gherkin", "Gherkin", "cucumber"],
         # ),
         LanguageDefinition(id="markdown", extensions=[".md"]),
     ]
 
-    def __init__(self, server: "RobotLanguageServer"):
+    def __init__(self, server: "RobotLanguageServer", profile: Optional[RobotBaseProfile] = None):
         super().__init__(server)
+        self.profile = profile if profile is not None else RobotBaseProfile()
         self.options = Options()
         self.on_initialize.add(self._on_initialize)
         self.on_initialized.add(self._on_initialized)
         self.on_shutdown.add(self._on_shutdown)
 
     @_logger.call
     async def _on_shutdown(self, sender: Any) -> None:
@@ -165,14 +167,26 @@
 
     async def _on_did_change_configuration(self, sender: Any, settings: Dict[str, Any]) -> None:
         pass
 
     async def _on_initialized(self, sender: Any) -> None:
         for folder in self.workspace.workspace_folders:
             config: RobotConfig = await self.workspace.get_configuration(RobotConfig, folder.uri, request=False)
+            for k, v in (self.profile.env or {}).items():
+                os.environ[k] = v
+
+            for p in self.profile.python_path or []:
+                pa = Path(str(p))
+                if not pa.is_absolute():
+                    pa = Path(folder.uri.to_path(), pa)
+
+                absolute_path = str(pa.absolute())
+                if absolute_path not in sys.path:
+                    sys.path.insert(0, absolute_path)
+
             if config is not None:
                 if config.env:
                     for k, v in config.env.items():
                         os.environ[k] = v
 
                 if config.python_path:
                     for p in config.python_path:
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -540,16 +540,20 @@
         self._variables_lock = Lock()
         self._variables: OrderedDict[_VariablesEntryKey, _VariablesEntry] = OrderedDict()
         self.file_watchers: List[FileWatcherEntry] = []
         self.parent_protocol.documents.did_create_uri.add(self._do_imports_changed)
         self.parent_protocol.documents.did_change.add(self.resource_document_changed)
         self._command_line_variables: Optional[List[VariableDefinition]] = None
         self._command_line_variables_lock = Lock()
+        self._resolvable_command_line_variables: Optional[Dict[str, Any]] = None
+        self._resolvable_command_line_variables_lock = Lock()
 
         self._environment = dict(os.environ)
+        if self.parent_protocol.profile.env:
+            self._environment.update(self.parent_protocol.profile.env)
         self._environment.update(self.config.robot.env)
 
         self._library_files_cache = AsyncSimpleLRUCache()
         self._resource_files_cache = AsyncSimpleLRUCache()
         self._variables_files_cache = AsyncSimpleLRUCache()
 
     @property
@@ -563,36 +567,67 @@
 
     @_logger.call
     async def get_command_line_variables(self) -> List[VariableDefinition]:
         from robot.utils.text import split_args_from_name_or_path
 
         async with self._command_line_variables_lock:
             if self._command_line_variables is None:
-                command_line_vars: List[VariableDefinition] = [
+                command_line_vars: List[VariableDefinition] = []
+                command_line_vars += [
+                    CommandLineVariableDefinition(0, 0, 0, 0, "", f"${{{k}}}", None, has_value=True, value=(v,))
+                    for k, v in (self.parent_protocol.profile.variables or {}).items()
+                ]
+
+                for variable_file in self.parent_protocol.profile.variable_files or []:
+                    name, args = split_args_from_name_or_path(str(variable_file))
+                    try:
+                        lib_doc = await self.get_libdoc_for_variables_import(
+                            name, tuple(args), str(self.folder.to_path()), self, resolve_command_line_vars=False
+                        )
+                        if lib_doc is not None:
+                            command_line_vars += lib_doc.variables
+
+                    except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
+                        raise
+                    except BaseException as e:
+                        # TODO add diagnostics
+                        self._logger.exception(e)
+
+                command_line_vars += [
                     CommandLineVariableDefinition(0, 0, 0, 0, "", f"${{{k}}}", None, has_value=True, value=(v,))
                     for k, v in self.config.robot.variables.items()
                 ]
                 for variable_file in self.config.robot.variable_files:
                     name, args = split_args_from_name_or_path(variable_file)
                     try:
                         lib_doc = await self.get_libdoc_for_variables_import(
-                            name, tuple(args), str(self.folder.to_path()), self
+                            name, tuple(args), str(self.folder.to_path()), self, resolve_command_line_vars=False
                         )
                         if lib_doc is not None:
                             command_line_vars += lib_doc.variables
 
                     except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
                         raise
                     except BaseException as e:
+                        # TODO add diagnostics
                         self._logger.exception(e)
 
                 self._command_line_variables = command_line_vars
 
             return self._command_line_variables or []
 
+    async def get_resolvable_command_line_variables(self) -> Dict[str, Any]:
+        async with self._resolvable_command_line_variables_lock:
+            if self._resolvable_command_line_variables is None:
+                self._resolvable_command_line_variables = {
+                    v.name: v.value for v in (await self.get_command_line_variables()) if v.has_value
+                }
+
+            return self._resolvable_command_line_variables
+
     @async_tasking_event
     async def libraries_changed(sender, libraries: List[LibraryDoc]) -> None:  # NOSONAR
         ...
 
     @async_tasking_event
     async def resources_changed(sender, resources: List[LibraryDoc]) -> None:  # NOSONAR
         ...
@@ -906,15 +941,15 @@
         from robot.variables.search import contains_variable
 
         if contains_variable(name, "$@&%"):
             return find_library(
                 name,
                 str(self.folder.to_path()),
                 base_dir,
-                self.config.robot.variables if self.config.robot is not None else None,
+                await self.get_resolvable_command_line_variables(),
                 variables,
             )
 
         if name in STDLIBS:
             result = ROBOT_LIBRARY_PACKAGE + "." + name
         else:
             result = name
@@ -936,15 +971,15 @@
         from robot.variables.search import contains_variable
 
         if contains_variable(name, "$@&%"):
             return find_file(
                 name,
                 str(self.folder.to_path()),
                 base_dir,
-                self.config.robot.variables if self.config.robot is not None else None,
+                await self.get_resolvable_command_line_variables(),
                 variables,
                 file_type,
             )
 
         return str(find_file_ex(name, base_dir, file_type))
 
     async def find_variables(self, name: str, base_dir: str, variables: Optional[Dict[str, Any]] = None) -> str:
@@ -955,15 +990,15 @@
         from robot.variables.search import contains_variable
 
         if contains_variable(name, "$@&%"):
             return find_variables(
                 name,
                 str(self.folder.to_path()),
                 base_dir,
-                self.config.robot.variables if self.config.robot is not None else None,
+                await self.get_resolvable_command_line_variables(),
                 variables,
             )
 
         if get_robot_version() >= (5, 0):
             if is_variables_by_path(name):
                 return str(find_file_ex(name, base_dir, "Variables"))
 
@@ -1023,15 +1058,15 @@
                     asyncio.get_running_loop().run_in_executor(
                         executor,
                         get_library_doc,
                         name,
                         args,
                         working_dir,
                         base_dir,
-                        self.config.robot.variables if self.config.robot is not None else None,
+                        await self.get_resolvable_command_line_variables(),
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
 
             if result.stdout:
                 self._logger.warning(lambda: f"stdout captured at loading library {name}{args!r}:\n{result.stdout}")
@@ -1058,15 +1093,15 @@
 
             return result
 
         resolved_args = resolve_args(
             args,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables(),
             variables,
         )
         entry_key = _LibrariesEntryKey(source, resolved_args)
 
         async with self._libaries_lock:
             if entry_key not in self._libaries:
                 self._libaries[entry_key] = _LibrariesEntry(
@@ -1215,14 +1250,15 @@
     async def get_libdoc_for_variables_import(
         self,
         name: str,
         args: Tuple[Any, ...],
         base_dir: str,
         sentinel: Any = None,
         variables: Optional[Dict[str, Any]] = None,
+        resolve_command_line_vars: bool = True,
     ) -> VariablesDoc:
         source = await self.find_variables(
             name,
             base_dir,
             variables,
         )
 
@@ -1265,15 +1301,15 @@
                     asyncio.get_running_loop().run_in_executor(
                         executor,
                         get_variables_doc,
                         name,
                         args,
                         str(self.folder.to_path()),
                         base_dir,
-                        self.config.robot.variables if self.config.robot is not None else None,
+                        await self.get_resolvable_command_line_variables() if resolve_command_line_vars else None,
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
 
                 if result.stdout:
                     self._logger.warning(
@@ -1301,15 +1337,15 @@
                     self._logger.exception(e)
                 return result
 
         resolved_args = resolve_args(
             args,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables() if resolve_command_line_vars else None,
             variables,
         )
         entry_key = _VariablesEntryKey(source, resolved_args)
 
         async with self._variables_lock:
             if entry_key not in self._variables:
                 self._variables[entry_key] = _VariablesEntry(
@@ -1389,41 +1425,41 @@
     async def complete_library_import(
         self, name: Optional[str], base_dir: str = ".", variables: Optional[Dict[str, Any]] = None
     ) -> Optional[List[CompleteResult]]:
         return complete_library_import(
             name,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables(),
             variables,
         )
 
     async def complete_resource_import(
         self, name: Optional[str], base_dir: str = ".", variables: Optional[Dict[str, Any]] = None
     ) -> Optional[List[CompleteResult]]:
         return complete_resource_import(
             name,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables(),
             variables,
         )
 
     async def complete_variables_import(
         self, name: Optional[str], base_dir: str = ".", variables: Optional[Dict[str, Any]] = None
     ) -> Optional[List[CompleteResult]]:
         return complete_variables_import(
             name,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables(),
             variables,
         )
 
-    def resolve_variable(self, name: str, base_dir: str = ".", variables: Optional[Dict[str, Any]] = None) -> Any:
+    async def resolve_variable(self, name: str, base_dir: str = ".", variables: Optional[Dict[str, Any]] = None) -> Any:
         return resolve_variable(
             name,
             str(self.folder.to_path()),
             base_dir,
-            self.config.robot.variables if self.config.robot is not None else None,
+            await self.get_resolvable_command_line_variables(),
             variables,
         )
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1054,15 +1054,15 @@
         "${CURDIR}": str(Path(base_dir).absolute()),
         "${EXECDIR}": str(Path(working_dir).absolute()),
     }.items():
         result[k] = v
 
     if command_line_variables:
         for k1, v1 in command_line_variables.items():
-            result[f"${{{k1}}}"] = v1
+            result[k1] = v1
 
     if variables is not None:
         vars = [_Variable(k, v) for k, v in variables.items() if v is not None and not isinstance(v, NativeValue)]
         result.set_from_variable_table(vars)
 
         for k2, v2 in variables.items():
             if isinstance(v2, NativeValue):
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,14 +396,15 @@
                 base_dir = base_dir.relative_to(workspace_folder.uri.to_path())
             except ValueError:
                 pass
 
         robot_variables = resolve_robot_variables(
             str(namespace.imports_manager.folder.to_path()),
             str(base_dir),
+            await namespace.imports_manager.get_resolvable_command_line_variables(),
             variables=await namespace.get_resolvable_variables(),
         )
         try:
             name = robot_variables.replace_string(name.replace("\\", "\\\\"), ignore_errors=False)
 
             args = tuple(robot_variables.replace_string(v.replace("\\", "\\\\"), ignore_errors=False) for v in args)
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,19 +66,18 @@
         if folder is None:
             return None
 
         result = self._workspace_languages.get(folder, None)
         if result is None:
             config = await self.parent.workspace.get_configuration(RobotConfig, folder.uri)
 
-            languages = config.languages
+            languages = [str(v) for v in self.parent.profile.languages or []]
+            languages += config.languages or []
 
-            if isinstance(languages, List) and len(languages) == 0:
-                languages = None
-            if languages is None:
+            if not languages:
                 return None
 
             result = RobotLanguages()
             for lang in languages:
                 try:
                     result.add_language(lang)
                 except ValueError as e:
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             # TODO if we found a commandline var, should we look if we found a variable definition and show it in hover?
             if token_and_var is not None:
                 var_token, variable = token_and_var
 
                 if variable.has_value or variable.resolvable:
                     try:
                         value = reprlib.repr(
-                            namespace.imports_manager.resolve_variable(
+                            await namespace.imports_manager.resolve_variable(
                                 variable.name,
                                 str(document.uri.to_path().parent),
                                 await namespace.get_resolvable_variables(nodes, position),
                             )
                         )
                     except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
                         raise
@@ -160,15 +160,15 @@
                 None,
             )
             if token_and_var is not None:
                 var_token, variable = token_and_var
 
                 if variable.has_value or variable.resolvable:
                     try:
-                        value = namespace.imports_manager.resolve_variable(
+                        value = await namespace.imports_manager.resolve_variable(
                             variable.name,
                             str(document.uri.to_path().parent),
                             await namespace.get_resolvable_variables(nodes, position),
                         )
                     except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException:
@@ -209,15 +209,15 @@
                 None,
             )
             if token_and_var is not None:
                 var_token, variable = token_and_var
 
                 if variable.has_value or variable.resolvable:
                     try:
-                        value = namespace.imports_manager.resolve_variable(
+                        value = await namespace.imports_manager.resolve_variable(
                             variable.name,
                             str(document.uri.to_path().parent),
                             await namespace.get_resolvable_variables(nodes, position),
                         )
                     except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException:
```

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.39.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/.gitignore` & `robotcode_language_server-0.39.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/LICENSE.txt` & `robotcode_language_server-0.39.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/README.md` & `robotcode_language_server-0.39.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.38.0/pyproject.toml` & `robotcode_language_server-0.39.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,23 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.38.0"]
+dependencies = [
+  "robotframework>=4.1.0",
+  "robotcode-jsonrpc2==0.39.0",
+  "robotcode==0.39.0",
+]
 dynamic = ["version"]
 
-[project.scripts]
-'robotcode.language_server' = 'robotcode.language_server.__main__:main'
+[project.entry-points.robotcode]
+langserver = "robotcode.language_server.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/d-biehl/robotcode/issues"
```

### Comparing `robotcode_language_server-0.38.0/PKG-INFO` & `robotcode_language_server-0.39.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.38.0
+Version: 0.39.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.38.0
+Requires-Dist: robotcode-jsonrpc2==0.39.0
+Requires-Dist: robotcode==0.39.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

