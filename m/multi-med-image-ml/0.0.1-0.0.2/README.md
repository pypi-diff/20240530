# Comparing `tmp/multi_med_image_ml-0.0.1.tar.gz` & `tmp/multi_med_image_ml-0.0.2.tar.gz`

## Comparing `multi_med_image_ml-0.0.1.tar` & `multi_med_image_ml-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/logo.png
--rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/model_diagram.png
--rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/regress_figure.png
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/example_train.py
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/base_options.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/test_options.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/train_options.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10687 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    45669 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11528 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/weights.json
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/logo.png
+-rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/model_diagram.png
+-rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/regress_figure.png
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/example_train.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/train_options.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10799 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17623 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/weights.json
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/README.md
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.1/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.1/.images/logo.png` & `multi_med_image_ml-0.0.2/.images/logo.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.1/.images/model_diagram.png` & `multi_med_image_ml-0.0.2/.images/model_diagram.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.1/.images/regress_figure.png` & `multi_med_image_ml-0.0.2/.images/regress_figure.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.1/example/options/test_options.py` & `multi_med_image_ml-0.0.2/example/options/test_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 	It also includes shared options defined in BaseOptions.
 	"""
 
 	def initialize(self, parser):
 		parser = BaseOptions.initialize(self, parser)  # define shared options
 		parser.add_argument('--val_ranges',default={'InstitutionNameSimplified':['BWH','OTHER']},help="What stuff to load into the training set")
 		#parser.add_argument('--val_ranges',default={'AlzStage':['CONTROL','AD'],'InstitutionNameSimplified':['BWH','OTHERS'],'MRModality':['T1'],'Angle':['AX']},help="What stuff to load into the test set")
-		parser.add_argument('--results_dir', type=str, default='./results/', help='saves results here.')
 		parser.add_argument('--aspect_ratio', type=float, default=1.0, help='aspect ratio of result images')
 		parser.add_argument('--phase', type=str, default='test', help='train, val, test, etc')
 		parser.add_argument('--save_net',default=False,action='store_true',help="Saves the full netG_A and netG_B models for loading later")
 		# Dropout and Batchnorm has different behavioir during training and test.
 		parser.add_argument('--eval', action='store_true', help='use eval mode during test time.')
 		parser.add_argument('--num_test', type=int, default=50, help='how many test images to run')
 		# rewrite devalue values
```

### Comparing `multi_med_image_ml-0.0.1/example/options/train_options.py` & `multi_med_image_ml-0.0.2/example/options/train_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,31 @@
 
 	It also includes shared options defined in BaseOptions.
 	"""
 
 	def initialize(self, parser):
 		parser = BaseOptions.initialize(self, parser)
 		# visdom and HTML visualization parameters
-		parser.add_argument('--pretrained_model',type=str,default="", help='Pretrained model to load in')
-		parser.add_argument('--display_freq', type=int, default=400, help='frequency of showing training results on screen')
-		parser.add_argument('--display_ncols', type=int, default=4, help='if positive, display all images in a single visdom web panel with certain number of images per row.')
+		parser.add_argument('--pretrained_model',type=str,default=None, help='Pretrained model to load in')
 		#parser.add_argument('--val_ranges',default={'DiffDem':['None','G30','F01'],'InstitutionNameSimplified':'MGH'},help="What stuff to load into the training set")
 		parser.add_argument('--val_ranges',default={'InstitutionNameSimplified_Date':['MGH_BEFORE_2019','MGH_AFTER_2019']})
 		# network saving and loading parameters
 		parser.add_argument('--save_latest_freq', type=int, default=100, help='frequency of saving the latest results')
 		parser.add_argument('--save_epoch_freq', type=int, default=5, help='frequency of saving checkpoints at the end of epochs')
 		parser.add_argument('--save_by_iter', action='store_true', help='whether saves model by iteration')
 		parser.add_argument('--continue_train', action='store_true', help='continue training: load the latest model')
 		parser.add_argument('--epoch_count', type=int, default=1, help='the starting epoch count, we save the model by <epoch_count>, <epoch_count>+<save_latest_freq>, ...')
 		parser.add_argument('--phase', type=str, default='train', help='train, val, test, etc')
 		# training parameters
-		parser.add_argument('--n_epochs', type=int, default=100, help='number of epochs with the initial learning rate')
-		parser.add_argument('--n_epochs_decay', type=int, default=100, help='number of epochs to linearly decay learning rate to zero')
+		parser.add_argument('--epochs', type=int, default=100, help='number of epochs with the initial learning rate')
+		#parser.add_argument('--epochs_decay', type=int, default=100, help='number of epochs to linearly decay learning rate to zero')
 		parser.add_argument('--beta1', type=float, default=0.9, help='momentum term of adam')
 		parser.add_argument('--lr', type=float, default=1e-5, help='initial learning rate for adam')
-		parser.add_argument('--lr_policy', type=str, default='linear', help='learning rate policy. [linear | step | plateau | cosine]')
-		parser.add_argument('--lr_decay_iters', type=int, default=50, help='multiply by a gamma every lr_decay_iters iterations')
-		parser.add_argument('--blur_b',action='store_true',default=False,help='Blurs the B data')
-		parser.add_argument('--max_iters',type=int,default=-1)
+		#parser.add_argument('--lr_policy', type=str, default='linear', help='learning rate policy. [linear | step | plateau | cosine]')
+		#parser.add_argument('--lr_decay_iters', type=int, default=50, help='multiply by a gamma every lr_decay_iters iterations')
+		#parser.add_argument('--max_iters',type=int,default=-1)
 		parser.add_argument('--use_mix',action='store_true',default=False,help='Uses an alternate loss function for the reconstruction')
 		parser.add_argument('--augment',action='store_true',default=True,help='Augments 3D images')
-		parser.add_argument('--total_load',type=int,default=30*45000,help='Total number of data to load into main memory')
+		#parser.add_argument('--total_load',type=int,default=30*45000,help='Total number of data to load into main memory')
 		parser.add_argument('--no_regress',action='store_true',default=False)
 		self.isTrain = True
 		return parser
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 	"""
 	def __init__(self,
 					all_vars = None,
 					filename=None,
 					labels=[],
 					confounds=[],
 					dim=None,
-					cdim=None):
+					cdim=None,
+					path_func = path_func_default):
+		self.path_func = path_func
+		check_path_func(self.path_func)
 
 		self.filename = filename
 		self.dim = dim
 		self.labels = [] if labels is None else labels
 		self.confounds = [] if confounds is None else confounds
 		if all_vars is not None:
 			self.all_vars = all_vars
@@ -203,14 +206,15 @@
 		d = self._get_val(fkey,["ExamEndDTS","Acquisition Date"])
 		return self.parse_date(d)
 	def get_birth_date(self,fkey):
 		d = self._get_val(fkey,["BirthDTS"])
 		return self.parse_date(d)
 	
 	def loc_val(self,fkey,c):
+		fkey = self.path_func(fkey)
 		try:
 			return self.all_vars.loc[fkey,c]
 		except KeyError:
 			nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii.gz")
 			
 			if not os.path.isfile(nifti_file):
 				nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii")
@@ -230,29 +234,31 @@
 			if not (os.path.isfile(json_file)):
 				json_file = os.path.join(
 					os.path.dirname(nifti_file),
 					"metadata.json")
 				if not os.path.isfile(json_file):
 					return
 		npy_file = get_dim_str(nifti_file,self.dim)
-		#if not os.path.isfile(npy_file):
-		#	return
+		
 		if npy_file not in self.jdict and npy_file not in self.all_vars.index:
 			with open(json_file,'r') as fileobj:
 				json_dict = json.load(fileobj)
 			json_dict["fkey"] = npy_file
 			json_dict["filename"] = npy_file
 			for item in json_dict:
 				if isinstance(json_dict[item],list):
 					json_dict[item] = "_".join(
 							[str(_) for _ in sorted(json_dict[item])]
 						)
 			self.columns = self.columns.union(set(json_dict))
 			self.jdict.append(json_dict)
 			assert(len(self.jdict) > 0)
+	def get_file_list(self):
+		return [self.path_func(str(_),reverse=True) \
+			for _ in self.all_vars.index]
 	def out_dataframe(self,fkey_ass = None):
 		if len(self.jdict) > 0:
 			out = pd.DataFrame(self.jdict,columns = list(self.columns))
 			out.set_index("fkey",inplace=True)
 			if len(self.all_vars) > 0:
 				self.all_vars = pd.concat([self.all_vars,out],
 						ignore_index=False,
@@ -265,14 +271,22 @@
 			if fkey_ass is not None: assert(fkey_ass in self.all_vars.index)
 			self.all_vars.drop_duplicates(inplace=True)
 			if fkey_ass is not None: assert(fkey_ass in self.all_vars.index)
 			self.all_vars.to_pickle(self.filename)
 			if fkey_ass is not None: assert(fkey_ass in self.all_vars.index)
 			self.jdict = []
 	def stack_list_by_label(self,filename_list,label):
-		assert(label in self.labels)
-		lnum = self.labels.index(label)
-		lencodes = [self.get_label_encode(f)[lnum] for f in filename_list]
+		if label in self.labels:
+			sel_list = self.labels
+		elif label in self.confounds:
+			sel_list = self.confounds
+		else:
+			raise Exception("%s not in labels or confounds")
+		lnum = sel_list.index(label)
+		if label in self.labels:
+			lencodes = [self.get_label_encode(f)[lnum] for f in filename_list]
+		elif label in self.confounds:
+			lencodes = [self.get_confound_encode(f)[lnum] for f in filename_list]
 		filename_list_stack = [[] for _ in range(len(np.unique(lencodes)))]
 		for filename,l in zip(filename_list,lencodes):
 			filename_list_stack[l].append(filename)
 		return filename_list_stack
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,63 +12,70 @@
 import shutil
 import nibabel as nb
 from nibabel.filebasedimages import *
 
 from Records import BatchRecord,ImageRecord
 from DataBaseWrapper import DataBaseWrapper
 
+# Translates a filename to a key and back, for storing files as keys in the
+# pandas dataframe. By default, the keys are the full filepaths. This function
+# may need to be changed when switching to different systems
+def path_func_default(fkey,reverse=False):
+	return fkey
+
 class MedImageLoader():
 	def __init__(self,*image_folders,
 			pandas_cache = '../pandas/',
 			cache = True,
-			path_func = None,
+			path_func = path_func_default,
 			batch_by_pid=True,
-			return_as_patient_record=False,
 			file_record_name=None,
-			n_out_y=None,
-			forcealt=True,
 			all_vars = None,
-			batch_size = 16,
+			batch_size = 14,
 			dim = (96,96,96),
 			get_encoded = False,
 			static_inputs = None,
 			confounds = [],
 			match_confounds = [],
 			label = [],
 			group_by = None,
 			augment = True,
 			val_ranges = {},
-			dtype="numpy",
-			Y_dim = (16,32),
+			dtype="torch",
+			Y_dim = (1,32),
 			C_dim = (16,32),
 			return_obj = False,
-			channels_first = True):
+			channels_first = True,
+			recycle=True):
 		self.channels_first = channels_first
 		self.image_folders = image_folders
 		self.augment = augment
 		self.dim=dim
 		self.dtype=dtype
 		self.cache = cache
 		self.pandas_cache = pandas_cache
 		self.val_ranges = val_ranges
 		self.get_encoded = get_encoded
 		self.batch_by_pid = group_by is not None
-		self.return_as_patient_record = return_as_patient_record
 		self.file_list_dict = {}
 		self.static_inputs = static_inputs
 		self.label = label
 		self.confounds = confounds
-		self.path_func = path_func
 		self.group_by = group_by
-		self.n_out_y = n_out_y # Set dimension for Y
-		self.forcealt = forcealt
 		self.Y_dim = Y_dim
 		self.C_dim = C_dim
 		self.mode = None
 		
+		# If set to true, restacks images every time via the data 
+		# matching function. Best for very large and imbalanced datasets
+		self.recycle=recycle
+		
+		self.path_func = path_func
+		check_path_func(self.path_func)
+
 		# Stores images so that they aren't repeated in different stacks
 		self.image_dict = {}
 		# If true, this uses one match confound at a time and cycles through
 		# them
 		self.zero_data_list = []
 		self.match_confounds = match_confounds
 		if self.batch_by_pid:
@@ -88,50 +95,46 @@
 				self.pandas_cache,
 				"all_vars_%s.pkl" % get_dim_str(dim=self.dim))
 		
 		self.all_vars = DataBaseWrapper(
 					filename=self.all_vars_file,
 					labels=self.label,
 					confounds=self.confounds,
-					dim=self.dim)
+					dim=self.dim,
+					path_func=self.path_func)
 		if not self.pickle_input():
 			self.build_pandas_database()
 		self.all_vars.build_metadata()
 		
 		# Determine which mode the scheduler is in
 		if (self.label is not None and len(self.label) > 0):
 			self.mode = "match"
 		else:
 			self.mode = "iterate"
 		
-		#if self.Y_dim is None:
-		#	self.Y_dim = (len(self.labels)
 		
 		# For outputting the records of files that were read in
 		self.file_record_name = file_record_name 
 		if self.file_record_name is not None:
 			self.file_record = {}
 			fd = os.path.join(wd,'json','dataloader_records')
 			if not os.path.isdir(fd): os.makedirs(fd)
 			self.file_record_output = os.path.join(fd,file_record_name)
-		
-		if self.path_func is None:
-			self.path_func = lambda k: k
+
 		self.uniques = None
 		self.n_buckets = 3
 		self.rmatch_confounds = self.confounds
 	
 		# Regular stack variables
 		self.file_list_dict = {}
 	
 		# Switch stack variables
 		self.file_list_dict_hidden = {}
 		self.match_confounds_hidden = []
 		self.mode_hidden = "iterate"
-		self.forcealt_hidden = False
 		if self.return_labels():
 			for l in self.label:
 				if l not in self.val_ranges:
 					self.match_confounds_hidden.append(l)
 		self.index = 0
 		self.load_image_stack()
 	# Builds up the entire cache in one go — may take a while
@@ -164,18 +167,18 @@
 		if len(self.label) == 0: tl = "Folder"
 		else: tl = self.label[0]
 		if tl not in self.file_list_dict:
 			self.file_list_dict[tl] = []
 		return tl
 	def get_file_list(self):
 		if self.pickle_input() and self.tl() == "Folder":
-			return [[str(_) for _ in self.all_vars.all_vars.index]]
+			return [[str(_) for _ in self.all_vars.get_file_list()]]
 		if self.mode == "iterate":
 			if self.pickle_input():
-				fname_list = [str(_) for _ in self.all_vars.all_vars.index]
+				fname_list = [str(_) for _ in self.all_vars.get_file_list()]
 				return self.all_vars.stack_list_by_label(fname_list,self.tl())
 			else:
 				all_filename_lists = []
 				duplicate_test = set()
 				for img in self.image_folders:
 					flist = get_file_list(img)#,db_builder=self.all_vars)
 					flist_set = set(flist)
@@ -273,15 +276,14 @@
 			self.label = self.label[1:] + [self.label[0]]
 	def switch_stack(self):
 		self.label,self.rmatch_confounds = self.rmatch_confounds,self.label
 		self.file_list_dict,self.file_list_dict_hidden = \
 			self.file_list_dict_hidden,self.file_list_dict
 		self.match_confounds,self.match_confounds_hidden = \
 			self.match_confounds_hidden,self.match_confounds
-		self.forcealt,self.forcealt_hidden = self.forcealt_hidden,self.forcealt
 		self.mode,self.mode_hidden = self.mode_hidden,self.mode
 	def __next__(self):
 		if len(self) == 0: self.load_image_stack()
 		if self.index > len(self):
 			self.all_vars.out_dataframe()
 			self.index = 0
 			self.rotate_labels()
@@ -294,15 +296,15 @@
 			if len(self.file_list_dict[self.tl()][b]) == 0: continue
 			for j in range(len(self.file_list_dict[self.tl()][b])):
 				im = self.file_list_dict[self.tl()][b].pop()
 				self.file_list_dict[self.tl()][b] = [im] + \
 					self.file_list_dict[self.tl()][b]
 				try:
 					if self.cache: assert self.all_vars is not None
-					img = im.get_image()
+					img = im.get_image(augment=self.augment)
 					temp.append(im)
 					self.index += 1
 					break
 				except ImageFileError:
 					self.file_list_dict[self.tl()][b] = \
 						self.file_list_dict[self.tl()][b][1:]
 					continue
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTester.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,28 +134,28 @@
 					len(self.x_files_read),self.name))
 			else:
 				print("%d: Class: %.6f, Dud: %.6f, Reg: %.6f (%d, %d) | %s" % \
 					(i,float(loss_Y), float(loss_C_dud),
 					float(loss_regressor),len(self.pids_read),
 					len(self.x_files_read),self.name))
 
-		if self.index % self.batch_size == 0:
+		if self.index % self.batch_size == 0 and self.index != 0:
 			if self.one_step:
 				self.optimizer.step()
 				self.optimizer.zero_grad()
 				self.model.classifier_freeze()
 				if dataloader is not None:
 					dataloader.switch_stack()
 			else:
 				self.optimizer_reg.step()
 				self.optimizer_reg.zero_step()
 				self.model.regressor_freeze()
 				if dataloader is not None:
 					dataloader.switch_stack()
-		
+			self.one_step = not self.one_step
 		if self.index % self.save_latest_freq == 0 and self.index != 0:
 			if self.checkpoint_dir is not None:
 				torch.save(
 					self.model.state_dict(),
 					self.model_file
 				)
 			if self.loss_image_dir is not None:
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/Records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import functools,os
 import numpy as np
 from monai.transforms import *
 from utils import *
 
+generate_transforms = Compose([
+		RandAffine(prob=0.5, translate_range=10), 
+		RandRotate(prob=0.5, range_x=10.0),
+		RandGaussianNoise(prob=0.5),
+		RandBiasField(prob=0.5)])
+#,
+#		RandSmoothDeform(spatial_size=(96,96,96),rand_size=(96,96,96))
+#])
+
 @functools.total_ordering
 class ImageRecord():
 	def __init__(self,
 		filename,
 		all_vars = None,
 		dim=(96,96,96),
 		dtype="torch",
@@ -50,15 +59,14 @@
 		self.loaded = False
 		if self.all_vars is not None:
 			if self.fkey in self.all_vars.all_vars:
 				self.load_extra_info()
 		
 		self.cache = cache
 		self.cached_record = None
-	
 	def get_exam_date(self):
 		if not self.loaded:
 			self.load_extra_info()
 		return self.exam_date
 	def get_birth_date(self):
 		if not self.loaded:
 			self.load_extra_info()
@@ -73,15 +81,17 @@
 		self.exam_date = self.all_vars.get_exam_date(self.fkey)
 		self.group_by = self.all_vars.get_ID(self.fkey)
 		self.loaded = True
 	def get_static_inputs(self):
 		if self.static_input_res is None:
 			self.static_input_res = []
 			for key in self.static_inputs:
-				static_inputs.append(self.all_vars.all_vars.loc[self.fkey,key])
+				static_inputs.append(
+					self.all_vars.loc_val(self.fkey,key)
+				)
 		return self.static_input_res
 	def _is_valid_operand(self, other):
 		return hasattr(other, "exam_date") and hasattr(other,"group_by")
 	def __eq__(self, other):
 		if not self._is_valid_operand(other):
 			return NotImplemented
 		return (self.exam_date == other.exam_date)
@@ -170,19 +180,21 @@
 		self.image = resize_np(self.image,self.dim)
 		if self.cache and not os.path.isfile(self.cached_record):
 			np.save(self.cached_record,self.image)
 		if self.all_vars is not None:
 			self.all_vars.add_json(nifti_file=self.filename)
 		if self.dtype == "torch":
 			self.image = torch.tensor(self.image)
-	def get_image(self):
+	def get_image(self,augment=False):
 		if self.image is None:
 			self.read_image()
 		self.load_extra_info()
-		return self.image
+		if augment and self.dtype == "torch":
+			return generate_transforms(self.image)
+		else: return self.image
 	def _get_Y(self):
 		"""Returns label"""
 		if self.y_nums is not None:
 			return self.y_nums
 		self.y_nums = self.all_vars.get_label_encode(self.fkey)
 		return self.y_nums
 	def _get_C(self):
@@ -267,21 +279,21 @@
 		self.X = torch.unsqueeze(self.X,1).float().cuda(device)
 		
 		self.C = torch.tensor(self.C).float().cuda(device)
 		self.C_dud = torch.tensor(self.C_dud).float().cuda(device)
 	
 	def name(self):
 		return 'BatchRecord'
-	def _get(self,callback):
+	def _get(self,callback,augment=False):
 		Xs = []
 		no_arr = False
 		for im in (self.image_records if (callback != "Y" and not self.batch_by_pid)\
 			else [self.image_records[-1]]):
 			if callback == "X":
-				X = im.get_image()
+				X = im.get_image(augment=augment)
 				if self.dtype == "torch":
 					assert(len(X.size()) == 3)
 					if self.channels_first:
 						X = torch.unsqueeze(X,0)
 					else:
 						X = torch.unsqueeze(X,-1)
 				elif self.dtype == "numpy":
@@ -323,30 +335,22 @@
 			Xs = torch.concatenate(Xs,0)
 			return Xs.float()
 		elif self.dtype == "numpy":
 			Xs = np.concatenate(Xs,axis=0)
 			return Xs #.astype(np.float32)
 		else:
 			raise Exception("Invalid dtype: %s" % self.dtype)
-	def get_image(self):
-		return self._get("X")
+	def get_image(self,augment=False):
+		return self._get("X",augment=augment)
 	def get_Y(self):
 		return self._get("Y")
 	def get_C(self):
 		return self._get("C")
 	def get_C_dud(self):
 		return self._get("C_dud")
 	def get_exam_dates(self):
 		return self._get("exam_dates")
 	def get_birth_dates(self):
 		return self._get("birth_dates")
 	def get_static_inputs(self):
 		return self._get("static_inputs")
 
-generate_transforms = Compose([
-		RandAffine(prob=0.5, translate_range=10), 
-		RandRotate(prob=0.5, range_x=10.0),
-		RandGaussianNoise(prob=0.5),
-		RandBiasField(prob=0.5),
-		RandSmoothDeform(spatial_size=(96,96,96),rand_size=(96,96,96))
-])
-
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,47 +64,14 @@
 	def __init__(self, *target_shape):
 		super().__init__()
 		self.target_shape = target_shape
 	
 	def forward(self, x):
 		return x.view(*self.target_shape)
 
-class NeuralNetwork(nn.Module):
-    def __init__(self,inp,outp):
-        super().__init__()
-        self.flatten = nn.Flatten()
-        self.linear_relu_stack = nn.Sequential(
-            nn.Linear(inp, 4096),
-            nn.LeakyReLU(),
-			nn.BatchNorm1d(4096),
-            nn.Linear(4096, 2048),
-            nn.LeakyReLU(),
-			nn.BatchNorm1d(2048),
-			nn.Dropout(0.5),
-			nn.Linear(2048, 1024),
-			nn.LeakyReLU(),
-			nn.BatchNorm1d(1024),
-			nn.Linear(1024, 512),
-			nn.LeakyReLU(),
-			nn.BatchNorm1d(512),
-			nn.Linear(512, 256),
-			nn.LeakyReLU(),
-			nn.BatchNorm1d(256),
-            nn.Linear(256, 64),
-			nn.LeakyReLU(),
-			nn.BatchNorm1d(64),
-			nn.Dropout(0.5),
-            nn.Linear(64, outp),
-			nn.Sigmoid(),
-        )
-    def forward(self, x):
-        x = self.flatten(x)
-        logits = self.linear_relu_stack(x)
-        return logits
-
 class Encoder(nn.Module):
 	def __init__(self,latent_dim=512):
 		super(Encoder,self).__init__()
 		nchan=1
 		base_feat = 64
 		self.encoder = nn.Sequential(
 			nn.Conv3d(in_channels = nchan, out_channels = base_feat, stride=2,
@@ -259,26 +226,26 @@
 	def parameters(self):
 		return self.classifier.parameters()
 	def forward(self,x):
 		return self.classifier(x)
 
 class MultiInputModule(nn.Module):
 	def __init__(self,
-				Y_dim = (16,32), # Number of labels, Number of choices
-				C_dim = (16,32), # Number of labels, Number of choices
-				n_dyn_inputs = 14,
-				n_stat_inputs = 2,
-				use_attn = False,
-				encode_age = False,
-				variational = False,
-				zero_input = False,
-				remove_uncertain = False,
+				Y_dim: tuple = (1,32), # Number of labels, Number of choices
+				C_dim: tuple = (16,32), # Number of labels, Number of choices
+				n_dyn_inputs: int = 14,
+				n_stat_inputs: int = 2,
+				use_attn: bool = False,
+				encode_age: bool = False,
+				variational: bool = False, # Makes it a variational encoder
+				zero_input: bool = False, # Repeats input into classifier or makes it zeros
+				remove_uncertain: bool = False,
 				device = torch.device('cpu'),
-				latent_dim = 128,
-				weights = None):
+				latent_dim: int = 128,
+				weights: bool = None):
 		super(MultiInputModule,self).__init__()
 		
 		# Model Parameters
 		self.latent_dim = latent_dim
 		
 		# Number of non-image, patient-specific demographic inputs. Sex and 
 		# ethnicity are two that can be applied.
@@ -286,19 +253,27 @@
 		
 		# Max number of images that can be passed in
 		self.n_dyn_inputs = n_dyn_inputs
 		
 		# Total number of inputs, which is used for the classifier model
 		self.n_inputs = self.n_stat_inputs + self.n_dyn_inputs
 		
-		self.Y_dim = (1,Y_dim) if isinstance(Y_dim,int) else Y_dim
-		num_heads = self.n_inputs
+		if (not isinstance(Y_dim,tuple)) or (len(Y_dim) != 2) or\
+			(not isinstance(C_dim,tuple)) or (len(C_dim) != 2):
+			raise Exception("""
+				Y_dim and C_dim must be tuples.
+				(<# labels>,<max # choices>)
+				One label with two choices: (1,2)
+			""")
+		self.Y_dim = Y_dim
 		self.C_dim = C_dim
 		self.zero_input = zero_input
 		self.remove_uncertain = remove_uncertain
+
+		# Under development
 		if self.remove_uncertain:
 			self.record_training_sample = False
 			self.num_training_samples = 300
 			self.training_sample = torch.zeros(
 				(
 					self.latent_dim,
 					self.num_training_samples
@@ -347,15 +322,15 @@
 			self.regressor = Regressor(self.latent_dim,
 				n_confounds=self.C_dim[0],
 				n_choices=self.C_dim[1],
 				device=device)
 		else: self.regressor = None
 		
 		if weights is not None:
-			if self.C_dim ! (16,32) or self.Y_dim != (16,32):
+			if self.C_dim != (16,32) or self.Y_dim != (1,32):
 				warnings.warn(
 					"Pretrained models may not function if defaults are altered"
 					)
 			if os.path.isfile(weights) and \
 				os.path.splitext(weights)[1] == ".pt":
 				self.load_state_dict(torch.load(weights))
 			else:
@@ -519,20 +494,15 @@
 					)
 			if self.training:
 				for i,e in enumerate(static_input):
 					self.static_record[i].add(e)
 			else:
 				for i,e in enumerate(self.static_record):
 					if static_input[i] not in e:
-						raise Exception(
-							"""
-								Input %s not a previous demographic
-								input (previous inputs were %s)
-							""" % (static_input[i],str(e))
-						)
+						raise Exception("Input %s not a previous demographic input (previous inputs were %s)" % (static_input[i],str(e)))
 			x_ = encode_static_inputs(static_input,d=self.latent_dim)
 			x_ = torch.tensor(x_,device = x.device)
 			x_ = torch.unsqueeze(x_,0)
 			for i in range(x_.shape[0]):
 				if ((not self.static_dropout) or random.choice([True,False]) and self.training) or\
 					(not self.static_dropout):
 					x[:,(-(self.n_stat_inputs) + i):,:] = x_[i,:]
@@ -557,23 +527,14 @@
 							device=x.device,
 							dtype=torch.bool)
 					),
 				axis=1)
 			m = m[:,r,...]
 			x,_ = self.multihead_attn(x,x,x,need_weights=False)#,attn_mask=m)
 
-		#x = self.encoder(x)
-		#x = torch.flatten(x, start_dim=1)
-		#z_mean = self.z_mean(x)
-		#z_log_sigma = self.z_log_sigma(x)
-		#z = z_mean + (z_log_sigma.exp()*self.epsilon.sample(z_mean.shape))
-		#z = nn.functional.sigmoid(z)
-		#y = self.decoder(z)
-		#self.kl = (z_mean**2 + z_log_sigma.exp()**2 - z_log_sigma - 0.5).sum()
-	
 		# Switch batch channel with layer channel prior to running classifier
 		x = torch.unsqueeze(x,-1)
 		x = x.contiguous().view([-1,1,self.latent_dim*self.n_inputs]) # 16*512 -> 1*[16*512]
 		x = self.classifier(x)
 		if use_regression: return x,reg
 		else: return x
 
@@ -594,169 +555,7 @@
 			new_output.append(torch.unsqueeze(output,3))
 			new_hidden.append(torch.unsqueeze(h,3))
 			#print("output.size(): %s" % str(output.size()))
 			#print("h.size(): %s" % str(h.size()))
 		new_output = torch.cat(new_output,dim=3)
 		new_hidden = torch.cat(new_hidden,dim=3)
 		return new_output,new_hidden
-
-class VariationalEncoder(nn.Module):
-	def __init__(self):
-		super(Encoder,self).__init__()
-		nchan=1
-		base_feat = 64
-		latent_dim = 512
-		self.encoder = nn.Sequential(
-			nn.Conv3d(in_channels = nchan, out_channels = base_feat, stride=2, kernel_size=5, padding = 2), #1*96*96*96 -> 64*48*48*48
-			nn.LeakyReLU(),
-			nn.Dropout(0.5),
-			nn.InstanceNorm3d(base_feat),
-			nn.Conv3d(in_channels = base_feat, out_channels = base_feat*2, stride=2, kernel_size = 5,padding=2), #64*48*48*48 -> 128*24*24*24
-			nn.LeakyReLU(),
-			nn.InstanceNorm3d(base_feat*2),
-			nn.Conv3d(in_channels = base_feat*2, out_channels = base_feat*4, stride=2,kernel_size = 3,padding=1), #128*24*24*24 -> 256*12*12*12
-			nn.LeakyReLU(),
-			nn.InstanceNorm3d(base_feat*4),
-			nn.Conv3d(in_channels = base_feat*4, out_channels = base_feat*4, stride=4,kernel_size = 5,padding=2), #256*12*12*12 -> 256*3*3*3
-			nn.LeakyReLU(),
-			nn.InstanceNorm3d(base_feat*4),
-			nn.Conv3d(in_channels = base_feat*4, out_channels = base_feat*32, stride=1,kernel_size = 3,padding=0), #256*3*3*3 -> 2048*1*1*1
-			nn.LeakyReLU(),
-			nn.Dropout(0.5),
-			Reshape([-1,base_feat*32]),
-			nn.Linear(in_features = base_feat*32, out_features = base_feat*16),
-			nn.LeakyReLU(),
-			nn.Linear(in_features = base_feat*16, out_features = latent_dim)
-		)
-	def forward(self, x):
-		self.z_mean = nn.Linear(64, latent_dim)
-		self.z_log_sigma = nn.Linear(64, latent_dim)
-		#self.epsilon = torch.normal(size=(1, latent_dim), mean=0, std=1.0,
-		#	device=self.device)
-		self.epsilon = torch.distributions.Normal(0, 1)
-		self.epsilon.loc = self.epsilon.loc.cuda(device)
-		self.epsilon.scale = self.epsilon.scale.cuda(device)
-		x = self.encoder(x)
-		return x
-
-	def forward(self, x):
-		x = self.encoder(x)
-		x = torch.flatten(x, start_dim=1)
-		z_mean = self.z_mean(x)
-		z_log_sigma = self.z_log_sigma(x)
-		z = z_mean + (z_log_sigma.exp()*self.epsilon.sample(z_mean.shape))
-		z = nn.functional.sigmoid(z)
-		y = self.decoder(z)
-		self.kl = (z_mean**2 + z_log_sigma.exp()**2 - z_log_sigma - 0.5).sum()
-		return y,z, z_mean, z_log_sigma
-
-
-
-class Encoder1D(nn.Module):
-	def __init__(self,input_dim,output_dim,conv=True):
-		super(Encoder1D,self).__init__()
-		base_feat = 1024
-		if conv:
-			self.encoder = nn.Sequential(
-				Reshape([-1,1,1,input_dim]),
-				nn.Conv2d(1,base_feat,kernel_size=(1,input_dim)),
-				nn.LeakyReLU(),
-				Reshape([-1,1,base_feat]),
-				nn.BatchNorm1d(1,affine=True),
-				Reshape([-1,base_feat]),
-				nn.Linear(base_feat,output_dim),
-				
-			)
-		else:
-			self.encoder = nn.Sequential(
-				#nn.Conv2d(in_channels = 1, out_channels = base_feat*4, stride=1, kernel_size=(self.latent_dim,1), padding =0), #1*96*96*96 -> 64*48*48*48
-				#Reshape([-1,self.latent_dim*self.n_inputs]),
-				nn.Linear(input_dim,input_dim//2),
-				nn.LeakyReLU(),
-				nn.BatchNorm1d(input_dim//2,affine=True),
-	
-				nn.Linear(in_features = input_dim//2, out_features = input_dim//4),
-				nn.LeakyReLU(),
-				nn.BatchNorm1d(input_dim//4,affine=True),
-				
-				nn.Linear(in_features = input_dim//4, out_features = input_dim//8),
-				nn.LeakyReLU(),
-				
-				nn.Linear(in_features = input_dim//8, out_features = output_dim),
-			)
-	def forward(self,x):
-		x = self.encoder(x)
-		return x
-
-
-class Decoder1D(nn.Module):
-	def __init__(self,input_dim,output_dim,conv=True):
-		super(Decoder1D, self).__init__()
-		base_feat = 1024
-		if conv:
-			self.decoder = nn.Sequential(
-				nn.Linear(output_dim,base_feat),
-				nn.LeakyReLU(),
-				Reshape([-1,1,base_feat]),
-				nn.BatchNorm1d(1,affine=True),
-				Reshape([-1,base_feat,1]),
-				nn.ConvTranspose1d(base_feat,1,kernel_size=input_dim)
-			)
-		else:
-			self.decoder = nn.Sequential(
-				nn.Linear(in_features = output_dim,out_features = input_dim//8),
-				nn.LeakyReLU(),
-				nn.Linear(in_features = input_dim//8,out_features = input_dim//4),
-				nn.LeakyReLU(),
-				nn.BatchNorm1d(input_dim//4,affine=True),
-				nn.Linear(in_features = input_dim//4,out_features = input_dim//2),
-				nn.LeakyReLU(),
-				nn.Linear(in_features = input_dim//2,out_features = input_dim),
-			)
-	def forward(self,x):
-		x = self.decoder(x)
-		return x
-		
-class VAE(nn.Module):
-	def __init__(self, input_dim,latent_dim=2,device=torch.device('cpu')):
-		super(VAE, self).__init__()
-		self.device = device
-		self.latent_dim = latent_dim
-		self.z_mean = nn.Linear(64, latent_dim)
-		self.z_log_sigma = nn.Linear(64, latent_dim)
-		#self.epsilon = torch.normal(size=(1, latent_dim), mean=0, std=1.0,
-		#	device=self.device)
-		self.epsilon = torch.distributions.Normal(0, 1)
-		self.epsilon.loc = self.epsilon.loc.cuda(device)
-		self.epsilon.scale = self.epsilon.scale.cuda(device)
-		self.encoder = Encoder1D(input_dim,64)
-		self.decoder = Decoder1D(input_dim,latent_dim)
-		
-	#	self.reset_parameters()
-	  
-	def reset_parameters(self):
-		for weight in self.parameters():
-			stdv = 1.0 / math.sqrt(weight.size(0))
-			torch.nn.init.uniform_(weight, -stdv, stdv)
-
-	def forward(self, x):
-		x = self.encoder(x)
-		x = torch.flatten(x, start_dim=1)
-		z_mean = self.z_mean(x)
-		z_log_sigma = self.z_log_sigma(x)
-		z = z_mean + (z_log_sigma.exp()*self.epsilon.sample(z_mean.shape))
-		#z = nn.functional.sigmoid(z)
-		y = self.decoder(z)
-		self.kl = (z_mean**2 + z_log_sigma.exp()**2 - z_log_sigma - 0.5).sum()
-		return y,z, z_mean, z_log_sigma
-
-class AutoEncoder1D(nn.Module):
-	def __init__(self,input_dim,latent_dim=2,device=torch.device('cpu')):
-		super(AutoEncoder1D,self).__init__()
-		
-		self.encoder = Encoder1D(input_dim,latent_dim).cuda(device)
-		self.decoder = Decoder1D(input_dim,latent_dim).cuda(device)
-		
-	def forward(self,x):
-		latent = self.encoder(x)
-		x = self.decoder(latent)
-		return latent,x
```

### Comparing `multi_med_image_ml-0.0.1/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.2/src/multi_med_image_ml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,25 @@
 def compile_dicom_py(dicom_folder):
 	dicom2nifti.convert_directory(dicom_folder,"conv.nii.gz")
 	dicom_files = (glob.glob(os.path.join("*.dcm")))
 
 import platform
 platform_system = platform.system()
 
+def path_func_default(filename,reverse=False):
+	return filename
+
+def check_path_func(path_func):
+	if path_func(path_func(os.path.realpath(__file__)),reverse=True) \
+		!= os.path.realpath(__file__):
+		raise Exception("""
+			path_func must be a function that translates
+			a filename to an index key and back with the
+			'reverse' option input""")
+
 """
 Uses dcm2niix, since that's had the best results overall when converting dicom
 to nifti, even though it's a UNIX command
 """
 
 def compile_dicom_folder(dicom_folder,db_builder=None):
 	if dcm2niix_installed:
@@ -160,19 +171,21 @@
 		#	"1Scl5iib7V5pWRULKnc6-k0edN2YfGhc7",
 		#	weights_lib_json)
 		file_id = "1Scl5iib7V5pWRULKnc6-k0edN2YfGhc7"
 		gdown.download(
 			f"https://drive.google.com/uc?export=download&confirm=pbef&id={file_id}",
    	 		weights_lib_json
 		)
-	print(weights_lib_json)
 	with open(weights_lib_json,'r') as fileobj:
 		weights_lib = json.load(fileobj)
 	if weights not in weights_lib:
-		raise Exception(f"No such model: {weights}")
+		raise Exception(
+			"No such model: %s. Available options are %s" % \
+			(weights," ".join(list(weights_lib)))
+			)
 	else:
 		#download_file_from_google_drive(
 		#	weights_lib[weights],
 		#	weights_file)
 		file_id = weights_lib[weights]
 		gdown.download(
 			f"https://drive.google.com/uc?export=download&confirm=pbef&id={file_id}",
```

### Comparing `multi_med_image_ml-0.0.1/tests/unit_tests.py` & `multi_med_image_ml-0.0.2/tests/unit_tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 				filepath = os.path.join(root,name)
 				ext = os.path.splitext(filepath)[1]
 				if ext == ".pkl":
 					os.remove(filepath)
 
 class TestSimple(unittest.TestCase):
 	def test_dicom_compile(self):
-		return
 		nifti_file,json_file = compile_dicom(im1)
 		self.assertTrue(os.path.isfile(nifti_file))
 		self.assertEqual(os.path.splitext(nifti_file)[1], ".gz")
 		self.assertTrue(os.path.isfile(json_file))
 		self.assertEqual(os.path.splitext(json_file)[1], ".json")
 		len_glob = len(glob.glob(os.path.join(im1,'*')))
 		nifti_file,json_file = compile_dicom(im1,cache=True)
@@ -66,58 +65,52 @@
 		if os.path.splitext(nifti_file)[1] == ".gz":
 			os.remove(nifti_file)
 		if os.path.splitext(json_file2)[1] == ".json":
 			os.remove(json_file2)
 		if os.path.splitext(nifti_file2)[1] == ".gz":
 			os.remove(nifti_file2)
 	def test_single_im_load(self):
-		return
 		im = ImageRecord(im1,dim=(24,48,32),cache=False)
 		img = im.get_image()
 		self.assertEqual(img.shape[0], 24)
 		self.assertEqual(img.shape[1], 48)
 		self.assertEqual(img.shape[2], 32)
 	def test_cache(self):
-		return
 		im = ImageRecord(im1,dim=(33,16,3),cache=True)
 		img = im.get_image()
 		self.assertEqual(img.shape[0], 33)
 		self.assertEqual(img.shape[1], 16)
 		self.assertEqual(img.shape[2], 3)
 		self.assertTrue(im.cached_record is not None)
 		self.assertTrue(os.path.isfile(im.cached_record))
 		self.assertEqual(os.path.splitext(im.cached_record)[1], ".npy")
 		if os.path.isfile(im.cached_record):
 			os.remove(im.cached_record)
 	def test_single_nifti_load(self):
-		return
 		im = ImageRecord(nifti_im,dim=(4,5,6),cache=True)
 		img = im.get_image()
 		self.assertEqual(img.shape[0], 4)
 		self.assertEqual(img.shape[1], 5)
 		self.assertEqual(img.shape[2], 6)
 	def test_npy_load(self):
-		return
 		#self.assertTrue(os.path.isfile(npy_im))
 		im = ImageRecord(npy_im,dim=(4,5,6))
 		img = im.get_image()
 		self.assertEqual(img.shape[0], 4)
 		self.assertEqual(img.shape[1], 5)
 		self.assertEqual(img.shape[2], 6)	
 	def test_single_nifti_load_torch(self):
-		return
 		im = ImageRecord(nifti_im,dim=(4,5,6),cache=False,
 			dtype='torch')
 		img = im.get_image()
 		self.assertTrue(torch.is_tensor(img))
 		self.assertEqual(img.size()[0], 4)
 		self.assertEqual(img.size()[1], 5)
 		self.assertEqual(img.size()[2], 6)
 	def test_basic_load_torch(self):
-		return
 		medim_loader = MedImageLoader(
 					imfolder1,
 					imfolder2,
 					dim=(48,32,24),
 					dtype="torch",
 					batch_size=16,
 					cache = False,
@@ -127,15 +120,14 @@
 			self.assertTrue(torch.is_tensor(label))
 			imsize = image.size()
 			self.assertEqual(imsize[0], 16)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	def test_basic_load_numpy(self):
-		return
 		medim_loader = MedImageLoader(
 					imfolder1,
 					imfolder2,
 					dim=(48,32,24),
 					dtype="numpy",
 					batch_size=16,
 					cache = False,
@@ -145,15 +137,14 @@
 			self.assertTrue(isinstance(label,np.ndarray))
 			imsize = image.shape
 			self.assertEqual(imsize[0], 16)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	def test_pandas(self):
-		return
 		medim_loader = MedImageLoader(
 					imfolder1,
 					imfolder2,
 					dim = (48,32,24),
 					dtype = "numpy",
 					cache = True,
 					channels_first=False)
@@ -178,15 +169,14 @@
 		for root, dirs, files in os.walk(im_root):
 			for name in files:
 				fpath = os.path.join(root,name)
 				if rstr in fpath:
 					self.assertTrue(fpath in df.index)
 		
 	def test_pandas_2(self):
-		return
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			dim=(48,32,24),
 			cache=True,
 			dtype="numpy",
 			channels_first=False)
 		for image,label in medim_loader: continue
 		pandas_file = medim_loader.all_vars_file
@@ -199,15 +189,14 @@
 			self.assertEqual(len(imsize),5)
 			self.assertEqual(imsize[0], 16)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	
 	def test_match_label_confounds(self):
-		return
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			dim=(48,32,24),
 			cache=True,
 			dtype="numpy",
 			channels_first=False)
 		for image,label in medim_loader: continue 
 		pandas_file = medim_loader.all_vars_file
@@ -222,15 +211,14 @@
 			imsize = image.shape
 			self.assertEqual(len(imsize),5)
 			self.assertEqual(imsize[0], 16)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	def test_grouping(self):
-		return
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			dim=(48,32,24),
 			cache=True,
 			dtype="torch",
 			channels_first=False)
 		pandas_file = medim_loader.all_vars_file
 		for image,label in medim_loader:
@@ -251,23 +239,21 @@
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 		C = patient.get_C()
 		C_dud = patient.get_C_dud()
 		Y = patient.get_Y()
 	def test_more(self):
-		return
 		medim_loader = MedImageLoader(imfolder1)
 		for image in medim_loader:
 			imsize = image.shape
 		medim_loader = MedImageLoader(imfolder2,augment=True)
 		for image in medim_loader:
 			continue
 	def test_model(self):
-		return
 		model = MultiInputModule(Y_dim=(32,32),C_dim=(32,32))
 		#medim_loader = MedImageLoader(imfolder1,imfolder2,
 		#	cache=True)
 		#for image,label in medim_loader: continue
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			group_by="Patient ID",
 			return_obj=True,
@@ -279,26 +265,19 @@
 			lr= 1e-5
 		)
 		loss_function = nn.MSELoss()
 		
 		for p in medim_loader:
 			optimizer.zero_grad()
 			y_pred,y_reg = model(p)
-			print("y_pred")
-			print(y_pred.size())
-			print("y_reg")
-			print(y_reg.size())
-			print("p.get_Y()")
-			print(p.get_Y().size())
 			loss = loss_function(p.get_Y(),y_pred)
 			loss.backward()
 			optimizer.step()
 			break
 	def test_trainer(self):
-		return
 		model = MultiInputModule(Y_dim = (17,2),C_dim=(13,11))
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			cache=True,
 			label=["MRAcquisitionType",
 					"ImageOrientationPatientDICOM"],
 			confounds=["Slice Thickness","Repetition Time"],
 			return_obj = True,
@@ -321,16 +300,32 @@
 			dtype="torch",
 			batch_size=14,Y_dim = (13,14),C_dim=(19,21))
 		trainer = MultiInputTrainer(model,batch_size=2)
 		for i in range(3):
 			#print(f"Epoch {i}")
 			for p in medim_loader:
 				trainer.loop(p,dataloader=medim_loader)	
+
+	def test_dyn_input(self):
+		model = MultiInputModule(Y_dim = (13,14),C_dim=(19,21))
+		medim_loader = MedImageLoader(imfolder1,imfolder2,
+			cache=False,
+			label=["MRAcquisitionType",
+					"Manufacturer"],
+			confounds=["Slice Thickness","Repetition Time"],
+			return_obj = True,
+			dtype="torch",
+			batch_size=14,Y_dim = (13,14),C_dim=(19,21),
+			static_inputs = ["User Data 7","Slice Thickness"])
+		trainer = MultiInputTrainer(model,batch_size=2)
+		for i in range(3):
+			for p in medim_loader:
+				trainer.loop(p,dataloader=medim_loader)
+
 	def test_cache3(self):
-		return
 		model = MultiInputModule((11,17),C_dim=(23,5))
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			cache=True,
 			label=["MRAcquisitionType",
 					"Manufacturer"],
 			confounds=["Slice Thickness","Repetition Time"],
 			return_obj = True,
@@ -340,15 +335,14 @@
 					batch_size=2,
 					loss_image_dir = '../loss_images',
 					checkpoint_dir = '../checkpoints',
 					name = 'unit_test',
 					verbose = False,
 					save_latest_freq = 1)
 		for i in range(3):
-			#print(f"Epoch {i}")
 			for p in medim_loader:
 				trainer.loop(p,dataloader=medim_loader)	
 	def test_weight_download(self):
 		return
 		model = MultiInputModule(weights="unit_test")
 if __name__ == "__main__":
 	#clear_files()
```

### Comparing `multi_med_image_ml-0.0.1/pyproject.toml` & `multi_med_image_ml-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.1"
+version = "0.0.2"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
@@ -16,15 +16,20 @@
   "nibabel",
   "datefinder",
   "monai",
   "dicom2nifti",
   "dateutil",
   "sklearn",
   "pydicom",
-  "dcm2niix"
+  "dcm2niix",
+  "platformdirs",
+  "urllib",
+  "pytorch_grad_cam",
+  "requests",
+  "gdown"
 ]
 requires-python = ">=3.8"
 
 authors = [
   {name = "Matt Leming", email = "mleming@mgh.harvard.edu"}
 ]
 maintainers = [
```

