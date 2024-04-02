# Comparing `tmp/LangSegment-0.2.8-py3-none-any.whl.zip` & `tmp/LangSegment-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 20509 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    43092 b- defN 24-Mar-20 17:53 LangSegment/LangSegment.py
--rw-rw-rw-  2.0 fat      250 b- defN 24-Mar-20 17:53 LangSegment/__init__.py
--rw-rw-rw-  2.0 fat    14714 b- defN 24-Mar-20 17:55 LangSegment-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-20 17:55 LangSegment-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-20 17:55 LangSegment-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 24-Mar-20 17:55 LangSegment-0.2.8.dist-info/RECORD
-6 files, 58638 bytes uncompressed, 19645 bytes compressed:  66.5%
+Zip file size: 20588 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    43484 b- defN 24-Apr-02 14:58 LangSegment/LangSegment.py
+-rw-rw-rw-  2.0 fat      250 b- defN 24-Apr-02 14:59 LangSegment/__init__.py
+-rw-rw-rw-  2.0 fat    14714 b- defN 24-Apr-02 15:00 LangSegment-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 15:00 LangSegment-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-02 15:00 LangSegment-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 24-Apr-02 15:00 LangSegment-0.2.9.dist-info/RECORD
+6 files, 59030 bytes uncompressed, 19724 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: LangSegment/LangSegment.py
 Comment: 
 
 Filename: LangSegment/__init__.py
 Comment: 
 
-Filename: LangSegment-0.2.8.dist-info/METADATA
+Filename: LangSegment-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: LangSegment-0.2.8.dist-info/WHEEL
+Filename: LangSegment-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: LangSegment-0.2.8.dist-info/top_level.txt
+Filename: LangSegment-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: LangSegment-0.2.8.dist-info/RECORD
+Filename: LangSegment-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## LangSegment/LangSegment.py

```diff
@@ -431,14 +431,24 @@
             if len(cleans_text) <= 5:
                 LangSegment._parse_language(words,text)
             else:
                 language,score = LangSegment._lang_classify(cleans_text)
                 LangSegment._addwords(words,language,text,score)
         pass
     
+        
+    @staticmethod
+    def _process_pinyin(words,data):
+        tag , match = data
+        text = match
+        language = "zh"
+        score = 1.0
+        LangSegment._addwords(words,language,text,score)
+        pass
+    
     @staticmethod
     def _process_number(words,data): # "$0" process only
         """
         Numbers alone cannot accurately identify language.
         Because numbers are universal in all languages.
         So it won't be executed here, just for testing.
         """
@@ -463,15 +473,15 @@
                 LangSegment._parse_language(words , text)
             pass
         return words
     
     @staticmethod
     def _parse_symbols(text):
         TAG_NUM = "00" # "00" => default channels , "$0" => testing channel
-        TAG_S1,TAG_P1,TAG_P2,TAG_EN,TAG_KO,TAG_RU,TAG_TH = "$1" ,"$2" ,"$3" ,"$4" ,"$5" ,"$6" ,"$7"
+        TAG_S1,TAG_S2,TAG_P1,TAG_P2,TAG_EN,TAG_KO,TAG_RU,TAG_TH = "$1" ,"$2" ,"$3" ,"$4" ,"$5" ,"$6" ,"$7","$8"
         TAG_BASE = re.compile(fr'(([【《（(“‘"\']*[LANGUAGE]+[\W\s]*)+)')
         # Get custom language filter
         filters = LangSegment.Langfilters
         filters = filters if filters is not None else ""
         # =======================================================================================================
         # Experimental: Other language support.Thử nghiệm: Hỗ trợ ngôn ngữ khác.Expérimental : prise en charge d’autres langues.
         # 相关语言字符如有缺失，熟悉相关语言的朋友，可以提交把缺失的发音符号补全。
@@ -486,15 +496,16 @@
         LangSegment.EnablePreview = enablePreview
         # 实验性：法语字符支持。Prise en charge des caractères français
         RE_FR = "" if not enablePreview else "àáâãäåæçèéêëìíîïðñòóôõöùúûüýþÿ"
         # 实验性：越南语字符支持。Hỗ trợ ký tự tiếng Việt
         RE_VI = "" if not enablePreview else "đơưăáàảãạắằẳẵặấầẩẫậéèẻẽẹếềểễệíìỉĩịóòỏõọốồổỗộớờởỡợúùủũụứừửữựôâêơưỷỹ"
         # -------------------------------------------------------------------------------------------------------
         process_list = [
-            (  TAG_S1  , re.compile(LangSegment.SYMBOLS_PATTERN) , LangSegment._process_symbol  ),     # Symbol Tag
+            (  TAG_S1  , re.compile(LangSegment.SYMBOLS_PATTERN) , LangSegment._process_symbol  ),               # Symbol Tag
+            (  TAG_S2  , re.compile(r'([\(（](?:\s*\w*\d\w*\s*)+[）\)])') , LangSegment._process_pinyin  ),      # Pinyin Tag
             (  TAG_KO  , re.compile(re.sub(r'LANGUAGE',f'\uac00-\ud7a3',TAG_BASE.pattern))    , LangSegment._process_korean  ),              # Korean words
             (  TAG_TH  , re.compile(re.sub(r'LANGUAGE',f'\u0E00-\u0E7F',TAG_BASE.pattern))    , LangSegment._process_Thai ),                 # Thai words support.
             (  TAG_RU  , re.compile(re.sub(r'LANGUAGE',f'А-Яа-яЁё',TAG_BASE.pattern))         , LangSegment._process_Russian ),              # Russian words support.
             (  TAG_NUM , re.compile(r'(\W*\d+\W+\d*\W*\d*)')        , LangSegment._process_number  ),  # Number words, Universal in all languages, Ignore it.
             (  TAG_EN  , re.compile(re.sub(r'LANGUAGE',f'a-zA-Z{RE_FR}{RE_VI}',TAG_BASE.pattern))    , LangSegment._process_english ),       # English words + Other language support.
             (  TAG_P1  , re.compile(r'(["\'])(.*?)(\1)')         , LangSegment._process_quotes  ),     # Regular quotes
             (  TAG_P2  , re.compile(r'([\n]*[【《（(“‘])([^【《（(“‘’”)）》】]{3,})([’”)）》】][\W\s]*[\n]{,1})')   , LangSegment._process_quotes  ),  # Special quotes, There are left and right.
```

## LangSegment/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .LangSegment import LangSegment,getTexts,classify,getCounts,printList,setfilters,getfilters,setPriorityThreshold,getPriorityThreshold,setEnablePreview,getEnablePreview
 
 # release
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 
 # develop
 __develop__ = 'dev-0.0.1'
```

## Comparing `LangSegment-0.2.8.dist-info/METADATA` & `LangSegment-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangSegment
-Version: 0.2.8
+Version: 0.2.9
 Summary: This is a multilingual tokenization tool that currently supports for zh/ja/en/ko, and more languages.
 Home-page: https://github.com/juntaosun/LangSegment
 Author: sunnyboxs
 License: BSD
 Keywords: language detection,language identification,langid,langid.py,nlp,language
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -35,15 +35,15 @@
 https://github.com/adbar/py3langid  
 
 
 功能：将文章或句子里的例如（中/英/日/韩），按不同语言自动识别分词，使文本更适合AI处理。    
 本代码专为各种 TTS 项目的前端文本多语种混合标注区分，多语言混合训练和推理而编写。
 
 ## 最近更新：News   
-* 版本：v0.2.7     
+* 版本：v0.2.9     
 fix: Repeat short sentences   
 * 添加支持： "ru"俄语Russian / "th"泰语Thai。（更新帮助见下文）。
 * 添加支持： "fr"法语French  / "vi"越南语Vietnamese。
 * 语言优先级，置信度评分和阀值。
 * 优化字符处理。fix: LangSegment.setfilters    
 * 更细致的处理，中日英韩，分词更精准！  
 * 多语言过滤组功能（默认:中/英/日/韩）！帮您自动清理不需要的语言内容。
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LangSegment Version: 0.2.8 Summary: This is a
+Metadata-Version: 2.1 Name: LangSegment Version: 0.2.9 Summary: This is a
 multilingual tokenization tool that currently supports for zh/ja/en/ko, and
 more languages. Home-page: https://github.com/juntaosun/LangSegment Author:
 sunnyboxs License: BSD Keywords: language detection,language
 identification,langid,langid.py,nlp,language Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -22,15 +22,15 @@
 TTS (Text-to-Speech) synthesis projects, preprocessing of multilingual text
 mixing for both training and inference. >Implementation based on
 py3langidï¼See LICENSE file for more info. https://github.com/adbar/py3langid
 åè½ï¼å°æç« æå¥å­éçä¾å¦ï¼ä¸­/è±/æ¥/
 é©ï¼ï¼æä¸åè¯­è¨èªå¨è¯å«åè¯ï¼ä½¿ææ¬æ´éåAIå¤çã
 æ¬ä»£ç ä¸ä¸ºåç§ TTS
 é¡¹ç®çåç«¯ææ¬å¤è¯­ç§æ··åæ æ³¨åºåï¼å¤è¯­è¨æ··åè®­ç»åæ¨çèç¼åã
-## æè¿æ´æ°ï¼News * çæ¬ï¼v0.2.7 fix: Repeat short sentences *
+## æè¿æ´æ°ï¼News * çæ¬ï¼v0.2.9 fix: Repeat short sentences *
 æ·»å æ¯æï¼ "ru"ä¿è¯­Russian /
 "th"æ³°è¯­Thaiãï¼æ´æ°å¸®å©è§ä¸æï¼ã * æ·»å æ¯æï¼
 "fr"æ³è¯­French / "vi"è¶åè¯­Vietnameseã *
 è¯­è¨ä¼åçº§ï¼ç½®ä¿¡åº¦è¯ååéå¼ã * ä¼åå­ç¬¦å¤çãfix:
 LangSegment.setfilters * æ´ç»è´çå¤çï¼ä¸­æ¥è±é©ï¼åè¯æ´ç²¾åï¼
 * å¤è¯­è¨è¿æ»¤ç»åè½ï¼é»è®¤:ä¸­/è±/æ¥/
 é©ï¼ï¼å¸®æ¨èªå¨æ¸çä¸éè¦çè¯­è¨åå®¹ã * æ·»å  WebUI
```

