# Comparing `tmp/imcascade-1.0.tar.gz` & `tmp/imcascade-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imcascade-1.0.tar", last modified: Wed Sep 29 00:35:46 2021, max compression
+gzip compressed data, was "imcascade-1.1.tar", last modified: Fri Apr  7 15:28:49 2023, max compression
```

## Comparing `imcascade-1.0.tar` & `imcascade-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2021-09-29 00:35:46.287839 imcascade-1.0/
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1071 2021-05-21 21:48:33.000000 imcascade-1.0/LICENSE
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)       43 2021-09-27 15:30:06.000000 imcascade-1.0/MANIFEST.in
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     2382 2021-09-29 00:35:46.283916 imcascade-1.0/PKG-INFO
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1433 2021-09-29 00:35:02.000000 imcascade-1.0/README.rst
-drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2021-09-29 00:35:46.219745 imcascade-1.0/imcascade/
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)      167 2021-09-28 18:54:22.000000 imcascade-1.0/imcascade/__init__.py
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)    32845 2021-09-28 17:18:42.000000 imcascade-1.0/imcascade/fitter.py
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)    15700 2021-09-20 00:39:57.000000 imcascade-1.0/imcascade/mgm.py
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)    10932 2021-05-24 17:32:14.000000 imcascade-1.0/imcascade/psf_fitter.py
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)    28664 2021-09-20 01:25:48.000000 imcascade-1.0/imcascade/results.py
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     5310 2021-07-05 20:26:16.000000 imcascade-1.0/imcascade/utils.py
-drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2021-09-29 00:35:46.279908 imcascade-1.0/imcascade.egg-info/
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     2382 2021-09-29 00:35:45.000000 imcascade-1.0/imcascade.egg-info/PKG-INFO
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)      343 2021-09-29 00:35:45.000000 imcascade-1.0/imcascade.egg-info/SOURCES.txt
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)        1 2021-09-29 00:35:45.000000 imcascade-1.0/imcascade.egg-info/dependency_links.txt
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)       43 2021-09-29 00:35:45.000000 imcascade-1.0/imcascade.egg-info/requires.txt
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)       10 2021-09-29 00:35:45.000000 imcascade-1.0/imcascade.egg-info/top_level.txt
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)       43 2021-05-21 21:54:04.000000 imcascade-1.0/requirements.txt
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)       38 2021-09-29 00:35:46.287839 imcascade-1.0/setup.cfg
--rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1195 2021-09-28 21:58:01.000000 imcascade-1.0/setup.py
+drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2023-04-07 15:28:49.971887 imcascade-1.1/
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1071 2021-05-21 21:48:33.000000 imcascade-1.1/LICENSE
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)       43 2021-09-27 15:30:06.000000 imcascade-1.1/MANIFEST.in
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     2346 2023-04-07 15:28:49.970221 imcascade-1.1/PKG-INFO
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1582 2023-04-07 15:28:25.000000 imcascade-1.1/README.rst
+drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2023-04-07 15:28:49.946247 imcascade-1.1/imcascade/
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)      167 2023-03-10 18:03:12.000000 imcascade-1.1/imcascade/__init__.py
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)    33657 2023-04-07 14:46:41.000000 imcascade-1.1/imcascade/fitter.py
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)    16113 2023-03-10 18:03:12.000000 imcascade-1.1/imcascade/mgm.py
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)    11642 2023-03-10 18:03:12.000000 imcascade-1.1/imcascade/psf_fitter.py
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)    32225 2023-04-07 14:46:41.000000 imcascade-1.1/imcascade/results.py
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     5541 2023-03-10 18:03:12.000000 imcascade-1.1/imcascade/utils.py
+drwxrwxrwx   0 tbm       (1000) tbm       (1000)        0 2023-04-07 15:28:49.969151 imcascade-1.1/imcascade.egg-info/
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     2346 2023-04-07 15:28:49.000000 imcascade-1.1/imcascade.egg-info/PKG-INFO
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)      343 2023-04-07 15:28:49.000000 imcascade-1.1/imcascade.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)        1 2023-04-07 15:28:49.000000 imcascade-1.1/imcascade.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)       43 2023-04-07 15:28:49.000000 imcascade-1.1/imcascade.egg-info/requires.txt
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)       10 2023-04-07 15:28:49.000000 imcascade-1.1/imcascade.egg-info/top_level.txt
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)       42 2023-03-10 18:03:12.000000 imcascade-1.1/requirements.txt
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)       38 2023-04-07 15:28:49.972116 imcascade-1.1/setup.cfg
+-rwxrwxrwx   0 tbm       (1000) tbm       (1000)     1186 2023-04-07 15:18:02.000000 imcascade-1.1/setup.py
```

### Comparing `imcascade-1.0/LICENSE` & `imcascade-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imcascade-1.0/PKG-INFO` & `imcascade-1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: imcascade
-Version: 1.0
+Version: 1.1
 Summary: imcascade: Fitting astronomical images using a 'cascade' of Gaussians
 Home-page: https://github.com/tbmiller-astro/imcascade
 Author: Tim Miller
 Author-email: tim.miller@yale.edu
 License: MIT
-Description: imcascade
-        =========
-        
-        |Docs|
-        |License|
-        |Arxiv|
-        
-        ``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method here (Link to come soon) and the documentation `here <https://imcascade.readthedocs.io>`_.
-        
-        Citation
-        --------
-        ``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite Miller & van Dokkum (2021) (Link to paper forthcoming)
-        
-        Help and Issues
-        ---------------
-        ``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`_. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
-        
-        .. |Docs| image:: https://readthedocs.org/projects/imcascade/badge/?version=latest
-           :target: http://imcascade.readthedocs.io/?badge=latest
-        .. |License| image:: https://img.shields.io/badge/license-MIT-blue
-        .. |Arxiv| image:: https://img.shields.io/badge/arXiv-2109.13262-blue
-           :target: https://arxiv.org/abs/2109.13262
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+imcascade
+=========
+
+|Docs|
+|License|
+|Arxiv|
+|pypi|
+
+``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method `here <https://arxiv.org/abs/2109.13262>`__  and the documentation `here <https://imcascade.readthedocs.io>`__.
+
+Citation
+--------
+``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite `Miller & van Dokkum (2021) <https://arxiv.org/abs/2109.13262>`__
+
+Help and Issues
+---------------
+``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`__. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
+
+.. |Docs| image:: https://readthedocs.org/projects/imcascade/badge/?version=latest
+   :target: http://imcascade.readthedocs.io/?badge=latest
+.. |License| image:: https://img.shields.io/badge/license-MIT-blue
+.. |Arxiv| image:: https://img.shields.io/badge/arXiv-2109.13262-blue
+   :target: https://arxiv.org/abs/2109.13262
+.. |pypi| image:: http://img.shields.io/pypi/v/imcascade.svg
+   :target: https://pypi.org/project/imcascade/
```

### Comparing `imcascade-1.0/README.rst` & `imcascade-1.1/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 imcascade
 =========
 
 |Docs|
 |License|
 |Arxiv|
+|pypi|
 
-``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method here (Link to come soon) and the documentation `here <https://imcascade.readthedocs.io>`_.
+``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method `here <https://arxiv.org/abs/2109.13262>`__  and the documentation `here <https://imcascade.readthedocs.io>`__.
 
 Citation
 --------
-``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite Miller & van Dokkum (2021) (Link to paper forthcoming)
+``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite `Miller & van Dokkum (2021) <https://arxiv.org/abs/2109.13262>`__
 
 Help and Issues
 ---------------
-``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`_. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
+``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`__. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
 
 .. |Docs| image:: https://readthedocs.org/projects/imcascade/badge/?version=latest
    :target: http://imcascade.readthedocs.io/?badge=latest
 .. |License| image:: https://img.shields.io/badge/license-MIT-blue
 .. |Arxiv| image:: https://img.shields.io/badge/arXiv-2109.13262-blue
    :target: https://arxiv.org/abs/2109.13262
+.. |pypi| image:: http://img.shields.io/pypi/v/imcascade.svg
+   :target: https://pypi.org/project/imcascade/
```

### Comparing `imcascade-1.0/imcascade/fitter.py` & `imcascade-1.1/imcascade/fitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-import numpy as np
+from asyncio.log import logger
+from cmath import log
+import importlib
 import asdf
 import logging
-from scipy.optimize import least_squares
-from scipy.stats import norm, truncnorm
+from scipy.optimize import least_squares,minimize,Bounds
+from scipy.stats import norm, truncnorm,cauchy
+import numpy as np
 
 from imcascade.mgm import MultiGaussModel
-from imcascade.results import ImcascadeResults,vars_to_use
-from imcascade.utils import dict_add, guess_weights,log_scale,expand_mask
+from imcascade.utils import dict_add, guess_weights,log_scale,expand_mask,vars_to_use
 from astropy.stats.biweight import biweight_location as bwl
 from astropy.stats.biweight import biweight_scale as bws
+from astropy.io import fits
 
 import dynesty
 from dynesty import utils as dyfunc
 
+
+
 log2pi = np.log(2.*np.pi)
 
+
 def initialize_fitter(im, psf, mask = None, err = None, x0 = None,y0 = None, re = None, flux = None,
- psf_oversamp = 1, sky_model = True, log_file = None, readnoise = None, gain = None, exp_time = None):
+ psf_oversamp = 1, sky_model = True, log_file = None, readnoise = None, gain = None, exp_time = None, num_components = None,
+ component_widths = None, log_weight_scale = True):
     """Function used to help Initialize Fitter instance from simple inputs
 
     Parameters
     ----------
     im: str or 2D Array
         The image or cutout to be fit with imcascade. If a string is given, it is
         interpretted as the location of a fits file with the cutout in it's first HDU.
@@ -93,64 +100,61 @@
     if psf is not None:
         #Find best fit gaussian decomposition of PSF
         psf_sig,psf_a = pfitter.auto_fit()
         logger.info("Fit PSF with %i components"%len(psf_sig))
         logger.info("Widths: "+ ','.join(map(str,np.round(psf_sig,2))) )
         logger.info("Fluxes: "+ ','.join(map(str,np.round(psf_a,2))))
 
-        #Calculate hwhm
-        psf_mp = np.ones(4+len(psf_sig))
-        psf_mp[4:] = psf_a
-        rdict = {'sig':psf_sig, 'Ndof':4+len(psf_sig), 'Ndof_gauss':len(psf_sig), 'Ndof_sky':0, 'log_weight_scale':False,'min_param':psf_mp, 'sky_model':False}
-        psf_res = ImcascadeResults(rdict)
-        psf_hwhm = psf_res.calc_iso_r(psf_res.calc_sbp(np.array([0,]))/2)
-
-        if psf_hwhm > 1:
-            sig_min = psf_hwhm*0.5
-        else:
-            sig_min = 0.5
-    else:
-        sig_min = 0.75
-
+    
+    
     #Load image data
     if type(im) == str:
         im_fits = fits.open(im)
         im_data = im_fits[0].data
     elif type(im) == np.ndarray:
         im_data = im.copy()
 
     if im_data.dtype.byteorder == '>':
         im_data = im_data.byteswap().newbyteorder()
 
     #Use sep to estimate object properties and rms depending
     import sep
-    bkg = sep.Background(im_data, bw = 16,bh = 16)
-    obj,seg = sep.extract(im_data, 2., err = bkg.globalrms, segmentation_map = True, deblend_cont=1e-4)
+    bkg = sep.Background(im_data, bw = 32,bh = 32)
+    obj,seg = sep.extract(im_data, 2.5, err = bkg.globalrms, segmentation_map = True, deblend_cont=1e-3)
     seg_obj = seg[int(x0), int(y0)]
 
     if re is None:
         a_guess = obj['a'][seg_obj-1]
     else:
         a_guess = re
 
     if flux is None:
         fl_guess = obj['flux'][seg_obj-1]
     else:
         fl_guess = None
-    sig_max = a_guess*9
+    sig_min = 0.75
+    sig_max = a_guess*8
 
     init_dict = {'re':a_guess, 'flux':fl_guess, 'sky0':bkg.globalback, 'x0':x0, 'y0':y0}
 
     #Calculate widths of components
-    if im_data.shape[0] > 100:
-        num_sig = 9
+    
+    if num_components is None:
+        if im_data.shape[0] > 100:
+            num_sig = 9
+        else:
+            num_sig = 7
     else:
-        num_sig = 7
-    sig_use = log_scale(sig_min,sig_max, num_sig)
-    logger.info("Using %i components with logarithmically spaced widths to fit galaxy"%num_sig)
+        num_sig = num_components
+
+    if component_widths is None:
+        sig_use = log_scale(sig_min,sig_max, num_sig)
+    else:
+        sig_use = component_widths.copy()
+    logger.info("Using %i components with logarithmically spaced widths to fit galaxy"%(len(sig_use) ) )
     logger.info(", ".join(map(str,np.round(sig_use,2))))
 
     #Use sep results to estimate mask
     if mask is None:
         logger.info("No mask was given, derriving one using sep")
         mask = np.copy(seg)
         mask[np.where(seg == seg_obj)] = 0
@@ -168,15 +172,15 @@
         logger.info("Using gain, exp_time and readnoise to calculate pixel weights")
     else:
         #If no info is given then default to sep results which do pretty well
         logger.info("Using sep rms map to calculate pixel weights")
         pix_weights = 1./bkg.rms()**2
 
     #Initalize Fitter
-    return Fitter(im_data,sig_use, psf_sig,psf_a, weight = pix_weights, mask = mask, init_dict = init_dict, sky_model = sky_model, log_file = log_file)
+    return Fitter(im_data,sig_use, psf_sig,psf_a, weight = pix_weights, mask = mask, init_dict = init_dict, sky_model = sky_model, log_file = log_file,log_weight_scale = log_weight_scale)
 
 
 def fitter_from_ASDF(file_name, init_dict= {}, bounds_dict = {}):
     """ Function used to initalize a fitter from a saved asdf file
 
     This can be useful for re-running or for initializing a series
     of galaxies beforehand and then transferring to somewhere else or running in
@@ -267,15 +271,15 @@
         Dictionary specifying boundss for least_squares fitting and priors. The code
         is desigined to make 'intelligent' guesses if none are provided
 """
     def __init__(self, img, sig, psf_sig, psf_a, weight = None, mask = None,\
       sky_model = True,sky_type = 'tilted-plane', render_mode = 'hybrid', log_weight_scale = True, verbose = True,
       psf_shape = None,init_dict = {}, bounds_dict = {}, log_file = None):
         """Initialize a Task instance"""
-        self.img  = img
+        self.img  = np.asarray(img)
         self.verbose = verbose
         
         if log_file is None:
             handler = logging.StreamHandler()
         else:
             handler = logging.FileHandler(log_file)
 
@@ -295,22 +299,22 @@
             if verbose: self.logger.info('No PSF input, running in non-psf mode')
 
         if weight is None:
             self.weight = np.ones(img.shape)
         else:
             if weight.shape != self.img.shape:
                 raise ValueError("'weight' array must have same shape as 'img'")
-            self.weight = weight
+            self.weight = np.asarray(weight)
 
 
         if mask is not None:
             if self.weight.shape != self.img.shape:
                 raise ValueError("'mask' array must have same shape as 'img' ")
             self.weight[np.where(mask == 1)] = 0
-            self.mask = mask
+            self.mask = np.asarray(mask)
         else:
             self.mask = np.zeros(self.img.shape)
 
         if np.sum(np.isnan(self.img) + np.sum(np.isnan(self.weight))) > 0:
             where_inf = np.where(np.isnan(self.img) + np.isnan(self.weight))
             self.logger.info("Masking nan values at locations:")
             self.logger.info(where_inf)
@@ -420,14 +424,15 @@
             self.param_init[4+self.Ndof_gauss+i] = init_dict['sky%i'%i]
             self.lb.append(bounds_dict['sky%i'%i][0] )
             self.ub.append(bounds_dict['sky%i'%i][1] )
 
         self.lb = np.asarray(self.lb)
         self.ub = np.asarray(self.ub)
         self.bnds = (self.lb,self.ub)
+        self.init_dict = init_dict
 
     def resid_1d(self,params):
         """ Given a set of parameters returns the 1-D flattened residuals
         when compared to the Data, to be used in run_ls_min Function
 
         Parameters
         ----------
@@ -459,15 +464,15 @@
         min_param: 1D array
             Returns a 1D array containing the optimized parameters that describe
             the best fit model.
 """
         if self.verbose: self.logger.info('Running least squares minimization')
         min_res = least_squares(self.resid_1d, self.param_init, bounds = self.bnds, **ls_kwargs)
         self.min_res = min_res
-        self.min_param = min_res.x
+        self.min_param = self.min_res.x
         if self.verbose: self.logger.info('Finished least squares minimization')
 
         return self.min_param
 
     def set_up_express_run(self, set_params = None):
         """ Function to set up 'express' run using pre-rendered images with a
         fixed x0,y0, phi and q. Sets class attribute 'express_gauss_arr' which
@@ -536,14 +541,21 @@
             sig = np.sqrt(np.diag(cov))[4:]
 
 
             #Set width to reasonable value if really big
             sig = sig*2.
             sig[sig>1] = 1.
             self._exp_pri_scales = sig.copy()
+        
+        self._lin_cauchy_locs = guess_weights(self.sig, self.init_dict['re'], self.init_dict['flux'])
+        self._lin_cauchy_scales = self._lin_cauchy_locs/3.
+        
+        if self.sky_model:
+            self._lin_cauchy_locs = np.append(self._lin_cauchy_locs, np.array([0,0,0]))
+            self._lin_cauchy_scales = np.append(self._lin_cauchy_scales, np.array([1e-3,1e-3,1e-3]))
         return stack
 
     def make_express_model(self, exp_params):
         """Function to generate a model for a given set of paramters,
         specifically using the pre-renedered model for the 'express' mode
 
         Parameters
@@ -580,15 +592,15 @@
             List of parameters to define model
         Returns
         -------
         chi^2: float
             Chi squared statistic for the given set of parameters
 """
         model = self.make_model(params)
-        return np.sum( (self.img - model)**2 *self.weight - self.log_weight + np.log(2*np.pi) )
+        return ( (self.img - model)**2 *self.weight - self.log_weight + np.log(2*np.pi) ).sum()
 
     def log_like(self,params):
         """Function to calculate the log likeliehood for a given set of paramters
 
         Parameters
         ----------
         params: Array
@@ -644,15 +656,15 @@
 
         Returns
         -------
         log likeliehood: float
             log likeliehood for a given set of paramters, defined as -0.5*chi^2
 """
         model = self.make_express_model(exp_params)
-        return -0.5*np.sum( (self.img - model)**2 *self.weight ) + self.loglike_const
+        return -0.5*( (self.img - model)**2 *self.weight ).sum() + self.loglike_const
 
     def ptform_exp_ls(self, u):
         """Prior transformation function to be used in dynesty 'express' mode using
         gaussian priors defined by the results of the least_squares minimization
 
         Parameters
         ----------
@@ -661,14 +673,30 @@
 
         Returns
         -------
         x: array
             array containing distribution of parameters from prior
 """
         return norm.ppf(u, loc = self._exp_pri_locs, scale = self._exp_pri_scales)
+    
+    def ptform_exp_lin_cauchy(self, u):
+        """Prior transformation function to be used in dynesty 'express' mode using
+        gaussian priors defined by the results of the least_squares minimization
+
+        Parameters
+        ----------
+        u: array
+            array of random numbers from 0 to 1
+
+        Returns
+        -------
+        x: array
+            array containing distribution of parameters from prior
+"""
+        return cauchy.ppf(u, loc = self._lin_cauchy_locs, scale = self._lin_cauchy_scales)
 
     def ptform_exp_unif(self, u):
         """Prior transformation function to be used in dynesty 'express' mode using
         unifrom priors defined by self.lb and self.ub
 
         Parameters
         ----------
@@ -710,30 +738,54 @@
         Returns
         -------
         Posterior: Array
             posterior distribution derrived. If method is 'express', the first 4 columns,
             containg x0, y0, PA and q, are all the same and equal to values used to pre-render the images
 """
         if self.verbose: self.logger.info('Running dynesty using the %s method'%method)
+
+
         if method == 'full':
             ndim = self.Ndof
             sampler = dynesty.DynamicNestedSampler( self.log_like, self.ptform, ndim= ndim, **sampler_kwargs)
         if method == 'express':
+            jax_check = importlib.util.find_spec('jax')
+        
+            if jax_check is None:
+                log_like_use = self.log_like_exp
+            else:
+                logger.info("jax module found, importing and 'jit'-ing likelihood function")
+                from jax import jit, numpy as jnp
+
+                #Convert to JAX array to allow jitting
+                self.img = jnp.array(self.img)
+                self.weight = jnp.array(self.weight)
+                log_like_use = jit(self.log_like_exp)
+            
             ndim = self.Ndof_gauss + self.Ndof_sky
             if not hasattr(self, 'express_gauss_arr'):
                 if self.verbose: self.logger.info('Setting up pre-rendered images')
                 _ = self.set_up_express_run()
+            
             if prior == 'min_results':
-                sampler = dynesty.DynamicNestedSampler( self.log_like_exp, self.ptform_exp_ls, ndim= ndim, **sampler_kwargs)
+                sampler = dynesty.DynamicNestedSampler( log_like_use, self.ptform_exp_ls, ndim= ndim, **sampler_kwargs)
             elif prior == 'uniform':
-                sampler = dynesty.DynamicNestedSampler( self.log_like_exp, self.ptform_exp_unif, ndim= ndim, **sampler_kwargs)
+                sampler = dynesty.DynamicNestedSampler( log_like_use, self.ptform_exp_unif, ndim= ndim, **sampler_kwargs)
+            elif prior == 'cauchy':
+                self.log_weight_scale = False
+                sampler = dynesty.DynamicNestedSampler( log_like_use, self.ptform_exp_lin_cauchy, ndim= ndim, **sampler_kwargs)
             else:
-                raise ("Chosen prior must be either 'min_results' or 'uniform' ")
+                raise ("Chosen prior must be either 'min_results', 'uniform' or 'cauchy'")
+        
         sampler.run_nested(**run_nested_kwargs)
 
+        #Reset to Numpy if jax was used
+        self.img = np.array(self.img)
+        self.weight = np.array(self.weight)
+
         if self.verbose: self.logger.info('Finished running dynesty, calculating posterior')
         self.dynesty_sampler = sampler
         res_cur = sampler.results
         self.logz = res_cur.logz[-1]
         self.logz_err = res_cur.logzerr[-1]
         dyn_samples, dyn_weights = res_cur.samples, np.exp(res_cur.logwt - res_cur.logz[-1])
         post_samp = dyfunc.resample_equal(dyn_samples, dyn_weights)
@@ -743,49 +795,32 @@
         else:
             set_arr = self.exp_set_params[:,np.newaxis] *np.ones((4,post_samp.shape[0] ) )
             set_arr = np.transpose(set_arr)
             self.posterior = np.hstack([set_arr, post_samp])
         self.post_method = 'dynesty-'+method
         return self.posterior
 
-
-    def save_results(self,file_name, run_basic_analysis = True, thin_posterior = 1, zpt = None, cutoff = None, errp_lo = 16, errp_hi =84):
+    def save_results(self,file_name):
         """Function to save results after run_ls_min, run_dynesty and/or run_emcee is performed. Will be saved as an ASDF file.
 
         Parameters
         ----------
         file_name: str
             Str defining location of where to save data
-        run_basic_analysis: Bool (default True)
-            If true will run ImcascadeResults.run_basic_analysis
-
         Returns
         -------
-        Posterior: Array
-            posterior distribution derrived. If method is 'express', the first 4 columns,
-            containg x0,y0,PA and q, are all the same and equal to values used to pre-rended the images
+        dict_saved: dict
+            Dictionary containing all the save quantities
 """
-        if run_basic_analysis:
-            if self.verbose: self.logger.info('Saving results to: %s'%file_name)
-            if self.verbose: self.logger.info('Running basic morphological analysis')
-
-            res = ImcascadeResults(self, thin_posterior = thin_posterior)
-            res_dict = res.run_basic_analysis(zpt = zpt, cutoff = cutoff, errp_lo = errp_lo, errp_hi =errp_hi,\
-              save_results = True , save_file = file_name)
-            if self.verbose:
-                for key in res_dict:
-                    self.logger.info('%s = '%(key) + str(res_dict[key]))
-            return res
-        else:
-            if self.verbose: self.logger.info('Saving results to: %s'%file_name)
-            #If analysis is not to be run then simply save the important contents of the class
-            dict_to_save = {}
-            for key in vars_to_use:
-                try:
-                    dict_to_save[key] = vars(self)[key]
-                except:
-                    continue
 
-            file = asdf.AsdfFile(dict_to_save)
-            file.write_to(file_name)
+        if self.verbose: self.logger.info('Saving results to: %s'%file_name)
+        #If analysis is not to be run then simply save the important contents of the class
+        dict_to_save = {}
+        for key in vars_to_use:
+            try:
+                dict_to_save[key] = vars(self)[key]
+            except:
+                continue
+        file = asdf.AsdfFile(dict_to_save)
+        file.write_to(file_name)
 
-            return dict_to_save
+        return dict_to_save
```

### Comparing `imcascade-1.0/imcascade/mgm.py` & `imcascade-1.1/imcascade/mgm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy.special import erf
 from scipy.ndimage import rotate,shift
+from scipy.ndimage import map_coordinates
 from numba import njit
 
 class MultiGaussModel():
     """A class used to generate models based series of Gaussians
 
     Parameters
     ----------
@@ -138,16 +139,16 @@
         Returns
         -------
         erf_model: array
             Array representing each rendered component
 """
         X_use = self.X_lg[:,:,None] - (x0 + self._lg_fac_x)
         Y_use = self.Y_lg[:,:,None] - (y0 + self._lg_fac_y)
-        c_x = 1./(np.sqrt(2*final_var))
-        c_y = 1./(np.sqrt(2*final_var)*final_q)
+        c_x = 1./(np.sqrt(2.*final_var))
+        c_y = 1./(np.sqrt(2.*final_var)*final_q)
 
         unrotated_stack = final_a/4.*( ( erf(c_x*(X_use-0.5)) - erf(c_x*(X_use+0.5)) )* ( erf(c_y*(Y_use-0.5)) - erf(c_y*(Y_use+0.5)) ) )
         return unrotated_stack
 
     def get_hybrid_stack(self,x0, y0, final_q, final_a, final_var):
         """ Function used to calculate render model using the hybrid method, which uses erf where neccesary to ensure accurate integration and gauss otherwise. Also set everything >5 sigma away to 0.
 
@@ -250,24 +251,24 @@
             return model_im + self.get_sky_model(param[-self.Ndof_sky:])
 
     def get_sky_model_flat(self,args):
         """ Function used to calculate flat sky model
 
         Parameters
                     ----------
-        args: (a,) (float,float,float)
+        args: (a,) (float,)
 
         Returns
         -------
         sky_model: 2D Array
             Model for sky background based on given parameters, same shape as 'shape'
 """
-        a = args[0]
+        
 
-        return a
+        return args[0]
             
     def get_sky_model_tp(self,args):
         """ Function used to calculate tilted-plane sky model
 
         Parameters
         ----------
         args: (a,b,c) (float,float,float)
@@ -276,17 +277,27 @@
         c - slope in y direction
 
         Returns
         -------
         sky_model: 2D Array
             Model for sky background based on given parameters, same shape as 'shape'
 """
-        a,b,c = args
 
-        return a + (self.X - self.x_mid)*b + (self.Y - self.y_mid)*c
+        return args[0] + (self.X - self.x_mid)*args[1] + (self.Y - self.y_mid)*args[2]
+
+def rot_im_jax_exp(img,phi,x0,y0):
+    """Experimental, do not use yet!"""
+    x = np.arange(img.shape[0])
+    y = np.arange(img.shape[1])
+    X,Y = np.meshgrid(x,y)
+
+    X_rot = (X - x0)*np.cos(phi) + (Y - y0)*np.sin(phi) + x0
+    Y_rot = -1*(X - x0)*np.sin(phi) + (Y - y0)*np.cos(phi) + y0
+    locs = np.stack([Y_rot,X_rot])
+    return map_coordinates(img,locs, order = 1 )
 
 def rot_im(img,phi,x0,y0):
     """Function to rotate image around a given point
     
     Parameters
     ----------
     img: 2D array
```

### Comparing `imcascade-1.0/imcascade/psf_fitter.py` & `imcascade-1.1/imcascade/psf_fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from astropy.io import fits
 import sep
 from scipy.optimize import least_squares
+from scipy.interpolate import interp1d
 from imcascade.fitter import Fitter
 from imcascade.utils import min_diff_array
 
 class PSFFitter():
     """A Class used to fit Gaussian models to a PSF image
 
 Parameters
@@ -29,18 +30,25 @@
 
 """
     def __init__(self,psf_img,oversamp = 1.):
         """ Initialize a PSFFitter instance
 """
 
         if type(psf_img) == str:
-            fits_file = fits.open(psf_img)
+            try:
+                fits_file = fits.open(psf_img)
+            except:
+                raise TypeError(f"The file '{ psf_img }' could not be opened as a FITS file")
             self.psf_data = np.array(fits_file[0].data, dtype = '<f4')
         elif type(psf_img) == np.ndarray:
+            if psf_img.ndim != 2:
+                raise TypeError("Array must be 2D image of PSF")
             self.psf_data = np.array(psf_img, dtype = '<f4')
+        else:
+            raise TypeError("psf_img must be either a numpy array or string with the location of a FITS file")
         self.oversamp = oversamp
 
         self.cent_pix_x = np.where(self.psf_data == np.max(self.psf_data) )[0][0]
         self.cent_pix_y = np.where(self.psf_data == np.max(self.psf_data) )[1][0]
 
         #calculate 1-D circular profile
         _,_ = self.calc_profile()
@@ -180,20 +188,20 @@
             ax1.set_ylim([np.log10(0.8*min_i), np.log10(2*max_i)])
             ax1.set_ylabel('log ( Intensity)')
             ax1.set_xlabel('Radius (pix)')
             ax1.set_aspect(1./ax1.get_data_ratio())
             ax1.legend(fontsize = 12, frameon = False)
 
             mod = fitter_cur.make_model(param)
-            resid = (self.psf_data - mod)/mod
+            resid = (self.psf_data - mod)
 
-            im2 = ax2.imshow(resid, vmin = -0.5, vmax = 0.5, cmap = 'RdGy')
+            im2 = ax2.imshow(resid, vmin = -0.01, vmax = 0.01, cmap = 'RdGy')
             ax2.axis('off')
 
-            ax2.set_title('Residual: (data-model)/model')
+            ax2.set_title('Residual: (data-model)')
 
             fig.colorbar(im2, cax=cax, orientation='vertical',fraction=0.046, pad=0.04)
             fig.subplots_adjust(wspace = 0.01)
 
             return sig_1d/self.oversamp, a2D_cur/self.oversamp**2, chi2_cur,fig
 
         else:
@@ -278,7 +286,17 @@
                 num_min = num_fit
         #Add Show fig
 
         if norm_a:
             return sig_min / self.oversamp, a_min / np.sum(a_min)
         else:
             return sig_min / self.oversamp, a_min / self.oversamp**2
+    
+    def calc_fwhm(self):
+        """ Function to estimate the FHWM of the PSF, by interpolating the measured profile
+
+    Returns
+    -------
+    FWHM: float
+        Estimate of the FWHM in pixels
+    """  
+        return interp1d(self.intens,self.radius, kind = 'quadratic')( self.intens[0]/2. )*2
```

### Comparing `imcascade-1.0/imcascade/results.py` & `imcascade-1.1/imcascade/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import numpy as np
+import matplotlib.pyplot as plt
 import asdf
 from scipy.optimize import root_scalar
 
-import imcascade
-from imcascade.utils import get_med_errors
+from imcascade.fitter import fitter_from_ASDF,Fitter
+from imcascade.utils import get_med_errors,vars_to_use
 
 
 def calc_flux_input(weights,sig, cutoff = None):
     if cutoff == None:
         return np.sum(weights, axis = -1)
     else:
         return np.sum(weights*(1. - np.exp(-1*cutoff**2/ (2*sig**2)) ), axis = -1 )
 
 def r_root_func(r,f_L, weights,sig,cutoff):
     return f_L - np.sum(weights*(1. - np.exp(-1.*r**2 / (2*sig**2)) ),axis = -1 ) / calc_flux_input(weights,sig,cutoff = cutoff)
 
-vars_to_use = ['img', 'weight', 'mask', 'sig', 'Ndof', 'Ndof_sky', 'Ndof_gauss',
- 'has_psf', 'psf_a','psf_sig','psf_shape','log_weight_scale','min_param','sky_model',
- 'posterior', 'post_method','log_file', 'logz','logz_err']
 
 class ImcascadeResults():
     """A class used for collating imcascade results and performing analysis
 
         Parameters
         ----------
         Obj: imcascade.fitter.Fitter class, dictionary or str
@@ -37,15 +35,15 @@
             to ensure the posterior is large enough, some of this analysis can
             take time if you have >10^6 samples so this is one way to speed up
             this task but use with caution.
 """
     def __init__(self, Obj, thin_posterior = 1):
         """Initialize a Task instance
 """
-        if type(Obj) == imcascade.fitter.Fitter:
+        if type(Obj) == Fitter:
             self.obj_type = 'class'
             dict_obj = vars(Obj)
         if type(Obj) == dict:
             self.obj_type = 'dict'
             dict_obj = Obj
         if type(Obj) == str:
             self.obj_type = 'file'
@@ -53,15 +51,17 @@
             dict_obj = file.tree
 
         self.input = Obj
 
         #To-do write better function to do this that can handle missing values
         for var_name in vars_to_use:
             if var_name in dict_obj.keys():
-                setattr(self, var_name, dict_obj[var_name] )
+                    setattr(self, var_name, dict_obj[var_name] )
+        if 'posterier'in dict_obj.keys():
+            setattr(self, 'posterior', dict_obj['posterier'] )
 
         if hasattr(self, 'posterior'):
             self.x0 = self.posterior[::int(thin_posterior),0]
             self.y0 = self.posterior[::int(thin_posterior),1]
             self.q = self.posterior[::int(thin_posterior),2]
             self.pa = self.posterior[::int(thin_posterior),3]
             self.weights = self.posterior[::int(thin_posterior),4:4+self.Ndof_gauss]
@@ -510,15 +510,15 @@
             res_dict['C80_20'] = get_med_errors(self.r80 / self.r20,lo = errp_lo, hi = errp_hi)
             res_dict['C90_50'] = get_med_errors(self.r90 / self.r50,lo = errp_lo, hi = errp_hi)
 
         if save_results:
             if self.obj_type == 'file':
                 input_asdf = asdf.open(self.input)
                 input_asdf.tree.update(res_dict)
-                input_asdf.write_to(self.input)
+                input_asdf.write_to(save_file)
             else:
                 dict_to_save = vars(self).copy()
                 dict_to_save.pop('input')
                 dict_to_save.pop('obj_type')
 
                 if hasattr(self, 'posterior'):
                     for key in ['flux','r20','r50','r80','r90']:
@@ -647,14 +647,104 @@
         r_2 = r[arg_min + 1 ]
 
         r_target = (P_ratio - I_1)*(P_ratio - I_2)/(I_0 - I_1)/(I_0 - I_2)*r_0
         r_target += (P_ratio - I_0)*(P_ratio - I_2)/(I_1 - I_0)/(I_1 - I_2)*r_1
         r_target += (P_ratio - I_0)*(P_ratio - I_1)/(I_2 - I_0)/(I_2 - I_1)*r_2
 
         return r_target
+    
+    def make_diagnostic_fig(self):
+        """Function which generates a diagnostic figure to assess fit
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        fig:  matplotlib figure
+            matplotlib figure object
+"""
+        if self.obj_type == 'dict':
+            print ('Cannot make diagnostic figure with dict as an input, please use a fitter class or an asdf file')
+        elif self.obj_type == 'class':
+            fitter = self.input 
+        elif self.obj_type == 'file':
+            fitter = fitter_from_ASDF(self.input)
+        
+        fig,((ax1,ax2,ax3,ax4),(ax5,ax6,ax7,ax8) ) = plt.subplots(2,4, figsize = (13,6.5))
+
+        param_no_sky = np.copy(self.min_param)
+        if fitter.sky_model:
+            param_no_sky[-3:] = 0
+            best_fit_sky = fitter.get_sky_model(self.min_param[-3:])
+        else:
+            best_fit_sky = np.zeros(shape= fitter.img.shape)
+        img = np.ma.masked_array(fitter.img, mask = fitter.mask)
+        best_fit_mod = fitter.make_model(param_no_sky)
+
+        resid = img - best_fit_mod - best_fit_sky
+
+        vlo,vhi = np.percentile(np.arcsinh(img.flatten()), [30,99]) 
+
+        ax1.set_title('Image')
+        ax1.imshow(np.arcsinh(img), vmin = vlo,vmax = vhi, cmap = 'cividis')
+        ax1.axis('off')
+
+        ax2.set_title('Best Fit Obs. Galaxy Model')
+        ax2.imshow(np.arcsinh(best_fit_mod), vmin = vlo,vmax = vhi, cmap = 'cividis')
+        ax2.axis('off')
+
+        ax3.set_title('Best Fit Sky Model')
+        ax3.imshow(np.arcsinh(best_fit_sky), vmin = vlo,vmax = vhi, cmap = 'cividis')
+        ax3.axis('off')
+
+        resid_std = np.std(resid)
+        ax4.set_title('Residuals')
+        ax4.imshow(np.arcsinh(resid),cmap = 'twilight', vmin = np.arcsinh(-3.5*resid_std), vmax = np.arcsinh(3.5*resid_std))
+        ax4.axis('off')
+
+        rplot = np.linspace(0, fitter.sig[-1]*1.2, num = 50)
+        sbp_ind = self.calc_sbp(rplot, return_ind = True)
+        sbp_tot = sbp_ind.sum(axis = -1)
+        cog = self.calc_cog(rplot)
+        rms_med = np.median(1./np.sqrt(fitter.weight) )
+        abs_sky_med = np.median(np.abs(best_fit_sky))
+
+        if len(sbp_tot.shape) > 1:
+            sbp_tot = sbp_tot.mean(axis = 1)
+            cog = cog.mean(axis = 1)
+            sbp_ind = sbp_ind.mean(axis = 1)
+
+        ax5.plot(rplot,sbp_tot, 'k-', lw = 2)
+        ax5.plot(rplot,sbp_ind, 'r--')
+        ax5.plot([rplot[0],rplot[-1]], [rms_med,rms_med], 'C0:', lw = 3, label = 'Med. RMS/pix')
+        ax5.plot([rplot[0],rplot[-1]], [abs_sky_med,abs_sky_med], 'C1:', lw = 3, label = 'Med. |Sky Model|')
+
+        ax5.set_yscale('log')
+        ax5.set_ylim(sbp_tot[-1] *0.4,sbp_tot[0]*1.4)
+        ax5.set_xlabel('radius (pixels)')
+        ax5.set_title('Intr. SBP')
+        ax5.legend(frameon = False)
+
+        ax6.plot(rplot, cog,'k-', lw = 2)
+        #ax6.set_yscale('log')
+        ax6.set_xlabel('radius (pixels)')
+        ax6.set_title('Intr. Curve-of-growth')
+
+        ax7.axis ('off')
+        ax8.axis('off')
+
+        ax7_str = f'Flux = {self.calc_flux():.2f} \nr_eff = {self.calc_r50():.2f} pixels\nq = {self.q:.2f}\nPA ={self.pa:.2f} rad'
+        ax7.text(0.01,0.99,ax7_str, transform = ax7.transAxes, fontsize = 16, ha = 'left', va= 'top')
+
+        ax8_str = f'# of components = {fitter.Ndof_gauss:d}\nPSF? - {fitter.has_psf}\nSky? - {fitter.sky_model}'
+        ax8.text(0.01,0.99,ax8_str, transform = ax8.transAxes, fontsize = 16, ha = 'left', va= 'top')
+        fig.subplots_adjust(wspace = 0.2)
+        
+        return fig
 
 class MultiResults():
     ''' A Class to analyze and combine multiple ImcascadeResults classes using evidence weighting'''
     def __init__(self, lofr):
         self.lofr = lofr
         self.num_res = len(lofr)
         self.len_post = np.array([res.posterior.shape[0] for res in self.lofr])
```

### Comparing `imcascade-1.0/imcascade/utils.py` & `imcascade-1.1/imcascade/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import numpy as np
 from scipy.special import gamma
 import itertools
 from astropy.convolution import convolve, Gaussian2DKernel
 
+vars_to_use = ['img', 'weight', 'mask', 'sig', 'Ndof', 'Ndof_sky', 'Ndof_gauss',
+ 'has_psf', 'psf_a','psf_sig','psf_shape','log_weight_scale','min_param','sky_model',
+ 'posterior', 'post_method','log_file', 'logz','logz_err']
+
 def guess_weights(sig, re, flux):
     """ Method to guess the weights of gaussian componenets given an re and flux.
     Based on a polynomial fit to the exp fits of Hogg & Lang 2013
 
     Parameters
     ----------
     sig: array
```

### Comparing `imcascade-1.0/imcascade.egg-info/PKG-INFO` & `imcascade-1.1/imcascade.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: imcascade
-Version: 1.0
+Version: 1.1
 Summary: imcascade: Fitting astronomical images using a 'cascade' of Gaussians
 Home-page: https://github.com/tbmiller-astro/imcascade
 Author: Tim Miller
 Author-email: tim.miller@yale.edu
 License: MIT
-Description: imcascade
-        =========
-        
-        |Docs|
-        |License|
-        |Arxiv|
-        
-        ``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method here (Link to come soon) and the documentation `here <https://imcascade.readthedocs.io>`_.
-        
-        Citation
-        --------
-        ``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite Miller & van Dokkum (2021) (Link to paper forthcoming)
-        
-        Help and Issues
-        ---------------
-        ``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`_. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
-        
-        .. |Docs| image:: https://readthedocs.org/projects/imcascade/badge/?version=latest
-           :target: http://imcascade.readthedocs.io/?badge=latest
-        .. |License| image:: https://img.shields.io/badge/license-MIT-blue
-        .. |Arxiv| image:: https://img.shields.io/badge/arXiv-2109.13262-blue
-           :target: https://arxiv.org/abs/2109.13262
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+imcascade
+=========
+
+|Docs|
+|License|
+|Arxiv|
+|pypi|
+
+``imcascade`` is a code designed for fitting objects in astronomical images using a "cascade" of Gaussians. It uses multi-guassian expansion (MGE) to model galaxies as a mixture of Gaussians in a Bayesian Framework. It was designed to study the morphology of faint, semi-resolved galaxies. If you are planning on using ``imcascade`` we suggest reading our paper describing the method `here <https://arxiv.org/abs/2109.13262>`__  and the documentation `here <https://imcascade.readthedocs.io>`__.
+
+Citation
+--------
+``imcascade`` is open source software made available under the MIT license, written by Tim Miller and Pieter van Dokkum. If you use this package in your work please cite `Miller & van Dokkum (2021) <https://arxiv.org/abs/2109.13262>`__
+
+Help and Issues
+---------------
+``imcacscade`` is maintained on Github. If you find a bug in the code or have a feature you would like to request, please open an `issue on Github <https://github.com/tbmiller-astro/imcascade/issues>`__. Additionally you can reach out to me directly if you are having issues using the code or have suggestions.
+
+.. |Docs| image:: https://readthedocs.org/projects/imcascade/badge/?version=latest
+   :target: http://imcascade.readthedocs.io/?badge=latest
+.. |License| image:: https://img.shields.io/badge/license-MIT-blue
+.. |Arxiv| image:: https://img.shields.io/badge/arXiv-2109.13262-blue
+   :target: https://arxiv.org/abs/2109.13262
+.. |pypi| image:: http://img.shields.io/pypi/v/imcascade.svg
+   :target: https://pypi.org/project/imcascade/
```

### Comparing `imcascade-1.0/setup.py` & `imcascade-1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import setuptools
+from setuptools import setup, Extension, find_packages
 
 with open('requirements.txt') as infd:
     INSTALL_REQUIRES = [x.strip('\n') for x in infd.readlines()]
     print(INSTALL_REQUIRES)
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
-setuptools.setup(
+setup(
     name="imcascade",
-    version="1.0",
+    version="1.1",
     author="Tim Miller",
     author_email="tim.miller@yale.edu",
     description="imcascade: Fitting astronomical images using a 'cascade' of Gaussians",
-    long_description=readme(),
     long_description_content_type="text/x-rst",
+    long_description=readme(),
     url="https://github.com/tbmiller-astro/imcascade",
-    entry_points = {},
-    packages=setuptools.find_packages(),
+    packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.5",
```

