# Comparing `tmp/noisepy_seis-0.5.2.tar.gz` & `tmp/noisepy_seis-0.5.3.tar.gz`

## Comparing `noisepy_seis-0.5.2.tar` & `noisepy_seis-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/LICENSE
--rw-r--r--   0        0        0    13663 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 noisepy_seis-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/LICENSE
+-rw-r--r--   0        0        0    13580 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    16001 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/PKG-INFO
```

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.5.3/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.5.3/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.5.3/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.5.3/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/main.py` & `noisepy_seis-0.5.3/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.5.3/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.5.3/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/LICENSE` & `noisepy_seis-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/README.md` & `noisepy_seis-0.5.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,111 +12,112 @@
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 # Citation:
 Please cite the following reference if you use the code for your publication:
 Jiang, C. and Denolle, M. "NoisePy: a new high-performance python tool for seismic ambient noise seismology." Seismological Research Letter 91 (3): 1853–1866.
 
 ## Major updates include
-* adding options for several stacking methods such as nth-root, robust-stacking, auto-covariance and selective in S2. A script is added to the folder of application_modules to cross-compare the effects of different stacking method (note that `substack` parameter in S2 has to be `True` in order to use it)
+* adding options for several stacking methods such as nth-root, robust-stacking, auto-covariance and selective. A script is added to the folder of application_modules to cross-compare the effects of different stacking method (note that `substack` parameter in S2 has to be `True` in order to use it)
 * adding a jupter notebook for tutorials on performing seismic monitoring analysis using NoisePy
 * adding a jupter notebook for generating response spectrum for a nodal array (to be done)
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install the library due to their convenience. Below are command lines we have tested to create a python environment to run NoisePy. Note that the test is performed on `macOS Mojave (10.14.5)`, so it could be slightly different for other OS.
 
 
 ### Note the order of the command lines below matters ###
 
 # With Conda:
 ```bash
-conda create -n noisepy python=3.8 pip
-conda activate noisepy
-conda install -c conda-forge openmpi
-pip install noisepy-seis 
+$ conda create -n noisepy python=3.8 pip
+$ conda activate noisepy
+$ conda install -c conda-forge openmpi
+$ pip install noisepy-seis 
 ```
 
 # With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```sh
-brew install open-mpi
+$ brew install open-mpi
 ```
 
-```bash
-python -m venv noisepy
-source noisepy/bin/activate
-pip install noisepy-seis
+```sh
+$ python -m venv noisepy
+$ source noisepy/bin/activate
+$ pip install noisepy-seis
 ```
 To run the code on a single core, open the terminal and activate the noisepy environment before run following command. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster. Examples of installation on Frontera are below.
 
 # Functionality
 * download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
 
-### 0A. Downloading seismic noise data (`src/S0A_download_ASDF_MPI.py`)
-This script (located in the directory of `src`) and its existing parameters allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
+### 0A. Downloading seismic noise data 
+This command allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
 
 In the script, short summary is provided for all input parameters that can be changed according to the user's needs. In the current form of the script, we set `inc_hours=24` to download day-long continous noise data as well as the meta info and store them into a single ASDF file. To increase the signal-to-noise (SNR) of the final cross-correlation functions (see Seats et al.,2012 for more details), we break the day-long sequence into smaller segments, each of `cc_len` (s) long with some overlapping defined by `step`. You may wanto to set `flag` to be `True` if intermediate outputs/operational time is preferred during the downloading process.
 
 ```bash
 noisepy download
 ```
 The data to be downloaded can be customized via command line arguments. See `noisepy download --help` for details.
 
 If you want to use multiple cores (e.g, 4), run the script with the following command using [mpi4py](https://mpi4py.readthedocs.io/en/stable/).
 ```bash
 mpirun -n 4 noisepy download
 ```
 
-The outputted files from S0A include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the script of S0A and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
+The outputted files from the download include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the download and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/RAW_DATA/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_waveform(sfile,'CI','BLC',0.01,0.4)
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/waveform3.png" width="600" height="400">
 
 Note that the script also offers the option to download data from an existing station list in a format same to the outputed CSV file. In this case, `down_list` should be set to `True` at L53. In reality, the downloading speed is dependent on many factors such as the original sampling rate of targeted data, the networks, the data center where it is hosted and the general structure you want to store on your machine etc. We tested a bunch of the parameters to evaluate their performance and the readers are referred to our paper for more details (Jiang et al., 2020).
 
 
 ### 0B. DEAL with local SAC/miniseed files using `S0B_to_ASDF.py`
-If you want to use the NoisePy to handel local data in SAC/miniseed format stored on your own disk, this is the script you need. Most of the variables are the same as those for S0A and thus should be pretty straighforward to follow and change. In this script, it preprocesses the data by merging, detrending, demeaning, downsampling and then trimming before saving them into ASDF format for later NoisePy processing. In particular, we expect the script to deal with very messydata, by which we mean that, seismic data is broken into small pieces and of messy time info such as overlapping time. REMEMBER to set `messydata` at L62 to `True` when you have messy data! (Tutorial on removing instrument response)
+If you want to use the NoisePy to handel local data in SAC/miniseed format stored on your own disk, this is the script you need. Most of the variables are the same as those for the download step and thus should be pretty straighforward to follow and change. In this script, it preprocesses the data by merging, detrending, demeaning, downsampling and then trimming before saving them into ASDF format for later NoisePy processing. In particular, we expect the script to deal with very messydata, by which we mean that, seismic data is broken into small pieces and of messy time info such as overlapping time. REMEMBER to set `messydata` at L62 to `True` when you have messy data! (Tutorial on removing instrument response)
+
 
 
+### 1. Perform cross correlations
+This is the core function of NoisePy, which performs [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform) to all noise data first and loads them into the memory before they are further cross-correlated. This means that we are performing [cross-correlation](https://en.wikipedia.org/wiki/Cross-correlation) in the frequency domain. In the script, we provide several options to calculate the cross correlation, including `raw`, `coherency` and `deconv` (see our paper<sup>*</sup> for detailed definition). We choose `coherency` as an example here. After running the script, it will create a new folder named `CCF`, in which new ASDF files containing all cross-correlation functions between different station pairs are located. It also creates a parameter file of `fft_cc_data.txt` that records all useful parameters used in this script.
 
-### 1. Perform cross correlations (`src/S1_fft_cc_MPI.py`)
-This is the core script of NoisePy, which performs [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform) to all noise data first and loads them into the memory before they are further cross-correlated. This means that we are performing [cross-correlation](https://en.wikipedia.org/wiki/Cross-correlation) in the frequency domain. In the script, we provide several options to calculate the cross correlation, including `raw`, `coherency` and `deconv` (see our paper<sup>*</sup> for detailed definition). We choose `coherency` as an example here. After running the script, it will create a new folder named `CCF`, in which new ASDF files containing all cross-correlation functions between different station pairs are located. It also creates a parameter file of `fft_cc_data.txt` that records all useful parameters used in this script.
 
 ```sh
-noisepy cross_correlate
+$ noisepy cross_correlate
 ```
 If you downloaded the data to a custom location, specify the `--path` argument. See `noisepy cross_correlate --help` for details.
 
 Once you get the cross-correlation file, you can show the daily temporal variation between all station-pair by calling `plot_substack_cc` function in `plotting_modules` as follows. NOTE that to make this plot, the parameter of `substack` has to be set to `True` in S1.
 
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/CCF/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_substack_cc(sfile,0.1,0.2,200,True,'/Users/chengxin/Documents/SCAL/CCF/figures')
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_NN.png" width="400" height="190"><img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_ZZ.png" width="400" height="190">
 
 
-### 2. Do stacking (`src/S2_stacking.py`)
-This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in S1 and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
+### 2. Do stacking 
+This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in the `cross_correlate` step and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
 
 ```sh
-noisepy stack --method linear
-noisepy stack --method pws
+$ noisepy stack --method linear
+$ noisepy stack --method pws
 ```
 
 In general, the pws produces waveforms with high SNR, and the snapshot below shows the waveform comparison from the two stacking methods. We use the folloing commend lines to make the move-out plot.
 
 ```python
 from noisepy.seis import plotting_modules
 import glob
```

### Comparing `noisepy_seis-0.5.2/pyproject.toml` & `noisepy_seis-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.2/PKG-INFO` & `noisepy_seis-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.5.2
+Version: 0.5.3
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@fas.harvard.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -62,111 +62,112 @@
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 # Citation:
 Please cite the following reference if you use the code for your publication:
 Jiang, C. and Denolle, M. "NoisePy: a new high-performance python tool for seismic ambient noise seismology." Seismological Research Letter 91 (3): 1853–1866.
 
 ## Major updates include
-* adding options for several stacking methods such as nth-root, robust-stacking, auto-covariance and selective in S2. A script is added to the folder of application_modules to cross-compare the effects of different stacking method (note that `substack` parameter in S2 has to be `True` in order to use it)
+* adding options for several stacking methods such as nth-root, robust-stacking, auto-covariance and selective. A script is added to the folder of application_modules to cross-compare the effects of different stacking method (note that `substack` parameter in S2 has to be `True` in order to use it)
 * adding a jupter notebook for tutorials on performing seismic monitoring analysis using NoisePy
 * adding a jupter notebook for generating response spectrum for a nodal array (to be done)
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install the library due to their convenience. Below are command lines we have tested to create a python environment to run NoisePy. Note that the test is performed on `macOS Mojave (10.14.5)`, so it could be slightly different for other OS.
 
 
 ### Note the order of the command lines below matters ###
 
 # With Conda:
 ```bash
-conda create -n noisepy python=3.8 pip
-conda activate noisepy
-conda install -c conda-forge openmpi
-pip install noisepy-seis 
+$ conda create -n noisepy python=3.8 pip
+$ conda activate noisepy
+$ conda install -c conda-forge openmpi
+$ pip install noisepy-seis 
 ```
 
 # With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```sh
-brew install open-mpi
+$ brew install open-mpi
 ```
 
-```bash
-python -m venv noisepy
-source noisepy/bin/activate
-pip install noisepy-seis
+```sh
+$ python -m venv noisepy
+$ source noisepy/bin/activate
+$ pip install noisepy-seis
 ```
 To run the code on a single core, open the terminal and activate the noisepy environment before run following command. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster. Examples of installation on Frontera are below.
 
 # Functionality
 * download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
 
-### 0A. Downloading seismic noise data (`src/S0A_download_ASDF_MPI.py`)
-This script (located in the directory of `src`) and its existing parameters allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
+### 0A. Downloading seismic noise data 
+This command allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
 
 In the script, short summary is provided for all input parameters that can be changed according to the user's needs. In the current form of the script, we set `inc_hours=24` to download day-long continous noise data as well as the meta info and store them into a single ASDF file. To increase the signal-to-noise (SNR) of the final cross-correlation functions (see Seats et al.,2012 for more details), we break the day-long sequence into smaller segments, each of `cc_len` (s) long with some overlapping defined by `step`. You may wanto to set `flag` to be `True` if intermediate outputs/operational time is preferred during the downloading process.
 
 ```bash
 noisepy download
 ```
 The data to be downloaded can be customized via command line arguments. See `noisepy download --help` for details.
 
 If you want to use multiple cores (e.g, 4), run the script with the following command using [mpi4py](https://mpi4py.readthedocs.io/en/stable/).
 ```bash
 mpirun -n 4 noisepy download
 ```
 
-The outputted files from S0A include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the script of S0A and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
+The outputted files from the download include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the download and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/RAW_DATA/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_waveform(sfile,'CI','BLC',0.01,0.4)
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/waveform3.png" width="600" height="400">
 
 Note that the script also offers the option to download data from an existing station list in a format same to the outputed CSV file. In this case, `down_list` should be set to `True` at L53. In reality, the downloading speed is dependent on many factors such as the original sampling rate of targeted data, the networks, the data center where it is hosted and the general structure you want to store on your machine etc. We tested a bunch of the parameters to evaluate their performance and the readers are referred to our paper for more details (Jiang et al., 2020).
 
 
 ### 0B. DEAL with local SAC/miniseed files using `S0B_to_ASDF.py`
-If you want to use the NoisePy to handel local data in SAC/miniseed format stored on your own disk, this is the script you need. Most of the variables are the same as those for S0A and thus should be pretty straighforward to follow and change. In this script, it preprocesses the data by merging, detrending, demeaning, downsampling and then trimming before saving them into ASDF format for later NoisePy processing. In particular, we expect the script to deal with very messydata, by which we mean that, seismic data is broken into small pieces and of messy time info such as overlapping time. REMEMBER to set `messydata` at L62 to `True` when you have messy data! (Tutorial on removing instrument response)
+If you want to use the NoisePy to handel local data in SAC/miniseed format stored on your own disk, this is the script you need. Most of the variables are the same as those for the download step and thus should be pretty straighforward to follow and change. In this script, it preprocesses the data by merging, detrending, demeaning, downsampling and then trimming before saving them into ASDF format for later NoisePy processing. In particular, we expect the script to deal with very messydata, by which we mean that, seismic data is broken into small pieces and of messy time info such as overlapping time. REMEMBER to set `messydata` at L62 to `True` when you have messy data! (Tutorial on removing instrument response)
+
 
 
+### 1. Perform cross correlations
+This is the core function of NoisePy, which performs [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform) to all noise data first and loads them into the memory before they are further cross-correlated. This means that we are performing [cross-correlation](https://en.wikipedia.org/wiki/Cross-correlation) in the frequency domain. In the script, we provide several options to calculate the cross correlation, including `raw`, `coherency` and `deconv` (see our paper<sup>*</sup> for detailed definition). We choose `coherency` as an example here. After running the script, it will create a new folder named `CCF`, in which new ASDF files containing all cross-correlation functions between different station pairs are located. It also creates a parameter file of `fft_cc_data.txt` that records all useful parameters used in this script.
 
-### 1. Perform cross correlations (`src/S1_fft_cc_MPI.py`)
-This is the core script of NoisePy, which performs [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform) to all noise data first and loads them into the memory before they are further cross-correlated. This means that we are performing [cross-correlation](https://en.wikipedia.org/wiki/Cross-correlation) in the frequency domain. In the script, we provide several options to calculate the cross correlation, including `raw`, `coherency` and `deconv` (see our paper<sup>*</sup> for detailed definition). We choose `coherency` as an example here. After running the script, it will create a new folder named `CCF`, in which new ASDF files containing all cross-correlation functions between different station pairs are located. It also creates a parameter file of `fft_cc_data.txt` that records all useful parameters used in this script.
 
 ```sh
-noisepy cross_correlate
+$ noisepy cross_correlate
 ```
 If you downloaded the data to a custom location, specify the `--path` argument. See `noisepy cross_correlate --help` for details.
 
 Once you get the cross-correlation file, you can show the daily temporal variation between all station-pair by calling `plot_substack_cc` function in `plotting_modules` as follows. NOTE that to make this plot, the parameter of `substack` has to be set to `True` in S1.
 
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/CCF/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_substack_cc(sfile,0.1,0.2,200,True,'/Users/chengxin/Documents/SCAL/CCF/figures')
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_NN.png" width="400" height="190"><img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_ZZ.png" width="400" height="190">
 
 
-### 2. Do stacking (`src/S2_stacking.py`)
-This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in S1 and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
+### 2. Do stacking 
+This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in the `cross_correlate` step and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
 
 ```sh
-noisepy stack --method linear
-noisepy stack --method pws
+$ noisepy stack --method linear
+$ noisepy stack --method pws
 ```
 
 In general, the pws produces waveforms with high SNR, and the snapshot below shows the waveform comparison from the two stacking methods. We use the folloing commend lines to make the move-out plot.
 
 ```python
 from noisepy.seis import plotting_modules
 import glob
```

