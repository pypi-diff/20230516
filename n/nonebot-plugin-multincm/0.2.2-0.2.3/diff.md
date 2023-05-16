# Comparing `tmp/nonebot_plugin_multincm-0.2.2.tar.gz` & `tmp/nonebot_plugin_multincm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.2.2.tar", last modified: Mon May 15 19:00:55 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.2.3.tar", last modified: Tue May 16 16:46:12 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.2.2.tar` & `nonebot_plugin_multincm-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/LICENSE
--rw-r--r--   0        0        0     5586 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/README.md
--rw-r--r--   0        0        0      769 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0     7284 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0     4562 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0     9924 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2573 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0   212591 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     1688 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      874 2023-05-15 19:00:43.426255 nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      826 2023-05-15 19:00:55.630407 nonebot_plugin_multincm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6487 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5789 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/README.md
+-rw-r--r--   0        0        0     1172 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0     7323 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0     4562 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    10221 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2573 2023-05-16 16:45:57.526707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0   212591 2023-05-16 16:45:57.530707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     1688 2023-05-16 16:45:57.530707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-16 16:45:57.530707 nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      826 2023-05-16 16:46:12.295750 nonebot_plugin_multincm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.2.2/LICENSE` & `nonebot_plugin_multincm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/README.md` & `nonebot_plugin_multincm-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -128,25 +128,29 @@
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
+  - 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐
   - 别名：`网易云`、`wyy`
-- 解析 <回复 音乐卡片 / 链接>（获取该音乐的播放链接并使用自定义卡片发送）
+- 解析 <回复 音乐卡片 / 链接>
+  - 介绍：获取该音乐的播放链接并使用自定义卡片发送
   - 别名：`resolve`、`parse`、`get`
-- 歌词 <回复 音乐卡片 / 链接>（获取该音乐的歌词）
+- 歌词 <回复 音乐卡片 / 链接>
+  - 介绍：获取该音乐的歌词，以图片形式发送
   - 别名：`lrc`、`lyric`、`lyrics`
-- 链接 <回复 音乐卡片 / 链接>（获取该音乐的网易云链接）
+- 链接 <回复 音乐卡片>
+  - 介绍：获取 Bot 发送的音乐卡片的网易云歌曲链接
   - 别名：`link`
 
 ### Tip
 
-- 点击 Bot 发送的音乐卡片可以跳转直链，可以直接下载该音乐
+- 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -167,14 +171,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 微调歌曲列表排版
+- 微调插件帮助文本
+
 ### 0.2.2
 
 - 修复搜歌 `KeyError`
 
 ### 0.2.1
 
 - 删除歌词尾部的空行与多余分割线
```

#### html2text {}

```diff
@@ -34,26 +34,28 @@
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
-æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] - å«åï¼`ç½æäº`ã`wyy` - è§£æ
-<åå¤ é³ä¹å¡ç /
-é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåéï¼ -
-å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç /
-é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ - å«åï¼`lrc`ã`lyric`ã`lyrics` -
-é¾æ¥ <åå¤ é³ä¹å¡ç / é¾æ¥>ï¼è·åè¯¥é³ä¹çç½æäºé¾æ¥ï¼ -
+æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+ä»ç»ï¼é¡¾åæä¹ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
+å«åï¼`ç½æäº`ã`wyy` - è§£æ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
+å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ <åå¤ é³ä¹å¡ç> -
+ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºæ­æ²é¾æ¥ -
 å«åï¼`link` ### Tip - ç¹å» Bot
-åéçé³ä¹å¡çå¯ä»¥è·³è½¬ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½è¯¥é³ä¹ ## ð
+åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ###
-0.2.1 - å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 -
-æ°å¢äºä¸ä¸ªæä»¤ `è§£æ`ã`æ­è¯`ã`é¾æ¥` -
-ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
+å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
+å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,19 +158,19 @@
     state["page"] = 1
     state["cache"] = {}
     await matcher.pause(await get_page(matcher, state))
 
 
 @cmd_pick_song.handle()
 async def _(matcher: Matcher, state: T_State, event: MessageEvent):
-    arg = event.get_message().extract_plain_text().strip()
+    arg = event.get_message().extract_plain_text().strip().lower()
     page: int = state["page"]
     page_max: int = state["page_max"]
 
-    if arg in ["退出", "tc", "exit", "e", "0"]:
+    if arg in ["退出", "tc", "取消", "qx", "exit", "e", "cancel", "c", "0"]:
         await matcher.finish("已退出选择")
 
     if arg in ["上一页", "syy", "previous", "p"]:
         if page <= 1:
             await matcher.reject("已经是第一页了")
         await matcher.reject(await get_page(matcher, state, page - 1))
```

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/draw.py`

 * *Files 13% similar despite different names*

```diff
@@ -219,53 +219,64 @@
     title_txt = Text2Image.from_text(
         "歌曲列表",
         80,
         weight="bold",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
+    tip_txt = Text2Image.from_bbcode_text(
+        "Tip：[b]发送序号[/b] 选择歌曲\n其他操作：[b]上一页[/b](P) | [b]下一页[/b](N) | [b]退出[/b](E)",
+        30,
+        align="center",
+        fill=(255, 255, 255),
+        fontname=config.ncm_list_font or "",
+    )
     footer_txt = Text2Image.from_bbcode_text(
-        (
-            f"第 [b]{page_num}[/b] / [b]{max_page}[/b] 页 | 共 [b]{res.songCount}[/b] 首\n"
-            "Tip：发送序号选择；发送 [b]上一页[/b] 或 [b]下一页[/b] 来翻页；发送 [b]退出[/b] 退出选择"
-        ),
+        f"第 [b]{page_num}[/b] / [b]{max_page}[/b] 页 | 共 [b]{res.songCount}[/b] 首",
         30,
         align="center",
         fill=(255, 255, 255),
         fontname=config.ncm_list_font or "",
     )
 
     width = table.width + pic_padding * 2 + table_padding * 2
-    height = table.height + title_txt.height + footer_txt.height + table_padding * 6
+    height = (
+        table.height
+        + title_txt.height
+        + tip_txt.height
+        + footer_txt.height
+        + table_padding * 7
+    )
 
     bg = BACKGROUND.copy().convert("RGBA").resize((width, height), keep_ratio=True)
-    title_txt.draw_on_image(bg.image, ((width - title_txt.width) // 2, table_padding))
+    y_offset = table_padding
+
+    title_txt.draw_on_image(bg.image, ((width - title_txt.width) // 2, y_offset))
+    y_offset += title_txt.height + table_padding
+
+    tip_txt.draw_on_image(bg.image, ((width - tip_txt.width) // 2, y_offset))
+    y_offset += tip_txt.height + table_padding
+
     bg.paste(
         (
             BuildImage.new(
                 "RGBA",
                 (table.width + table_padding * 2, table.height + table_padding * 2),
                 (0, 0, 0, 80),
             ).circle_corner(table_border_radius)
         ),
-        (pic_padding, title_txt.height + table_padding * 2),
+        (pic_padding, y_offset),
         alpha=True,
     )
-    bg.paste(
-        table,
-        (
-            pic_padding + table_padding,
-            title_txt.height + table_padding * 3,
-        ),
-        alpha=True,
-    )
-    footer_txt.draw_on_image(
-        bg.image,
-        ((width - footer_txt.width) // 2, height - table_padding - footer_txt.height),
-    )
+    y_offset += table_padding
+
+    bg.paste(table, (pic_padding + table_padding, y_offset), alpha=True)
+    y_offset += table.height + table_padding * 2
+
+    footer_txt.draw_on_image(bg.image, ((width - footer_txt.width) // 2, y_offset))
 
     return bg.save_jpg()
 
 
 def format_lrc(lrc: LyricData) -> Optional[str]:
     def fmt_usr(usr: User) -> str:
         return f"{usr.nickname} [{usr.userid}]"
```

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.2/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.2.3/nonebot_plugin_multincm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
 
 def format_alias(name: str, alias: List[str]) -> str:
     return f'{name}（{"；".join(alias)}）' if alias else name
 
 
 def format_artists(artists: List[Artist]) -> str:
-    return "、".join([format_alias(x.name, x.alias) for x in artists])
+    return "、".join([x.name for x in artists])
```

### Comparing `nonebot_plugin_multincm-0.2.2/pyproject.toml` & `nonebot_plugin_multincm-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.2.2"
+version = "0.2.3"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.2.2/PKG-INFO` & `nonebot_plugin_multincm-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.2.2
+Version: 0.2.3
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -153,25 +153,29 @@
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
+  - 介绍：顾名思义。当输入音乐 ID 时会直接发送对应音乐
   - 别名：`网易云`、`wyy`
-- 解析 <回复 音乐卡片 / 链接>（获取该音乐的播放链接并使用自定义卡片发送）
+- 解析 <回复 音乐卡片 / 链接>
+  - 介绍：获取该音乐的播放链接并使用自定义卡片发送
   - 别名：`resolve`、`parse`、`get`
-- 歌词 <回复 音乐卡片 / 链接>（获取该音乐的歌词）
+- 歌词 <回复 音乐卡片 / 链接>
+  - 介绍：获取该音乐的歌词，以图片形式发送
   - 别名：`lrc`、`lyric`、`lyrics`
-- 链接 <回复 音乐卡片 / 链接>（获取该音乐的网易云链接）
+- 链接 <回复 音乐卡片>
+  - 介绍：获取 Bot 发送的音乐卡片的网易云歌曲链接
   - 别名：`link`
 
 ### Tip
 
-- 点击 Bot 发送的音乐卡片可以跳转直链，可以直接下载该音乐
+- 点击 Bot 发送的音乐卡片会跳转到音乐直链，可以直接下载
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -192,14 +196,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.3
+
+- 微调歌曲列表排版
+- 微调插件帮助文本
+
 ### 0.2.2
 
 - 修复搜歌 `KeyError`
 
 ### 0.2.1
 
 - 删除歌词尾部的空行与多余分割线
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.2 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.3 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -47,26 +47,28 @@
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
-æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] - å«åï¼`ç½æäº`ã`wyy` - è§£æ
-<åå¤ é³ä¹å¡ç /
-é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåéï¼ -
-å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç /
-é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ - å«åï¼`lrc`ã`lyric`ã`lyrics` -
-é¾æ¥ <åå¤ é³ä¹å¡ç / é¾æ¥>ï¼è·åè¯¥é³ä¹çç½æäºé¾æ¥ï¼ -
+æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+ä»ç»ï¼é¡¾åæä¹ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
+å«åï¼`ç½æäº`ã`wyy` - è§£æ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç / é¾æ¥> -
+ä»ç»ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ä»¥å¾çå½¢å¼åé -
+å«åï¼`lrc`ã`lyric`ã`lyrics` - é¾æ¥ <åå¤ é³ä¹å¡ç> -
+ä»ç»ï¼è·å Bot åéçé³ä¹å¡ççç½æäºæ­æ²é¾æ¥ -
 å«åï¼`link` ### Tip - ç¹å» Bot
-åéçé³ä¹å¡çå¯ä»¥è·³è½¬ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½è¯¥é³ä¹ ## ð
+åéçé³ä¹å¡çä¼è·³è½¬å°é³ä¹ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ###
-0.2.1 - å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 -
-æ°å¢äºä¸ä¸ªæä»¤ `è§£æ`ã`æ­è¯`ã`é¾æ¥` -
-ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
+å¾®è°æä»¶å¸®å©ææ¬ ### 0.2.2 - ä¿®å¤ææ­ `KeyError` ### 0.2.1 -
+å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

