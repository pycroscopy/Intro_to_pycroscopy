# Intro_to_pycroscopy
Introduction to the Pycroscopy Ecosystem: https://pycroscopy.github.io/pycroscopy/ecosystem.html 

Brief Overview of Pycroscopy Package for scientific analysis of nanoscience data: https://pycroscopy.github.io/pycroscopy/about.html

Homepage: https://github.com/pycroscopy

# How to get started

Download Anaconda: https://www.anaconda.com *(This should automatically install Anaconda-Navigator and allow you to lauch Jupyter Notebooks.)*

Install NumPy: https://numpy.org/install/

Install sidpy package through Anaconda: https://anaconda.org/conda-forge/sidpy

Install h5py: https://docs.h5py.org/en/stable/build.html

# Repositories & Notebooks
*The notebooks for their respective respositories are available in the files section.*

## SciFiReaders
Tools for extracting data and metadata from scientific data files

SciFiReaders is a collection of sidpy.Reader python classes that extract data and metadata from scientific data files. The extracted information are returned as sidpy.Dataset objects which are standardized and exchangable data objects across all packages in the pycroscopy ecosystem.

About: https://pycroscopy.github.io/SciFiReaders/about.html
###### • Notebook - Developing a reader: https://github.com/pycroscopy/SciFiReaders/blob/master/notebooks/00_developing_a_reader/developing_a_reader.ipynb
###### • Notebook - Using Readers: https://github.com/pycroscopy/SciFiReaders/blob/master/notebooks/01_using_readers/convert_hyperspy.ipynb

Coming soon: short-video with example

## sidpy
Python utilities for storing and visualizing Spectroscopic and Imaging Data (SID)

Installation: https://pycroscopy.github.io/sidpy/install.html

###### • Notebook - Basic Usage: https://pycroscopy.github.io/sidpy/notebooks/00_basic_usage/create_dataset.html
###### • Notebook - Parallel Computing: https://github.com/pycroscopy/sidpy/blob/master/notebooks/01_parallel_computing/parallel_compute.ipynb
###### • Notebooks - Visualization: https://github.com/pycroscopy/sidpy/tree/master/notebooks/02_visualization
###### • Notebooks - hdf5: https://github.com/pycroscopy/sidpy/tree/master/notebooks/03_hdf5

## pyNSID
Python framework for storing, visualizing, and processing spectroscopy, imaging or any observational / experimental data

About: https://pycroscopy.github.io/pyNSID/about.html

###### • Notebook - Write SIDpy Dataset via pyNSID: https://github.com/pycroscopy/pyNSID/blob/master/notebooks/00_basic_usage/write_read_sidpy_dataset.ipynb

Why not just use h5py? -> https://pycroscopy.github.io/pyNSID/nsid.html

# HDF5 Files
If you already have an HDF5, follow the following structure for identifying contents, shapes of datasets, and plotting.
## Fast Force Mapping Example
After setting your file path as directed in the Basic Usage notebook, use the following command to print out the contents of your HDF5 file:
```
usid.hdf_utils.print_tree(h5_f)
```
<img width="290" alt="Screen Shot 2021-08-09 at 4 49 54 PM" src="https://user-images.githubusercontent.com/79813375/128772579-671a3597-ff4e-48f7-8a01-c10b0b955c11.png">

Here, you can see that you have two groups or "keys" in your file with the following datasets.

To see the keys and shape of your datasets use the following command:
```
print(h5_f.keys())
print(h5_f['FFM']['Defl'][:].shape, h5_f['FFM']['Drive'][:].shape, h5_f['FFM']['Raw'][:].shape)
```
