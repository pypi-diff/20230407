# Comparing `tmp/robotcode_language_server-0.32.2.tar.gz` & `tmp/robotcode_language_server-0.32.3.tar.gz`

## Comparing `robotcode_language_server-0.32.2.tar` & `robotcode_language_server-0.32.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/lsp_types.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18305 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63852 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83660 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80204 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    39775 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/README.md
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/pyproject.toml
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/lsp_types.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18305 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63852 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83660 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80204 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/discovering.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    39775 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/README.md
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/pyproject.toml
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/PKG-INFO
```

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/lsp_types.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/lsp_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/discovering.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/discovering.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,97 +91,82 @@
     async def format_robot_tidy(
         self,
         document: TextDocument,
         options: FormattingOptions,
         range: Optional[Range] = None,
         **further_options: Any,
     ) -> Optional[List[TextEdit]]:
-        from difflib import SequenceMatcher
-
         from robotidy.version import __version__
 
         try:
             robotidy_version = create_version_from_str(__version__)
 
             model = await self.parent.documents_cache.get_model(document, False)
 
             if robotidy_version >= (3, 0):
                 from robotidy.api import get_robotidy
                 from robotidy.disablers import RegisterDisablers
 
                 robot_tidy = get_robotidy(document.uri.to_path(), None)
 
                 if range is not None:
-                    robot_tidy.config.formatting.start_line = range.start.line
+                    robot_tidy.config.formatting.start_line = range.start.line + 1
                     robot_tidy.config.formatting.end_line = range.end.line + 1
 
                 disabler_finder = RegisterDisablers(
                     robot_tidy.config.formatting.start_line,
                     robot_tidy.config.formatting.end_line,
                 )
                 disabler_finder.visit(model)
                 if disabler_finder.file_disabled:
                     return None
-                changed, _, new = robot_tidy.transform(model, disabler_finder.disablers)
+
+                if robotidy_version >= (4, 0):
+                    _, _, new, _ = robot_tidy.transform_until_stable(model, disabler_finder)
+                else:
+                    _, _, new = robot_tidy.transform(model, disabler_finder.disablers)
 
             else:
                 from robotidy.api import RobotidyAPI
 
                 robot_tidy = RobotidyAPI(document.uri.to_path(), None)
 
                 if range is not None:
-                    robot_tidy.formatting_config.start_line = range.start.line
+                    robot_tidy.formatting_config.start_line = range.start.line + 1
                     robot_tidy.formatting_config.end_line = range.end.line + 1
 
                 if robotidy_version >= (2, 2):
                     from robotidy.disablers import RegisterDisablers
 
                     disabler_finder = RegisterDisablers(
                         robot_tidy.formatting_config.start_line,
                         robot_tidy.formatting_config.end_line,
                     )
                     disabler_finder.visit(model)
                     if disabler_finder.file_disabled:
                         return None
-                    changed, _, new = robot_tidy.transform(model, disabler_finder.disablers)
+                    _, _, new = robot_tidy.transform(model, disabler_finder.disablers)
                 else:
-                    changed, _, new = robot_tidy.transform(model)
+                    _, _, new = robot_tidy.transform(model)
 
-            if not changed:
+            if new.text == document.text():
                 return None
 
-            new_lines = self.RE_LINEBREAKS.split(new.text)
-
-            result: List[TextEdit] = []
-            matcher = SequenceMatcher(a=document.get_lines(), b=new_lines, autojunk=False)
-            for code, old_start, old_end, new_start, new_end in matcher.get_opcodes():
-                if code == "insert" or code == "replace":
-                    result.append(
-                        TextEdit(
-                            range=Range(
-                                start=Position(line=old_start, character=0),
-                                end=Position(line=old_end, character=0),
-                            ),
-                            new_text=os.linesep.join(new_lines[new_start:new_end]) + os.linesep,
-                        )
-                    )
-
-                elif code == "delete":
-                    result.append(
-                        TextEdit(
-                            range=Range(
-                                start=Position(line=old_start, character=0),
-                                end=Position(line=old_end, character=0),
-                            ),
-                            new_text="",
-                        )
-                    )
-
-            if result:
-                return result
+            return [
+                TextEdit(
+                    range=Range(
+                        start=Position(line=0, character=0),
+                        end=Position(
+                            line=len(document.get_lines()),
+                            character=len((document.get_lines())[-1]),
+                        ),
+                    ),
+                    new_text=new.text,
+                )
+            ]
 
         except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
             raise
         except BaseException as e:
             self._logger.exception(e)
         return None
```

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/.gitignore` & `robotcode_language_server-0.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/LICENSE.txt` & `robotcode_language_server-0.32.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/README.md` & `robotcode_language_server-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/pyproject.toml` & `robotcode_language_server-0.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.2/PKG-INFO` & `robotcode_language_server-0.32.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.32.2
+Version: 0.32.3
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

