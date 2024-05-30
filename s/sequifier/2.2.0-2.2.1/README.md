# Comparing `tmp/sequifier-2.2.0.tar.gz` & `tmp/sequifier-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequifier-2.2.0.tar", max compression
+gzip compressed data, was "sequifier-2.2.1.tar", max compression
```

## Comparing `sequifier-2.2.0.tar` & `sequifier-2.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.2.0/LICENSE
--rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.2.0/README.md
--rw-r--r--   0        0        0      919 2024-05-26 14:50:12.735681 sequifier-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4707 2024-05-01 11:32:11.871058 sequifier-2.2.0/src/sequifier/config/infer_config.py
--rw-r--r--   0        0        0     1760 2024-05-01 11:32:11.871370 sequifier-2.2.0/src/sequifier/config/preprocess_config.py
--rw-r--r--   0        0        0     7582 2024-05-26 14:50:12.736059 sequifier-2.2.0/src/sequifier/config/train_config.py
--rw-r--r--   0        0        0     2851 2024-05-26 14:50:12.736267 sequifier-2.2.0/src/sequifier/helpers.py
--rw-r--r--   0        0        0    20796 2024-05-26 14:50:12.736739 sequifier-2.2.0/src/sequifier/infer.py
--rw-r--r--   0        0        0    12716 2024-05-01 11:32:11.872842 sequifier-2.2.0/src/sequifier/preprocess.py
--rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.2.0/src/sequifier/sequifier.py
--rw-r--r--   0        0        0    23893 2024-05-26 14:50:12.737107 sequifier-2.2.0/src/sequifier/train.py
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.2.1/LICENSE
+-rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.2.1/README.md
+-rw-r--r--   0        0        0      919 2024-05-30 06:54:53.765251 sequifier-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4706 2024-05-30 06:54:53.765652 sequifier-2.2.1/src/sequifier/config/infer_config.py
+-rw-r--r--   0        0        0     1760 2024-05-01 11:32:11.871370 sequifier-2.2.1/src/sequifier/config/preprocess_config.py
+-rw-r--r--   0        0        0     7581 2024-05-30 06:54:53.766119 sequifier-2.2.1/src/sequifier/config/train_config.py
+-rw-r--r--   0        0        0     2802 2024-05-30 06:54:53.766510 sequifier-2.2.1/src/sequifier/helpers.py
+-rw-r--r--   0        0        0    20794 2024-05-30 06:54:53.767039 sequifier-2.2.1/src/sequifier/infer.py
+-rw-r--r--   0        0        0    12713 2024-05-30 06:54:53.767369 sequifier-2.2.1/src/sequifier/preprocess.py
+-rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.2.1/src/sequifier/sequifier.py
+-rw-r--r--   0        0        0    23887 2024-05-30 06:54:53.767693 sequifier-2.2.1/src/sequifier/train.py
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.2.1/PKG-INFO
```

### Comparing `sequifier-2.2.0/LICENSE` & `sequifier-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sequifier-2.2.0/README.md` & `sequifier-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sequifier-2.2.0/pyproject.toml` & `sequifier-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequifier"
-version = "2.2.0"
+version = "2.2.1"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "Train a transformer model with the command line"
 keywords = ["transformer", "sequence classification", "machine learning", "sequence", "sequence modelling", "nlp", "language", "language modelling", "torch", "pytorch"]
 readme = "README.md"
 license = "BSD 3-Clause"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `sequifier-2.2.0/src/sequifier/config/infer_config.py` & `sequifier-2.2.1/src/sequifier/config/infer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         assert v == False or np.max(
             np.array(list(values["target_column_types"].values())) == "categorical"
         ), f"map_to_id can only be True if at least one target variable is categorical: {np.array(values['target_column_types'].values()) == 'categorical'}"
         return v
 
     @validator("sample_from_distribution", always=True)
     def validate_sample_from_distribution(cls, v, values):
-
         if (
             v
             and np.max(np.array(list(values["target_column_types"].values())) == "real")
             == 1
         ):
             raise ValueError(
                 "sample_from_distribution can only be used when all target columns are categorical"
```

### Comparing `sequifier-2.2.0/src/sequifier/config/preprocess_config.py` & `sequifier-2.2.1/src/sequifier/config/preprocess_config.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.2.0/src/sequifier/config/train_config.py` & `sequifier-2.2.1/src/sequifier/config/train_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
     dropout: float = 0.0
     loss_weights: Optional[dict[str, float]]
     optimizer: CustomValidation[DotDict]  # mandatory; default value in __init__
     scheduler: CustomValidation[DotDict]  # mandatory; default value in __init__
     continue_training: bool = True
 
     def __init__(self, **kwargs):
-
         super().__init__(
             **{k: v for k, v in kwargs.items() if k not in ["optimizer", "scheduler"]}
         )
 
         optimizer = kwargs.get("optimizer", {"name": "Adam"})
         scheduler = kwargs.get(
             "scheduler", {"name": "StepLR", "step_size": 1, "gamma": 0.99}
```

### Comparing `sequifier-2.2.0/src/sequifier/helpers.py` & `sequifier-2.2.1/src/sequifier/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,25 +43,22 @@
         (data["inputCol"].values == input_col) for input_col in selected_columns
     ]
     filter_ = np.logical_or.reduce(column_filters)
     return data.loc[filter_, :]
 
 
 def numpy_to_pytorch(data, column_types, target_columns, seq_length, device, to_device):
-
     if "target" in data:
         targets = {}
         for target_column in target_columns:
             target = tensor(
                 data.query(f"inputCol=='{target_column}'")["target"].values
             ).to(column_types[target_column])
             if to_device:
                 target = target.to(device)
-            else:
-                target = None
             targets[target_column] = target
     else:
         targets = None
 
     sequence = {}
     for col in column_types.keys():
         f = data["inputCol"].values == col
```

### Comparing `sequifier-2.2.0/src/sequifier/infer.py` & `sequifier-2.2.1/src/sequifier/infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
     if config.output_probabilities:
         os.makedirs(
             os.path.join(config.project_path, "outputs", "probabilities"), exist_ok=True
         )
         for target_column in inferer.target_columns:
             if inferer.target_column_types[target_column] == "categorical":
-
                 probabilities_path = os.path.join(
                     config.project_path,
                     "outputs",
                     "probabilities",
                     f"{model_id}-{target_column}-probabilities.{config.write_format}",
                 )
                 print(f"Writing probabilities to {probabilities_path}")
@@ -168,15 +167,14 @@
         [data] + autoregression_additional_observations, axis=0
     ).sort_values(["sequenceId", "subsequenceId"])
 
     return data
 
 
 def get_probs_preds(config, inferer, data, column_types):
-
     X, _ = numpy_to_pytorch(
         data,
         column_types,
         config.target_columns,
         config.seq_length,
         config.device,
         to_device=True,
```

### Comparing `sequifier-2.2.0/src/sequifier/preprocess.py` & `sequifier-2.2.1/src/sequifier/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 
         delete_path = os.path.join(project_path, "data", "temp")
         assert len(delete_path) > 9
         delete_command = f"rm -rf {delete_path}*"
         os.system(delete_command)
 
     def export_metadata(self, id_maps, n_classes, col_types, min_max_values):
-
         data_driven_config = {
             "n_classes": n_classes,
             "id_maps": id_maps,
             "split_paths": self.split_paths,
             "column_types": col_types,
             "min_max_values": min_max_values,
         }
@@ -280,15 +279,14 @@
     )
     return sequences
 
 
 def extract_subsequences(
     in_seq, seq_length, data_columns, target_columns, return_targets
 ):
-
     if return_targets:
         nseq = max(
             len(in_seq[target_columns[0]]) - seq_length - 1,  # any column will do
             min(1, len(in_seq[target_columns[0]])),  # any column will do
         )
 
         targets = [
@@ -361,15 +359,14 @@
     return data
 
 
 def combine_multiprocessing_outputs(
     project_path, n_splits, n_batches, dataset_name, write_format
 ):
     for split in range(n_splits):
-
         out_path = os.path.join(
             project_path, "data", f"{dataset_name}-split{split}.{write_format}"
         )
 
         files = [
             os.path.join(
                 project_path,
```

### Comparing `sequifier-2.2.0/src/sequifier/sequifier.py` & `sequifier-2.2.1/src/sequifier/sequifier.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.2.0/src/sequifier/train.py` & `sequifier-2.2.1/src/sequifier/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     X_train, y_train = numpy_to_pytorch(
         data_train,
         column_types,
         config.target_columns,
         config.seq_length,
         config.training_spec.device,
-        to_device=True,
+        to_device=False,
     )
     del data_train
 
     data_valid = read_data(
         normalize_path(config.validation_data_path, config.project_path),
         config.read_format,
     )
@@ -60,15 +60,15 @@
 
     X_valid, y_valid = numpy_to_pytorch(
         data_valid,
         column_types,
         config.target_columns,
         config.seq_length,
         config.training_spec.device,
-        to_device=True,
+        to_device=False,
     )
     del data_valid
 
     torch.manual_seed(config.seed)
     np.random.seed(config.seed)
 
     model = torch.compile(TransformerModel(config).to(config.training_spec.device))
@@ -268,15 +268,14 @@
     def train_model(self, X_train, y_train, X_valid, y_valid):
         best_val_loss = float("inf")
         n_epochs_no_improvemet = 0
 
         for epoch in range(
             self.start_epoch, self.hparams.training_spec.epochs + self.start_epoch
         ):
-
             if (
                 self.early_stopping_epochs is None
                 or n_epochs_no_improvemet < self.early_stopping_epochs
             ):
                 epoch_start_time = time.time()
                 self.train_epoch(X_train, y_train, epoch)
                 total_loss, total_losses, output = self.evaluate(X_valid, y_valid)
@@ -343,15 +342,15 @@
             np.random.choice(
                 np.arange(num_batches), size=num_batches, replace=False
             ).flatten()
         )
         for batch_count, batch in enumerate(batch_order):
             batch_start = batch * self.batch_size
             data, targets = self.get_batch(
-                X_train, y_train, batch_start, self.batch_size, to_device=False
+                X_train, y_train, batch_start, self.batch_size, to_device=True
             )
             output = self(data)
             loss, losses = self.calculate_loss(output, targets)
 
             loss.backward()
 
             torch.nn.utils.clip_grad_norm_(self.parameters(), 0.5)
@@ -382,15 +381,14 @@
         losses = {}
         for target_column, target_column_type in self.target_column_types.items():
             if target_column_type == "categorical":
                 output[target_column] = output[target_column].view(
                     -1, self.n_classes[target_column]
                 )
             elif target_column_type == "real":
-
                 output[target_column] = output[target_column].flatten()
             else:
                 pass
             losses[target_column] = self.criterion[target_column](
                 output[target_column], targets[target_column]
             )
 
@@ -418,15 +416,15 @@
         with torch.no_grad():
             for batch_start in range(
                 0,
                 X_valid[self.target_columns[0]].size(0),
                 self.batch_size,  # any column will do
             ):
                 data, targets = self.get_batch(
-                    X_valid, y_valid, batch_start, self.batch_size, to_device=False
+                    X_valid, y_valid, batch_start, self.batch_size, to_device=True
                 )
                 output = self(data)
                 loss, losses = self.calculate_loss(output, targets)
                 for target_column, bloss in losses.items():
                     total_losses[target_column] += bloss
                 total_loss += loss
 
@@ -569,30 +567,28 @@
         open_mode = "w" if self.start_epoch == 1 else "a"
         self.log_file = LogFile(
             os.path.join(self.project_path, "logs", f"sequifier-{self.model_name}.txt"),
             open_mode,
         )
 
     def load_weights_conditional(self):
-
         latest_model_path = self.get_latest_model_name()
 
         if latest_model_path is not None and self.continue_training:
             checkpoint = torch.load(latest_model_path)
             self.load_state_dict(checkpoint["model_state_dict"])
             self.start_epoch = (
                 int(re.findall("epoch-([0-9]+)", latest_model_path)[0]) + 1
             )
             return f"Loading model weights from {latest_model_path}"
         else:
             self.start_epoch = 1
             return "Initializing new model"
 
     def get_latest_model_name(self):
-
         checkpoint_path = os.path.join(self.project_path, "checkpoints", "*")
 
         files = glob.glob(
             checkpoint_path
         )  # * means all if need specific format then *.csv
         files = [
             file for file in files if os.path.split(file)[1].startswith(self.model_name)
@@ -607,15 +603,14 @@
     model_path, training_config_path, args_config, device, infer_with_dropout
 ):
     training_config = load_train_config(
         training_config_path, args_config, args_config["on_unprocessed"]
     )
 
     with torch.no_grad():
-
         model = TransformerModel(training_config)
         model.log_file.write(f"Loading model weights from {model_path}")
         model_state = torch.load(model_path)
         model.load_state_dict(model_state["model_state_dict"])
 
         model.eval()
 
@@ -630,15 +625,14 @@
 
         model = torch.compile(model).to(device)
 
     return model
 
 
 def infer_with_model(model, x, device, size, target_columns):
-
     outs0 = [
         model({col: torch.from_numpy(x_).to(device) for col, x_ in x_sub.items()})
         for x_sub in x
     ]
     outs = {
         target_column: np.concatenate(
             [o[target_column].cpu().detach().numpy() for o in outs0],
```

### Comparing `sequifier-2.2.0/PKG-INFO` & `sequifier-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequifier
-Version: 2.2.0
+Version: 2.2.1
 Summary: Train a transformer model with the command line
 Home-page: https://github.com/0xideas/sequifier
 License: BSD 3-Clause
 Keywords: transformer,sequence classification,machine learning,sequence,sequence modelling,nlp,language,language modelling,torch,pytorch
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.9,<4.0
```

