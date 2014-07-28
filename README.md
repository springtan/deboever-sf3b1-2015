deboever-sf3b1-2014
===================

Code for reproducing SF3B1 study.

This repository is designed to allow for the replication of [XXX paper]
starting *after* some of the time intensive steps such as read-mapping,
expression estimation, etc.  Information on those steps is available in the
methods section of the paper.

This git repository holds IPython notebooks and code needed to replicate the
study.  Additional data are available from Figshare [XXX URL] and must be
downloaded before attempting to replicate the study. After cloning this github
repository, you can use the XXX notebook to download the data from Figshare.

### Cloning from Github

Important: don't change the name of the repository (e.g. deboever-sf3b1-2014).

### Dependencies

#### Python

A working IPython notebook environment is needed along with some of the common
scientific python packages that you likely already have as part of a working
IPython notebook environment. I recommend using 
[Anaconda python](https://store.continuum.io/cshop/anaconda/) since it includes
most of the needed packages. Besides the default Anaconda packages, you will 
need

* pybedtools
* [cdpybio](https://github.com/cdeboever3/cdpybio)
* [my figshare fork](https://github.com/cdeboever3/figshare)

You can download cdpybio and figshare from their github repos (links above) and
install using `python setup.py install`. 

You will also need to install the project specific python package from this
repository. If you are using Anaconda, I'd recommend making a new environment.
From the `deboever-sf3b1-2014` directory, you can change into `ds2014` and
install using `python setup.py install` or `python setup.py develop` if you
think you may want to make changes to the ds2014 package and have these
changes instantly propagated.

### Downloading data from Figshare

### Directory structure

##### data  
Downloaded from Figshare. Contains primary data files (i.e. those that aren't
created by any of the code here).

##### notebooks  
IPython notebooks tracked by git. Use these to rerun different analyses.

##### output  
Output from IPython notebooks. Contains intermediate files (i.e. files that are
created using the primary data and other external data) as well as images,
table, etc.

##### software

### Numbers from paper
The notebook `numbers_from_paper.ipynb` contains commands that print most of
numbers/statistics in the paper. Numbers in the figure legends are printed out
in the figure notebooks however (although they may be duplicated in
`number_from_paper.ipynb`).

### Figures
Each figure has its own notebook (e.g. `figure01.ipynb` or `sfigure01.ipynb`).
These notebooks create the entire figure in go except for a couple cases where
some parts of the figure have to be inserted manually. The things to be
inserted manually are either created by the notebook and saved in its output
folder or they are available in the `data` directory from figshare.

