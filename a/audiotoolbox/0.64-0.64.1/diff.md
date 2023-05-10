# Comparing `tmp/audiotoolbox-0.64-py3-none-any.whl.zip` & `tmp/audiotoolbox-0.64.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 49674 bytes, number of entries: 21
+Zip file size: 49706 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      425 b- defN 22-Aug-15 12:42 audiotools/__init__.py
--rw-rw-r--  2.0 unx    53186 b- defN 23-May-02 00:40 audiotools/audiotools.py
+-rw-rw-r--  2.0 unx    53167 b- defN 23-May-10 01:04 audiotools/audiotools.py
 -rw-rw-r--  2.0 unx     1139 b- defN 21-Jul-02 20:55 audiotools/auditory_filter.py
 -rw-rw-r--  2.0 unx     3644 b- defN 21-Aug-20 11:41 audiotools/interfaces.py
 -rw-rw-r--  2.0 unx     3684 b- defN 22-Sep-26 08:51 audiotools/wav.py
--rw-rw-r--  2.0 unx      299 b- defN 22-Sep-26 08:51 audiotools/filter/__init__.py
+-rw-rw-r--  2.0 unx      299 b- defN 23-May-02 01:34 audiotools/filter/__init__.py
 -rw-rw-r--  2.0 unx     1121 b- defN 21-Aug-20 11:41 audiotools/filter/brickwall_filt.py
--rw-rw-r--  2.0 unx     4694 b- defN 22-Oct-20 08:07 audiotools/filter/butterworth_filt.py
+-rw-rw-r--  2.0 unx     4694 b- defN 23-May-02 01:30 audiotools/filter/butterworth_filt.py
 -rw-rw-r--  2.0 unx     3658 b- defN 22-Aug-15 12:42 audiotools/filter/filter.py
--rw-rw-r--  2.0 unx     6267 b- defN 22-Sep-26 08:51 audiotools/filter/filterbank.py
+-rw-rw-r--  2.0 unx     6267 b- defN 23-May-02 01:34 audiotools/filter/filterbank.py
 -rw-rw-r--  2.0 unx     5186 b- defN 22-Oct-20 08:07 audiotools/filter/gammatone_filt.py
 -rw-rw-r--  2.0 unx       55 b- defN 21-Aug-20 11:41 audiotools/oaudio/__init__.py
 -rw-rw-r--  2.0 unx     6153 b- defN 22-Oct-20 08:07 audiotools/oaudio/base_signal.py
--rw-rw-r--  2.0 unx     5748 b- defN 23-May-02 00:40 audiotools/oaudio/freqdomain_signal.py
+-rw-rw-r--  2.0 unx     5775 b- defN 23-May-10 01:04 audiotools/oaudio/freqdomain_signal.py
 -rw-rw-r--  2.0 unx    26645 b- defN 23-May-02 00:21 audiotools/oaudio/signal.py
 -rw-rw-r--  2.0 unx     1132 b- defN 22-Oct-20 08:07 audiotools/oaudio/stats.py
--rw-r--r--  2.0 unx    35148 b- defN 23-May-02 01:00 audiotoolbox-0.64.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2173 b- defN 23-May-02 01:00 audiotoolbox-0.64.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 01:00 audiotoolbox-0.64.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-02 01:00 audiotoolbox-0.64.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1779 b- defN 23-May-02 01:00 audiotoolbox-0.64.dist-info/RECORD
-21 files, 162239 bytes uncompressed, 46774 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx    35148 b- defN 23-May-10 01:07 audiotoolbox-0.64.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2175 b- defN 23-May-10 01:07 audiotoolbox-0.64.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-10 01:07 audiotoolbox-0.64.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-10 01:07 audiotoolbox-0.64.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1789 b- defN 23-May-10 01:07 audiotoolbox-0.64.1.dist-info/RECORD
+21 files, 162259 bytes uncompressed, 46786 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: audiotools/oaudio/signal.py
 Comment: 
 
 Filename: audiotools/oaudio/stats.py
 Comment: 
 
-Filename: audiotoolbox-0.64.dist-info/LICENSE
+Filename: audiotoolbox-0.64.1.dist-info/LICENSE
 Comment: 
 
-Filename: audiotoolbox-0.64.dist-info/METADATA
+Filename: audiotoolbox-0.64.1.dist-info/METADATA
 Comment: 
 
-Filename: audiotoolbox-0.64.dist-info/WHEEL
+Filename: audiotoolbox-0.64.1.dist-info/WHEEL
 Comment: 
 
-Filename: audiotoolbox-0.64.dist-info/top_level.txt
+Filename: audiotoolbox-0.64.1.dist-info/top_level.txt
 Comment: 
 
-Filename: audiotoolbox-0.64.dist-info/RECORD
+Filename: audiotoolbox-0.64.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## audiotools/audiotools.py

```diff
@@ -1832,15 +1832,15 @@
 
     # calculate analytical signal and its spectrum
     fsig = sig.to_freqdomain().to_analytical()
     asig = fsig.to_timedomain()
 
     # calculate coherence by convolving first channel with complex
     # conjugate of the second channel (done by multiplying fft)
-    coh = ((fsig.ch[0] * fsig.ch[1].conj()) / sig.n_samples**2).to_timedomain()
+    coh = ((fsig.ch[0] * fsig.ch[1].conj())).to_timedomain()
 
     # normalize by energy so that we gain the normalized coherence function
     coh /= np.sqrt(np.product(np.mean(np.abs(asig)**2, axis=0), axis=0))
 
     # if input was an ndarray convert output back to ndarray
     coh[:] = np.roll(coh, coh.n_samples//2, axis=0)
```

## audiotools/oaudio/freqdomain_signal.py

```diff
@@ -184,19 +184,20 @@
         Returns:
         --------
         The timedomain representation: Signal
 
         """
 
         # revert normalization
-        self *= self.n_samples
-        wv = np.fft.ifft(self, axis=0)
+        fsig = self.copy()
+        fsig *= fsig.n_samples
+        wv = np.fft.ifft(fsig, axis=0)
         wv = np.real_if_close(wv)
-        signal = audio.Signal(self.n_channels, self.duration,
-                              self.fs, dtype=wv.dtype)
+        signal = audio.Signal(fsig.n_channels, fsig.duration,
+                              fsig.fs, dtype=wv.dtype)
         signal[:] = wv
         return signal
 
     def to_analytical(self):
         """Convert spectrum to analytical signal
 
         Converts the spectrum to that of the equivalent analytical
```

## Comparing `audiotoolbox-0.64.dist-info/LICENSE` & `audiotoolbox-0.64.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `audiotoolbox-0.64.dist-info/METADATA` & `audiotoolbox-0.64.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiotoolbox
-Version: 0.64
+Version: 0.64.1
 Summary: Toolbox for generating and working with audio signals
 Home-page: https://jencke.github.io/audiotools/
 Author: Jörg Encke
 Author-email: joerg.encke@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Sound/Audio
```

## Comparing `audiotoolbox-0.64.dist-info/RECORD` & `audiotoolbox-0.64.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 audiotools/__init__.py,sha256=kQqqK8JFrSUZ_kdQEPPf64jAq-MMXQHIQ3U0WIuKzX4,425
-audiotools/audiotools.py,sha256=IaCsoqyDx1AxyC5xFs3UnOI4S7C_fmEUPku7EC2kXzQ,53186
+audiotools/audiotools.py,sha256=QL5UXnNyIkq6qONQRrQGF0O1iVRwGcLLA2faOsVovLY,53167
 audiotools/auditory_filter.py,sha256=PZek07yjF7JXbeovj5woWVY4DQkQXk3GJaQn6r__sfs,1139
 audiotools/interfaces.py,sha256=GCatZhboHL4oF_D6YZeqa7Cf1xg9jy51GqLOR5PXEbo,3644
 audiotools/wav.py,sha256=La8U4LL4kSTeylpowbiMOKGxTPkZawXRWy_Rbml-LtM,3684
 audiotools/filter/__init__.py,sha256=HSKXXu5dSt0yzxE1ps59oaGjbMV5QI6-8hv-m_fsL-I,299
 audiotools/filter/brickwall_filt.py,sha256=ra2Xr20jw-fR1Q-S9R9iZONIKbm9pu18-aYTid2xgr8,1121
 audiotools/filter/butterworth_filt.py,sha256=VNhuR2T7me7SDRemX9ElSHTIUI0waEOmwRQM5qeKJ-M,4694
 audiotools/filter/filter.py,sha256=fLKV0UY3CGUKt4PBUf-shsjm_lrLWdz3TFrLrrllZmo,3658
 audiotools/filter/filterbank.py,sha256=oZ8ZVfAvk5fWwmsKHn9g7sC58mALiqR3504E5kln-yM,6267
 audiotools/filter/gammatone_filt.py,sha256=50wYFLclbG8DK6Bc6wJ9IQ2IeNj00V6TxSENH0J_nO4,5186
 audiotools/oaudio/__init__.py,sha256=vOl_qDiXORz6ZRomIHg3hiqn9DVSUXtLWgVnRMqdtGE,55
 audiotools/oaudio/base_signal.py,sha256=7Y2JwCoDjPCTmN6SKA8O6Z4KEoto3Z7-2_bEzQhxQjQ,6153
-audiotools/oaudio/freqdomain_signal.py,sha256=1hNd_g2RX4kJhzGBxCHGGVA2i6HZLZ03nTBY-tiFYpE,5748
+audiotools/oaudio/freqdomain_signal.py,sha256=uct2LIyo_OIyqP0M1gOJ0M7dTMnULM-CdNQ65bC5BiI,5775
 audiotools/oaudio/signal.py,sha256=BmQbbbyf2lLlaU-UEq_oBSd7z7IP2sB1Jj7q-hSu4GI,26645
 audiotools/oaudio/stats.py,sha256=FjQN4iJQos0yF6GZM0IdkQnPqXidStJisMNHyX0kO9I,1132
-audiotoolbox-0.64.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-audiotoolbox-0.64.dist-info/METADATA,sha256=ciPshsMWLQRuqo3mbccZfiLYFiUiERAJ1nf4d2LsWe4,2173
-audiotoolbox-0.64.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-audiotoolbox-0.64.dist-info/top_level.txt,sha256=LAgV3Ghq1Of8ioRlBxjMpwxXMZ-kkLOea5jnXzsru3w,11
-audiotoolbox-0.64.dist-info/RECORD,,
+audiotoolbox-0.64.1.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+audiotoolbox-0.64.1.dist-info/METADATA,sha256=5tlJrzlcissPgzLBkp__WP-4LQZbyvNTWstc5Xvesto,2175
+audiotoolbox-0.64.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+audiotoolbox-0.64.1.dist-info/top_level.txt,sha256=LAgV3Ghq1Of8ioRlBxjMpwxXMZ-kkLOea5jnXzsru3w,11
+audiotoolbox-0.64.1.dist-info/RECORD,,
```

