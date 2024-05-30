# Comparing `tmp/aigarmic-1.0.0.tar.gz` & `tmp/aigarmic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigarmic-1.0.0.tar", max compression
+gzip compressed data, was "aigarmic-1.0.1.tar", max compression
```

## Comparing `aigarmic-1.0.0.tar` & `aigarmic-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-03-18 14:37:24.051056 aigarmic-1.0.0/LICENSE
--rw-r--r--   0        0        0     1621 2024-04-02 13:48:27.405010 aigarmic-1.0.0/README.md
--rw-r--r--   0        0        0     1230 2024-04-02 14:09:42.845157 aigarmic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      725 2024-04-02 13:48:27.407941 aigarmic-1.0.0/src/aigarmic/__init__.py
--rw-r--r--   0        0        0     4315 2024-04-02 13:48:27.408048 aigarmic-1.0.0/src/aigarmic/_img_utils.py
--rw-r--r--   0        0        0     2635 2024-04-02 13:48:27.408156 aigarmic-1.0.0/src/aigarmic/_nn_design.py
--rw-r--r--   0        0        0     1766 2024-04-02 13:48:27.408419 aigarmic-1.0.0/src/aigarmic/clean_up_annotations.py
--rw-r--r--   0        0        0     7370 2024-04-02 13:48:27.408707 aigarmic-1.0.0/src/aigarmic/file_handlers.py
--rw-r--r--   0        0        0     7386 2024-04-02 13:48:27.409076 aigarmic-1.0.0/src/aigarmic/main.py
--rw-r--r--   0        0        0     3601 2024-04-02 13:48:27.409543 aigarmic-1.0.0/src/aigarmic/manual_annotator.py
--rw-r--r--   0        0        0     8270 2024-04-02 13:48:27.409706 aigarmic-1.0.0/src/aigarmic/model.py
--rw-r--r--   0        0        0     3324 2024-04-02 13:48:27.409853 aigarmic-1.0.0/src/aigarmic/model_performance.py
--rw-r--r--   0        0        0    29130 2024-04-02 13:48:27.410129 aigarmic-1.0.0/src/aigarmic/plate.py
--rw-r--r--   0        0        0     4100 2024-04-02 13:48:27.410320 aigarmic-1.0.0/src/aigarmic/process_plate_image.py
--rw-r--r--   0        0        0     2025 2024-04-02 13:48:27.410557 aigarmic-1.0.0/src/aigarmic/rename_images.py
--rw-r--r--   0        0        0     8898 2024-04-02 13:48:27.410719 aigarmic-1.0.0/src/aigarmic/train.py
--rw-r--r--   0        0        0     5899 2024-04-02 13:48:27.410970 aigarmic-1.0.0/src/aigarmic/train_modular.py
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 aigarmic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-18 14:37:24.051056 aigarmic-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2651 2024-04-16 10:50:53.412995 aigarmic-1.0.1/README.md
+-rw-r--r--   0        0        0     1482 2024-05-30 19:00:24.902979 aigarmic-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      725 2024-04-02 13:48:27.407941 aigarmic-1.0.1/src/aigarmic/__init__.py
+-rw-r--r--   0        0        0     4402 2024-04-16 10:44:23.894310 aigarmic-1.0.1/src/aigarmic/_img_utils.py
+-rw-r--r--   0        0        0     2735 2024-04-16 10:44:23.894800 aigarmic-1.0.1/src/aigarmic/_nn_design.py
+-rw-r--r--   0        0        0     1838 2024-04-16 10:44:23.894958 aigarmic-1.0.1/src/aigarmic/clean_up_annotations.py
+-rw-r--r--   0        0        0     7486 2024-04-16 10:44:23.895211 aigarmic-1.0.1/src/aigarmic/file_handlers.py
+-rw-r--r--   0        0        0     7531 2024-04-16 10:44:23.895538 aigarmic-1.0.1/src/aigarmic/main.py
+-rw-r--r--   0        0        0     3680 2024-04-16 10:44:23.895749 aigarmic-1.0.1/src/aigarmic/manual_annotator.py
+-rw-r--r--   0        0        0     8328 2024-04-16 10:44:23.896009 aigarmic-1.0.1/src/aigarmic/model.py
+-rw-r--r--   0        0        0     3353 2024-04-16 10:44:23.896613 aigarmic-1.0.1/src/aigarmic/model_performance.py
+-rw-r--r--   0        0        0    29245 2024-04-16 10:44:23.896903 aigarmic-1.0.1/src/aigarmic/plate.py
+-rw-r--r--   0        0        0     4374 2024-04-16 10:44:23.897095 aigarmic-1.0.1/src/aigarmic/process_plate_image.py
+-rw-r--r--   0        0        0     2025 2024-04-02 13:48:27.410557 aigarmic-1.0.1/src/aigarmic/rename_images.py
+-rw-r--r--   0        0        0     9265 2024-04-16 10:44:23.897243 aigarmic-1.0.1/src/aigarmic/train.py
+-rw-r--r--   0        0        0     5969 2024-04-16 10:44:23.897393 aigarmic-1.0.1/src/aigarmic/train_modular.py
+-rw-r--r--   0        0        0     3554 1970-01-01 00:00:00.000000 aigarmic-1.0.1/PKG-INFO
```

### Comparing `aigarmic-1.0.0/LICENSE` & `aigarmic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aigarmic-1.0.0/README.md` & `aigarmic-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -34,15 +34,40 @@
 https://aigarmic.readthedocs.io/en/latest/introduction.html#typical-workflows
 
 ## Author information
 
 The lead developer of ``AIgarMIC`` is Alessandro Gerada (https://github.com/agerada/ and https://agerada.github.io/), 
 University of Liverpool, UK (alessandro.gerada@liverpool.ac.uk).
 
+## Cite
+
+If you are using `AIgarMIC` in your research project, please cite [TO FOLLOW].
+
+To cite the validation data and developmental approach described in the `AIgarMIC` validation manuscript, please cite:
+
+    @article{geradaDeterminationMinimumInhibitory2024,
+      title = {Determination of Minimum Inhibitory Concentrations Using Machine-Learning-Assisted Agar Dilution},
+      author = {Gerada, Alessandro and Harper, Nicholas and Howard, Alex and Reza, Nada and Hope, William},
+      editor = {Shier, Kileen L.},
+      date = {2024-03-22},
+      journaltitle = {Microbiology Spectrum},
+      shortjournal = {Microbiol Spectr},
+      pages = {e04209-23},
+      issn = {2165-0497},
+      doi = {10.1128/spectrum.04209-23},
+      url = {https://journals.asm.org/doi/10.1128/spectrum.04209-23},
+      urldate = {2024-04-02},
+      langid = {english}
+    }
+
 ## External links
 
 The manuscript describing the validation of `AIgarMIC` can be found at: https://doi.org/10.1128/spectrum.04209-23.
 Optional asset data is available at: https://10.17638/datacat.liverpool.ac.uk/2631.
 
+## Contributing
+
+We welcome contributions to ``AIgarMIC``. Please follow our [contributing guidelines](https://github.com/agerada/AIgarMIC/blob/paper/CONTRIBUTING.md).
+
 ## License
 
 `AIgarMIC` is provided under the GNU General Public License v3.0. For more information, see the LICENSE file.
```

### Comparing `aigarmic-1.0.0/pyproject.toml` & `aigarmic-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigarmic"
-version = "1.0.0"
+version = "1.0.1"
 description = "Machine-learning assisted agar dilution MIC"
 authors = ["Alessandro Gerada"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 AIgarMIC = "aigarmic.main:main"
@@ -18,15 +18,15 @@
 python = ">=3.9,<3.11"
 imutils = ">=0.5"
 matplotlib = ">=3.6"
 numpy = ">=1.26"
 opencv-python = ">=4.9"
 pytest = ">=8.1"
 tensorflow-macos = { version = ">=2.11,<=2.15", markers = "platform_system=='Darwin' and platform_machine=='arm64'"}
-tensorflow = { version = ">=2.11,<=2.15", markers = "platform_system!='Darwin' and platform_machine!='arm64'"}
+tensorflow = { version = ">=2.11,<=2.15", markers = "platform_system!='Darwin' and platform_machine!='arm64' or platform_system=='Darwin' and platform_machine!='arm64'"}
 scikit-learn = ">=1.4"
 sphinx = ">=7.2"
 sphinx-argparse = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
@@ -34,7 +34,15 @@
 myst-nb = {version = ">=1.0.0", python = ">=3.9"}
 sphinx-autoapi = ">=3.0.0"
 sphinx-rtd-theme = ">=2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+markers = [
+    "assets_required: requires optional assets in project root (skip with '-m \"not assets_required\"'"
+]
+
+[tool.pylint]
+ignored-modules = ["cv2.errors"]
```

### Comparing `aigarmic-1.0.0/src/aigarmic/__init__.py` & `aigarmic-1.0.1/src/aigarmic/__init__.py`

 * *Files identical despite different names*

### Comparing `aigarmic-1.0.0/src/aigarmic/_img_utils.py` & `aigarmic-1.0.1/src/aigarmic/_img_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 
     :param image: Image loaded using cv2.imread
     :param size_x: Width to resize image to (pixels)
     :param size_y: Height to resize image to (pixels)
     :return: Image as a numpy array
     """
     # resize
-    image = cv2.resize(image, (size_x, size_y))
+    image = cv2.resize(image, (size_x, size_y))  # pylint: disable=no-member
     # convert from BGR to RGB
-    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)  # pylint: disable=no-member
     image = image.reshape(1, size_x, size_y, 3)
     image = image.astype(np.float32)
     return image
 
 
 def keras_image_to_cv2(image: tf.Tensor) -> np.ndarray:
     """
     Convert a keras image to a cv2 image
 
     :param image: Image as a tensor
     :return: Image as a numpy array
     """
     img = image.numpy().astype(np.uint8)
-    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)  # pylint: disable=no-member
     return img
 
 
 def get_image_paths(dir_path,
                     extensions: tuple[str, ...] = ('.jpg', '.JPG')) -> Union[list[str], dict[str, list[str]]]:
     """
     If there are no subdirectories in dir, returns a list of image paths
```

### Comparing `aigarmic-1.0.0/src/aigarmic/_nn_design.py` & `aigarmic-1.0.1/src/aigarmic/_nn_design.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # Author: 	Alessandro Gerada
 # Date: 	2023-08-11
 # Copyright: 	Alessandro Gerada 2023
 # Email: 	alessandro.gerada@liverpool.ac.uk
 
 """Template NN designs as reported in Gerada et al. 2024 Microbiology Spectrum paper"""
 
-from tensorflow.keras import layers
-from tensorflow.keras.models import Sequential
+from tensorflow.keras import layers  # pylint: disable=import-error,no-name-in-module
+from tensorflow.keras.models import Sequential  # pylint: disable=import-error,no-name-in-module
 
 
 def model_design_spectrum_2024_binary_first_step(image_width: int,
                                                  image_height: int,
                                                  augmentation: bool = True):
     design = [
         #  spectrum 2024 first-step model
```

### Comparing `aigarmic-1.0.0/src/aigarmic/clean_up_annotations.py` & `aigarmic-1.0.1/src/aigarmic/clean_up_annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 import argparse
 import cv2  # pylint: disable=import-error
 from aigarmic._img_utils import get_image_paths, Deleter, in_list
 
 
 def clean_up_annotations_parser():
-    parser = argparse.ArgumentParser("""
+    parser = argparse.ArgumentParser(description="""
         Clean up duplicate images in annotation folders
         """)
     parser.add_argument('input_dir', type=str,
-                        help="Input directory - can contain subdirectory of images which will be processed separately")
+                        help="Input directory - can contain subdirectories of images which will be processed separately")
     parser.add_argument('-q', '--quiet', action='store_true',
                         help="Suppress file deletion warnings (CAUTION)")
     return parser
 
 
 def main():
     parser = clean_up_annotations_parser()
@@ -30,25 +30,25 @@
     images_paths = get_image_paths(args.input_dir)
     
     deleter = Deleter(confirm=False if args.quiet else True)
 
     _images_list = []
     if isinstance(images_paths, list):
         for i in images_paths: 
-            _image = cv2.imread(i)
+            _image = cv2.imread(i)  # pylint: disable=no-member
             if not in_list(_image, _images_list): 
                 _images_list.append(_image)
             else: 
                 deleter.delete_file(i)
 
     if isinstance(images_paths, dict):
         for _, v in images_paths.items():
             _images_list = []
             for i in v: 
-                _image = cv2.imread(i)
+                _image = cv2.imread(i)  # pylint: disable=no-member
                 if not in_list(_image, _images_list): 
                     _images_list.append(_image)
                 else: 
                     deleter.delete_file(i)
 
 
 if __name__ == "__main__":
```

### Comparing `aigarmic-1.0.0/src/aigarmic/file_handlers.py` & `aigarmic-1.0.1/src/aigarmic/file_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,37 +34,37 @@
     :param image_width: Image width in pixels
     :param image_height: Image height in pixels
     :param seed: Random seed for dataset splitting
     :param val_split: Proportion of data to use for validation
     :param batch_size: Batch size for datasets
     :return: Tuple containing training and validation datasets
     """
-    train_dataset = tf.keras.utils.image_dataset_from_directory(
+    train_dataset = tf.keras.utils.image_dataset_from_directory(  # pylint: disable=no-member
                 directory,
                 validation_split=val_split, 
                 subset='training',
                 seed=seed,
                 image_size=(image_width, image_height), 
                 batch_size=batch_size, 
                 label_mode=label_mode
             )
-    val_dataset = tf.keras.utils.image_dataset_from_directory(
+    val_dataset = tf.keras.utils.image_dataset_from_directory(  # pylint: disable=no-member
         directory,
         validation_split=val_split, 
         subset='validation', 
         seed=seed,
         image_size=(image_width, image_height), 
         batch_size=batch_size, 
         label_mode=label_mode
     )
     return train_dataset, val_dataset
 
 
 def predict_colony_images_from_directory(directory: Optional[Union[str, pathlib.Path]],
-                                         model: tf.keras.models.Model,
+                                         model: tf.keras.models.Model,  # pylint: disable=no-member
                                          class_names: list[str],
                                          image_width: int,
                                          image_height: int,
                                          model_type: str,
                                          save_path: Optional[Union[str, pathlib.Path]] = None,
                                          binary_threshold: float = 0.5) -> list[dict]:
     """
@@ -84,15 +84,15 @@
     output = []
     file_paths = {i: os.listdir(os.path.join(directory, i)) for i in class_names}
     # add subdirectories
     file_paths = {i: [os.path.join(directory, i, j) for j in file_paths[i] if j.count(".jpg") > 0] for i in file_paths}
 
     for i in file_paths:
         for j in file_paths[i]:
-            image = cv2.imread(j)
+            image = cv2.imread(j)  # pylint: disable=no-member
             true_class = i
             directory = j
             prediction = model.predict(convert_cv2_to_keras(image, image_width, image_height))
             if model_type == "binary":
                 [prediction] = prediction.reshape(-1)
                 predicted_class = class_names[0] if prediction <= binary_threshold else class_names[1]
             elif model_type == "softmax":
```

### Comparing `aigarmic-1.0.0/src/aigarmic/main.py` & `aigarmic-1.0.1/src/aigarmic/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,30 +56,30 @@
     model_image_x = args.dimensions[0]
     model_image_y = args.dimensions[1]
     supported_model_types = ['softmax', 'binary']
 
     plate_images_paths = get_paths_from_directory(args.directory)
 
     if args.check_contours:
-        cv2.startWindowThread()
+        cv2.startWindowThread()  # pylint: disable=no-member
         for abx, paths in plate_images_paths.items():
             for path in paths:
-                _image = cv2.imread(path)
+                _image = cv2.imread(path)  # pylint: disable=no-member
                 try:
                     split_by_grid(_image,
                                   visualise_contours=True,
                                   plate_name=abx + '_' + str(get_concentration_from_path(path)))
                 except ValueError as e:
                     raise ValueError from e
 
         pos_replies = ['y', 'yes', 'ye']
         neg_replies = ['n', 'no']
-        cv2.waitKey(1)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
+        cv2.waitKey(1)  # pylint: disable=no-member
+        cv2.destroyAllWindows()  # pylint: disable=no-member
+        cv2.waitKey(1)  # pylint: disable=no-member
         while True:
             input_key = input("""Completed contour checks. Would you like to continue with annotation? [Y / N]
                               Please only proceed if all images have correctly identified 96 boxes!
                               """)
             input_key = input_key.lower()
             if input_key in neg_replies:
                 sys.exit()
```

### Comparing `aigarmic-1.0.0/src/aigarmic/manual_annotator.py` & `aigarmic-1.0.1/src/aigarmic/manual_annotator.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 # Author: 	Alessandro Gerada
 # Date: 	2023-01-28
 # Copyright: 	Alessandro Gerada 2023
 # Email: 	alessandro.gerada@liverpool.ac.uk
 
 """
 This script shows random images from 96-well plates, and waits for user input to 
-annotate the image. Use the following key: 
-0 = no growth
-1 = faint growth or colony
-2 = normal growth
+annotate the image. Supports up to 10 growth labels (0 to 9).
 The output is stored in annotations/
 """
 
 from aigarmic.file_handlers import get_concentration_from_path, get_paths_from_directory
 from aigarmic.plate import Plate
 import os
 import cv2  # pylint: disable=import-error
 import argparse
 from random import choice
 from datetime import datetime
 
 
 def manual_annotator_parser():
-    parser = argparse.ArgumentParser(description="Manually annotate plate images")
+    parser = argparse.ArgumentParser(description="""
+        Manually label random colony images from plates to generate annotated image database.
+        Supports labels from 0 to 9. """)
     parser.add_argument('input_directory', type=str,
                         help="Directory containing plate images")
     parser.add_argument('-o', '--output_directory', type=str, default='annotations/',
                         help='Path to store annotation output files')
     return parser
 
 
@@ -51,18 +50,15 @@
                 concentration = get_concentration_from_path(path)
                 plates.append(Plate(abx, concentration, path, visualise_contours=False,
                                     n_row=8, n_col=12))
             except FileNotFoundError as e:
                 print(f"Error while trying to import {path}: ")
                 print(e)
 
-    print("Use the following key for input: ")
-    print("0 = no growth")
-    print("1 = faint growth or colony")
-    print("2 = normal growth")
+    print("Enter a number from 0 to 9 corresponding to growth quality")
     print("Press esc to cancel at any time. ")
     print()
 
     n = 0
     while True: 
         try: 
             n = int(input("How many images do you want to annotate? "))
@@ -74,18 +70,18 @@
     output_images = []
     output_annotations = []
     output_image_codes = []
 
     for i in range(n): 
         x, code = choice(plates).get_colony_image()
         code = code + '_' + datetime.now().strftime('%Y-%m-%d_%H%M%S')
-        cv2.imshow('image', x)
+        cv2.imshow('image', x)  # pylint: disable=no-member
         print("Please enter classification for this image..")
         while True: 
-            input_key = cv2.waitKey()
+            input_key = cv2.waitKey()  # pylint: disable=no-member
             if input_key not in codes: 
                 print("Input not recognised, please try again..")
                 continue
             else: 
                 break
         if input_key in stop_codes:
             print("Exiting.")
@@ -101,12 +97,12 @@
 
     # make class folders
     for a in output_annotations: 
         if not os.path.exists(os.path.join(output_dir, str(a))): 
             os.mkdir(os.path.join(output_dir, str(a)))
     
     for i, a, c in zip(output_images, output_annotations, output_image_codes):
-        cv2.imwrite(os.path.join(output_dir, str(a), c + '.jpg'), i)
+        cv2.imwrite(os.path.join(output_dir, str(a), c + '.jpg'), i)  # pylint: disable=no-member
 
 
 if __name__ == "__main__": 
     main()
```

### Comparing `aigarmic-1.0.0/src/aigarmic/model.py` & `aigarmic-1.0.1/src/aigarmic/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         :param path: path to saved model
         :param trained_x: image width used to train model
         :param trained_y: image height used to train model
         :param key: key to interpret model output
         """
         self.path = path
-        self.keras_data = tf.keras.models.load_model(path)
+        self.keras_data = tf.keras.models.load_model(path)  # pylint: disable=no-member
         if key:
             self.key = key
         else:
             # infer key from final output layer of loaded model
             final_layer = self.keras_data.layers[-1]
             inferred_key = [str(i) for i in range(final_layer.output.shape[1])]
             self.key = inferred_key
@@ -66,15 +66,15 @@
 
     def load_model(self, path: str) -> None:
         """
         Load a keras model from file
 
         :param path: path to saved model
         """
-        self.keras_data = tf.keras.models.load_model(path)
+        self.keras_data = tf.keras.models.load_model(path)  # pylint: disable=no-member
 
     def predict(self, image: np.ndarray) -> dict:
         raise NotImplementedError
 
 
 class SoftmaxModel(KerasModel):
     """
```

### Comparing `aigarmic-1.0.0/src/aigarmic/model_performance.py` & `aigarmic-1.0.1/src/aigarmic/model_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                         trained_x=args.trained_x,
                         trained_y=args.trained_y,
                         key=['No growth', 'Growth'])
 
     results = []
     for i, paths in images.items():
         for path in paths:
-            image = cv2.imread(path)
+            image = cv2.imread(path)  # pylint: disable=no-member
             p = model.predict(image)
             p['true_class'] = int(i)
             results.append(p)
 
     color_end = '\033[0m'
     color_red = '\033[91m'
     color_green = '\033[92m'
```

### Comparing `aigarmic-1.0.0/src/aigarmic/plate.py` & `aigarmic-1.0.1/src/aigarmic/plate.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.predictions_matrix = None
         self.image_matrix = None
         self.image = None
         self.model_image_x = None
         self.model_image_y = None
         
         if self.image_path: 
-            self.image = cv2.imread(self.image_path)
+            self.image = cv2.imread(self.image_path)  # pylint: disable=no-member
             self.image_matrix = split_by_grid(self.image, self.n_row, visualise_contours=visualise_contours,
                                               plate_name=self.drug + '_' + str(self.concentration))
 
     def add_growth_code_matrix(self, growth_code_matrix: list[list[int]]) -> None:
         if not self.valid_growth_code_matrix(growth_code_matrix):
             raise ValueError("Invalid growth code matrix, please provide a 2D growth coe matrix (list), values"
                              "must be integers, and cannot be negative")
@@ -331,18 +331,18 @@
             image, stamp = self.get_colony_image(image_index)
             i, j = image_index
             growth = self.growth_matrix[i][j]
             accuracy = self.accuracy_matrix[i][j]
             print()
             print(f"This image ({self.drug + str(self.concentration)} position {i} {j}) was labelled as {growth} "
                   f"with an accuracy of {accuracy * 100:.2f}")
-            cv2.imshow(self.drug + str(self.concentration) + f" position {i} {j}", image)
+            cv2.imshow(self.drug + str(self.concentration) + f" position {i} {j}", image)  # pylint: disable=no-member
             print("Press enter to continue, or enter new classification: ")
             while True: 
-                input_key = cv2.waitKey()
+                input_key = cv2.waitKey()  # pylint: disable=no-member
                 if input_key not in codes:
                     print("Input not recognised, please try again..")
                     continue
                 if input_key in stop_codes or input_key in skip_codes:
                     break
                 try:
                     _ = self.get_key()[codes[input_key]]
@@ -376,15 +376,15 @@
                     os.mkdir(save_dir)
                 class_dir = os.path.join(save_dir, str(input_code))
                 if not os.path.exists(class_dir):
                     print(f"Creating class subdirectory: {class_dir}")
                     os.mkdir(class_dir)
                 save_path = os.path.join(class_dir, stamp + ".jpg")
                 print(f"Saving image to: {save_path}")
-                cv2.imwrite(save_path, image)
+                cv2.imwrite(save_path, image)  # pylint: disable=no-member
         return changed_log
 
     def convert_growth_codes(self, key: list[str]) -> list[list[str]]:
         """
         Convert growth codes to human-readable format using key
         E.g., [0, 1, 2] -> ["No growth", "Poor growth", "Good growth"]
         Sets self.growth_matrix
@@ -445,15 +445,15 @@
             self.key = key
         else:
             _list_of_keys = []
             try:
                 _list_of_keys = [i.get_key() for i in plates_list]
                 self.key = _list_of_keys[0]
             except LookupError:
-                warn(f"No key provided to PlateSet")
+                warn("No key provided to PlateSet")
             if not all(i == _list_of_keys[0] for i in _list_of_keys):
                 raise ValueError("Plates supplied to PlateSet have different growth keys")
             if not _list_of_keys:
                 self.key = None
 
         drug_names = [i.drug for i in plates_list]
         if len(set(drug_names)) > 1:
```

### Comparing `aigarmic-1.0.0/src/aigarmic/process_plate_image.py` & `aigarmic-1.0.1/src/aigarmic/process_plate_image.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     :param end: ending threshold value
     :param by: threshold increment value
     :param look_for: target sub-images
     :param area_lower_bound: minimum area for a contour to be considered
     :return: tuple of contours and threshold value
     """
     for i in range(start, end, by):
-        ret, thresh = cv2.threshold(image, i, 255, cv2.THRESH_BINARY_INV)
+        _, thresh = cv2.threshold(image, i, 255, cv2.THRESH_BINARY_INV)  # pylint: disable=no-member
 
         # Find contours and filter using area
-        _contours = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
+        _contours = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)  # pylint: disable=no-member
         _contours = _contours[0] if len(_contours) == 2 else _contours[1]
         grid_contours = []
         for c in _contours:
-            area = cv2.contourArea(c)
+            area = cv2.contourArea(c)  # pylint: disable=no-member
             if area > area_lower_bound:
                 grid_contours.append(c)
 
         # sort contours and remove biggest (outer) grid square
-        grid_contours = sorted(grid_contours, key=cv2.contourArea)
+        grid_contours = sorted(grid_contours, key=cv2.contourArea)  # pylint: disable=no-member
         grid_contours = grid_contours[:-1]
 
         # If we find the target boxes, return contours and threshold
         if len(grid_contours) == look_for:
             return grid_contours, i
     return None
 
@@ -60,23 +60,23 @@
     :param n_rows: number of rows in the grid (columns will be inferred automatically)
     :param visualise_contours: if True, display the contours found (useful for validation)
     :param plate_name: name of plate to display in visualisation (useful for validation)
     :return: matrix of sub-images
     """
     if visualise_contours and not plate_name:
         raise ValueError("Pass plate name to split_by_grid if using visualise_contours")
-    blur = cv2.GaussianBlur(image, (25, 25), 0)
-    gray = cv2.cvtColor(blur, cv2.COLOR_BGR2GRAY)
-    grid_contours, threshold_value = find_threshold_value(gray)
+    blur = cv2.GaussianBlur(image, (25, 25), 0)  # pylint: disable=no-member
+    gray = cv2.cvtColor(blur, cv2.COLOR_BGR2GRAY)  # pylint: disable=no-member
+    grid_contours, _ = find_threshold_value(gray)
 
     if visualise_contours:
         _image = image
-        cv2.drawContours(_image, grid_contours, -1, (0, 255, 0), 10)
-        cv2.imshow(plate_name, _image)
-        cv2.waitKey()
+        cv2.drawContours(_image, grid_contours, -1, (0, 255, 0), 10)  # pylint: disable=no-member
+        cv2.imshow(plate_name, _image)  # pylint: disable=no-member
+        cv2.waitKey()  # pylint: disable=no-member
 
     if not grid_contours:
         raise ValueError("Unable to find contours threshold that returns correct number of colony images")
 
     # Sort contours, starting left to right
     (grid_contours, _) = contours.sort_contours(grid_contours, method="left-to-right")
     sorted_grid = []
@@ -91,12 +91,12 @@
             col = []
 
     out_matrix = [[empty(shape=1) for _ in range(len(sorted_grid))] for _ in range(n_rows)]
 
     # Iterate through each box
     for j, col in enumerate(sorted_grid):
         for i, c in enumerate(col):
-            x, y, w, h = cv2.boundingRect(c)
+            x, y, w, h = cv2.boundingRect(c)  # pylint: disable=no-member
             cropped_image = image[y:y + h, x:x + w]
             out_matrix[i][j] = cropped_image
 
     return out_matrix
```

### Comparing `aigarmic-1.0.0/src/aigarmic/rename_images.py` & `aigarmic-1.0.1/src/aigarmic/rename_images.py`

 * *Files identical despite different names*

### Comparing `aigarmic-1.0.0/src/aigarmic/train.py` & `aigarmic-1.0.1/src/aigarmic/train.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 """
 Functions and classes that allow for training neural network models for colony image classification.
 """
 
 from aigarmic.file_handlers import create_dataset_from_directory
 import tensorflow as tf
-from tensorflow.keras.models import Sequential
-from tensorflow.keras import layers
-from tensorflow.keras.utils import image_dataset_from_directory
-from tensorflow.keras.initializers import Constant
+from tensorflow.keras.models import Sequential  # pylint: disable=import-error, no-name-in-module
+from tensorflow.keras import layers  # pylint: disable=import-error, no-name-in-module
+from tensorflow.keras.utils import image_dataset_from_directory  # pylint: disable=import-error, no-name-in-module
+from tensorflow.keras.initializers import Constant  # pylint: disable=import-error, no-name-in-module
 import keras.callbacks
 from sklearn.utils import class_weight
-from tensorflow.keras import initializers
+from tensorflow.keras import initializers  # pylint: disable=import-error, no-name-in-module
 from pathlib import Path
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 def train_binary(annotations_path,
                  model_design: Sequential,
@@ -68,28 +68,29 @@
                                                 image_size=(image_height, image_width),
                                                 batch_size=batch_size,
                                                 label_mode="binary")
 
     full_dataset_unbatched = tuple(full_dataset.unbatch())
     labels = [0, 0]
     for (_, label) in full_dataset_unbatched:
-        labels[int(label.numpy())] += 1
+        labels[int(label.numpy()[0])] += 1
     neg = labels[0]
     pos = labels[1]
     initial_bias = np.log([pos / neg])
     initial_bias = Constant(initial_bias)
 
     weight_0 = (1 / neg) * ((neg + pos) / 2)
     weight_1 = (1 / pos) * ((neg + pos) / 2)
     class_weights = {0: weight_0, 1: weight_1}
 
     model_design.add(layers.Dense(1, activation='sigmoid',
                                   bias_initializer=initial_bias))
     with tf.device('/device:GPU:0'):
-        model_design.compile(optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=learning_rate),
+        lr = learning_rate
+        model_design.compile(optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=lr),  # pylint: disable=no-member
                              loss='binary_crossentropy',
                              metrics=['accuracy'])
 
     val_callback = ValidationThresholdCallback(threshold=stop_training_threshold)
     history = model_design.fit(
         train_dataset,
         validation_data=val_dataset,
@@ -197,24 +198,24 @@
     plt.plot(epochs_range, loss, label='Training Loss')
     plt.plot(epochs_range, val_loss, label='Validation Loss')
     plt.legend(loc='upper right')
     plt.title('Training and Validation Loss')
     plt.show()
 
 
-class ValidationThresholdCallback(tf.keras.callbacks.Callback):
+class ValidationThresholdCallback(tf.keras.callbacks.Callback):  # pylint: disable=no-member
     def __init__(self, threshold):
         """
         Stop training if validation accuracy is above threshold
 
         :param threshold: Threshold to stop training
         """
         super().__init__()
         self.threshold = threshold
 
-    def on_epoch_end(self, epoch, logs=None) -> None:
+    def on_epoch_end(self, epoch, logs=None) -> None:  # pylint: disable=unused-argument
         """
         Determines whether to stop training based on validation accuracy
         """
         val_acc = logs["val_accuracy"]
         if val_acc >= self.threshold:
             self.model.stop_training = True
```

### Comparing `aigarmic-1.0.0/src/aigarmic/train_modular.py` & `aigarmic-1.0.1/src/aigarmic/train_modular.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import cv2  # pylint: disable=import-error
 import argparse
 import pathlib
 import warnings
 
 
 def train_modular_parser():
-    parser = argparse.ArgumentParser("""
+    parser = argparse.ArgumentParser(description="""
         This script loads images from annotations directory and trains ML to classify colony growth.
         """)
     parser.add_argument("annotations", type=str,
                         help="Directory containing annotated images")
     parser.add_argument("-v", "--visualise", action="store_true",
                         help="Generate visualisations for model diagnostics")
     parser.add_argument("-s", "--save", type=str,
@@ -103,16 +103,16 @@
         if args.visualise:
             for i in annotation_log:
                 if i["predicted_class"] != i["true_class"]:
                     print(
                         f"This image was misclassified as {i['predicted_class']} "
                         f"with prediction of {i['prediction']} "
                         f"(should have been {i['true_class']})")
-                    cv2.imshow(str(i['path']), i['image'])
-                    cv2.waitKey()
+                    cv2.imshow(str(i['path']), i['image'])  # pylint: disable=no-member
+                    cv2.waitKey()  # pylint: disable=no-member
                 else:
                     print(f"Correct classification with prediction {i['prediction']} (class {i['true_class']})")
 
     if args.visualise:
         visualise_training(history)
```

