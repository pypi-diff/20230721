# Comparing `tmp/bio-corgi-0.2.2.tar.gz` & `tmp/bio_corgi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-corgi-0.2.2.tar", max compression
+gzip compressed data, was "bio_corgi-0.4.0.tar", max compression
```

## Comparing `bio-corgi-0.2.2.tar` & `bio_corgi-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11334 2021-07-29 03:38:45.000000 bio-corgi-0.2.2/LICENSE
--rw-r--r--   0        0        0     2247 2022-09-12 14:56:09.970728 bio-corgi-0.2.2/README.rst
--rw-r--r--   0        0        0       24 2022-09-05 00:17:00.884664 bio-corgi-0.2.2/corgi/__init__.py
--rw-r--r--   0        0        0     9236 2022-09-12 12:27:26.048758 bio-corgi-0.2.2/corgi/apps.py
--rw-r--r--   0        0        0    10179 2022-09-05 00:17:00.885878 bio-corgi-0.2.2/corgi/dataloaders.py
--rw-r--r--   0        0        0    11354 2022-09-12 14:18:31.127336 bio-corgi-0.2.2/corgi/models.py
--rw-r--r--   0        0        0     1083 2022-09-05 00:17:00.887166 bio-corgi-0.2.2/corgi/preprocessing.py
--rw-r--r--   0        0        0      421 2022-09-05 00:17:00.887687 bio-corgi-0.2.2/corgi/profiling.py
--rw-r--r--   0        0        0    13540 2022-09-05 00:17:00.888624 bio-corgi-0.2.2/corgi/refseq.py
--rw-r--r--   0        0        0     1698 2022-09-05 00:13:39.443441 bio-corgi-0.2.2/corgi/tensor.py
--rw-r--r--   0        0        0     4002 2022-09-05 00:17:00.889254 bio-corgi-0.2.2/corgi/transforms.py
--rw-r--r--   0        0        0     1985 2022-09-12 15:07:27.371818 bio-corgi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 bio-corgi-0.2.2/setup.py
--rw-r--r--   0        0        0     4080 1970-01-01 00:00:00.000000 bio-corgi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2021-07-29 03:38:45.000000 bio_corgi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2307 2023-07-14 05:27:52.869364 bio_corgi-0.4.0/README.rst
+-rw-r--r--   0        0        0       24 2022-09-05 00:17:00.884664 bio_corgi-0.4.0/corgi/__init__.py
+-rw-r--r--   0        0        0    13307 2023-07-14 05:20:22.610751 bio_corgi-0.4.0/corgi/apps.py
+-rw-r--r--   0        0        0    13392 2023-07-14 05:20:22.612332 bio_corgi-0.4.0/corgi/dataloaders.py
+-rw-r--r--   0        0        0    16923 2023-07-14 03:32:16.543081 bio_corgi-0.4.0/corgi/models.py
+-rw-r--r--   0        0        0     1083 2022-09-05 00:17:00.887166 bio_corgi-0.4.0/corgi/preprocessing.py
+-rw-r--r--   0        0        0      421 2022-09-05 00:17:00.887687 bio_corgi-0.4.0/corgi/profiling.py
+-rw-r--r--   0        0        0    13540 2022-09-05 00:17:00.888624 bio_corgi-0.4.0/corgi/refseq.py
+-rw-r--r--   0        0        0     1850 2023-07-14 03:32:16.545007 bio_corgi-0.4.0/corgi/tensor.py
+-rw-r--r--   0        0        0     6928 2023-07-14 03:32:16.546512 bio_corgi-0.4.0/corgi/transforms.py
+-rw-r--r--   0        0        0     1987 2023-07-21 01:21:06.192631 bio_corgi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 bio_corgi-0.4.0/PKG-INFO
```

### Comparing `bio-corgi-0.2.2/LICENSE` & `bio_corgi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-corgi-0.2.2/README.rst` & `bio_corgi-0.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 Usage
 ============
 
 To make predictions, run the ``corgi`` command line tool:
 
 .. code-block:: bash
 
-    corgi --fasta <input fasta file> --output-csv <results>
+    corgi --file <input seq file>
+
+This will create a directory with the predictions in a CSV file and in fasta format.
 
 For more information about the other options, see the help with:
 
 .. code-block:: bash
 
     corgi --help
```

### Comparing `bio-corgi-0.2.2/corgi/apps.py` & `bio_corgi-0.4.0/corgi/apps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
 from typing import List
 from torch import nn
-import torch
 import pandas as pd
 from fastai.data.core import DataLoaders
 from torchapp.util import copy_func, call_func, change_typer_to_defaults, add_kwargs
 from fastai.learner import Learner, load_learner
 from fastai.metrics import accuracy, Precision, Recall, RocAuc, F1Score
 import torchapp as ta
 from rich.console import Console
 from rich.table import Table
 from rich.box import SIMPLE
+from Bio import SeqIO
+import time
 
 from fastai.losses import CrossEntropyLossFlat
 
 console = Console()
 
 from . import dataloaders, models, refseq, transforms
 
@@ -36,28 +37,35 @@
         self,
         csv: Path = ta.Param(help="The CSV which has the sequences to use."),
         base_dir: Path = ta.Param(help="The base directory with the RefSeq HDF5 files."),
         batch_size: int = ta.Param(default=32, help="The batch size."),
         dataloader_type: dataloaders.DataloaderType = ta.Param(
             default=dataloaders.DataloaderType.PLAIN, case_sensitive=False
         ),
+        validation_seq_length:int = 1_000,
+        deform_lambda:float = ta.Param(default=None, help="The lambda for the deform transform."),
     ) -> DataLoaders:
         """
         Creates a FastAI DataLoaders object which Corgi uses in training and prediction.
 
         Args:
             inputs (Path): The input file.
             batch_size (int): The number of elements to use in a batch for training and prediction. Defaults to 32.
         """
         if csv is None:
             raise Exception("No CSV given")
         if base_dir is None:
             raise Exception("No base_dir given")
         dls = dataloaders.create_dataloaders_refseq_path(
-            csv, base_dir=base_dir, batch_size=batch_size, dataloader_type=dataloader_type
+            csv, 
+            base_dir=base_dir, 
+            batch_size=batch_size, 
+            dataloader_type=dataloader_type, 
+            deform_lambda=deform_lambda, 
+            validation_seq_length=validation_seq_length,
         )
         self.categories = dls.vocab
         return dls
 
     def model(
         self,
         embedding_dim: int = ta.Param(
@@ -84,65 +92,95 @@
             help="The size of the pooling before going to the LSTM.",
         ),
         lstm_dims: int = ta.Param(default=256, help="The size of the hidden layers in the LSTM in both directions."),
         final_layer_dims: int = ta.Param(
             default=0, help="The size of a dense layer after the LSTM. If this is zero then this layer isn't used."
         ),
         dropout: float = ta.Param(
-            default=0.5,
+            default=0.2,
             help="The amount of dropout to use. (not currently enabled)",
             tune=True,
             tune_min=0.0,
-            tune_max=1.0,
+            tune_max=0.3,
         ),
         final_bias: bool = ta.Param(
             default=True,
             help="Whether or not to use bias in the final layer.",
             tune=True,
         ),
         cnn_only: bool = True,
         kernel_size: int = ta.Param(
             default=3, help="The size of the kernels for CNN only classifier.", tune=True, tune_choices=[3, 5, 7, 9]
         ),
         cnn_dims_start: int = ta.Param(
-            default=64,
-            help="The size of the number of filters in the first CNN layer.",
-            tune=True,
-            log=True,
-            tune_min=32,
-            tune_max=1024,
+            default=None,
+            help="The size of the number of filters in the first CNN layer. If not set then it is derived from the MACC",
         ),
         factor: float = ta.Param(
             default=2.0,
             help="The factor to multiply the number of filters in the CNN layers each time it is downscaled.",
             tune=True,
             log=True,
             tune_min=0.5,
-            tune_max=4.0,
+            tune_max=2.5,
+        ),
+        penultimate_dims: int = ta.Param(
+            default=1024,
+            help="The factor to multiply the number of filters in the CNN layers each time it is downscaled.",
+            tune=True,
+            log=True,
+            tune_min=512,
+            tune_max=2048,
+        ),
+        include_length: bool = False,
+        transformer_heads: int = ta.Param(8, help="The number of heads in the transformer."),
+        transformer_layers: int = ta.Param(0, help="The number of layers in the transformer. If zero then no transformer is used."),
+        macc:int = ta.Param(
+            default=10_000_000,
+            help="The approximate number of multiply or accumulate operations in the model. Used to set cnn_dims_start if not provided explicitly.",
         ),
     ) -> nn.Module:
         """
         Creates a deep learning model for the Corgi to use.
 
         Returns:
             nn.Module: The created model.
         """
         num_classes = len(self.categories)
 
+        # if cnn_dims_start not given then calculate it from the MACC
+        if not cnn_dims_start:
+            assert macc
+
+            cnn_dims_start = models.calc_cnn_dims_start(
+                macc=macc,
+                seq_len=1024, # arbitary number
+                embedding_dim=embedding_dim,
+                cnn_layers=cnn_layers,
+                kernel_size=kernel_size,
+                factor=factor,
+                penultimate_dims=penultimate_dims,
+                num_classes=num_classes,
+            )
+
         if cnn_only:
             return models.ConvClassifier(
                 num_embeddings=5,  # i.e. the size of the vocab which is N, A, C, G, T
                 kernel_size=kernel_size,
                 factor=factor,
                 cnn_layers=cnn_layers,
                 num_classes=num_classes,
                 kernel_size_maxpool=kernel_size_maxpool,
                 final_bias=final_bias,
                 dropout=dropout,
                 cnn_dims_start=cnn_dims_start,
+                penultimate_dims=penultimate_dims,
+                include_length=include_length,
+                transformer_layers=transformer_layers,
+                transformer_heads=transformer_heads,
             )
 
         return models.ConvRecurrantClassifier(
             num_classes=num_classes,
             embedding_dim=embedding_dim,
             filters=filters,
             cnn_layers=cnn_layers,
@@ -168,51 +206,98 @@
 
     # def loss_func(self, label_smoothing:float=ta.Param(0.1, help="The amount of label smoothing.")):
     #     return CrossEntropyLossFlat(label_smoothing=label_smoothing)
 
     def inference_dataloader(
         self,
         learner,
-        fasta: List[Path] = ta.Param(None, help="A fasta file with sequences to be classified."),
+        file: List[Path] = ta.Param(None, help="A fasta file with sequences to be classified."),
         max_seqs: int = None,
+        batch_size:int = 1,
+        max_length:int = 5_000,
+        min_length:int = 128,
         **kwargs,
     ):
-        df = dataloaders.fastas_to_dataframe(fasta_paths=fasta, max_seqs=max_seqs)  # hack. should be generator
-        dataloader = learner.dls.test_dl(df)
-        dataloader.before_batch.fs = [transforms.PadBatch()]
+        self.seqio_dataloader = dataloaders.SeqIODataloader(files=file, device=learner.dls.device, batch_size=batch_size, max_length=max_length, max_seqs=max_seqs, min_length=min_length)
         self.categories = learner.dls.vocab
-        self.inference_df = df
-        return dataloader
+        return self.seqio_dataloader
 
     def output_results(
         self,
         results,
-        output_csv: Path = ta.Param(default=None, help="A path to output the results as a CSV."),
+        output_dir:Path = ta.Param(default=None, help="A path to output the results as a CSV."),
+        csv: Path = ta.Param(default=None, help="A path to output the results as a CSV. If not given then a default name is chosen inside the output directory."),
+        save_filtered:bool = ta.Param(default=True, help="Whether or not to save the filtered sequences."),
+        threshold: float = ta.Param(
+            default=None, 
+            help="The threshold to use for filtering. "
+                "If not given, then only the most likely category used for filtering.",
+        ),
         **kwargs,
     ):
+        if not output_dir:
+            time_string = time.strftime("%Y_%m_%d-%I_%M_%S_%p")
+            output_dir = f"corgi-output-{time_string}"
+
+        output_dir = Path(output_dir)
+
+        chunk_details = pd.DataFrame(self.seqio_dataloader.chunk_details, columns=["file", "accession", "chunk"])
         predictions_df = pd.DataFrame(results[0].numpy(), columns=self.categories)
         results_df = pd.concat(
-            [self.inference_df, predictions_df],
+            [chunk_details.drop(columns=['chunk']), predictions_df],
             axis=1,
         )
 
-        predictions = torch.argmax(results[0], dim=1)
+        # Average over chunks
+        results_df = results_df.groupby(["file", "accession"]).mean().reset_index()
+
         columns = set(predictions_df.columns)
 
-        results_df['prediction'] = [self.categories[p] for p in predictions]
+        results_df['prediction'] = results_df[self.categories].idxmax(axis=1)
         results_df['eukaryotic'] = predictions_df[list(columns & set(refseq.EUKARYOTIC))].sum(axis=1)
         results_df['prokaryotic'] = predictions_df[list(columns & set(refseq.PROKARYOTIC))].sum(axis=1)
         results_df['organellar'] = predictions_df[list(columns & set(refseq.ORGANELLAR))].sum(axis=1)
 
-        results_df = results_df.drop(['sequence', 'validation', 'category'], axis=1)
-        if output_csv:
-            console.print(f"Writing results for {len(results_df)} sequences to: {output_csv}")
-            results_df.to_csv(output_csv, index=False)
-        else:
-            print("No output file given.")
+        if not csv:
+            output_dir.mkdir(parents=True, exist_ok=True)
+            csv = output_dir / f"corgi-output.csv"
+
+        console.print(f"Writing results for {len(results_df)} sequences to: {csv}")
+        results_df.to_csv(csv, index=False)
+
+        # Write all the sequences to fasta files
+        if save_filtered:
+            output_dir.mkdir(parents=True, exist_ok=True)
+            
+            file_handles = {}
+
+            for file, record in self.seqio_dataloader.iter_records():
+                row = results_df[ (results_df.accession == record.id) & (results_df.file == file) ]
+                if len(row) == 0:
+                    categories = ["unclassified"]
+                else:
+                    # Get the categories to write to
+                    if not threshold:
+                        # if no threshold then just use the most likely category
+                        categories = [row['prediction'].item()]
+                    else:
+                        # otherwise use all categories above or equal to the threshold
+                        category_predictions = row.iloc[0][self.categories]
+                        categories = [category_predictions[category_predictions >= threshold].index.item()]
+
+                for category in categories:
+                    if category not in file_handles:
+                        file_path = output_dir / f"{category}.fasta"
+                        file_handles[category] = open(file_path, "w")
+                        console.print(f"Writing {category} sequences to: {file_path}")
+
+                    SeqIO.write(record, file_handles[category], "fasta")
+
+            for file_handle in file_handles.values():
+                file_handle.close()
 
         # Output bar chart
         from termgraph.module import Data, BarChart, Args
 
         value_counts = results_df['prediction'].value_counts()
         data = Data([[count] for count in value_counts], value_counts.index)
         chart = BarChart(
@@ -248,8 +333,8 @@
 
     def category_counts(self, **kwargs):
         dataloaders = call_func(self.dataloaders, **kwargs)
         self.category_counts_dataloader(dataloaders.train, "Training")
         self.category_counts_dataloader(dataloaders.valid, "Validation")
 
     def pretrained_location(self) -> str:
-        return "https://github.com/rbturnbull/corgi/releases/download/v0.2.2-alpha/corgi-learner-0.2.2.pkl"
+        return "https://github.com/rbturnbull/corgi/releases/download/v0.3.1-alpha/corgi-0.3.pkl"
```

### Comparing `bio-corgi-0.2.2/corgi/dataloaders.py` & `bio_corgi-0.4.0/corgi/dataloaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import torch
 from enum import Enum
 import random
 from itertools import chain
 
 import gzip
 import pandas as pd
 from pathlib import Path
@@ -17,15 +18,15 @@
 from fastai.data.core import TfmdDL, DataLoaders, get_empty_df
 from fastai.callback.data import WeightedDL
 from fastai.data.block import DataBlock, TransformBlock, CategoryBlock
 from fastai.torch_core import display_df
 from fastai.data.transforms import ColSplitter, ColReader, RandomSplitter
 
 from .tensor import TensorDNA, dna_seq_to_numpy, dna_seq_to_tensor
-from .transforms import RandomSliceBatch, SliceTransform, RowToTensorDNA
+from .transforms import RandomSliceBatch, SliceTransform, RowToTensorDNA, PadBatchX, DeterministicSliceBatch, DeformBatch
 from .refseq import RefSeqCategory
 
 
 def fasta_open(fasta_path):
     if fasta_path.suffix == ".gz":
         return gzip.open(fasta_path, "rt")
     return open(fasta_path, "rt")
@@ -129,39 +130,63 @@
 
 class DataloaderType(str, Enum):
     PLAIN = "PLAIN"
     WEIGHTED = "WEIGHTED"
     STRATIFIED = "STRATIFIED"
 
 
-def create_dataloaders_refseq_path(dataframe_path: Path, base_dir: Path, batch_size=64, **kwargs):
+def create_dataloaders_refseq_path(
+    dataframe_path: Path, 
+    base_dir: Path, 
+    batch_size:int=64, 
+    deform_lambda: float = None,
+    validation_seq_length:int=1_000, 
+    **kwargs
+):
     dataframe_path = Path(dataframe_path)
 
     print('Training using:\t', dataframe_path)
     if dataframe_path.suffix == ".parquet":
         df = pd.read_parquet(str(dataframe_path), engine="pyarrow")
     else:
         df = pd.read_csv(str(dataframe_path))
 
     print(f'Dataframe has {len(df)} sequences.')
-    dls = create_dataloaders_refseq(df, batch_size=batch_size, base_dir=base_dir, **kwargs)
+    dls = create_dataloaders_refseq(
+        df, 
+        batch_size=batch_size, 
+        base_dir=base_dir, 
+        deform_lambda=deform_lambda, 
+        validation_seq_length=validation_seq_length, 
+        **kwargs
+    )
     return dls
 
 
 def create_dataloaders_refseq(
     df: pd.DataFrame,
     base_dir: Path,
     batch_size=64,
     dataloader_type: DataloaderType = DataloaderType.PLAIN,
     verbose: bool = True,
+    validation_seq_length:int = 1_000,
+    deform_lambda: float = None,
     **kwargs,
 ) -> DataLoaders:
     categories = [RefSeqCategory(name, base_dir=base_dir) for name in df.category.unique()]
 
-    dataloaders_kwargs = dict(bs=batch_size, drop_last=False, before_batch=RandomSliceBatch)
+    # Set up batch transforms
+    before_batch = [
+        RandomSliceBatch(only_split_index=0), 
+        DeterministicSliceBatch(seq_length=validation_seq_length, only_split_index=1),
+    ]
+    if deform_lambda is not None:
+        before_batch.append(DeformBatch(deform_lambda=deform_lambda))
+
+    dataloaders_kwargs = dict(bs=batch_size, drop_last=False, before_batch=before_batch)
 
     validation_column = "validation"
     random.seed(42)
     if validation_column not in df:
         df[validation_column] = 0
         value_counts = df.category.value_counts()
         validation_per_category = int(0.2 * value_counts.min())
@@ -228,15 +253,15 @@
 
     if not fasta_path.exists():
         raise FileNotFoundError(f"Cannot find fasta file {fasta_path}.")
 
     seq_count = fasta_seq_count(fasta_path)
     print(f"{seq_count} sequences")
     if max_seqs and seq_count >= max_seqs:
-        print("Limiting to maximum number of sequences: {max_seqs}")
+        print(f"Limiting to maximum number of sequences: {max_seqs}")
         seq_count = max_seqs
 
     data = []
     fasta = fasta_open(fasta_path)
 
     if validation_from_filename:
         if "valid" in str(fasta_path):
@@ -290,7 +315,94 @@
         for b in _loaders[self.fake_l.num_workers == 0](self.fake_l):
             if self.device is not None:
                 b = to_device(b, self.device)
             yield self.after_batch(b)
         self.after_iter()
         if hasattr(self, 'it'):
             del self.it
+
+
+class SeqIODataloader:
+    def __init__(self, files, device, batch_size:int=1, min_length:int=128, max_length:int=5_000, max_seqs:int=None, format:str=""):
+        self.files = list(files)
+        self.device = device
+        self.format = format
+        self.chunk_details = []
+        self.max_length = max_length
+        self.batch_size = batch_size
+        self.min_length = min_length
+        self.pad = PadBatchX()
+        self.count = 0
+        self.max_seqs = max_seqs
+        seqs = 0
+        for file in self.files:
+            for record in self.parse(file):
+                if len(record.seq) < self.min_length:
+                    continue
+
+                if self.max_seqs and seqs >= self.max_seqs:
+                    break
+
+                chunks = len(record.seq)//self.max_length + 1
+                self.count += chunks
+                seqs += 1
+
+
+    def get_file_format(self, file):
+        if self.format:
+            return self.format
+        
+        file = Path(file)
+        suffix = file.suffix.lower()
+
+        if suffix in [".fa", ".fna", ".fasta"]:
+            return "fasta"
+
+        if suffix in [".genbank", ".gb", ".gbk"]:
+            return "genbank"
+
+        if suffix in [".tab", ".tsv"]:
+            return "tsv"
+
+        if suffix in [".fastq", ".fq"]:
+            return "fastq"
+
+        raise ValueError(f"Cannot determine file format of {file}.")
+    
+    def __len__(self):
+        return self.count
+
+    def parse(self, file):
+        return SeqIO.parse(file, self.get_file_format(file))
+
+    def iter_records(self):
+        for file in self.files:
+            for record in self.parse(file):
+                yield file, record
+
+    def __iter__(self):
+        batch = []
+        seqs = 0
+
+        for file in self.files:
+            for record in self.parse(file):
+                if len(record.seq) < self.min_length:
+                    continue
+
+                if self.max_seqs and seqs >= self.max_seqs:
+                    break
+
+                seqs += 1
+                t = dna_seq_to_tensor(record.seq)
+                chunks = len(t)//self.max_length + 1
+
+                for chunk_index, chunk in enumerate(t.chunk(chunks)):
+                    self.chunk_details.append( (file, record.id, chunk_index) )
+                    batch.append(chunk)
+                    if len(batch) >= self.batch_size:
+                        batch = self.pad(batch)
+                        yield batch
+                        batch = []
+
+        if batch:
+            batch = self.pad(batch)
+            yield batch
```

### Comparing `bio-corgi-0.2.2/corgi/models.py` & `bio_corgi-0.4.0/corgi/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,44 @@
 from typing import Callable, Optional
-
+import math
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
+from rich.console import Console
+console = Console()
+
+
+class PositionalEncoding(nn.Module):
+    """
+    Adapted from https://pytorch.org/tutorials/beginner/transformer_tutorial.html
+    """
+
+    def __init__(self, d_model: int, dropout: float = 0.1, max_len: int = 5000):
+        super().__init__()
+        self.dropout = nn.Dropout(p=dropout)
+
+        position = torch.arange(max_len).unsqueeze(1)
+        div_term = torch.exp(torch.arange(0, d_model, 2) * (-math.log(10000.0) / d_model))
+        pe = torch.zeros(max_len, 1, d_model)
+        pe[:, 0, 0::2] = torch.sin(position * div_term)
+        pe[:, 0, 1::2] = torch.cos(position * div_term)
+        self.register_buffer('pe', pe)
+
+    def forward(self, x: Tensor) -> Tensor:
+        """
+        Arguments:
+            x: Tensor, shape ``[seq_len, batch_size, embedding_dim]``
+        """
+        x = x + self.pe[:x.size(0)]
+        return self.dropout(x)
+
+
 
 def conv3(in_planes: int, out_planes: int, stride: int = 1, groups: int = 1, dilation: int = 1) -> nn.Conv1d:
     """convolution of width 3 with padding"""
     return nn.Conv1d(
         in_planes,
         out_planes,
         kernel_size=3,
@@ -240,26 +270,35 @@
         kernel_size=3,
         factor=2,
         padding="same",
         padding_mode="zeros",
         dropout=0.5,
         final_bias=True,
         lstm_dims: int = 0,
+        penultimate_dims: int = 1028,
+        include_length: bool = False,
+        length_scaling:float = 3_000.0,
+        transformer_heads: int = 8,
+        transformer_layers: int = 6,
     ):
         super().__init__()
 
         self.embedding_dim = embedding_dim
         self.cnn_layers = cnn_layers
         self.num_classes = num_classes
         self.kernel_size_maxpool = kernel_size_maxpool
 
         self.num_embeddings = num_embeddings
         self.kernel_size = kernel_size
         self.factor = factor
         self.dropout = dropout
+        self.include_length = include_length
+        self.length_scaling = length_scaling
+        self.transformer_layers = transformer_layers
+        self.transformer_heads = transformer_heads
 
         self.embedding = nn.Embedding(
             num_embeddings=num_embeddings,
             embedding_dim=embedding_dim,
         )
 
         in_channels = embedding_dim
@@ -285,14 +324,21 @@
                 # ),
             ]
             in_channels = out_channels
             out_channels = int(out_channels * factor)
 
         self.conv = nn.Sequential(*conv_layers)
 
+        if self.transformer_layers:
+            self.positional_encoding = PositionalEncoding(d_model=in_channels)
+            encoder_layer = nn.TransformerEncoderLayer(d_model=in_channels, nhead=self.transformer_heads, batch_first=True)
+            self.transformer_encoder = nn.TransformerEncoder(encoder_layer, num_layers=self.transformer_layers)
+        else:
+            self.transformer_encoder = None
+
         self.lstm_dims = lstm_dims
         if lstm_dims:
             self.bi_lstm = nn.LSTM(
                 input_size=in_channels,  # Is this dimension? - this should receive output from maxpool
                 hidden_size=lstm_dims,
                 bidirectional=True,
                 bias=True,
@@ -301,41 +347,157 @@
             )
             current_dims = lstm_dims * 2
         else:
             current_dims = in_channels
 
         self.average_pool = nn.AdaptiveAvgPool1d(1)
 
+        current_dims += int(include_length)
         self.final = nn.Sequential(
             # nn.Linear(in_features=current_dims, out_features=current_dims, bias=True),
             # nn.ReLU(),
-            nn.Linear(in_features=current_dims, out_features=current_dims, bias=True),
+            nn.Linear(in_features=current_dims, out_features=penultimate_dims, bias=True),
             nn.ReLU(),
-            nn.Linear(in_features=current_dims, out_features=num_classes, bias=final_bias),
+            nn.Linear(in_features=penultimate_dims, out_features=num_classes, bias=final_bias),
         )
 
     def forward(self, x):
         # Convert to int because it may be simply a byte
         x = x.int()
+        length = x.shape[-1]
         x = self.embedding(x)
 
         # Transpose seq_len with embedding dims to suit convention of pytorch CNNs (batch_size, input_size, seq_len)
         x = x.transpose(1, 2)
         x = self.conv(x)
 
+        if hasattr(self, 'transformer_encoder') and self.transformer_encoder:
+            x = x.transpose(2, 1)
+            x = self.positional_encoding(x)
+            x = self.transformer_encoder(x)
+            x = x.transpose(1, 2)
+
         if self.lstm_dims:
             x = x.transpose(2, 1)
             output, (h_n, c_n) = self.bi_lstm(x)
             # h_n of shape (num_layers * num_directions, batch, hidden_size)
             # We are using a single layer with 2 directions so the two output vectors are
             # [0,:,:] and [1,:,:]
             # [0,:,:] -> considers the first index from the first dimension
             x = torch.cat((h_n[0, :, :], h_n[1, :, :]), dim=-1)
         elif hasattr(x, 'average_pool'):
             x = self.average_pool(x)
             x = torch.flatten(x, 1)
         else:
             x = torch.mean(x, axis=-1)
 
+        if getattr(self, 'include_length', False):
+            length_tensor = torch.full( (x.shape[0], 1), length/self.length_scaling, device=x.device )
+            x = torch.cat([x, length_tensor], dim=1)
+
         predictions = self.final(x)
 
         return predictions
+
+    def new_final(self, output_size):
+        final_in_features = list(self.final.modules())[1].in_features
+
+        self.final = nn.Sequential(
+            nn.Linear(in_features=final_in_features, out_features=final_in_features, bias=True),
+            nn.ReLU(),
+            nn.Linear(in_features=final_in_features, out_features=output_size, bias=final_bias),
+        )
+
+
+class SequentialDebug(nn.Sequential):
+    def forward(self, input):
+        macs_cummulative = 0
+        from thop import profile
+
+        console.print(f"Input shape {input.shape}")
+        for module in self:
+            console.print(f"Module: {module} ({type(module)})")
+            macs, _ = profile(module, inputs=(input, ))
+            macs_cummulative += int(macs)
+            console.print(f"MACs: {int(macs)} (cummulative {macs_cummulative})")
+
+            input = module(input)
+            console.print(f"Output shape: {input.shape}")
+
+        return input
+
+
+
+class ConvProcessor(nn.Sequential):
+    def __init__(
+        self,
+        in_channels=8,
+        cnn_layers=6,
+        cnn_dims_start=64,
+        kernel_size_maxpool=2,
+        kernel_size=3,
+        factor=2,
+        dropout=0.5,
+        padding="same",
+        padding_mode="zeros",
+    ):
+        out_channels = cnn_dims_start
+        conv_layers = []
+        for layer_index in range(cnn_layers):
+            conv_layers += [
+                nn.Conv1d(
+                    in_channels=in_channels,
+                    out_channels=out_channels,
+                    kernel_size=kernel_size,
+                    padding=padding,
+                    padding_mode=padding_mode,
+                ),
+                nn.ReLU(),
+                nn.Dropout(dropout),
+                nn.MaxPool1d(kernel_size_maxpool),
+                # nn.Conv1d(
+                #     in_channels=out_channels,
+                #     out_channels=out_channels,
+                #     kernel_size=kernel_size,
+                #     stride=kernel_size_maxpool,
+                # ),
+            ]
+            in_channels = out_channels
+            out_channels = int(out_channels * factor)
+
+        super().__init__(*conv_layers)
+
+
+def calc_cnn_dims_start(
+    macc,
+    seq_len:int,
+    embedding_dim:int,
+    cnn_layers:int,
+    kernel_size:int,
+    factor:float,
+    penultimate_dims: int,
+    num_classes: int,
+):
+    """
+    Solving equation M = s k e c + \sum_{l=1}^{L-1} \frac{s}{2^{l} } k c^2 f^{2l-1} + c f^{L-1} p + p o
+    for c.
+
+    Args:
+        macc_per_base (int): the number of multiply-accumulate operations per base pair in the sequence.
+        embedding_dim (int): The size of the embedding.
+        cnn_layers (int): The number of CNN layers.
+        kernel_size (int): The size of the kernel in the CNN
+        factor (float): The multiplying factor for the CNN output layers.
+    """
+    b = kernel_size * embedding_dim * seq_len + factor ** (cnn_layers-1) * penultimate_dims
+    c = penultimate_dims * num_classes - macc
+
+    if cnn_layers == 1:
+        cnn_dims_start = -c/b
+    else:        
+        a = 0.0
+        for layer_index in range(1, cnn_layers):
+            a += seq_len * kernel_size * (0.5**layer_index) * (factor**(2 * layer_index - 1))
+        
+        cnn_dims_start = (-b + np.sqrt(b**2 - 4*a*c))/(2 * a)
+
+    return int(cnn_dims_start + 0.5)
```

### Comparing `bio-corgi-0.2.2/corgi/preprocessing.py` & `bio_corgi-0.4.0/corgi/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bio-corgi-0.2.2/corgi/refseq.py` & `bio_corgi-0.4.0/corgi/refseq.py`

 * *Files identical despite different names*

### Comparing `bio-corgi-0.2.2/corgi/tensor.py` & `bio_corgi-0.4.0/corgi/tensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,47 @@
 
 vocab_to_int = {"A": 1, "C": 2, "G": 3, "T": 4, "N": 0}
 int_to_vocab = dict(zip(vocab_to_int.values(), vocab_to_int.keys()))
 
 
 class TensorDNA(TensorBase):
     def __str__(self):
-        # return str(self.tolist())[:50]
+        seq_str = self.as_chars()
+        return f"{seq_str} [{len(seq_str)}]"
+
+    def show(self, ctx=None, **kwargs):
+        return str(self)
+
+    def as_chars(self):
         items = self.tolist()
         truncate_at = 50
         if type(items) == int:
             items = [items]
 
         length = len(items)
 
         if length > truncate_at:
             midpoint = truncate_at // 2
             items = items[:midpoint] + [".."] + items[-midpoint:]
         chars = [int_to_vocab[x] if x in int_to_vocab else str(x) for x in items]
         seq_str = "".join(chars)
-        return f"{seq_str} [{length}]"
+        return seq_str
 
-    def show(self, ctx=None, **kwargs):
-        return str(self)
+    def as_biopython(self):
+        from Bio.Seq import Seq
+        return Seq(self.as_chars())
 
 
 def dna_seq_to_numpy(seq) -> np.ndarray:
     """
     Transforms a sequence from biopython to a numpy array.
 
     Should this be a transform??
     """
-    seq_as_numpy = np.array(str(seq), "c")
+    seq_as_numpy = np.array(str(seq).upper(), "c")
     seq_as_numpy = seq_as_numpy.view(np.uint8)
     # Ignore any characters in sequence which are below an ascii value of 'A' i.e. 65
     seq_as_numpy = seq_as_numpy[seq_as_numpy >= ord("A")]
     for character, value in vocab_to_int.items():
         seq_as_numpy[seq_as_numpy == ord(character)] = value
     seq_as_numpy = seq_as_numpy[seq_as_numpy < len(vocab_to_int)]
     seq_as_numpy = np.array(seq_as_numpy, dtype="u1")
```

### Comparing `bio-corgi-0.2.2/pyproject.toml` & `bio_corgi-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bio-corgi"
-version = "0.2.2"
+version = "0.4.0"
 description = "Classifier for ORganelle Genomes Inter alia"
 authors = ["Robert Turnbull <robert.turnbull@unimelb.edu.au>"]
 license = "Apache Software License 2.0"
 readme = "README.rst"
 repository = "https://github.com/rbturnbull/corgi"
 documentation = "https://rbturnbull.github.io/corgi/"
 homepage = "https://github.com/rbturnbull/corgi"
@@ -24,25 +24,25 @@
 python = ">=3.8,<3.12"
 biopython = "^1.79"
 fastai = "^2.4.1"
 dask = "^2021.7.1"
 progressbar2 = "^3.53.1"
 h5py = "^3.1.0"
 humanize = "^3.10.0"
-pyarrow = "^4.0.1"
+pyarrow = ">=5.0.0"
 plotly = "^5.3.1"
 appdirs = "^1.4.4"
 beautifulsoup4 = "^4.10.0"
 httpx = "^0.20.0"
 wandb = "^0.12.9"
 optuna = "^2.10.0"
 cryptography = "^36.0.1"
 PyMySQL = "^1.0.2"
 termgraph = "^0.5.3"
-torchapp = "^0.2.3"
+torchapp = ">=0.3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 ipykernel = "^6.6.1"
 coverage = "^5.5"
 autopep8 = "^1.5.7"
 Sphinx = "^4.2.0"
```

### Comparing `bio-corgi-0.2.2/PKG-INFO` & `bio_corgi-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bio-corgi
-Version: 0.2.2
+Version: 0.4.0
 Summary: Classifier for ORganelle Genomes Inter alia
 Home-page: https://github.com/rbturnbull/corgi
 License: Apache Software License 2.0
 Keywords: metagenomic classifier,tiara,DNA,bioinformatics,fastai,pytorch,deep learning,command-line interface
 Author: Robert Turnbull
 Author-email: robert.turnbull@unimelb.edu.au
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: biopython (>=1.79,<2.0)
@@ -27,17 +28,17 @@
 Requires-Dist: fastai (>=2.4.1,<3.0.0)
 Requires-Dist: h5py (>=3.1.0,<4.0.0)
 Requires-Dist: httpx (>=0.20.0,<0.21.0)
 Requires-Dist: humanize (>=3.10.0,<4.0.0)
 Requires-Dist: optuna (>=2.10.0,<3.0.0)
 Requires-Dist: plotly (>=5.3.1,<6.0.0)
 Requires-Dist: progressbar2 (>=3.53.1,<4.0.0)
-Requires-Dist: pyarrow (>=4.0.1,<5.0.0)
+Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: termgraph (>=0.5.3,<0.6.0)
-Requires-Dist: torchapp (>=0.2.3,<0.3.0)
+Requires-Dist: torchapp (>=0.3.1)
 Requires-Dist: wandb (>=0.12.9,<0.13.0)
 Project-URL: Documentation, https://rbturnbull.github.io/corgi/
 Project-URL: Repository, https://github.com/rbturnbull/corgi
 Description-Content-Type: text/x-rst
 
 .. image:: https://raw.githubusercontent.com/rbturnbull/corgi/main/docs/images/corgi-banner.svg
 
@@ -94,15 +95,17 @@
 Usage
 ============
 
 To make predictions, run the ``corgi`` command line tool:
 
 .. code-block:: bash
 
-    corgi --fasta <input fasta file> --output-csv <results>
+    corgi --file <input seq file>
+
+This will create a directory with the predictions in a CSV file and in fasta format.
 
 For more information about the other options, see the help with:
 
 .. code-block:: bash
 
     corgi --help
```

