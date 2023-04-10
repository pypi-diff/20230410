# Comparing `tmp/bpnet_lite-0.2.0-py3-none-any.whl.zip` & `tmp/bpnet_lite-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,18 @@
-Zip file size: 19652 bytes, number of entries: 12
--rwxr-xr-x  2.0 unx     7005 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.data/scripts/bpnet
--rw-r--r--  2.0 unx      140 b- defN 21-Dec-01 23:09 bpnetlite/__init__.py
--rw-r--r--  2.0 unx     7450 b- defN 22-May-05 04:43 bpnetlite/attributions.py
--rw-r--r--  2.0 unx     9063 b- defN 22-Jun-07 00:11 bpnetlite/bpnet.py
--rw-r--r--  2.0 unx    16233 b- defN 22-Sep-09 22:10 bpnetlite/io.py
+Zip file size: 29969 bytes, number of entries: 16
+-rwxr-xr-x  2.0 unx     8723 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.data/scripts/bpnet
+-rwxr-xr-x  2.0 unx     8649 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.data/scripts/chrombpnet
+-rw-r--r--  2.0 unx      175 b- defN 23-Apr-10 16:26 bpnetlite/__init__.py
+-rw-r--r--  2.0 unx    10712 b- defN 23-Mar-23 21:47 bpnetlite/attributions.py
+-rw-r--r--  2.0 unx    15776 b- defN 23-Feb-26 20:40 bpnetlite/bpnet.py
+-rw-r--r--  2.0 unx     5827 b- defN 23-Feb-26 21:40 bpnetlite/chrombpnet.py
+-rw-r--r--  2.0 unx    17015 b- defN 22-Nov-17 02:16 bpnetlite/io.py
+-rw-r--r--  2.0 unx     1643 b- defN 22-Oct-24 22:28 bpnetlite/logging.py
 -rw-r--r--  2.0 unx     2418 b- defN 22-May-03 00:14 bpnetlite/losses.py
+-rw-r--r--  2.0 unx     3674 b- defN 23-Jan-20 02:13 bpnetlite/marginalize.py
 -rw-r--r--  2.0 unx    13599 b- defN 22-May-04 18:11 bpnetlite/performance.py
--rw-r--r--  2.0 unx     1072 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      530 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      957 b- defN 22-Sep-12 17:01 bpnet_lite-0.2.0.dist-info/RECORD
-12 files, 58569 bytes uncompressed, 18056 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      533 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1294 b- defN 23-Apr-10 16:26 bpnet_lite-0.3.0.dist-info/RECORD
+16 files, 91212 bytes uncompressed, 27855 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,37 +1,49 @@
-Filename: bpnet_lite-0.2.0.data/scripts/bpnet
+Filename: bpnet_lite-0.3.0.data/scripts/bpnet
+Comment: 
+
+Filename: bpnet_lite-0.3.0.data/scripts/chrombpnet
 Comment: 
 
 Filename: bpnetlite/__init__.py
 Comment: 
 
 Filename: bpnetlite/attributions.py
 Comment: 
 
 Filename: bpnetlite/bpnet.py
 Comment: 
 
+Filename: bpnetlite/chrombpnet.py
+Comment: 
+
 Filename: bpnetlite/io.py
 Comment: 
 
+Filename: bpnetlite/logging.py
+Comment: 
+
 Filename: bpnetlite/losses.py
 Comment: 
 
+Filename: bpnetlite/marginalize.py
+Comment: 
+
 Filename: bpnetlite/performance.py
 Comment: 
 
-Filename: bpnet_lite-0.2.0.dist-info/LICENSE
+Filename: bpnet_lite-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: bpnet_lite-0.2.0.dist-info/METADATA
+Filename: bpnet_lite-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bpnet_lite-0.2.0.dist-info/WHEEL
+Filename: bpnet_lite-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bpnet_lite-0.2.0.dist-info/top_level.txt
+Filename: bpnet_lite-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bpnet_lite-0.2.0.dist-info/RECORD
+Filename: bpnet_lite-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bpnetlite/__init__.py

```diff
@@ -1,7 +1,8 @@
 # bpnet-lite
 # Author: Jacob Schreiber
 # Code adapted from Avanti Shrikumar and Ziga Avsec
 
 from .bpnet import BPNet
+from .chrombpnet import ChromBPNet
 
-__version__ = '0.1.1'
+__version__ = '0.3.0'
```

## bpnetlite/attributions.py

```diff
@@ -1,17 +1,20 @@
 # attributions.py
 # Author: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import numpy
 import numba
 import torch
+import pandas
+import logomaker
 
 from tqdm import trange
 from captum.attr import DeepLiftShap
 
+
 class ProfileWrapper(torch.nn.Module):
 	"""A wrapper class that returns transformed profiles.
 
 	This class takes in a trained model and returns the weighted softmaxed
 	outputs of the first dimension. Specifically, it takes the predicted
 	"logits" and takes the dot product between them and the softmaxed versions
 	of those logits. This is for convenience when using captum to calculate
@@ -26,18 +29,20 @@
 	def __init__(self, model):
 		super(ProfileWrapper, self).__init__()
 		self.model = model
 
 	def forward(self, X, X_ctl=None, **kwargs):
 		logits = self.model(X, X_ctl, **kwargs)[0]
 		logits = logits.reshape(X.shape[0], -1)
-		
-		y = torch.nn.functional.log_softmax(logits, dim=-1)
-		y = torch.exp(y)
-		return (logits * y).sum(axis=-1).unsqueeze(-1)
+		logits = logits - torch.mean(logits, dim=-1, keepdims=True)
+		l = torch.clone(logits).detach()
+
+		y = torch.exp(l - torch.logsumexp(l, dim=-1, keepdims=True))
+		return (logits * y).sum(axis=-1, keepdims=True)
+
 
 class CountWrapper(torch.nn.Module):
 	"""A wrapper class that only returns the predicted counts.
 
 	This class takes in a trained model and returns only the second output.
 	For BPNet models, this means that it is only returning the count
 	predictions. This is for convenience when using captum to calculate
@@ -52,14 +57,60 @@
 	def __init__(self, model):
 		super(CountWrapper, self).__init__()
 		self.model = model
 
 	def forward(self, X, X_ctl=None, **kwargs):
 		return self.model(X, X_ctl, **kwargs)[1]
 
+
+def hypothetical_attributions(multipliers, inputs, baselines):
+    """A function for aggregating contributions into hypothetical attributions.
+
+    When handling categorical data, like one-hot encodings, the attributions
+    returned by a method like DeepLIFT/SHAP may need to be modified slightly.
+    Specifically, one needs to account for each nucleotide change actually
+    being the addition of one category AND the subtraction of another category.
+    Basically, once you've calculated the multipliers, you need to subtract
+    out the contribution of the nucleotide actually present and then add in
+    the contribution of the nucleotide you are becomming.
+
+    These values are then averaged over all references.
+
+
+    Parameters
+    ----------
+    multipliers: torch.tensor, shape=(n_baselines, 4, length)
+    	The multipliers determined by DeepLIFT
+
+    inputs: torch.tensor, shape=(n_baselines, 4, length)
+    	The one-hot encoded sequence being explained, copied several times.
+
+    baselines: torch.tensor, shape=(n_baselines, 4, length)
+    	The one-hot encoded baseline sequences.
+
+
+    Returns
+    -------
+	projected_contribs: torch.tensor, shape=(1, 4, length)
+		The attribution values for each nucleotide in the input.
+	"""
+
+    projected_contribs = torch.zeros_like(baselines[0], dtype=baselines[0].dtype)
+    
+    for i in range(inputs[0].shape[1]):
+        hypothetical_input = torch.zeros_like(inputs[0], dtype=baselines[0].dtype)
+        hypothetical_input[:, i] = 1.0
+        hypothetical_diffs = hypothetical_input - baselines[0]
+        hypothetical_contribs = hypothetical_diffs * multipliers[0]
+        
+        projected_contribs[:, i] = torch.sum(hypothetical_contribs, dim=1)
+    
+    return (projected_contribs,)
+
+
 @numba.jit('void(int64, int64[:], int64[:], int32[:, :], int32[:,], int32[:, :], float32[:, :, :])')
 def _fast_shuffle(n_shuffles, chars, idxs, next_idxs, next_idxs_counts, counters, shuffled_sequences):
 	"""An internal function for fast shuffling using numba."""
 
 	for i in range(n_shuffles):
 		for char in chars:
 			n = next_idxs_counts[char]
@@ -138,23 +189,25 @@
 		counters, shuffled_sequences)
 	
 	shuffled_sequences = torch.from_numpy(shuffled_sequences)
 	return shuffled_sequences
 
 
 def calculate_attributions(model, X, args=None, model_output="profile", 
-	hypothetical=False, n_shuffles=20, verbose=False, random_state=None):
+	hypothetical=False, n_shuffles=20, return_references=False, verbose=False, 
+	random_state=None):
 	"""Calculate attributions using DeepLift/Shap and a given model. 
 
 	This function will calculate DeepLift/Shap attributions on a set of
 	sequences. It assumes that the model returns "logits" in the first output,
 	not softmax probabilities, and count predictions in the second output.
 	It will create GC-matched negatives to use as a reference and proceed
 	using the given batch size.
 
+
 	Parameters
 	----------
 	model: torch.nn.Module
 		The model to use, either BPNet or one of it's variants.
 
 	X: torch.tensor, shape=(-1, 4, -1)
 		A one-hot encoded sequence input to the model.
@@ -178,46 +231,96 @@
 	n_shuffles: int, optional
 		The number of dinucleotide shuffles to return. Default is 10.
 
 	batch_size: int, optional
 		The number of attributions to calculate at the same time. This is
 		limited by GPU memory. Default is 8.
 
+	return_references: bool, optional
+		Whether to return the references that were generated during this
+		process.
+
 	verbose: bool, optional
 		Whether to display a progress bar.
 
 	random_state: int or None or numpy.random.RandomState, optional
 		The random seed to use to ensure determinism. If None, the
 		process is not deterministic. Default is None. 
+
+
+	Returns
+	-------
+	attributions: torch.tensor
+		The attributions calculated for each input sequence, with the same
+		shape as the input sequences.
+
+	references: torch.tensor, optional
+		The references used for each input sequence, with the shape
+		(n_input_sequences, n_shuffles, 4, length). Only returned if
+		`return_references = True`. 
 	"""
 
 	if model_output == "profile":
 		wrapper = ProfileWrapper(model)
 	elif model_output == "count":
 		wrapper = CountWrapper(model)
 	else:
 		raise ValueError("model_output must be one of 'profile' or 'count'.")
 
 	ig = DeepLiftShap(wrapper)
 	
 	attributions = []
+	references = []
 	with torch.no_grad():
 		for i in trange(len(X), disable=not verbose):
 			X_ = X[i:i+1]
 			reference = dinucleotide_shuffle(X_[0], n_shuffles=n_shuffles, 
 				random_state=random_state).cuda()
+
 			X_ = X_.cuda()
 
 			if args is None:
 				args_ = None
 			else:
 				args_ = tuple([arg[i:i+1].cuda() for arg in args])
 						
-			attr = ig.attribute(X_, reference, target=0, additional_forward_args=args_)
+			attr = ig.attribute(X_, reference, target=0, 
+				additional_forward_args=args_, 
+				custom_attribution_func=hypothetical_attributions)
 
 			if not hypothetical:
 				attr = (attr * X_)
 			
+			if return_references:
+				references.append(reference.unsqueeze(0))
+
 			attributions.append(attr.cpu())
 	
-	attributions = torch.cat(attributions)    
-	return attributions
+	attributions = torch.cat(attributions)
+
+	if return_references:
+		return attributions, torch.cat(references)
+	return attributions
+
+
+def plot_attributions(X_attr, ax):
+	"""Plot the attributions using logomaker.
+
+	Takes in a matrix of attributions and plots the attribution-weighted
+	sequence using logomaker. This is a convenience function.
+
+
+	Parameters
+	----------
+	X_attr: torch.tensor, shape=(4, -1)
+		A tensor of the attributions. Can be either the hypothetical
+		attributions, where the entire matrix has values, or the projected
+		attributions, where only the actual bases have their attributions
+		stored, i.e., 3 values per column are zero.
+	"""
+
+	df = pandas.DataFrame(X_attr.T, columns=['A', 'C', 'G', 'T'])
+	df.index.name = 'pos'
+	
+	logo = logomaker.Logo(df, ax=ax)
+	logo.style_spines(visible=False)
+	return logo
```

## bpnetlite/bpnet.py

```diff
@@ -3,26 +3,30 @@
 
 """
 This module contains a reference implementation of BPNet that can be used
 or adapted for your own circumstances. The implementation takes in a
 stranded control track and makes predictions for stranded outputs.
 """
 
+import h5py
 import time 
 import numpy
 import torch
 
 from .losses import MNLLLoss
 from .losses import log1pMSELoss
 
 from .performance import pearson_corr
 from .performance import calculate_performance_measures
 
+from .logging import Logger
+
 torch.backends.cudnn.benchmark = True
 
+
 class BPNet(torch.nn.Module):
 	"""A basic BPNet model with stranded profile and total count prediction.
 
 	This is a reference implementation for BPNet. The model takes in
 	one-hot encoded sequence, runs it through: 
 
 	(1) a single wide convolution operation 
@@ -58,117 +62,184 @@
 	two strands are concatenated together, a log softmax is applied,
 	and the MNLL loss is calculated on the concatenation. 
 
 	(4) The count prediction task is predicting the total counts across
 	both strands. The counts are then distributed across strands according
 	to the single log softmax from 3.
 
+	Note that this model is also used as components in the ChromBPNet model,
+	as both the bias model and the accessibility model. Both components are
+	the same BPNet architecture but trained on different loci.
+
+
 	Parameters
 	----------
 	n_filters: int, optional
 		The number of filters to use per convolution. Default is 64.
 
 	n_layers: int, optional
 		The number of dilated residual layers to include in the model.
 		Default is 8.
 
 	n_outputs: int, optional
 		The number of profile outputs from the model. Generally either 1 or 2 
 		depending on if the data is unstranded or stranded. Default is 2.
 
+	n_control_tracks: int, optional
+		The number of control tracks to feed into the model. When predicting
+		TFs, this is usually 2. When predicting accessibility, this is usualy
+		0. When 0, this input is removed from the model. Default is 2.
+
 	alpha: float, optional
 		The weight to put on the count loss.
 
+	profile_output_bias: bool, optional
+		Whether to include a bias term in the final profile convolution.
+		Removing this term can help with attribution stability and will usually
+		not affect performance. Default is True.
+
+	count_output_bias: bool, optional
+		Whether to include a bias term in the linear layer used to predict
+		counts. Removing this term can help with attribution stability but
+		may affect performance. Default is True.
+
 	name: str or None, optional
 		The name to save the model to during training.
 
 	trimming: int or None, optional
 		The amount to trim from both sides of the input window to get the
 		output window. This value is removed from both sides, so the total
 		number of positions removed is 2*trimming.
+
+	verbose: bool, optional
+		Whether to display statistics during training. Setting this to False
+		will still save the file at the end, but does not print anything to
+		screen during training. Default is True.
 	"""
 
 	def __init__(self, n_filters=64, n_layers=8, n_outputs=2, 
 		n_control_tracks=2, alpha=1, profile_output_bias=True, 
-		count_output_bias=True, name=None, trimming=None):
+		count_output_bias=True, name=None, trimming=None, verbose=True):
 		super(BPNet, self).__init__()
 		self.n_filters = n_filters
 		self.n_layers = n_layers
 		self.n_outputs = n_outputs
 		self.n_control_tracks = n_control_tracks
 
 		self.alpha = alpha
 		self.name = name or "bpnet.{}.{}".format(n_filters, n_layers)
 		self.trimming = trimming or 2 ** n_layers
 
 		self.iconv = torch.nn.Conv1d(4, n_filters, kernel_size=21, padding=10)
+		self.irelu = torch.nn.ReLU()
 
 		self.rconvs = torch.nn.ModuleList([
 			torch.nn.Conv1d(n_filters, n_filters, kernel_size=3, padding=2**i, 
 				dilation=2**i) for i in range(1, self.n_layers+1)
 		])
+		self.rrelus = torch.nn.ModuleList([
+			torch.nn.ReLU() for i in range(1, self.n_layers+1)
+		])
 
-		self.fconv = torch.nn.Conv1d(n_filters+n_control_tracks, n_outputs, kernel_size=75, 
-			padding=37, bias=profile_output_bias)
+		self.fconv = torch.nn.Conv1d(n_filters+n_control_tracks, n_outputs, 
+			kernel_size=75, padding=37, bias=profile_output_bias)
 		
 		n_count_control = 1 if n_control_tracks > 0 else 0
 		self.linear = torch.nn.Linear(n_filters+n_count_control, 1, 
 			bias=count_output_bias)
 
+		self.logger = Logger(["Epoch", "Iteration", "Training Time",
+			"Validation Time", "Training MNLL", "Training Count MSE", 
+			"Validation MNLL", "Validation Profile Pearson", 
+			"Validation Count Pearson", "Validation Count MSE", "Saved?"], 
+			verbose=verbose)
+
+
 	def forward(self, X, X_ctl=None):
 		"""A forward pass of the model.
 
 		This method takes in a nucleotide sequence X, a corresponding
 		per-position value from a control track, and a per-locus value
 		from the control track and makes predictions for the profile 
 		and for the counts. This per-locus value is usually the
 		log(sum(X_ctl_profile)+1) when the control is an experimental
 		read track but can also be the output from another model.
 
 		Parameters
 		----------
-		X: torch.tensor, shape=(batch_size, 4, sequence_length)
+		X: torch.tensor, shape=(batch_size, 4, length)
 			The one-hot encoded batch of sequences.
 
-		X_ctl: torch.tensor, shape=(batch_size, n_strands, sequence_length)
-			A value representing the signal of the control at each position in the
-			sequence.
+		X_ctl: torch.tensor or None, shape=(batch_size, n_strands, length)
+			A value representing the signal of the control at each position in 
+			the sequence. If no controls, pass in None. Default is None.
 
 		Returns
 		-------
 		y_profile: torch.tensor, shape=(batch_size, n_strands, out_length)
-			The output predictions for each strand.
+			The output predictions for each strand trimmed to the output
+			length.
 		"""
 
 		start, end = self.trimming, X.shape[2] - self.trimming
 
-		X = torch.nn.ReLU()(self.iconv(X))
+		X = self.irelu(self.iconv(X))
 		for i in range(self.n_layers):
-			X_conv = torch.nn.ReLU()(self.rconvs[i](X))
+			X_conv = self.rrelus[i](self.rconvs[i](X))
 			X = torch.add(X, X_conv)
 
 		if X_ctl is None:
 			X_w_ctl = X
 		else:
 			X_w_ctl = torch.cat([X, X_ctl], dim=1)
 
 		y_profile = self.fconv(X_w_ctl)[:, :, start:end]
 
 		# counts prediction
-		X = torch.mean(X[:, :, start-37:end+37], axis=2)
+		X = torch.mean(X[:, :, start-37:end+37], dim=2)
 
 		if X_ctl is not None:
-			X_ctl = torch.sum(X_ctl[:, :, start-37:end+37], axis=(1, 2))
+			X_ctl = torch.sum(X_ctl[:, :, start-37:end+37], dim=(1, 2))
 			X_ctl = X_ctl.unsqueeze(-1)
 			X = torch.cat([X, torch.log(X_ctl+1)], dim=-1)
 
 		y_counts = self.linear(X).reshape(X.shape[0], 1)
 		return y_profile, y_counts
 
+
 	def predict(self, X, X_ctl=None, batch_size=64):
+		"""Make predictions for a large number of examples.
+
+		This method will make predictions for a number of examples that exceed
+		the batch size. It is similar to the forward method in terms of inputs 
+		and outputs, but will run wrapped with `torch.no_grad()` to speed up
+		computation and prevent information leakage into the model.
+
+
+		Parameters
+		----------
+		X: torch.tensor, shape=(-1, 4, length)
+			The one-hot encoded batch of sequences.
+
+		X_ctl: torch.tensor or None, shape=(-1, n_strands, length)
+			A value representing the signal of the control at each position in 
+			the sequence. If no controls, pass in None. Default is None.
+
+		batch_size: int, optional
+			The number of examples to run at a time. Default is 64.
+
+
+		Returns
+		-------
+		y_profile: torch.tensor, shape=(-1, n_strands, out_length)
+			The output predictions for each strand trimmed to the output
+			length.
+		"""
+
+
 		with torch.no_grad():
 			starts = numpy.arange(0, X.shape[0], batch_size)
 			ends = starts + batch_size
 
 			y_profiles, y_counts = [], []
 			for start, end in zip(starts, ends):
 				X_batch = X[start:end].cuda()
@@ -181,34 +252,83 @@
 				y_profiles.append(y_profiles_)
 				y_counts.append(y_counts_)
 
 			y_profiles = torch.cat(y_profiles)
 			y_counts = torch.cat(y_counts)
 			return y_profiles, y_counts
 
-	def fit_generator(self, training_data, optimizer, X_valid=None, 
-		X_ctl_valid=None, y_valid=None, max_epochs=100, batch_size=64, 
-		validation_iter=100, verbose=True):
+
+	def fit(self, training_data, optimizer, X_valid=None, X_ctl_valid=None, 
+		y_valid=None, max_epochs=100, batch_size=64, validation_iter=100, 
+		verbose=True):
+		"""Fit the model to data and validate it periodically.
+
+		This method controls the training of a BPNet model. It will fit the
+		model to examples generated by the `training_data` DataLoader object
+		and, if validation data is provided, will periodically validate the
+		model against it and return those values. The periodicity can be
+		controlled using the `validation_iter` parameter.
+
+		Two versions of the model will be saved: the best model found during
+		training according to the validation measures, and the final model
+		at the end of training. Additionally, a log will be saved of the
+		training and validation statistics, e.g. time and performance.
+
+
+		Parameters
+		----------
+		training_data: torch.utils.data.DataLoader
+			A generator that produces examples to train on. If n_control_tracks
+			is greater than 0, must product two inputs, otherwise must produce
+			only one input.
+
+		optimizer: torch.optim.Optimizer
+			An optimizer to control the training of the model.
+
+		X_valid: torch.tensor or None, shape=(n, 4, 2114)
+			A block of sequences to validate on periodically. If None, do not
+			perform validation. Default is None.
+
+		X_ctl_valid: torch.tensor or None, shape=(n, n_control_tracks, 2114)
+			A block of control sequences to validate on periodically. If
+			n_control_tracks is None, pass in None. Default is None.
+
+		y_valid: torch.tensor or None, shape=(n, n_outputs, 1000)
+			A block of signals to validate against. Must be provided if
+			X_valid is also provided. Default is None.
+
+		max_epochs: int
+			The maximum number of epochs to train for, as measured by the
+			number of times that `training_data` is exhausted. Default is 100.
+
+		batch_size: int
+			The number of examples to include in each batch. Default is 64.
+
+		validation_iter: int
+			The number of batches to train on before validating against the
+			entire validation set. When the validation set is large, this
+			enables the total validating time to be small compared to the
+			training time by only validating periodically. Default is 100.
+
+		verbose: bool
+			Whether to print out the training and evaluation statistics during
+			training. Default is True.
+		"""
 
 		if X_valid is not None:
 			X_valid = X_valid.cuda()
-			y_valid_counts = y_valid.sum(axis=2)
+			y_valid_counts = y_valid.sum(dim=2)
 
 		if X_ctl_valid is not None:
 			X_ctl_valid = X_ctl_valid.cuda()
 
-		columns = "Epoch\tIteration\tTraining Time\tValidation Time\t"
-		columns += "T MNLL\tT Count log1pMSE\t"
-		columns += "V MNLL\tV Profile Pearson\tV Count Pearson\tV Count log1pMSE"
-		columns += "\tSaved?"
-		if verbose:
-			print(columns)
 
 		iteration = 0
 		best_loss = float("inf")
+		self.logger.start()
 
 		for epoch in range(max_epochs):
 			tic = time.time()
 
 			for data in training_data:
 				if len(data) == 3:
 					X, X_ctl, y = data
@@ -247,44 +367,117 @@
 					train_time = time.time() - tic
 
 					with torch.no_grad():
 						self.eval()
 
 						tic = time.time()
 						y_profile, y_counts = self.predict(X_valid, X_ctl_valid)
-						valid_time = time.time() - tic
 
 						z = y_profile.shape
 						y_profile = y_profile.reshape(y_profile.shape[0], -1)
 						y_profile = torch.nn.functional.log_softmax(y_profile, dim=-1)
 						y_profile = y_profile.reshape(*z)
 
 						measures = calculate_performance_measures(y_profile, 
 							y_valid, y_counts, kernel_sigma=7, 
 							kernel_width=81, measures=['profile_mnll', 
 							'profile_pearson', 'count_pearson', 'count_mse'])
 
-						line = "{}\t{}\t{:4.4}\t{:4.4}\t".format(epoch, iteration,
-							train_time, valid_time)
-
-						line += "{:4.4}\t{:4.4}\t".format(profile_loss_, 
-							count_loss_)
+						profile_corr = measures['profile_pearson']
+						count_corr = measures['count_pearson']
+						
+						valid_loss = measures['profile_mnll'].mean()
+						valid_loss += self.alpha * measures['count_mse'].mean()
+						valid_time = time.time() - tic
 
-						line += "{:4.4}\t{:4.4}\t{:4.4}\t{:4.4}".format(
-							measures['profile_mnll'].mean(), 
-							numpy.nan_to_num(measures['profile_pearson']).mean(),
-							numpy.nan_to_num(measures['count_pearson']).mean(), 
-							measures['count_mse'].mean()
-						)
+						self.logger.add([epoch, iteration, train_time, 
+							valid_time, profile_loss_, count_loss_, 
+							measures['profile_mnll'].mean().item(), 
+							numpy.nan_to_num(profile_corr).mean(),
+							numpy.nan_to_num(count_corr).mean(), 
+							measures['count_mse'].mean().item(),
+							(valid_loss < best_loss).item()])
 
-						valid_loss = measures['profile_mnll'].mean() + self.alpha * measures['count_mse'].mean()
-						line += "\t{}".format(valid_loss < best_loss)
+						self.logger.save("{}.log".format(self.name))
 
 						if valid_loss < best_loss:
 							torch.save(self, "{}.torch".format(self.name))
 							best_loss = valid_loss
-					
-						print(line)
 
 				iteration += 1
 
 		torch.save(self, "{}.final.torch".format(self.name))
+
+
+	@classmethod
+	def from_chrombpnet_lite(cls, filename):
+		"""Loads a model from ChromBPNet-lite TensorFlow format.
+	
+		This method will load a ChromBPNet-lite model from TensorFlow format.
+		Note that this is not the same as ChromBPNet format. Specifically,
+		ChromBPNet-lite was a preceeding package that had a slightly different
+		saving format, whereas ChromBPNet is the packaged version of that
+		code that is applied at scale.
+
+		This method does not load the entire ChromBPNet model. If that is
+		the desired behavior, see the `ChromBPNet` object and its associated
+		loading functions. Instead, this loads a single BPNet model -- either
+		the bias model or the accessibility model, depending on what is encoded
+		in the stored file.
+
+
+		Parameters
+		----------
+		filename: str
+			The name of the h5 file that stores the trained model parameters.
+
+
+		Returns
+		-------
+		model: BPNet
+			A BPNet model compatible with this repository in PyTorch.
+		"""
+
+		h5 = h5py.File(filename, "r")
+		w = h5['model_weights']
+
+		if 'model_1' in w.keys():
+			w = w['model_1']
+			bias = False
+		else:
+			bias = True
+
+		k, b = 'kernel:0', 'bias:0'
+		name = "conv1d_{}_1" if not bias else "conv1d_{0}/conv1d_{0}"
+
+		layer_names = []
+		for layer_name in w.keys():
+			try:
+				idx = int(layer_name.split("_")[1])
+				layer_names.append(idx)
+			except:
+				pass
+
+		n_filters = w[name.format(1)][k].shape[2]
+		n_layers = max(layer_names) - 2
+
+		model = BPNet(n_layers=n_layers, n_filters=n_filters, n_outputs=1,
+			n_control_tracks=0, trimming=(2114-1000)//2)
+
+		convert_w = lambda x: torch.nn.Parameter(torch.tensor(
+			x[:]).permute(2, 1, 0))
+		convert_b = lambda x: torch.nn.Parameter(torch.tensor(x[:]))
+
+		model.iconv.weight = convert_w(w[name.format(1)][k])
+		model.iconv.bias = convert_b(w[name.format(1)][b])
+
+		for i in range(2, n_layers+2):
+			model.rconvs[i-2].weight = convert_w(w[name.format(i)][k])
+			model.rconvs[i-2].bias = convert_b(w[name.format(i)][b])
+
+		model.fconv.weight = convert_w(w[name.format(n_layers+2)][k])
+		model.fconv.bias = convert_b(w[name.format(n_layers+2)][b])
+
+		name = "logcounts_1" if not bias else "logcounts/logcounts"
+		model.linear.weight = torch.nn.Parameter(torch.tensor(w[name][k][:].T))
+		model.linear.bias = convert_b(w[name][b])
+		return model
```

## bpnetlite/io.py

```diff
@@ -1,9 +1,9 @@
 # io.py
-# Author: Jacob Schreiber
+# Author: Jacob Schreiber <jmschreiber91@gmail.com>
 # Code adapted from Avanti Shrikumar and Ziga Avsec
 
 import numpy
 import torch
 import pandas
 
 import pyfaidx
@@ -159,37 +159,40 @@
 				X_ctl = torch.flip(X_ctl, [0, 1])
 
 		if self.controls is not None:
 			return X, X_ctl, y
 
 		return X, y
 
-def extract_peaks(peaks, sequences, signals=None, controls=None, chroms=None, 
+def extract_loci(loci, sequences, signals=None, controls=None, chroms=None, 
 	in_window=2114, out_window=1000, max_jitter=128, min_counts=None,
 	max_counts=None, verbose=False):
-	"""Extract sequences and signals at coordinates from a peak file.
+	"""Extract sequences and signals at coordinates from a locus file.
 
 	This function will take in genome-wide sequences, signals, and optionally
 	controls, and extract the values of each at the coordinates specified in
-	the peak file and return them as tensors.
+	the locus file/s and return them as tensors.
 
 	Signals and controls are both lists with the length of the list, n_s
 	and n_c respectively, being the middle dimension of the returned
 	tensors. Specifically, the returned tensors of size 
-	(len(peaks), n_s/n_c, (out_window/in_wndow)+max_jitter*2).
+	(len(loci), n_s/n_c, (out_window/in_wndow)+max_jitter*2).
 
 	The values for sequences, signals, and controls, can either be filepaths
 	or dictionaries of numpy arrays or a mix of the two. When a filepath is 
 	passed in it is loaded using pyfaidx or pyBigWig respectively.   
 
 	Parameters
 	----------
-	peaks: str or pandas.DataFrame
+	loci: str or pandas.DataFrame or list/tuple of such
 		Either the path to a bed file or a pandas DataFrame object containing
-		three columns: the chromosome, the start, and the end, of each peak.
+		three columns: the chromosome, the start, and the end, of each locus
+		to train on. Alternatively, a list or tuple of strings/DataFrames where
+		the intention is to train on the interleaved concatenation, i.e., when
+		you want to train on peaks and negatives.
 
 	sequences: str or dictionary
 		Either the path to a fasta file to read from or a dictionary where the
 		keys are the unique set of chromosoms and the values are one-hot
 		encoded sequences as numpy arrays or memory maps.
 
 	signals: list of strs or list of dictionaries or None, optional
@@ -201,16 +204,16 @@
 	controls: list of strs or list of dictionaries or None, optional
 		A list of filepaths to bigwig files, where each filepath will be read
 		using pyBigWig, or a list of dictionaries where the keys are the same
 		set of unique chromosomes and the values are numpy arrays or memory
 		maps. If None, no control tensor is returned. Default is None. 
 
 	chroms: list or None, optional
-		A set of chromosomes to extact peaks from. Peaks in other chromosomes
-		in the peak file are ignored. If None, all peaks are used. Default is
+		A set of chromosomes to extact loci from. Loci in other chromosomes
+		in the locus file are ignored. If None, all loci are used. Default is
 		None.
 
 	in_window: int, optional
 		The input window size. Default is 2114.
 
 	out_window: int, optional
 		The output window size. Default is 1000.
@@ -231,64 +234,80 @@
 
 	verbose: bool, optional
 		Whether to display a progress bar while loading. Default is False.
 
 	Returns
 	-------
 	seqs: torch.tensor, shape=(n, 4, in_window+2*max_jitter)
-		The extracted sequences in the same order as the peaks in the peak
+		The extracted sequences in the same order as the loci in the locus
 		file after optional filtering by chromosome.
 
 	signals: torch.tensor, shape=(n, len(signals), out_window+2*max_jitter)
 		The extracted signals where the first dimension is in the same order
-		as peaks in the peak file after optional filtering by chromosome and
+		as loci in the locus file after optional filtering by chromosome and
 		the second dimension is in the same order as the list of signal files.
 		If no signal files are given, this is not returned.
 
 	controls: torch.tensor, shape=(n, len(controls), out_window+2*max_jitter)
 		The extracted controls where the first dimension is in the same order
-		as peaks in the peak file after optional filtering by chromosome and
+		as loci in the locus file after optional filtering by chromosome and
 		the second dimension is in the same order as the list of control files.
 		If no control files are given, this is not returned.
 	"""
 
 	seqs, signals_, controls_ = [], [], []
 	in_width, out_width = in_window // 2, out_window // 2
 
 	# Load the sequences
 	if isinstance(sequences, str):
 		sequences = pyfaidx.Fasta(sequences)
 
-	# Load the peaks or rename the columns to be consistent
 	names = ['chrom', 'start', 'end']
-	if isinstance(peaks, str):
-		peaks = pandas.read_csv(peaks, sep="\t", usecols=(0, 1, 2), 
-			header=None, index_col=False, names=names)
-	else:
-		peaks = peaks.copy()
-		peaks.columns = names
+	if not isinstance(loci, (tuple, list)):
+		loci = [loci]
+
+	loci_dfs = []
+	for i, df in enumerate(loci):
+	    if isinstance(df, str):
+	        df = pandas.read_csv(df, sep='\t', usecols=[0, 1, 2], 
+	            header=None, index_col=False, names=names)
+	        df['idx'] = numpy.arange(len(df)) * len(loci) + i
+
+	    loci_dfs.append(df)
+
+	loci = pandas.concat(loci_dfs).set_index("idx").sort_index().reset_index(drop=True)
 
 	if chroms is not None:
-		peaks = peaks[numpy.isin(peaks['chrom'], chroms)]
+		loci = loci[numpy.isin(loci['chrom'], chroms)]
 
 	# Load the signal and optional control tracks if filenames are given
 	if signals is not None:
 		for i, signal in enumerate(signals):
 			if isinstance(signal, str):
 				signals[i] = pyBigWig.open(signal, "r")
 
 	if controls is not None:
 		for i, control in enumerate(controls):
 			if isinstance(control, str):
 				controls[i] = pyBigWig.open(control, "r")
 
-	desc = "Loading Peaks"
+	desc = "Loading Loci"
 	d = not verbose
-	for chrom, start, end in tqdm(peaks.values, disable=d, desc=desc):
+
+	max_width = max(in_width, out_width)
+
+	for chrom, start, end in tqdm(loci.values, disable=d, desc=desc):
 		mid = start + (end - start) // 2
+
+		if start - max_width - max_jitter < 0:
+			continue
+
+		if end + max_width + max_jitter >= len(sequences[chrom]):
+			continue
+
 		start = mid - out_width - max_jitter
 		end = mid + out_width + max_jitter
 
 		# Extract the signal from each of the signal files
 		if signals is not None:
 			signals_.append([])
 			for signal in signals:
@@ -345,29 +364,32 @@
 		if controls is not None:
 			controls_ = torch.tensor(numpy.array(controls_), dtype=torch.float32)
 			return seqs, controls_
 
 		return seqs			
 
 
-def PeakGenerator(peaks, sequences, signals, controls=None, chroms=None, 
+def PeakGenerator(loci, sequences, signals, controls=None, chroms=None, 
 	in_window=2114, out_window=1000, max_jitter=128, reverse_complement=True, 
 	min_counts=None, max_counts=None, random_state=None, pin_memory=True, 
 	num_workers=0, batch_size=32, verbose=False):
 	"""This is a constructor function that handles all IO.
 
 	This function will extract signal from all signal and control files,
 	pass that into a DataGenerator, and wrap that using a PyTorch data
 	loader. This is the only function that needs to be used.
 
 	Parameters
 	----------
-	peaks: str or pandas.DataFrame
+	loci: str or pandas.DataFrame or list/tuple of such
 		Either the path to a bed file or a pandas DataFrame object containing
-		three columns: the chromosome, the start, and the end, of each peak.
+		three columns: the chromosome, the start, and the end, of each locus
+		to train on. Alternatively, a list or tuple of strings/DataFrames where
+		the intention is to train on the interleaved concatenation, i.e., when
+		you want ot train on peaks and negatives.
 
 	sequences: str or dictionary
 		Either the path to a fasta file to read from or a dictionary where the
 		keys are the unique set of chromosoms and the values are one-hot
 		encoded sequences as numpy arrays or memory maps.
 
 	signals: list of strs or list of dictionaries
@@ -379,16 +401,16 @@
 	controls: list of strs or list of dictionaries or None, optional
 		A list of filepaths to bigwig files, where each filepath will be read
 		using pyBigWig, or a list of dictionaries where the keys are the same
 		set of unique chromosomes and the values are numpy arrays or memory
 		maps. If None, no control tensor is returned. Default is None. 
 
 	chroms: list or None, optional
-		A set of chromosomes to extact peaks from. Peaks in other chromosomes
-		in the peak file are ignored. If None, all peaks are used. Default is
+		A set of chromosomes to extact loci from. Loci in other chromosomes
+		in the locus file are ignored. If None, all loci are used. Default is
 		None.
 
 	in_window: int, optional
 		The input window size. Default is 2114.
 
 	out_window: int, optional
 		The output window size. Default is 1000.
@@ -429,15 +451,15 @@
 
 	Returns
 	-------
 	X: torch.utils.data.DataLoader
 		A PyTorch DataLoader wrapped DataGenerator object.
 	"""
 
-	X = extract_peaks(peaks=peaks, sequences=sequences, signals=signals, 
+	X = extract_loci(loci=loci, sequences=sequences, signals=signals, 
 		controls=controls, chroms=chroms, in_window=in_window, 
 		out_window=out_window, max_jitter=max_jitter, min_counts=min_counts,
 		max_counts=max_counts, verbose=verbose)
 
 	if controls is not None:
 		sequences, signals_, controls_ = X
 	else:
```

## Comparing `bpnet_lite-0.2.0.data/scripts/bpnet` & `bpnet_lite-0.3.0.data/scripts/bpnet`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 #!python
 # BPNet command-line tool
 # Author: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import sys
 import numpy
 import torch
+import pyfaidx
 import argparse
 
 from bpnetlite import BPNet
 from bpnetlite.io import PeakGenerator
-from bpnetlite.io import extract_peaks
+from bpnetlite.io import extract_loci
+
 from bpnetlite.attributions import calculate_attributions
+from bpnetlite.marginalize import marginalization_report
 
 import json
 
 desc = """BPNet is an neural network primarily composed of dilated residual
 	convolution layers for modeling the associations between biological
 	sequences and biochemical readouts. This tool will take in a fasta
 	file for the sequence, a bed file for signal peak locations, and bigWig
 	files for the signal to predict and the control signal, and train a
 	BPNet model for you."""
 
 # Read in the arguments
 parser = argparse.ArgumentParser(description=desc)
-subparsers = parser.add_subparsers(help="Must be either 'train', 'predict', or 'interpret'.", required=True, dest='cmd')
+subparsers = parser.add_subparsers(help="Must be either 'train', 'predict', 'interpret', or 'marginalize'.", required=True, dest='cmd')
 
 train_parser = subparsers.add_parser("train", help="Train a BPNet model.")
 train_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for training the model.")
 
 predict_parser = subparsers.add_parser("predict", help="Make predictions using a trained BPNet model.")
 predict_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for making predictions.")
 
 interpret_parser = subparsers.add_parser("interpret", help="Make interpretations using a trained BPNet model.")
 interpret_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for calculating attributions.")
 
+marginalize_parser = subparsers.add_parser("marginalize", help="Run marginalizations given motifs.")
+marginalize_parser.add_argument("-p", "--parameters", type=str, required=True,
+	help="A JSON file containing the parameters for calculating attributions.")
+
+
 # Pull the arguments
 args = parser.parse_args()
 
 if args.cmd == "train":
 	with open(args.parameters, "r") as infile:
 		parameters = json.load(infile)
 
@@ -62,15 +70,15 @@
 		'max_counts': 99999999,
 
 		'training_chroms': ['chr1', 'chr2', 'chr3', 'chr5', 'chr6', 'chr7', 
 			'chr8', 'chr9', 'chr10', 'chr12', 'chr13', 'chr14', 'chr16', 
 			'chr18', 'chr19', 'chr20', 'chr22'],
 		'validation_chroms': ['chr4', 'chr15', 'chr21'],
 		'sequences': None,
-		'peaks': None,
+		'loci': None,
 		'signals': None,
 		'controls': None,
 		'random_state': None
 	}
 
 	for parameter, value in default_parameters.items():
 		if parameter not in parameters:
@@ -78,15 +86,15 @@
 				raise ValueError("Must provide value for '{}'".format(parameter))
 
 			parameters[parameter] = value
 
 	###
 
 	training_data = PeakGenerator(
-		peaks=parameters['peaks'], 
+		loci=parameters['loci'], 
 		sequences=parameters['sequences'],
 		signals=parameters['signals'],
 		controls=parameters['controls'],
 		chroms=parameters['training_chroms'],
 		in_window=parameters['in_window'],
 		out_window=parameters['out_window'],
 		max_jitter=parameters['max_jitter'],
@@ -95,19 +103,19 @@
 		max_counts=parameters['max_counts'],
 		random_state=parameters['random_state'],
 		batch_size=parameters['batch_size'],
 		verbose=parameters['verbose']
 	)
 
 
-	valid_sequences, valid_signals, valid_controls = extract_peaks(
+	valid_sequences, valid_signals, valid_controls = extract_loci(
 		sequences=parameters['sequences'],
 		signals=parameters['signals'],
 		controls=parameters['controls'],
-		peaks=parameters['peaks'],
+		loci=parameters['loci'],
 		chroms=parameters['validation_chroms'],
 		in_window=parameters['in_window'],
 		out_window=parameters['out_window'],
 		max_jitter=0,
 		verbose=parameters['verbose']
 	)
 
@@ -135,34 +143,34 @@
 		'in_window': 2114,
 		'out_window': 1000,
 		'verbose': False,
 		'chroms': ['chr1', 'chr2', 'chr3', 'chr5', 'chr6', 'chr7', 
 			'chr8', 'chr9', 'chr10', 'chr12', 'chr13', 'chr14', 'chr16', 
 			'chr18', 'chr19', 'chr20', 'chr22'],
 		'sequences': None,
-		'peaks': None,
+		'loci': None,
 		'controls': None,
 		'model': None,
 		'profile_filename': 'y_profile.npz',
 		'count_filename': 'y_count.npz'
 	}
 
 	for parameter, value in default_parameters.items():
 		if parameter not in parameters:
 			if value is None and parameter != "controls":
 				raise ValueError("Must provide value for '{}'".format(parameter))
 
 			parameters[parameter] = value
 
-	model = torch.load(parameters['model'])
+	model = torch.load(parameters['model']).cuda()
 
-	examples = extract_peaks(
+	examples = extract_loci(
 		sequences=parameters['sequences'],
 		controls=parameters['controls'],
-		peaks=parameters['peaks'],
+		loci=parameters['loci'],
 		chroms=parameters['chroms'],
 		max_jitter=0,
 		verbose=parameters['verbose']
 	)
 
 	if parameters['controls'] == None:
 		X = examples
@@ -188,41 +196,95 @@
 		'in_window': 2114,
 		'out_window': 1000,
 		'verbose': False,
 		'chroms': ['chr1', 'chr2', 'chr3', 'chr5', 'chr6', 'chr7', 
 			'chr8', 'chr9', 'chr10', 'chr12', 'chr13', 'chr14', 'chr16', 
 			'chr18', 'chr19', 'chr20', 'chr22'],
 		'sequences': None,
-		'peaks': None,
+		'loci': None,
 		'model': None,
 		'output': 'count',
 		'ohe_filename': 'ohe.npz',
 		'shap_filename': 'shap.npz',
 		'random_state':0,
 	}
 
 	for parameter, value in default_parameters.items():
 		if parameter not in parameters:
 			if value is None and parameter != "controls":
 				raise ValueError("Must provide value for '{}'".format(parameter))
 
 			parameters[parameter] = value
 
-	model = torch.load(parameters['model'])
+	model = torch.load(parameters['model']).cuda()
 
-	X = extract_peaks(
+	X = extract_loci(
 		sequences=parameters['sequences'],
-		peaks=parameters['peaks'],
+		loci=parameters['loci'],
 		chroms=parameters['chroms'],
 		max_jitter=0,
 		verbose=parameters['verbose']
 	)
 
-	X_ctl = torch.zeros(X.shape[0], model.n_control_tracks, X.shape[-1])
+	if model.n_control_tracks > 0:
+		X_ctl = (torch.zeros(X.shape[0], model.n_control_tracks, X.shape[-1]),)
+	else:
+		X_ctl = None
 
-	X_attr = calculate_attributions(model, X, args=(X_ctl,),
+	X_attr = calculate_attributions(model, X, args=X_ctl,
 		model_output=parameters['output'], hypothetical=True, 
 		random_state=parameters['random_state'],
 		verbose=parameters['verbose'])
 
 	numpy.savez_compressed(parameters['ohe_filename'], X)
-	numpy.savez_compressed(parameters['shap_filename'], X_attr)
+	numpy.savez_compressed(parameters['shap_filename'], X_attr)
+
+elif args.cmd == 'marginalize':
+	with open(args.parameters, "r") as infile:
+		parameters = json.load(infile)
+
+	default_parameters = {
+		'batch_size': 64,
+		'in_window': 2114,
+		'out_window': 1000,
+		'verbose': False,
+		'chroms': ['chr1', 'chr2', 'chr3', 'chr5', 'chr6', 'chr7', 
+			'chr8', 'chr9', 'chr10', 'chr12', 'chr13', 'chr14', 'chr16', 
+			'chr18', 'chr19', 'chr20', 'chr22'],
+		'sequences': None,
+		'motifs': None,
+		'loci': None,
+		'n_loci': None,
+		'shuffle': False,
+		'model': None,
+		'output_filename':'marginalize/',
+		'random_state':0,
+	}
+
+	for parameter, value in default_parameters.items():
+		if parameter not in parameters:
+			if value is None and parameter != "controls":
+				raise ValueError("Must provide value for '{}'".format(parameter))
+
+			parameters[parameter] = value
+
+	model = torch.load(parameters['model']).cuda()
+
+	X = extract_loci(
+		sequences=parameters['sequences'],
+		loci=parameters['loci'],
+		chroms=parameters['chroms'],
+		max_jitter=0,
+		verbose=parameters['verbose']
+	)
+
+	if parameters['shuffle'] == True:
+		idxs = numpy.arange(X.shape[0])
+		numpy.random.shuffle(idxs)
+		X = X[idxs]
+
+	if parameters['n_loci'] is not None:
+		X = X[:parameters['n_loci']]
+
+	motifs = pyfaidx.Fasta(parameters['motifs'])
+	marginalization_report(model, motifs, X, 
+		parameters['output_filename'])
```

## Comparing `bpnet_lite-0.2.0.dist-info/LICENSE` & `bpnet_lite-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bpnet_lite-0.2.0.dist-info/METADATA` & `bpnet_lite-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: bpnet-lite
-Version: 0.2.0
+Version: 0.3.0
 Summary: bpnet-lite is a minimal implementation of BPNet, a neural network aimed at interpreting regulatory activity of the genome.
 Home-page: https://github.com/jmschrei/bpnet-lite
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
-Platform: UNKNOWN
 License-File: LICENSE
 Requires-Dist: numpy (>=1.14.2)
 Requires-Dist: scipy (>=1.0.0)
 Requires-Dist: pandas (>=1.3.3)
 Requires-Dist: pyBigWig (>=0.3.17)
 Requires-Dist: torch (>=1.9.0)
-
-UNKNOWN
+Requires-Dist: h5py (>=3.7.0)
```

## Comparing `bpnet_lite-0.2.0.dist-info/RECORD` & `bpnet_lite-0.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-bpnet_lite-0.2.0.data/scripts/bpnet,sha256=mmzNKf7RWgHzuhtVawd_owobtqkNm6vfM6clPOUT9xY,7005
-bpnetlite/__init__.py,sha256=rWPuqJGixrsNRsBAvHIrYph211b8pJFyTKWwn250Lq8,140
-bpnetlite/attributions.py,sha256=LiVq9FRvccOuK_LSXqksaqs4rLHrKlRi-1zPxYgr7fg,7450
-bpnetlite/bpnet.py,sha256=hOxmr3TdHYbzxYdVo9_IIIj8fktGtIobqsUrs4kgdeY,9063
-bpnetlite/io.py,sha256=9zyB-r6D2faOme6gsU_V4FZRmEzGxdTINsuxaJDEUss,16233
+bpnet_lite-0.3.0.data/scripts/bpnet,sha256=50s_NV-O0KNC5hs8-BNhnKfkch-EuspXE7ozEfg9f28,8723
+bpnet_lite-0.3.0.data/scripts/chrombpnet,sha256=-q6JKUd4uPZfPjWRkmB0tKbWDTnvsdHwlR4Z9vP7ohQ,8649
+bpnetlite/__init__.py,sha256=q6bovXNUCw0oGZuDdUUoGMr157Tkxdi1-VQ9RyEFaoM,175
+bpnetlite/attributions.py,sha256=5n1PKmAc_XBPTGILEgas7YyZh87L4ZlLb7emRFSJGHU,10712
+bpnetlite/bpnet.py,sha256=GaJdYf2fNf5c9Jl3I-3Bxzg4oGbXHwtpsVYFOp0LtrE,15776
+bpnetlite/chrombpnet.py,sha256=aTtNg9hkXdlNPswmQczERSn9HZkEUYw38QBnjzKnrm0,5827
+bpnetlite/io.py,sha256=JCqy5evhTgjJGZ7PlWddBe8ESeonPOk4CaXHZ3bWUvo,17015
+bpnetlite/logging.py,sha256=7dT7lGHcMxZgbI6_kqOBPN87WzJMvVrsA0XXLd3ZbAQ,1643
 bpnetlite/losses.py,sha256=2kPpx-_HpmjGdOaHgG9eKVEOQga2wCzkYuxXgBc64OE,2418
+bpnetlite/marginalize.py,sha256=DWv764jJmkQK4NYErIheD3GLh-9i-Yts6fo-7mwSa6k,3674
 bpnetlite/performance.py,sha256=P6hbqcGsZscN8ee_R10TftQCt1moi0kU4s3Pa8LQGM4,13599
-bpnet_lite-0.2.0.dist-info/LICENSE,sha256=7INkXi8uNRhuIecag4RwrinhCQmP-P6pAWoK6UOxi1U,1072
-bpnet_lite-0.2.0.dist-info/METADATA,sha256=gih1ikpmkvn8FZCivf6J7SwqIiTpQ6PY93SAO3dbl3Q,530
-bpnet_lite-0.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bpnet_lite-0.2.0.dist-info/top_level.txt,sha256=SKuFVvK8spuR4slxk09vQL-IR3R_x4ahC68BLEU7y3g,10
-bpnet_lite-0.2.0.dist-info/RECORD,,
+bpnet_lite-0.3.0.dist-info/LICENSE,sha256=7INkXi8uNRhuIecag4RwrinhCQmP-P6pAWoK6UOxi1U,1072
+bpnet_lite-0.3.0.dist-info/METADATA,sha256=37Z4Db4BId3c8I4vAgh4mr8j9ZrerEdI3jHBqNt66TA,533
+bpnet_lite-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bpnet_lite-0.3.0.dist-info/top_level.txt,sha256=SKuFVvK8spuR4slxk09vQL-IR3R_x4ahC68BLEU7y3g,10
+bpnet_lite-0.3.0.dist-info/RECORD,,
```

