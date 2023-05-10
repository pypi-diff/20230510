# Comparing `tmp/ecg_quality-0.1.2.tar.gz` & `tmp/ecg_quality-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecg_quality-0.1.2.tar", last modified: Sun May  7 01:23:28 2023, max compression
+gzip compressed data, was "ecg_quality-0.1.3.tar", last modified: Wed May 10 08:12:38 2023, max compression
```

## Comparing `ecg_quality-0.1.2.tar` & `ecg_quality-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.818211 ecg_quality-0.1.2/
--rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      416 2023-05-07 01:23:28.818211 ecg_quality-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-04-21 20:39:12.000000 ecg_quality-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.768785 ecg_quality-0.1.2/ecg_quality/
--rw-rw-rw-   0        0        0    10091 2023-05-06 22:43:31.000000 ecg_quality-0.1.2/ecg_quality/ECGQualityChecker.py
--rw-rw-rw-   0        0        0       41 2023-05-06 20:18:00.000000 ecg_quality-0.1.2/ecg_quality/__init__.py
--rw-rw-rw-   0        0        0      807 2023-04-22 20:35:15.000000 ecg_quality-0.1.2/ecg_quality/model.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.817178 ecg_quality-0.1.2/ecg_quality/models/
--rw-rw-rw-   0        0        0   128640 2023-04-29 16:55:23.000000 ecg_quality-0.1.2/ecg_quality/models/CNN2s.h5
--rw-rw-rw-   0        0        0  7528704 2023-05-02 21:37:58.000000 ecg_quality-0.1.2/ecg_quality/models/CNN5s.h5
--rw-rw-rw-   0        0        0  1224424 2023-04-29 16:55:22.000000 ecg_quality-0.1.2/ecg_quality/models/LSTM2s.h5
--rw-rw-rw-   0        0        0   472672 2023-05-05 11:00:32.000000 ecg_quality-0.1.2/ecg_quality/models/OSCNN2s.h5
--rw-rw-rw-   0        0        0        0 2023-05-07 00:50:50.000000 ecg_quality-0.1.2/ecg_quality/models/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-05-06 23:14:45.000000 ecg_quality-0.1.2/ecg_quality/tf_model.py
--rw-rw-rw-   0        0        0     1107 2023-05-06 23:14:45.000000 ecg_quality-0.1.2/ecg_quality/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:23:28.797701 ecg_quality-0.1.2/ecg_quality.egg-info/
--rw-rw-rw-   0        0        0      416 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-07 01:23:28.000000 ecg_quality-0.1.2/ecg_quality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-07 01:23:28.819211 ecg_quality-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-05-07 01:20:36.000000 ecg_quality-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.320969 ecg_quality-0.1.3/
+-rw-rw-rw-   0        0        0    35149 2023-04-21 20:39:12.000000 ecg_quality-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3296 2023-05-10 08:12:38.320969 ecg_quality-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2023-05-10 07:54:02.000000 ecg_quality-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.293178 ecg_quality-0.1.3/ecg_quality/
+-rw-rw-rw-   0        0        0    10411 2023-05-10 08:09:39.000000 ecg_quality-0.1.3/ecg_quality/ECGQualityChecker.py
+-rw-rw-rw-   0        0        0       41 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-04-22 20:35:15.000000 ecg_quality-0.1.3/ecg_quality/model.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.319927 ecg_quality-0.1.3/ecg_quality/models/
+-rw-rw-rw-   0        0        0   128640 2023-04-29 16:55:23.000000 ecg_quality-0.1.3/ecg_quality/models/CNN2s.h5
+-rw-rw-rw-   0        0        0  7528704 2023-05-02 21:37:58.000000 ecg_quality-0.1.3/ecg_quality/models/CNN5s.h5
+-rw-rw-rw-   0        0        0  1224424 2023-04-29 16:55:22.000000 ecg_quality-0.1.3/ecg_quality/models/LSTM2s.h5
+-rw-rw-rw-   0        0        0   472672 2023-05-05 11:00:32.000000 ecg_quality-0.1.3/ecg_quality/models/OSCNN2s.h5
+-rw-rw-rw-   0        0        0        0 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/models/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/tf_model.py
+-rw-rw-rw-   0        0        0     1140 2023-05-10 07:25:34.000000 ecg_quality-0.1.3/ecg_quality/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:12:38.301756 ecg_quality-0.1.3/ecg_quality.egg-info/
+-rw-rw-rw-   0        0        0     3296 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 08:12:38.000000 ecg_quality-0.1.3/ecg_quality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-10 08:12:38.322937 ecg_quality-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-05-10 08:03:01.000000 ecg_quality-0.1.3/setup.py
```

### Comparing `ecg_quality-0.1.2/LICENSE` & `ecg_quality-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/ECGQualityChecker.py` & `ecg_quality-0.1.3/ecg_quality/ECGQualityChecker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,219 +1,222 @@
-import numpy as np
-from ecg_quality.utils import MODEL_PATH_DICT
-
-from ecg_quality import utils
-from ecg_quality import tf_model
-import neurokit2 as nk
-import warnings
-
-
-
-class ECGQualityChecker:
-    """
-    **ECG_Quality_Checker**
-    ===================
-
-    This class takes care of the processing and checking of the quality of ECG signal. Currently, it uses three main classes of signal in different modes:
-    * Class 1: This corresponds to signal that is clean, with all waves being present.
-    * Class 2 : This signal has some level of noise and the P and T waves are not detectable, but the QRS complex is still detectable.
-    * Class 3: The noise is too large and no ECG segment can be found.
-
-    The model works by using a sliding window, where each window is graded by a neural network with a score between 0 and 1. Over the signal, this score is averaged where the scores overlap and thresholds are applied. There are saved thresholds to be automatically used to prioritize better signal quality classification precision. The class works with signal in mV.
-
-    To use this checker, first create an during which creation everything is specified. Then the class can repeatedly process EKG signal with the ecg_process method.
-    """
-
-
-
-
-
-
-
-
-    def __init__(self, model:str = 'cnn2s', stride:float = 0.0, return_mode:str = 'score', thresholds:list = None, return_type:str = 'full', sampling_rate:int = 250, clean_data:bool=True):
-        """
-        Parameters
-        --------------
-
-        **model : str**
-            This is the model to be used by the class. There are currently 4 possible models to use:
-        * cnn2s : This model uses CNN architecture with the size of the sliding window being 2 seconds.
-        * cnn5s : This model also uses CNN architecture but with the size of sliding window being 5 seconds.
-        * lstm2s : This model uses LSTM based architecture with the sliding window size of 2 seconds.
-        * oscnn2s : This model uses Omni-Scale block architecture, that is CNN based, with sliding window of size 2 seconds.
-
-
-        **stride: float**
-        This is the size of the step to be used represented as the ratio of the length of the window length. The class makes sure the length is at least 1 second and that the stride is a divisor of window length.
-
-
-        **return_mode : str**
-        There are totally 4 different modes that can be used when using this class to specify type of 		returned values:
-
-        * score : The model will return continuous values of score in the range 0 to 1
-        * three_value : The model will use two thresholds and return all three classes of signal, with values 1.0, 2.0 or 3.0.
-        * binary_clean : The model will return either 1.0 for signal of Class 1 or 2.0 for signals of Class 2 and 3.
-        * binary_qrs : The model will return 1.0 for signals of Class 1 and 2 and 2.0 for signal of class 3.0.
-
-
-
-        **thresholds : list**
-        The thresholds to be used by the model. Their amount needs to correspond to the type of classification we want to do. If we want to do three class classification, there need to be two thresholds, for both binary classifications, there needs to be just one.
-
-        **return_type : str**
-
-        This is how long will be the returned values. For mode full, the values of the length of the input signal will be used. The other mode, intervals, means that there will be a value returned for each short interval where the score does not change. These intervals are always the length of the stride in real values. For each of these intervals, there will be just one value returned.
-
-        **sampling_rate : int**
-
-        The models currently only support 250 Hz. Using any other frequency will result in fail. Slightly different frequencies can theoretically be used, but that is to be done at your own risk.
-
-        **clean_data : bool**
-
-        Whether the data should be cleaned before processing. The models were trained on cleaned data so this is advised unless you already cleaned data beforehand. For cleaning, we are using neurokit2 function ecg_clean with its default settings as of version 0.2.4.
-
-
-
-
-        :param model: Model to be used
-        :param stride: The soze of the step of the moving window
-        :param return_mode: The type of classification to be done by the class
-        :param thresholds: The thresholds to be used when and if other return_mode than socre is chosen
-        :param return_type: how mnay values should be returned
-        :param sampling_rate: The sampling rate of the ECG signal to be processed, currently just 250 Hz is supported
-        :param clean_data: Whether to clean data before processing them.
-        """
-        # urobime checks vsetkych modelov
-
-        if model not in list(MODEL_PATH_DICT.keys()):
-            raise ValueError(model + ' is not a known model that can be used')
-
-        if return_mode not in ['score', 'three_value', 'binary_clean', 'binary_qrs']:
-            raise ValueError('Return mode needs to be one of: score, three_value, binary_clean, binary_qrs. Currently is ' + str(return_mode))
-
-        if thresholds is None:
-            thresholds = utils.get_default_thresholds(model, return_mode)
-
-
-        if return_mode == 'score':
-            if thresholds is not None:
-                raise ValueError('Threshold count does not correspond to return mode')
-        elif return_mode in ['binary_clean', 'binary_qrs']:
-            if len(thresholds) != 1:
-                raise ValueError('Threshold count does not correspond to return mode')
-            elif not 0 <= thresholds[0] <= 1.0:
-                raise ValueError('Threshold value not in 0 to 1 interval')
-        elif return_mode == 'three_value':
-            if len(thresholds) != 2:
-                raise ValueError('Threshold count does not correspond to return mode')
-            elif not 0 <= thresholds[0] <= 1.0 or not 0 <= thresholds[1] <= 1.0:
-                raise ValueError('Threshold value not in 0 to 1 interval')
-            thresholds = np.sort(thresholds)
-
-        if return_type not in ['intervals', 'full']:
-            raise ValueError('Return type needs to be one of: intervals, full. Currently is ' + str(return_type))
-
-        if sampling_rate != 250:
-            raise NotImplementedError('This class currently only support ECG with frequency of 250 Hz. Consider modyfing your data to comply with this prerequisite.')
-
-        if stride < 0:
-            raise ValueError('Stride for a model can not be negative')
-
-        self.model = tf_model.tf_model(model)
-
-        self.input_length = self.model.get_input_length()
-
-        self.stride = utils.get_stride_length(self.model.get_input_length(), stride, sampling_rate)
-        self.return_mode = return_mode
-        self.return_type = return_type
-        self.thresholds = thresholds
-        self.sampling_rate = sampling_rate
-        self.clean_data = clean_data
-
-    def process_signal(self, signal):
-        """
-
-        This method processes ECG signal and returns specified values.
-
-        Parameters:
-        --------------
-
-        **signal : list**
-
-        This is the signal to be processed by the object. The ECG needs to be in mV.
-
-
-        Returns:
-        ----------
-
-        **results : list**
-        These are the results. Their specific properties depend on the parameters passed when creating the class.
-
-        :param signal: The ECG to be processed.
-        :return: list - This is the list of the found values. Their specific properties depend on the parameters passed inside constructor.
-        """
-
-
-        if self.return_type == 'full':
-            return self._process_signal_full(signal)
-        elif self.return_type == 'intervals':
-            return self._process_signal_interval(signal)
-
-    def _process_signal_full(self, signal):
-        if self.clean_data:
-            signal = nk.ecg_clean(signal, sampling_rate=self.sampling_rate)
-
-        output = np.zeros_like(signal)
-        win_count = np.zeros_like(signal)
-
-        for win_start in range(0, len(signal)-self.input_length + 1, self.stride):
-            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
-            output[win_start:win_start + self.input_length] = output[win_start:win_start + self.input_length] + score
-            win_count[win_start:win_start + self.input_length] = win_count[win_start:win_start + self.input_length] + 1
-        return self._calc_precise_scores(output, win_count)
-
-    def _process_signal_interval(self, signal):
-
-        if self.clean_data:
-            signal = nk.ecg_clean(signal, sampling_rate=self.sampling_rate)
-
-        output = np.zeros(len(signal) // self.stride)
-        win_count = np.zeros(len(signal) // self.stride)
-
-        for win_start in range(0, len(signal) - self.input_length + 1, self.stride):
-            a = win_start // self.stride
-            b = (win_start + self.input_length) // self.stride
-
-            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
-            output[a:b] = output[a:b] + score
-            win_count[a:b] = win_count[a:b] + 1
-        return self._calc_precise_scores(output, win_count)
-
-    def _get_two_value(self, scores):
-        return [0.0 if x < self.thresholds[0] else 1.0 for x in scores]
-
-    def _get_three_value(self, scores):
-
-        def mapper(val):
-            if val < self.thresholds[0]:
-                return 0.0
-            elif val < self.thresholds[1]:
-                return 0.5
-            else:
-                return 1.0
-        return [mapper(x) for x in scores]
-
-    def _calc_precise_scores(self, scores, win_counts):
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            scores = np.divide(scores, win_counts)
-        # scores = scores[~np.isnan(scores)]
-
-        if self.return_mode == 'score':
-            return scores
-        elif self.return_mode == 'two_value':
-            return self._get_two_value(scores)
-        elif self.return_mode == 'three_value':
-            return self._get_three_value(scores)
-
-
+import numpy as np
+from ecg_quality.utils import MODEL_PATH_DICT
+
+from ecg_quality import utils
+from ecg_quality import tf_model
+import neurokit2 as nk
+import warnings
+
+
+
+class ECGQualityChecker:
+    """
+    **ECG_Quality_Checker**
+    ===================
+
+    This class takes care of the processing and checking of the quality of ECG signal. Currently, it uses three main classes of signal in different modes:
+    * Class 1: This corresponds to signal that is clean, with all waves being present.
+    * Class 2 : This signal has some level of noise and the P and T waves are not detectable, but the QRS complex is still detectable.
+    * Class 3: The noise is too large and no ECG segment can be found.
+
+    The model works by using a sliding window, where each window is graded by a neural network with a score between 0 and 1. Over the signal, this score is averaged where the scores overlap and thresholds are applied. There are saved thresholds to be automatically used to prioritize better signal quality classification precision. The class works with signal in mV.
+
+    To use this checker, first create an during which creation everything is specified. Then the class can repeatedly process EKG signal with the ecg_process method.
+    """
+
+
+
+
+
+
+
+
+    def __init__(self, model:str = 'cnn2s', stride:float = 0.0, return_mode:str = 'score', thresholds:list = None, return_type:str = 'full', sampling_rate:int = 250, clean_data:bool=True):
+        """
+        Parameters
+        --------------
+
+        **model : str**
+            This is the model to be used by the class. There are currently 4 possible models to use:
+        * cnn2s : This model uses CNN architecture with the size of the sliding window being 2 seconds.
+        * cnn5s : This model also uses CNN architecture but with the size of sliding window being 5 seconds.
+        * lstm2s : This model uses LSTM based architecture with the sliding window size of 2 seconds.
+        * oscnn2s : This model uses Omni-Scale block architecture, that is CNN based, with sliding window of size 2 seconds.
+
+
+        **stride: float**
+        This is the size of the step to be used represented as the ratio of the length of the window length. The class makes sure the length is at least 1 second and that the stride is a divisor of window length.
+
+
+        **return_mode : str**
+        There are totally 4 different modes that can be used when using this class to specify type of 		returned values:
+
+        * score : The model will return continuous values of score in the range 0 to 1
+        * three_value : The model will use two thresholds and return all three classes of signal, with values 1.0, 2.0 or 3.0.
+        * binary_clean : The model will return either 1.0 for signal of Class 1 or 2.0 for signals of Class 2 and 3.
+        * binary_qrs : The model will return 1.0 for signals of Class 1 and 2 and 2.0 for signal of class 3.0.
+
+
+
+        **thresholds : list**
+        The thresholds to be used by the model. Their amount needs to correspond to the type of classification we want to do. If we want to do three class classification, there need to be two thresholds, for both binary classifications, there needs to be just one.
+
+        **return_type : str**
+
+        This is how long will be the returned values. For mode full, the values of the length of the input signal will be used. The other mode, intervals, means that there will be a value returned for each short interval where the score does not change. These intervals are always the length of the stride in real values. For each of these intervals, there will be just one value returned.
+
+        **sampling_rate : int**
+
+        The models currently only support 250 Hz. Using any other frequency will result in fail. Slightly different frequencies can theoretically be used, but that is to be done at your own risk.
+
+        **clean_data : bool**
+
+        Whether the data should be cleaned before processing. The models were trained on cleaned data so this is advised unless you already cleaned data beforehand. For cleaning, we are using neurokit2 function ecg_clean with its default settings as of version 0.2.4.
+
+
+
+
+        :param model: Model to be used
+        :param stride: The soze of the step of the moving window
+        :param return_mode: The type of classification to be done by the class
+        :param thresholds: The thresholds to be used when and if other return_mode than socre is chosen
+        :param return_type: how mnay values should be returned
+        :param sampling_rate: The sampling rate of the ECG signal to be processed, currently just 250 Hz is supported
+        :param clean_data: Whether to clean data before processing them.
+        """
+        # urobime checks vsetkych modelov
+
+        if model not in list(MODEL_PATH_DICT.keys()):
+            raise ValueError(model + ' is not a known model that can be used')
+
+        if return_mode not in ['score', 'three_value', 'binary_clean', 'binary_qrs']:
+            raise ValueError('Return mode needs to be one of: score, three_value, binary_clean, binary_qrs. Currently is ' + str(return_mode))
+
+        if thresholds is None:
+            thresholds = utils.get_default_thresholds(model, return_mode)
+
+
+        if return_mode == 'score':
+            if thresholds is not None:
+                raise ValueError('Threshold count does not correspond to return mode')
+        elif return_mode in ['binary_clean', 'binary_qrs']:
+            if type(thresholds) == float:
+                thresholds = [thresholds]
+            if len(thresholds) != 1:
+                raise ValueError('Threshold count does not correspond to return mode')
+            elif not 0 <= thresholds[0] <= 1.0:
+                raise ValueError('Threshold value not in 0 to 1 interval')
+        elif return_mode == 'three_value':
+            if len(thresholds) != 2:
+                raise ValueError('Threshold count does not correspond to return mode')
+            elif not 0 <= thresholds[0] <= 1.0 or not 0 <= thresholds[1] <= 1.0:
+                raise ValueError('Threshold value not in 0 to 1 interval')
+            thresholds = np.sort(thresholds)
+
+        if return_type not in ['intervals', 'full']:
+            raise ValueError('Return type needs to be one of: intervals, full. Currently is ' + str(return_type))
+
+        if sampling_rate != 250:
+            raise NotImplementedError('This class currently only support ECG with frequency of 250 Hz. Consider modyfing your data to comply with this prerequisite.')
+
+        if stride < 0:
+            raise ValueError('Stride for a model can not be negative')
+
+        self.model = tf_model.tf_model(model)
+
+        self.input_length = self.model.get_input_length()
+
+        self.stride = utils.get_stride_length(self.model.get_input_length(), stride, sampling_rate)
+        self.return_mode = return_mode
+        self.return_type = return_type
+        self.thresholds = thresholds
+        self.sampling_rate = sampling_rate
+        self.clean_data = clean_data
+
+    def process_signal(self, signal):
+        """
+
+        This method processes ECG signal and returns specified values.
+
+        Parameters:
+        --------------
+
+        **signal : list**
+
+        This is the signal to be processed by the object. The ECG needs to be in mV.
+
+
+        Returns:
+        ----------
+
+        **results : list**
+        These are the results. Their specific properties depend on the parameters passed when creating the class.
+
+        :param signal: The ECG to be processed.
+        :return: list - This is the list of the found values. Their specific properties depend on the parameters passed inside constructor.
+        """
+
+
+        if self.return_type == 'full':
+            return self._process_signal_full(signal)
+        elif self.return_type == 'intervals':
+            return self._process_signal_interval(signal)
+
+    def _process_signal_full(self, signal):
+        if self.clean_data:
+            signal = nk.ecg_clean(signal, sampling_rate=self.sampling_rate)
+
+        output = np.zeros_like(signal)
+        win_count = np.zeros_like(signal)
+
+        for win_start in range(0, len(signal)-self.input_length + 1, self.stride):
+            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
+            output[win_start:win_start + self.input_length] = output[win_start:win_start + self.input_length] + score
+            win_count[win_start:win_start + self.input_length] = win_count[win_start:win_start + self.input_length] + 1
+        return self._calc_precise_scores(output, win_count)
+
+    def _process_signal_interval(self, signal):
+
+        if self.clean_data:
+            signal = nk.ecg_clean(signal, sampling_rate=self.sampling_rate)
+
+        output = np.zeros(len(signal) // self.stride)
+        win_count = np.zeros(len(signal) // self.stride)
+
+        for win_start in range(0, len(signal) - self.input_length + 1, self.stride):
+            a = win_start // self.stride
+            b = (win_start + self.input_length) // self.stride
+
+            score = self.model.process_ecg(signal[win_start:win_start + self.input_length])
+            output[a:b] = output[a:b] + score
+            win_count[a:b] = win_count[a:b] + 1
+        return self._calc_precise_scores(output, win_count)
+
+    def _get_binary(self, scores):
+        return [1.0 if x < self.thresholds[0] else 2.0 for x in scores]
+
+
+    def _get_three_value(self, scores):
+
+        def mapper(val):
+            if val < self.thresholds[0]:
+                return 1.0
+            elif val < self.thresholds[1]:
+                return 2.0
+            else:
+                return 3.0
+        return [mapper(x) for x in scores]
+
+    def _calc_precise_scores(self, scores, win_counts):
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            scores = np.divide(scores, win_counts)
+        # scores = scores[~np.isnan(scores)]
+
+        if self.return_mode == 'score':
+            return scores
+        elif self.return_mode in ['binary_clean', 'binary_qrs']:
+            return self._get_binary(scores)
+        elif self.return_mode == 'three_value':
+            return self._get_three_value(scores)
+
+
```

### Comparing `ecg_quality-0.1.2/ecg_quality/model.py` & `ecg_quality-0.1.3/ecg_quality/model.py`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/models/CNN2s.h5` & `ecg_quality-0.1.3/ecg_quality/models/CNN2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/models/CNN5s.h5` & `ecg_quality-0.1.3/ecg_quality/models/CNN5s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/models/LSTM2s.h5` & `ecg_quality-0.1.3/ecg_quality/models/LSTM2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/models/OSCNN2s.h5` & `ecg_quality-0.1.3/ecg_quality/models/OSCNN2s.h5`

 * *Files identical despite different names*

### Comparing `ecg_quality-0.1.2/ecg_quality/tf_model.py` & `ecg_quality-0.1.3/ecg_quality/tf_model.py`

 * *Files identical despite different names*

