# Comparing `tmp/TPEBot-0.5.0.tar.gz` & `tmp/TPEBot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPEBot-0.5.0.tar", last modified: Tue May 16 14:56:08 2023, max compression
+gzip compressed data, was "TPEBot-0.5.1.tar", last modified: Tue May 16 15:04:58 2023, max compression
```

## Comparing `TPEBot-0.5.0.tar` & `TPEBot-0.5.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.307421 TPEBot-0.5.0/
--rw-rw-rw-   0        0        0      226 2023-05-16 14:56:08.299450 TPEBot-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-05-12 06:25:07.000000 TPEBot-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:07.638905 TPEBot-0.5.0/TPEBot.egg-info/
--rw-rw-rw-   0        0        0      226 2023-05-16 14:56:07.000000 TPEBot-0.5.0/TPEBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6085 2023-05-16 14:56:07.000000 TPEBot-0.5.0/TPEBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:56:07.000000 TPEBot-0.5.0/TPEBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-16 14:56:07.000000 TPEBot-0.5.0/TPEBot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:07.674925 TPEBot-0.5.0/buildABot/
--rw-rw-rw-   0        0        0    40255 2023-05-16 14:52:32.000000 TPEBot-0.5.0/buildABot/Analytics.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:07.674925 TPEBot-0.5.0/buildABot/Data/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:07.859156 TPEBot-0.5.0/buildABot/Data/Default - Learn/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Learn/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:07.995182 TPEBot-0.5.0/buildABot/Data/Default - Recommended/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.003170 TPEBot-0.5.0/buildABot/Data/Entities/
--rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Entities/LoginID.json
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.211366 TPEBot-0.5.0/buildABot/Data/WebApp/
--rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/WebApp/index_template_LEARN.html
--rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/WebApp/index_template_RECO.html
--rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/WebApp/reset_template_RECO.js
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.267455 TPEBot-0.5.0/buildABot/Data/Webhook/
--rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
--rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
--rw-rw-rw-   0        0        0     5497 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Webhook/index_template_LEARN.js
--rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPEBot-0.5.0/buildABot/Data/Webhook/index_template_RECO.js
--rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPEBot-0.5.0/buildABot/Data/__init__.py
--rw-rw-rw-   0        0        0    15847 2023-05-16 14:52:32.000000 TPEBot-0.5.0/buildABot/Entities.py
--rw-rw-rw-   0        0        0    12267 2023-05-16 14:52:32.000000 TPEBot-0.5.0/buildABot/FallbackSocialTag.py
--rw-rw-rw-   0        0        0    12103 2023-05-16 14:52:32.000000 TPEBot-0.5.0/buildABot/Firebase_Learn.py
--rw-rw-rw-   0        0        0    14879 2023-05-16 14:52:32.000000 TPEBot-0.5.0/buildABot/Firebase_Reco.py
--rw-rw-rw-   0        0        0    36243 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Intents.py
--rw-rw-rw-   0        0        0    42171 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/LearnMenu.py
--rw-rw-rw-   0        0        0    72431 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Manager.py
--rw-rw-rw-   0        0        0    15947 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Paraphraser.py
--rw-rw-rw-   0        0        0     6151 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Password.py
--rw-rw-rw-   0        0        0    44723 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/RecommendedMenu.py
--rw-rw-rw-   0        0        0     8791 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/TelegramLogs.py
--rw-rw-rw-   0        0        0     7539 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/WebApp_Learn.py
--rw-rw-rw-   0        0        0    11283 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/WebApp_Reco.py
--rw-rw-rw-   0        0        0     9259 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Webhook_Learn.py
--rw-rw-rw-   0        0        0    19235 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Webhook_Reco.py
--rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/Worksheets.py
--rw-rw-rw-   0        0        0     5075 2023-05-16 14:52:33.000000 TPEBot-0.5.0/buildABot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.283425 TPEBot-0.5.0/buildABot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEBot-0.5.0/buildABot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.291422 TPEBot-0.5.0/parrot/
--rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPEBot-0.5.0/parrot/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPEBot-0.5.0/parrot/demo.py
--rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPEBot-0.5.0/parrot/filters.py
--rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPEBot-0.5.0/parrot/parrot.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:56:08.299450 TPEBot-0.5.0/parrot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEBot-0.5.0/parrot/pytransform/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-16 14:56:08.307421 TPEBot-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-05-16 14:55:45.000000 TPEBot-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.382914 TPEBot-0.5.1/
+-rw-rw-rw-   0        0        0      226 2023-05-16 15:04:58.382914 TPEBot-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-05-12 06:25:07.000000 TPEBot-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.148422 TPEBot-0.5.1/TPEBot.egg-info/
+-rw-rw-rw-   0        0        0      226 2023-05-16 15:04:57.000000 TPEBot-0.5.1/TPEBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6085 2023-05-16 15:04:58.000000 TPEBot-0.5.1/TPEBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:04:57.000000 TPEBot-0.5.1/TPEBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-16 15:04:57.000000 TPEBot-0.5.1/TPEBot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.180391 TPEBot-0.5.1/buildABot/
+-rw-rw-rw-   0        0        0    40255 2023-05-16 14:52:32.000000 TPEBot-0.5.1/buildABot/Analytics.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.188697 TPEBot-0.5.1/buildABot/Data/
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.261530 TPEBot-0.5.1/buildABot/Data/Default - Learn/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Learn/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.350420 TPEBot-0.5.1/buildABot/Data/Default - Recommended/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.350420 TPEBot-0.5.1/buildABot/Data/Entities/
+-rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Entities/LoginID.json
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.358722 TPEBot-0.5.1/buildABot/Data/WebApp/
+-rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/WebApp/index_template_LEARN.html
+-rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/WebApp/index_template_RECO.html
+-rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/WebApp/reset_template_RECO.js
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.374756 TPEBot-0.5.1/buildABot/Data/Webhook/
+-rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
+-rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
+-rw-rw-rw-   0        0        0     5497 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Webhook/index_template_LEARN.js
+-rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPEBot-0.5.1/buildABot/Data/Webhook/index_template_RECO.js
+-rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPEBot-0.5.1/buildABot/Data/__init__.py
+-rw-rw-rw-   0        0        0    15847 2023-05-16 14:52:32.000000 TPEBot-0.5.1/buildABot/Entities.py
+-rw-rw-rw-   0        0        0    12267 2023-05-16 14:52:32.000000 TPEBot-0.5.1/buildABot/FallbackSocialTag.py
+-rw-rw-rw-   0        0        0    12103 2023-05-16 14:52:32.000000 TPEBot-0.5.1/buildABot/Firebase_Learn.py
+-rw-rw-rw-   0        0        0    14879 2023-05-16 14:52:32.000000 TPEBot-0.5.1/buildABot/Firebase_Reco.py
+-rw-rw-rw-   0        0        0    36243 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Intents.py
+-rw-rw-rw-   0        0        0    42171 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/LearnMenu.py
+-rw-rw-rw-   0        0        0    72431 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Manager.py
+-rw-rw-rw-   0        0        0    15947 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Paraphraser.py
+-rw-rw-rw-   0        0        0     6151 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Password.py
+-rw-rw-rw-   0        0        0    44723 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/RecommendedMenu.py
+-rw-rw-rw-   0        0        0     8791 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/TelegramLogs.py
+-rw-rw-rw-   0        0        0     7539 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/WebApp_Learn.py
+-rw-rw-rw-   0        0        0    11283 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/WebApp_Reco.py
+-rw-rw-rw-   0        0        0     9259 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Webhook_Learn.py
+-rw-rw-rw-   0        0        0    19235 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Webhook_Reco.py
+-rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/Worksheets.py
+-rw-rw-rw-   0        0        0     5075 2023-05-16 14:52:33.000000 TPEBot-0.5.1/buildABot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.374756 TPEBot-0.5.1/buildABot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEBot-0.5.1/buildABot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.382914 TPEBot-0.5.1/parrot/
+-rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPEBot-0.5.1/parrot/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPEBot-0.5.1/parrot/demo.py
+-rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPEBot-0.5.1/parrot/filters.py
+-rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPEBot-0.5.1/parrot/parrot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:04:58.382914 TPEBot-0.5.1/parrot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEBot-0.5.1/parrot/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 15:04:58.382914 TPEBot-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-05-16 15:01:30.000000 TPEBot-0.5.1/setup.py
```

### Comparing `TPEBot-0.5.0/README.md` & `TPEBot-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/TPEBot.egg-info/SOURCES.txt` & `TPEBot-0.5.1/TPEBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Analytics.py` & `TPEBot-0.5.1/buildABot/Analytics.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Fallback Intent.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Default Welcome Intent.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Downvote.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Downvote_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Email Enquiry.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Exit Conversation.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - no.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Remember Name.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Log In_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Menu - Main.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Thankyou.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Thankyou_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Learn/Upvote.json` & `TPEBot-0.5.1/buildABot/Data/Default - Learn/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Fallback Intent.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Default Welcome Intent.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Downvote.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Downvote_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Email Enquiry.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Exit Conversation.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Remember Name.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Log In_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Menu - Main.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Thankyou.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Default - Recommended/Upvote.json` & `TPEBot-0.5.1/buildABot/Data/Default - Recommended/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/WebApp/index_template_LEARN.html` & `TPEBot-0.5.1/buildABot/Data/WebApp/index_template_LEARN.html`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/WebApp/index_template_RECO.html` & `TPEBot-0.5.1/buildABot/Data/WebApp/index_template_RECO.html`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/WebApp/reset_template_RECO.js` & `TPEBot-0.5.1/buildABot/Data/WebApp/reset_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Webhook/CheckPwd_Template_RECO.js` & `TPEBot-0.5.1/buildABot/Data/Webhook/CheckPwd_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js` & `TPEBot-0.5.1/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Webhook/index_template_LEARN.js` & `TPEBot-0.5.1/buildABot/Data/Webhook/index_template_LEARN.js`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Data/Webhook/index_template_RECO.js` & `TPEBot-0.5.1/buildABot/Data/Webhook/index_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Entities.py` & `TPEBot-0.5.1/buildABot/Entities.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/FallbackSocialTag.py` & `TPEBot-0.5.1/buildABot/FallbackSocialTag.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Firebase_Learn.py` & `TPEBot-0.5.1/buildABot/Firebase_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Firebase_Reco.py` & `TPEBot-0.5.1/buildABot/Firebase_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Intents.py` & `TPEBot-0.5.1/buildABot/Intents.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/LearnMenu.py` & `TPEBot-0.5.1/buildABot/LearnMenu.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Manager.py` & `TPEBot-0.5.1/buildABot/Manager.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Paraphraser.py` & `TPEBot-0.5.1/buildABot/Paraphraser.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Password.py` & `TPEBot-0.5.1/buildABot/Password.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/RecommendedMenu.py` & `TPEBot-0.5.1/buildABot/RecommendedMenu.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/TelegramLogs.py` & `TPEBot-0.5.1/buildABot/TelegramLogs.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/WebApp_Learn.py` & `TPEBot-0.5.1/buildABot/WebApp_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/WebApp_Reco.py` & `TPEBot-0.5.1/buildABot/WebApp_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Webhook_Learn.py` & `TPEBot-0.5.1/buildABot/Webhook_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Webhook_Reco.py` & `TPEBot-0.5.1/buildABot/Webhook_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/Worksheets.py` & `TPEBot-0.5.1/buildABot/Worksheets.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/__init__.py` & `TPEBot-0.5.1/buildABot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/buildABot/pytransform/__init__.py` & `TPEBot-0.5.1/buildABot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/parrot/__init__.py` & `TPEBot-0.5.1/parrot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/parrot/demo.py` & `TPEBot-0.5.1/parrot/demo.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/parrot/filters.py` & `TPEBot-0.5.1/parrot/filters.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/parrot/parrot.py` & `TPEBot-0.5.1/parrot/parrot.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/parrot/pytransform/__init__.py` & `TPEBot-0.5.1/parrot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEBot-0.5.0/setup.py` & `TPEBot-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TPEBot", # Replace with your own username
-    version="0.5.0",
+    version="0.5.1",
     author="Ester Goh",
     description="A TPEdu chatbot pakage",
     packages=setuptools.find_packages(),
     package_data={'': ['Data/*/*.js', 'Data/*/*.html', 'Data/*/*.json']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```

