# Comparing `tmp/bambooai-0.2.1.tar.gz` & `tmp/bambooai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.2.1.tar", last modified: Sun May 14 11:31:30 2023, max compression
+gzip compressed data, was "bambooai-0.2.2.tar", last modified: Tue May 16 08:49:14 2023, max compression
```

## Comparing `bambooai-0.2.1.tar` & `bambooai-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:31:30.959430 bambooai-0.2.1/
--rw-rw-rw-   0        0        0     5719 2023-05-14 11:31:30.958430 bambooai-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5221 2023-05-10 12:51:46.000000 bambooai-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 11:31:30.924428 bambooai-0.2.1/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.2.1/bambooai/__init__.py
--rw-rw-rw-   0        0        0    12847 2023-05-14 11:14:43.000000 bambooai-0.2.1/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:31:30.957428 bambooai-0.2.1/bambooai.egg-info/
--rw-rw-rw-   0        0        0     5719 2023-05-14 11:31:30.000000 bambooai-0.2.1/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-14 11:31:30.000000 bambooai-0.2.1/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:31:30.000000 bambooai-0.2.1/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-14 11:31:30.000000 bambooai-0.2.1/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 11:31:30.000000 bambooai-0.2.1/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 11:31:30.959430 bambooai-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-14 11:27:46.000000 bambooai-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:49:14.629097 bambooai-0.2.2/
+-rw-rw-rw-   0        0        0     6317 2023-05-16 08:49:14.628207 bambooai-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5783 2023-05-14 12:03:23.000000 bambooai-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:49:14.580350 bambooai-0.2.2/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.2.2/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    14222 2023-05-16 08:41:27.000000 bambooai-0.2.2/bambooai/bambooai.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:49:14.626233 bambooai-0.2.2/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     6317 2023-05-16 08:49:14.000000 bambooai-0.2.2/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-16 08:49:14.000000 bambooai-0.2.2/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:49:14.000000 bambooai-0.2.2/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-16 08:49:14.000000 bambooai-0.2.2/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 08:49:14.000000 bambooai-0.2.2/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:49:14.629467 bambooai-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-05-16 08:45:50.000000 bambooai-0.2.2/setup.py
```

### Comparing `bambooai-0.2.1/PKG-INFO` & `bambooai-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.2.1
+Version: 0.2.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
+Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -21,40 +22,56 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
     - Obtains a response with corresponding Python code
     - Executes the code to generate an answer or visualization
       - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code.
+      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
   - The loop continues until the user enters 'exit', at which point the program terminates
   - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
   
+**Flow chart:**
+
+![](images/flow_chart.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
 
 **Usage**
 
+Args
+
+```
+bamboo = BambooAI(df,max_conversations=3,llm='gpt-3.5-turbo,llm_switch=False)
+
+df: pd.DataFrame - Dataframe
+max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context
+llm: str - Base LLM model
+llm_switch: bool - If True the agent will switch to gpt-4 after error
+```
+
 Run in a loop
+
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
 from bambooai import BambooAI
 
 df = pd.read_csv('test_activity_data.csv')
 bamboo = BambooAI(df)
```

### Comparing `bambooai-0.2.1/README.md` & `bambooai-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,40 +9,56 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
     - Obtains a response with corresponding Python code
     - Executes the code to generate an answer or visualization
       - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code.
+      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
   - The loop continues until the user enters 'exit', at which point the program terminates
   - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
   
+**Flow chart:**
+
+![](images/flow_chart.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
 
 **Usage**
 
+Args
+
+```
+bamboo = BambooAI(df,max_conversations=3,llm='gpt-3.5-turbo,llm_switch=False)
+
+df: pd.DataFrame - Dataframe
+max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context
+llm: str - Base LLM model
+llm_switch: bool - If True the agent will switch to gpt-4 after error
+```
+
 Run in a loop
+
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
 from bambooai import BambooAI
 
 df = pd.read_csv('test_activity_data.csv')
 bamboo = BambooAI(df)
```

### Comparing `bambooai-0.2.1/bambooai/bambooai.py` & `bambooai-0.2.2/bambooai/bambooai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,803 +1,889 @@
 00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
 00000010: 6f72 7420 7265 0d0a 696d 706f 7274 2073  ort re..import s
-00000020: 7973 0d0a 6672 6f6d 2063 6f6e 7465 7874  ys..from context
-00000030: 6c69 6220 696d 706f 7274 2072 6564 6972  lib import redir
-00000040: 6563 745f 7374 646f 7574 0d0a 696d 706f  ect_stdout..impo
-00000050: 7274 2069 6f0d 0a69 6d70 6f72 7420 7469  rt io..import ti
-00000060: 6d65 0d0a 696d 706f 7274 206f 7065 6e61  me..import opena
-00000070: 690d 0a69 6d70 6f72 7420 7061 6e64 6173  i..import pandas
-00000080: 2061 7320 7064 0d0a 6672 6f6d 2074 6572   as pd..from ter
-00000090: 6d63 6f6c 6f72 2069 6d70 6f72 7420 636f  mcolor import co
-000000a0: 6c6f 7265 642c 2063 7072 696e 740d 0a66  lored, cprint..f
-000000b0: 726f 6d20 4950 7974 686f 6e2e 6469 7370  rom IPython.disp
-000000c0: 6c61 7920 696d 706f 7274 2064 6973 706c  lay import displ
-000000d0: 6179 2c20 4854 4d4c 0d0a 0d0a 636c 6173  ay, HTML....clas
-000000e0: 7320 4261 6d62 6f6f 4149 3a0d 0a20 2020  s BambooAI:..   
-000000f0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000100: 6c66 2c20 6466 3a20 7064 2e44 6174 6146  lf, df: pd.DataF
-00000110: 7261 6d65 2c6d 6178 5f63 6f6e 7665 7273  rame,max_convers
-00000120: 6174 696f 6e73 3a20 696e 7420 3d20 3320  ations: int = 3 
-00000130: 2c6c 6c6d 3a20 7374 7220 3d20 2767 7074  ,llm: str = 'gpt
-00000140: 2d33 2e35 2d74 7572 626f 272c 6c6c 6d5f  -3.5-turbo',llm_
-00000150: 7377 6974 6368 3a20 626f 6f6c 203d 2046  switch: bool = F
-00000160: 616c 7365 293a 0d0a 0d0a 2020 2020 2020  alse):....      
-00000170: 2020 7365 6c66 2e41 5049 5f4b 4559 203d    self.API_KEY =
-00000180: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
-00000190: 274f 5045 4e41 495f 4150 495f 4b45 5927  'OPENAI_API_KEY'
-000001a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000001b0: 4d41 585f 4552 524f 525f 434f 5252 4543  MAX_ERROR_CORREC
-000001c0: 5449 4f4e 5320 3d20 350d 0a20 2020 2020  TIONS = 5..     
-000001d0: 2020 2023 2053 6574 2074 6865 206d 6178     # Set the max
-000001e0: 696d 756d 206e 756d 6265 7220 6f66 2071  imum number of q
-000001f0: 7565 7374 696f 6e2f 616e 7377 6572 2070  uestion/answer p
-00000200: 6169 7273 2074 6f20 6265 206b 6570 7420  airs to be kept 
-00000210: 696e 2074 6865 2063 6f6e 7665 7273 6174  in the conversat
-00000220: 696f 6e20 6d65 6d6d 6f72 790d 0a20 2020  ion memmory..   
-00000230: 2020 2020 2073 656c 662e 4d41 585f 434f       self.MAX_CO
-00000240: 4e56 4552 5341 5449 4f4e 5320 3d20 286d  NVERSATIONS = (m
-00000250: 6178 5f63 6f6e 7665 7273 6174 696f 6e73  ax_conversations
-00000260: 2a32 2920 2d20 310d 0a0d 0a20 2020 2020  *2) - 1....     
-00000270: 2020 2073 656c 662e 6f72 6967 696e 616c     self.original
-00000280: 5f64 6620 3d20 6466 0d0a 2020 2020 2020  _df = df..      
-00000290: 2020 7365 6c66 2e64 6620 3d20 6466 2e63    self.df = df.c
-000002a0: 6f70 7928 2920 2023 206d 616b 6520 6120  opy()  # make a 
-000002b0: 636f 7079 206f 6620 7468 6520 6461 7461  copy of the data
-000002c0: 6672 616d 650d 0a20 2020 2020 2020 2073  frame..        s
-000002d0: 656c 662e 6466 5f68 6561 6420 3d20 7365  elf.df_head = se
-000002e0: 6c66 2e6f 7269 6769 6e61 6c5f 6466 2e68  lf.original_df.h
-000002f0: 6561 6428 3129 0d0a 2020 2020 0d0a 2020  ead(1)..    ..  
-00000300: 2020 2020 2020 7365 6c66 2e6c 6c6d 203d        self.llm =
-00000310: 206c 6c6d 0d0a 2020 2020 2020 2020 7365   llm..        se
-00000320: 6c66 2e6c 6c6d 5f73 7769 7463 6820 3d20  lf.llm_switch = 
-00000330: 6c6c 6d5f 7377 6974 6368 0d0a 0d0a 2020  llm_switch....  
-00000340: 2020 2020 2020 7365 6c66 2e74 6173 6b20        self.task 
-00000350: 3d20 2222 220d 0a20 2020 2020 2020 2054  = """..        T
-00000360: 6865 7265 2069 7320 6120 7061 6e64 6173  here is a pandas
-00000370: 2064 6174 6166 7261 6d65 2e0d 0a20 2020   dataframe...   
-00000380: 2020 2020 2054 6865 206e 616d 6520 6f66       The name of
-00000390: 2074 6865 2064 6174 6166 7261 6d65 2069   the dataframe i
-000003a0: 7320 6064 6660 2e0d 0a20 2020 2020 2020  s `df`...       
-000003b0: 2054 6869 7320 6973 2074 6865 2072 6573   This is the res
-000003c0: 756c 7420 6f66 2060 7072 696e 7428 6466  ult of `print(df
-000003d0: 2e68 6561 6428 3129 2960 3a0d 0a20 2020  .head(1))`:..   
-000003e0: 2020 2020 207b 7d2e 0d0a 2020 2020 2020       {}...      
-000003f0: 2020 5265 7475 726e 2074 6865 2070 7974    Return the pyt
-00000400: 686f 6e20 636f 6465 2074 6861 7420 7072  hon code that pr
-00000410: 696e 7473 206f 7574 2074 6865 2061 6e73  ints out the ans
-00000420: 7765 7220 746f 2074 6865 2066 6f6c 6c6f  wer to the follo
-00000430: 7769 6e67 2071 7565 7374 696f 6e20 3a20  wing question : 
-00000440: 7b7d 2e0d 0a20 2020 2020 2020 2041 6c77  {}...        Alw
-00000450: 6179 7320 696e 636c 7564 6520 7468 6520  ays include the 
-00000460: 696d 706f 7274 2073 7461 7465 6d65 6e74  import statement
-00000470: 7320 6174 2074 6865 2074 6f70 206f 6620  s at the top of 
-00000480: 7468 6520 636f 6465 2c20 616e 6420 636f  the code, and co
-00000490: 6d6d 656e 7473 2077 6865 7265 206e 6563  mments where nec
-000004a0: 6573 7361 7279 2e20 0d0a 2020 2020 2020  essary. ..      
-000004b0: 2020 5072 6566 6978 2074 6865 2070 7974    Prefix the pyt
-000004c0: 686f 6e20 636f 6465 2077 6974 6820 3c63  hon code with <c
-000004d0: 6f64 653e 2061 6e64 2073 7566 6669 7820  ode> and suffix 
-000004e0: 7468 6520 636f 6465 2077 6974 6820 3c2f  the code with </
-000004f0: 636f 6465 3e20 2e0d 0a20 2020 2020 2020  code> ...       
-00000500: 204f 6666 6572 2061 2073 686f 7274 2c20   Offer a short, 
-00000510: 636f 7570 6c65 206f 6620 7365 6e74 656e  couple of senten
-00000520: 6365 7320 7265 666c 6563 7469 6f6e 206f  ces reflection o
-00000530: 6e20 796f 7572 2061 6e73 7765 722e 0d0a  n your answer...
-00000540: 2020 2020 2020 2020 5072 6566 6978 2074          Prefix t
-00000550: 6865 2072 6566 6c65 6374 696f 6e20 7769  he reflection wi
-00000560: 7468 203c 7265 666c 6563 7469 6f6e 3e20  th <reflection> 
-00000570: 616e 6420 7375 6666 6978 2074 6865 2072  and suffix the r
-00000580: 6566 6c65 6374 696f 6e20 7769 7468 203c  eflection with <
-00000590: 2f72 6566 6c65 6374 696f 6e3e 2e0d 0a20  /reflection>... 
-000005a0: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-000005b0: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-000005c0: 5f63 6f72 7265 6374 5f74 6173 6b20 3d20  _correct_task = 
-000005d0: 2222 220d 0a20 2020 2020 2020 2054 6865  """..        The
-000005e0: 2063 6f64 6520 796f 7520 7072 6f76 6964   code you provid
-000005f0: 6564 2072 6573 756c 7465 6420 696e 2061  ed resulted in a
-00000600: 6e20 6572 726f 722e 0d0a 2020 2020 2020  n error...      
-00000610: 2020 5468 6520 6572 726f 7220 6d65 7373    The error mess
-00000620: 6167 6520 6973 3a20 7b7d 2e0d 0a20 2020  age is: {}...   
-00000630: 2020 2020 2054 6865 2063 6f64 6520 796f       The code yo
-00000640: 7520 7072 6f76 6964 6564 2069 733a 207b  u provided is: {
-00000650: 7d2e 0d0a 2020 2020 2020 2020 5468 6520  }...        The 
-00000660: 7175 6573 7469 6f6e 2077 6173 3a20 7b7d  question was: {}
-00000670: 2e0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00000680: 6e20 6120 636f 7272 6563 7465 6420 7079  n a corrected py
-00000690: 7468 6f6e 2063 6f64 6520 7468 6174 2066  thon code that f
-000006a0: 6978 6573 2074 6865 2065 7272 6f72 2e0d  ixes the error..
-000006b0: 0a20 2020 2020 2020 2041 6c77 6179 7320  .        Always 
-000006c0: 696e 636c 7564 6520 7468 6520 696d 706f  include the impo
-000006d0: 7274 2073 7461 7465 6d65 6e74 7320 6174  rt statements at
-000006e0: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
-000006f0: 636f 6465 2c20 616e 6420 636f 6d6d 656e  code, and commen
-00000700: 7473 2077 6865 7265 206e 6563 6573 7361  ts where necessa
-00000710: 7279 2e0d 0a20 2020 2020 2020 2050 7265  ry...        Pre
-00000720: 6669 7820 7468 6520 7079 7468 6f6e 2063  fix the python c
-00000730: 6f64 6520 7769 7468 203c 636f 6465 3e20  ode with <code> 
-00000740: 616e 6420 7375 6666 6978 2074 6865 2063  and suffix the c
-00000750: 6f64 6520 7769 7468 203c 2f63 6f64 653e  ode with </code>
-00000760: 2e0d 0a20 2020 2020 2020 204f 6666 6572  ...        Offer
-00000770: 2061 2073 686f 7274 2c20 636f 7570 6c65   a short, couple
-00000780: 206f 6620 7365 6e74 656e 6365 7320 7265   of sentences re
-00000790: 666c 6563 7469 6f6e 206f 6e20 796f 7572  flection on your
-000007a0: 2061 6e73 7765 722e 0d0a 2020 2020 2020   answer...      
-000007b0: 2020 5072 6566 6978 2074 6865 2072 6566    Prefix the ref
-000007c0: 6c65 6374 696f 6e20 7769 7468 203c 7265  lection with <re
-000007d0: 666c 6563 7469 6f6e 3e20 616e 6420 7375  flection> and su
-000007e0: 6666 6978 2074 6865 2072 6566 6c65 6374  ffix the reflect
-000007f0: 696f 6e20 7769 7468 203c 2f72 6566 6c65  ion with </refle
-00000800: 6374 696f 6e3e 2e0d 0a20 2020 2020 2020  ction>...       
-00000810: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00000820: 6f70 656e 6169 2e61 7069 5f6b 6579 203d  openai.api_key =
-00000830: 2073 656c 662e 4150 495f 4b45 590d 0a20   self.API_KEY.. 
-00000840: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-00000850: 6c5f 746f 6b65 6e73 5f75 7365 6420 3d20  l_tokens_used = 
-00000860: 5b5d 0d0a 0d0a 2020 2020 6465 6620 6c6c  []....    def ll
-00000870: 6d5f 6361 6c6c 2873 656c 662c 206d 6573  m_call(self, mes
-00000880: 7361 6765 733a 2073 7472 2c20 7465 6d70  sages: str, temp
-00000890: 6572 6174 7572 653a 2066 6c6f 6174 203d  erature: float =
-000008a0: 2030 2c20 6d61 785f 746f 6b65 6e73 3a20   0, max_tokens: 
-000008b0: 696e 7420 3d20 3130 3030 293a 0d0a 2020  int = 1000):..  
-000008c0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-000008d0: 206f 7065 6e61 692e 4368 6174 436f 6d70   openai.ChatComp
-000008e0: 6c65 7469 6f6e 2e63 7265 6174 6528 0d0a  letion.create(..
-000008f0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00000900: 6c3d 7365 6c66 2e6c 6c6d 2c0d 0a20 2020  l=self.llm,..   
-00000910: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00000920: 733d 6d65 7373 6167 6573 2c0d 0a20 2020  s=messages,..   
-00000930: 2020 2020 2020 2020 2074 656d 7065 7261           tempera
-00000940: 7475 7265 3d74 656d 7065 7261 7475 7265  ture=temperature
-00000950: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00000960: 6178 5f74 6f6b 656e 733d 6d61 785f 746f  ax_tokens=max_to
-00000970: 6b65 6e73 2c0d 0a20 2020 2020 2020 2029  kens,..        )
-00000980: 0d0a 0d0a 2020 2020 2020 2020 636f 6e74  ....        cont
-00000990: 656e 7420 3d20 7265 7370 6f6e 7365 2e63  ent = response.c
-000009a0: 686f 6963 6573 5b30 5d2e 6d65 7373 6167  hoices[0].messag
-000009b0: 652e 636f 6e74 656e 742e 7374 7269 7028  e.content.strip(
-000009c0: 290d 0a20 2020 2020 2020 2074 6f6b 656e  )..        token
-000009d0: 735f 7573 6564 203d 2072 6573 706f 6e73  s_used = respons
-000009e0: 652e 7573 6167 652e 746f 7461 6c5f 746f  e.usage.total_to
-000009f0: 6b65 6e73 0d0a 0d0a 2020 2020 2020 2020  kens....        
-00000a00: 7265 7475 726e 2063 6f6e 7465 6e74 2c20  return content, 
-00000a10: 746f 6b65 6e73 5f75 7365 640d 0a20 2020  tokens_used..   
-00000a20: 200d 0a20 2020 2023 2046 756e 6374 696f   ..    # Functio
-00000a30: 6e20 746f 2073 616e 6974 697a 6520 7468  n to sanitize th
-00000a40: 6520 6f75 7470 7574 2066 726f 6d20 7468  e output from th
-00000a50: 6520 4c4c 4d0d 0a20 2020 2064 6566 205f  e LLM..    def _
-00000a60: 6578 7472 6163 745f 636f 6465 2873 656c  extract_code(sel
-00000a70: 662c 7265 7370 6f6e 7365 3a20 7374 722c  f,response: str,
-00000a80: 2073 6570 6172 6174 6f72 3a20 7374 7220   separator: str 
-00000a90: 3d20 2260 6060 2229 202d 3e20 7374 723a  = "```") -> str:
-00000aa0: 0d0a 0d0a 2020 2020 2020 2020 2320 4465  ....        # De
-00000ab0: 6669 6e65 2061 2062 6c61 636b 6c69 7374  fine a blacklist
-00000ac0: 206f 6620 5079 7468 6f6e 206b 6579 776f   of Python keywo
-00000ad0: 7264 7320 616e 6420 6675 6e63 7469 6f6e  rds and function
-00000ae0: 7320 7468 6174 2061 7265 206e 6f74 2061  s that are not a
-00000af0: 6c6c 6f77 6564 0d0a 2020 2020 2020 2020  llowed..        
-00000b00: 626c 6163 6b6c 6973 7420 3d20 5b27 6f73  blacklist = ['os
-00000b10: 272c 2773 7562 7072 6f63 6573 7327 2c27  ','subprocess','
-00000b20: 7379 7327 2c27 6576 616c 272c 2765 7865  sys','eval','exe
-00000b30: 6327 2c27 6669 6c65 272c 2773 6f63 6b65  c','file','socke
-00000b40: 7427 2c27 7572 6c6c 6962 272c 0d0a 2020  t','urllib',..  
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2773 6875 7469 6c27 2c27 7069 636b    'shutil','pick
-00000b70: 6c65 272c 2763 7479 7065 7327 2c27 6d75  le','ctypes','mu
-00000b80: 6c74 6970 726f 6365 7373 696e 6727 2c27  ltiprocessing','
-00000b90: 7465 6d70 6669 6c65 272c 2767 6c6f 6227  tempfile','glob'
-00000ba0: 2c27 636f 6465 272c 2770 7479 272c 2763  ,'code','pty','c
-00000bb0: 6f6d 6d61 6e64 7327 2c0d 0a20 2020 2020  ommands',..     
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000bd0: 7265 7175 6573 7473 272c 2763 6769 272c  requests','cgi',
-00000be0: 2763 6769 7462 272c 2778 6d6c 2e65 7472  'cgitb','xml.etr
-00000bf0: 6565 2e45 6c65 6d65 6e74 5472 6565 272c  ee.ElementTree',
-00000c00: 2762 7569 6c74 696e 7327 0d0a 2020 2020  'builtins'..    
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 5d0d 0a20 2020 2020 2020 200d 0a20 2020  ]..        ..   
-00000c30: 2020 2020 2023 2053 6561 7263 6820 666f       # Search fo
-00000c40: 7220 6120 7061 7474 6572 6e20 6265 7477  r a pattern betw
-00000c50: 6565 6e20 3c72 6566 6c65 6374 696f 6e3e  een <reflection>
-00000c60: 2061 6e64 203c 2f72 6566 6c65 6374 696f   and </reflectio
-00000c70: 6e3e 2069 6e20 7468 6520 7265 7370 6f6e  n> in the respon
-00000c80: 7365 0d0a 2020 2020 2020 2020 6d61 7463  se..        matc
-00000c90: 6820 3d20 7265 2e73 6561 7263 6828 7222  h = re.search(r"
-00000ca0: 3c72 6566 6c65 6374 696f 6e3e 282e 2a29  <reflection>(.*)
-00000cb0: 3c2f 7265 666c 6563 7469 6f6e 3e22 2c20  </reflection>", 
-00000cc0: 7265 7370 6f6e 7365 2c20 7265 2e44 4f54  response, re.DOT
-00000cd0: 414c 4c29 0d0a 2020 2020 2020 2020 6966  ALL)..        if
-00000ce0: 206d 6174 6368 3a0d 0a20 2020 2020 2020   match:..       
-00000cf0: 2020 2020 2023 2049 6620 6120 6d61 7463       # If a matc
-00000d00: 6820 6973 2066 6f75 6e64 2c20 6578 7472  h is found, extr
-00000d10: 6163 7420 7468 6520 7265 666c 6563 7469  act the reflecti
-00000d20: 6f6e 2062 6574 7765 656e 203c 7265 666c  on between <refl
-00000d30: 6563 7469 6f6e 3e20 616e 6420 3c2f 7265  ection> and </re
-00000d40: 666c 6563 7469 6f6e 3e0d 0a20 2020 2020  flection>..     
-00000d50: 2020 2020 2020 2072 6566 6c65 6374 696f         reflectio
-00000d60: 6e20 3d20 6d61 7463 682e 6772 6f75 7028  n = match.group(
-00000d70: 3129 0d0a 2020 2020 2020 2020 656c 7365  1)..        else
-00000d80: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000d90: 6566 6c65 6374 696f 6e20 3d20 2222 0d0a  eflection = ""..
-00000da0: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-00000db0: 7468 6520 696e 6974 6961 6c20 7661 6c75  the initial valu
-00000dc0: 6520 6f66 2063 6f64 6520 746f 2074 6865  e of code to the
-00000dd0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00000de0: 2020 2063 6f64 6520 3d20 7265 7370 6f6e     code = respon
-00000df0: 7365 0d0a 0d0a 2020 2020 2020 2020 2320  se....        # 
-00000e00: 4966 2074 6865 2072 6573 706f 6e73 6520  If the response 
-00000e10: 636f 6e74 6169 6e73 2074 6865 2073 6570  contains the sep
-00000e20: 6172 6174 6f72 2c20 6578 7472 6163 7420  arator, extract 
-00000e30: 7468 6520 636f 6465 2062 6c6f 636b 2062  the code block b
-00000e40: 6574 7765 656e 2074 6865 2073 6570 6172  etween the separ
-00000e50: 6174 6f72 730d 0a20 2020 2020 2020 2069  ators..        i
-00000e60: 6620 6c65 6e28 7265 7370 6f6e 7365 2e73  f len(response.s
-00000e70: 706c 6974 2873 6570 6172 6174 6f72 2929  plit(separator))
-00000e80: 203e 2031 3a0d 0a20 2020 2020 2020 2020   > 1:..         
-00000e90: 2020 2063 6f64 6520 3d20 7265 7370 6f6e     code = respon
-00000ea0: 7365 2e73 706c 6974 2873 6570 6172 6174  se.split(separat
-00000eb0: 6f72 295b 315d 0d0a 0d0a 2020 2020 2020  or)[1]....      
-00000ec0: 2020 2320 5365 6172 6368 2066 6f72 2061    # Search for a
-00000ed0: 2070 6174 7465 726e 2062 6574 7765 656e   pattern between
-00000ee0: 203c 636f 6465 3e20 616e 6420 3c2f 636f   <code> and </co
-00000ef0: 6465 3e20 696e 2074 6865 2065 7874 7261  de> in the extra
-00000f00: 6374 6564 2063 6f64 650d 0a20 2020 2020  cted code..     
-00000f10: 2020 206d 6174 6368 203d 2072 652e 7365     match = re.se
-00000f20: 6172 6368 2872 223c 636f 6465 3e28 2e2a  arch(r"<code>(.*
-00000f30: 293c 2f63 6f64 653e 222c 2063 6f64 652c  )</code>", code,
-00000f40: 2072 652e 444f 5441 4c4c 290d 0a20 2020   re.DOTALL)..   
-00000f50: 2020 2020 2069 6620 6d61 7463 683a 0d0a       if match:..
-00000f60: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-00000f70: 2061 206d 6174 6368 2069 7320 666f 756e   a match is foun
-00000f80: 642c 2065 7874 7261 6374 2074 6865 2063  d, extract the c
-00000f90: 6f64 6520 6265 7477 6565 6e20 3c63 6f64  ode between <cod
-00000fa0: 653e 2061 6e64 203c 2f63 6f64 653e 0d0a  e> and </code>..
-00000fb0: 2020 2020 2020 2020 2020 2020 636f 6465              code
-00000fc0: 203d 206d 6174 6368 2e67 726f 7570 2831   = match.group(1
-00000fd0: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00000fe0: 2052 656d 6f76 6520 7468 6520 2270 7974   Remove the "pyt
-00000ff0: 686f 6e22 206f 7220 2270 7922 2070 7265  hon" or "py" pre
-00001000: 6669 7820 6966 2070 7265 7365 6e74 0d0a  fix if present..
-00001010: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00001020: 652e 6d61 7463 6828 7222 5e28 7079 7468  e.match(r"^(pyth
-00001030: 6f6e 7c70 7929 222c 2063 6f64 6529 3a0d  on|py)", code):.
-00001040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001050: 2063 6f64 6520 3d20 7265 2e73 7562 2872   code = re.sub(r
-00001060: 225e 2870 7974 686f 6e7c 7079 2922 2c20  "^(python|py)", 
-00001070: 2222 2c20 636f 6465 290d 0a0d 0a20 2020  "", code)....   
-00001080: 2020 2020 2023 2049 6620 7468 6520 636f       # If the co
-00001090: 6465 2069 7320 6265 7477 6565 6e20 7369  de is between si
-000010a0: 6e67 6c65 2062 6163 6b74 6963 6b73 2c20  ngle backticks, 
-000010b0: 6578 7472 6163 7420 7468 6520 636f 6465  extract the code
-000010c0: 2062 6574 7765 656e 2074 6865 6d0d 0a20   between them.. 
-000010d0: 2020 2020 2020 2069 6620 7265 2e6d 6174         if re.mat
-000010e0: 6368 2872 225e 602e 2a60 2422 2c20 636f  ch(r"^`.*`$", co
-000010f0: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
-00001100: 2020 636f 6465 203d 2072 652e 7375 6228    code = re.sub(
-00001110: 7222 5e60 282e 2a29 6024 222c 2072 225c  r"^`(.*)`$", r"\
-00001120: 3122 2c20 636f 6465 290d 0a0d 0a20 2020  1", code)....   
-00001130: 2020 2020 2023 2052 656d 6f76 6520 616e       # Remove an
-00001140: 7920 696e 7374 616e 6365 7320 6f66 2022  y instances of "
-00001150: 6466 203d 2070 642e 7265 6164 5f63 7376  df = pd.read_csv
-00001160: 2827 6669 6c65 6e61 6d65 2e63 7376 2729  ('filename.csv')
-00001170: 2220 6672 6f6d 2074 6865 2063 6f64 650d  " from the code.
-00001180: 0a20 2020 2020 2020 2063 6f64 6520 3d20  .        code = 
-00001190: 7265 2e73 7562 2872 2264 665c 732a 3d5c  re.sub(r"df\s*=\
-000011a0: 732a 7064 5c2e 7265 6164 5f63 7376 5c28  s*pd\.read_csv\(
-000011b0: 272e 2a3f 275c 2922 2c20 2222 2c20 636f  '.*?'\)", "", co
-000011c0: 6465 290d 0a20 2020 2020 2020 200d 0a20  de)..        .. 
-000011d0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-000011e0: 616e 7920 6f63 6375 7272 656e 6365 7320  any occurrences 
-000011f0: 6f66 2064 6620 3d20 7064 2e44 6174 6146  of df = pd.DataF
-00001200: 7261 6d65 2829 2077 6974 6820 616e 7920  rame() with any 
-00001210: 6e75 6d62 6572 206f 6620 6368 6172 6163  number of charac
-00001220: 7465 7273 2069 6e73 6964 6520 7468 6520  ters inside the 
-00001230: 7061 7265 6e74 6865 7365 732e 0d0a 2020  parentheses...  
-00001240: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
-00001250: 7375 6228 7222 6466 5c73 2a3d 5c73 2a70  sub(r"df\s*=\s*p
-00001260: 645c 2e44 6174 6146 7261 6d65 5c28 2e2a  d\.DataFrame\(.*
-00001270: 3f5c 2922 2c20 2222 2c20 636f 6465 290d  ?\)", "", code).
-00001280: 0a0d 0a20 2020 2020 2020 2023 2044 6566  ...        # Def
-00001290: 696e 6520 7468 6520 7265 6775 6c61 7220  ine the regular 
-000012a0: 6578 7072 6573 7369 6f6e 2070 6174 7465  expression patte
-000012b0: 726e 2074 6f20 6d61 7463 6820 7468 6520  rn to match the 
-000012c0: 626c 6163 6b6c 6973 7420 6974 656d 730d  blacklist items.
-000012d0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-000012e0: 203d 2072 225e 282e 2a5c 6228 2220 2b20   = r"^(.*\b(" + 
-000012f0: 227c 222e 6a6f 696e 2862 6c61 636b 6c69  "|".join(blackli
-00001300: 7374 2920 2b20 7222 295c 622e 2a29 2422  st) + r")\b.*)$"
-00001310: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
-00001320: 706c 6163 6520 7468 6520 626c 6163 6b6c  place the blackl
-00001330: 6973 7420 6974 656d 7320 7769 7468 2063  ist items with c
-00001340: 6f6d 6d65 6e74 730d 0a20 2020 2020 2020  omments..       
-00001350: 2063 6f64 6520 3d20 7265 2e73 7562 2870   code = re.sub(p
-00001360: 6174 7465 726e 2c20 7222 2320 6e6f 7420  attern, r"# not 
-00001370: 616c 6c6f 7765 6420 5c31 222c 2063 6f64  allowed \1", cod
-00001380: 652c 2066 6c61 6773 3d72 652e 4d55 4c54  e, flags=re.MULT
-00001390: 494c 494e 4529 0d0a 0d0a 2020 2020 2020  ILINE)....      
-000013a0: 2020 2320 5265 7475 726e 2074 6865 2063    # Return the c
-000013b0: 6c65 616e 6564 2061 6e64 2065 7874 7261  leaned and extra
-000013c0: 6374 6564 2063 6f64 650d 0a20 2020 2020  cted code..     
-000013d0: 2020 2072 6574 7572 6e20 636f 6465 2e73     return code.s
-000013e0: 7472 6970 2829 2c20 7265 666c 6563 7469  trip(), reflecti
-000013f0: 6f6e 2e73 7472 6970 2829 0d0a 0d0a 2020  on.strip()....  
-00001400: 2020 6465 6620 7064 5f61 6765 6e74 5f63    def pd_agent_c
-00001410: 6f6e 7665 7273 6528 7365 6c66 2c20 7175  onverse(self, qu
-00001420: 6573 7469 6f6e 3d4e 6f6e 6529 3a0d 0a20  estion=None):.. 
-00001430: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
-00001440: 697a 6520 7468 6520 6d65 7373 6167 6573  ize the messages
-00001450: 206c 6973 7420 7769 7468 2061 2073 7973   list with a sys
-00001460: 7465 6d20 6d65 7373 6167 6520 636f 6e74  tem message cont
-00001470: 6169 6e69 6e67 2074 6865 2074 6173 6b20  aining the task 
-00001480: 7072 6f6d 7074 0d0a 2020 2020 2020 2020  prompt..        
-00001490: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-000014a0: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
-000014b0: 636f 6e74 656e 7422 3a20 7365 6c66 2e74  content": self.t
-000014c0: 6173 6b2e 666f 726d 6174 2873 656c 662e  ask.format(self.
-000014d0: 6466 5f68 6561 642c 2022 2229 7d5d 0d0a  df_head, "")}]..
-000014e0: 0d0a 2020 2020 2020 2020 2320 4675 6e63  ..        # Func
-000014f0: 7469 6f6e 2074 6f20 6469 7370 6c61 7920  tion to display 
-00001500: 7265 7375 6c74 7320 6e69 6365 6c79 0d0a  results nicely..
-00001510: 2020 2020 2020 2020 6465 6620 6469 7370          def disp
-00001520: 6c61 795f 7265 7375 6c74 7328 616e 7377  lay_results(answ
-00001530: 6572 2c20 636f 6465 2c20 7265 666c 6563  er, code, reflec
-00001540: 7469 6f6e 2c20 746f 7461 6c5f 746f 6b65  tion, total_toke
-00001550: 6e73 5f75 7365 645f 7375 6d29 3a0d 0a20  ns_used_sum):.. 
-00001560: 2020 2020 2020 2020 2020 2069 6620 2769             if 'i
-00001570: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
-00001580: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
-00001590: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
-000015a0: 7974 6572 206e 6f74 6562 6f6f 6b20 6f72  yter notebook or
-000015b0: 2069 7079 7468 6f6e 0d0a 2020 2020 2020   ipython..      
-000015c0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-000015d0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
-000015e0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
-000015f0: 3b22 3e41 6e73 7765 723a 3c2f 623e 3c62  ;">Answer:</b><b
-00001600: 723e 3c70 7265 2073 7479 6c65 3d22 636f  r><pre style="co
-00001610: 6c6f 723a 626c 6163 6b3b 223e 3c62 3e7b  lor:black;"><b>{
-00001620: 616e 7377 6572 7d3c 2f62 3e3c 2f70 7265  answer}</b></pre
-00001630: 3e3c 2f70 3e3c 6272 3e27 2929 0d0a 2020  ></p><br>'))..  
-00001640: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00001650: 7370 6c61 7928 4854 4d4c 2866 273c 703e  splay(HTML(f'<p>
-00001660: 3c62 2073 7479 6c65 3d22 636f 6c6f 723a  <b style="color:
-00001670: 626c 7565 3b22 3e43 6f64 653a 3c2f 623e  blue;">Code:</b>
-00001680: 3c62 723e 3c70 7265 2073 7479 6c65 3d22  <br><pre style="
-00001690: 636f 6c6f 723a 2335 3535 3535 353b 223e  color:#555555;">
-000016a0: 7b63 6f64 657d 3c2f 7072 653e 3c2f 703e  {code}</pre></p>
-000016b0: 3c62 723e 2729 290d 0a20 2020 2020 2020  <br>'))..       
-000016c0: 2020 2020 2020 2020 2064 6973 706c 6179           display
-000016d0: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
-000016e0: 796c 653d 2263 6f6c 6f72 3a62 6c75 653b  yle="color:blue;
-000016f0: 223e 5468 6f75 6768 7473 3a3c 2f62 3e3c  ">Thoughts:</b><
-00001700: 6272 3e3c 6220 7374 796c 653d 2263 6f6c  br><b style="col
-00001710: 6f72 3a62 6c61 636b 3b22 3e7b 7265 666c  or:black;">{refl
-00001720: 6563 7469 6f6e 7d3c 2f62 3e3c 2f70 3e3c  ection}</b></p><
-00001730: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00001740: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00001750: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-00001760: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
-00001770: 3e54 6f74 616c 2054 6f6b 656e 7320 5573  >Total Tokens Us
-00001780: 6564 3a3c 2f62 3e3c 6272 3e3c 7370 616e  ed:</b><br><span
-00001790: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
-000017a0: 6163 6b3b 223e 7b74 6f74 616c 5f74 6f6b  ack;">{total_tok
-000017b0: 656e 735f 7573 6564 5f73 756d 7d3c 2f73  ens_used_sum}</s
-000017c0: 7061 6e3e 3c2f 703e 3c62 723e 2729 290d  pan></p><br>')).
-000017d0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000017e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000017f0: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
-00001800: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
-00001810: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
-00001820: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00001830: 6622 5c6e 416e 7377 6572 3a5c 6e7b 616e  f"\nAnswer:\n{an
-00001840: 7377 6572 7d5c 6e22 2c20 2767 7265 656e  swer}\n", 'green
-00001850: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-00001860: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00001870: 2020 2020 6370 7269 6e74 2866 2243 6f64      cprint(f"Cod
-00001880: 653a 5c6e 7b63 6f64 657d 5c6e 222c 2027  e:\n{code}\n", '
-00001890: 6772 6565 6e27 2c20 6174 7472 733d 5b27  green', attrs=['
-000018a0: 626f 6c64 275d 290d 0a20 2020 2020 2020  bold'])..       
-000018b0: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-000018c0: 6622 5468 6f75 6768 7473 3a5c 6e7b 7265  f"Thoughts:\n{re
-000018d0: 666c 6563 7469 6f6e 7d5c 6e22 2c20 2767  flection}\n", 'g
-000018e0: 7265 656e 272c 2061 7474 7273 3d5b 2762  reen', attrs=['b
-000018f0: 6f6c 6427 5d29 0d0a 2020 2020 2020 2020  old'])..        
-00001900: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
-00001910: 2254 6f74 616c 2074 6f6b 656e 7320 7573  "Total tokens us
-00001920: 6564 3a5c 6e7b 746f 7461 6c5f 746f 6b65  ed:\n{total_toke
-00001930: 6e73 5f75 7365 645f 7375 6d7d 5c6e 222c  ns_used_sum}\n",
-00001940: 2027 7965 6c6c 6f77 272c 2061 7474 7273   'yellow', attrs
-00001950: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
-00001960: 2020 2020 2020 2320 4966 2061 2071 7565        # If a que
-00001970: 7374 696f 6e20 6973 2070 726f 7669 6465  stion is provide
-00001980: 642c 2073 6b69 7020 7468 6520 696e 7075  d, skip the inpu
-00001990: 7420 7072 6f6d 7074 0d0a 2020 2020 2020  t prompt..      
-000019a0: 2020 6966 2071 7565 7374 696f 6e20 6973    if question is
-000019b0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-000019c0: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
-000019d0: 6865 2070 645f 6167 656e 7420 6d65 7468  he pd_agent meth
-000019e0: 6f64 2077 6974 6820 7468 6520 7573 6572  od with the user
-000019f0: 2773 2071 7565 7374 696f 6e2c 2074 6865  's question, the
-00001a00: 206d 6573 7361 6765 7320 6c69 7374 2c20   messages list, 
-00001a10: 616e 6420 7468 6520 6461 7461 6672 616d  and the datafram
-00001a20: 650d 0a20 2020 2020 2020 2020 2020 2061  e..            a
-00001a30: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
-00001a40: 6c65 6374 696f 6e2c 2074 6f74 616c 5f74  lection, total_t
-00001a50: 6f6b 656e 735f 7573 6564 5f73 756d 203d  okens_used_sum =
-00001a60: 2073 656c 662e 7064 5f61 6765 6e74 2871   self.pd_agent(q
-00001a70: 7565 7374 696f 6e2c 206d 6573 7361 6765  uestion, message
-00001a80: 732c 2073 656c 662e 6466 290d 0a20 2020  s, self.df)..   
-00001a90: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00001aa0: 5f72 6573 756c 7473 2861 6e73 7765 722c  _results(answer,
-00001ab0: 2063 6f64 652c 2072 6566 6c65 6374 696f   code, reflectio
-00001ac0: 6e2c 2074 6f74 616c 5f74 6f6b 656e 735f  n, total_tokens_
-00001ad0: 7573 6564 5f73 756d 290d 0a20 2020 2020  used_sum)..     
-00001ae0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00001af0: 0a20 2020 2020 2020 2023 2053 7461 7274  .        # Start
-00001b00: 2061 6e20 696e 6669 6e69 7465 206c 6f6f   an infinite loo
-00001b10: 7020 746f 206b 6565 7020 6173 6b69 6e67  p to keep asking
-00001b20: 2074 6865 2075 7365 7220 666f 7220 7175   the user for qu
-00001b30: 6573 7469 6f6e 730d 0a20 2020 2020 2020  estions..       
-00001b40: 2077 6869 6c65 2054 7275 653a 0d0a 2020   while True:..  
-00001b50: 2020 2020 2020 2020 2020 2320 5072 6f6d            # Prom
-00001b60: 7074 2074 6865 2075 7365 7220 746f 2065  pt the user to e
-00001b70: 6e74 6572 2061 2071 7565 7374 696f 6e20  nter a question 
-00001b80: 6f72 2074 7970 6520 2765 7869 7427 2074  or type 'exit' t
-00001b90: 6f20 7175 6974 0d0a 2020 2020 2020 2020  o quit..        
-00001ba0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
-00001bb0: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
-00001bc0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001bd0: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
-00001be0: 2827 3c62 2073 7479 6c65 3d22 636f 6c6f  ('<b style="colo
-00001bf0: 723a 626c 7565 3b22 3e45 6e74 6572 2079  r:blue;">Enter y
-00001c00: 6f75 7220 7175 6573 7469 6f6e 206f 7220  our question or 
-00001c10: 7479 7065 205c 2765 7869 745c 2720 746f  type \'exit\' to
-00001c20: 2071 7569 743a 3c2f 623e 2729 290d 0a20   quit:</b>')).. 
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-00001c40: 7565 7374 696f 6e20 3d20 696e 7075 7428  uestion = input(
-00001c50: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00001c60: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001c70: 2020 2020 2020 6370 7269 6e74 2822 5c6e        cprint("\n
-00001c80: 456e 7465 7220 796f 7572 2071 7565 7374  Enter your quest
-00001c90: 696f 6e20 6f72 2074 7970 6520 2765 7869  ion or type 'exi
-00001ca0: 7427 2074 6f20 7175 6974 3a22 2c20 2762  t' to quit:", 'b
-00001cb0: 6c75 6527 2c20 6174 7472 733d 5b27 626f  lue', attrs=['bo
-00001cc0: 6c64 275d 290d 0a20 2020 2020 2020 2020  ld'])..         
-00001cd0: 2020 2020 2020 2071 7565 7374 696f 6e20         question 
-00001ce0: 3d20 696e 7075 7428 290d 0a0d 0a20 2020  = input()....   
-00001cf0: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
-00001d00: 6520 7573 6572 2074 7970 6573 2027 6578  e user types 'ex
-00001d10: 6974 272c 2062 7265 616b 206f 7574 206f  it', break out o
-00001d20: 6620 7468 6520 6c6f 6f70 0d0a 2020 2020  f the loop..    
-00001d30: 2020 2020 2020 2020 6966 2071 7565 7374          if quest
-00001d40: 696f 6e2e 7374 7269 7028 292e 6c6f 7765  ion.strip().lowe
-00001d50: 7228 2920 3d3d 2027 6578 6974 273a 0d0a  r() == 'exit':..
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 6272 6561 6b0d 0a0d 0a20 2020 2020 2020  break....       
-00001d80: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
-00001d90: 7064 5f61 6765 6e74 206d 6574 686f 6420  pd_agent method 
-00001da0: 7769 7468 2074 6865 2075 7365 7227 7320  with the user's 
-00001db0: 7175 6573 7469 6f6e 2c20 7468 6520 6d65  question, the me
-00001dc0: 7373 6167 6573 206c 6973 742c 2061 6e64  ssages list, and
-00001dd0: 2074 6865 2064 6174 6166 7261 6d65 0d0a   the dataframe..
-00001de0: 2020 2020 2020 2020 2020 2020 616e 7377              answ
-00001df0: 6572 2c20 636f 6465 2c20 7265 666c 6563  er, code, reflec
-00001e00: 7469 6f6e 2c20 746f 7461 6c5f 746f 6b65  tion, total_toke
-00001e10: 6e73 5f75 7365 645f 7375 6d20 3d20 7365  ns_used_sum = se
-00001e20: 6c66 2e70 645f 6167 656e 7428 7175 6573  lf.pd_agent(ques
-00001e30: 7469 6f6e 2c20 6d65 7373 6167 6573 2c20  tion, messages, 
-00001e40: 7365 6c66 2e64 6629 0d0a 2020 2020 2020  self.df)..      
-00001e50: 2020 2020 2020 6469 7370 6c61 795f 7265        display_re
-00001e60: 7375 6c74 7328 616e 7377 6572 2c20 636f  sults(answer, co
-00001e70: 6465 2c20 7265 666c 6563 7469 6f6e 2c20  de, reflection, 
-00001e80: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00001e90: 645f 7375 6d29 0d0a 0d0a 2020 2020 6465  d_sum)....    de
-00001ea0: 6620 7064 5f61 6765 6e74 2873 656c 662c  f pd_agent(self,
-00001eb0: 2071 7565 7374 696f 6e2c 206d 6573 7361   question, messa
-00001ec0: 6765 732c 2064 663d 4e6f 6e65 293a 0d0a  ges, df=None):..
-00001ed0: 2020 2020 2020 2020 2320 4164 6420 6120          # Add a 
-00001ee0: 7573 6572 206d 6573 7361 6765 2077 6974  user message wit
-00001ef0: 6820 7468 6520 7570 6461 7465 6420 7461  h the updated ta
-00001f00: 736b 2070 726f 6d70 7420 746f 2074 6865  sk prompt to the
-00001f10: 206d 6573 7361 6765 7320 6c69 7374 0d0a   messages list..
-00001f20: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
-00001f30: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
-00001f40: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
-00001f50: 7422 3a20 7365 6c66 2e74 6173 6b2e 666f  t": self.task.fo
-00001f60: 726d 6174 2873 656c 662e 6466 5f68 6561  rmat(self.df_hea
-00001f70: 642c 2071 7565 7374 696f 6e29 7d29 0d0a  d, question)})..
-00001f80: 0d0a 2020 2020 2020 2020 6966 2027 6970  ..        if 'ip
-00001f90: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
-00001fa0: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
-00001fb0: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
-00001fc0: 6e6f 7465 626f 6f6b 206f 7220 6970 7974  notebook or ipyt
-00001fd0: 686f 6e0d 0a20 2020 2020 2020 2020 2020  hon..           
-00001fe0: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
-00001ff0: 3c70 2073 7479 6c65 3d22 636f 6c6f 723a  <p style="color:
-00002000: 6d61 6765 6e74 613b 223e 5c6e 5573 696e  magenta;">\nUsin
-00002010: 6720 4d6f 6465 6c3a 207b 7365 6c66 2e6c  g Model: {self.l
-00002020: 6c6d 7d3c 2f70 3e27 2929 0d0a 2020 2020  lm}</p>'))..    
-00002030: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00002040: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-00002050: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
-00002060: 613b 223e 5072 6f63 6573 7369 6e67 2079  a;">Processing y
-00002070: 6f75 7220 7265 7175 6573 742c 2070 6c65  our request, ple
-00002080: 6173 6520 7761 6974 2e2e 2e3c 2f62 3e3c  ase wait...</b><
-00002090: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
-000020a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000020b0: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
-000020c0: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
-000020d0: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
-000020e0: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
-000020f0: 6c6f 7265 6428 6622 5c6e 5573 696e 6720  lored(f"\nUsing 
-00002100: 4d6f 6465 6c3a 207b 7365 6c66 2e6c 6c6d  Model: {self.llm
-00002110: 7d22 2c20 226d 6167 656e 7461 2229 290d  }", "magenta")).
-00002120: 0a20 2020 2020 2020 2020 2020 2063 7072  .            cpr
-00002130: 696e 7428 6622 5c6e 3e20 5072 6f63 6573  int(f"\n> Proces
-00002140: 7369 6e67 2079 6f75 7220 7265 7175 6573  sing your reques
-00002150: 742c 2070 6c65 6173 6520 7761 6974 2e2e  t, please wait..
-00002160: 2e5c 6e22 2c20 276d 6167 656e 7461 272c  .\n", 'magenta',
-00002170: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-00002180: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
-00002190: 6c6c 2074 6865 204f 7065 6e41 4920 4150  ll the OpenAI AP
-000021a0: 4920 616e 6420 6861 6e64 6c65 2072 6174  I and handle rat
-000021b0: 6520 6c69 6d69 7420 6572 726f 7273 0d0a  e limit errors..
-000021c0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000021d0: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
-000021e0: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
-000021f0: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
-00002200: 616c 6c28 6d65 7373 6167 6573 290d 0a20  all(messages).. 
-00002210: 2020 2020 2020 2065 7863 6570 7420 6f70         except op
-00002220: 656e 6169 2e65 7272 6f72 2e52 6174 654c  enai.error.RateL
-00002230: 696d 6974 4572 726f 723a 0d0a 2020 2020  imitError:..    
-00002240: 2020 2020 2020 2020 7072 696e 7428 0d0a          print(..
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2254 6865 204f 7065 6e41 4920 4150 4920  "The OpenAI API 
-00002270: 7261 7465 206c 696d 6974 2068 6173 2062  rate limit has b
-00002280: 6565 6e20 6578 6365 6564 6564 2e20 5761  een exceeded. Wa
-00002290: 6974 696e 6720 3130 2073 6563 6f6e 6473  iting 10 seconds
-000022a0: 2061 6e64 2074 7279 696e 6720 6167 6169   and trying agai
-000022b0: 6e2e 220d 0a20 2020 2020 2020 2020 2020  n."..           
-000022c0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000022d0: 7469 6d65 2e73 6c65 6570 2831 3029 0d0a  time.sleep(10)..
-000022e0: 2020 2020 2020 2020 2020 2020 6c6c 6d5f              llm_
-000022f0: 7265 7370 6f6e 7365 2c20 746f 6b65 6e73  response, tokens
-00002300: 5f75 7365 6420 3d20 7365 6c66 2e6c 6c6d  _used = self.llm
-00002310: 5f63 616c 6c28 6d65 7373 6167 6573 290d  _call(messages).
-00002320: 0a0d 0a20 2020 2020 2020 2023 2045 7874  ...        # Ext
-00002330: 7261 6374 2074 6865 2063 6f64 6520 6672  ract the code fr
-00002340: 6f6d 2074 6865 2041 5049 2072 6573 706f  om the API respo
-00002350: 6e73 650d 0a20 2020 2020 2020 2063 6f64  nse..        cod
-00002360: 652c 7265 666c 6563 7469 6f6e 203d 2073  e,reflection = s
-00002370: 656c 662e 5f65 7874 7261 6374 5f63 6f64  elf._extract_cod
-00002380: 6528 6c6c 6d5f 7265 7370 6f6e 7365 290d  e(llm_response).
-00002390: 0a0d 0a20 2020 2020 2020 2023 2055 7064  ...        # Upd
-000023a0: 6174 6520 7468 6520 746f 7461 6c20 746f  ate the total to
-000023b0: 6b65 6e73 2075 7365 640d 0a20 2020 2020  kens used..     
-000023c0: 2020 2073 656c 662e 746f 7461 6c5f 746f     self.total_to
-000023d0: 6b65 6e73 5f75 7365 642e 6170 7065 6e64  kens_used.append
-000023e0: 2874 6f6b 656e 735f 7573 6564 290d 0a20  (tokens_used).. 
-000023f0: 2020 2020 2020 2074 6f74 616c 5f74 6f6b         total_tok
-00002400: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
-00002410: 756d 2873 656c 662e 746f 7461 6c5f 746f  um(self.total_to
-00002420: 6b65 6e73 5f75 7365 6429 0d0a 0d0a 2020  kens_used)....  
-00002430: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-00002440: 7a65 2065 7272 6f72 2063 6f72 7265 6374  ze error correct
-00002450: 696f 6e20 636f 756e 7465 720d 0a20 2020  ion counter..   
-00002460: 2020 2020 2065 7272 6f72 5f63 6f72 7265       error_corre
-00002470: 6374 696f 6e73 203d 2030 0d0a 0d0a 2020  ctions = 0....  
-00002480: 2020 2020 2020 2320 5374 6f72 6520 7468        # Store th
-00002490: 6520 6f72 6967 696e 616c 206c 6c6d 2076  e original llm v
-000024a0: 616c 7565 0d0a 2020 2020 2020 2020 6f72  alue..        or
-000024b0: 6967 696e 616c 5f6c 6c6d 203d 2073 656c  iginal_llm = sel
-000024c0: 662e 6c6c 6d0d 0a0d 0a20 2020 2020 2020  f.llm....       
-000024d0: 2023 2052 6564 6972 6563 7420 7374 616e   # Redirect stan
-000024e0: 6461 7264 206f 7574 7075 7420 746f 2061  dard output to a
-000024f0: 2053 7472 696e 6749 4f20 6275 6666 6572   StringIO buffer
-00002500: 0d0a 2020 2020 2020 2020 7769 7468 2072  ..        with r
-00002510: 6564 6972 6563 745f 7374 646f 7574 2869  edirect_stdout(i
-00002520: 6f2e 5374 7269 6e67 494f 2829 2920 6173  o.StringIO()) as
-00002530: 206f 7574 7075 743a 0d0a 2020 2020 2020   output:..      
-00002540: 2020 2020 2020 2320 5472 7920 746f 2065        # Try to e
-00002550: 7865 6375 7465 2074 6865 2063 6f64 6520  xecute the code 
-00002560: 616e 6420 6861 6e64 6c65 2065 7272 6f72  and handle error
-00002570: 730d 0a20 2020 2020 2020 2020 2020 2077  s..            w
-00002580: 6869 6c65 2065 7272 6f72 5f63 6f72 7265  hile error_corre
-00002590: 6374 696f 6e73 203c 2073 656c 662e 4d41  ctions < self.MA
-000025a0: 585f 4552 524f 525f 434f 5252 4543 5449  X_ERROR_CORRECTI
-000025b0: 4f4e 533a 0d0a 2020 2020 2020 2020 2020  ONS:..          
-000025c0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 6d65 7373 6167 6573 2e61 7070 656e 6428  messages.append(
-000025f0: 7b22 726f 6c65 223a 2022 6173 7369 7374  {"role": "assist
-00002600: 616e 7422 2c20 2263 6f6e 7465 6e74 223a  ant", "content":
-00002610: 206c 6c6d 5f72 6573 706f 6e73 657d 290d   llm_response}).
-00002620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002630: 2020 2020 2023 2052 656d 6f76 6520 7468       # Remove th
-00002640: 6520 6f6c 6465 7374 2063 6f6e 7665 7273  e oldest convers
-00002650: 6174 696f 6e20 6672 6f6d 2074 6865 206d  ation from the m
-00002660: 6573 7361 6765 7320 6c69 7374 0d0a 2020  essages list..  
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 2020 6966 206c 656e 286d 6573 7361 6765    if len(message
-00002690: 7329 203e 2073 656c 662e 4d41 585f 434f  s) > self.MAX_CO
-000026a0: 4e56 4552 5341 5449 4f4e 533a 0d0a 2020  NVERSATIONS:..  
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 2020 6d65 7373 6167 6573 2e70        messages.p
-000026d0: 6f70 2831 290d 0a20 2020 2020 2020 2020  op(1)..         
-000026e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000026f0: 6573 7361 6765 732e 706f 7028 3129 0d0a  essages.pop(1)..
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2320 5265 7365 7420 6466 2074      # Reset df t
-00002720: 6f20 7468 6520 6f72 6967 696e 616c 2073  o the original s
-00002730: 7461 7465 2062 6566 6f72 6520 6578 6563  tate before exec
-00002740: 7574 696e 6720 7468 6520 636f 6465 0d0a  uting the code..
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 2020 7365 6c66 2e64 6620 3d20 7365      self.df = se
-00002770: 6c66 2e6f 7269 6769 6e61 6c5f 6466 2e63  lf.original_df.c
-00002780: 6f70 7928 290d 0a20 2020 2020 2020 2020  opy()..         
-00002790: 2020 2020 2020 2020 2020 2023 2045 7865             # Exe
-000027a0: 6375 7465 2074 6865 2063 6f64 650d 0a20  cute the code.. 
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2065 7865 6328 636f 6465 290d 0a20     exec(code).. 
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-000027f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00002800: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00002810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002820: 2020 2020 2020 2320 5072 696e 7420 7468        # Print th
-00002830: 6520 6572 726f 7220 6d65 7373 6167 650d  e error message.
-00002840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002850: 2020 2020 2069 6620 2769 7079 6b65 726e       if 'ipykern
-00002860: 656c 2720 696e 2073 7973 2e6d 6f64 756c  el' in sys.modul
-00002870: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00002880: 2020 2020 2020 2020 2020 2020 2023 204a               # J
-00002890: 7570 7974 6572 206e 6f74 6562 6f6f 6b0d  upyter notebook.
-000028a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028b0: 2020 2020 2020 2020 2064 6973 706c 6179           display
-000028c0: 2848 544d 4c28 6627 3c62 3e3c 7370 616e  (HTML(f'<b><span
-000028d0: 2073 7479 6c65 3d22 636f 6c6f 723a 2072   style="color: r
-000028e0: 6564 3b22 3e45 7272 6f72 3a3c 6272 3e3c  ed;">Error:<br><
-000028f0: 7072 653e 7b65 7d3c 2f70 7265 3e3c 6272  pre>{e}</pre><br
-00002900: 3e54 6865 2061 6765 6e74 2077 696c 6c20  >The agent will 
-00002910: 7265 7472 792e 3c2f 7370 616e 3e3c 2f62  retry.</span></b
-00002920: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00002930: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00002940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002950: 2020 2020 2020 2020 2023 2043 4c49 0d0a           # CLI..
-00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
-00002980: 6c6f 7265 6428 6627 4572 726f 723a 207b  lored(f'Error: {
-00002990: 657d 2e20 5468 6520 6167 656e 7420 7769  e}. The agent wi
-000029a0: 6c6c 2072 6574 7279 2e27 2c20 2772 6564  ll retry.', 'red
-000029b0: 2729 290d 0a0d 0a20 2020 2020 2020 2020  '))....         
-000029c0: 2020 2020 2020 2020 2020 2023 2049 6e63             # Inc
-000029d0: 7265 6d65 6e74 2074 6865 2065 7272 6f72  rement the error
-000029e0: 2063 6f72 7265 6374 696f 6e20 636f 756e   correction coun
-000029f0: 7465 7220 616e 6420 7570 6461 7465 2074  ter and update t
-00002a00: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
-00002a10: 2077 6974 6820 7468 6520 6572 726f 720d   with the error.
-00002a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a30: 2020 2020 2065 7272 6f72 5f63 6f72 7265       error_corre
-00002a40: 6374 696f 6e73 202b 3d20 310d 0a20 2020  ctions += 1..   
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 206d 6573 7361 6765 732e 6170 7065 6e64   messages.append
-00002a70: 287b 2272 6f6c 6522 3a20 2275 7365 7222  ({"role": "user"
-00002a80: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
-00002a90: 662e 6572 726f 725f 636f 7272 6563 745f  f.error_correct_
-00002aa0: 7461 736b 2e66 6f72 6d61 7428 652c 2063  task.format(e, c
-00002ab0: 6f64 652c 2071 7565 7374 696f 6e29 7d29  ode, question)})
-00002ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002ad0: 2020 2020 2020 2020 2320 5377 6974 6368          # Switch
-00002ae0: 2074 6f20 6770 742d 3420 6966 206c 6c6d   to gpt-4 if llm
-00002af0: 5f73 7769 7463 6820 6973 2054 7275 650d  _switch is True.
-00002b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b10: 2020 2020 2069 6620 7365 6c66 2e6c 6c6d       if self.llm
-00002b20: 5f73 7769 7463 683a 0d0a 2020 2020 2020  _switch:..      
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 7365 6c66 2e6c 6c6d 203d 2027 6770    self.llm = 'gp
-00002b50: 742d 3427 0d0a 2020 2020 2020 2020 2020  t-4'..          
-00002b60: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002b70: 2027 6970 796b 6572 6e65 6c27 2069 6e20   'ipykernel' in 
-00002b80: 7379 732e 6d6f 6475 6c65 733a 0d0a 2020  sys.modules:..  
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2020 2020 2020 2320 4a75 7079            # Jupy
-00002bb0: 7465 7220 6e6f 7465 626f 6f6b 0d0a 2020  ter notebook..  
+00000020: 7973 0d0a 696d 706f 7274 2062 6173 6536  ys..import base6
+00000030: 340d 0a66 726f 6d20 636f 6e74 6578 746c  4..from contextl
+00000040: 6962 2069 6d70 6f72 7420 7265 6469 7265  ib import redire
+00000050: 6374 5f73 7464 6f75 740d 0a69 6d70 6f72  ct_stdout..impor
+00000060: 7420 696f 0d0a 696d 706f 7274 2074 696d  t io..import tim
+00000070: 650d 0a69 6d70 6f72 7420 6f70 656e 6169  e..import openai
+00000080: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
+00000090: 6173 2070 640d 0a66 726f 6d20 7465 726d  as pd..from term
+000000a0: 636f 6c6f 7220 696d 706f 7274 2063 6f6c  color import col
+000000b0: 6f72 6564 2c20 6370 7269 6e74 0d0a 6672  ored, cprint..fr
+000000c0: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
+000000d0: 6179 2069 6d70 6f72 7420 6469 7370 6c61  ay import displa
+000000e0: 792c 2049 6d61 6765 2c20 4854 4d4c 0d0a  y, Image, HTML..
+000000f0: 0d0a 636c 6173 7320 4261 6d62 6f6f 4149  ..class BambooAI
+00000100: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
+00000110: 745f 5f28 7365 6c66 2c20 6466 3a20 7064  t__(self, df: pd
+00000120: 2e44 6174 6146 7261 6d65 2c6d 6178 5f63  .DataFrame,max_c
+00000130: 6f6e 7665 7273 6174 696f 6e73 3a20 696e  onversations: in
+00000140: 7420 3d20 3320 2c6c 6c6d 3a20 7374 7220  t = 3 ,llm: str 
+00000150: 3d20 2767 7074 2d33 2e35 2d74 7572 626f  = 'gpt-3.5-turbo
+00000160: 272c 6c6c 6d5f 7377 6974 6368 3a20 626f  ',llm_switch: bo
+00000170: 6f6c 203d 2046 616c 7365 293a 0d0a 0d0a  ol = False):....
+00000180: 2020 2020 2020 2020 7365 6c66 2e41 5049          self.API
+00000190: 5f4b 4559 203d 206f 732e 656e 7669 726f  _KEY = os.enviro
+000001a0: 6e2e 6765 7428 274f 5045 4e41 495f 4150  n.get('OPENAI_AP
+000001b0: 495f 4b45 5927 290d 0a20 2020 2020 2020  I_KEY')..       
+000001c0: 2073 656c 662e 4d41 585f 4552 524f 525f   self.MAX_ERROR_
+000001d0: 434f 5252 4543 5449 4f4e 5320 3d20 350d  CORRECTIONS = 5.
+000001e0: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
+000001f0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
+00000200: 7220 6f66 2071 7565 7374 696f 6e2f 616e  r of question/an
+00000210: 7377 6572 2070 6169 7273 2074 6f20 6265  swer pairs to be
+00000220: 206b 6570 7420 696e 2074 6865 2063 6f6e   kept in the con
+00000230: 7665 7273 6174 696f 6e20 6d65 6d6d 6f72  versation memmor
+00000240: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
+00000250: 4d41 585f 434f 4e56 4552 5341 5449 4f4e  MAX_CONVERSATION
+00000260: 5320 3d20 286d 6178 5f63 6f6e 7665 7273  S = (max_convers
+00000270: 6174 696f 6e73 2a32 2920 2d20 310d 0a0d  ations*2) - 1...
+00000280: 0a20 2020 2020 2020 2073 656c 662e 6f72  .        self.or
+00000290: 6967 696e 616c 5f64 6620 3d20 6466 0d0a  iginal_df = df..
+000002a0: 2020 2020 2020 2020 7365 6c66 2e64 6620          self.df 
+000002b0: 3d20 6466 2e63 6f70 7928 2920 2023 206d  = df.copy()  # m
+000002c0: 616b 6520 6120 636f 7079 206f 6620 7468  ake a copy of th
+000002d0: 6520 6461 7461 6672 616d 650d 0a20 2020  e dataframe..   
+000002e0: 2020 2020 2073 656c 662e 6466 5f68 6561       self.df_hea
+000002f0: 6420 3d20 7365 6c66 2e6f 7269 6769 6e61  d = self.origina
+00000300: 6c5f 6466 2e68 6561 6428 3129 0d0a 2020  l_df.head(1)..  
+00000310: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00000320: 2e6c 6c6d 203d 206c 6c6d 0d0a 2020 2020  .llm = llm..    
+00000330: 2020 2020 7365 6c66 2e6c 6c6d 5f73 7769      self.llm_swi
+00000340: 7463 6820 3d20 6c6c 6d5f 7377 6974 6368  tch = llm_switch
+00000350: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00000360: 2e74 6173 6b20 3d20 2222 220d 0a20 2020  .task = """..   
+00000370: 2020 2020 2054 6865 7265 2069 7320 6120       There is a 
+00000380: 7061 6e64 6173 2064 6174 6166 7261 6d65  pandas dataframe
+00000390: 2e0d 0a20 2020 2020 2020 2054 6865 206e  ...        The n
+000003a0: 616d 6520 6f66 2074 6865 2064 6174 6166  ame of the dataf
+000003b0: 7261 6d65 2069 7320 6064 6660 2e0d 0a20  rame is `df`... 
+000003c0: 2020 2020 2020 2054 6869 7320 6973 2074         This is t
+000003d0: 6865 2072 6573 756c 7420 6f66 2060 7072  he result of `pr
+000003e0: 696e 7428 6466 2e68 6561 6428 3129 2960  int(df.head(1))`
+000003f0: 3a0d 0a20 2020 2020 2020 207b 7d2e 0d0a  :..        {}...
+00000400: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+00000410: 6865 2070 7974 686f 6e20 636f 6465 2074  he python code t
+00000420: 6861 7420 7072 696e 7473 206f 7574 2074  hat prints out t
+00000430: 6865 2061 6e73 7765 7220 746f 2074 6865  he answer to the
+00000440: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
+00000450: 696f 6e20 3a20 7b7d 2e0d 0a20 2020 2020  ion : {}...     
+00000460: 2020 2041 6c77 6179 7320 696e 636c 7564     Always includ
+00000470: 6520 7468 6520 696d 706f 7274 2073 7461  e the import sta
+00000480: 7465 6d65 6e74 7320 6174 2074 6865 2074  tements at the t
+00000490: 6f70 206f 6620 7468 6520 636f 6465 2c20  op of the code, 
+000004a0: 616e 6420 636f 6d6d 656e 7473 2077 6865  and comments whe
+000004b0: 7265 206e 6563 6573 7361 7279 2e20 0d0a  re necessary. ..
+000004c0: 2020 2020 2020 2020 5072 6566 6978 2074          Prefix t
+000004d0: 6865 2070 7974 686f 6e20 636f 6465 2077  he python code w
+000004e0: 6974 6820 3c63 6f64 653e 2061 6e64 2073  ith <code> and s
+000004f0: 7566 6669 7820 7468 6520 636f 6465 2077  uffix the code w
+00000500: 6974 6820 3c2f 636f 6465 3e2e 0d0a 2020  ith </code>...  
+00000510: 2020 2020 2020 4f66 6665 7220 6120 7368        Offer a sh
+00000520: 6f72 742c 2063 6f75 706c 6520 6f66 2073  ort, couple of s
+00000530: 656e 7465 6e63 6573 2072 6566 6c65 6374  entences reflect
+00000540: 696f 6e20 6f6e 2079 6f75 7220 616e 7377  ion on your answ
+00000550: 6572 2e0d 0a20 2020 2020 2020 2050 7265  er...        Pre
+00000560: 6669 7820 7468 6520 7265 666c 6563 7469  fix the reflecti
+00000570: 6f6e 2077 6974 6820 3c72 6566 6c65 6374  on with <reflect
+00000580: 696f 6e3e 2061 6e64 2073 7566 6669 7820  ion> and suffix 
+00000590: 7468 6520 7265 666c 6563 7469 6f6e 2077  the reflection w
+000005a0: 6974 6820 3c2f 7265 666c 6563 7469 6f6e  ith </reflection
+000005b0: 3e2e 0d0a 2020 2020 2020 2020 4669 6e61  >...        Fina
+000005c0: 6c6c 7920 6f75 7470 7574 2061 2063 6f64  lly output a cod
+000005d0: 6520 666f 7220 6d65 726d 6169 6420 6469  e for mermaid di
+000005e0: 6167 7261 6d2e 2054 6865 2063 6f64 6520  agram. The code 
+000005f0: 7368 6f75 6c64 2073 7461 7274 2077 6974  should start wit
+00000600: 6820 2267 7261 7068 2054 443b 220d 0a20  h "graph TD;".. 
+00000610: 2020 2020 2020 2050 7265 6669 7820 7468         Prefix th
+00000620: 6520 6d65 726d 6169 6420 636f 6465 2077  e mermaid code w
+00000630: 6974 6820 3c66 6c6f 773e 2061 6e64 2073  ith <flow> and s
+00000640: 7566 6669 7820 7468 6520 6d65 726d 6169  uffix the mermai
+00000650: 6420 666c 6f77 2077 6974 6820 3c2f 666c  d flow with </fl
+00000660: 6f77 3e2e 0d0a 2020 2020 2020 2020 2222  ow>...        ""
+00000670: 220d 0a0d 0a20 2020 2020 2020 2073 656c  "....        sel
+00000680: 662e 6572 726f 725f 636f 7272 6563 745f  f.error_correct_
+00000690: 7461 736b 203d 2022 2222 0d0a 2020 2020  task = """..    
+000006a0: 2020 2020 5468 6520 636f 6465 2079 6f75      The code you
+000006b0: 2070 726f 7669 6465 6420 7265 7375 6c74   provided result
+000006c0: 6564 2069 6e20 616e 2065 7272 6f72 2e0d  ed in an error..
+000006d0: 0a20 2020 2020 2020 2054 6865 2065 7272  .        The err
+000006e0: 6f72 206d 6573 7361 6765 2069 733a 207b  or message is: {
+000006f0: 7d2e 0d0a 2020 2020 2020 2020 5468 6520  }...        The 
+00000700: 636f 6465 2079 6f75 2070 726f 7669 6465  code you provide
+00000710: 6420 6973 3a20 7b7d 2e0d 0a20 2020 2020  d is: {}...     
+00000720: 2020 2054 6865 2071 7565 7374 696f 6e20     The question 
+00000730: 7761 733a 207b 7d2e 0d0a 2020 2020 2020  was: {}...      
+00000740: 2020 5265 7475 726e 2061 2063 6f72 7265    Return a corre
+00000750: 6374 6564 2070 7974 686f 6e20 636f 6465  cted python code
+00000760: 2074 6861 7420 6669 7865 7320 7468 6520   that fixes the 
+00000770: 6572 726f 722e 0d0a 2020 2020 2020 2020  error...        
+00000780: 416c 7761 7973 2069 6e63 6c75 6465 2074  Always include t
+00000790: 6865 2069 6d70 6f72 7420 7374 6174 656d  he import statem
+000007a0: 656e 7473 2061 7420 7468 6520 746f 7020  ents at the top 
+000007b0: 6f66 2074 6865 2063 6f64 652c 2061 6e64  of the code, and
+000007c0: 2063 6f6d 6d65 6e74 7320 7768 6572 6520   comments where 
+000007d0: 6e65 6365 7373 6172 792e 0d0a 2020 2020  necessary...    
+000007e0: 2020 2020 5072 6566 6978 2074 6865 2070      Prefix the p
+000007f0: 7974 686f 6e20 636f 6465 2077 6974 6820  ython code with 
+00000800: 3c63 6f64 653e 2061 6e64 2073 7566 6669  <code> and suffi
+00000810: 7820 7468 6520 636f 6465 2077 6974 6820  x the code with 
+00000820: 3c2f 636f 6465 3e2e 0d0a 2020 2020 2020  </code>...      
+00000830: 2020 4f66 6665 7220 6120 7368 6f72 742c    Offer a short,
+00000840: 2063 6f75 706c 6520 6f66 2073 656e 7465   couple of sente
+00000850: 6e63 6573 2072 6566 6c65 6374 696f 6e20  nces reflection 
+00000860: 6f6e 2079 6f75 7220 616e 7377 6572 2e0d  on your answer..
+00000870: 0a20 2020 2020 2020 2050 7265 6669 7820  .        Prefix 
+00000880: 7468 6520 7265 666c 6563 7469 6f6e 2077  the reflection w
+00000890: 6974 6820 3c72 6566 6c65 6374 696f 6e3e  ith <reflection>
+000008a0: 2061 6e64 2073 7566 6669 7820 7468 6520   and suffix the 
+000008b0: 7265 666c 6563 7469 6f6e 2077 6974 6820  reflection with 
+000008c0: 3c2f 7265 666c 6563 7469 6f6e 3e2e 0d0a  </reflection>...
+000008d0: 2020 2020 2020 2020 4669 6e61 6c6c 7920          Finally 
+000008e0: 6f75 7470 7574 2061 2063 6f64 6520 666f  output a code fo
+000008f0: 7220 6d65 726d 6169 6420 6469 6167 7261  r mermaid diagra
+00000900: 6d2e 2054 6865 2063 6f64 6520 7368 6f75  m. The code shou
+00000910: 6c64 2073 7461 7274 2077 6974 6820 2267  ld start with "g
+00000920: 7261 7068 2054 443b 220d 0a20 2020 2020  raph TD;"..     
+00000930: 2020 2050 7265 6669 7820 7468 6520 6d65     Prefix the me
+00000940: 726d 6169 6420 636f 6465 2077 6974 6820  rmaid code with 
+00000950: 3c66 6c6f 773e 2061 6e64 2073 7566 6669  <flow> and suffi
+00000960: 7820 7468 6520 6d65 726d 6169 6420 666c  x the mermaid fl
+00000970: 6f77 2077 6974 6820 3c2f 666c 6f77 3e2e  ow with </flow>.
+00000980: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+00000990: 0a20 2020 2020 2020 206f 7065 6e61 692e  .        openai.
+000009a0: 6170 695f 6b65 7920 3d20 7365 6c66 2e41  api_key = self.A
+000009b0: 5049 5f4b 4559 0d0a 2020 2020 2020 2020  PI_KEY..        
+000009c0: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+000009d0: 735f 7573 6564 203d 205b 5d0d 0a20 2020  s_used = []..   
+000009e0: 200d 0a20 2020 2023 2046 756e 6374 696f   ..    # Functio
+000009f0: 6e20 746f 2063 6f6e 7665 7274 2074 6865  n to convert the
+00000a00: 2067 7261 7068 2074 6f20 616e 2069 6d61   graph to an ima
+00000a10: 6765 2075 7369 6e67 206d 6572 6d61 6964  ge using mermaid
+00000a20: 2e69 6e6b 0d0a 2020 2020 6465 6620 6d6d  .ink..    def mm
+00000a30: 2873 656c 662c 2067 7261 7068 293a 0d0a  (self, graph):..
+00000a40: 2020 2020 2020 2020 6772 6170 6862 7974          graphbyt
+00000a50: 6573 203d 2067 7261 7068 2e65 6e63 6f64  es = graph.encod
+00000a60: 6528 2261 7363 6969 2229 0d0a 2020 2020  e("ascii")..    
+00000a70: 2020 2020 6261 7365 3634 5f62 7974 6573      base64_bytes
+00000a80: 203d 2062 6173 6536 342e 6236 3465 6e63   = base64.b64enc
+00000a90: 6f64 6528 6772 6170 6862 7974 6573 290d  ode(graphbytes).
+00000aa0: 0a20 2020 2020 2020 2062 6173 6536 345f  .        base64_
+00000ab0: 7374 7269 6e67 203d 2062 6173 6536 345f  string = base64_
+00000ac0: 6279 7465 732e 6465 636f 6465 2822 6173  bytes.decode("as
+00000ad0: 6369 6922 290d 0a20 2020 2020 2020 2069  cii")..        i
+00000ae0: 6d67 5f75 726c 203d 2022 6874 7470 733a  mg_url = "https:
+00000af0: 2f2f 6d65 726d 6169 642e 696e 6b2f 696d  //mermaid.ink/im
+00000b00: 672f 2220 2b20 6261 7365 3634 5f73 7472  g/" + base64_str
+00000b10: 696e 670d 0a20 2020 2020 2020 2072 6574  ing..        ret
+00000b20: 7572 6e20 696d 675f 7572 6c0d 0a0d 0a20  urn img_url.... 
+00000b30: 2020 2064 6566 206c 6c6d 5f63 616c 6c28     def llm_call(
+00000b40: 7365 6c66 2c20 6d65 7373 6167 6573 3a20  self, messages: 
+00000b50: 7374 722c 2074 656d 7065 7261 7475 7265  str, temperature
+00000b60: 3a20 666c 6f61 7420 3d20 302c 206d 6178  : float = 0, max
+00000b70: 5f74 6f6b 656e 733a 2069 6e74 203d 2031  _tokens: int = 1
+00000b80: 3030 3029 3a0d 0a20 2020 2020 2020 2072  000):..        r
+00000b90: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
+00000ba0: 2e43 6861 7443 6f6d 706c 6574 696f 6e2e  .ChatCompletion.
+00000bb0: 6372 6561 7465 280d 0a20 2020 2020 2020  create(..       
+00000bc0: 2020 2020 206d 6f64 656c 3d73 656c 662e       model=self.
+00000bd0: 6c6c 6d2c 0d0a 2020 2020 2020 2020 2020  llm,..          
+00000be0: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
+00000bf0: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
+00000c00: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
+00000c10: 6d70 6572 6174 7572 652c 0d0a 2020 2020  mperature,..    
+00000c20: 2020 2020 2020 2020 6d61 785f 746f 6b65          max_toke
+00000c30: 6e73 3d6d 6178 5f74 6f6b 656e 732c 0d0a  ns=max_tokens,..
+00000c40: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00000c50: 2020 2020 2063 6f6e 7465 6e74 203d 2072       content = r
+00000c60: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
+00000c70: 305d 2e6d 6573 7361 6765 2e63 6f6e 7465  0].message.conte
+00000c80: 6e74 2e73 7472 6970 2829 0d0a 2020 2020  nt.strip()..    
+00000c90: 2020 2020 746f 6b65 6e73 5f75 7365 6420      tokens_used 
+00000ca0: 3d20 7265 7370 6f6e 7365 2e75 7361 6765  = response.usage
+00000cb0: 2e74 6f74 616c 5f74 6f6b 656e 730d 0a0d  .total_tokens...
+00000cc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000cd0: 636f 6e74 656e 742c 2074 6f6b 656e 735f  content, tokens_
+00000ce0: 7573 6564 0d0a 2020 2020 0d0a 2020 2020  used..    ..    
+00000cf0: 2320 4675 6e63 7469 6f6e 2074 6f20 7361  # Function to sa
+00000d00: 6e69 7469 7a65 2074 6865 206f 7574 7075  nitize the outpu
+00000d10: 7420 6672 6f6d 2074 6865 204c 4c4d 0d0a  t from the LLM..
+00000d20: 2020 2020 6465 6620 5f65 7874 7261 6374      def _extract
+00000d30: 5f63 6f64 6528 7365 6c66 2c72 6573 706f  _code(self,respo
+00000d40: 6e73 653a 2073 7472 2c20 7365 7061 7261  nse: str, separa
+00000d50: 746f 723a 2073 7472 203d 2022 6060 6022  tor: str = "```"
+00000d60: 2920 2d3e 2073 7472 3a0d 0a0d 0a20 2020  ) -> str:....   
+00000d70: 2020 2020 2023 2044 6566 696e 6520 6120       # Define a 
+00000d80: 626c 6163 6b6c 6973 7420 6f66 2050 7974  blacklist of Pyt
+00000d90: 686f 6e20 6b65 7977 6f72 6473 2061 6e64  hon keywords and
+00000da0: 2066 756e 6374 696f 6e73 2074 6861 7420   functions that 
+00000db0: 6172 6520 6e6f 7420 616c 6c6f 7765 640d  are not allowed.
+00000dc0: 0a20 2020 2020 2020 2062 6c61 636b 6c69  .        blackli
+00000dd0: 7374 203d 205b 276f 7327 2c27 7375 6270  st = ['os','subp
+00000de0: 726f 6365 7373 272c 2773 7973 272c 2765  rocess','sys','e
+00000df0: 7661 6c27 2c27 6578 6563 272c 2766 696c  val','exec','fil
+00000e00: 6527 2c27 736f 636b 6574 272c 2775 726c  e','socket','url
+00000e10: 6c69 6227 2c0d 0a20 2020 2020 2020 2020  lib',..         
+00000e20: 2020 2020 2020 2020 2020 2027 7368 7574             'shut
+00000e30: 696c 272c 2770 6963 6b6c 6527 2c27 6374  il','pickle','ct
+00000e40: 7970 6573 272c 276d 756c 7469 7072 6f63  ypes','multiproc
+00000e50: 6573 7369 6e67 272c 2774 656d 7066 696c  essing','tempfil
+00000e60: 6527 2c27 676c 6f62 272c 2763 6f64 6527  e','glob','code'
+00000e70: 2c27 7074 7927 2c27 636f 6d6d 616e 6473  ,'pty','commands
+00000e80: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00000e90: 2020 2020 2020 2020 2772 6571 7565 7374          'request
+00000ea0: 7327 2c27 6367 6927 2c27 6367 6974 6227  s','cgi','cgitb'
+00000eb0: 2c27 786d 6c2e 6574 7265 652e 456c 656d  ,'xml.etree.Elem
+00000ec0: 656e 7454 7265 6527 2c27 6275 696c 7469  entTree','builti
+00000ed0: 6e73 270d 0a20 2020 2020 2020 2020 2020  ns'..           
+00000ee0: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00000ef0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+00000f00: 5365 6172 6368 2066 6f72 2061 2070 6174  Search for a pat
+00000f10: 7465 726e 2062 6574 7765 656e 203c 7265  tern between <re
+00000f20: 666c 6563 7469 6f6e 3e20 616e 6420 3c2f  flection> and </
+00000f30: 7265 666c 6563 7469 6f6e 3e20 696e 2074  reflection> in t
+00000f40: 6865 2072 6573 706f 6e73 650d 0a20 2020  he response..   
+00000f50: 2020 2020 206d 6174 6368 203d 2072 652e       match = re.
+00000f60: 7365 6172 6368 2872 223c 7265 666c 6563  search(r"<reflec
+00000f70: 7469 6f6e 3e28 2e2a 293c 2f72 6566 6c65  tion>(.*)</refle
+00000f80: 6374 696f 6e3e 222c 2072 6573 706f 6e73  ction>", respons
+00000f90: 652c 2072 652e 444f 5441 4c4c 290d 0a20  e, re.DOTALL).. 
+00000fa0: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
+00000fb0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00000fc0: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
+00000fd0: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
+00000fe0: 2072 6566 6c65 6374 696f 6e20 6265 7477   reflection betw
+00000ff0: 6565 6e20 3c72 6566 6c65 6374 696f 6e3e  een <reflection>
+00001000: 2061 6e64 203c 2f72 6566 6c65 6374 696f   and </reflectio
+00001010: 6e3e 0d0a 2020 2020 2020 2020 2020 2020  n>..            
+00001020: 7265 666c 6563 7469 6f6e 203d 206d 6174  reflection = mat
+00001030: 6368 2e67 726f 7570 2831 290d 0a20 2020  ch.group(1)..   
+00001040: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001050: 2020 2020 2020 2020 7265 666c 6563 7469          reflecti
+00001060: 6f6e 203d 2022 220d 0a0d 0a20 2020 2020  on = ""....     
+00001070: 2020 2023 2053 6561 7263 6820 666f 7220     # Search for 
+00001080: 6120 7061 7474 6572 6e20 6265 7477 6565  a pattern betwee
+00001090: 6e20 3c66 6c6f 773e 2061 6e64 203c 2f66  n <flow> and </f
+000010a0: 6c6f 773e 2069 6e20 7468 6520 7265 7370  low> in the resp
+000010b0: 6f6e 7365 0d0a 2020 2020 2020 2020 6d61  onse..        ma
+000010c0: 7463 6820 3d20 7265 2e73 6561 7263 6828  tch = re.search(
+000010d0: 7222 3c66 6c6f 773e 282e 2a29 3c2f 666c  r"<flow>(.*)</fl
+000010e0: 6f77 3e22 2c20 7265 7370 6f6e 7365 2c20  ow>", response, 
+000010f0: 7265 2e44 4f54 414c 4c29 0d0a 2020 2020  re.DOTALL)..    
+00001100: 2020 2020 6966 206d 6174 6368 3a0d 0a20      if match:.. 
+00001110: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00001120: 6120 6d61 7463 6820 6973 2066 6f75 6e64  a match is found
+00001130: 2c20 6578 7472 6163 7420 7468 6520 7265  , extract the re
+00001140: 666c 6563 7469 6f6e 2062 6574 7765 656e  flection between
+00001150: 203c 7265 666c 6563 7469 6f6e 3e20 616e   <reflection> an
+00001160: 6420 3c2f 7265 666c 6563 7469 6f6e 3e0d  d </reflection>.
+00001170: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
+00001180: 7720 3d20 6d61 7463 682e 6772 6f75 7028  w = match.group(
+00001190: 3129 0d0a 2020 2020 2020 2020 656c 7365  1)..        else
+000011a0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+000011b0: 6c6f 7720 3d20 2222 0d0a 0d0a 2020 2020  low = ""....    
+000011c0: 2020 2020 2320 5365 6172 6368 2066 6f72      # Search for
+000011d0: 2061 2070 6174 7465 726e 2062 6574 7765   a pattern betwe
+000011e0: 656e 203c 636f 6465 3e20 616e 6420 3c2f  en <code> and </
+000011f0: 636f 6465 3e20 696e 2074 6865 2065 7874  code> in the ext
+00001200: 7261 6374 6564 2063 6f64 650d 0a20 2020  racted code..   
+00001210: 2020 2020 206d 6174 6368 203d 2072 652e       match = re.
+00001220: 7365 6172 6368 2872 223c 636f 6465 3e28  search(r"<code>(
+00001230: 2e2a 293c 2f63 6f64 653e 222c 2072 6573  .*)</code>", res
+00001240: 706f 6e73 652c 2072 652e 444f 5441 4c4c  ponse, re.DOTALL
+00001250: 290d 0a20 2020 2020 2020 2069 6620 6d61  )..        if ma
+00001260: 7463 683a 0d0a 2020 2020 2020 2020 2020  tch:..          
+00001270: 2020 2320 4966 2061 206d 6174 6368 2069    # If a match i
+00001280: 7320 666f 756e 642c 2065 7874 7261 6374  s found, extract
+00001290: 2074 6865 2063 6f64 6520 6265 7477 6565   the code betwee
+000012a0: 6e20 3c63 6f64 653e 2061 6e64 203c 2f63  n <code> and </c
+000012b0: 6f64 653e 0d0a 2020 2020 2020 2020 2020  ode>..          
+000012c0: 2020 636f 6465 203d 206d 6174 6368 2e67    code = match.g
+000012d0: 726f 7570 2831 290d 0a20 2020 2020 2020  roup(1)..       
+000012e0: 2020 2020 2023 2049 6620 7468 6520 7265       # If the re
+000012f0: 7370 6f6e 7365 2063 6f6e 7461 696e 7320  sponse contains 
+00001300: 7468 6520 7365 7061 7261 746f 722c 2065  the separator, e
+00001310: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
+00001320: 626c 6f63 6b20 6265 7477 6565 6e20 7468  block between th
+00001330: 6520 7365 7061 7261 746f 7273 0d0a 2020  e separators..  
+00001340: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00001350: 2863 6f64 652e 7370 6c69 7428 7365 7061  (code.split(sepa
+00001360: 7261 746f 7229 2920 3e20 313a 0d0a 2020  rator)) > 1:..  
+00001370: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001380: 6465 203d 2063 6f64 652e 7370 6c69 7428  de = code.split(
+00001390: 7365 7061 7261 746f 7229 5b31 5d0d 0a0d  separator)[1]...
+000013a0: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+000013b0: 6520 7265 7370 6f6e 7365 2063 6f6e 7461  e response conta
+000013c0: 696e 7320 7468 6520 7365 7061 7261 746f  ins the separato
+000013d0: 722c 2065 7874 7261 6374 2074 6865 2063  r, extract the c
+000013e0: 6f64 6520 626c 6f63 6b20 6265 7477 6565  ode block betwee
+000013f0: 6e20 7468 6520 7365 7061 7261 746f 7273  n the separators
+00001400: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00001410: 2872 6573 706f 6e73 652e 7370 6c69 7428  (response.split(
+00001420: 7365 7061 7261 746f 7229 2920 3e20 313a  separator)) > 1:
+00001430: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00001440: 6465 203d 2072 6573 706f 6e73 652e 7370  de = response.sp
+00001450: 6c69 7428 7365 7061 7261 746f 7229 5b31  lit(separator)[1
+00001460: 5d0d 0a20 2020 2020 2020 2020 2020 200d  ]..            .
+00001470: 0a20 2020 2020 2020 2023 2052 656d 6f76  .        # Remov
+00001480: 6520 7468 6520 2270 7974 686f 6e22 206f  e the "python" o
+00001490: 7220 2270 7922 2070 7265 6669 7820 6966  r "py" prefix if
+000014a0: 2070 7265 7365 6e74 0d0a 2020 2020 2020   present..      
+000014b0: 2020 6966 2072 652e 6d61 7463 6828 7222    if re.match(r"
+000014c0: 5e28 7079 7468 6f6e 7c70 7929 222c 2063  ^(python|py)", c
+000014d0: 6f64 6529 3a0d 0a20 2020 2020 2020 2020  ode):..         
+000014e0: 2020 2063 6f64 6520 3d20 7265 2e73 7562     code = re.sub
+000014f0: 2872 225e 2870 7974 686f 6e7c 7079 2922  (r"^(python|py)"
+00001500: 2c20 2222 2c20 636f 6465 290d 0a20 2020  , "", code)..   
+00001510: 2020 2020 2023 2049 6620 7468 6520 636f       # If the co
+00001520: 6465 2069 7320 6265 7477 6565 6e20 7369  de is between si
+00001530: 6e67 6c65 2062 6163 6b74 6963 6b73 2c20  ngle backticks, 
+00001540: 6578 7472 6163 7420 7468 6520 636f 6465  extract the code
+00001550: 2062 6574 7765 656e 2074 6865 6d0d 0a20   between them.. 
+00001560: 2020 2020 2020 2069 6620 7265 2e6d 6174         if re.mat
+00001570: 6368 2872 225e 602e 2a60 2422 2c20 636f  ch(r"^`.*`$", co
+00001580: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
+00001590: 2020 636f 6465 203d 2072 652e 7375 6228    code = re.sub(
+000015a0: 7222 5e60 282e 2a29 6024 222c 2072 225c  r"^`(.*)`$", r"\
+000015b0: 3122 2c20 636f 6465 290d 0a0d 0a20 2020  1", code)....   
+000015c0: 2020 2020 2023 2052 656d 6f76 6520 616e       # Remove an
+000015d0: 7920 696e 7374 616e 6365 7320 6f66 2022  y instances of "
+000015e0: 6466 203d 2070 642e 7265 6164 5f63 7376  df = pd.read_csv
+000015f0: 2827 6669 6c65 6e61 6d65 2e63 7376 2729  ('filename.csv')
+00001600: 2220 6672 6f6d 2074 6865 2063 6f64 650d  " from the code.
+00001610: 0a20 2020 2020 2020 2063 6f64 6520 3d20  .        code = 
+00001620: 7265 2e73 7562 2872 2264 665c 732a 3d5c  re.sub(r"df\s*=\
+00001630: 732a 7064 5c2e 7265 6164 5f63 7376 5c28  s*pd\.read_csv\(
+00001640: 272e 2a3f 275c 2922 2c20 2222 2c20 636f  '.*?'\)", "", co
+00001650: 6465 290d 0a20 2020 2020 2020 200d 0a20  de)..        .. 
+00001660: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
+00001670: 616e 7920 6f63 6375 7272 656e 6365 7320  any occurrences 
+00001680: 6f66 2064 6620 3d20 7064 2e44 6174 6146  of df = pd.DataF
+00001690: 7261 6d65 2829 2077 6974 6820 616e 7920  rame() with any 
+000016a0: 6e75 6d62 6572 206f 6620 6368 6172 6163  number of charac
+000016b0: 7465 7273 2069 6e73 6964 6520 7468 6520  ters inside the 
+000016c0: 7061 7265 6e74 6865 7365 732e 0d0a 2020  parentheses...  
+000016d0: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
+000016e0: 7375 6228 7222 6466 5c73 2a3d 5c73 2a70  sub(r"df\s*=\s*p
+000016f0: 645c 2e44 6174 6146 7261 6d65 5c28 2e2a  d\.DataFrame\(.*
+00001700: 3f5c 2922 2c20 2222 2c20 636f 6465 290d  ?\)", "", code).
+00001710: 0a0d 0a20 2020 2020 2020 2023 2044 6566  ...        # Def
+00001720: 696e 6520 7468 6520 7265 6775 6c61 7220  ine the regular 
+00001730: 6578 7072 6573 7369 6f6e 2070 6174 7465  expression patte
+00001740: 726e 2074 6f20 6d61 7463 6820 7468 6520  rn to match the 
+00001750: 626c 6163 6b6c 6973 7420 6974 656d 730d  blacklist items.
+00001760: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+00001770: 203d 2072 225e 282e 2a5c 6228 2220 2b20   = r"^(.*\b(" + 
+00001780: 227c 222e 6a6f 696e 2862 6c61 636b 6c69  "|".join(blackli
+00001790: 7374 2920 2b20 7222 295c 622e 2a29 2422  st) + r")\b.*)$"
+000017a0: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
+000017b0: 706c 6163 6520 7468 6520 626c 6163 6b6c  place the blackl
+000017c0: 6973 7420 6974 656d 7320 7769 7468 2063  ist items with c
+000017d0: 6f6d 6d65 6e74 730d 0a20 2020 2020 2020  omments..       
+000017e0: 2063 6f64 6520 3d20 7265 2e73 7562 2870   code = re.sub(p
+000017f0: 6174 7465 726e 2c20 7222 2320 6e6f 7420  attern, r"# not 
+00001800: 616c 6c6f 7765 6420 5c31 222c 2063 6f64  allowed \1", cod
+00001810: 652c 2066 6c61 6773 3d72 652e 4d55 4c54  e, flags=re.MULT
+00001820: 494c 494e 4529 0d0a 0d0a 2020 2020 2020  ILINE)....      
+00001830: 2020 2320 5265 7475 726e 2074 6865 2063    # Return the c
+00001840: 6c65 616e 6564 2061 6e64 2065 7874 7261  leaned and extra
+00001850: 6374 6564 2063 6f64 650d 0a20 2020 2020  cted code..     
+00001860: 2020 2072 6574 7572 6e20 636f 6465 2e73     return code.s
+00001870: 7472 6970 2829 2c20 7265 666c 6563 7469  trip(), reflecti
+00001880: 6f6e 2e73 7472 6970 2829 2c20 666c 6f77  on.strip(), flow
+00001890: 2e73 7472 6970 2829 0d0a 0d0a 2020 2020  .strip()....    
+000018a0: 6465 6620 7064 5f61 6765 6e74 5f63 6f6e  def pd_agent_con
+000018b0: 7665 7273 6528 7365 6c66 2c20 7175 6573  verse(self, ques
+000018c0: 7469 6f6e 3d4e 6f6e 6529 3a0d 0a20 2020  tion=None):..   
+000018d0: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
+000018e0: 6520 7468 6520 6d65 7373 6167 6573 206c  e the messages l
+000018f0: 6973 7420 7769 7468 2061 2073 7973 7465  ist with a syste
+00001900: 6d20 6d65 7373 6167 6520 636f 6e74 6169  m message contai
+00001910: 6e69 6e67 2074 6865 2074 6173 6b20 7072  ning the task pr
+00001920: 6f6d 7074 0d0a 2020 2020 2020 2020 6d65  ompt..        me
+00001930: 7373 6167 6573 203d 205b 7b22 726f 6c65  ssages = [{"role
+00001940: 223a 2022 7379 7374 656d 222c 2022 636f  ": "system", "co
+00001950: 6e74 656e 7422 3a20 7365 6c66 2e74 6173  ntent": self.tas
+00001960: 6b2e 666f 726d 6174 2873 656c 662e 6466  k.format(self.df
+00001970: 5f68 6561 642c 2022 2229 7d5d 0d0a 0d0a  _head, "")}]....
+00001980: 2020 2020 2020 2020 2320 4675 6e63 7469          # Functi
+00001990: 6f6e 2074 6f20 6469 7370 6c61 7920 7265  on to display re
+000019a0: 7375 6c74 7320 6e69 6365 6c79 0d0a 2020  sults nicely..  
+000019b0: 2020 2020 2020 6465 6620 6469 7370 6c61        def displa
+000019c0: 795f 7265 7375 6c74 7328 616e 7377 6572  y_results(answer
+000019d0: 2c20 636f 6465 2c20 7265 666c 6563 7469  , code, reflecti
+000019e0: 6f6e 2c20 666c 6f77 2c20 746f 7461 6c5f  on, flow, total_
+000019f0: 746f 6b65 6e73 5f75 7365 645f 7375 6d29  tokens_used_sum)
+00001a00: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00001a10: 6620 2769 7079 6b65 726e 656c 2720 696e  f 'ipykernel' in
+00001a20: 2073 7973 2e6d 6f64 756c 6573 3a0d 0a20   sys.modules:.. 
+00001a30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001a40: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
+00001a50: 6b20 6f72 2069 7079 7468 6f6e 0d0a 2020  k or ipython..  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001a70: 7370 6c61 7928 4854 4d4c 2866 273c 703e  splay(HTML(f'<p>
+00001a80: 3c62 2073 7479 6c65 3d22 636f 6c6f 723a  <b style="color:
+00001a90: 626c 7565 3b22 3e41 6e73 7765 723a 3c2f  blue;">Answer:</
+00001aa0: 623e 3c62 723e 3c70 7265 2073 7479 6c65  b><br><pre style
+00001ab0: 3d22 636f 6c6f 723a 626c 6163 6b3b 223e  ="color:black;">
+00001ac0: 3c62 3e7b 616e 7377 6572 7d3c 2f62 3e3c  <b>{answer}</b><
+00001ad0: 2f70 7265 3e3c 2f70 3e3c 6272 3e27 2929  /pre></p><br>'))
+00001ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001af0: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
+00001b00: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
+00001b10: 6c6f 723a 626c 7565 3b22 3e43 6f64 653a  lor:blue;">Code:
+00001b20: 3c2f 623e 3c62 723e 3c70 7265 2073 7479  </b><br><pre sty
+00001b30: 6c65 3d22 636f 6c6f 723a 2335 3535 3535  le="color:#55555
+00001b40: 353b 223e 7b63 6f64 657d 3c2f 7072 653e  5;">{code}</pre>
+00001b50: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00001b60: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00001b70: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
+00001b80: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
+00001b90: 6c75 653b 223e 5468 6f75 6768 7473 3a3c  lue;">Thoughts:<
+00001ba0: 2f62 3e3c 6272 3e3c 6220 7374 796c 653d  /b><br><b style=
+00001bb0: 2263 6f6c 6f72 3a62 6c61 636b 3b22 3e7b  "color:black;">{
+00001bc0: 7265 666c 6563 7469 6f6e 7d3c 2f62 3e3c  reflection}</b><
+00001bd0: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
+00001be0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00001bf0: 6c61 7928 4854 4d4c 2866 273c 703e 3c62  lay(HTML(f'<p><b
+00001c00: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
+00001c10: 7565 3b22 3e41 6e61 6c79 7369 7320 466c  ue;">Analysis Fl
+00001c20: 6f77 3a3c 2f62 3e3c 6272 3e3c 696d 6720  ow:</b><br><img 
+00001c30: 7372 633d 227b 7365 6c66 2e6d 6d28 666c  src="{self.mm(fl
+00001c40: 6f77 297d 2220 616c 743d 2241 6e61 6c79  ow)}" alt="Analy
+00001c50: 7369 7320 466c 6f77 223e 3c2f 696d 673e  sis Flow"></img>
+00001c60: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00001c70: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00001c80: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
+00001c90: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
+00001ca0: 6c75 653b 223e 546f 7461 6c20 546f 6b65  lue;">Total Toke
+00001cb0: 6e73 2055 7365 643a 3c2f 623e 3c62 723e  ns Used:</b><br>
+00001cc0: 3c73 7061 6e20 7374 796c 653d 2263 6f6c  <span style="col
+00001cd0: 6f72 3a62 6c61 636b 3b22 3e7b 746f 7461  or:black;">{tota
+00001ce0: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
+00001cf0: 6d7d 3c2f 7370 616e 3e3c 2f70 3e3c 6272  m}</span></p><br
+00001d00: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
+00001d10: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00001d20: 2020 2020 2020 2020 2023 204f 7468 6572           # Other
+00001d30: 2065 6e76 6972 6f6e 6d65 6e74 2028 6c69   environment (li
+00001d40: 6b65 2074 6572 6d69 6e61 6c29 0d0a 2020  ke terminal)..  
+00001d50: 2020 2020 2020 2020 2020 2020 2020 6370                cp
+00001d60: 7269 6e74 2866 225c 6e41 6e73 7765 723a  rint(f"\nAnswer:
+00001d70: 5c6e 7b61 6e73 7765 727d 5c6e 222c 2027  \n{answer}\n", '
+00001d80: 6772 6565 6e27 2c20 6174 7472 733d 5b27  green', attrs=['
+00001d90: 626f 6c64 275d 290d 0a20 2020 2020 2020  bold'])..       
+00001da0: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
+00001db0: 6622 436f 6465 3a5c 6e7b 636f 6465 7d5c  f"Code:\n{code}\
+00001dc0: 6e22 2c20 2767 7265 656e 272c 2061 7474  n", 'green', att
+00001dd0: 7273 3d5b 2762 6f6c 6427 5d29 0d0a 2020  rs=['bold'])..  
+00001de0: 2020 2020 2020 2020 2020 2020 2020 6370                cp
+00001df0: 7269 6e74 2866 2254 686f 7567 6874 733a  rint(f"Thoughts:
+00001e00: 5c6e 7b72 6566 6c65 6374 696f 6e7d 5c6e  \n{reflection}\n
+00001e10: 222c 2027 6772 6565 6e27 2c20 6174 7472  ", 'green', attr
+00001e20: 733d 5b27 626f 6c64 275d 290d 0a20 2020  s=['bold'])..   
+00001e30: 2020 2020 2020 2020 2020 2020 2063 7072               cpr
+00001e40: 696e 7428 6622 546f 7461 6c20 746f 6b65  int(f"Total toke
+00001e50: 6e73 2075 7365 643a 5c6e 7b74 6f74 616c  ns used:\n{total
+00001e60: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+00001e70: 7d5c 6e22 2c20 2779 656c 6c6f 7727 2c20  }\n", 'yellow', 
+00001e80: 6174 7472 733d 5b27 626f 6c64 275d 290d  attrs=['bold']).
+00001e90: 0a0d 0a20 2020 2020 2020 2023 2049 6620  ...        # If 
+00001ea0: 6120 7175 6573 7469 6f6e 2069 7320 7072  a question is pr
+00001eb0: 6f76 6964 6564 2c20 736b 6970 2074 6865  ovided, skip the
+00001ec0: 2069 6e70 7574 2070 726f 6d70 740d 0a20   input prompt.. 
+00001ed0: 2020 2020 2020 2069 6620 7175 6573 7469         if questi
+00001ee0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0d  on is not None:.
+00001ef0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00001f00: 616c 6c20 7468 6520 7064 5f61 6765 6e74  all the pd_agent
+00001f10: 206d 6574 686f 6420 7769 7468 2074 6865   method with the
+00001f20: 2075 7365 7227 7320 7175 6573 7469 6f6e   user's question
+00001f30: 2c20 7468 6520 6d65 7373 6167 6573 206c  , the messages l
+00001f40: 6973 742c 2061 6e64 2074 6865 2064 6174  ist, and the dat
+00001f50: 6166 7261 6d65 0d0a 2020 2020 2020 2020  aframe..        
+00001f60: 2020 2020 616e 7377 6572 2c20 636f 6465      answer, code
+00001f70: 2c20 7265 666c 6563 7469 6f6e 2c20 666c  , reflection, fl
+00001f80: 6f77 2c20 746f 7461 6c5f 746f 6b65 6e73  ow, total_tokens
+00001f90: 5f75 7365 645f 7375 6d20 3d20 7365 6c66  _used_sum = self
+00001fa0: 2e70 645f 6167 656e 7428 7175 6573 7469  .pd_agent(questi
+00001fb0: 6f6e 2c20 6d65 7373 6167 6573 2c20 7365  on, messages, se
+00001fc0: 6c66 2e64 6629 0d0a 2020 2020 2020 2020  lf.df)..        
+00001fd0: 2020 2020 6469 7370 6c61 795f 7265 7375      display_resu
+00001fe0: 6c74 7328 616e 7377 6572 2c20 636f 6465  lts(answer, code
+00001ff0: 2c20 7265 666c 6563 7469 6f6e 2c20 666c  , reflection, fl
+00002000: 6f77 2c20 746f 7461 6c5f 746f 6b65 6e73  ow, total_tokens
+00002010: 5f75 7365 645f 7375 6d29 0d0a 2020 2020  _used_sum)..    
+00002020: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00002030: 0d0a 2020 2020 2020 2020 2320 5374 6172  ..        # Star
+00002040: 7420 616e 2069 6e66 696e 6974 6520 6c6f  t an infinite lo
+00002050: 6f70 2074 6f20 6b65 6570 2061 736b 696e  op to keep askin
+00002060: 6720 7468 6520 7573 6572 2066 6f72 2071  g the user for q
+00002070: 7565 7374 696f 6e73 0d0a 2020 2020 2020  uestions..      
+00002080: 2020 7768 696c 6520 5472 7565 3a0d 0a20    while True:.. 
+00002090: 2020 2020 2020 2020 2020 2023 2050 726f             # Pro
+000020a0: 6d70 7420 7468 6520 7573 6572 2074 6f20  mpt the user to 
+000020b0: 656e 7465 7220 6120 7175 6573 7469 6f6e  enter a question
+000020c0: 206f 7220 7479 7065 2027 6578 6974 2720   or type 'exit' 
+000020d0: 746f 2071 7569 740d 0a20 2020 2020 2020  to quit..       
+000020e0: 2020 2020 2069 6620 2769 7079 6b65 726e       if 'ipykern
+000020f0: 656c 2720 696e 2073 7973 2e6d 6f64 756c  el' in sys.modul
+00002100: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00002110: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
+00002120: 4c28 273c 6220 7374 796c 653d 2263 6f6c  L('<b style="col
+00002130: 6f72 3a62 6c75 653b 223e 456e 7465 7220  or:blue;">Enter 
+00002140: 796f 7572 2071 7565 7374 696f 6e20 6f72  your question or
+00002150: 2074 7970 6520 5c27 6578 6974 5c27 2074   type \'exit\' t
+00002160: 6f20 7175 6974 3a3c 2f62 3e27 2929 0d0a  o quit:</b>'))..
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 7175 6573 7469 6f6e 203d 2069 6e70 7574  question = input
+00002190: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000021a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000021b0: 2020 2020 2020 2063 7072 696e 7428 225c         cprint("\
+000021c0: 6e45 6e74 6572 2079 6f75 7220 7175 6573  nEnter your ques
+000021d0: 7469 6f6e 206f 7220 7479 7065 2027 6578  tion or type 'ex
+000021e0: 6974 2720 746f 2071 7569 743a 222c 2027  it' to quit:", '
+000021f0: 626c 7565 272c 2061 7474 7273 3d5b 2762  blue', attrs=['b
+00002200: 6f6c 6427 5d29 0d0a 2020 2020 2020 2020  old'])..        
+00002210: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
+00002220: 203d 2069 6e70 7574 2829 0d0a 0d0a 2020   = input()....  
+00002230: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
+00002240: 6865 2075 7365 7220 7479 7065 7320 2765  he user types 'e
+00002250: 7869 7427 2c20 6272 6561 6b20 6f75 7420  xit', break out 
+00002260: 6f66 2074 6865 206c 6f6f 700d 0a20 2020  of the loop..   
+00002270: 2020 2020 2020 2020 2069 6620 7175 6573           if ques
+00002280: 7469 6f6e 2e73 7472 6970 2829 2e6c 6f77  tion.strip().low
+00002290: 6572 2829 203d 3d20 2765 7869 7427 3a0d  er() == 'exit':.
+000022a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022b0: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+000022c0: 2020 2020 2020 2320 4361 6c6c 2074 6865        # Call the
+000022d0: 2070 645f 6167 656e 7420 6d65 7468 6f64   pd_agent method
+000022e0: 2077 6974 6820 7468 6520 7573 6572 2773   with the user's
+000022f0: 2071 7565 7374 696f 6e2c 2074 6865 206d   question, the m
+00002300: 6573 7361 6765 7320 6c69 7374 2c20 616e  essages list, an
+00002310: 6420 7468 6520 6461 7461 6672 616d 650d  d the dataframe.
+00002320: 0a20 2020 2020 2020 2020 2020 2061 6e73  .            ans
+00002330: 7765 722c 2063 6f64 652c 2072 6566 6c65  wer, code, refle
+00002340: 6374 696f 6e2c 2066 6c6f 772c 2074 6f74  ction, flow, tot
+00002350: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+00002360: 756d 203d 2073 656c 662e 7064 5f61 6765  um = self.pd_age
+00002370: 6e74 2871 7565 7374 696f 6e2c 206d 6573  nt(question, mes
+00002380: 7361 6765 732c 2073 656c 662e 6466 290d  sages, self.df).
+00002390: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+000023a0: 706c 6179 5f72 6573 756c 7473 2861 6e73  play_results(ans
+000023b0: 7765 722c 2063 6f64 652c 2072 6566 6c65  wer, code, refle
+000023c0: 6374 696f 6e2c 666c 6f77 2c20 746f 7461  ction,flow, tota
+000023d0: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
+000023e0: 6d29 0d0a 0d0a 2020 2020 6465 6620 7064  m)....    def pd
+000023f0: 5f61 6765 6e74 2873 656c 662c 2071 7565  _agent(self, que
+00002400: 7374 696f 6e2c 206d 6573 7361 6765 732c  stion, messages,
+00002410: 2064 663d 4e6f 6e65 293a 0d0a 2020 2020   df=None):..    
+00002420: 2020 2020 2320 4164 6420 6120 7573 6572      # Add a user
+00002430: 206d 6573 7361 6765 2077 6974 6820 7468   message with th
+00002440: 6520 7570 6461 7465 6420 7461 736b 2070  e updated task p
+00002450: 726f 6d70 7420 746f 2074 6865 206d 6573  rompt to the mes
+00002460: 7361 6765 7320 6c69 7374 0d0a 2020 2020  sages list..    
+00002470: 2020 2020 6d65 7373 6167 6573 2e61 7070      messages.app
+00002480: 656e 6428 7b22 726f 6c65 223a 2022 7573  end({"role": "us
+00002490: 6572 222c 2022 636f 6e74 656e 7422 3a20  er", "content": 
+000024a0: 7365 6c66 2e74 6173 6b2e 666f 726d 6174  self.task.format
+000024b0: 2873 656c 662e 6466 5f68 6561 642c 2071  (self.df_head, q
+000024c0: 7565 7374 696f 6e29 7d29 0d0a 0d0a 2020  uestion)})....  
+000024d0: 2020 2020 2020 6966 2027 6970 796b 6572        if 'ipyker
+000024e0: 6e65 6c27 2069 6e20 7379 732e 6d6f 6475  nel' in sys.modu
+000024f0: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
+00002500: 2020 2320 4a75 7079 7465 7220 6e6f 7465    # Jupyter note
+00002510: 626f 6f6b 206f 7220 6970 7974 686f 6e0d  book or ipython.
+00002520: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00002530: 706c 6179 2848 544d 4c28 6627 3c70 2073  play(HTML(f'<p s
+00002540: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+00002550: 6e74 613b 223e 5c6e 5573 696e 6720 4d6f  nta;">\nUsing Mo
+00002560: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c  del: {self.llm}<
+00002570: 2f70 3e27 2929 0d0a 2020 2020 2020 2020  /p>'))..        
+00002580: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+00002590: 2866 273c 703e 3c62 2073 7479 6c65 3d22  (f'<p><b style="
+000025a0: 636f 6c6f 723a 6d61 6765 6e74 613b 223e  color:magenta;">
+000025b0: 5072 6f63 6573 7369 6e67 2079 6f75 7220  Processing your 
+000025c0: 7265 7175 6573 742c 2070 6c65 6173 6520  request, please 
+000025d0: 7761 6974 2e2e 2e3c 2f62 3e3c 2f70 3e3c  wait...</b></p><
+000025e0: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
+000025f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00002600: 2020 2023 204f 7468 6572 2065 6e76 6972     # Other envir
+00002610: 6f6e 6d65 6e74 2028 6c69 6b65 2074 6572  onment (like ter
+00002620: 6d69 6e61 6c29 0d0a 2020 2020 2020 2020  minal)..        
+00002630: 2020 2020 7072 696e 7428 636f 6c6f 7265      print(colore
+00002640: 6428 6622 5c6e 5573 696e 6720 4d6f 6465  d(f"\nUsing Mode
+00002650: 6c3a 207b 7365 6c66 2e6c 6c6d 7d22 2c20  l: {self.llm}", 
+00002660: 226d 6167 656e 7461 2229 290d 0a20 2020  "magenta"))..   
+00002670: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
+00002680: 6622 5c6e 3e20 5072 6f63 6573 7369 6e67  f"\n> Processing
+00002690: 2079 6f75 7220 7265 7175 6573 742c 2070   your request, p
+000026a0: 6c65 6173 6520 7761 6974 2e2e 2e5c 6e22  lease wait...\n"
+000026b0: 2c20 276d 6167 656e 7461 272c 2061 7474  , 'magenta', att
+000026c0: 7273 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a  rs=['bold'])....
+000026d0: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
+000026e0: 6865 204f 7065 6e41 4920 4150 4920 616e  he OpenAI API an
+000026f0: 6420 6861 6e64 6c65 2072 6174 6520 6c69  d handle rate li
+00002700: 6d69 7420 6572 726f 7273 0d0a 2020 2020  mit errors..    
+00002710: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002720: 2020 2020 2020 6c6c 6d5f 7265 7370 6f6e        llm_respon
+00002730: 7365 2c20 746f 6b65 6e73 5f75 7365 6420  se, tokens_used 
+00002740: 3d20 7365 6c66 2e6c 6c6d 5f63 616c 6c28  = self.llm_call(
+00002750: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
+00002760: 2020 2065 7863 6570 7420 6f70 656e 6169     except openai
+00002770: 2e65 7272 6f72 2e52 6174 654c 696d 6974  .error.RateLimit
+00002780: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+00002790: 2020 2020 7072 696e 7428 0d0a 2020 2020      print(..    
+000027a0: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+000027b0: 204f 7065 6e41 4920 4150 4920 7261 7465   OpenAI API rate
+000027c0: 206c 696d 6974 2068 6173 2062 6565 6e20   limit has been 
+000027d0: 6578 6365 6564 6564 2e20 5761 6974 696e  exceeded. Waitin
+000027e0: 6720 3130 2073 6563 6f6e 6473 2061 6e64  g 10 seconds and
+000027f0: 2074 7279 696e 6720 6167 6169 6e2e 220d   trying again.".
+00002800: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00002810: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00002820: 2e73 6c65 6570 2831 3029 0d0a 2020 2020  .sleep(10)..    
+00002830: 2020 2020 2020 2020 6c6c 6d5f 7265 7370          llm_resp
+00002840: 6f6e 7365 2c20 746f 6b65 6e73 5f75 7365  onse, tokens_use
+00002850: 6420 3d20 7365 6c66 2e6c 6c6d 5f63 616c  d = self.llm_cal
+00002860: 6c28 6d65 7373 6167 6573 290d 0a0d 0a20  l(messages).... 
+00002870: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+00002880: 2074 6865 2063 6f64 6520 6672 6f6d 2074   the code from t
+00002890: 6865 2041 5049 2072 6573 706f 6e73 650d  he API response.
+000028a0: 0a20 2020 2020 2020 2063 6f64 652c 7265  .        code,re
+000028b0: 666c 6563 7469 6f6e 2c66 6c6f 7720 3d20  flection,flow = 
+000028c0: 7365 6c66 2e5f 6578 7472 6163 745f 636f  self._extract_co
+000028d0: 6465 286c 6c6d 5f72 6573 706f 6e73 6529  de(llm_response)
+000028e0: 0d0a 0d0a 2020 2020 2020 2020 2320 5570  ....        # Up
+000028f0: 6461 7465 2074 6865 2074 6f74 616c 2074  date the total t
+00002900: 6f6b 656e 7320 7573 6564 0d0a 2020 2020  okens used..    
+00002910: 2020 2020 7365 6c66 2e74 6f74 616c 5f74      self.total_t
+00002920: 6f6b 656e 735f 7573 6564 2e61 7070 656e  okens_used.appen
+00002930: 6428 746f 6b65 6e73 5f75 7365 6429 0d0a  d(tokens_used)..
+00002940: 2020 2020 2020 2020 746f 7461 6c5f 746f          total_to
+00002950: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
+00002960: 7375 6d28 7365 6c66 2e74 6f74 616c 5f74  sum(self.total_t
+00002970: 6f6b 656e 735f 7573 6564 290d 0a0d 0a20  okens_used).... 
+00002980: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+00002990: 697a 6520 6572 726f 7220 636f 7272 6563  ize error correc
+000029a0: 7469 6f6e 2063 6f75 6e74 6572 0d0a 2020  tion counter..  
+000029b0: 2020 2020 2020 6572 726f 725f 636f 7272        error_corr
+000029c0: 6563 7469 6f6e 7320 3d20 300d 0a0d 0a20  ections = 0.... 
+000029d0: 2020 2020 2020 2023 2053 746f 7265 2074         # Store t
+000029e0: 6865 206f 7269 6769 6e61 6c20 6c6c 6d20  he original llm 
+000029f0: 7661 6c75 650d 0a20 2020 2020 2020 206f  value..        o
+00002a00: 7269 6769 6e61 6c5f 6c6c 6d20 3d20 7365  riginal_llm = se
+00002a10: 6c66 2e6c 6c6d 0d0a 0d0a 2020 2020 2020  lf.llm....      
+00002a20: 2020 2320 5265 6469 7265 6374 2073 7461    # Redirect sta
+00002a30: 6e64 6172 6420 6f75 7470 7574 2074 6f20  ndard output to 
+00002a40: 6120 5374 7269 6e67 494f 2062 7566 6665  a StringIO buffe
+00002a50: 720d 0a20 2020 2020 2020 2077 6974 6820  r..        with 
+00002a60: 7265 6469 7265 6374 5f73 7464 6f75 7428  redirect_stdout(
+00002a70: 696f 2e53 7472 696e 6749 4f28 2929 2061  io.StringIO()) a
+00002a80: 7320 6f75 7470 7574 3a0d 0a20 2020 2020  s output:..     
+00002a90: 2020 2020 2020 2023 2054 7279 2074 6f20         # Try to 
+00002aa0: 6578 6563 7574 6520 7468 6520 636f 6465  execute the code
+00002ab0: 2061 6e64 2068 616e 646c 6520 6572 726f   and handle erro
+00002ac0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
+00002ad0: 7768 696c 6520 6572 726f 725f 636f 7272  while error_corr
+00002ae0: 6563 7469 6f6e 7320 3c20 7365 6c66 2e4d  ections < self.M
+00002af0: 4158 5f45 5252 4f52 5f43 4f52 5245 4354  AX_ERROR_CORRECT
+00002b00: 494f 4e53 3a0d 0a20 2020 2020 2020 2020  IONS:..         
+00002b10: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 206d 6573 7361 6765 732e 6170 7065 6e64   messages.append
+00002b40: 287b 2272 6f6c 6522 3a20 2261 7373 6973  ({"role": "assis
+00002b50: 7461 6e74 222c 2022 636f 6e74 656e 7422  tant", "content"
+00002b60: 3a20 6c6c 6d5f 7265 7370 6f6e 7365 7d29  : llm_response})
+00002b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002b80: 2020 2020 2020 2320 5265 6d6f 7665 2074        # Remove t
+00002b90: 6865 206f 6c64 6573 7420 636f 6e76 6572  he oldest conver
+00002ba0: 7361 7469 6f6e 2066 726f 6d20 7468 6520  sation from the 
+00002bb0: 6d65 7373 6167 6573 206c 6973 740d 0a20  messages list.. 
 00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-00002be0: 7928 4854 4d4c 2827 3c73 7061 6e20 7374  y(HTML('<span st
-00002bf0: 796c 653d 2263 6f6c 6f72 3a20 7265 643b  yle="color: red;
-00002c00: 223e 5377 6974 6368 696e 6720 6d6f 6465  ">Switching mode
-00002c10: 6c20 746f 2067 7074 2d34 2074 6f20 7472  l to gpt-4 to tr
-00002c20: 7920 746f 2069 6d70 726f 7665 2074 6865  y to improve the
-00002c30: 206f 7574 636f 6d65 2e3c 2f73 7061 6e3e   outcome.</span>
-00002c40: 2729 290d 0a20 2020 2020 2020 2020 2020  '))..           
-00002c50: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00002c60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2320 434c 490d 0a20 2020 2020 2020 2020  # CLI..         
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ca0: 2020 2070 7269 6e74 2863 6f6c 6f72 6564     print(colored
-00002cb0: 2827 5377 6974 6368 696e 6720 6d6f 6465  ('Switching mode
-00002cc0: 6c20 746f 2067 7074 2d34 2074 6f20 7472  l to gpt-4 to tr
-00002cd0: 7920 746f 2069 6d70 726f 7665 2074 6865  y to improve the
-00002ce0: 206f 7574 636f 6d65 2e27 2c20 2772 6564   outcome.', 'red
-00002cf0: 2729 290d 0a0d 0a20 2020 2020 2020 2020  '))....         
-00002d00: 2020 2020 2020 2020 2020 2023 2041 7474             # Att
-00002d10: 656d 7074 2074 6f20 636f 7272 6563 7420  empt to correct 
-00002d20: 7468 6520 636f 6465 2061 6e64 2068 616e  the code and han
-00002d30: 646c 6520 7261 7465 206c 696d 6974 2065  dle rate limit e
-00002d40: 7272 6f72 730d 0a20 2020 2020 2020 2020  rrors..         
-00002d50: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00002d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d70: 2020 2020 2020 2020 206c 6c6d 5f72 6573           llm_res
-00002d80: 706f 6e73 652c 2074 6f6b 656e 735f 7573  ponse, tokens_us
-00002d90: 6564 203d 2073 656c 662e 6c6c 6d5f 6361  ed = self.llm_ca
-00002da0: 6c6c 286d 6573 7361 6765 7329 0d0a 2020  ll(messages)..  
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 2020 2020 636f 6465 2c72 6566 6c65        code,refle
-00002dd0: 6374 696f 6e20 3d20 7365 6c66 2e5f 6578  ction = self._ex
-00002de0: 7472 6163 745f 636f 6465 286c 6c6d 5f72  tract_code(llm_r
-00002df0: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
-00002e20: 656e 735f 7573 6564 2e61 7070 656e 6428  ens_used.append(
-00002e30: 746f 6b65 6e73 5f75 7365 6429 0d0a 2020  tokens_used)..  
-00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 2020 2020 2020 746f 7461 6c5f 746f 6b65        total_toke
-00002e60: 6e73 5f75 7365 645f 7375 6d20 3d20 7375  ns_used_sum = su
-00002e70: 6d28 7365 6c66 2e74 6f74 616c 5f74 6f6b  m(self.total_tok
-00002e80: 656e 735f 7573 6564 290d 0a20 2020 2020  ens_used)..     
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002ea0: 7863 6570 7420 6f70 656e 6169 2e65 7272  xcept openai.err
-00002eb0: 6f72 2e52 6174 654c 696d 6974 4572 726f  or.RateLimitErro
-00002ec0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00002ed0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002ee0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f00: 2254 6865 204f 7065 6e41 4920 4150 4920  "The OpenAI API 
-00002f10: 7261 7465 206c 696d 6974 2068 6173 2062  rate limit has b
-00002f20: 6565 6e20 6578 6365 6564 6564 2e20 5761  een exceeded. Wa
-00002f30: 6974 696e 6720 3130 2073 6563 6f6e 6473  iting 10 seconds
-00002f40: 2061 6e64 2074 7279 696e 6720 6167 6169   and trying agai
-00002f50: 6e2e 220d 0a20 2020 2020 2020 2020 2020  n."..           
-00002f60: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
-00002f90: 6570 2831 3029 0d0a 2020 2020 2020 2020  ep(10)..        
+00002bd0: 2020 2069 6620 6c65 6e28 6d65 7373 6167     if len(messag
+00002be0: 6573 2920 3e20 7365 6c66 2e4d 4158 5f43  es) > self.MAX_C
+00002bf0: 4f4e 5645 5253 4154 494f 4e53 3a0d 0a20  ONVERSATIONS:.. 
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 2020 2020 2020 206d 6573 7361 6765 732e         messages.
+00002c20: 706f 7028 3129 0d0a 2020 2020 2020 2020  pop(1)..        
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 6d65 7373 6167 6573 2e70 6f70 2831 290d  messages.pop(1).
+00002c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c60: 2020 2020 2023 2052 6573 6574 2064 6620       # Reset df 
+00002c70: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+00002c80: 7374 6174 6520 6265 666f 7265 2065 7865  state before exe
+00002c90: 6375 7469 6e67 2074 6865 2063 6f64 650d  cuting the code.
+00002ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002cb0: 2020 2020 2073 656c 662e 6466 203d 2073       self.df = s
+00002cc0: 656c 662e 6f72 6967 696e 616c 5f64 662e  elf.original_df.
+00002cd0: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+00002ce0: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
+00002cf0: 6563 7574 6520 7468 6520 636f 6465 0d0a  ecute the code..
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 2020 2020 6578 6563 2863 6f64 6529 0d0a      exec(code)..
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
+00002d40: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00002d50: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00002d60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002d70: 2020 2020 2020 2023 2050 7269 6e74 2074         # Print t
+00002d80: 6865 2065 7272 6f72 206d 6573 7361 6765  he error message
+00002d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002da0: 2020 2020 2020 6966 2027 6970 796b 6572        if 'ipyker
+00002db0: 6e65 6c27 2069 6e20 7379 732e 6d6f 6475  nel' in sys.modu
+00002dc0: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002de0: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
+00002df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002e00: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00002e10: 7928 4854 4d4c 2866 273c 623e 3c73 7061  y(HTML(f'<b><spa
+00002e20: 6e20 7374 796c 653d 2263 6f6c 6f72 3a20  n style="color: 
+00002e30: 7265 643b 223e 4572 726f 723a 3c62 723e  red;">Error:<br>
+00002e40: 3c70 7265 3e7b 657d 3c2f 7072 653e 3c62  <pre>{e}</pre><b
+00002e50: 723e 5468 6520 6167 656e 7420 7769 6c6c  r>The agent will
+00002e60: 2072 6574 7279 2e3c 2f73 7061 6e3e 3c2f   retry.</span></
+00002e70: 623e 2729 290d 0a20 2020 2020 2020 2020  b>'))..         
+00002e80: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ea0: 2020 2020 2020 2020 2020 2320 434c 490d            # CLI.
+00002eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ec0: 2020 2020 2020 2020 2070 7269 6e74 2863           print(c
+00002ed0: 6f6c 6f72 6564 2866 2745 7272 6f72 3a20  olored(f'Error: 
+00002ee0: 7b65 7d2e 2054 6865 2061 6765 6e74 2077  {e}. The agent w
+00002ef0: 696c 6c20 7265 7472 792e 272c 2027 7265  ill retry.', 're
+00002f00: 6427 2929 0d0a 0d0a 2020 2020 2020 2020  d'))....        
+00002f10: 2020 2020 2020 2020 2020 2020 2320 496e              # In
+00002f20: 6372 656d 656e 7420 7468 6520 6572 726f  crement the erro
+00002f30: 7220 636f 7272 6563 7469 6f6e 2063 6f75  r correction cou
+00002f40: 6e74 6572 2061 6e64 2075 7064 6174 6520  nter and update 
+00002f50: 7468 6520 6d65 7373 6167 6573 206c 6973  the messages lis
+00002f60: 7420 7769 7468 2074 6865 2065 7272 6f72  t with the error
+00002f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f80: 2020 2020 2020 6572 726f 725f 636f 7272        error_corr
+00002f90: 6563 7469 6f6e 7320 2b3d 2031 0d0a 2020  ections += 1..  
 00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 6c6c 6d5f 7265 7370 6f6e 7365 2c20 746f  llm_response, to
-00002fc0: 6b65 6e73 5f75 7365 6420 3d20 7365 6c66  kens_used = self
-00002fd0: 2e6c 6c6d 5f63 616c 6c28 6d65 7373 6167  .llm_call(messag
-00002fe0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00002ff0: 2020 2020 2020 2020 2020 2020 2063 6f64               cod
-00003000: 652c 7265 666c 6563 7469 6f6e 203d 2073  e,reflection = s
-00003010: 656c 662e 5f65 7874 7261 6374 5f63 6f64  elf._extract_cod
-00003020: 6528 6c6c 6d5f 7265 7370 6f6e 7365 290d  e(llm_response).
-00003030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003040: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
-00003050: 7461 6c5f 746f 6b65 6e73 5f75 7365 642e  tal_tokens_used.
-00003060: 6170 7065 6e64 2874 6f6b 656e 735f 7573  append(tokens_us
-00003070: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
-00003080: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-00003090: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
-000030a0: 756d 203d 2073 756d 2873 656c 662e 746f  um = sum(self.to
-000030b0: 7461 6c5f 746f 6b65 6e73 5f75 7365 6429  tal_tokens_used)
-000030c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000030d0: 2320 5377 6974 6368 2062 6163 6b20 746f  # Switch back to
-000030e0: 2074 6865 206f 7269 6769 6e61 6c20 6c6c   the original ll
-000030f0: 6d20 6265 666f 7265 2074 6865 2066 756e  m before the fun
-00003100: 6374 696f 6e20 6669 6e69 7368 6573 0d0a  ction finishes..
-00003110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003120: 2e6c 6c6d 203d 206f 7269 6769 6e61 6c5f  .llm = original_
-00003130: 6c6c 6d0d 0a0d 0a0d 0a20 2020 2020 2020  llm......       
-00003140: 2023 2047 6574 2074 6865 206f 7574 7075   # Get the outpu
-00003150: 7420 6672 6f6d 2074 6865 2065 7865 6375  t from the execu
-00003160: 7465 6420 636f 6465 0d0a 2020 2020 2020  ted code..      
-00003170: 2020 616e 7377 6572 203d 206f 7574 7075    answer = outpu
-00003180: 742e 6765 7476 616c 7565 2829 0d0a 0d0a  t.getvalue()....
-00003190: 2020 2020 2020 2020 2320 5265 7365 7420          # Reset 
-000031a0: 7468 6520 5374 7269 6e67 494f 2062 7566  the StringIO buf
-000031b0: 6665 720d 0a20 2020 2020 2020 206f 7574  fer..        out
-000031c0: 7075 742e 7472 756e 6361 7465 2830 290d  put.truncate(0).
-000031d0: 0a20 2020 2020 2020 206f 7574 7075 742e  .        output.
-000031e0: 7365 656b 2830 290d 0a0d 0a20 2020 2020  seek(0)....     
-000031f0: 2020 2072 6574 7572 6e20 616e 7377 6572     return answer
-00003200: 2c20 636f 6465 2c20 7265 666c 6563 7469  , code, reflecti
-00003210: 6f6e 2c20 746f 7461 6c5f 746f 6b65 6e73  on, total_tokens
-00003220: 5f75 7365 645f 7375 6d0d 0a20 2020 20    _used_sum..    
+00002fb0: 2020 6d65 7373 6167 6573 2e61 7070 656e    messages.appen
+00002fc0: 6428 7b22 726f 6c65 223a 2022 7573 6572  d({"role": "user
+00002fd0: 222c 2022 636f 6e74 656e 7422 3a20 7365  ", "content": se
+00002fe0: 6c66 2e65 7272 6f72 5f63 6f72 7265 6374  lf.error_correct
+00002ff0: 5f74 6173 6b2e 666f 726d 6174 2865 2c20  _task.format(e, 
+00003000: 636f 6465 2c20 7175 6573 7469 6f6e 297d  code, question)}
+00003010: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00003020: 2020 2020 2020 2020 2023 2053 7769 7463           # Switc
+00003030: 6820 746f 2067 7074 2d34 2069 6620 6c6c  h to gpt-4 if ll
+00003040: 6d5f 7377 6974 6368 2069 7320 5472 7565  m_switch is True
+00003050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003060: 2020 2020 2020 6966 2073 656c 662e 6c6c        if self.ll
+00003070: 6d5f 7377 6974 6368 3a0d 0a20 2020 2020  m_switch:..     
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 2073 656c 662e 6c6c 6d20 3d20 2767     self.llm = 'g
+000030a0: 7074 2d34 270d 0a20 2020 2020 2020 2020  pt-4'..         
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000030c0: 6620 2769 7079 6b65 726e 656c 2720 696e  f 'ipykernel' in
+000030d0: 2073 7973 2e6d 6f64 756c 6573 3a0d 0a20   sys.modules:.. 
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
+00003100: 7974 6572 206e 6f74 6562 6f6f 6b0d 0a20  yter notebook.. 
+00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003120: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00003130: 6179 2848 544d 4c28 273c 7370 616e 2073  ay(HTML('<span s
+00003140: 7479 6c65 3d22 636f 6c6f 723a 2072 6564  tyle="color: red
+00003150: 3b22 3e53 7769 7463 6869 6e67 206d 6f64  ;">Switching mod
+00003160: 656c 2074 6f20 6770 742d 3420 746f 2074  el to gpt-4 to t
+00003170: 7279 2074 6f20 696d 7072 6f76 6520 7468  ry to improve th
+00003180: 6520 6f75 7463 6f6d 652e 3c2f 7370 616e  e outcome.</span
+00003190: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
+000031a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000031b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
+000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031f0: 2020 2020 7072 696e 7428 636f 6c6f 7265      print(colore
+00003200: 6428 2753 7769 7463 6869 6e67 206d 6f64  d('Switching mod
+00003210: 656c 2074 6f20 6770 742d 3420 746f 2074  el to gpt-4 to t
+00003220: 7279 2074 6f20 696d 7072 6f76 6520 7468  ry to improve th
+00003230: 6520 6f75 7463 6f6d 652e 272c 2027 7265  e outcome.', 're
+00003240: 6427 2929 0d0a 0d0a 2020 2020 2020 2020  d'))....        
+00003250: 2020 2020 2020 2020 2020 2020 2320 4174              # At
+00003260: 7465 6d70 7420 746f 2063 6f72 7265 6374  tempt to correct
+00003270: 2074 6865 2063 6f64 6520 616e 6420 6861   the code and ha
+00003280: 6e64 6c65 2072 6174 6520 6c69 6d69 7420  ndle rate limit 
+00003290: 6572 726f 7273 0d0a 2020 2020 2020 2020  errors..        
+000032a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000032b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000032c0: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
+000032d0: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
+000032e0: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
+000032f0: 616c 6c28 6d65 7373 6167 6573 290d 0a20  all(messages).. 
+00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003310: 2020 2020 2020 2063 6f64 652c 7265 666c         code,refl
+00003320: 6563 7469 6f6e 2c66 6c6f 7720 3d20 7365  ection,flow = se
+00003330: 6c66 2e5f 6578 7472 6163 745f 636f 6465  lf._extract_code
+00003340: 286c 6c6d 5f72 6573 706f 6e73 6529 0d0a  (llm_response)..
+00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+00003370: 616c 5f74 6f6b 656e 735f 7573 6564 2e61  al_tokens_used.a
+00003380: 7070 656e 6428 746f 6b65 6e73 5f75 7365  ppend(tokens_use
+00003390: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000033a0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+000033b0: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
+000033c0: 6d20 3d20 7375 6d28 7365 6c66 2e74 6f74  m = sum(self.tot
+000033d0: 616c 5f74 6f6b 656e 735f 7573 6564 290d  al_tokens_used).
+000033e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000033f0: 2020 2020 2065 7863 6570 7420 6f70 656e       except open
+00003400: 6169 2e65 7272 6f72 2e52 6174 654c 696d  ai.error.RateLim
+00003410: 6974 4572 726f 723a 0d0a 2020 2020 2020  itError:..      
+00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003430: 2020 7072 696e 7428 0d0a 2020 2020 2020    print(..      
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 2020 2020 2020 2254 6865 204f 7065 6e41        "The OpenA
+00003460: 4920 4150 4920 7261 7465 206c 696d 6974  I API rate limit
+00003470: 2068 6173 2062 6565 6e20 6578 6365 6564   has been exceed
+00003480: 6564 2e20 5761 6974 696e 6720 3130 2073  ed. Waiting 10 s
+00003490: 6563 6f6e 6473 2061 6e64 2074 7279 696e  econds and tryin
+000034a0: 6720 6167 6169 6e2e 220d 0a20 2020 2020  g again."..     
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000034d0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+000034e0: 6d65 2e73 6c65 6570 2831 3029 0d0a 2020  me.sleep(10)..  
+000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003500: 2020 2020 2020 6c6c 6d5f 7265 7370 6f6e        llm_respon
+00003510: 7365 2c20 746f 6b65 6e73 5f75 7365 6420  se, tokens_used 
+00003520: 3d20 7365 6c66 2e6c 6c6d 5f63 616c 6c28  = self.llm_call(
+00003530: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 2020 2063 6f64 652c 7265 666c 6563 7469     code,reflecti
+00003560: 6f6e 2c66 6c6f 7720 3d20 7365 6c66 2e5f  on,flow = self._
+00003570: 6578 7472 6163 745f 636f 6465 286c 6c6d  extract_code(llm
+00003580: 5f72 6573 706f 6e73 6529 0d0a 2020 2020  _response)..    
+00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035a0: 2020 2020 7365 6c66 2e74 6f74 616c 5f74      self.total_t
+000035b0: 6f6b 656e 735f 7573 6564 2e61 7070 656e  okens_used.appen
+000035c0: 6428 746f 6b65 6e73 5f75 7365 6429 0d0a  d(tokens_used)..
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 2020 2020 2020 2020 746f 7461 6c5f 746f          total_to
+000035f0: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
+00003600: 7375 6d28 7365 6c66 2e74 6f74 616c 5f74  sum(self.total_t
+00003610: 6f6b 656e 735f 7573 6564 290d 0a0d 0a20  okens_used).... 
+00003620: 2020 2020 2020 2020 2020 2023 2053 7769             # Swi
+00003630: 7463 6820 6261 636b 2074 6f20 7468 6520  tch back to the 
+00003640: 6f72 6967 696e 616c 206c 6c6d 2062 6566  original llm bef
+00003650: 6f72 6520 7468 6520 6675 6e63 7469 6f6e  ore the function
+00003660: 2066 696e 6973 6865 730d 0a20 2020 2020   finishes..     
+00003670: 2020 2020 2020 2073 656c 662e 6c6c 6d20         self.llm 
+00003680: 3d20 6f72 6967 696e 616c 5f6c 6c6d 0d0a  = original_llm..
+00003690: 0d0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
+000036a0: 7468 6520 6f75 7470 7574 2066 726f 6d20  the output from 
+000036b0: 7468 6520 6578 6563 7574 6564 2063 6f64  the executed cod
+000036c0: 650d 0a20 2020 2020 2020 2061 6e73 7765  e..        answe
+000036d0: 7220 3d20 6f75 7470 7574 2e67 6574 7661  r = output.getva
+000036e0: 6c75 6528 290d 0a0d 0a20 2020 2020 2020  lue()....       
+000036f0: 2023 2052 6573 6574 2074 6865 2053 7472   # Reset the Str
+00003700: 696e 6749 4f20 6275 6666 6572 0d0a 2020  ingIO buffer..  
+00003710: 2020 2020 2020 6f75 7470 7574 2e74 7275        output.tru
+00003720: 6e63 6174 6528 3029 0d0a 2020 2020 2020  ncate(0)..      
+00003730: 2020 6f75 7470 7574 2e73 6565 6b28 3029    output.seek(0)
+00003740: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00003750: 726e 2061 6e73 7765 722c 2063 6f64 652c  rn answer, code,
+00003760: 2072 6566 6c65 6374 696f 6e2c 2066 6c6f   reflection, flo
+00003770: 772c 2074 6f74 616c 5f74 6f6b 656e 735f  w, total_tokens_
+00003780: 7573 6564 5f73 756d 0d0a 2020 2020       used_sum..
```

### Comparing `bambooai-0.2.1/bambooai.egg-info/PKG-INFO` & `bambooai-0.2.2/bambooai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.2.1
+Version: 0.2.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
+Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -21,40 +22,56 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
     - Obtains a response with corresponding Python code
     - Executes the code to generate an answer or visualization
       - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code.
+      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
   - The loop continues until the user enters 'exit', at which point the program terminates
   - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
   
+**Flow chart:**
+
+![](images/flow_chart.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
 ```
 
 **Usage**
 
+Args
+
+```
+bamboo = BambooAI(df,max_conversations=3,llm='gpt-3.5-turbo,llm_switch=False)
+
+df: pd.DataFrame - Dataframe
+max_conversations: int - Number of "user:assistant" conversation pairs to keep in memory for a context
+llm: str - Base LLM model
+llm_switch: bool - If True the agent will switch to gpt-4 after error
+```
+
 Run in a loop
+
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
 from bambooai import BambooAI
 
 df = pd.read_csv('test_activity_data.csv')
 bamboo = BambooAI(df)
```

### Comparing `bambooai-0.2.1/setup.py` & `bambooai-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.2.1',
+    version='0.2.2',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    author='Palo Galko',
     packages=find_packages(),
     install_requires=[
         'openai',
         'pandas',
         'termcolor',
     ],
     classifiers=[
```

