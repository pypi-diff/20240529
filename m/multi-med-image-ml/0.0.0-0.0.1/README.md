# Comparing `tmp/multi_med_image_ml-0.0.0.tar.gz` & `tmp/multi_med_image_ml-0.0.1.tar.gz`

## Comparing `multi_med_image_ml-0.0.0.tar` & `multi_med_image_ml-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    23237 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    45395 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/tests/unit_tests.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/logo.png
+-rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/model_diagram.png
+-rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/.images/regress_figure.png
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/example_train.py
+-rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/base_options.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/test_options.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/example/options/train_options.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10687 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    45669 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    11528 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/tests/weights.json
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.1/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.0/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.0/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.1/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 					labels=[],
 					confounds=[],
 					dim=None,
 					cdim=None):
 
 		self.filename = filename
 		self.dim = dim
+		self.labels = [] if labels is None else labels
+		self.confounds = [] if confounds is None else confounds
 		if all_vars is not None:
 			self.all_vars = all_vars
 			self.columns = set(self.all_vars.columns)
 		elif os.path.isfile(filename):
 			self.all_vars = pd.read_pickle(self.filename)
 			self.columns = set(self.all_vars.columns)
 		elif self.filename is not None:
@@ -31,17 +33,20 @@
 		else:
 			raise Exception("DatabaseWrapper cannot have no inputs")
 		self.jdict = []
 		
 		if isinstance(self.all_vars,str) and os.path.isfile(self.all_vars)\
 			 and os.path.splitext(self.all_vars)[1] == ".pkl":
 			self.all_vars = pd.read_pickle(self.all_vars)
-		self.labels = [] if labels is None else labels
-		self.confounds = [] if confounds is None else confounds
+	
+	def build_metadata(self):
 		for l in self.labels:
+			if l not in self.all_vars.columns:
+				print("%s was dead the whole time" % l)
+				print(self.all_vars)
 			assert(l in self.all_vars.columns)
 		for c in self.confounds:
 			assert(c in self.all_vars.columns)
 		assert(len(set(self.labels).intersection(set(self.confounds)))==0)
 		self.uniques = {}
 		self.n_buckets=10
 		for c in self.confounds + self.labels:
@@ -196,14 +201,15 @@
 			return dateutil.parser.parse(d)
 	def get_exam_date(self,fkey: str) -> datetime.date:
 		d = self._get_val(fkey,["ExamEndDTS","Acquisition Date"])
 		return self.parse_date(d)
 	def get_birth_date(self,fkey):
 		d = self._get_val(fkey,["BirthDTS"])
 		return self.parse_date(d)
+	
 	def loc_val(self,fkey,c):
 		try:
 			return self.all_vars.loc[fkey,c]
 		except KeyError:
 			nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii.gz")
 			
 			if not os.path.isfile(nifti_file):
@@ -224,16 +230,16 @@
 			if not (os.path.isfile(json_file)):
 				json_file = os.path.join(
 					os.path.dirname(nifti_file),
 					"metadata.json")
 				if not os.path.isfile(json_file):
 					return
 		npy_file = get_dim_str(nifti_file,self.dim)
-		if not os.path.isfile(npy_file):
-			return
+		#if not os.path.isfile(npy_file):
+		#	return
 		if npy_file not in self.jdict and npy_file not in self.all_vars.index:
 			with open(json_file,'r') as fileobj:
 				json_dict = json.load(fileobj)
 			json_dict["fkey"] = npy_file
 			json_dict["filename"] = npy_file
 			for item in json_dict:
 				if isinstance(json_dict[item],list):
```

### Comparing `multi_med_image_ml-0.0.0/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.1/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from Records import BatchRecord,ImageRecord
 from DataBaseWrapper import DataBaseWrapper
 
 class MedImageLoader():
 	def __init__(self,*image_folders,
 			pandas_cache = '../pandas/',
-			cache = False,
+			cache = True,
 			path_func = None,
 			batch_by_pid=True,
 			return_as_patient_record=False,
 			file_record_name=None,
 			n_out_y=None,
 			forcealt=True,
 			all_vars = None,
@@ -34,16 +34,16 @@
 			confounds = [],
 			match_confounds = [],
 			label = [],
 			group_by = None,
 			augment = True,
 			val_ranges = {},
 			dtype="numpy",
-			Y_dim = (32,32),
-			C_dim = (32,32),
+			Y_dim = (16,32),
+			C_dim = (16,32),
 			return_obj = False,
 			channels_first = True):
 		self.channels_first = channels_first
 		self.image_folders = image_folders
 		self.augment = augment
 		self.dim=dim
 		self.dtype=dtype
@@ -59,14 +59,15 @@
 		self.confounds = confounds
 		self.path_func = path_func
 		self.group_by = group_by
 		self.n_out_y = n_out_y # Set dimension for Y
 		self.forcealt = forcealt
 		self.Y_dim = Y_dim
 		self.C_dim = C_dim
+		self.mode = None
 		
 		# Stores images so that they aren't repeated in different stacks
 		self.image_dict = {}
 		# If true, this uses one match confound at a time and cycles through
 		# them
 		self.zero_data_list = []
 		self.match_confounds = match_confounds
@@ -75,28 +76,30 @@
 		else:
 			self.batch_size = batch_size
 		self.return_obj = return_obj
 		
 		# Create or read in the image database
 		if self.pickle_input():
 			self.all_vars_file = self.image_folders[0]
-			assert(self.cache or os.path.isfile(self.all_vars_file))
+			#assert(self.cache or os.path.isfile(self.all_vars_file))
 		else:
 			os.makedirs(os.path.dirname(self.pandas_cache),
 				exist_ok=True)
 			self.all_vars_file = os.path.join(
 				self.pandas_cache,
-				"all_vars_%s.pkl" % get_dim_str(dim=self.dim))		
-		if self.batch_by_pid and not os.path.isfile(self.all_vars_file):
-			warnings.warn("Must have working all vars file to group files. One once without group_by set")
+				"all_vars_%s.pkl" % get_dim_str(dim=self.dim))
+		
 		self.all_vars = DataBaseWrapper(
 					filename=self.all_vars_file,
 					labels=self.label,
 					confounds=self.confounds,
 					dim=self.dim)
+		if not self.pickle_input():
+			self.build_pandas_database()
+		self.all_vars.build_metadata()
 		
 		# Determine which mode the scheduler is in
 		if (self.label is not None and len(self.label) > 0):
 			self.mode = "match"
 		else:
 			self.mode = "iterate"
 		
@@ -126,15 +129,36 @@
 		self.mode_hidden = "iterate"
 		self.forcealt_hidden = False
 		if self.return_labels():
 			for l in self.label:
 				if l not in self.val_ranges:
 					self.match_confounds_hidden.append(l)
 		self.index = 0
-		self.load_image_stack()	
+		self.load_image_stack()
+	# Builds up the entire cache in one go — may take a while
+	def build_pandas_database(self):
+		assert(self.all_vars is not None)
+		assert(not self.pickle_input())
+		old_mode = self.mode
+		self.mode = "iterate"
+		self._load_list_stack()
+		
+		for i,filename in enumerate(self.image_dict):
+			im = self.image_dict[filename]
+			if im.fkey not in self.all_vars.all_vars.index:
+				try:
+					im.get_image()
+					im.clear_image()
+				except ImageFileError:
+					continue
+			if i % 100 == 0:
+				self.all_vars.out_dataframe()
+		self.clear_mem()
+		self.all_vars.out_dataframe()
+		self.mode = old_mode
 	def pickle_input(self):
 		return len(self.image_folders) == 1 and \
 			os.path.splitext(self.image_folders[0])[1] == ".pkl"
 	def tl(self):
 		# Top label
 		
 		if len(self.label) == 0: tl = "Folder"
@@ -167,42 +191,48 @@
 			[fname_list],_ = get_balanced_filename_list(self.tl(),
 				self.match_confounds,
 				selection_ratios=[1], total_size_limit=np.inf,
 				non_confound_value_ranges = self.val_ranges,verbose=False,
 				all_vars=self.all_vars.all_vars)
 			fname_list = list(fname_list)
 			if len(fname_list) == 0:
+				
+				print(self.all_vars.all_vars.loc[:,self.tl()])
 				raise Exception("No valid files from %s" % self.tl())
 			assert(isinstance(fname_list,list))
 			return self.all_vars.stack_list_by_label(fname_list,self.tl())
 		else:
 			raise Exception("Invalid mode: %s" % self.mode)
-	def load_image_stack(self):
-		if self.get_mem() > 10000000000:
-			print("Clearing memory")
-			self.clear_mem()
-		#self.rotate_labels()
-		if self.tl() not in self.file_list_dict:
-			self.file_list_dict[self.tl()] = []
+	def _load_list_stack(self):
 		X_files = self.get_file_list() 
 		for i,filename_list in enumerate(X_files):
 			for j,filename in enumerate(filename_list):
 				if filename in self.image_dict:
 					X_files[i][j] = self.image_dict[filename]
 				else:
+					
 					X_files[i][j] = ImageRecord(filename,
 								dim=self.dim,
 								y_nums=[i] if len(X_files) == 1 else None,
 								Y_dim = self.Y_dim,
 								C_dim = self.C_dim,
 								dtype=self.dtype,
 								all_vars = self.all_vars,
 								cache=self.cache,
 								static_inputs = self.static_inputs)
 					self.image_dict[filename] = X_files[i][j]
+		return X_files
+	def load_image_stack(self):
+		if self.get_mem() > 10000000000:
+			print("Clearing memory")
+			self.clear_mem()
+		#self.rotate_labels()
+		if self.tl() not in self.file_list_dict:
+			self.file_list_dict[self.tl()] = []
+		X_files = self._load_list_stack()
 		if self.batch_by_pid:
 			pdict = {}
 			for images in X_files:
 				for image in images:
 					image.load_extra_info()
 					if not is_nan(image.group_by):
 						if image.group_by not in pdict:
@@ -248,16 +278,15 @@
 		self.match_confounds,self.match_confounds_hidden = \
 			self.match_confounds_hidden,self.match_confounds
 		self.forcealt,self.forcealt_hidden = self.forcealt_hidden,self.forcealt
 		self.mode,self.mode_hidden = self.mode_hidden,self.mode
 	def __next__(self):
 		if len(self) == 0: self.load_image_stack()
 		if self.index > len(self):
-			if self.cache:
-				self.all_vars.out_dataframe()
+			self.all_vars.out_dataframe()
 			self.index = 0
 			self.rotate_labels()
 			self.load_image_stack()
 			raise StopIteration
 		temp = []
 		for i in range(self.batch_size):
 			b = i % len(self.file_list_dict[self.tl()])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multi_med_image_ml-0.0.0/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.1/src/multi_med_image_ml/Records.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 		all_vars = None,
 		dim=(96,96,96),
 		dtype="torch",
 		ID = None,
 		extra_info_list = None,
 		y_on_c = True,
 		cache = True,
-		Y_dim = (32,32),
-		C_dim = (32,32),
+		Y_dim = (16,32),
+		C_dim = (16,32),
 		y_nums = None,
 		c_nums = None,
 		static_inputs=[]):
 		
 		self.dim=dim
 		self.filename = filename
 		self.fkey = get_dim_str(self.filename,self.dim)
@@ -102,15 +102,39 @@
 				elif ext  == ".nii":
 					self.image_type = "nifti"
 				elif ext == ".gz" and os.path.splitext(name)[1] == ".nii":
 					self.image_type = "nifti"
 				elif ext == ".dcm":
 					self.image_type = "dicom"
 				else:
-					raise Exception("Not implemented for extension %s" % ext)
+					raise Exception(
+					"Not implemented for extension %s" % ext)
+			elif os.path.isfile(
+				get_dim_str(self.filename,
+						dim=self.dim,
+						outtype='.nii.gz')):
+				self.filename = get_dim_str(self.filename,
+							dim=self.dim,
+							outtype='.nii.gz')
+				return self.get_image_type()
+			elif os.path.isfile(
+				get_dim_str(self.filename,
+						dim=self.dim,
+						outtype='.nii')):
+				self.filename = get_dim_str(self.filename,
+							dim=self.dim,
+							outtype='.nii')
+				return self.get_image_type()
+			elif os.path.isdir(get_dim_str(self.filename,
+							dim=self.dim,
+							outtype='dicom')):
+				self.filename = get_dim_str(self.filename,
+							dim=self.dim,
+							outtype='dicom')
+				return self.get_image_type()
 		return self.image_type
 	def get_mem(self):
 		if self.image is None:
 			return 0
 		#else:
 		#	return np.prod(self.image.shape) * \
 		#		np.dtype(self.image.dtype).itemsize
```

### Comparing `multi_med_image_ml-0.0.0/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.1/src/multi_med_image_ml/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import itertools
 import numpy as np
 from datetime import datetime
 import hashlib
 import os,sys
 from copy import deepcopy as copy
 from Records import ImageRecord,BatchRecord
+from utils import download_weights
 
 # Three functions that are used to get the age encoding functions
 def time_index(i,pos,d=512,c=10000):
 	if i % 2 == 0:
 		v = math.sin(pos/(c**(2*i/d)))
 	else:
 		v = math.cos(pos/(c**(2*i/d)))
@@ -97,15 +98,15 @@
         )
     def forward(self, x):
         x = self.flatten(x)
         logits = self.linear_relu_stack(x)
         return logits
 
 class Encoder(nn.Module):
-	def __init__(self,LATENT_SIZE=512):
+	def __init__(self,latent_dim=512):
 		super(Encoder,self).__init__()
 		nchan=1
 		base_feat = 64
 		self.encoder = nn.Sequential(
 			nn.Conv3d(in_channels = nchan, out_channels = base_feat, stride=2,
 				kernel_size=5, padding = 2), #1*96*96*96 -> 64*48*48*48
 			nn.LeakyReLU(),
@@ -126,32 +127,32 @@
 			nn.InstanceNorm3d(base_feat*4),
 			nn.Conv3d(in_channels = base_feat*4, out_channels = base_feat*32,
 				stride=1,kernel_size = 3,padding=0), #256*3*3*3 -> 2048*1*1*1
 			nn.LeakyReLU(),
 			Reshape([-1,base_feat*32]),
 			nn.Linear(in_features = base_feat*32, out_features = base_feat*16),
 			nn.LeakyReLU(),
-			nn.Linear(in_features = base_feat*16, out_features = LATENT_SIZE),
+			nn.Linear(in_features = base_feat*16, out_features = latent_dim),
 			
 		)
 	def parameters(self):
 		return self.encoder.parameters()
 	def forward(self, x):
 		x = self.encoder(x)
 		return x
 
 
 class Decoder(nn.Module):
 	def __init__(self):
 		super(Decoder,self).__init__()
 		nchan=1
 		base_feat = 64
-		LATENT_SIZE = 512	
+		latent_dim = 512	
 		self.decoder = nn.Sequential(
-			nn.Linear(in_features = LATENT_SIZE, out_features = base_feat*16),
+			nn.Linear(in_features = latent_dim, out_features = base_feat*16),
 			nn.ReLU(),
 			nn.BatchNorm1d(base_feat*16),
 			nn.Linear(in_features = base_feat*16, out_features = base_feat*32),
 			nn.ReLU(),
 			Reshape([-1,base_feat*32,1,1,1]),
 			nn.ConvTranspose3d(in_channels = base_feat*32,
 				out_channels = base_feat*16, kernel_size = 3,stride=1,
@@ -229,15 +230,15 @@
 	def cpu(self):
 		for r in self.regressor_set:
 			r.cpu()
 	def forward(self,x):
 		return torch.cat([r(x) for r in self.regressor_set],2)
 		
 class Classifier(nn.Module):
-	def __init__(self,latent_dim,n_inputs,base_feat,nout,nlabels):
+	def __init__(self,latent_dim,n_inputs,base_feat,n_out,n_labels):
 		super(Classifier,self).__init__()
 		
 		self.classifier = nn.Sequential(
 			nn.Linear(latent_dim*n_inputs,n_inputs*base_feat*4),
 			nn.LeakyReLU(),
 			Reshape([-1,n_inputs,base_feat*4]),
 			nn.InstanceNorm1d(n_inputs,affine=True),
@@ -247,106 +248,123 @@
 				out_features = n_inputs*base_feat*2),
 			nn.LeakyReLU(),
 			Reshape([-1,n_inputs,base_feat*2]),
 			nn.InstanceNorm1d(n_inputs,affine=True),
 			Reshape([-1,1,n_inputs*base_feat*2]),
 
 			nn.Linear(in_features = n_inputs*base_feat*2,
-				out_features = nout*nlabels),
-			Reshape([-1,nout,nlabels]),
+				out_features = n_out*n_labels),
+			Reshape([-1,n_out,n_labels]),
 			nn.Sigmoid(),	
 		)
 	def parameters(self):
 		return self.classifier.parameters()
 	def forward(self,x):
 		return self.classifier(x)
 
 class MultiInputModule(nn.Module):
 	def __init__(self,
-				n_out,
+				Y_dim = (16,32), # Number of labels, Number of choices
+				C_dim = (16,32), # Number of labels, Number of choices
 				n_dyn_inputs = 14,
-				n_stat_inputs = 0,
+				n_stat_inputs = 2,
 				use_attn = False,
 				encode_age = False,
-				regressor_dims = None,
 				variational = False,
 				zero_input = False,
 				remove_uncertain = False,
 				device = torch.device('cpu'),
-				latent_dim = 128):
+				latent_dim = 128,
+				weights = None):
 		super(MultiInputModule,self).__init__()
 		
 		# Model Parameters
-		self.LATENT_DIM = latent_dim
+		self.latent_dim = latent_dim
+		
+		# Number of non-image, patient-specific demographic inputs. Sex and 
+		# ethnicity are two that can be applied.
 		self.n_stat_inputs = n_stat_inputs
+		
+		# Max number of images that can be passed in
 		self.n_dyn_inputs = n_dyn_inputs
+		
+		# Total number of inputs, which is used for the classifier model
 		self.n_inputs = self.n_stat_inputs + self.n_dyn_inputs
-		base_feat = 64
-		self.nout = n_out
+		
+		self.Y_dim = (1,Y_dim) if isinstance(Y_dim,int) else Y_dim
 		num_heads = self.n_inputs
-		embed_dim = self.LATENT_DIM
-		self.regressor_dims = regressor_dims
+		self.C_dim = C_dim
 		self.zero_input = zero_input
 		self.remove_uncertain = remove_uncertain
 		if self.remove_uncertain:
 			self.record_training_sample = False
 			self.num_training_samples = 300
 			self.training_sample = torch.zeros(
 				(
-					self.LATENT_DIM,
+					self.latent_dim,
 					self.num_training_samples
 				),
 				device=device)
 
-		if isinstance(n_out,int):
-			n_out = (n_out,1)
 		# Training options
 		self.use_attn = use_attn
 		self.encode_age = encode_age
 		self.static_dropout = True # Randomly mask static inputs in training
 		self.variational = variational
 		
 		# A record that prevents unrecognized keys from being applied during
 		# the test phase
 		self.static_record = [set() for _ in range(self.n_stat_inputs)]
 		
+		# Sets the multiplier for the number of features in each model component
+		base_feat = 64
 		# Modules
 		
 		# Makes the encoder output a variational latent space, so it's a
 		# Gaussian distribution.
 		if self.variational:
-			self.encoder = Encoder(LATENT_SIZE=2*self.LATENT_DIM)
+			self.encoder = Encoder(latent_dim=self.latent_dim)
 			self.z_mean = nn.Sequential(
-				nn.Linear(2*self.LATENT_DIM,self.LATENT_DIM)
+				nn.Linear(2*self.latent_dim,self.latent_dim)
 			)
 			self.z_log_sigma = nn.Sequential(
-				nn.Linear(2*self.LATENT_DIM,self.LATENT_DIM)
+				nn.Linear(2*self.latent_dim,self.latent_dim)
 			)
 			self.epsilon = torch.distributions.Normal(0, 1)
 			self.epsilon.loc = self.epsilon.loc.cuda(device)
 			self.epsilon.scale = self.epsilon.scale.cuda(device)
 		else:
-			self.encoder = Encoder(LATENT_SIZE=self.LATENT_DIM)
-		#self.decoder = Decoder()
-		if self.use_attn:
-			self.multihead_attn = nn.MultiheadAttention(
-										embed_dim,
-										num_heads,
-										batch_first=True)
-		self.classifier = Classifier(self.LATENT_DIM,
-										self.n_inputs,
-										base_feat,
-										self.nout[0],
-										self.nout[1])
-		if self.regressor_dims is not None:
-			n_confounds,n_choices = self.regressor_dims
-			self.regressor = Regressor(self.LATENT_DIM,n_confounds,n_choices,
+			self.encoder = Encoder(latent_dim=self.latent_dim)
+		# The output of the classifier and regressor, and encoder are kept
+		# consistent, to 16 max outputs and 32 possible choices. This makes
+		# cross-training easier, though it's less efficient.
+		self.classifier = Classifier(latent_dim = self.latent_dim,
+										n_inputs = self.n_inputs,
+										base_feat = base_feat,
+										n_out = self.Y_dim[0],#16,
+										n_labels = self.Y_dim[1])#32)
+		if self.C_dim is not None:
+			n_confounds,n_choices = self.C_dim
+			self.regressor = Regressor(self.latent_dim,
+				n_confounds=self.C_dim[0],
+				n_choices=self.C_dim[1],
 				device=device)
 		else: self.regressor = None
-	
+		
+		if weights is not None:
+			if self.C_dim ! (16,32) or self.Y_dim != (16,32):
+				warnings.warn(
+					"Pretrained models may not function if defaults are altered"
+					)
+			if os.path.isfile(weights) and \
+				os.path.splitext(weights)[1] == ".pt":
+				self.load_state_dict(torch.load(weights))
+			else:
+				self.load_state_dict(torch.load(download_weights(weights)))
+
 	def forward_ensemble(self,kwargs,n_ens=10):
 		x = []
 		for i in range(n_ens):
 			x.append(self(**kwargs))
 		return x
 
 	def cuda(self,device):
@@ -465,15 +483,15 @@
 				random.choice([True,False])):
 			age_encodings = []
 			if dates1 is not None:
 				for i,date in enumerate(dates1):
 					age_encoding = get_age_encoding(
 									date,
 									bdate1,
-									d=self.LATENT_DIM)
+									d=self.latent_dim)
 					age_encodings.append(age_encoding)
 				age_encodings = np.array(age_encodings)
 				age_encodings =  torch.tensor(
 									age_encodings,
 									device=x.device
 									).float()
 				x = torch.add(x,age_encodings)
@@ -507,15 +525,15 @@
 					if static_input[i] not in e:
 						raise Exception(
 							"""
 								Input %s not a previous demographic
 								input (previous inputs were %s)
 							""" % (static_input[i],str(e))
 						)
-			x_ = encode_static_inputs(static_input,d=self.LATENT_DIM)
+			x_ = encode_static_inputs(static_input,d=self.latent_dim)
 			x_ = torch.tensor(x_,device = x.device)
 			x_ = torch.unsqueeze(x_,0)
 			for i in range(x_.shape[0]):
 				if ((not self.static_dropout) or random.choice([True,False]) and self.training) or\
 					(not self.static_dropout):
 					x[:,(-(self.n_stat_inputs) + i):,:] = x_[i,:]
 		
@@ -550,15 +568,15 @@
 		#z = z_mean + (z_log_sigma.exp()*self.epsilon.sample(z_mean.shape))
 		#z = nn.functional.sigmoid(z)
 		#y = self.decoder(z)
 		#self.kl = (z_mean**2 + z_log_sigma.exp()**2 - z_log_sigma - 0.5).sum()
 	
 		# Switch batch channel with layer channel prior to running classifier
 		x = torch.unsqueeze(x,-1)
-		x = x.contiguous().view([-1,1,self.LATENT_DIM*self.n_inputs]) # 16*512 -> 1*[16*512]
+		x = x.contiguous().view([-1,1,self.latent_dim*self.n_inputs]) # 16*512 -> 1*[16*512]
 		x = self.classifier(x)
 		if use_regression: return x,reg
 		else: return x
 
 class EnsembleModel(nn.Module):
 	def __init__(self,model_list):
 		super(EnsembleModel,self).__init__()
@@ -582,15 +600,15 @@
 		return new_output,new_hidden
 
 class VariationalEncoder(nn.Module):
 	def __init__(self):
 		super(Encoder,self).__init__()
 		nchan=1
 		base_feat = 64
-		LATENT_SIZE = 512
+		latent_dim = 512
 		self.encoder = nn.Sequential(
 			nn.Conv3d(in_channels = nchan, out_channels = base_feat, stride=2, kernel_size=5, padding = 2), #1*96*96*96 -> 64*48*48*48
 			nn.LeakyReLU(),
 			nn.Dropout(0.5),
 			nn.InstanceNorm3d(base_feat),
 			nn.Conv3d(in_channels = base_feat, out_channels = base_feat*2, stride=2, kernel_size = 5,padding=2), #64*48*48*48 -> 128*24*24*24
 			nn.LeakyReLU(),
@@ -603,15 +621,15 @@
 			nn.InstanceNorm3d(base_feat*4),
 			nn.Conv3d(in_channels = base_feat*4, out_channels = base_feat*32, stride=1,kernel_size = 3,padding=0), #256*3*3*3 -> 2048*1*1*1
 			nn.LeakyReLU(),
 			nn.Dropout(0.5),
 			Reshape([-1,base_feat*32]),
 			nn.Linear(in_features = base_feat*32, out_features = base_feat*16),
 			nn.LeakyReLU(),
-			nn.Linear(in_features = base_feat*16, out_features = LATENT_SIZE)
+			nn.Linear(in_features = base_feat*16, out_features = latent_dim)
 		)
 	def forward(self, x):
 		self.z_mean = nn.Linear(64, latent_dim)
 		self.z_log_sigma = nn.Linear(64, latent_dim)
 		#self.epsilon = torch.normal(size=(1, latent_dim), mean=0, std=1.0,
 		#	device=self.device)
 		self.epsilon = torch.distributions.Normal(0, 1)
@@ -646,16 +664,16 @@
 				nn.BatchNorm1d(1,affine=True),
 				Reshape([-1,base_feat]),
 				nn.Linear(base_feat,output_dim),
 				
 			)
 		else:
 			self.encoder = nn.Sequential(
-				#nn.Conv2d(in_channels = 1, out_channels = base_feat*4, stride=1, kernel_size=(self.LATENT_DIM,1), padding =0), #1*96*96*96 -> 64*48*48*48
-				#Reshape([-1,self.LATENT_DIM*self.n_inputs]),
+				#nn.Conv2d(in_channels = 1, out_channels = base_feat*4, stride=1, kernel_size=(self.latent_dim,1), padding =0), #1*96*96*96 -> 64*48*48*48
+				#Reshape([-1,self.latent_dim*self.n_inputs]),
 				nn.Linear(input_dim,input_dim//2),
 				nn.LeakyReLU(),
 				nn.BatchNorm1d(input_dim//2,affine=True),
 	
 				nn.Linear(in_features = input_dim//2, out_features = input_dim//4),
 				nn.LeakyReLU(),
 				nn.BatchNorm1d(input_dim//4,affine=True),
```

### Comparing `multi_med_image_ml-0.0.0/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.1/src/multi_med_image_ml/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from sklearn.metrics import roc_curve, auc
 from dateutil import relativedelta,parser
 import datetime,datefinder
 import pydicom as dicom
 import dicom2nifti
 import dicom2nifti.settings as settings
 settings.disable_validate_slice_increment()
+from platformdirs import user_cache_dir
+import urllib.request
 
 # Used to get a training set with equal distributions of input covariates
 # Can also be used to only have certain ranges of continuous covariates,
 # or certain labels of discrete covariates.
 
 if shutil.which('dcm2niix') is None:
 	dcm2niix_installed = False
@@ -33,14 +35,15 @@
 import platform
 platform_system = platform.system()
 
 """
 Uses dcm2niix, since that's had the best results overall when converting dicom
 to nifti, even though it's a UNIX command
 """
+
 def compile_dicom_folder(dicom_folder,db_builder=None):
 	if dcm2niix_installed:
 		if platform_system == "Windows":
 			os.system('dcm2niix %s 2> nul' % os.path.join(dicom_folder,'*.dcm'))
 		else:
 			os.system('dcm2niix %s >/dev/null 2>&1' % os.path.join(dicom_folder,
 					'*.dcm'))
@@ -84,42 +87,119 @@
 	if filename is not None:
 		base,ext1 = os.path.splitext(filename)
 		base,ext2 = os.path.splitext(base)
 		if outtype == ".npy":
 			if filename.endswith(f"resized_{dim_str}.npy"):
 				return filename
 			elif ext1.lower() == ".npy":
-				foo = re.sub("resized_[0-9].*.npy$",f"resized_{dim_str}.npy",filename)
+				foo = re.sub("resized_[0-9].*.npy$",
+						f"resized_{dim_str}.npy",filename)
 				print(filename)
 				print(foo)
 				print("get_dim_str")
 				return foo
 			return "%s_resized_%s.npy" % (base,dim_str)
+		elif outtype == "dicom":
+			return os.path.dirname(filename)
 		else:
 			assert(outtype[0] == ".")
 			if filename.endswith(f"_resized_{dim_str}.npy"):
 				return filename.replace(f"_resized_{dim_str}.npy",outtype)
 			else:
 				return filename.replace(ext2+ext1,outtype)
 	#assert(".nii" in [ext1.lower(),ext2.lower()])
 	else:
 		return dim_str
-	
+
+# Downloads and caches pretrained model weights
+def download_file_from_google_drive(file_id, destination):
+	URL = "https://docs.google.com/uc?export=download&confirm=t"
+
+	session = requests.Session()
+
+	response = session.get(URL, params={"id": file_id}, stream=True)
+	token = get_confirm_token(response)
+	print("token")
+	print(token)
+	print("response")
+	print(response)
+	token = "t"
+	if token:
+		params = {"id": file_id, "confirm": token}
+		response = session.get(URL, params=params, stream=True)
+	print(destination)
+	save_response_content(response, destination)
+
+
+def get_confirm_token(response):
+	for key, value in response.cookies.items():
+		if key.startswith("download_warning"):
+			return value
+
+	return None
+
+
+def save_response_content(response, destination):
+	CHUNK_SIZE = 32768
+
+	with open(destination, "wb") as f:
+		for chunk in response.iter_content(CHUNK_SIZE):
+			if chunk:  # filter out keep-alive new chunks
+				f.write(chunk)
+
+import requests,gdown
+def download_weights(weights):
+	weights_dir = os.path.join(user_cache_dir(),"MultiMedImageML","weights")
+	print(weights_dir)
+	os.makedirs(weights_dir,exist_ok=True)
+	weights_file = os.path.join(weights_dir,f"{weights}.pt")
+	if os.path.isfile(weights_file):
+		return weights_file
+	weights_lib_json = os.path.join(weights_dir,"weights.json")
+	if not os.path.isfile(weights_lib_json):
+		#download_file_from_google_drive(
+		#	"1Scl5iib7V5pWRULKnc6-k0edN2YfGhc7",
+		#	weights_lib_json)
+		file_id = "1Scl5iib7V5pWRULKnc6-k0edN2YfGhc7"
+		gdown.download(
+			f"https://drive.google.com/uc?export=download&confirm=pbef&id={file_id}",
+   	 		weights_lib_json
+		)
+	print(weights_lib_json)
+	with open(weights_lib_json,'r') as fileobj:
+		weights_lib = json.load(fileobj)
+	if weights not in weights_lib:
+		raise Exception(f"No such model: {weights}")
+	else:
+		#download_file_from_google_drive(
+		#	weights_lib[weights],
+		#	weights_file)
+		file_id = weights_lib[weights]
+		gdown.download(
+			f"https://drive.google.com/uc?export=download&confirm=pbef&id={file_id}",
+   	 		weights_file
+		)
+	assert(os.path.isfile(weights_file))
+	return weights_file
+
+# Determines if the input is an applicable image file. Excludes temporary files
 def is_image_file(filename):
 	basename,ext = os.path.splitext(filename)
 	_,ext2 = os.path.splitext(basename)
 	ext = ext2 + ext
 	basename = os.path.basename(basename)
-	if basename == "temp": return False
+	if not not_temp(basename): return False
 	return ext.lower() in [".nii",".nii.gz"]
 
+# Determines if file is dicom
 def is_dicom(filename):
 	basename,ext = os.path.splitext(filename)
 	return ext.lower() == ".dcm"
 
+# Three functions that search a folder path for all applicable images.
 def get_file_list_from_str(obj,db_builder=None):
 	assert(isinstance(obj, str))
 	if os.path.isfile(obj):
 		if is_image_file(obj):
 			return [obj]
 		else:
 			return []
@@ -173,15 +253,15 @@
 	assert(np.all([isinstance(_,str) for _ in obj]))
 	if np.all([len(_) == 0 for _ in obj]):
 		raise Exception("No valid files found")
 	elif np.any([len(_) == 0 for _ in obj]):
 		raise Exception("One without valid files")
 	return obj
 
-
+# Ad-hoc function that determines whether given keys are equal
 def equal_terms(term):
 	trans_dict = {'NOT_HISPANIC':'NO_NON_HISPANIC',
 				'HISPANIC':'YES_HISPANIC',
 				'PREFER_NOT_TO_SAY/DECLINE':'UNAVAILABLE',
 				'DECLINED': 'UNAVAILABLE',
 				'NULL':'UNAVAILABLE'}
 	if term in trans_dict: return trans_dict[term]
@@ -195,21 +275,17 @@
 
 def date_sorter(folder,ext):
 	filelist = glob.glob(os.path.join(folder,"*" + ext))
 	filelist = list(filter(lambda k: not_temp(k),filelist))
 	filelist = sorted(filelist,key=os.path.getmtime)
 	return filelist
 
-# Takes a folder of dicom files and turns it into a .nii.gz file. Relies on 
-# a bunch of UNIX programs. It's crap, but it works.
+# Takes a folder of dicom files and turns it into a .nii.gz file, with metadata.
+# stored in a .json file. Relies on dcm2niix.
 def compile_dicom(dicom_folder,cache=True,db_builder=None):
-	
-	#if not os.path.isdir(output_dir):
-	#	print(output_dir)
-	#	os.makedirs(output_dir)
 	assert(os.path.isdir(dicom_folder))
 	json_file = date_sorter(dicom_folder,'.json')
 	nii_file = date_sorter(dicom_folder,'.nii*')
 	if (len(json_file) == 0 or len(nii_file) == 0) or (not cache):
 		nii_file,json_file = compile_dicom_folder(dicom_folder,
 			db_builder=db_builder)
 	else:
@@ -231,14 +307,15 @@
 		os.system("gzip '%s' >/dev/null 2>&1" % nii_file)
 		nii_file = nii_file + ".gz"
 		assert(os.path.isfile(nii_file))
 	if db_builder is not None:
 		db_builder.add_json(nifti_file=nii_file,json_file=json_file)
 	return nii_file,json_file
 
+# Resizes and standardizes 3d numpy arrays to normalized dimensions
 def resize_np(nifti_data,dim):
 	if nifti_data.min() < 0 or nifti_data.max() > 1:
 		nifti_data -= nifti_data.min()
 		m = nifti_data.max()
 		nifti_data = nifti_data / m
 	if nifti_data.dtype != np.float32:
 		nifti_data = nifti_data.astype(np.float32)
@@ -248,15 +325,15 @@
 			nifti_data = np.squeeze(np.mean(nifti_data,axis=-1))
 		assert(len(nifti_data.shape) == len(dim))
 	if nifti_data.shape != dim:
 		zp = [dim[i]/nifti_data.shape[i] for i in range(len(dim))]
 		nifti_data = ndimage.zoom(nifti_data,zp)
 	return nifti_data
 
-
+# Prime number functions used in the data matching schemes
 def prime(i, primes):
 	for prime in primes:
 		if not (i == prime or i % prime):
 			return False
 	primes.append(i)
 	return i
 
@@ -288,21 +365,23 @@
 	n_primes = get_first_n_primes(np.sum(n_buckets) + 1)
 	discretized_confounds = np.zeros(confounds.shape)
 	for i in range(confounds.shape[0]):
 		if isinstance(confounds[i,0],str):
 			buckets = np.unique(confounds[i,:])
 		else:
 			buckets_s = []
-			for kk in range(0,sorted_confounds.shape[1],int(np.ceil(sorted_confounds.shape[1]/float(n_buckets[i])))):
+			lim = int(np.ceil(sorted_confounds.shape[1]/float(n_buckets[i])))
+			for kk in range(0,sorted_confounds.shape[1],lim):
 				buckets_s.append(sorted_confounds[i,kk])
 			buckets_s.append(sorted_confounds[i,-1])
 			buckets_s = np.array(buckets_s)
 			min_conf = sorted_confounds[i,0]
 			max_conf = sorted_confounds[i,-1]
-			buckets_v = (np.array(range(n_buckets[i] + 1))/float(n_buckets[i])) * (max_conf - min_conf) + min_conf
+			buckets_v = (np.array(range(n_buckets[i] + 1))/float(n_buckets[i]))\
+				 * (max_conf - min_conf) + min_conf
 			sv_ratio = 1.0
 			buckets = (sv_ratio) * buckets_s + (1.0 - sv_ratio) * buckets_v
 		for j in range(confounds.shape[1]):
 			d = discretize_value(confounds[i,j],buckets)
 			d = n_primes[int(np.sum(n_buckets[:i])) + d]
 			discretized_confounds[i,j] = d
 	return discretized_confounds
@@ -387,16 +466,16 @@
 	while i < len(S1):
 		if S1[i]:
 			output[i] = S2[i2]
 			i2 += 1
 		i += 1
 	return output
 
-# Returns a boolean array that is true if either classes or confounds has a None or
-# NaN value anywhere at the given index
+# Returns a boolean array that is true if either classes or confounds has a None
+# or NaN value anywhere at the given index
 def get_none_array(classes=None,confounds=None):
 	if classes is not None and confounds is not None:
 		assert(confounds.shape[1] == classes.shape[0])
 	elif classes is None:
 		classes = np.ones((confounds.shape[1],))
 	elif confounds is None:
 		confounds = np.ones((1,classes.shape[0]))
@@ -421,31 +500,16 @@
 # also forcing equal ratios between each class.
 
 def class_balance(classes,confounds,plim = 0.05,recurse=True,exclude_none=True,unique_classes = None):
 	classes = np.array(classes)
 	confounds = np.array(confounds)
 	if len(confounds) == 0:
 		confounds = np.ones((1,len(classes)),dtype=object)
-	#print(confounds)
 	ff = {}
-	'''
-	for i in range(confounds.shape[1]):
-		gg = str(classes[i]) + " " + str(confounds[1,i]) #+ " " + str(confounds[1,i])
-		if gg not in ff:
-			ff[gg] = gg
-			print(gg)
-	for i in range(confounds.shape[0]):
-		print(str(confounds[i,0]) + " is str: " + str(isinstance(confounds[i,0],str)))
-		print(np.unique(confounds[i,:]))
-		'''
-	
 	if exclude_none:
-		#print("classes shape " + str(classes.shape))
-		#print("confounds shape " + str(confounds.shape))
-		#print("classes[0] " + str(classes[0]))
 		has_none = get_none_array(classes,confounds)
 		confounds = confounds[:,~has_none]
 		classes = classes[~has_none]
 	else:
 		has_none = get_none_array(classes=None,confounds=confounds)
 		confounds[:,has_none] = "none"
 		has_none = get_none_array(classes=classes,confounds=None)
@@ -454,24 +518,22 @@
 	classes = np.array(classes)
 	if unique_classes is None:
 		try:
 			unique_classes = np.unique(classes)
 		except:
 			print(classes)
 			exit()
-		#print(unique_classes)
 	elif isinstance(unique_classes,list):
 		unique_classes = np.unique(unique_classes)
 	if not np.all(sorted(unique_classes) == list(range(len(unique_classes)))):
 		for i in range(len(classes)):
 			for j in range(len(unique_classes)):
 				if classes[i] == unique_classes[j]:
 					classes[i] = j
 					break
-	#print(classes)
 	n_buckets = [1 for x in range(confounds.shape[0])]
 	# Used for bucketing purposes
 	sorted_confounds = np.sort(confounds,axis=1)
 	# Automatically marks strings as discrete, giving each its own bucket
 	string_mapper = {}
 	unique_strs = []
 	for i in range(confounds.shape[0]):
@@ -480,31 +542,29 @@
 			unique_strs.append(u)
 			n_buckets[i] = len(u)
 	p_vals = [0 for x in range(confounds.shape[0])]
 	selection = np.ones(classes.shape,dtype=bool)
 	while min(p_vals) < plim and np.sum(selection) > 0:
 		primed = get_prime_form(confounds,n_buckets, sorted_confounds)
 		primed = np.prod(primed,axis=0,dtype=int)
-		selection = get_class_selection(classes,primed,unique_classes=unique_classes)
+		selection = get_class_selection(classes,
+										primed,
+										unique_classes=unique_classes)
 		rr = list(range(confounds.shape[0]))
 		random.shuffle(rr)
 		for i in rr:
-			#print("h " + str(i))
 			if not isinstance(confounds[i,0],str):
-				
-				ts = [confounds[i,np.logical_and(selection, classes == j)] for j in range(len(unique_classes))]
-				#print(ts)
-				# Makes sure there are at least five instances of each class remaining
-				if np.any(list(map(lambda k: len(k) < 5, ts))):# or len(ts) <= 1:
+				ts = [confounds[i,np.logical_and(selection, classes == j)] \
+					for j in range(len(unique_classes))]
+				# Makes sure there are at least five instances of 
+				# each class remaining
+				if np.any(list(map(lambda k: len(k) < 5, ts))):
 					selection = np.zeros(classes.shape,dtype=bool)
-					break
-				#print("HERE")
-				
+					break				
 				min_p,max_p = multi_mannwhitneyu(ts)
-				#print("%f %f" % (min_p,max_p))
 				p_vals[i] = min_p
 				if p_vals[i] < plim:
 					n_buckets[i] += 1
 					break
 			else:
 				p_vals[i] = 1
 	if np.sum(selection) > 40 and confounds[:,~selection].shape[1] > 0:
@@ -519,46 +579,44 @@
 def separate_set(selections,set_divisions = [0.5,0.5],IDs=None):
 	assert(isinstance(set_divisions,list))
 	set_divisions = [i/np.sum(set_divisions) for i in set_divisions]
 	rr = list(range(len(selections)))
 	random.shuffle(rr)
 	if IDs is None:
 		IDs = np.array(list(range(len(selections))))
-	#if len(IDs.shape) == 1:
-	#	IDs = np.expand_dims(IDs,0)
-	#print(IDs.shape)
-	#IDs = get_prime_form(IDs,[len(np.unique(IDs[x,:])) for x in range(IDs.shape[0])],np.sort(IDs,axis=1))
 	selections_ids = np.zeros(selections.shape,dtype=int)
 	totals = list(range(len(set_divisions)))
 	prime_hasher = {}
 	for i in rr:
 		if not selections[i]:
 			continue
 		is_none = IDs[i] == None or IDs[i] == "NULL"
 		if not is_none and IDs[i] in prime_hasher:
 			selections_ids[i] = prime_hasher[IDs[i]]
 			totals[selections_ids[i] - 1] += 1
 			continue
 		for j in range(len(set_divisions)):
-			if np.sum(totals) == 0 or totals[j] / np.sum(totals) < set_divisions[j]:
+			if np.sum(totals) == 0 or \
+				totals[j] / np.sum(totals) < set_divisions[j]:
 				break
 		selections_ids[i] = j+1
 		totals[j] += 1
 		if not is_none and IDs[i] not in prime_hasher:
 			prime_hasher[IDs[i]] = j + 1
 	return selections_ids
 
 def nifti_to_np(nifti_filepath,output_image_dim):
 	nifti_file = nb.load(nifti_filepath)
 	nifti_data = nifti_file.get_fdata()
 	nifti_data -= nifti_data.min()
 	m = nifti_data.max()
 	nifti_data = nifti_data / m
 	nifti_data = nifti_data.astype(np.float32)
-	zp = [output_image_dim[i]/nifti_data.shape[i] for i in range(len(output_image_dim))]
+	zp = [output_image_dim[i]/nifti_data.shape[i] \
+		for i in range(len(output_image_dim))]
 	nifti_data_zoomed = ndimage.zoom(nifti_data,zp)
 	return nifti_data_zoomed
 
 def str_to_list(s,nospace=False):
 	if s is None or s == "": return []
 	if s[0] == "[" and  s[-1] == "]":
 		s = s[1:-1]
@@ -567,23 +625,23 @@
 		s = s.split(",")
 		if nospace and "" in s: s.remove("")
 		return s
 	else:
 		return [s]
 
 def get_lr(optimizer):
-    for param_group in optimizer.param_groups:
-        return param_group['lr']
+	for param_group in optimizer.param_groups:
+		return param_group['lr']
 
 def parsedate(d,date_format="%Y-%m-%d %H:%M:%S",verbose=True):
 	try:
-		#for match in datefinder.find_dates(d.replace("_"," ")): return match
-		return datetime.datetime.strptime(d.replace("_"," ").split(".")[0],date_format)
+		return datetime.datetime.strptime(
+			d.replace("_"," ").split(".")[0],
+			date_format)
 	except ValueError:
-		#print("Bad date: %s" % d)
 		return parser.parse(d.replace("_"," "))
 
 def is_float(N):
 	try:
 		float(N)
 		return True
 	except:
@@ -665,21 +723,20 @@
 			set_arr[l] = set()
 		set_arr[l].add(i)
 	return [set_arr[_] for _ in set_arr]
 
 def determine_random_partition2(arr2d,labels):
 	assert(isinstance(arr2d,np.ndarray))
 	assert(isinstance(labels,np.ndarray))
-	G = nx.from_numpy_array(arr2d)#   (((arr2d - arr2d.min())/arr2d.max()))
+	G = nx.from_numpy_array(arr2d)
 	true_modularity = nx.community.modularity(G,label_to_community(labels))
 	return true_modularity
 	random_modularities = []
 	n_labels = np.sum(labels)
-	rand_labels = copy(labels)#np.zeros((labels.shape),dtype=bool)
-	#rand_labels[:n_labels] = True
+	rand_labels = copy(labels)
 	for i in range(200):
 		random.shuffle(rand_labels)
 		random_modularities.append(
 			nx.community.modularity(G,label_to_community(rand_labels))
 		)
 	random_modularities = np.sort(random_modularities)
 	index = np.searchsorted(random_modularities,true_modularity)
@@ -776,15 +833,18 @@
 				X_single = X_single.cpu().detach().numpy()
 				X_single = np.squeeze(X_single)
 		except:
 			print("Error")
 			selection[i] = 0
 			continue
 		if X is None:
-			X = np.zeros((len(filename_list),X_single.shape[1],X_single.shape[2]))
+			X = np.zeros(
+				(len(filename_list),
+				X_single.shape[1],
+				X_single.shape[2]))
 		X[i,...] = X_single
 		if test_variable is not None:
 			for j,t in enumerate(test_variable):
 				Y_strs[j][i] = str_to_list(all_vars.loc[f_key,t],nospace=True)
 			if confounds is not None:
 				for j,c in enumerate(confounds):
 					confound_strs[i][j] = all_vars.loc[f_key,c]
@@ -982,15 +1042,16 @@
 	
 	covars_df = all_vars
 	if verbose: print("len(covars): %d" % len(covars_df))
 	value_selection = np.ones((len(covars_df),),dtype=bool)
 	for ncv in non_confound_value_ranges:
 		if ncv in confounds_array:
 			print("confounds_array: %s" % str(confounds_array))
-			print("non_confound_value_ranges: %s" % str(non_confound_value_ranges))
+			print("non_confound_value_ranges: %s" % \
+				str(non_confound_value_ranges))
 			print("ncv: %s" % str(ncv))
 		assert(ncv not in confounds_array)
 		confounds_array.append(ncv)
 		value_ranges.append(non_confound_value_ranges[ncv])
 	confounds_array.append(test_variable)
 	value_ranges.append(test_value_ranges)
 	if verbose: print("confounds_array: %s" % str(confounds_array))
@@ -1033,31 +1094,23 @@
 		print("value_selection.shape: %s"%str(value_selection.shape))
 	covars_df = covars_df[value_selection]
 	covars_df = covars_df.sample(frac=1)
 	test_vars = covars_df[test_variable].to_numpy(dtype=np.dtype(object))
 	# If it's a string array, it just returns strings
 	test_vars = bucketize(test_vars,n_buckets)
 	ccc = {}
-	#for t in test_vars:
-	#	if t not in ccc: ccc[t] = 0
-	#	ccc[t] += 1
-	#for t in ccc: print("%s: %d" % (t,ccc[t]))
-	#assert(np.all([isinstance(i,str) for i in test_vars]))
 	if output_selection_savepath is not None and \
 			os.path.isfile(output_selection_savepath):
 		selection = np.load(output_selection_savepath)
 	else:
 		
 		if len(confounds_array) == 0:
 			if verbose: print(test_value_ranges)
-			#blanks = np.array(["" for _ in range(len(test_vars))])
-			#blanks = np.reshape(blanks,(1,blanks.shape[0]))
 			selection = class_balance(test_vars,[],
 				unique_classes=test_value_ranges,plim=0.1)
-			#selection = np.ones(test_vars.shape)
 		else:
 			selection = class_balance(test_vars,
 				covars_df[confounds_array].to_numpy(\
 					dtype=np.dtype(object)).T,
 				unique_classes=test_value_ranges,plim=0.1)
 		selection_ratios = recompute_selection_ratios(selection_ratios,
 			selection_limits,np.sum(selection))
@@ -1113,18 +1166,20 @@
 def parsedate(d,date_format="%Y-%m-%d %H:%M:%S"):
 	for match in datefinder.find_dates(d.replace("_"," ")): return match
 	return datetime.datetime.strptime(d.split(".")[0],date_format)
 
 def validate_all_vars(all_vars,args):
 	for c in args.confounds:
 		if c not in all_vars.columns:
-			raise Exception("Confound %s not in columns of %s"%(c,args.var_file))
+			raise Exception("Confound %s not in columns of %s"\
+				%(c,args.var_file))
 	
 	if args.label not in all_vars.columns:
-		raise Exception("Label %s not in columns of %s"%(args.label,args.var_file))
+		raise Exception("Label %s not in columns of %s"\
+			%(args.label,args.var_file))
 	
 	for index in all_vars.index:
 		if os.path.splitext(index)[1] != ".npy":
 			raise Exception(("Indices of %s must all be .npy files: "+\
 				"exception at index %s") % (args.var_file,index))
 
 def hidden_batch_predictions(
@@ -1141,41 +1196,53 @@
 	hidden_size = last_hidden_var.size()[1]
 	if ensemble:
 		ensemble_size = last_hidden_var.size()[2]
 	if ensemble:
 		if device is None:
 			hidden_batch = torch.zeros((batch_size,1,hidden_size,ensemble_size))
 		else:
-			hidden_batch = torch.zeros((batch_size,1,hidden_size,ensemble_size)).cuda(device)
+			hidden_batch = torch.zeros(
+					(batch_size,1,hidden_size,ensemble_size)
+				).cuda(device)
 	else:
 		if device is None:
 			hidden_batch = torch.zeros((batch_size,1,hidden_size))
 		else:
 			hidden_batch = torch.zeros((batch_size,1,hidden_size)).cuda(device)
 	preds = None
 	for i in range(batch_size):
 		hidden_batch[i,:] = last_hidden_var
 		if (i == 0 and group_vars[i] == last_icd) or \
 				(i > 0 and group_vars[i-1] != group_vars[i]):
 			if ensemble:
 				if device is None:
-					last_hidden_var = torch.zeros((1,1,hidden_size,ensemble_size))
+					last_hidden_var = torch.zeros(
+							(1,1,hidden_size,ensemble_size)
+						)
 				else: last_hidden_var = torch.zeros((1,1,hidden_size,ensemble_size)).cuda(device)
 			else:
 				if device is None:
 					last_hidden_var = torch.zeros((1,1,hidden_size))
-				else: last_hidden_var = torch.zeros((1,1,hidden_size)).cuda(device)
+				else: last_hidden_var = torch.zeros(
+										(1,1,hidden_size)).cuda(device)
 		#print(last_hidden_var.size())
-		if (ensemble and len(last_hidden_var.size()) == 3) or ((not ensemble) and len(last_hidden_var.size()) == 2):
+		if (ensemble and len(last_hidden_var.size()) == 3) or\
+			 ((not ensemble) and len(last_hidden_var.size()) == 2):
 			last_hidden_var = torch.unsqueeze(last_hidden_var,0)
 		with torch.no_grad():
-			out,last_hidden_var = model(torch.unsqueeze(X[i,...],0),last_hidden_var)
+			out,last_hidden_var = model(torch.unsqueeze(X[i,...],0),
+				last_hidden_var)
 		if preds is None:
-			if ensemble: preds = torch.zeros((batch_size,out.size()[1],out.size()[2],out.size()[3]))
-			else: preds = torch.zeros((batch_size,out.size()[1],out.size()[2]))
+			if ensemble: preds = torch.zeros((batch_size,
+									out.size()[1],
+									out.size()[2],
+									out.size()[3]))
+			else: preds = torch.zeros((batch_size,
+									out.size()[1],
+									out.size()[2]))
 		preds[i,...] = out
 	return preds,hidden_batch
 
 ## Outputs the test set evaluations
 
 def output_test(
 		args,
@@ -1184,16 +1251,16 @@
 		test_predictions_file,
 		mucran,
 		all_vars,
 		X_files = None,
 		return_Xfiles = False):
 	pred   = None
 	c_pred = None
-	Y      = None
-	C      = None
+	Y	  = None
+	C	  = None
 	cert   = None
 	results = {}
 	b = args.label
 	batch_size = args.batch_size
 	confounds = args.confounds
 	y_weight = args.y_weight
 	np.random.seed(0)
@@ -1201,46 +1268,45 @@
 		[X_files],_ = get_balanced_filename_list(b,[],
 			selection_ratios=[1],
 			total_size_limit=np.inf,
 			non_confound_value_ranges = test_val_ranges,
 			all_vars=all_vars)
 	temp = X_files
 	while len(X_files) > 0:
-		X_,Y_,C_,choice_arr,output_labels = get_data_from_filenames(X_files[:batch_size],
-			b,confounds=confounds,
-			return_as_strs = False,
-			unique_test_vals = None,return_choice_arr=True,all_vars=all_vars)
-		#YC_,YC_dud_ = YC_conv(Y_,C_,y_weight)
+		X_,Y_,C_,choice_arr,output_labels = get_data_from_filenames(
+					X_files[:batch_size],
+					b,confounds=confounds,
+					return_as_strs = False,
+					unique_test_vals = None,
+					return_choice_arr=True,
+					all_vars=all_vars)
 		YC_pred = mucran.predict(X_)
 		pred_ = np.mean(YC_pred[:,:y_weight,:],axis=1)
 		c_pred_ = YC_pred[:,y_weight:,:]
 		cert_ = None
 		####
 		if Y is None:
 			X = X_
 			Y = Y_
 			C = C_
 			pred = pred_
 			c_pred = c_pred_
 			cert = cert_
-			#X,Y,C,pred,c_pred,cert = X_,Y_,C_,pred_,c_pred_,cert_
 		else:
-			pred   = np.concatenate((pred,pred_),     axis=0)
+			pred   = np.concatenate((pred,pred_),	 axis=0)
 			c_pred = np.concatenate((c_pred,c_pred_), axis=0)
-			Y      = np.concatenate((Y,Y_),           axis=0)
-			C      = np.concatenate((C,C_),           axis=0)
-			#cert   = np.concatenate((cert,cert_),     axis=0)
+			Y	  = np.concatenate((Y,Y_),		   axis=0)
+			C	  = np.concatenate((C,C_),		   axis=0)
 		X_files = X_files[batch_size:]
 	X_files = temp
 	save_dict = {}
-	#print("cert.shape: %s" % str(cert.shape))
 	for i in range(Y.shape[0]):
 		X_file = X_files[i]
 		save_dict[X_file] = [[float(_) for _ in pred[i,:]],
-			[float(_) for _ in Y[i,:]]]#,float(cert[i])]
+			[float(_) for _ in Y[i,:]]]
 	json.dump(save_dict,open(test_predictions_file,'w'),indent=4)
 	pred_bin = np.zeros(Y.shape)
 	Y_bin = np.zeros(Y.shape)
 	for i in range(pred_bin.shape[0]):
 		pred_bin[i,np.argmax(pred[i,:Y.shape[1]])] = 1
 		Y_bin[i,np.argmax(Y[i,:])] = 1
 	roc_aucs = []
@@ -1256,31 +1322,29 @@
 		roc_aucs.append(roc_auc)
 		print("%s AUROC: %s" % (output_labels[i],str(roc_auc)))
 		results[b][output_labels[i]] = float(roc_auc)
 	results[b]["Mean AUROC"] = float(np.mean(roc_aucs))
 	
 	print("Mean AUROC: % s" % str(np.mean(roc_aucs)))
 	print("Y acc: %f" % results[b]["Y_acc"])
-	#print("Y AUROC: %s" % str(roc_auc))
-
 	print("+++")
 	print("MAX CONFOUND AUROCS")
 	for i in range(len(confounds)):
 		confound = confounds[i]
 		roc_aucs = []
 		roc_aucs_counts = []
 		for j in range(C.shape[2]):
 			if np.any(C[:,i,j] == 1):
 				fpr, tpr, threshold = roc_curve(C[:,i,j],c_pred[:,i,j])
 				roc_auc = auc(fpr, tpr)
 				if not is_nan(roc_auc):
-					#roc_aucs[roc_auc] = int(np.sum(C[:,i,j]))
 					roc_aucs.append(roc_auc)
 					roc_aucs_counts.append(int(np.sum(C[:,i,j])))
-		weighted_mean = np.sum([c1*c2 for c1,c2 in zip(roc_aucs,roc_aucs_counts)]) /\
+		weighted_mean = np.sum(
+				[c1*c2 for c1,c2 in zip(roc_aucs,roc_aucs_counts)]) /\
 				 np.sum(roc_aucs_counts)
 		try:
 			results[confound] = {}
 			if len(roc_aucs) == 0:
 				print("No AUCs for %s" % confound)
 			else:
 				mroc = int(np.argmax(roc_aucs))
@@ -1297,101 +1361,82 @@
 			print("Error in outputting %s" % confound)
 
 	json.dump(results,open(output_results,'w'),indent=4)
 	if return_Xfiles: return X_files
 
 
 def tensor2im(input_image, imtype=np.uint8):
-    """"Converts a Tensor array into a numpy image array.
+	""""Converts a Tensor array into a numpy image array.
 
-    Parameters:
-        input_image (tensor) --  the input image tensor array
-        imtype (type)        --  the desired type of the converted numpy array
-    """
-    if not isinstance(input_image, np.ndarray):
-        if isinstance(input_image, torch.Tensor):  # get the data from a variable
-            image_tensor = input_image.data
-        else:
-            return input_image
-        image_numpy = image_tensor[0].cpu().float().numpy()  # convert it into a numpy array
-        if image_numpy.shape[0] == 1:  # grayscale to RGB
-            image_numpy = np.tile(image_numpy, (3, 1, 1))
-        image_numpy = (np.transpose(image_numpy, (1, 2, 0)) + 1) / 2.0 * 255.0  # post-processing: tranpose and scaling
-    else:  # if it is a numpy array, do nothing
-        image_numpy = input_image
-    return image_numpy.astype(imtype)
+	Parameters:
+		input_image (tensor) --  the input image tensor array
+		imtype (type)		--  the desired type of the converted numpy array
+	"""
+	if not isinstance(input_image, np.ndarray):
+		if isinstance(input_image, torch.Tensor): # get the data from a variable
+			image_tensor = input_image.data
+		else:
+			return input_image
+		# convert it into a numpy array
+		image_numpy = image_tensor[0].cpu().float().numpy()
+		if image_numpy.shape[0] == 1:  # grayscale to RGB
+			image_numpy = np.tile(image_numpy, (3, 1, 1))
+		# post-processing: tranpose and scaling
+		image_numpy = (np.transpose(image_numpy, (1, 2, 0)) + 1) / 2.0 * 255.0
+	else:
+		# if it is a numpy array, do nothing
+		image_numpy = input_image
+	return image_numpy.astype(imtype)
 
 
 def diagnose_network(net, name='network'):
-    """Calculate and print the mean of average absolute(gradients)
+	"""Calculate and print the mean of average absolute(gradients)
 
-    Parameters:
-        net (torch network) -- Torch network
-        name (str) -- the name of the network
-    """
-    mean = 0.0
-    count = 0
-    for param in net.parameters():
-        if param.grad is not None:
-            mean += torch.mean(torch.abs(param.grad.data))
-            count += 1
-    if count > 0:
-        mean = mean / count
-    print(name)
-    print(mean)
+	Parameters:
+		net (torch network) -- Torch network
+		name (str) -- the name of the network
+	"""
+	mean = 0.0
+	count = 0
+	for param in net.parameters():
+		if param.grad is not None:
+			mean += torch.mean(torch.abs(param.grad.data))
+			count += 1
+	if count > 0:
+		mean = mean / count
+	print(name)
+	print(mean)
 
 
 def save_image(image_numpy, image_path, aspect_ratio=1.0):
-    """Save a numpy image to the disk
+	"""Save a numpy image to the disk
 
-    Parameters:
-        image_numpy (numpy array) -- input numpy array
-        image_path (str)          -- the path of the image
-    """
-
-    image_pil = Image.fromarray(image_numpy)
-    h, w, _ = image_numpy.shape
-
-    if aspect_ratio > 1.0:
-        image_pil = image_pil.resize((h, int(w * aspect_ratio)), Image.BICUBIC)
-    if aspect_ratio < 1.0:
-        image_pil = image_pil.resize((int(h / aspect_ratio), w), Image.BICUBIC)
-    image_pil.save(image_path)
+	Parameters:
+		image_numpy (numpy array) -- input numpy array
+		image_path (str)		  -- the path of the image
+	"""
+
+	image_pil = Image.fromarray(image_numpy)
+	h, w, _ = image_numpy.shape
+
+	if aspect_ratio > 1.0:
+		image_pil = image_pil.resize((h, int(w * aspect_ratio)), Image.BICUBIC)
+	if aspect_ratio < 1.0:
+		image_pil = image_pil.resize((int(h / aspect_ratio), w), Image.BICUBIC)
+	image_pil.save(image_path)
 
 
 def print_numpy(x, val=True, shp=False):
-    """Print the mean, min, max, median, std, and size of a numpy array
+	"""Print the mean, min, max, median, std, and size of a numpy array
 
-    Parameters:
-        val (bool) -- if print the values of the numpy array
-        shp (bool) -- if print the shape of the numpy array
-    """
-    x = x.astype(np.float64)
-    if shp:
-        print('shape,', x.shape)
-    if val:
-        x = x.flatten()
-        print('mean = %3.3f, min = %3.3f, max = %3.3f, median = %3.3f, std=%3.3f' % (
-            np.mean(x), np.min(x), np.max(x), np.median(x), np.std(x)))
-
-
-def mkdirs(paths):
-    """create empty directories if they don't exist
-
-    Parameters:
-        paths (str list) -- a list of directory paths
-    """
-    if isinstance(paths, list) and not isinstance(paths, str):
-        for path in paths:
-            mkdir(path)
-    else:
-        mkdir(paths)
-
-
-def mkdir(path):
-    """create a single empty directory if it didn't exist
-
-    Parameters:
-        path (str) -- a single directory path
-    """
-    if not os.path.exists(path):
-        os.makedirs(path)
+	Parameters:
+		val (bool) -- if print the values of the numpy array
+		shp (bool) -- if print the shape of the numpy array
+	"""
+	x = x.astype(np.float64)
+	if shp:
+		print('shape,', x.shape)
+	if val:
+		x = x.flatten()
+		print(('mean = %3.3f, min = %3.3f, "+\
+			"max = %3.3f, median = %3.3f, std=%3.3f') % (
+			np.mean(x), np.min(x), np.max(x), np.median(x), np.std(x)))
```

### Comparing `multi_med_image_ml-0.0.0/pyproject.toml` & `multi_med_image_ml-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.0"
+version = "0.0.1"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
@@ -15,15 +15,16 @@
   "pillow",
   "nibabel",
   "datefinder",
   "monai",
   "dicom2nifti",
   "dateutil",
   "sklearn",
-  "pydicom"
+  "pydicom",
+  "dcm2niix"
 ]
 requires-python = ">=3.8"
 
 authors = [
   {name = "Matt Leming", email = "mleming@mgh.harvard.edu"}
 ]
 maintainers = [
```

