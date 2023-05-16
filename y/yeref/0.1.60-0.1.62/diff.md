# Comparing `tmp/yeref-0.1.60.tar.gz` & `tmp/yeref-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.60.tar", last modified: Tue May  9 14:36:45 2023, max compression
+gzip compressed data, was "yeref-0.1.62.tar", last modified: Tue May 16 16:19:26 2023, max compression
```

## Comparing `yeref-0.1.60.tar` & `yeref-0.1.62.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:36:45.029971 yeref-0.1.60/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-09 14:36:45.030146 yeref-0.1.60/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-09 14:36:45.030809 yeref-0.1.60/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-09 14:36:40.000000 yeref-0.1.60/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:36:45.022513 yeref-0.1.60/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.60/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.60/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   198893 2023-05-08 17:51:39.000000 yeref-0.1.60/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-09 14:36:45.029414 yeref-0.1.60/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-09 14:36:44.000000 yeref-0.1.60/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-09 14:36:45.000000 yeref-0.1.60/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-09 14:36:44.000000 yeref-0.1.60/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-09 14:36:44.000000 yeref-0.1.60/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.409659 yeref-0.1.62/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-16 16:19:26.410076 yeref-0.1.62/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-16 16:19:26.410873 yeref-0.1.62/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-16 16:19:11.000000 yeref-0.1.62/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.400857 yeref-0.1.62/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.62/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.62/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   200404 2023-05-16 13:39:01.000000 yeref-0.1.62/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-16 16:19:26.409029 yeref-0.1.62/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-16 16:19:26.000000 yeref-0.1.62/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.60/setup.py` & `yeref-0.1.62/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.60',
+      version='0.1.62',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.60-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.62-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.60/yeref/l_.py` & `yeref-0.1.62/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.60/yeref/yeref.py` & `yeref-0.1.62/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 from aiogram.utils.text_decorations import markdown_decoration
 from exiftool import ExifToolHelper
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
 from loguru import logger
 from oauth2client.service_account import ServiceAccountCredentials
 from pydub import AudioSegment
-from pyrogram import enums, Client
+from pyrogram import enums, Client, utils
 from pyrogram.errors import FloodWait, UserAlreadyParticipant, UsernameInvalid, BadRequest, SlowmodeWait, \
     UserDeactivatedBan, SessionRevoked, SessionExpired, AuthKeyUnregistered, AuthKeyInvalid, AuthKeyDuplicated, \
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
-from telegraph import Telegraph
+from telegraph.aio import Telegraph
 
 import yeref
 
 one_minute = 60
 one_hour = 3600
 seconds_in_day = 86400
 my_tid = 5491025132
@@ -68,28 +68,28 @@
 passwd = 'lost9'
 bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
 hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
 str_empty = bin_empty.decode('utf-8')
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
 TGPH_TOKENS = {
-    'https://telegra.ph/pst-FereyDemoBot-05-08': 'f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f',
-    'https://telegra.ph/pst-FereyBotBot-05-08': 'e7f943fcc98bac07ad6aaf6e570d0f51abadf02567938c997dbc1ad1923b',
-    'https://telegra.ph/pst-FereyPostBot-05-08': '14085be3058c0a25616d094f4bb65c73dc61f783468f01da41d99fb6ace1',
-    'https://telegra.ph/pst-FereyMediaBot-05-08': 'cf71a596b7ecdc96d30ddffdbf1e26863dd39755f47b4fc343fc3867f373',
-    'https://telegra.ph/pst-FereyChannelBot-05-08': 'f43f375b8aec531cee0d5048878943a3ccee97da4143d311d5b2c7ed3237',
-    'https://telegra.ph/pst-FereyGroupBot-05-08': 'c08f94618b94dd25ef75de70c1ed565853efef5479057c68a5720609bb7f',
-    'https://telegra.ph/pst-FereyFindBot-05-08': '2d005bb366dc5bef023d58b93d5f45fb9a02a7d2b0f9063a6fc277b5a62d',
-    'https://telegra.ph/pst-FereyTargetBot-05-08': 'bda8c0a4b7a35101d34252568acd46df7bd3d8d85f4e13dd35f3bddc2f80',
-    'https://telegra.ph/pst-FereyToolsBot-05-08': 'ea83403eb6ac7d2ad24d7e7a86163be20cd2d7f4734267808e154a8fd0a6',
-    'https://telegra.ph/pst-FereyVPNBot-05-08': '38086caf43905ef827715da999aae0be2427ebd7a05d9ff7420543b50613',
-    'https://telegra.ph/pst-FereyAIBot-05-08': 'bcda631d991c16b4fdfd15e7af6512bcf8fd679fee6bd4c717f6266671a0',
-    'https://telegra.ph/pst-FereyUserBot-05-08': '3698a3432c233bef48c238b35cfe94db844858b2ba98594007c7757dcf03',
-    'https://telegra.ph/pst-FereyWorkBot-05-08': 'd4930b2a9311ad63f7f0ae3d61ca7224ecf76a2434a50161e239a45199c5',
-    'https://telegra.ph/pst-FereyAdsBot-05-08': 'c1024508f1a5de4f9544dd10793b1401da95de5719bdcf0b4c9f6c26a672',
+    "https://telegra.ph/pst-FereyDemoBot-05-08": "f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f",
+    "https://telegra.ph/pst-FereyBotBot-05-08": "e7f943fcc98bac07ad6aaf6e570d0f51abadf02567938c997dbc1ad1923b",
+    "https://telegra.ph/pst-FereyPostBot-05-08": "14085be3058c0a25616d094f4bb65c73dc61f783468f01da41d99fb6ace1",
+    "https://telegra.ph/pst-FereyMediaBot-05-08": "cf71a596b7ecdc96d30ddffdbf1e26863dd39755f47b4fc343fc3867f373",
+    "https://telegra.ph/pst-FereyChannelBot-05-08": "f43f375b8aec531cee0d5048878943a3ccee97da4143d311d5b2c7ed3237",
+    "https://telegra.ph/pst-FereyGroupBot-05-08": "c08f94618b94dd25ef75de70c1ed565853efef5479057c68a5720609bb7f",
+    "https://telegra.ph/pst-FereyFindBot-05-08": "2d005bb366dc5bef023d58b93d5f45fb9a02a7d2b0f9063a6fc277b5a62d",
+    "https://telegra.ph/pst-FereyTargetBot-05-08": "bda8c0a4b7a35101d34252568acd46df7bd3d8d85f4e13dd35f3bddc2f80",
+    "https://telegra.ph/pst-FereyToolsBot-05-08": "ea83403eb6ac7d2ad24d7e7a86163be20cd2d7f4734267808e154a8fd0a6",
+    "https://telegra.ph/pst-FereyVPNBot-05-08": "38086caf43905ef827715da999aae0be2427ebd7a05d9ff7420543b50613",
+    "https://telegra.ph/pst-FereyAIBot-05-08": "bcda631d991c16b4fdfd15e7af6512bcf8fd679fee6bd4c717f6266671a0",
+    "https://telegra.ph/pst-FereyUserBot-05-08": "3698a3432c233bef48c238b35cfe94db844858b2ba98594007c7757dcf03",
+    "https://telegra.ph/pst-FereyWorkBot-05-08": "d4930b2a9311ad63f7f0ae3d61ca7224ecf76a2434a50161e239a45199c5",
+    "https://telegra.ph/pst-FereyAdsBot-05-08": "c1024508f1a5de4f9544dd10793b1401da95de5719bdcf0b4c9f6c26a672",
 }
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
@@ -214,24 +214,206 @@
     return 0
 
 
 # endregion
 
 
 # region menu
+async def post_offer(bot, data, BASE_D):
+    try:
+        for item in data:
+            try:
+                OFFER_ID, OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, \
+                    OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
+                    OFFER_DT, OFFER_TZ = item
+
+                sign_ = OFFER_TZ[0]
+                h_, m_ = OFFER_TZ.strip(sign_).split(':')
+                dt_now = datetime.datetime.utcnow()
+                if sign_ == "+":
+                    dt_cur = dt_now + datetime.timedelta(hours=int(h_), minutes=int(m_))
+                else:
+                    dt_cur = dt_now - datetime.timedelta(hours=int(h_), minutes=int(m_))
+                timedelta_ = (dt_cur - datetime.datetime.strptime(OFFER_DT, "%d-%m-%Y %H:%M"))
+
+                if timedelta_.days >= 0 and timedelta_.seconds >= 0:
+                    sql = "UPDATE OFFER SET OFFER_DT=NULL, OFFER_STATUS=0 WHERE OFFER_ID=?"
+                    await db_change(sql, (OFFER_ID,), BASE_D)
+
+                    loop_minute = asyncio.get_event_loop()
+                    loop_minute.create_task(broadcast_send_admin(bot, OFFER_USERTID, 'en', OFFER_ID, BASE_D, []))
+            except Exception as e:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+
+async def bots_by_inline(chat_id, message, BASE_D):
+    result = []
+    try:
+        lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
+
+        data = [
+            ['👩🏽‍💻 @FereyDemoBot', yeref.l_inline_demo[lz], 'https://t.me/FereyDemoBot'],
+            ['👩🏽‍💻 @FereyBotBot', yeref.l_inline_bot[lz], 'https://t.me/FereyBotBot'],
+            ['👩🏽‍💻 @FereyPostBot', yeref.l_inline_post[lz], 'https://t.me/FereyPostBot'],
+            ['👩🏽‍💻 @FereyMediaBot', yeref.l_inline_media[lz], 'https://t.me/FereyMediaBot'],
+            ['👩🏽‍💻 @FereyChannelBot', yeref.l_inline_channel[lz], 'https://t.me/FereyChannelBot'],
+            ['👩🏽‍💻 @FereyGroupBot', yeref.l_inline_group[lz], 'https://t.me/FereyGroupBot'],
+            ['👩🏽‍💻 @FereyFindBot', yeref.l_inline_find[lz], 'https://t.me/FereyFindBot'],
+            ['👩🏽‍💻 @FereyAIBot', yeref.l_inline_ai[lz], 'https://t.me/FereyAIBot'],
+            ['👩🏽‍💻 @FereyAdsBot', yeref.l_inline_ads[lz], 'https://t.me/FereyAdsBot'],
+            ['👩🏽‍💻 @FereyVPNBot', yeref.l_inline_vpn[lz], 'https://t.me/FereyVPNBot'],
+            ['👩🏽‍💻 @FereyTargetBot', yeref.l_inline_target[lz], 'https://t.me/FereyTargetBot'],
+            ['👩🏽‍💻 @FereyUserBot', yeref.l_inline_user[lz], 'https://t.me/FereyUserBot'],
+            ['👩🏽‍💻 @FereyToolsBot', yeref.l_inline_tools[lz], 'https://t.me/FereyToolsBot'],
+            ['👩🏽‍💻 @FereyWorkBot', yeref.l_inline_work[lz], 'https://t.me/FereyWorkBot'],
+        ]
+
+        for i in range(0, len(data)):
+            title, desc, text = data[i]
+
+            input_message_content = types.InputTextMessageContent(message_text=text, disable_web_page_preview=False)
+            result.append(types.InlineQueryResultArticle(id=str(uuid4()),
+                                                         title=title,
+                                                         description=desc,
+                                                         thumb_url=bot_logo_jpeg,
+                                                         input_message_content=input_message_content))
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
+
+
+async def get_buttons_main(lz, bot_un, BASE_D):
+    result = []
+    try:
+        result = [
+            types.InlineKeyboardButton(text="👩🏽‍💼Acc", url=f"tg://user?id={my_tid}"),
+            types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph')),
+            types.InlineKeyboardButton(text="🔗Share",
+                                       url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_un}&text=%40{bot_un}'),
+            types.InlineKeyboardButton(text=f"{(await read_likes(BASE_D))}♥️Like", callback_data=f"like"),
+            types.InlineKeyboardButton(text="🦋Chan", url=f"https://t.me/{get_tg_channel(lz)}"),
+            types.InlineKeyboardButton(text="🫥Bots", switch_inline_query_current_chat=f"~"),
+        ]
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
+
+
+# endregion
+
+
+# region telegraph
+async def get_telegraph_page(access_token, url):
+    result = telegraph_ = None
+    try:
+        telegraph_ = Telegraph(access_token=access_token)
+        pages_ = (await telegraph_.get_page_list())['pages']
+
+        for page_ in pages_:
+            if page_['url'] == url:
+                result = await telegraph_.get_page(path=page_['path'], return_content=True, return_html=False)
+                return
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return telegraph_, result
+
+
+async def tgph_change(access_token, url, json_):
+    retry = 2
+    while retry > 0:
+        try:
+            await asyncio.sleep(round(random.uniform(0, 1), 2))
+            telegraph_ = Telegraph(access_token=access_token)
+            pages_ = await telegraph_.get_page_list()
+
+            for page_ in pages_['pages']:
+                if page_['url'] != url: continue
+
+                get_page_ = await telegraph_.get_page(path=page_['path'], return_content=True, return_html=False)
+                try:
+                    content_json = json.loads(str(get_page_['content'][0]))
+                except:
+                    content_json = {}
+
+                timestamp_ = str(utils.datetime_to_timestamp(datetime.datetime.utcnow()))
+                content_json[timestamp_] = json_
+                post_dumps = json.dumps(content_json, ensure_ascii=False)
+                await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content=post_dumps)
+                return 1
+        except Exception as e:
+            logger.info(log_ % str(e))
+            await asyncio.sleep(round(random.uniform(1, 2), 2))
+        finally:
+            retry -= 1
+    return 0
+
+
+async def tgph_clear(access_token, url):
+    retry = 2
+    while retry > 0:
+        try:
+            await asyncio.sleep(round(random.uniform(0, 1), 2))
+            telegraph_ = Telegraph(access_token=access_token)
+            pages_ = await telegraph_.get_page_list()
+
+            for page_ in pages_['pages']:
+                if page_['url'] == url:
+                    await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content='{}')
+                return 1
+        except Exception as e:
+            logger.info(log_ % str(e))
+            await asyncio.sleep(round(random.uniform(1, 2), 2))
+        finally:
+            retry -= 1
+    return 0
+
+
+async def get_tgph_link(file_name):
+    result = None
+    try:
+        if file_name and os.path.exists(file_name) and os.path.getsize(file_name) < 5242880:
+            try:
+                # jpg, .jpeg, .png, .gif and .mp4
+                telegraph_ = Telegraph()
+                res = await telegraph_.upload_file(file_name)
+                if res:
+                    result = f"{'https://telegra.ph'}{res[0]['src']}"
+            except Exception as e:
+                logger.info(log_ % f"Telegraph: {str(e)}")
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+    finally:
+        return result
+
+
 async def is_ban_menu(chat_id):
     result = False
     try:
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
-        pages = telegraph_.get_page_list()
+        pages = await telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
-                    page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
+                    page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
 
                     if str(chat_id) in ban_ids:
                         result = True
                     return
             except Exception as e:
                 logger.info(log_ % str(e))
@@ -251,21 +433,21 @@
     finally:
         return result
 
 
 async def ban_handler_menu(bot, chat_id, args):
     try:
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
-        pages = telegraph_.get_page_list()
+        pages = await telegraph_.get_page_list()
 
         if not args:
             for item in pages['pages']:
                 try:
                     if item['path'] == 'ban-04-11-7':
-                        page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
+                        page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                         ban_ids = str(page['content'])
                         ban_ids = ban_ids[:4096]
                         ban_ids = ' '.join([f"<code>{it}</code>" for it in ban_ids.split()])
 
                         await bot.send_message(chat_id, ban_ids)
                         return
                 except Exception as e:
@@ -275,23 +457,23 @@
         prepare_ids = args.split()
         prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
         if not len(prepare_ids): return
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
-                    page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
+                    page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
                     length1 = len(ban_ids)
                     ban_ids = f"{page['content']} {' '.join(prepare_ids)}"
                     ban_ids = ban_ids.split()
                     ban_ids = list(set(ban_ids))
                     length2 = len(ban_ids)
                     modul = abs(length1 - length2)
-                    telegraph_.edit_page(path=item['path'], title="ban", html_content=' '.join(ban_ids))
+                    await telegraph_.edit_page(path=item['path'], title="ban", html_content=' '.join(ban_ids))
 
                     if length1 != length2:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th added to /ban (len: {length2})")
                     else:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th already in /ban (len: {length2})")
                     break
             except Exception as e:
@@ -311,30 +493,30 @@
             return
         else:
             prepare_ids = args.split()
 
         prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
         if not len(prepare_ids): return
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
-        pages = telegraph_.get_page_list()
+        pages = await telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
-                    page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
+                    page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
                     length1 = len(ban_ids)
 
                     ban_ids = [ban_id for ban_id in ban_ids if ban_id not in prepare_ids]
                     length2 = len(ban_ids)
                     ban_ids = list(set(ban_ids))
                     modul = abs(length1 - length2)
                     html_content = ' '.join(ban_ids)
                     html_content = '0' if html_content == '' else html_content
-                    telegraph_.edit_page(path=item['path'], title="ban", html_content=html_content)
+                    await telegraph_.edit_page(path=item['path'], title="ban", html_content=html_content)
 
                     if length1 != length2:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th removed from /ban (len: {length2})")
                     else:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th already deleted from /ban (len: {length2})")
                     break
             except Exception as e:
@@ -352,20 +534,20 @@
     try:
         arr = [k for k, v in TGPH_TOKENS.items() if bot_username in k]
         access_key = arr[0] if len(arr) else None
         if not access_key: return
 
         access_token = TGPH_TOKENS[access_key]
         telegraph_ = Telegraph(access_token=access_token)
-        pages = telegraph_.get_page_list()
+        pages = await telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['url'] == access_key:
-                    page = telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
+                    page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
                     try:
                         content_json = json.loads(str(page['content'][0]))
                     except:
                         content_json = {}
 
                     for OFFER_USERTID, v in content_json.items():
                         OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
@@ -380,118 +562,25 @@
                                               v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
                                               v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
                                               v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
                                               v[OFFER_DT], v[OFFER_TZ],), BASE_D)
 
                         del content_json[str(OFFER_USERTID)]
                         post_dumps = json.dumps(content_json, ensure_ascii=False)
-                        telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
+                        await telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
                         return
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
-
-
-async def post_offer(bot, data, BASE_D):
-    try:
-        for item in data:
-            try:
-                OFFER_ID, OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, \
-                    OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
-                    OFFER_DT, OFFER_TZ = item
-
-                sign_ = OFFER_TZ[0]
-                h_, m_ = OFFER_TZ.strip(sign_).split(':')
-                dt_now = datetime.datetime.utcnow()
-                if sign_ == "+":
-                    dt_cur = dt_now + datetime.timedelta(hours=int(h_), minutes=int(m_))
-                else:
-                    dt_cur = dt_now - datetime.timedelta(hours=int(h_), minutes=int(m_))
-                timedelta_ = (dt_cur - datetime.datetime.strptime(OFFER_DT, "%d-%m-%Y %H:%M"))
-
-                if timedelta_.days >= 0 and timedelta_.seconds >= 0:
-                    sql = "UPDATE OFFER SET OFFER_DT=NULL, OFFER_STATUS=0 WHERE OFFER_ID=?"
-                    await db_change(sql, (OFFER_ID,), BASE_D)
-
-                    loop_minute = asyncio.get_event_loop()
-                    loop_minute.create_task(broadcast_send_admin(bot, OFFER_USERTID, 'en', OFFER_ID, BASE_D, []))
-            except Exception as e:
-                logger.info(log_ % str(e))
-                await asyncio.sleep(round(random.uniform(0, 1), 2))
-    except TelegramRetryAfter as e:
-        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-
-
-async def bots_by_inline(chat_id, message, BASE_D):
-    result = []
-    try:
-        lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
-
-        data = [
-            ['👩🏽‍💻 @FereyDemoBot', yeref.l_inline_demo[lz], 'https://t.me/FereyDemoBot'],
-            ['👩🏽‍💻 @FereyBotBot', yeref.l_inline_bot[lz], 'https://t.me/FereyBotBot'],
-            ['👩🏽‍💻 @FereyPostBot', yeref.l_inline_post[lz], 'https://t.me/FereyPostBot'],
-            ['👩🏽‍💻 @FereyMediaBot', yeref.l_inline_media[lz], 'https://t.me/FereyMediaBot'],
-            ['👩🏽‍💻 @FereyChannelBot', yeref.l_inline_channel[lz], 'https://t.me/FereyChannelBot'],
-            ['👩🏽‍💻 @FereyGroupBot', yeref.l_inline_group[lz], 'https://t.me/FereyGroupBot'],
-            ['👩🏽‍💻 @FereyFindBot', yeref.l_inline_find[lz], 'https://t.me/FereyFindBot'],
-            ['👩🏽‍💻 @FereyAIBot', yeref.l_inline_ai[lz], 'https://t.me/FereyAIBot'],
-            ['👩🏽‍💻 @FereyAdsBot', yeref.l_inline_ads[lz], 'https://t.me/FereyAdsBot'],
-            ['👩🏽‍💻 @FereyVPNBot', yeref.l_inline_vpn[lz], 'https://t.me/FereyVPNBot'],
-            ['👩🏽‍💻 @FereyTargetBot', yeref.l_inline_target[lz], 'https://t.me/FereyTargetBot'],
-            ['👩🏽‍💻 @FereyUserBot', yeref.l_inline_user[lz], 'https://t.me/FereyUserBot'],
-            ['👩🏽‍💻 @FereyToolsBot', yeref.l_inline_tools[lz], 'https://t.me/FereyToolsBot'],
-            ['👩🏽‍💻 @FereyWorkBot', yeref.l_inline_work[lz], 'https://t.me/FereyWorkBot'],
-        ]
-
-        for i in range(0, len(data)):
-            title, desc, text = data[i]
-
-            input_message_content = types.InputTextMessageContent(message_text=text, disable_web_page_preview=False)
-            result.append(types.InlineQueryResultArticle(id=str(uuid4()),
-                                                         title=title,
-                                                         description=desc,
-                                                         thumb_url=bot_logo_jpeg,
-                                                         input_message_content=input_message_content))
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
-async def get_buttons_main(lz, bot_un, BASE_D):
-    result = []
-    try:
-        result = [
-            types.InlineKeyboardButton(text="👩🏽‍💼Acc", url=f"tg://user?id={my_tid}"),
-            types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph')),
-            types.InlineKeyboardButton(text="🔗Share",
-                                       url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_un}&text=%40{bot_un}'),
-            types.InlineKeyboardButton(text=f"{(await read_likes(BASE_D))}♥️Like", callback_data=f"like"),
-            types.InlineKeyboardButton(text="🦋Chan", url=f"https://t.me/{get_tg_channel(lz)}"),
-            types.InlineKeyboardButton(text="🫥Bots", switch_inline_query_current_chat=f"~"),
-        ]
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
 # endregion
 
 
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
@@ -1301,24 +1390,18 @@
                     media_type = 'document'
                     file_name_part_new = obj.video.file_name
 
                 file_name = os.path.join(MEDIA_D, file_name_part_new)
                 file = await bot.get_file(media_id)
                 await bot.download_file(file.file_path, file_name)
 
-                tgph_link = ''
-                if file_name and os.path.exists(file_name) and os.path.getsize(file_name) < 5242880:
-                    try:
-                        telegraph = Telegraph()
-                        res = telegraph.upload_file(file_name)
-                        tgph_link = f"{'https://telegra.ph'}{res[0]['src']}"
-                    except Exception as e:
-                        logger.info(log_ % f"Telegraph: {str(e)}")
-                        await asyncio.sleep(round(random.uniform(0, 1), 2))
+                tgph_link = await get_tgph_link(file_name)
+                tgph_link = '' if tgph_link is None else tgph_link
                 if file_name and os.path.exists(file_name): os.remove(file_name)
+
                 offer_tgph_link = (ast.literal_eval(str(offer_tgph_link)) + [tgph_link]) if offer_tgph_link else [
                     tgph_link]
                 file_name_part = (ast.literal_eval(str(file_name_part)) + [file_name_part_new]) if file_name_part else [
                     file_name_part_new]
                 offer_file_id = (ast.literal_eval(str(offer_file_id)) + [media_id]) if offer_file_id else [media_id]
                 offer_file_type = (ast.literal_eval(str(offer_file_type)) + [media_type]) if offer_file_type else [
                     media_type]
@@ -1471,25 +1554,18 @@
                 file_id_note = res.video.file_id
                 await bot.delete_message(chat_id, res.message_id)
             elif message.document:
                 file_id = message.document.file_id
                 file_name_part = f"{message.document.file_name}"
                 file_type = 'document'
 
-            if file_name and os.path.exists(file_name) and os.path.getsize(file_name) < 5242880:
-                try:
-                    # jpg, .jpeg, .png, .gif and .mp4
-                    telegraph = Telegraph()
-                    res = telegraph.upload_file(file_name)
-                    if res:
-                        offer_tgph_link = f"{'https://telegra.ph'}{res[0]['src']}"
-                except Exception as e:
-                    logger.info(log_ % f"Telegraph: {str(e)}")
-                    await asyncio.sleep(round(random.uniform(0, 1), 2))
+            offer_tgph_link = await get_tgph_link(file_name)
+            offer_tgph_link = '' if offer_tgph_link is None else offer_tgph_link
             if file_name and os.path.exists(file_name): os.remove(file_name)
+
             await state.update_data(offer_file_id=file_id, offer_file_id_note=file_id_note, offer_file_type=file_type,
                                     offer_tgph_link=offer_tgph_link, file_name_part=file_name_part)
 
             text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
                 yeref.l_post_button[lz].replace('XXXXX', '')
             await bot.send_message(chat_id, text)
             await state.set_state(FsmOffer.button)
@@ -2006,15 +2082,15 @@
 async def get_chat_channel(bot, link, SESSION_D, BASE_S):
     result = None
     try:
         sql = "SELECT SESSION_TID, SESSION_STATUS FROM SESSION"
         data = await db_select(sql, (), BASE_S)
         random.shuffle(data)
 
-        for item in data:
+        for _ in data:
             sql = "SELECT SESSION_TID, SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_STATUS FROM SESSION"
             data = await db_select(sql, (), BASE_S)
             random.shuffle(data)
             SESSION_TID, SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_STATUS = data[0]
             if SESSION_STATUS is not None: continue
 
             try:
@@ -3543,40 +3619,14 @@
     except Exception as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
-async def save_photo(bot, photo, MEDIA_D):
-    result = None
-    try:
-        if not photo: return
-        file_id = photo.big_file_id
-        photo_path = os.path.join(MEDIA_D, (datetime.datetime.utcnow()).strftime("%d-%m-%Y_%H-%M-%S.jpg"))
-        await bot.download_file_by_id(file_id, photo_path)
-
-        # jpg, .jpeg, .png, .gif and .mp4
-        if os.path.exists(photo_path) and os.path.getsize(photo_path) < 5242880:
-            try:
-                telegraph = Telegraph()
-                res = telegraph.upload_file(photo_path)
-                if res:
-                    result = f"{'https://telegra.ph'}{res[0]['src']}"
-                    if os.path.exists(photo_path): os.remove(photo_path)
-            except Exception as e:
-                await log(e)
-                await asyncio.sleep(round(random.uniform(1, 2), 2))
-    except Exception as e:
-        logger.info(log_ % f"{str(e)}")
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
 async def delete_account(bot, SESSION_TID, SESSIONS_D, CONF_P, BASE_S):
     try:
         sql = "SELECT SESSION_NAME FROM SESSION WHERE SESSION_TID=?"
         data = await db_select(sql, (SESSION_TID,), BASE_S)
         if not data:
             await bot.send_message(my_tid, f"✅ Account {SESSION_TID} doesnt exist")
             return
@@ -3906,15 +3956,17 @@
         await log(e)
         logger.info(log_ % f"\tsend to user {USER_TID}-{USER_USERNAME} error")
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return cnt
 
 
-async def api_get_file_list(drive_service, folder_id, tmp_dic={} or None, parent_name='', is_file=False):
+async def api_get_file_list(drive_service, folder_id, tmp_dic=None, parent_name='', is_file=False):
+    if tmp_dic is None:
+        tmp_dic = {} or None
     if is_file:
         file = drive_service.files().get(fileId=folder_id, fields="id, name, size, modifiedTime, mimeType").execute()
         tmp_dic[file['id']] = [file['name'], file['mimeType'], parent_name, file['modifiedTime']]
         return tmp_dic
     q = "\'" + folder_id + "\'" + " in parents"
     fields = "nextPageToken, files(id, name, size, modifiedTime, mimeType)"
     results = drive_service.files().list(pageSize=1000, q=q, fields=fields).execute()
```

