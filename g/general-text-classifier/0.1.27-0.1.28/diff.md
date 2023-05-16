# Comparing `tmp/general_text_classifier-0.1.27-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.28-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12846 bytes, number of entries: 6
--rw-r--r--  2.0 unx    56115 b- defN 23-May-12 20:24 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/RECORD
-6 files, 59049 bytes uncompressed, 11802 bytes compressed:  80.0%
+Zip file size: 12865 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    56186 b- defN 23-May-16 10:07 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-16 10:08 general_text_classifier-0.1.28.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-16 10:08 general_text_classifier-0.1.28.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 10:08 general_text_classifier-0.1.28.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-16 10:08 general_text_classifier-0.1.28.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-16 10:08 general_text_classifier-0.1.28.dist-info/RECORD
+6 files, 59120 bytes uncompressed, 11821 bytes compressed:  80.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.27.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.28.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.27.dist-info/METADATA
+Filename: general_text_classifier-0.1.28.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.27.dist-info/WHEEL
+Filename: general_text_classifier-0.1.28.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.27.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.28.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.27.dist-info/RECORD
+Filename: general_text_classifier-0.1.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -895,18 +895,18 @@
         Returns
         -------
         None
 
         """
 
         if self.do_train:
-            train_data["labels_original"] = train_data["labels"].tolist()
+            train_data["labels_original"] = copy.deepcopy(train_data["labels"].tolist())
 
             if val_data is not None:
-                val_data["labels_original"] = val_data["labels"].tolist()
+                val_data["labels_original"] = copy.deepcopy(val_data["labels"].tolist())
 
             if self.classification_type == "single":
                 label_encoder = LabelEncoder()
 
             else:
                 label_encoder = MultiLabelBinarizer()
                 train_data["labels"] = train_data["labels"].apply(
@@ -922,19 +922,19 @@
                 train_data["labels"].tolist()
             ).tolist()
 
             if val_data is not None:
                 val_data["labels"] = label_encoder.transform(
                     val_data["labels"].tolist()
                 ).tolist()
-
+            
             return [train_data, val_data, label_encoder]
 
         else:
-            val_data["labels_original"] = val_data["labels"].tolist()
+            val_data["labels_original"] = copy.deepcopy(val_data["labels"].tolist())
 
             if self.classification_type == "multi":
                 val_data["labels"] = val_data["labels"].apply(
                     lambda x: [elem.strip() for elem in x.split(";")]
                 )
 
             val_data["labels"] = self.label_encoder.transform(
@@ -950,15 +950,14 @@
         None
 
         Returns
         -------
         None
 
         """
-
         # training data is valid, moving to model fitting procedure...
         self.train_data["text"] = self.train_data["text"].astype(str)
 
         if self.do_lowercase and self.data_lang == "tr":
             self.train_data["text"] = self.train_data["text"].apply(
                 self.lowercase_turkish
             )
@@ -1057,15 +1056,15 @@
                     self.model_train_data = pd.DataFrame(
                         {"text": x_train.values, "labels": y_train.values}
                     )
 
                     self.model_val_data = pd.DataFrame(
                         {"text": x_val.values, "labels": y_val.values}
                     )
-
+        
         else:
             (
                 self.model_train_data,
                 self.model_val_data,
                 self.label_encoder,
             ) = self.encode_labels(self.train_data, self.val_data)
 
@@ -1177,14 +1176,15 @@
             assert "text" in val_data.columns.tolist(), self.print_error_messages(22)
             assert "labels" in val_data.columns.tolist(), self.print_error_messages(23)
             assert val_data["text"].isnull().sum() == 0, self.print_error_messages(24)
             assert val_data["labels"].isnull().sum() == 0, self.print_error_messages(25)
 
         self.train_data = train_data
         self.val_data = val_data
+        
         self.prepare_training_data()
         self.print_log_messages(6)
 
         # Following Andrew Ng's advice on selecting mini-batch size
         # https://cs230.stanford.edu/files/C2M2.pdf
         if len(self.model_train_data) <= 2000 and "train_batch_size" not in self.model_args:
             self.model_args["train_batch_size"] = 1
@@ -1495,10 +1495,8 @@
             ]
             self.test_data = self.test_data[reindex_cols]
 
         if result_save_path is not None:
             self.test_data.to_csv(result_save_path, index=False)
             self.print_log_messages(14)
 
-        self.print_log_messages(15)
-
-            
+        self.print_log_messages(15)
```

## Comparing `general_text_classifier-0.1.27.dist-info/LICENSE.txt` & `general_text_classifier-0.1.28.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.27.dist-info/METADATA` & `general_text_classifier-0.1.28.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.27
+Version: 0.1.28
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `general_text_classifier-0.1.27.dist-info/RECORD` & `general_text_classifier-0.1.28.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=rJ4veaBT44L1t5dhW7BhkkKyVcDeOp9Gg1AmWa1JdfM,56115
-general_text_classifier-0.1.27.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.27.dist-info/METADATA,sha256=hvvWvjQnoBS288AvKaBCB5JR323cSqVli16X7dGz3qQ,1188
-general_text_classifier-0.1.27.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.27.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.27.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=iOWi1P8MQXP1S9uvEXRtPeWQMIAWyxBLn4dd5iVuXNU,56186
+general_text_classifier-0.1.28.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.28.dist-info/METADATA,sha256=ngCiqTHt00YIWD0-aALW6L2PqDEhp2SN8kvXm1gtGbI,1188
+general_text_classifier-0.1.28.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.28.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.28.dist-info/RECORD,,
```

