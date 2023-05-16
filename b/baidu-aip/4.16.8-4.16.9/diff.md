# Comparing `tmp/baidu_aip-4.16.8-py3-none-any.whl.zip` & `tmp/baidu_aip-4.16.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 24023 bytes, number of entries: 19
+Zip file size: 26866 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      468 b- defN 22-Aug-18 07:38 aip/__init__.py
 -rw-r--r--  2.0 unx     7844 b- defN 22-Aug-18 07:38 aip/base.py
 -rw-r--r--  2.0 unx     3471 b- defN 22-Aug-18 07:38 aip/bodyanalysis.py
 -rw-r--r--  2.0 unx     1011 b- defN 22-Aug-18 07:38 aip/easydl.py
 -rw-r--r--  2.0 unx    10775 b- defN 22-Aug-18 07:38 aip/face.py
 -rw-r--r--  2.0 unx     6024 b- defN 22-Aug-18 07:38 aip/imagecensor.py
--rw-r--r--  2.0 unx    21706 b- defN 22-Aug-18 07:55 aip/imageclassify.py
+-rw-r--r--  2.0 unx    22656 b- defN 22-Dec-22 08:54 aip/imageclassify.py
 -rw-r--r--  2.0 unx     4347 b- defN 22-Aug-18 07:38 aip/imageprocess.py
--rw-r--r--  2.0 unx    14354 b- defN 22-Aug-18 07:38 aip/imagesearch.py
+-rw-r--r--  2.0 unx    18040 b- defN 22-Dec-07 06:26 aip/imagesearch.py
 -rw-r--r--  2.0 unx     2617 b- defN 22-Aug-18 07:38 aip/kg.py
--rw-r--r--  2.0 unx     6875 b- defN 22-Aug-18 07:38 aip/nlp.py
--rw-r--r--  2.0 unx    41789 b- defN 22-Aug-18 07:38 aip/ocr.py
+-rw-r--r--  2.0 unx    15727 b- defN 22-Dec-22 08:54 aip/nlp.py
+-rw-r--r--  2.0 unx    62385 b- defN 22-Dec-07 06:26 aip/ocr.py
 -rw-r--r--  2.0 unx     2108 b- defN 22-Aug-18 07:38 aip/speech.py
--rwxr-xr-x  2.0 unx      420 b- defN 22-Aug-18 07:38 baidu_aip-4.16.8.data/scripts/aip_client
--rw-r--r--  2.0 unx    11357 b- defN 22-Oct-25 07:23 baidu_aip-4.16.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      309 b- defN 22-Oct-25 07:23 baidu_aip-4.16.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-25 07:23 baidu_aip-4.16.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Oct-25 07:23 baidu_aip-4.16.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1426 b- defN 22-Oct-25 07:23 baidu_aip-4.16.8.dist-info/RECORD
-19 files, 136997 bytes uncompressed, 21757 bytes compressed:  84.1%
+-rwxr-xr-x  2.0 unx      420 b- defN 22-Aug-18 07:38 baidu_aip-4.16.9.data/scripts/aip_client
+-rw-r--r--  2.0 unx    11357 b- defN 22-Dec-22 11:30 baidu_aip-4.16.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      309 b- defN 22-Dec-22 11:30 baidu_aip-4.16.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Dec-22 11:30 baidu_aip-4.16.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 22-Dec-22 11:30 baidu_aip-4.16.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1427 b- defN 22-Dec-22 11:30 baidu_aip-4.16.9.dist-info/RECORD
+19 files, 171082 bytes uncompressed, 24600 bytes compressed:  85.6%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: aip/ocr.py
 Comment: 
 
 Filename: aip/speech.py
 Comment: 
 
-Filename: baidu_aip-4.16.8.data/scripts/aip_client
+Filename: baidu_aip-4.16.9.data/scripts/aip_client
 Comment: 
 
-Filename: baidu_aip-4.16.8.dist-info/LICENSE
+Filename: baidu_aip-4.16.9.dist-info/LICENSE
 Comment: 
 
-Filename: baidu_aip-4.16.8.dist-info/METADATA
+Filename: baidu_aip-4.16.9.dist-info/METADATA
 Comment: 
 
-Filename: baidu_aip-4.16.8.dist-info/WHEEL
+Filename: baidu_aip-4.16.9.dist-info/WHEEL
 Comment: 
 
-Filename: baidu_aip-4.16.8.dist-info/top_level.txt
+Filename: baidu_aip-4.16.9.dist-info/top_level.txt
 Comment: 
 
-Filename: baidu_aip-4.16.8.dist-info/RECORD
+Filename: baidu_aip-4.16.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aip/imageclassify.py

```diff
@@ -107,14 +107,17 @@
 
     # 车辆检测-高空版
     __vehicle_detect_highUrl = "https://aip.baidubce.com/rest/2.0/image-classify/v1/vehicle_detect_high"
 
     # 车辆分割
     __vehicle_seg_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/vehicle_seg";
 
+    __carClassifyV1Url = 'https://aip.baidubce.com/rest/2.0/vis-classify/v1/car'
+    __vehicleAttrClassifyV2Url = 'https://aip.baidubce.com/rest/2.0/image-classify/v2/vehicle_attr'
+
 
     def combinationByImage(self, image, scenes, options=None):
         """
         组合接口
         """
         options = options or {}
         data = {}
@@ -810,7 +813,30 @@
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__vehicle_seg_url, data)
 
+    def vehicleAttrClassifyV2Image(self, image, options=None):
+        """
+            车辆属性识别
+            接口使用说明: https://ai.baidu.com/ai-doc/VEHICLE/mk3hb3fde
+        """
+        options = options or {}
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data.update(options)
+        return self._request(self.__vehicleAttrClassifyV2Url, data)
+
+    def vehicleAttrClassifyV2Url(self, url, options=None):
+        """
+            车辆属性识别
+            接口使用说明: https://ai.baidu.com/ai-doc/VEHICLE/mk3hb3fde
+        """
+        options = options or {}
+        data = {}
+        data['url'] = url
+        data.update(options)
+        return self._request(self.__vehicleAttrClassifyV2Url, data)
+
+
```

## aip/imagesearch.py

```diff
@@ -16,14 +16,21 @@
 from .base import quote
 
 class AipImageSearch(AipBase):
 
     """
     图像搜索
     """
+    __materielAddUrl = "https://aip.baidubce.com/rest/2.0/image-classify/v1/realtime_search/materiel/add"
+
+    __materielSearchUrl = "https://aip.baidubce.com/rest/2.0/image-classify/v1/realtime_search/materiel/search"
+
+    __materielUpdateUrl = "https://aip.baidubce.com/rest/2.0/image-classify/v1/realtime_search/materiel/update"
+
+    __materielDeleteUrl = "https://aip.baidubce.com/rest/2.0/image-classify/v1/realtime_search/materiel/delete"
 
     __sameHqAddUrl = 'https://aip.baidubce.com/rest/2.0/realtime_search/same_hq/add'
 
     __sameHqSearchUrl = 'https://aip.baidubce.com/rest/2.0/realtime_search/same_hq/search'
 
     __sameHqUpdateUrl = 'https://aip.baidubce.com/rest/2.0/realtime_search/same_hq/update'
 
@@ -50,14 +57,152 @@
     __picturebookSearch = "https://aip.baidubce.com/rest/2.0/imagesearch/v1/realtime_search/picturebook/search"
 
     __picturebookDelete = "https://aip.baidubce.com/rest/2.0/imagesearch/v1/realtime_search/picturebook/delete"
 
     __picturebookUpdate = "https://aip.baidubce.com/rest/2.0/imagesearch/v1/realtime_search/picturebook/update"
 
 
+
+
+    def materielAdd(self, image, brief, options=None):
+        """
+            面料图片检索—入库
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data['brief'] = brief
+
+        data.update(options)
+
+        return self._request(self.__materielAddUrl, data)
+
+    def materielAddUrl(self, url, brief, options=None):
+        """
+            面料图片检索—入库
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+        data['brief'] = brief
+
+        data.update(options)
+
+        return self._request(self.__materielAddUrl, data)
+
+    def materielSearch(self, image, options=None):
+        """
+            面料图片检索—检索
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__materielSearchUrl, data)
+
+    def materielSearchUrl(self, url, options=None):
+        """
+            面料图片检索—检索
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__materielSearchUrl, data)
+
+
+    def materielUpdate(self, image, brief, options=None):
+        """
+            面料图片检索—更新
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data['brief'] = brief
+
+        data.update(options)
+
+        return self._request(self.__materielUpdateUrl, data)
+    
+    def materielUpdateUrl(self, url, brief, options=None):
+        """
+            面料图片检索—更新
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+        data['brief'] = brief
+
+        data.update(options)
+
+        return self._request(self.__materielUpdateUrl, data)
+    
+    def materielUpdateContSign(self, cont_sign, brief, options=None):
+        """
+            面料图片检索—更新
+        """
+        options = options or {}
+
+        data = {}
+        data['cont_sign'] = cont_sign
+        data['brief'] = brief
+
+        data.update(options)
+
+        return self._request(self.__materielUpdateUrl, data)       
+
+    def materielDeleteByImage(self, image, options=None):
+        """
+            面料图片检索—删除
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__materielDeleteUrl, data)
+    
+    def materielDeleteByUrl(self, url, options=None):
+        """
+            面料图片检索—删除
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__materielDeleteUrl, data)
+    
+    def materielDeleteBySign(self, cont_sign, options=None):
+        """
+            面料图片检索—删除
+        """
+        options = options or {}
+
+        data = {}
+        data['cont_sign'] = cont_sign
+
+        data.update(options)
+
+        return self._request(self.__materielDeleteUrl, data)         
+
     
     def sameHqAdd(self, image, brief, options=None):
         """
             相同图检索—入库
         """
         options = options or {}
```

## aip/nlp.py

```diff
@@ -47,14 +47,34 @@
 
     __emotionUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/emotion'
 
     __newsSummaryUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/news_summary'
 
     __addressUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/address'
 
+    __commentTagCustomUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v2/comment_tag_custom'
+    __sentimentClassifyCustomUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/sentiment_classify_custom'
+    __coupletsUrl = 'https://aip.baidubce.com/rpc/2.0/creation/v1/couplets'
+    __poemUrl = 'https://aip.baidubce.com/rpc/2.0/creation/v1/poem'
+    __entityLevelSentimentUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment'
+    __entityLevelSentimentAddUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment/add'
+    __entityLevelSentimentDeleteUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment/delete'
+    __entityLevelSentimentDeleteRepoUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment/delete_repo'
+    __entityLevelSentimentListUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment/list'
+    __entityLevelSentimentQueryUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_level_sentiment/query'
+    __topicPhraseUrl = 'https://aip.baidubce.com/rpc/2.0/creation/v1/topic_phrase'
+    __cvparserUrl = 'https://aip.baidubce.com/rpc/2.0/recruitment/v1/cvparser'
+    __personPostUrl = 'https://aip.baidubce.com/rpc/2.0/recruitment/v1/person_post'
+    __personasUrl = 'https://aip.baidubce.com/rpc/2.0/recruitment/v1/personas'
+    __titlepredictorUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/titlepredictor'
+    __depparserV2Url = 'https://aip.baidubce.com/rpc/2.0/nlp/v2/depparser'
+    __blessCreationUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/bless_creation'
+    __entityAnalysisUrl = 'https://aip.baidubce.com/rpc/2.0/nlp/v1/entity_analysis'
+
+
     def _proccessResult(self, content):
         """
             formate result
         """
 
         if sys.version_info.major == 2:
             if chardet.detect(content).get('encoding') == 'utf-8':
@@ -275,7 +295,263 @@
 
         data = {}
         data['text'] = text
 
         data.update(options)
 
         return self._request(self.__addressUrl, data)
+
+    def commentTagCustom(self, text, options=None):
+        """
+            评论观点抽取（定制）
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/ok6z52g8q
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__commentTagCustomUrl, data)
+
+    def sentimentClassifyCustom(self, text, options=None):
+        """
+            情感倾向分析（定制）
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/zk6z52hds
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__sentimentClassifyCustomUrl, data)
+
+    def couplets(self, text, options=None):
+        """
+            智能春联
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Ok53wb6dh
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__coupletsUrl, data)
+
+    def poem(self, text, options=None):
+        """
+            智能写诗
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/ak53wc3o3
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__poemUrl, data)
+
+    def entityLevelSentiment(self, title, content, type, options=None):
+        """
+            实体抽取与情感倾向分析
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04
+        """
+        options = options or {}
+
+        data = {}
+        data['title'] = title
+        data['content'] = content
+        data['type'] = type
+
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentUrl, data)
+
+    def entityLevelSentimentAdd(self, repository, entities, options=None):
+        """
+            增加实体/实体库新增
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04#%E5%AE%9E%E4%BD%93%E5%BA%93%E6%96%B0%E5%A2%9E%E6%8E%A5%E5%8F%A3
+        """
+        options = options or {}
+
+        data = {}
+        data['repository'] = repository
+        data['entities'] = entities
+
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentAddUrl, data)
+
+    def entityLevelSentimentDelete(self, repository, entities, options=None):
+        """
+            删除实体/实体名单删除
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04#%E5%AE%9E%E4%BD%93%E5%90%8D%E5%8D%95%E5%88%A0%E9%99%A4%E6%8E%A5%E5%8F%A3
+        """
+        options = options or {}
+
+        data = {}
+        data['repository'] = repository
+        data['entities'] = entities
+
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentDeleteUrl, data)
+
+    def entityLevelSentimentDeleteRepo(self, repositories, options=None):
+        """
+            删除实体库/实体库删除
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04#%E5%AE%9E%E4%BD%93%E5%BA%93%E5%88%A0%E9%99%A4%E6%8E%A5%E5%8F%A3
+        """
+        options = options or {}
+
+        data = {}
+        data['repositories'] = repositories
+
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentDeleteRepoUrl, data)
+
+    def entityLevelSentimentList(self, options=None):
+        """
+            实体库列表/实体库查询
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04#%E5%AE%9E%E4%BD%93%E5%BA%93%E6%9F%A5%E8%AF%A2%E6%8E%A5%E5%8F%A3
+        """
+        options = options or {}
+        data = {}
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentListUrl, data)
+
+    def entityLevelSentimentQuery(self, repository, options=None):
+        """
+            查询实体/实体名单查询
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Fk6z52g04#%E5%AE%9E%E4%BD%93%E5%90%8D%E5%8D%95%E6%9F%A5%E8%AF%A2%E6%8E%A5%E5%8F%A3
+        """
+        options = options or {}
+
+        data = {}
+        data['repository'] = repository
+
+        data.update(options)
+
+        return self._request(self.__entityLevelSentimentQueryUrl, data)
+
+    def topicPhrase(self, title, summary, options=None):
+        """
+            文章主题短语生成
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/9k53w3qob
+        """
+        options = options or {}
+
+        data = {}
+        data['title'] = title
+        data['summary'] = summary
+
+        data.update(options)
+
+        return self._request(self.__topicPhraseUrl, data)
+
+    def recruitmentCvparser(self, resume, options=None):
+        """
+            智能招聘-简历解析
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Xkahvfeqa
+        """
+        options = options or {}
+
+        data = {}
+        data['resume'] = resume
+
+        data.update(options)
+
+        return self._request(self.__cvparserUrl, data)
+
+    def recruitmentPersonPost(self, resume, job_description, options=None):
+        """
+            智能招聘-人岗匹配
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/Pkahwzux5
+        """
+        options = options or {}
+
+        data = {}
+        data['resume'] = resume
+        data['job_description'] = job_description
+
+        data.update(options)
+
+        return self._request(self.__personPostUrl, data)
+
+    def recruitmentPersonas(self, resume, options=None):
+        """
+            智能招聘-简历画像
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/5kc1kmz3w
+        """
+        options = options or {}
+
+        data = {}
+        data['resume'] = resume
+
+        data.update(options)
+
+        return self._request(self.__personasUrl, data)
+
+    def titlepredictor(self, doc, options=None):
+        """
+            文章标题生成
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/0kvc1u1eg
+        """
+        options = options or {}
+
+        data = {}
+        data['doc'] = doc
+
+        data.update(options)
+
+        return self._request(self.__titlepredictorUrl, data)
+        
+    def depParserV2(self, text, options=None):
+        """
+            依存句法分析V2
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/nk6z52eu6
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__depparserV2Url, data)
+
+    def blessCreation(self, text, options=None):
+        """
+            祝福语生成
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/sl4cg75jk
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__blessCreationUrl, data)
+
+    def entityAnalysis(self, text, options=None):
+        """
+            实体分析
+            接口文档链接: https://ai.baidu.com/ai-doc/NLP/al631z295
+        """
+        options = options or {}
+
+        data = {}
+        data['text'] = text
+
+        data.update(options)
+
+        return self._request(self.__entityAnalysisUrl, data)
+
```

## aip/ocr.py

```diff
@@ -1,32 +1,32 @@
-
 # -*- coding: utf-8 -*-
 
 """
-文字识别
+文字识别HTTP SDK
+
 """
 
 import re
 import sys
 import math
 import time
 from .base import AipBase
 from .base import base64
 from .base import json
 from .base import urlencode
 from .base import quote
 
 
-
 class AipOcr(AipBase):
-
     """
     文字识别
     """
 
+    """通用场景文字识别"""
+
     # 通用文字识别（高精度版）
     __accurateBasicUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/accurate_basic'
 
     # 通用文字识别（高精度含位置版）
     __accurateUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/accurate'
 
     # 通用文字识别（标准版）
@@ -55,28 +55,33 @@
 
     # 表格文字识别（异步接口）--获取结果
     __tableResultGetUrl = 'https://aip.baidubce.com/rest/2.0/solution/v1/form_ocr/get_request_result'
 
     # 手写文字识别
     __handwritingUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/handwriting'
 
+    # 表格文字识别V2
+    __tableUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/table'
+
     # 数字识别
     __numbersUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/numbers'
 
     # 二维码识别
     __qrcodeUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/qrcode'
 
     # 通用文字识别（含生僻字版）已停止更新
     __generalEnhancedUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/general_enhanced'
 
+    """卡证文字识别"""
+
     # 身份证识别
     __idcardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/idcard'
 
-    # 身份证混贴识别（邀测）
-    # 暂不封装，待公测后更新
+    # 身份证混贴识别
+    __multi_idcardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/multi_idcard'
 
     # 身份证识别（金融加密版）
     # 无
 
     # 银行卡识别
     __bankcardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/bankcard'
 
@@ -85,31 +90,33 @@
 
     # 名片识别
     __businessCardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/business_card'
 
     # 护照识别
     __passportUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/passport'
 
-    # 社保卡识别（邀测）
-    # 暂不封装，待公测后更新
+    # 社保卡识别
+    __social_security_cardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/social_security_card'
 
     # 港澳通行证识别
     __HKMacauExitentrypermitUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/HK_Macau_exitentrypermit'
 
     # 台湾通行证识别
     __taiwanExitentrypermitUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/taiwan_exitentrypermit'
 
     # 户口本识别
     __householdRegisterUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/household_register'
 
     # 出生医学证明识别
     __birthCertificateUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/birth_certificate'
 
-    # 多卡证类别检测（邀测）
-    # 暂不封装，待公测后更新
+    # 多卡证类别检测
+    __multi_card_classifyUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/multi_card_classify'
+
+    """交通场景文字识别"""
 
     # 行驶证识别
     __vehicleLicenseUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vehicle_license'
 
     # 驾驶证识别
     __drivingLicenseUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/driving_license'
 
@@ -121,31 +128,36 @@
 
     # VIN码识别
     __vinCodeUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vin_code'
 
     # 机动车销售发票识别
     __vehicleInvoiceUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vehicle_invoice'
 
-    # 二手车销售发票识别（邀测）
-    # 暂不封装，待公测后更新
+    # 二手车销售发票识别
+    __used_vehicle_invoiceUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/used_vehicle_invoice'
 
     # 车辆合格证识别
     __vehicleCertificateUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vehicle_certificate'
 
     # 机动车登记证书识别
     __vehicle_registration_certificateUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vehicle_registration_certificate'
 
     # 磅单识别
     __weight_noteUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/weight_note"
 
-    # 快递面单识别（邀测）
-    # 暂不封装，待公测后更新
+    # 快递面单识别
+    __waybillUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/waybill'
+
+    # 道路运输证识别
+    __road_transport_certificateUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/road_transport_certificate'
+
+    """财务票据文字识别"""
 
     # 智能财务票据识别
-    __multipleInvoiceUrl ="https://aip.baidubce.com/rest/2.0/ocr/v1/multiple_invoice"
+    __multipleInvoiceUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/multiple_invoice"
 
     # 增值税发票识别
     __vatInvoiceUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/vat_invoice'
 
     # 增值税发票验真
     __vat_invoice_verificationUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/vat_invoice_verification"
 
@@ -160,82 +172,118 @@
 
     # 出租车票识别
     __taxiReceiptUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/taxi_receipt'
 
     # 飞机行程单识别
     __airTicketUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/air_ticket'
 
-    # 汽车票识别（邀测）
-    # 暂不封装，待公测后更新
+    # 汽车票识别
+    __bus_ticketUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/bus_ticket'
 
-    # 过路过桥费发票识别（邀测）
-    # 暂不封装，待公测后更新
+    # 过路过桥费发票识别
+    __toll_invoiceUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/toll_invoice'
 
-    # 船票识别（邀测）
-    # 暂不封装，待公测后更新
+    # 船票识别
+    __ferry_ticketUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/ferry_ticket'
 
     # 网约车行程单识别
     __online_taxi_itineraryUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/online_taxi_itinerary"
 
     # 通用票据识别
     __receiptUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/receipt'
 
-    # 购物小票识别（邀测）
-    # 暂不封装，待公测后更新
+    # 购物小票识别
+    __shopping_receiptUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/shopping_receipt'
+
+    """医疗票据文字识别"""
 
     # 医疗发票识别
     __medicalInvoiceUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/medical_invoice"
 
     # 医疗费用明细识别
     __medical_detailUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/medical_detail"
 
-    # 医疗费用结算单识别（邀测）
-    # 暂不封装，待公测后更新
+    # 医疗费用结算单识别
+    __medical_statementUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_statement'
+
+    # 医疗检验报告单识别
+    __medical_report_detectionUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_report_detection'
+
+    # 医疗诊断报告单识别
+    __health_reportUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/health_report'
+
+    # 病案首页识别
+    __medical_recordUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_record'
+
+    # 出院小结识别
+    __medical_summaryUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_summary'
 
-    # 医疗检验报告单识别（邀测）
-    # 暂不封装，待公测后更新
+    # 诊断证明识别
+    __medical_summary_diagnosisUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_summary_diagnosis'
 
-    # 病案首页识别（邀测）
-    # 暂不封装，待公测后更新
+    # 门诊病历识别
+    __medical_outpatientUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_outpatient'
 
-    # 出院小结识别（邀测）
-    # 暂不封装，待公测后更新
+    # 处方笺识别
+    __medical_prescriptionUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_prescription'
 
-    # 医疗票据类别检测（邀测）
-    # 暂不封装，待公测后更新
+    # 医疗票据类别检测
+    __medical_recipts_classifyUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/medical_recipts_classify'
 
     # 保险单识别
     __insuranceDocumentsUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/insurance_documents'
 
+    """防疫场景文字识别"""
+
+    # 通信行程卡识别
+    __travel_cardUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/travel_card'
+
+    # 健康码识别
+    __health_codeUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/health_code'
+
+    # 核酸证明识别
+    __covid_testUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/covid_test'
+
+    """教育场景文字识别"""
+
     # 试卷分析与识别
     __docAnalysis = "https://aip.baidubce.com/rest/2.0/ocr/v1/doc_analysis"
 
-    # 公式识别（公测）
+    # 公式识别
     __formulaUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/formula"
 
+    """其他场景文字识别"""
+
     # 仪器仪表盘读数识别
     __meter = "https://aip.baidubce.com/rest/2.0/ocr/v1/meter"
 
-    # 通信行程卡识别（公测）
-    # 无
-
-    # 彩票识别（邀测）
+    # 彩票识别
     __lotteryUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/lottery'
 
     # 门脸文字识别
     __facadeUrl = "https://aip.baidubce.com/rest/2.0/ocr/v1/facade"
 
-    # 智能结构化识别（邀测）
-    # 暂不封装，待公测后更新
+    # 智能结构化识别
+    __intelligent_ocrUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/intelligent_ocr'
+
+    """文档图像处理"""
+
+    # 文档矫正增强
+    __doc_crop_enhanceUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/doc_crop_enhance'
+
+    # 文档去手写
+    __remove_handwritingUrl = 'https://aip.baidubce.com/rest/2.0/ocr/v1/remove_handwriting'
+
+    """iOCR自定义模板文字识别"""
 
     # iOCR通用版
     __customUrl = 'https://aip.baidubce.com/rest/2.0/solution/v1/iocr/recognise'
 
     # iOCR财会版
-    # 暂不封装，不是主要维护方向
+    __custom_financeUrl = 'https://aip.baidubce.com/rest/2.0/solution/v1/iocr/recognise/finance'
 
     def basicAccurate(self, image, options=None):
         """
             通用文字识别（高精度版）
         """
         options = options or {}
 
@@ -319,15 +367,15 @@
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__generalBasicUrl, data)
-    
+
     def basicGeneralUrl(self, url, options=None):
         """
             通用文字识别（标准版）_url图片方式
         """
         options = options or {}
 
         data = {}
@@ -358,15 +406,15 @@
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__generalUrl, data)
-    
+
     def generalUrl(self, url, options=None):
         """
             通用文字识别（标准含位置版）_url图片方式
         """
         options = options or {}
 
         data = {}
@@ -642,14 +690,53 @@
         data = {}
         data['pdf_file'] = base64.b64encode(pdf_file).decode()
 
         data.update(options)
 
         return self._request(self.__handwritingUrl, data)
 
+    def table(self, image, options=None):
+        """
+            表格文字识别V2
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__tableUrl, data)
+
+    def tableUrl(self, url, options=None):
+        """
+            表格文字识别V2_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__tableUrl, data)
+
+    def tablePdf(self, pdf_file, options=None):
+        """
+            表格文字识别V2_pdf文件方式
+        """
+        options = options or {}
+
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+
+        data.update(options)
+
+        return self._request(self.__tableUrl, data)
+
     def numbers(self, image, options=None):
         """
             数字识别
         """
         options = options or {}
 
         data = {}
@@ -706,28 +793,28 @@
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__generalEnhancedUrl, data)
-    
+
     def enhancedGeneralUrl(self, url, options=None):
         """
             通用文字识别（含生僻字版）_url图片方式已停止更新
         """
         options = options or {}
 
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__generalEnhancedUrl, data)
-    
+
     def idcard(self, image, id_card_side, options=None):
         """
             身份证识别
         """
         options = options or {}
 
         data = {}
@@ -747,15 +834,41 @@
         data = {}
         data['url'] = url
         data['id_card_side'] = id_card_side
 
         data.update(options)
 
         return self._request(self.__idcardUrl, data)
-    
+
+    def multi_idcard(self, image, options=None):
+        """
+            身份证混贴识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__multi_idcardUrl, data)
+
+    def multi_idcardUrl(self, url, options=None):
+        """
+            身份证混贴识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__multi_idcardUrl, data)
+
     def bankcard(self, image, options=None):
         """
             银行卡识别
         """
         options = options or {}
 
         data = {}
@@ -839,14 +952,40 @@
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__passportUrl, data)
 
+    def social_security_card(self, image, options=None):
+        """
+            社保卡识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__social_security_cardUrl, data)
+
+    def social_security_cardUrl(self, url, options=None):
+        """
+           社保卡识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__social_security_cardUrl, data)
+
     def HKMacauExitentrypermit(self, image, options=None):
         """
             港澳通行证识别
         """
         options = options or {}
 
         data = {}
@@ -904,14 +1043,53 @@
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__birthCertificateUrl, data)
 
+    def birthCertificateUrl(self, url, options=None):
+        """
+            出生医学证明识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__birthCertificateUrl, data)
+
+    def multi_card_classify(self, image, options=None):
+        """
+            多卡证类别检测
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__multi_card_classifyUrl, data)
+
+    def multi_card_classifyUrl(self, url, options=None):
+        """
+            多卡证类别检测_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__multi_card_classifyUrl, data)
+
     def vehicleLicense(self, image, options=None):
         """
             行驶证识别
         """
         options = options or {}
 
         data = {}
@@ -929,15 +1107,15 @@
 
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__vehicleLicenseUrl, data)
-    
+
     def drivingLicense(self, image, options=None):
         """
             驾驶证识别
         """
         options = options or {}
 
         data = {}
@@ -955,15 +1133,15 @@
 
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__drivingLicenseUrl, data)
-    
+
     def licensePlate(self, image, options=None):
         """
             车牌识别
         """
         options = options or {}
 
         data = {}
@@ -1057,14 +1235,40 @@
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__vehicleInvoiceUrl, data)
 
+    def used_vehicle_invoice(self, image, options=None):
+        """
+            二手车销售发票识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__used_vehicle_invoiceUrl, data)
+
+    def used_vehicle_invoiceUrl(self, url, options=None):
+        """
+            二手车销售发票识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__used_vehicle_invoiceUrl, data)
+
     def vehicleCertificate(self, image, options=None):
         """
             车辆合格证识别
         """
         options = options or {}
 
         data = {}
@@ -1118,47 +1322,108 @@
             磅单识别
         """
         options = options or {}
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
-
         data.update(options)
 
         return self._request(self.__weight_noteUrl, data)
 
     def weightNoteUrl(self, url, options=None):
         """
             磅单识别_url图片方式
         """
         options = options or {}
 
         data = {}
         data['url'] = url
 
-
         data.update(options)
 
         return self._request(self.__weight_noteUrl, data)
 
     def weightNotePdf(self, pdf_file, options=None):
         """
             磅单识别_pdf文件方式
         """
         options = options or {}
 
         data = {}
         data['pdf_file'] = base64.b64encode(pdf_file).decode()
 
-
         data.update(options)
 
         return self._request(self.__weight_noteUrl, data)
 
+    def waybill(self, image, options=None):
+        """
+            快递面单识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__waybillUrl, data)
+
+    def waybillUrl(self, url, options=None):
+        """
+            快递面单识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__waybillUrl, data)
+
+    def road_transport_certificate(self, image, options=None):
+        """
+            道路运输证识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+        return self._request(self.__road_transport_certificateUrl, data)
+
+    def road_transport_certificateUrl(self, url, options=None):
+        """
+            道路运输证识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__road_transport_certificateUrl, data)
+
+    def road_transport_certificatePdf(self, pdf_file, options=None):
+        """
+            道路运输证识别_pdf文件方式
+        """
+        options = options or {}
+
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+
+        data.update(options)
+
+        return self._request(self.__road_transport_certificateUrl, data)
+
     def multipleInvoice(self, image, options=None):
         """
             智能财务票据识别
         """
         options = options or {}
 
         data = {}
@@ -1410,14 +1675,92 @@
         data = {}
         data['pdf_file'] = base64.b64encode(pdf_file).decode()
 
         data.update(options)
 
         return self._request(self.__airTicketUrl, data)
 
+    def bus_ticket(self, image, options=None):
+        """
+            汽车票识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__bus_ticketUrl, data)
+
+    def bus_ticketUrl(self, url, options=None):
+        """
+            汽车票识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__bus_ticketUrl, data)
+
+    def toll_invoice(self, image, options=None):
+        """
+            过路过桥费发票识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__toll_invoiceUrl, data)
+
+    def toll_invoiceUrl(self, url, options=None):
+        """
+            过路过桥费发票识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__toll_invoiceUrl, data)
+
+    def ferry_ticket(self, image, options=None):
+        """
+            船票识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__ferry_ticketUrl, data)
+
+    def ferry_ticketUrl(self, url, options=None):
+        """
+            船票识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__ferry_ticketUrl, data)
+
     def onlineTaxiItinerary(self, image):
         """
             网约车行程单识别
         """
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
@@ -1467,14 +1810,53 @@
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__receiptUrl, data)
 
+    def shopping_receipt(self, image, options=None):
+        """
+            购物小票识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__shopping_receiptUrl, data)
+
+    def shopping_receiptUrl(self, url, options=None):
+        """
+            购物小票识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__shopping_receiptUrl, data)
+
+    def shopping_receiptPdf(self, pdf_file, options=None):
+        """
+            购物小票识别_pdf文件方式
+        """
+        options = options or {}
+
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+
+        data.update(options)
+
+        return self._request(self.__shopping_receiptUrl, data)
+
     def medicalInvoice(self, image, options=None):
         """
             医疗发票识别
         """
         options = options or {}
 
         data = {}
@@ -1491,25 +1873,24 @@
 
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__medicalInvoiceUrl, data)
-    
+
     def medicalDetail(self, image, options=None):
         """
             医疗费用明细识别
         """
         options = options or {}
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
-
         data.update(options)
 
         return self._request(self.__medical_detailUrl, data)
 
     def medicalDetailUrl(self, url, options=None):
         """
             医疗费用明细识别_url图片方式
@@ -1519,27 +1900,300 @@
         data = {}
         data['url'] = url
 
         data.update(options)
 
         return self._request(self.__medical_detailUrl, data)
 
+    def medical_statement(self, image, options=None):
+        """
+            医疗费用结算单识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_statementUrl, data)
+
+    def medical_statementUrl(self, url, options=None):
+        """
+            医疗费用结算单识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_statementUrl, data)
+
+    def medical_report_detection(self, image, options=None):
+        """
+            医疗检验报告单识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_report_detectionUrl, data)
+
+    def medical_report_detectionUrl(self, url, options=None):
+        """
+            医疗检验报告单识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_report_detectionUrl, data)
+
+    def health_report(self, image, options=None):
+        """
+            医疗诊断报告单识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__health_reportUrl, data)
+
+    def health_reportUrl(self, url, options=None):
+        """
+            医疗诊断报告单识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__health_reportUrl, data)
+
+    def medical_record(self, image, options=None):
+        """
+            病案首页识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_recordUrl, data)
+
+    def medical_recordUrl(self, url, options=None):
+        """
+            病案首页识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_recordUrl, data)
+
+    def medical_summary(self, image, options=None):
+        """
+            出院小结识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_summaryUrl, data)
+
+    def medical_summaryUrl(self, url, options=None):
+        """
+            出院小结识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_summaryUrl, data)
+
+    def medical_summary_diagnosis(self, image, options=None):
+        """
+            诊断证明识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_summary_diagnosisUrl, data)
+
+    def medical_summary_diagnosisUrl(self, url, options=None):
+        """
+            诊断证明识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_summary_diagnosisUrl, data)
+
+    def medical_outpatient(self, image, options=None):
+        """
+            门诊病历识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_outpatientUrl, data)
+
+    def medical_outpatientUrl(self, url, options=None):
+        """
+            门诊病历识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_outpatientUrl, data)
+
+    def medical_prescription(self, image, options=None):
+        """
+            处方笺识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_prescriptionUrl, data)
+
+    def medical_prescriptionUrl(self, url, options=None):
+        """
+            处方笺识别_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_prescriptionUrl, data)
+
+    def medical_recipts_classify(self, image, options=None):
+        """
+           医疗票据类别检测
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__medical_recipts_classifyUrl, data)
+
+    def medical_recipts_classifyUrl(self, url, options=None):
+        """
+            医疗票据类别检测_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__medical_recipts_classifyUrl, data)
+
     def insuranceDocuments(self, image, options=None):
         """
             保险单识别
         """
         options = options or {}
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__insuranceDocumentsUrl, data)
 
+    def travel_card(self, image, options=None):
+        """
+            通信行程卡识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__travel_cardUrl, data)
+
+    def health_code(self, image, options=None):
+        """
+            健康码识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__health_codeUrl, data)
+
+    def covid_test(self, image, options=None):
+        """
+            核酸证明识别
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__covid_testUrl, data)
+
     def docAnalysis(self, image, options=None):
         """
             试卷分析与识别
         """
         options = options or {}
         data = {}
         data['image'] = base64.b64encode(image).decode()
@@ -1642,20 +2296,173 @@
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__facadeUrl, data)
-    
+
+    def intelligent_ocr(self, image, options=None):
+        """
+            智能结构化识别
+        """
+        options = options or {}
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data.update(options)
+
+        return self._request(self.__intelligent_ocrUrl, data)
+
+    def intelligent_ocrUrl(self, url, options=None):
+        """
+            智能结构化识别_url图片方式
+        """
+        options = options or {}
+        data = {}
+        data['url'] = url
+        data.update(options)
+
+        return self._request(self.__intelligent_ocrUrl, data)
+
+    def doc_crop_enhance(self, image, options=None):
+        """
+            文档矫正增强
+        """
+        options = options or {}
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data.update(options)
+
+        return self._request(self.__doc_crop_enhanceUrl, data)
+
+    def doc_crop_enhanceUrl(self, url, options=None):
+        """
+            文档矫正增强_url图片方式
+        """
+        options = options or {}
+        data = {}
+        data['url'] = url
+        data.update(options)
+
+        return self._request(self.__doc_crop_enhanceUrl, data)
+
+    def doc_crop_enhancePdf(self, pdf_file, options=None):
+        """
+            文档矫正增强_pdf文件方式
+        """
+        options = options or {}
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+        data.update(options)
+
+        return self._request(self.__doc_crop_enhanceUrl, data)
+
+    def remove_handwriting(self, image, options=None):
+        """
+            文档去手写
+        """
+        options = options or {}
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+        data.update(options)
+
+        return self._request(self.__remove_handwritingUrl, data)
+
+    def remove_handwritingUrl(self, url, options=None):
+        """
+            文档去手写_url图片方式
+        """
+        options = options or {}
+        data = {}
+        data['url'] = url
+        data.update(options)
+
+        return self._request(self.__remove_handwritingUrl, data)
+
+    def remove_handwritingPdf(self, pdf_file, options=None):
+        """
+            文档去手写_pdf文件方式
+        """
+        options = options or {}
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+        data.update(options)
+
+        return self._request(self.__remove_handwritingUrl, data)
+
     def custom(self, image, options=None):
         """
             iOCR通用版
         """
         options = options or {}
 
         data = {}
         data['image'] = base64.b64encode(image).decode()
 
         data.update(options)
 
         return self._request(self.__customUrl, data)
+
+    def customUrl(self, url, options=None):
+        """
+            iOCR通用版_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__customUrl, data)
+
+    def customPdf(self, pdf_file, options=None):
+        """
+            iOCR通用版_pdf文件方式
+        """
+        options = options or {}
+
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+
+        data.update(options)
+
+        return self._request(self.__customUrl, data)
+
+    def custom_finance(self, image, options=None):
+        """
+            iOCR财会版
+        """
+        options = options or {}
+
+        data = {}
+        data['image'] = base64.b64encode(image).decode()
+
+        data.update(options)
+
+        return self._request(self.__custom_financeUrl, data)
+
+    def custom_financeUrl(self, url, options=None):
+        """
+            iOCR财会版_url图片方式
+        """
+        options = options or {}
+
+        data = {}
+        data['url'] = url
+
+        data.update(options)
+
+        return self._request(self.__custom_financeUrl, data)
+
+    def custom_financePdf(self, pdf_file, options=None):
+        """
+            iOCR财会版_pdf文件方式
+        """
+        options = options or {}
+
+        data = {}
+        data['pdf_file'] = base64.b64encode(pdf_file).decode()
+
+        data.update(options)
+
+        return self._request(self.__custom_financeUrl, data)
```

## Comparing `baidu_aip-4.16.8.dist-info/LICENSE` & `baidu_aip-4.16.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `baidu_aip-4.16.8.dist-info/RECORD` & `baidu_aip-4.16.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 aip/__init__.py,sha256=tKk552A6U9y7YnWtpxvOlfrcViJygzu151G1LgMPOhs,468
 aip/base.py,sha256=MdV0sEePX_inaSMlkEdT8hi0vDx4bLvlJvso3QBcAik,7844
 aip/bodyanalysis.py,sha256=YiDVbyZ-iipO6QigPjtsOKmeHLTPrygTYUpQOuXkGVU,3471
 aip/easydl.py,sha256=9_q62PH_J56UqSaLM1ejxFm4mhzGf2_xXpXxuI9scvI,1011
 aip/face.py,sha256=TPDXfv5V985rXYSBUEmhsIu-IC5_egMizH_obYdPoe0,10775
 aip/imagecensor.py,sha256=OI34gbE0Phid-6rA49_zLvXLvrq1aH1uxsEpIORmCC0,6024
-aip/imageclassify.py,sha256=lprDilG4UuE2CFzM51u6gE4cEHiv7iM84KGNL4CLnSo,21706
+aip/imageclassify.py,sha256=pBIBBxy0Kp1Isd20H7Sia_1mNUNcCwaNFTBkmw0NdZ0,22656
 aip/imageprocess.py,sha256=GyeYzSN6g9kTwFfkHAV8Un_BJ7snHoSnLHM-4UjR4eU,4347
-aip/imagesearch.py,sha256=5mI2Nlr5w7cOXfvwCml5k0UnfQuKUAMdMiC6qoFf4zM,14354
+aip/imagesearch.py,sha256=QRmUyAdxeHZt_rxfRg7Jlubpp9rY1HLLDY2GnDlpZcs,18040
 aip/kg.py,sha256=GWnpHPH7-xWZH8vKRxat_dVdPhK9Quy6TukfeS7CJAE,2617
-aip/nlp.py,sha256=yXCtZyiFdzPjmyCOVsjY88088slMw4WDifYFA5_XbZs,6875
-aip/ocr.py,sha256=8BDBBAPVKZb6-1-EhbTIYwkORV1iF4Z6fgDvw2CCePk,41789
+aip/nlp.py,sha256=yfqWa5d-fnVEYQbm8SO50yp65rBj2ZanbCBWOe-S7sQ,15727
+aip/ocr.py,sha256=f0ieKOd5QhtkaL5g7JPCdSjDFK0Ax8lCRs88hXH4Mo4,62385
 aip/speech.py,sha256=vddwMCUrfg8R1ofDZOgrJWShB-6St5MmIfg0gA0OGes,2108
-baidu_aip-4.16.8.data/scripts/aip_client,sha256=wugufptMm_fhk-eXcl7poG6VHjN2YULioYBpLIkZN6o,420
-baidu_aip-4.16.8.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-baidu_aip-4.16.8.dist-info/METADATA,sha256=tIMKV4QXOy8AlT5ZdKtxj5aumFB0DyE95bwDtUyhpPQ,309
-baidu_aip-4.16.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-baidu_aip-4.16.8.dist-info/top_level.txt,sha256=Wnb2qhdNwCL-tN1ehbCyVY0QR-OF5uvO4xNuHG8LX2w,4
-baidu_aip-4.16.8.dist-info/RECORD,,
+baidu_aip-4.16.9.data/scripts/aip_client,sha256=wugufptMm_fhk-eXcl7poG6VHjN2YULioYBpLIkZN6o,420
+baidu_aip-4.16.9.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+baidu_aip-4.16.9.dist-info/METADATA,sha256=nOzpwSbyA8cvJ9QmUASMalGqcC7a3XcjlSHAdNhCeS4,309
+baidu_aip-4.16.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+baidu_aip-4.16.9.dist-info/top_level.txt,sha256=Wnb2qhdNwCL-tN1ehbCyVY0QR-OF5uvO4xNuHG8LX2w,4
+baidu_aip-4.16.9.dist-info/RECORD,,
```

