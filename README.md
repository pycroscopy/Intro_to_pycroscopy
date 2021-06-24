# Intro_to_pycroscopy
Introduction to the Pycroscopy Ecosystem: https://pycroscopy.github.io/pycroscopy/ecosystem.html 

Brief Overview of Pycroscopy Package for scientific analysis of nanoscience data: https://pycroscopy.github.io/pycroscopy/about.html

Homepage: https://github.com/pycroscopy

# How to get started

Download Anaconda: https://www.anaconda.com *(This should automatically install Anaconda-Navigator and allow you to lauch Jupyther Notebooks.)*

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

###### • Notebooks - Basic Usage: https://github.com/pycroscopy/pyNSID/tree/master/notebooks/00_basic_usage
###### • Notebook - Write/read SIDpy Dataset via pyNSID: https://github.com/pycroscopy/pyNSID/blob/master/notebooks/00_basic_usage/write_read_sidpy_dataset.ipynb

Why not just use h5py? -> https://pycroscopy.github.io/pyNSID/nsid.html

