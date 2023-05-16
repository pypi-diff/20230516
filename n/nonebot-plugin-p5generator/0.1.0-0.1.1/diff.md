# Comparing `tmp/nonebot_plugin_p5generator-0.1.0.tar.gz` & `tmp/nonebot_plugin_p5generator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_p5generator-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_p5generator-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_p5generator-0.1.0.tar` & `nonebot_plugin_p5generator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      543 2023-05-14 15:11:17.671866 nonebot_plugin_p5generator-0.1.0/nonebot_plugin_p5generator/__init__.py
--rw-r--r--   0        0        0     4612 2023-05-14 15:39:45.728508 nonebot_plugin_p5generator-0.1.0/nonebot_plugin_p5generator/generator.py
--rw-r--r--   0        0        0      631 2023-05-14 18:39:36.242315 nonebot_plugin_p5generator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1485 2023-05-14 16:32:09.433330 nonebot_plugin_p5generator-0.1.0/README.md
--rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.0/setup.py
--rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-05-16 06:42:08.922667 nonebot_plugin_p5generator-0.1.1/nonebot_plugin_p5generator/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-16 06:42:08.923667 nonebot_plugin_p5generator-0.1.1/nonebot_plugin_p5generator/generator.py
+-rw-r--r--   0        0        0      487 2023-05-16 06:42:09.511380 nonebot_plugin_p5generator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1485 2023-05-16 06:42:08.922667 nonebot_plugin_p5generator-0.1.1/README.md
+-rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.1/setup.py
+-rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 nonebot_plugin_p5generator-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_p5generator-0.1.0/nonebot_plugin_p5generator/__init__.py` & `nonebot_plugin_p5generator-0.1.1/nonebot_plugin_p5generator/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
-from nonebot.params import CommandArg
-
-from .generator import generate_image
-
-p5=on_command('p5generator', aliases={'p5预告信'})
-
-@p5.handle()
-async def p5generator(args: Message = CommandArg()):
-    if not args.extract_plain_text():
-        await p5.finish(f"给我要生成的语句啊，不然佐仓双叶来了都没办法生成")
-    image = await generate_image(args.extract_plain_text())
-    await p5.finish(MessageSegment.image(image))
-
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot.params import CommandArg
+
+from .generator import generate_image
+
+p5=on_command('p5generator', aliases={'p5预告信'})
+
+@p5.handle()
+async def p5generator(args: Message = CommandArg()):
+    if not args.extract_plain_text():
+        await p5.finish(f"给我要生成的语句啊，不然佐仓双叶来了都没办法生成")
+    image = await generate_image(args.extract_plain_text())
+    await p5.finish(MessageSegment.image(image))
+
```

### Comparing `nonebot_plugin_p5generator-0.1.0/nonebot_plugin_p5generator/generator.py` & `nonebot_plugin_p5generator-0.1.1/nonebot_plugin_p5generator/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from base64 import b64encode
-from io import BytesIO
-from pathlib import Path
-from typing import Union
-
-from PIL import Image, ImageDraw, ImageFont
-import random
-
-RESOURCES_PATH = Path() / 'data' / 'p5generator'
-RESOURCES_PATH.mkdir(exist_ok=True)
-
-
-async def generate_image(text):
-    # 设置字体列表
-    fonts = [f'{RESOURCES_PATH}\\msyh.ttc', f'{RESOURCES_PATH}\\STHUPO.TTF', f'{RESOURCES_PATH}\\simsun.ttc',
-             f'{RESOURCES_PATH}\\msyhbd.ttc', f'{RESOURCES_PATH}\\simhei.ttf']
-    # 设置颜色列表
-    colors = ['white', 'black', 'gray', 'red']
-    # 设置背景颜色列表
-    bg_colors = {'white': ['black', 'gray'], 'black': ['white', 'gray'], 'gray': ['white', 'black'], 'red': ['white']}
-
-    # 打开背景图片
-    background_image = Image.open(f'{RESOURCES_PATH}\\background.png')
-
-    # 获取背景图片大小
-    width, height = background_image.size
-
-    # 分割文本为多个句子
-    sentences = text.split('\n')
-
-    # 计算文本总高度
-    text_height = 0
-    max_char_height = 0
-    sentences_count = len(sentences)
-    for sentence in sentences:
-        sentence = sentence.replace('\r', "")
-        sentence = sentence.replace('\r\n', "")
-        text_size = min(1770 // len(sentence), 1300 // (sentences_count + 6))
-        for char in sentence:
-            # 随机选择字体和大小
-            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
-            # 获取字符大小
-            char_width, char_height = font.getsize(char)
-            max_char_height = max(max_char_height, char_height)
-        text_height += max_char_height + 20
-
-    # 计算文本起始位置
-    y = (height - text_height) // 2
-
-    # 遍历每个句子
-    for sentence in sentences:
-        # 计算句子宽度
-        sentence = sentence.replace('\r', "")
-        sentence = sentence.replace('\r\n', "")
-        sentence_width = 0
-        text_size = min(1770 // (len(sentence) + 6), 1300 // (sentences_count + 6))
-        for char in sentence:
-            # 随机选择字体和大小
-            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
-            # 获取字符大小
-            char_width, char_height = font.getsize(char)
-            sentence_width += char_width + 20
-
-        # 计算句子起始位置
-        x = (width - sentence_width) // 2
-
-        # 遍历句子中的每个字符
-        for index, char in enumerate(sentence):
-            # 随机选择字体和大小
-            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
-            # 随机选择颜色
-            color = random.choice(colors)
-            # 根据颜色选择背景颜色
-            bg_color = random.choice(bg_colors[color])
-            # 获取字符大小
-            char_width, char_height = font.getsize(char)
-
-            # 创建字符图像和绘图对象
-            char_image = Image.new('RGBA', (char_width, char_height))
-            char_draw = ImageDraw.Draw(char_image)
-
-            # 绘制背景色块
-            char_draw.rectangle((0, 0, char_width, char_height), fill=bg_color)
-            # 绘制字符
-            char_draw.text((0, 0), char, fill=color, font=font)
-
-            # 随机旋转角度
-            angle = random.randint(-5, 5)
-            char_image = char_image.rotate(angle, resample=Image.BICUBIC, expand=True)
-
-            # 将字符图像粘贴到背景图像上
-            background_image.paste(char_image, (x, y), char_image)
-
-            # 更新x坐标
-            x += char_width + 20
-
-            # 更新y坐标以换行
-        y += max_char_height + 20
-    # 返回图像
-    result = await convert_img(background_image)
-    return result
-
-
-async def convert_img(
-        img: Union[Image.Image, str, Path, bytes], is_base64: bool = False
-):
-    """
-    :说明:
-      将PIL.Image对象转换为bytes或者base64格式。
-    :参数:
-      * img (Image): 图片。
-      * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
-    :返回:
-      * res: bytes对象或base64编码图片。
-    """
-    if isinstance(img, Image.Image):
-        img = img.convert('RGB')
-        result_buffer = BytesIO()
-        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
-        res = result_buffer.getvalue()
-        if is_base64:
-            res = 'base64://' + b64encode(res).decode()
-        return res
-    elif isinstance(img, bytes):
-        return 'base64://' + b64encode(img).decode()
-    else:
-        return f'[CQ:image,file=file:///{str(img)}]'
+from base64 import b64encode
+from io import BytesIO
+from pathlib import Path
+from typing import Union
+
+from PIL import Image, ImageDraw, ImageFont
+import random
+
+RESOURCES_PATH = Path() / 'data' / 'p5generator'
+RESOURCES_PATH.mkdir(parents=True, exist_ok=True)
+
+
+async def generate_image(text):
+    # 设置字体列表
+    fonts = [f'{RESOURCES_PATH}\\msyh.ttc', f'{RESOURCES_PATH}\\STHUPO.TTF', f'{RESOURCES_PATH}\\simsun.ttc',
+             f'{RESOURCES_PATH}\\msyhbd.ttc', f'{RESOURCES_PATH}\\simhei.ttf']
+    # 设置颜色列表
+    colors = ['white', 'black', 'gray', 'red']
+    # 设置背景颜色列表
+    bg_colors = {'white': ['black', 'gray'], 'black': ['white', 'gray'], 'gray': ['white', 'black'], 'red': ['white']}
+
+    # 打开背景图片
+    background_image = Image.open(f'{RESOURCES_PATH}\\background.png')
+
+    # 获取背景图片大小
+    width, height = background_image.size
+
+    # 分割文本为多个句子
+    sentences = text.split('\n')
+
+    # 计算文本总高度
+    text_height = 0
+    max_char_height = 0
+    sentences_count = len(sentences)
+    for sentence in sentences:
+        sentence = sentence.replace('\r', "")
+        sentence = sentence.replace('\r\n', "")
+        text_size = min(1770 // len(sentence), 1300 // (sentences_count + 6))
+        for char in sentence:
+            # 随机选择字体和大小
+            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
+            # 获取字符大小
+            char_width, char_height = font.getsize(char)
+            max_char_height = max(max_char_height, char_height)
+        text_height += max_char_height + 20
+
+    # 计算文本起始位置
+    y = (height - text_height) // 2
+
+    # 遍历每个句子
+    for sentence in sentences:
+        # 计算句子宽度
+        sentence = sentence.replace('\r', "")
+        sentence = sentence.replace('\r\n', "")
+        sentence_width = 0
+        text_size = min(1770 // (len(sentence) + 6), 1300 // (sentences_count + 6))
+        for char in sentence:
+            # 随机选择字体和大小
+            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
+            # 获取字符大小
+            char_width, char_height = font.getsize(char)
+            sentence_width += char_width + 20
+
+        # 计算句子起始位置
+        x = (width - sentence_width) // 2
+
+        # 遍历句子中的每个字符
+        for index, char in enumerate(sentence):
+            # 随机选择字体和大小
+            font = ImageFont.truetype(random.choice(fonts), random.randint(text_size, text_size + 20))
+            # 随机选择颜色
+            color = random.choice(colors)
+            # 根据颜色选择背景颜色
+            bg_color = random.choice(bg_colors[color])
+            # 获取字符大小
+            char_width, char_height = font.getsize(char)
+
+            # 创建字符图像和绘图对象
+            char_image = Image.new('RGBA', (char_width, char_height))
+            char_draw = ImageDraw.Draw(char_image)
+
+            # 绘制背景色块
+            char_draw.rectangle((0, 0, char_width, char_height), fill=bg_color)
+            # 绘制字符
+            char_draw.text((0, 0), char, fill=color, font=font)
+
+            # 随机旋转角度
+            angle = random.randint(-5, 5)
+            char_image = char_image.rotate(angle, resample=Image.BICUBIC, expand=True)
+
+            # 将字符图像粘贴到背景图像上
+            background_image.paste(char_image, (x, y), char_image)
+
+            # 更新x坐标
+            x += char_width + 20
+
+            # 更新y坐标以换行
+        y += max_char_height + 20
+    # 返回图像
+    result = await convert_img(background_image)
+    return result
+
+
+async def convert_img(
+        img: Union[Image.Image, str, Path, bytes], is_base64: bool = False
+):
+    """
+    :说明:
+      将PIL.Image对象转换为bytes或者base64格式。
+    :参数:
+      * img (Image): 图片。
+      * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
+    :返回:
+      * res: bytes对象或base64编码图片。
+    """
+    if isinstance(img, Image.Image):
+        img = img.convert('RGB')
+        result_buffer = BytesIO()
+        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
+        res = result_buffer.getvalue()
+        if is_base64:
+            res = 'base64://' + b64encode(res).decode()
+        return res
+    elif isinstance(img, bytes):
+        return 'base64://' + b64encode(img).decode()
+    else:
+        return f'[CQ:image,file=file:///{str(img)}]'
```

### Comparing `nonebot_plugin_p5generator-0.1.0/README.md` & `nonebot_plugin_p5generator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_p5generator-0.1.0/setup.py` & `nonebot_plugin_p5generator-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 install_requires = \
 ['nonebot-adapter-onebot>=2.2.0,<3.0.0',
  'nonebot2>=2.0.0rc2,<3.0.0',
  'pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-p5generator',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A generator of persona5 chatbot based on nonebot2 framework',
     'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-p5generator\n\n《女神异闻录5》预告信的生成插件\n\n</div>\n\n## 💬 前言\n\n可以生成仿《女神异闻录5》中心之怪盗团向罪人宣战的预告信，做的不太好请见谅\n\n## 📖 介绍\n\n使用Pillow库制作的一款插件，因为p5中的预告信字都是从报纸上面剪下来的，所以还原了随机的字体。\n代码比较烂，随便看看吧。\n知识和勇气增加了。\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n  \n    nb plugin install nonebot-plugin-p5generator\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n  \n    pip install nonebot-plugin-p5generator\n\n</details>\n\n## 🍰 资源文件\n\n`data`文件夹中的`p5generator`会存储与插件有关的文件\n\n下载仓库中p5generator文件夹后放入data文件夹中\n\n## 🎉 使用\n\n输入`p5预告信`后接你想要输入的内容即可生成：\n\n![946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)\n\n![5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)\n',
     'author': 'xi-yue-233',
     'author_email': '1004514855@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/xi-yue-233/nonebot-plugin-p5generator',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_p5generator'] package_data = \ {'': ['*']} install_requires =
 \ ['nonebot-adapter-onebot>=2.2.0,<3.0.0', 'nonebot2>=2.0.0rc2,<3.0.0',
 'pillow>=9.5.0,<10.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-p5generator',
-'version': '0.1.0', 'description': 'A generator of persona5 chatbot based on
+'version': '0.1.1', 'description': 'A generator of persona5 chatbot based on
 nonebot2 framework', 'long_description': '
                                 \n [nonebot]\n
 \n\n
                              \n\n# nonebot-plugin-
        p5generator\n\nãå¥³ç¥å¼é»å½5ãé¢åä¿¡ççææä»¶\n\n
 \n\n## ð¬
 åè¨\n\nå¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡ï¼åçä¸å¤ªå¥½è¯·è§è°\n\n##
@@ -20,11 +20,10 @@
 ð
 ä½¿ç¨\n\nè¾å¥`p5é¢åä¿¡`åæ¥ä½ æ³è¦è¾å¥çåå®¹å³å¯çæï¼\n\n!
 [946CE1499E017FE129710E8B6E2FB725](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/0a19bacc-bde4-4693-93e7-83678bde4835)\n\n!
 [5C4D9FCBE4F060A12612D6062287E7E6](https://github.com/xi-yue-233/nonebot-
 plugin-p5generator/assets/58218656/4aade3a7-34a0-4e81-96ea-612146b76808)\n',
 'author': 'xi-yue-233', 'author_email': '1004514855@qq.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/xi-yue-233/
-nonebot-plugin-p5generator', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+'None', 'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_p5generator-0.1.0/PKG-INFO` & `nonebot_plugin_p5generator-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-p5generator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A generator of persona5 chatbot based on nonebot2 framework
-Home-page: https://github.com/xi-yue-233/nonebot-plugin-p5generator
 Author: xi-yue-233
 Author-email: 1004514855@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Project-URL: Repository, https://github.com/xi-yue-233/nonebot-plugin-p5generator
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-p5generator Version: 0.1.0 Summary:
-A generator of persona5 chatbot based on nonebot2 framework Home-page: https://
-github.com/xi-yue-233/nonebot-plugin-p5generator Author: xi-yue-233 Author-
-email: 1004514855@qq.com Requires-Python: >=3.9,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
+Metadata-Version: 2.1 Name: nonebot-plugin-p5generator Version: 0.1.1 Summary:
+A generator of persona5 chatbot based on nonebot2 framework Author: xi-yue-233
+Author-email: 1004514855@qq.com Requires-Python: >=3.9,<4.0 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
 (>=2.2.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0) Requires-Dist:
-pillow (>=9.5.0,<10.0.0) Project-URL: Repository, https://github.com/xi-yue-
-233/nonebot-plugin-p5generator Description-Content-Type: text/markdown
+pillow (>=9.5.0,<10.0.0) Description-Content-Type: text/markdown
                                    [nonebot]
   # nonebot-plugin-p5generator ãå¥³ç¥å¼é»å½5ãé¢åä¿¡ççææä»¶
 ## ð¬ åè¨
 å¯ä»¥çæä»¿ãå¥³ç¥å¼é»å½5ãä¸­å¿ä¹æªçå¢åç½ªäººå®£æçé¢åä¿¡ï¼åçä¸å¤ªå¥½è¯·è§è°
 ## ð ä»ç»
 ä½¿ç¨Pillowåºå¶ä½çä¸æ¬¾æä»¶ï¼å ä¸ºp5ä¸­çé¢åä¿¡å­é½æ¯ä»æ¥çº¸ä¸é¢åªä¸æ¥çï¼æä»¥è¿åäºéæºçå­ä½ã
 ä»£ç æ¯è¾çï¼éä¾¿ççå§ã ç¥è¯ååæ°å¢å äºã ## ð¿ å®è£
```

