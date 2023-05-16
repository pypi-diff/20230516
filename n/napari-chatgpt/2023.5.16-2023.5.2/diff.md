# Comparing `tmp/napari-chatgpt-2023.5.16.tar.gz` & `tmp/napari-chatgpt-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.5.16.tar", last modified: Tue May 16 16:57:06 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.5.2.tar", last modified: Wed May  3 00:41:13 2023, max compression
```

## Comparing `napari-chatgpt-2023.5.16.tar` & `napari-chatgpt-2023.5.2.tar`

### file list

```diff
@@ -1,219 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.706876 napari-chatgpt-2023.5.16/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.658875 napari-chatgpt-2023.5.16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.670876 napari-chatgpt-2023.5.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.674876 napari-chatgpt-2023.5.16/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-16 16:57:06.706876 napari-chatgpt-2023.5.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 16:57:06.706876 napari-chatgpt-2023.5.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.674876 napari-chatgpt-2023.5.16/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.674876 napari-chatgpt-2023.5.16/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/bard_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/gpt4all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/openai_list_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/callback_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/callback_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/prism.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.682876 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/llms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/llm/test/bard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.686876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/demo/tools_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/file_download_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/functions_info_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/google_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/human_input_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/async_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/napari_plugin_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/tool_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_file_open_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_viewer_control_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_viewer_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_widget_maker_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/cellpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/tests/google_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.690876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/async_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/async_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/async_utils/run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/gpt4all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/test/download_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/test/summarizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/open_in_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.694876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.698876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/missing_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/required_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.698876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/exception_guard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/inspection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/installed_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/required_imports_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.698876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/qt/download_file_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/qt/qt_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.702876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/python_code_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.702876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/extract_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/extract_url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.702876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/system/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.702876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/metasearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/scrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.706876 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/google_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/metasearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/scrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/test/wikipedia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:57:06.678876 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 16:57:06.000000 napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 16:56:45.000000 napari-chatgpt-2023.5.16/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.646624 napari-chatgpt-2023.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.650624 napari-chatgpt-2023.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.654624 napari-chatgpt-2023.5.2/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.658624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.662624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/file_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/functions_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/google_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/human_input_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/math_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_file_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_widget_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cellpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/google_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tool_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/browser_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/camel_case_to_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.666624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/api_key_vault_dialog_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/browser_widget_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/missing_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/open_in_napari.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/openai_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.678624 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/api_key_vault_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/download_files_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/duckduckgo_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/dynamic_import_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/exception_guard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_code_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_url_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/filter_lines_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/find_function_name_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/google_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/inspection_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/installed_packages_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/missing_imports_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/missing_libraries_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/run_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/scrapper_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/summarizer_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/wikipedia_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:41:13.654624 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20605 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 00:41:13.000000 napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-03 00:40:46.000000 napari-chatgpt-2023.5.2/tox.ini
```

### Comparing `napari-chatgpt-2023.5.16/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.5.2/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.5.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/.gitignore` & `napari-chatgpt-2023.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/.napari-hub/config.yml` & `napari-chatgpt-2023.5.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/.pre-commit-config.yaml` & `napari-chatgpt-2023.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/LICENSE` & `napari-chatgpt-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/PKG-INFO` & `napari-chatgpt-2023.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.5.16
+Version: 2023.5.2
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -23,16 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-chatgpt
-## Home of _Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
+# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
@@ -102,26 +101,18 @@
 
 - wikipedia search:
     Gives Omega access to the whole wikipedia
 
 
 ----------------------------------
 
-## Installation from within napari:
+## Installation:
 
-You can install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment).
-
-IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the latest one!
-
-
-## Installation in an new conda environment (RECOMMENDED):
-
-Make sure you have an anaocnda/miniconda installation on your system. 
-Ask ChatGPT what is that all about if you are unsure ;-)
+You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the corresponding environment)
 
 Create environment: 
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
@@ -188,15 +179,15 @@
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
 (The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
+You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
 and start having an hopefully nice chat with Omega.
 
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
@@ -354,15 +345,15 @@
 FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 ## Contributing
 
-Contributions are extremely welcome. Tests can be run with [tox], please ensure
+Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.16/README.md` & `napari-chatgpt-2023.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# napari-chatgpt
-## Home of _Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
+# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
@@ -73,26 +72,18 @@
 
 - wikipedia search:
     Gives Omega access to the whole wikipedia
 
 
 ----------------------------------
 
-## Installation from within napari:
+## Installation:
 
-You can install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment).
-
-IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the latest one!
-
-
-## Installation in an new conda environment (RECOMMENDED):
-
-Make sure you have an anaocnda/miniconda installation on your system. 
-Ask ChatGPT what is that all about if you are unsure ;-)
+You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the corresponding environment)
 
 Create environment: 
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
@@ -159,15 +150,15 @@
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
 (The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
+You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
 and start having an hopefully nice chat with Omega.
 
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
@@ -325,15 +316,15 @@
 FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 ## Contributing
 
-Contributions are extremely welcome. Tests can be run with [tox], please ensure
+Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.16/setup.cfg` & `napari-chatgpt-2023.5.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	scikit-image
 	qtpy
-	langchain==0.0.167
+	langchain==0.0.144
 	fastapi
 	uvicorn
 	websockets
 	openai
 	tiktoken
 	wikipedia
 	lxml
@@ -47,30 +47,26 @@
 	matplotlib
 	xarray
 	arbol
 	playwright
 	duckduckgo_search
 	ome-zarr
 	scikit-video
-	pygpt4all==1.1.0
-	GoogleBard==1.0.2
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 napari.manifest = 
 	napari-chatgpt = napari_chatgpt:napari.yaml
-omega.tools = 
-	example_tool = napari_chatgpt.omega.tools.examples.example_omega_tool:ExampleOmegaTool
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/callback_handle_chat.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handle_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from typing import Any, Dict, Union, List
 
 from arbol import aprint
 from langchain.callbacks.base import AsyncCallbackHandler
 from langchain.schema import AgentFinish, AgentAction, LLMResult
 
 from napari_chatgpt.chat_server.chat_response import ChatResponse
-from napari_chatgpt.utils.strings.camel_case_to_normal import \
-    camel_case_to_lower_case
+from napari_chatgpt.utils.camel_case_to_normal import camel_case_to_lower_case
 
 
 class ChatCallbackHandler(AsyncCallbackHandler):
     """Callback handler for chat responses."""
 
     def __init__(self, websocket):
         self.websocket = websocket
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/callback_handler_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/callback_handler_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, Union, List
 
 from arbol import aprint
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentFinish, AgentAction, LLMResult
 
 from napari_chatgpt.chat_server.chat_response import ChatResponse
-from napari_chatgpt.utils.async_utils.run_async import run_async
+from napari_chatgpt.utils.tests.run_async import run_async
 
 
 class ToolCallbackHandler(BaseCallbackHandler):
     """Callback handler for tool responses."""
 
     def __init__(self, websocket):
         self.websocket = websocket
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/chat_server.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/chat_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 from threading import Thread
 
 import napari
 from PyQt5.QtCore import QTimer
 from arbol import aprint
 from fastapi import FastAPI, Request, WebSocket, WebSocketDisconnect
 from fastapi.templating import Jinja2Templates
+from langchain.callbacks import AsyncCallbackManager
+from langchain.chat_models import ChatOpenAI
 from starlette.staticfiles import StaticFiles
 
 from napari_chatgpt.chat_server.callback_handle_chat import ChatCallbackHandler
 from napari_chatgpt.chat_server.callback_handler_tool import ToolCallbackHandler
 from napari_chatgpt.chat_server.chat_response import ChatResponse
-from napari_chatgpt.llm.llms import instantiate_LLMs
 from napari_chatgpt.omega.napari_bridge import NapariBridge
 from napari_chatgpt.omega.omega_init import initialize_omega_agent
-from napari_chatgpt.utils.api_keys.api_key import set_api_key
-from napari_chatgpt.utils.download.gpt4all import get_gpt4all_model
-from napari_chatgpt.utils.python.installed_packages import is_package_installed
+from napari_chatgpt.utils.openai_key import set_openai_key
 
 
 class NapariChatServer:
     def __init__(self,
-                 napari_bridge: NapariBridge,
-                 llm_model_name: str = 'gpt-3.5-turbo',
-                 temperature: float = 0.01,
-                 memory_type: str = 'standard',
-                 agent_personality: str = 'neutral',
+                 napari_bridge: NapariBridge
                  ):
 
         # Napari bridge:
         self.napari_bridge = napari_bridge
 
         # Instantiate FastAPI:
         self.app = FastAPI()
@@ -68,32 +63,50 @@
 
             # Chat callback handler:
             chat_callback_handler = ChatCallbackHandler(websocket)
 
             # Tool callback handler:
             tool_callback_handler = ToolCallbackHandler(websocket)
 
-            main_llm, memory_llm, tool_llm = instantiate_LLMs(
-                llm_model_name=llm_model_name,
-                temperature=temperature,
-                chat_callback_handler=chat_callback_handler)
+            # Instantiates OpenAI's LLM:
+            main_llm = ChatOpenAI(
+                model_name='gpt-3.5-turbo',
+                verbose=True,
+                streaming=True,
+                temperature=0.0,
+                callback_manager=AsyncCallbackManager([chat_callback_handler])
+            )
+
+            # Instantiates OpenAI's LLM:
+            tool_llm = ChatOpenAI(
+                model_name='gpt-3.5-turbo',
+                verbose=True,
+                streaming=True,
+                temperature=0.0,
+                # callback_manager=AsyncCallbackManager([tool_callback_handler])
+            )
+
+            memory_llm = ChatOpenAI(
+                model_name='gpt-3.5-turbo',
+                verbose=False,
+                temperature=0.01,
+                # callback_manager=AsyncCallbackManager([tool_callback_handler])
+            )
 
             # Agent
             agent_chain = initialize_omega_agent(
                 to_napari_queue=napari_bridge.to_napari_queue,
                 from_napari_queue=napari_bridge.from_napari_queue,
                 main_llm=main_llm,
                 tool_llm=tool_llm,
                 memory_llm=memory_llm,
                 is_async=True,
                 chat_callback_handler=chat_callback_handler,
                 tool_callback_handler=tool_callback_handler,
-                has_human_input_tool=False,
-                memory_type=memory_type,
-                agent_personality=agent_personality,
+                has_human_input_tool=False
             )
 
             # Dialog Loop:
             while True:
                 try:
                     # Receive and send back the client message
                     question = await websocket.receive_text()
@@ -130,70 +143,47 @@
                         message=f"Sorry, something went wrong ({type(e).__name__}: {e.args[0]}). Try again.",
                         type="error",
                     )
                     await websocket.send_json(resp.dict())
 
     def run(self):
         import uvicorn
-        uvicorn.run(self.app, host="127.0.0.1", port=9000)
+        uvicorn.run(self.app, host="0.0.0.0", port=9000)
 
 
-def start_chat_server(viewer: napari.Viewer = None,
-                      llm_model_name: str = 'gpt-3.5-turbo',
-                      temperature: float = 0.01,
-                      memory_type: str = 'standard',
-                      agent_personality: str = 'neutral'):
-    # Set OpenAI key if necessary:
-    if 'gpt' in llm_model_name and '4all' not in llm_model_name and is_package_installed(
-            'openai'):
-        set_api_key('OpenAI')
-
-    if 'bard' in llm_model_name:
-        set_api_key('GoogleBard')
-
-    # Set Anthropic key if necessary:
-    if 'claude' in llm_model_name and is_package_installed('anthropic'):
-        set_api_key('Anthropic')
-
-    # Download GPT4All model if necessary:
-    if 'ggml' in llm_model_name and is_package_installed('pygpt4all'):
-        # The first this is run it will download the file, afterwards
-        # it uses the downloaded file in ~/.gpt4all
-        get_gpt4all_model(llm_model_name)
+def start_chat_server(viewer: napari.Viewer = None):
+    # Set OpenAI key:
+    set_openai_key()
 
     # Instantiates napari viewer:
     if not viewer:
         viewer = napari.Viewer()
 
     # Instantiates a napari bridge:
     bridge = NapariBridge(viewer)
 
     # Instantiates server:
-    chat_server = NapariChatServer(bridge,
-                                   llm_model_name=llm_model_name,
-                                   temperature=temperature,
-                                   memory_type=memory_type,
-                                   agent_personality=agent_personality)
+    chat_server = NapariChatServer(bridge)
 
     # Define server thread code:
     def server_thread_function():
         # Start Chat server:
         chat_server.run()
 
     # Create and start the thread that will run Omega:s
     server_thread = Thread(target=server_thread_function, args=())
     server_thread.start()
 
     # function to open browser on page:
     def _open_browser():
-        url = "http://127.0.0.1:9000"
+        url = "http://0.0.0.0:9000"
         webbrowser.open(url, new=0, autoraise=True)
 
     # open browser after delay of a few seconds:
     QTimer.singleShot(2000, _open_browser)
 
+    # Start qt event loop and wait for it to stop:
+    napari.run()
+
 
 if __name__ == "__main__":
     start_chat_server()
-
-    # Start qt event loop and wait for it to stop:
-    napari.run()
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/chat_server/templates/index.html` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/chat_server/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     <link href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css"
           rel="stylesheet">
     <link href="static/prism.css" rel="stylesheet"/>
 
     <style>
         .chat-body {
             width: 90%;
-            height: 90%;
             margin: 50px auto;
         }
 
         .card-body {
             background-color: #333;
             color: #fff;
             border-radius: 10px;
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/memory/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type
 
-from langchain.base_language import BaseLanguageModel
 from langchain.chains.llm import LLMChain
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.memory.prompt import SUMMARY_PROMPT
 from langchain.prompts.base import BasePromptTemplate
 from langchain.schema import (
+    BaseLanguageModel,
     BaseMessage,
     SystemMessage,
     get_buffer_string,
 )
 from pydantic import BaseModel, root_validator
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import napari
 import napari.viewer
 from arbol import aprint, asection
 from napari import Viewer
 from napari.qt.threading import thread_worker
 
-from napari_chatgpt.utils.python.exception_guard import ExceptionGuard
+from napari_chatgpt.utils.exception_guard import ExceptionGuard
 
 
 class NapariBridge():
 
     def __init__(self, viewer: Viewer):
         self.viewer = viewer
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/agent.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,33 +22,30 @@
             words = re.split(r'(\s+)', cleaned_output)
 
             # Simple state machine to robustly parse output:
             action = ''
             input = ''
             state = 'start'
             for word in words:
-                normalised_word = word.strip().lower()
-                if 'action:' == normalised_word or '**action:**' == normalised_word:
+                normalised_line = word.strip().lower()
+                if 'action:' == normalised_line:
                     state = 'action'
                     continue
-                elif 'input:' == normalised_word or '**input:**' == normalised_word:
+                elif 'input:' == normalised_line:
                     state = 'input'
                     continue
 
                 if state == 'action':
                     action += word
                 elif state == 'input':
                     input += word
 
             action = action.strip()
             input = input.strip()
 
-            # Clean up the input, necessary for Bard:
-            input = input.split("FinalAnswer:")[0].strip()
-
             if action.lower() == "finalanswer":
                 return AgentFinish({"output": input}, text)
             else:
                 return AgentAction(action, input, text)
 
         except Exception as e:
             traceback.print_exc()
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/prompts.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,48 +13,40 @@
 image analysis, and computer vision. 
 Additionally, you are able to generate your own text based on the input received, 
 allowing you to engage in discussions and provide explanations, 
 and descriptions on a wide range of topics. 
 
 """
 
-PERSONALITY = {}
-
-PERSONALITY['neutral'] = ''
-PERSONALITY[
-    'prof'] = '\nYour personality and the style of your writting is that of a highly qualified University Professor. You are an expert that puts effort in understanding the user and explaining in details what you do and how you do it. \n'
-PERSONALITY[
-    'mobster'] = '\nYour personality and the style of your writting is that of a New York mobster. You do have a witty attitude when you answer but you genuinely want to help. You are nevertheless a strong an competent expert. \n'
-
 OMEGA_FORMAT_INSTRUCTIONS = """RESPONSE FORMAT INSTRUCTIONS
 ----------------------------
 
 When responding to me, please output a response in one of two formats:
 
 **Option 1:**
 Use this if you want the human to use a tool.
 Use the following schema:
 
-Action:\\ newline required here  
+Action: 
 string \\ The action to take. Must be one of {tool_names}
 
-Input: \\ newline required here
+Input: 
 string \\ The input to the action
 
 
 **Option #2:**
 Use this if you want to respond directly to me. 
 Particularly if you think you have succeeded in doing what I want, or answered the question,
 or if you are not sure what I asked from you.
 Use the following schema:
 
-Action:     \\ newline required here 
+Action:
 FinalAnswer \\ The final action
 
-Input: \\ newline required here
+Input:
 string \\ You should put what you want to return to the human here
 
 Notes: 
 - Please choose the FinalAnswer action if you have answered the question or performed the task, or if you have determined that you can't.
 - Input of tools must be in PLAIN TEXT ONLY, not in pseudo code!
 """
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/file_download_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/file_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from arbol import asection
 
-from napari_chatgpt.omega.tools.machinery.async_base_tool import AsyncBaseTool
-from napari_chatgpt.utils.download.download_files import download_files
-from napari_chatgpt.utils.strings.extract_urls import extract_urls
+from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
+from napari_chatgpt.utils.download_files import download_files
+from napari_chatgpt.utils.extract_urls import extract_urls
 
 
 class FileDownloadTool(AsyncBaseTool):
-    name = "UrlDownloadTool"
+    name = "UrlDownload"
     description = (
-        "Use this tool to download file(s) by writing: download(<url>) where <url> is a valid syntatically correct URL. "
+        "Use this tool to download file(s) by writing: download(<url>) where <url> is a valid syntatically corect url. "
         "The file(s) is(are) stored in the current folder using its(their) filename as found in the URL, "
         "and thus is(are) directly accessible using its(their) filename. "
         "Use this tool to download files before any subsequent operations.")
 
     def _run(self, query: str) -> str:
         """Use the tool."""
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/functions_info_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/functions_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A tool for running python code in a REPL."""
 import traceback
 
-from napari_chatgpt.omega.tools.machinery.async_base_tool import AsyncBaseTool
-from napari_chatgpt.utils.llm.summarizer import summarize
-from napari_chatgpt.utils.python.inspection import extract_package_path, \
+from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
+from napari_chatgpt.utils.inspection import extract_package_path, \
     get_function_info
+from napari_chatgpt.utils.summarizer import summarize
 
 
 class PythonFunctionsInfoTool(AsyncBaseTool):
     """A tool for querying the signature and docstrings of python functions."""
 
     name = "PythonFunctionsInfoTool"
     description = (
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/human_input_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/human_input_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Tool for asking human input."""
 
 from typing import Callable
 
 from pydantic import Field
 
-from napari_chatgpt.omega.tools.machinery.async_base_tool import AsyncBaseTool
+from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 
 
 def _print_func(text: str) -> None:
     print("\n")
     print(text)
 
 
 class HumanInputTool(AsyncBaseTool):
     """Tool that adds the capability to ask user for input."""
 
-    name = "HumanInputTool"
+    name = "Human"
     description = (
         "You can ask a human for guidance when you think you "
         "got stuck or you are not sure what to do next. "
         "The input should be a question for the human."
     )
     prompt_func: Callable[[str], None] = Field(
         default_factory=lambda: _print_func)
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/async_base_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/napari_base_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_base_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """A tool for running python code in a REPL."""
 import sys
 from queue import Queue
-from typing import Union
 
 from arbol import aprint
 from langchain import LLMChain, PromptTemplate
 from langchain.callbacks import StdOutCallbackHandler
-from langchain.chat_models.base import BaseChatModel
-from langchain.llms.base import LLM
+from langchain.chat_models import ChatOpenAI
 from napari import Viewer
 from pydantic import Field
 
-from napari_chatgpt.omega.tools.machinery.async_base_tool import AsyncBaseTool
-from napari_chatgpt.utils.python.installed_packages import \
-    installed_package_list
-from napari_chatgpt.utils.python.missing_libraries import required_libraries, \
+from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
+from napari_chatgpt.utils.extract_code import extract_code_from_markdown
+from napari_chatgpt.utils.filter_lines import filter_lines
+from napari_chatgpt.utils.installed_packages import installed_package_list
+from napari_chatgpt.utils.missing_libraries import required_libraries, \
     pip_install
-from napari_chatgpt.utils.python.required_imports import required_imports
-from napari_chatgpt.utils.strings.extract_code import extract_code_from_markdown
-from napari_chatgpt.utils.strings.filter_lines import filter_lines
 
 _generic_codegen_instructions = """
 PYTHON CODE INSTRUCTIONS:
 - The code should be fully functional and not depend on any missing code, data or computation.
 - Use any functions from the standard python {python_version} library, 
 - Use any functions from installed libraries from this list: "{packages}" -- write your code against the installed version of these libraries. 
 - ONLY USE parameters or arguments of functions that you are certain exist in the corresponding package or library version!
@@ -43,31 +39,31 @@
         "Here"
     )
     code_prefix: str = ''
     generic_codegen_instructions: str = _generic_codegen_instructions
     prompt: str = None
     to_napari_queue: Queue = Field(default=None)
     from_napari_queue: Queue = Field(default=None)
-    llm: Union[BaseChatModel, LLM] = Field(default=None)
+    llm: ChatOpenAI = Field(default=None)
     return_direct = False
 
     def _run(self, query: str) -> str:
         """Use the tool."""
 
         if self.prompt:
             # Instantiate chain:
             chain = LLMChain(
-                prompt=self._get_prompt_template(),
+                prompt=self.get_prompt_template(),
                 llm=self.llm,
                 verbose=True,
-                callbacks=self.callbacks
+                callback_manager=self.callback_manager
             )
 
             # chain.callback_manager.add_handler(ToolCallbackHandler(type(self).__name__))
-            chain.callbacks.add_handler(StdOutCallbackHandler())
+            chain.callback_manager.add_handler(StdOutCallbackHandler())
 
             # List of installed packages:
             package_list = installed_package_list()
 
             generic_codegen_instructions = self.generic_codegen_instructions.format(
                 python_version=str(sys.version.split()[0]),
                 packages=', '.join(package_list))
@@ -105,15 +101,19 @@
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
         """
         This is the code that is executed, see implementations for details,
         must return 'Success: ...' if things went well, otherwise it is failure!
         """
         raise NotImplementedError("This method must be implemented")
 
-    def _get_prompt_template(self):
+    # async def _arun(self, query: str) -> str:
+    #     """Use the tool asynchronously."""
+    #     raise NotImplementedError(f"{type(self).__name__} does not support async")
+
+    def get_prompt_template(self):
 
         prompt_template = PromptTemplate(template=self.prompt,
                                          input_variables=["input",
                                                           "generic_codegen_instructions"])
 
         return prompt_template
 
@@ -128,20 +128,14 @@
 
         # Remove any viewer instantiation code:
         code = filter_lines(code, ['napari.Viewer(', '= Viewer(', 'gui_qt('])
 
         # Add spaces around code:
         code = '\n\n' + code + '\n\n'
 
-        # Are there any missing imports?
-        imports = required_imports(code, llm=self.llm)
-
-        # prepend missing imports:
-        code = '\n'.join(imports) + '\n\n' + code
-
         # Are there missing libraries that need to be installed?
-        libraries = required_libraries(code, llm=self.llm)
+        libraries = required_libraries(code)
 
         # Install them:
         pip_install(libraries)
 
         return code
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/machinery/tool_callback_handler.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/tool_callback_handler.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_file_open_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_file_open.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """A tool for opening ome-zarr files in napari"""
 
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.machinery.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.napari.open_in_napari import open_in_napari
+from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.open_in_napari import open_in_napari
 
 
 class NapariFileOpenTool(NapariBaseTool):
     """A tool for running python code in a REPL."""
 
-    name = "NapariFileOpenTool"
+    name = "NapariFileOpen"
     description = (
         "Forward plain text requests to this tool when you need to open image files in napari. "
         "Requests must be a newline (\\n) delimited list of local file paths or URLs to be opened. "
         "This tool can open image files with these extensions: .tif, .png, .jpg, .zarr, and more..."
 
     )
     prompt: str = None
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_viewer_control_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A tool for controlling a napari instance."""
 from contextlib import redirect_stdout
 from io import StringIO
 
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.machinery.napari_base_tool import NapariBaseTool
+from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
 
 _napari_viewer_control_prompt = """
 "
 Task:
 Given a plain text request, you competently write python code to control an already instantiated napari viewer instance.
 The napari viewer instance is immediately available by using the variable: 'viewer'. 
 For example, you can directly write: viewer.add_image(np.zeros((10,10))) without preamble.
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_viewer_query_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_viewer_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A tool for controlling a napari instance."""
 
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.machinery.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.python.dynamic_import import dynamic_import
+from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.dynamic_import import dynamic_import
 
 _napari_viewer_query_prompt = """
 "
 Task:
 Given a plain text request, you competently write python code to query an already instantiated napari viewer instance.
 
 You can, for example:
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/napari_widget_maker_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/napari_widget_maker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A tool for making a napari widget."""
 
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.machinery.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.python.dynamic_import import dynamic_import
-from napari_chatgpt.utils.strings.filter_lines import filter_lines
-from napari_chatgpt.utils.strings.find_function_name import find_function_name
+from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.dynamic_import import dynamic_import
+from napari_chatgpt.utils.filter_lines import filter_lines
+from napari_chatgpt.utils.find_function_name import find_function_name
 
 _napari_widget_maker_prompt = """
 Task:
 You competently write image processing and image analysis functions in python given a plain text request. 
 The function should be pure, self-contained, effective, well-written, syntactically correct.
 The function should work on 2D and 3D images, and images of any number of dimensions (nD), 
 unless the request is explicit about the number of dimensions. 
@@ -22,18 +22,17 @@
 - DO NOT clip (np.clip) the resulting image.
 
 Instructions for manipulating arrays from Labels layers:
 - DO NOT convert to float arrays originating from labels layers, instead cast to np.uint32.
 
 Instructions for Function Signature:
 - Integers, floats, boolean, or any other type accepted by the magicgui library.
-- Decorate the function with the magicgui decorator: '@magicgui(call_button='Run')'.
+- Decorate the function with the magicgui decorator: '@magicgui(call_button='Run')' where <function_name> is the name of the function that you wrote.
 - DO NOT CREATE A NEW INSTANCE OF A NAPARI VIEWER, use the one provided in the variable: 'viewer'.
 - DO NOT write code to add the widget to the napari window by calling viewer.window.add_dock_widget().
-- DO NOT add layers to the viewer within the function, instead use a return statement to return the result.
 
 You have two mutually exclusive options for passing data:
 
     (i) The first kind of function signature must be typed with any of the following type hints:
     napari layer data types: ImageData, LabelsData, PointsData, ShapesData, 
     SurfaceData, TracksData, VectorsData. These types must be imported with import 
     statements such as: 'from napari.types import ImageData'
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cell_nuclei_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A tool for controlling a napari instance."""
 from pathlib import Path
 
 from napari import Viewer
 
-from napari_chatgpt.omega.tools.machinery.napari_base_tool import NapariBaseTool
-from napari_chatgpt.utils.python.dynamic_import import dynamic_import
+from napari_chatgpt.omega.tools.napari_base_tool import NapariBaseTool
+from napari_chatgpt.utils.dynamic_import import dynamic_import
 
 _cell_segmentation_prompt = """
 "
 Task:
 Given a plain text request, you competently write a python function segment(viewer) that calls the cellpose_segmentation() function.
 Segmentation is performed on images present as layers of the instantiated napari viewer.
 The napari viewer instance is immediately available by using the variable: 'viewer'.
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/segmentation/cellpose.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/segmentation/cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/omega/tools/wikipedia_query_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from langchain import WikipediaAPIWrapper
 
-from napari_chatgpt.omega.tools.machinery.async_base_tool import AsyncBaseTool
+from napari_chatgpt.omega.tools.async_base_tool import AsyncBaseTool
 
 _api_wrapper = WikipediaAPIWrapper()
 
 
 class WikipediaQueryTool(AsyncBaseTool):
     """Tool that adds the capability to search using the Wikipedia API."""
 
-    name = "WikipediaQueryTool"
+    name = "Wikipedia"
     description = (
-        "Useful for when you need to answer general questions on topics covered by an encyclopedia such as historical events, scientific concepts, geography, etc... "
+        "A wrapper around Wikipedia. "
+        "Useful for when you need to answer general questions on topics covered by an encyclopedia. "
         "Input should be a search query."
     )
 
     def _run(self, query: str) -> str:
         """Use the Wikipedia tool."""
         return _api_wrapper.run(query)
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/api_key_vault_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PyQt5.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton
 from arbol import aprint
+from cryptography.fernet import InvalidToken
 
-from napari_chatgpt.utils.api_keys.api_key_vault import KeyVault
+from napari_chatgpt.utils.api_key_vault import KeyVault
 
 
 class APIKeyDialog(QDialog):
     def __init__(self, api_key_name: str, parent=None):
         super().__init__(parent)
 
         self.api_key = None
@@ -51,15 +52,14 @@
 
         # Connect the button to a slot
         self.button.clicked.connect(self.button_clicked)
 
     def button_clicked(self):
 
         if self.key_vault.is_key_present():
-            from cryptography.fernet import InvalidToken
             try:
                 password = self.password_textbox.text()
 
                 # Decrypt API key:
                 self.api_key = self.key_vault.read_api_key(password=password)
 
                 # Close the dialog box
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/api_key_vault_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from napari_chatgpt.utils.api_keys.api_key_vault import KeyVault, _encode64, \
-    _decode64
+from napari_chatgpt.utils.api_key_vault import KeyVault, _encode64, _decode64
 
 
 def test_b64_encode_decode():
     plain = '1234'
     encoded = _encode64(plain)
     decoded = _decode64(encoded)
     assert plain == decoded
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/demo/api_key_vault_dialog_demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from PyQt5.QtWidgets import QApplication, QMainWindow, QPushButton
 
-from napari_chatgpt.utils.api_keys.api_key_vault_dialog import \
+from napari_chatgpt.utils.api_key_vault_dialog import \
     request_if_needed_api_key_dialog
 
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/download_files.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/download/test/download_files_test.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/download_files_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tempfile
 
 from arbol import aprint
 
-from napari_chatgpt.utils.download.download_files import download_files
-from napari_chatgpt.utils.strings.extract_urls import extract_urls
+from src.napari_chatgpt.utils.download_files import download_files
+from src.napari_chatgpt.utils.extract_urls import extract_urls
 
 
 def test_download_files():
     # Example string with urls:
     text = "Check out my website at https://www.example.com! " \
            "For more information, visit http://en.wikipedia.org/wiki/URL."
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/llm/summarizer.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/summarizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from langchain.chains.summarize import load_summarize_chain
 from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.llms import BaseLLM
 from langchain.text_splitter import CharacterTextSplitter
 
+from napari_chatgpt.utils.openai_key import set_openai_key
 
-def summarize(text: str, llm: BaseLLM = None):
-    # Clean up text:
-    text = text.strip()
 
-    # Is there anything to summarise?
-    if len(text) == 0:
-        return text
+def summarize(text: str, llm: BaseLLM = None):
+    # Ensure that OpenAI key is set:
+    set_openai_key()
 
     # Instantiates LLM if needed:
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Splits the text:
     text_splitter = CharacterTextSplitter()
     texts = text_splitter.split_text(text)
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/napari/open_in_napari.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/open_in_napari.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 'mov') or url.endswith('avi') or url.endswith('m4v')):
             return False
 
         # temp folder:
         temp_folder = tempfile.gettempdir()
 
         # Download video file:
-        from napari_chatgpt.utils.download.download_files import download_files
+        from napari_chatgpt.utils.download_files import download_files
         files = download_files(urls=[url], path=temp_folder)
         file = files[0]
 
         # make full path:
         file_path = os.path.join(temp_folder, file)
 
         # open video:
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/dynamic_import.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/exception_guard.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/exception_guard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/inspection.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/installed_packages.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/installed_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,13 +65,7 @@
                             not line.startswith('#')]
 
         return package_list
 
     except Exception as e:
         print(traceback.format_exc())
         return []
-
-
-def is_package_installed(package_name: str):
-    from pkgutil import find_loader
-    loader = find_loader(package_name)
-    return loader is not None
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/missing_libraries.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/missing_libraries.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import traceback
 from functools import cache
 from subprocess import CalledProcessError
 from typing import List
 
 from arbol import aprint, asection
 from langchain import LLMChain, PromptTemplate
-from langchain.callbacks import StdOutCallbackHandler
-from langchain.callbacks.manager import CallbackManager
+from langchain.callbacks import StdOutCallbackHandler, CallbackManager
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import BaseLLM
 
-from napari_chatgpt.utils.python.installed_packages import is_package_installed
+from napari_chatgpt.utils.openai_key import set_openai_key
 
 _pip_install_missing_prompt = f"""
 Task:
 You competently write the 'pip install <list_of_packages>' command required to run the following python {sys.version.split()[0]} code:
 
 CODE:
 #______________
@@ -34,14 +33,17 @@
     # Cleanup code:
     code = code.strip()
 
     # If code is empty, nothing is missing!
     if len(code) == 0:
         return []
 
+    # Ensure that OpenAI key is set:
+    set_openai_key()
+
     # Instantiates LLM if needed:
     llm = llm or ChatOpenAI(model_name='gpt-3.5-turbo', temperature=0)
 
     # Make prompt template:
     prompt_template = PromptTemplate(template=_pip_install_missing_prompt,
                                      input_variables=["input"])
 
@@ -69,16 +71,15 @@
     if ignore_obvious:
         packages = [p for p in packages if
                     not p in ['numpy', 'napari', 'magicgui', 'scikit-image']]
 
     try:
         with asection(f"Installing {len(packages)} packages with pip:"):
             for package in packages:
-                if not is_package_installed(package):
-                    _pip_install_single_package(package)
+                _pip_install_single_package(package)
         return True
     except CalledProcessError:
         aprint(traceback.format_exc())
         return False
 
 
 @cache
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/python/test/missing_libraries_test.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/missing_libraries_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
-from napari_chatgpt.utils.api_keys.api_key import is_api_key_available
-from napari_chatgpt.utils.python.missing_libraries import required_libraries
+from napari_chatgpt.utils.missing_libraries import required_libraries, \
+    pip_install
+from napari_chatgpt.utils.openai_key import is_openai_key_available
 
 generated_python_code = """
 
 from magicgui import magicgui
 from napari.types import ImageData, LabelsData, PointsData, ShapesData, SurfaceData, TracksData, VectorsData
 import numpy as np
 from typing import Union
@@ -18,18 +19,14 @@
 def denoise_bilateral(image: ImageData, d: int = 15, sigmaColor: float = 75, sigmaSpace: float = 75) -> ImageData:
     img = image.astype(np.float32)
     img = cv2.bilateralFilter(img, d, sigmaColor, sigmaSpace)
     return img
 
 """
 
-
-@pytest.mark.skipif(not is_api_key_available('OpenAI'),
-                    reason="requires OpenAI key to run")
-def test_missing_libraries():
+@pytest.mark.skipif(not is_openai_key_available(), reason="requires OpenAI key to run")
+def test_pip_install_missing():
     libraries = required_libraries(generated_python_code)
     print(libraries)
     assert libraries
-    assert 'magicgui' in libraries
-    assert 'napari' in libraries
-    assert 'numpy' in libraries
-    assert 'opencv-python-headless' in libraries
+
+    pip_install(libraries)
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/camel_case_to_normal.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/extract_urls.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/filter_lines.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/extract_code_test.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/extract_code_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from napari_chatgpt.utils.strings.extract_code import extract_code_from_markdown
+from napari_chatgpt.utils.extract_code import extract_code_from_markdown
 
 markdown = """
 ```python
 # some python code
 from napari_chatgpt.utils.extract_code import extract_code_from_markdown
 
 def filter_lines(text:str, filter_out: List[str]=None) -> str:
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/strings/test/filter_lines_test.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/tests/filter_lines_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from napari_chatgpt.utils.strings.filter_lines import filter_lines
+from napari_chatgpt.utils.filter_lines import filter_lines
 
 ___text = """
 from magicgui import magicgui
 from typing import Union
 from napari.types import ImageData
 from magicgui import magicgui
 import numpy as np
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/duckduckgo.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/duckduckgo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 import traceback
 
 from duckduckgo_search import ddg, ddg_images
 
-from napari_chatgpt.utils.llm.summarizer import summarize
+from napari_chatgpt.utils.summarizer import summarize
 
 
 def summary_ddg(query: str,
                 num_results: int = 3,
-                lang: str = "en",
+                lang: str = "us-en",
                 do_summarize: bool = True,
                 ) -> str:
     try:
-
         results = search_ddg(query=query,
                              num_results=num_results,
                              lang=lang)
 
-        # Are there any results?
-        if len(results) == 0:
-            return "No results."
-
         text = f"The following results were found for the web search query: '{query}'"
 
         for result in results:
             text += f"Title: {result['title']}\n Description: {result['body']}\n URL: {result['href']}\n\n "
 
+        text += "How do the results inform the query ?"
+
         if do_summarize:
-            # summary prompt:
-            text += "Please summarise these results and list facts and information that help answer the query:"
             text = summarize(text)
 
         return text
 
     except Exception as e:
         traceback.format_exc()
         return f"Web search failed for: '{query}'"
 
 
 def search_ddg(query: str,
                num_results: int = 3,
-               lang: str = "en",
+               lang: str = "us-en",
                safesearch: str = 'moderate'
                ) -> str:
-    lang = 'en-us' if lang == 'en' else lang
-
     results = ddg(query,
                   region=lang,
                   time='h_',
                   safesearch=safesearch,
                   max_results=num_results)
 
     if results:
@@ -56,19 +49,17 @@
         results = []
 
     return results
 
 
 def search_images_ddg(query: str,
                       num_results: int = 3,
-                      lang: str = "en",
+                      lang: str = "us-en",
                       safesearch: str = 'moderate'
                       ) -> str:
-    lang = 'en-us' if lang == 'en' else lang
-
     results = ddg_images(query,
                          region=lang,
                          safesearch=safesearch,
                          size=None,
                          color=None,
                          type_image=None,
                          layout=None,
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/google.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Code vendored from: https://github.com/Nv7-GitHub/googlesearch/blob/master/googlesearch/__init__.py
 
 import random
 
-from napari_chatgpt.utils.web.headers import _scrapping_request_headers
-from napari_chatgpt.utils.web.scrapper import text_from_url
+from napari_chatgpt.utils.headers import _scrapping_request_headers
+from napari_chatgpt.utils.scrapper import text_from_url
 
 _useragent_list = [
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0) Gecko/20100101 Firefox/66.0',
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
     'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
@@ -55,15 +55,15 @@
         return f"SearchResult(url={self.url}, title={self.title}, description={self.description})"
 
 
 def search_overview(query: str,
                     num_results: int = 3,
                     lang: str = "en",
                     max_text_snippets: int = 5,
-                    max_query_freq_hz: float = 0.5) -> str:
+                    max_query_freq_hz: float = 1.0) -> str:
     url = f"https://www.google.com/search?q={query}&num={num_results}&hl={lang}"
     text = text_from_url(url,
                          max_text_snippets=max_text_snippets,
                          max_query_freq_hz=max_query_freq_hz)
     return text
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/headers.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/scrapper.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/scrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from typing import Optional
 
 from bs4 import BeautifulSoup
 from bs4.element import Comment
 from requests import Session
 
-from napari_chatgpt.utils.web.headers import _scrapping_request_headers
+from napari_chatgpt.utils.headers import _scrapping_request_headers
 
 
 def _tag_visible(element):
     if element.parent.name in ['style', 'script', 'head', 'title', 'meta',
                                '[document]']:
         return False
     if isinstance(element, Comment):
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt/utils/web/wikipedia.py` & `napari-chatgpt-2023.5.2/src/napari_chatgpt/utils/wikipedia.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Code vendored from: https://github.com/Nv7-GitHub/googlesearch/blob/master/googlesearch/__init__.py
 from langchain.llms import BaseLLM
 
-from napari_chatgpt.utils.llm.summarizer import summarize
-from napari_chatgpt.utils.web.duckduckgo import search_ddg
+from napari_chatgpt.utils.duckduckgo import search_ddg
+from napari_chatgpt.utils.summarizer import summarize
 
 
 def search_wikipedia(query: str,
                      num_results: int = 3,
                      max_text_length: int = 4000,
                      do_summarize: bool = False,
                      llm: BaseLLM = None) -> str:
```

### Comparing `napari-chatgpt-2023.5.16/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.5.2/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.5.16
+Version: 2023.5.2
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -23,16 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# napari-chatgpt
-## Home of _Omega_, a napari-aware autonomous LLM-based agent specialised in image processing and analysis.
+# napari-chatgpt, home of _Omega_, a napari-aware autonomous LLM-based agent.
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-chatgpt.svg?color=green)](https://github.com/royerlab/napari-chatgpt/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-chatgpt.svg?color=green)](https://pypi.org/project/napari-chatgpt)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-chatgpt.svg?color=green)](https://python.org)
 [![tests](https://github.com/royerlab/napari-chatgpt/workflows/tests/badge.svg)](https://github.com/royerlab/napari-chatgpt/actions)
 [![codecov](https://codecov.io/gh/royerlab/napari-chatgpt/branch/main/graph/badge.svg)](https://codecov.io/gh/royerlab/napari-chatgpt)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-chatgpt)](https://napari-hub.org/plugins/napari-chatgpt)
@@ -102,26 +101,18 @@
 
 - wikipedia search:
     Gives Omega access to the whole wikipedia
 
 
 ----------------------------------
 
-## Installation from within napari:
+## Installation:
 
-You can install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
-(Please note that the Omega agent will hapilly install packages in the corresponding environment).
-
-IMPORTANT NOTE: Makre sure you have a recent version of napari! Ideally the latest one!
-
-
-## Installation in an new conda environment (RECOMMENDED):
-
-Make sure you have an anaocnda/miniconda installation on your system. 
-Ask ChatGPT what is that all about if you are unsure ;-)
+You can also install `napari-chatgpt` directly from within napari in the Plugins>Install/Uninstall Plugins menu.
+(Please note that the Omega agent will hapilly install packages in the corresponding environment)
 
 Create environment: 
 
     conda create -y -n napari-chatgpt -c conda-forge python=3.9
 
 Activate environment:
 
@@ -188,15 +179,15 @@
 Just enter an encryption/decription key, your OpenAI key, and
 everytime you start Omega it will just ask for the decryption key:
 
 <img width="300" alt="image" src="https://user-images.githubusercontent.com/1870994/235794262-4c0eff4d-1c81-47b0-a097-f34e3d5c93b8.png">
 
 (The idea is that you might not be able to remember your openAI key by heart, but you might be able to do so with your own password or passphrase)
 
-You can then direct your browser to: [http://127.0.0.1:9000/](http://127.0.0.1:9000/)
+You can then direct your browser to: [http://0.0.0.0:9000/](http://0.0.0.0:9000/)
 and start having an hopefully nice chat with Omega.
 
 
 ## Example prompts:
 
 Here are example prompts/questions/requests to try:
 
@@ -354,15 +345,15 @@
 FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, 
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE 
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 ## Contributing
 
-Contributions are extremely welcome. Tests can be run with [tox], please ensure
+Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-chatgpt" is free and open source software
```

### Comparing `napari-chatgpt-2023.5.16/tox.ini` & `napari-chatgpt-2023.5.2/tox.ini`

 * *Files identical despite different names*

