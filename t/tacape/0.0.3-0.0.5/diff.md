# Comparing `tmp/tacape-0.0.3-py3-none-any.whl.zip` & `tmp/tacape-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11112 bytes, number of entries: 17
+Zip file size: 11493 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      232 b- defN 23-Apr-06 13:15 tacape/__init__.py
 -rw-rw-r--  2.0 unx      266 b- defN 23-Apr-06 13:15 tacape/logo.py
--rw-rw-r--  2.0 unx     1729 b- defN 23-Apr-06 15:28 tacape/run_classifier.py
--rw-rw-r--  2.0 unx     4485 b- defN 23-Apr-06 18:27 tacape/run_generator.py
--rw-rw-r--  2.0 unx     3324 b- defN 23-Apr-06 18:29 tacape/train_classifier.py
--rw-rw-r--  2.0 unx     3187 b- defN 23-Apr-06 15:44 tacape/train_generator.py
+-rw-rw-r--  2.0 unx     1872 b- defN 23-Jul-21 12:20 tacape/run_classifier.py
+-rw-rw-r--  2.0 unx     4736 b- defN 23-Jul-21 12:48 tacape/run_generator.py
+-rw-rw-r--  2.0 unx     3810 b- defN 23-Jul-21 12:37 tacape/train_classifier.py
+-rw-rw-r--  2.0 unx     3614 b- defN 23-Jul-21 12:38 tacape/train_generator.py
 -rw-rw-r--  2.0 unx       30 b- defN 23-Mar-30 15:33 tacape/models/__init__.py
 -rw-rw-r--  2.0 unx     1530 b- defN 23-Mar-30 15:24 tacape/models/layers.py
 -rw-rw-r--  2.0 unx     1167 b- defN 23-Apr-03 18:33 tacape/models/model.py
 -rw-rw-r--  2.0 unx       18 b- defN 23-Apr-03 17:27 tacape/utils/__init__.py
 -rw-rw-r--  2.0 unx      321 b- defN 23-Apr-03 17:27 tacape/utils/load.py
--rw-rw-r--  2.0 unx     1064 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7750 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx      215 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1339 b- defN 23-Apr-06 18:37 tacape-0.0.3.dist-info/RECORD
-17 files, 26756 bytes uncompressed, 8924 bytes compressed:  66.6%
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7907 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      215 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1339 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/RECORD
+17 files, 28220 bytes uncompressed, 9305 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: tacape/utils/__init__.py
 Comment: 
 
 Filename: tacape/utils/load.py
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/LICENSE
+Filename: tacape-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/METADATA
+Filename: tacape-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/WHEEL
+Filename: tacape-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/entry_points.txt
+Filename: tacape-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/top_level.txt
+Filename: tacape-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tacape-0.0.3.dist-info/RECORD
+Filename: tacape-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tacape/run_classifier.py

```diff
@@ -4,14 +4,15 @@
 from .models import build_model
 from sklearn.preprocessing import LabelEncoder
 from argparse import ArgumentParser
 import pandas as pd
 import numpy as np
 import tensorflow as tf
 import pickle
+import json
 
 def main():
 
     print(logo)
 
     argument_parser = ArgumentParser(prog='TACaPe: Predict')
     argument_parser.add_argument('--input', required=True, help='Input file')
@@ -21,21 +22,24 @@
 
     arguments = argument_parser.parse_args()
 
     run_model(arguments.input, arguments.format, arguments.classifier_prefix, arguments.output)
 
 def run_model(input, format, model_prefix, output):
 
+    with open(model_prefix + '_config.json', 'r') as reader:
+        config = json.loads(reader.read())
+
     with open(model_prefix + '.tokenizer', 'rb') as reader:
         tokenizer = pickle.loads(reader.read())
 
     with open(model_prefix + '.le', 'rb') as reader:
         le = pickle.loads(reader.read())
 
-    X = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(load_data(input, format)), maxlen = 60)
+    X = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(load_data(input, format)), maxlen = config['max_peptide_length'])
 
     model  = build_model(output_shape=(len(le.classes_)))
     model.load_weights(model_prefix + '.weights')
     y_pred = model.predict(X)[:,1]
 
     print(y_pred)
```

## tacape/run_generator.py

```diff
@@ -1,88 +1,91 @@
 from tacape.logo import logo
 from tacape.utils.load import load_data
 from tensorflow import keras
 from tacape.models import build_model
 from sklearn.preprocessing import LabelEncoder
 from argparse import ArgumentParser
 from tqdm import tqdm
-import pandas as pd
+import warnings
 import numpy as np
 import tensorflow as tf
 import pickle
+import json
+
+warnings.simplefilter('ignore')
 
 def main():
 
     print(logo)
 
     argument_parser = ArgumentParser(prog='TACaPe: Generate')
     argument_parser.add_argument('--generator-prefix', required=True, help='Path to the file prefix of the trained generative model')
     argument_parser.add_argument('--classifier-prefix', help='[optional] Path to the file prefix of the trained classification model')
     argument_parser.add_argument('--number-of-sequences', default=1000, type=int, help='[optional] Number of sequences to be generated (default: 1000)')
-    argument_parser.add_argument('--temperature', default=1.0, help='[optional] Temperature used for logit scaling when sampling aminoacids during auto-regressive generation (default: 1.0)')
-    argument_parser.add_argument('--threshold', default=0.5, help='[optional] Classification probability threshold (default: 0.5)')
-    argument_parser.add_argument('--output', required=True, help='Path to the output CSV file')
+    argument_parser.add_argument('--temperature', default=1.0, type=float, help='[optional] Temperature used for logit scaling when sampling aminoacids during auto-regressive generation (default: 1.0)')
+    argument_parser.add_argument('--threshold', default=0.5, type=float, help='[optional] Classification probability threshold (default: 0.5)')
+    argument_parser.add_argument('--output', required=True, help='Path to the output FASTA file')
 
     arguments = argument_parser.parse_args()
 
-    run_generator(arguments.generator_prefix, arguments.classifier_prefix, arguments.output, arguments.number_of_sequences, arguments.temperature)
+    run_generator(arguments.generator_prefix, arguments.classifier_prefix, arguments.output, arguments.number_of_sequences, arguments.temperature, arguments.threshold)
+
+def run_generator(generator_prefix, classifier_prefix, output, number_of_sequences, temperature, threshold):
 
-def run_generator(generator_prefix, classifier_prefix, output, number_of_sequences, temperature):
+    with open(generator_prefix + '_config.json', 'r') as reader:
+        config = json.loads(reader.read())
 
     with open(generator_prefix + '.tokenizer', 'rb') as reader:
         generator_tokenizer = pickle.loads(reader.read())
 
     with open(generator_prefix + '.le', 'rb') as reader:
         generator_le = pickle.loads(reader.read())    
 
     generator_model  = build_model(output_shape=(len(generator_le.classes_)))
-    generator_model.load_weights(generator_prefix + '.weights')
+    generator_model.load_weights(generator_prefix + '.weights').expect_partial()
 
     if classifier_prefix:
 
         with open(classifier_prefix + '.tokenizer', 'rb') as reader:
             classifier_tokenizer = pickle.loads(reader.read())
 
         with open(classifier_prefix + '.le', 'rb') as reader:
             classifier_le = pickle.loads(reader.read())
 
         classifier_model  = build_model(output_shape=(len(classifier_le.classes_)))
         classifier_model.load_weights(classifier_prefix + '.weights')
 
     number_of_generated_sequences = 0
 
-    generated_sequences = []
-
     progress_bar = tqdm(total=number_of_sequences)
 
-    while number_of_generated_sequences < number_of_sequences:
-        sequence = generate_sequence(generator_model, generator_tokenizer, generator_le, temperature=temperature)
-        if classifier_prefix:
-            score = classify_sequence(sequence, classifier_model, classifier_tokenizer)
-            if score > 0.5:
-                generated_sequences.append({'sequence': sequence, 'score': score})
+    with open(output, 'w') as writer:
+
+        while number_of_generated_sequences < number_of_sequences:
+            sequence = generate_sequence(generator_model, generator_tokenizer, generator_le, temperature=temperature, max_len=config['max_peptide_length'])
+            if classifier_prefix:
+                score = classify_sequence(sequence, classifier_model, classifier_tokenizer)
+                if score > threshold:
+                    writer.write(f'>{number_of_generated_sequences+1} {score}\n{sequence}\n')
+                    number_of_generated_sequences += 1
+                    progress_bar.update(1)
+            else:
+                writer.write(f'>{number_of_generated_sequences+1}\n{sequence}\n')
                 number_of_generated_sequences += 1
                 progress_bar.update(1)
-        else:
-            generated_sequences.append({'sequence': sequence})
-            number_of_generated_sequences += 1
-            progress_bar.update(1)
-    progress_bar.close()
-
-    df_output = pd.DataFrame(generated_sequences)
-    df_output.to_csv(output, index=False)
+        progress_bar.close()
 
 def sample(a, temperature=1.0):
     a = np.array(a).astype('float64')
     a = np.log(a) / temperature
     a = np.exp(a) / np.sum(np.exp(a))
     return np.argmax(np.random.multinomial(1, a, 1))
 
 def generate_sequence(generator_model, generator_tokenizer, generator_le, min_len=5, max_len=50, temperature=1.0):
-        
+
     while True:
         sequence = '$'
         next_token = None
         while True:
             tokenized  = keras.preprocessing.sequence.pad_sequences(generator_tokenizer.texts_to_sequences([sequence]), maxlen = 60)
             next_token = generator_le.inverse_transform([sample(generator_model.predict(tokenized, verbose=False)[0], temperature=temperature)])[0]
             sequence += next_token
```

## tacape/train_classifier.py

```diff
@@ -2,53 +2,65 @@
 from tacape.utils.load import load_data
 from tensorflow import keras
 from tacape.models import build_model
 from sklearn.preprocessing import LabelEncoder
 from argparse import ArgumentParser
 import tensorflow as tf
 import pickle
+import json
 
 def main():
 
     print(logo)
 
     argument_parser = ArgumentParser(prog='TACaPe: Model Training')
     argument_parser.add_argument('--positive-train', required=True, help='Input file containing positive peptides for training')
     argument_parser.add_argument('--negative-train', required=True, help='Input file containing negative peptides for training')
     argument_parser.add_argument('--positive-test', required=True, help='Input file containing positive peptides for testing')
     argument_parser.add_argument('--negative-test', required=True, help='Input file containing negative peptides for testing')
     argument_parser.add_argument('--format', choices=['text', 'fasta'], default='text', help='[optional] Input file format (default: text)')
     argument_parser.add_argument('--output', required=True, help='Path prefix of the output files containing the trained model')
     argument_parser.add_argument('--epochs', type=int, default=30, help="[optional] Number of epochs to be used during training (default: 30)")
+    argument_parser.add_argument('--max-peptide-length', type=int, default=60, help="[optional] Max length for peptides (for sequence padding / truncation) (default: 60)")
 
     arguments = argument_parser.parse_args()
 
     train_model(
         arguments.positive_train, 
         arguments.negative_train,
         arguments.positive_test, 
         arguments.negative_test, 
         format=arguments.format, 
         output=arguments.output,
-        epochs=arguments.epochs
+        epochs=arguments.epochs,
+        max_peptide_length=arguments.max_peptide_length
     )
 
-def train_model(positive_train, negative_train, positive_test, negative_test, output, format='text', epochs=30):
+def train_model(positive_train, negative_train, positive_test, negative_test, output, format='text', epochs=30, max_peptide_length=60):
+
+    config = {
+        'max_peptide_length': max_peptide_length
+    }
+
+    with open(output + '_config.json', 'w') as writer:
+        writer.write(
+            json.dumps(config)
+        )
 
     raw_X_train = [*load_data(positive_train, format), *load_data(negative_train, format)]
     raw_X_test  = [*load_data(positive_test, format), *load_data(negative_test, format)]
 
     y_train = [1 for _ in load_data(positive_train, format)] + [0 for _ in load_data(negative_train, format)]
     y_test  = [1 for _ in load_data(positive_test, format)] + [0 for _ in load_data(negative_test, format)]
 
     tokenizer = keras.preprocessing.text.Tokenizer(char_level = True)
     tokenizer.fit_on_texts(raw_X_train)
 
-    X_train = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(raw_X_train), maxlen = 60)
-    X_test  = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(raw_X_test), maxlen = 60)
+    X_train = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(raw_X_train), maxlen = max_peptide_length)
+    X_test  = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(raw_X_test), maxlen = max_peptide_length)
 
     with open(output + '.tokenizer', 'wb') as writer:
         writer.write(pickle.dumps(tokenizer))
 
     le = LabelEncoder()
     le.fit(y_train)
```

## tacape/train_generator.py

```diff
@@ -2,50 +2,61 @@
 from tacape.utils.load import load_data
 from tensorflow import keras
 from tacape.models import build_model
 from sklearn.preprocessing import LabelEncoder
 from argparse import ArgumentParser
 import tensorflow as tf
 import pickle
+import json
 
 def main():
 
     print(logo)
 
     argument_parser = ArgumentParser(prog='TACaPe: Model Training')
     argument_parser.add_argument('--positive-train', required=True, help='Input file containing positive peptides for training')
     argument_parser.add_argument('--positive-test', required=True, help='Input file containing positive peptides for testing')
     argument_parser.add_argument('--format', choices=['text', 'fasta'], default='text', help='[optional] Input file format (default: text)')
     argument_parser.add_argument('--output', required=True, help='Path prefix of the output files containing the trained model')
     argument_parser.add_argument('--epochs', type=int, default=30, help="[optional] Number of epochs to be used during training (default: 30)")
+    argument_parser.add_argument('--max-peptide-length', type=int, default=60, help="[optional] Max length for peptides (for sequence padding / truncation) (default: 60)")
 
     arguments = argument_parser.parse_args()
 
     train_model(
         arguments.positive_train, 
         arguments.positive_test, 
         format=arguments.format, 
         output=arguments.output,
-        epochs=arguments.epochs
+        epochs=arguments.epochs,
+        max_peptide_length=arguments.max_peptide_length
     )
 
-def train_model(positive_train, positive_test, output, format='text', epochs=30):
+def train_model(positive_train, positive_test, output, format='text', epochs=30, max_peptide_length=60):
 
+    config = {
+        'max_peptide_length': max_peptide_length
+    }
+
+    with open(output + '_config.json', 'w') as writer:
+        writer.write(
+            json.dumps(config)
+        )
+    
     raw_X_train = [*load_data(positive_train, format)]
     raw_X_test  = [*load_data(positive_test, format)]
 
     X_train = []
     y_train = []
 
     for sequence in raw_X_train:
         sequence = '$' + sequence + '.'
         for i in range(1, len(sequence)):
             X_train.append(sequence[0:i])
             y_train.append(sequence[i])
-            print(y_train[-1])
 
     X_test = []
     y_test = []
 
     for sequence in raw_X_test:
         sequence = '$' + sequence + '.'
         for i in range(1, len(sequence)):
```

## Comparing `tacape-0.0.3.dist-info/LICENSE` & `tacape-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tacape-0.0.3.dist-info/METADATA` & `tacape-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacape
-Version: 0.0.3
+Version: 0.0.5
 Summary: TACaPe: Transformed-based Anti-Cancer Peptide Classification and Generation
 Home-page: https://github.com/omixlab/anticancer-peptide
 Author: Isadora Leitzke Guidotti, Frederico Schmitt Kremer
 Author-email: fred.s.kremer@gmail.com
 License: UNKNOWN
 Keywords: bioinformatics machine-learning data science drug discovery QSAR
 Platform: UNKNOWN
@@ -210,7 +210,16 @@
 $ tacape-generate \
     --generator-prefix data/models/generator \
     --classifier-prefix data/models/classifier \
     --number-of-sequence 100 \
     --output data/models/generated.csv
 ```
 
+### Convert generated peptides to FASTA
+
+```
+$ tacape-csv-to-fasta \
+    --input data/models/generated.csv \
+    --output data/models/generated.fasta
+```
+ 
+
```

## Comparing `tacape-0.0.3.dist-info/RECORD` & `tacape-0.0.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 tacape/__init__.py,sha256=djG1eYXbcqwm5Gr_K3wQSs9MlzmDkePC1hp4OP0HGKA,232
 tacape/logo.py,sha256=tdtlyP3-qkmrWodSjxazRQRw101ok6sRV9lMYkDTgS4,266
-tacape/run_classifier.py,sha256=l7GqwRXNR9Ls2BCIRvcIx4eNAQc_YLGBmCsMBPQ6Q_s,1729
-tacape/run_generator.py,sha256=Lzuo4WdGvNN-w83-JPsOGvCLlOhee8fiBC9Eyh1Dkuc,4485
-tacape/train_classifier.py,sha256=b10JcdBSpIS_1Iy750h0q6swwi96gWQTkmbA34eHh3A,3324
-tacape/train_generator.py,sha256=q5ACcATxD7ECfGQh1J4WXXrIAy4IzFHb1NYGdLBvf6U,3187
+tacape/run_classifier.py,sha256=Vgb0vZaD7WmpdfNBR4JmMx8gWdYOUKaTzobus7zJcbo,1872
+tacape/run_generator.py,sha256=-MiEYFb5DED3vXEpS5v6_8ZetMzw_ie0LyayoOBQ8T4,4736
+tacape/train_classifier.py,sha256=U0-nT0LYroMjj4kt2MjNOnAIweezttyqWKrxJIQhv5Y,3810
+tacape/train_generator.py,sha256=hB20eOpK0a7Pedh1vnWTJmhQotJNke2_Qwr_f5sKAso,3614
 tacape/models/__init__.py,sha256=B_zIwHcareHucr4JqgdnFAVvDfFijR__w-SsyunG2xw,30
 tacape/models/layers.py,sha256=xgp0RICRpUgrbn_18tsvaWkA_D_dZ8CLz43xRDggNCo,1530
 tacape/models/model.py,sha256=e8boh62n5oNWCIe2pawyiC5wYPqj7eWnaITujOwVZdY,1167
 tacape/utils/__init__.py,sha256=AQT2L8X2AdWB_Wk__JStBuwtUvfTGz8wTFcR94_81Zo,18
 tacape/utils/load.py,sha256=XknlskZOrjcd5Z5M9ER5yxzDLqhxiU5YAPp9s388JDg,321
-tacape-0.0.3.dist-info/LICENSE,sha256=lL6wJjUrwH3bCmb2msANo8SHV4OUCyoWfR9FeG-T4XU,1064
-tacape-0.0.3.dist-info/METADATA,sha256=_gOmXLu-Rfepz_DEpFqi9dXHjkJl95DZj3xSvld0Pq4,7750
-tacape-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tacape-0.0.3.dist-info/entry_points.txt,sha256=TfKUjYa52O20d8pXWYEm76xX5T7w0xm-V4d4pkUcSCc,215
-tacape-0.0.3.dist-info/top_level.txt,sha256=2LcJzKwy0vqun3FbnQSXQGlBqZdxGMypEu26pZtvWQ0,7
-tacape-0.0.3.dist-info/RECORD,,
+tacape-0.0.5.dist-info/LICENSE,sha256=lL6wJjUrwH3bCmb2msANo8SHV4OUCyoWfR9FeG-T4XU,1064
+tacape-0.0.5.dist-info/METADATA,sha256=leKJ0FVUhphIdRuJprBKkSTHGSZHGh7KBkhtQSl54d4,7907
+tacape-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tacape-0.0.5.dist-info/entry_points.txt,sha256=TfKUjYa52O20d8pXWYEm76xX5T7w0xm-V4d4pkUcSCc,215
+tacape-0.0.5.dist-info/top_level.txt,sha256=2LcJzKwy0vqun3FbnQSXQGlBqZdxGMypEu26pZtvWQ0,7
+tacape-0.0.5.dist-info/RECORD,,
```

