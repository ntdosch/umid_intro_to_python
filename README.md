# Introduction to Python - UMid F2F 2023
FPL Building 1, Room 101
## Agenda
### 8:15-9:45: Getting started (Part 1 of 2) 
### 9:45-10:00: Break
### 10:00-11:30: Working with data (Part 2 of 2)

## 0. Getting started (8:15-9:45)

0. Welcome & introductions
1. Download or clone the [class materials](https://code.usgs.gov/ncorson-dosch/umid_intro_to_python) 
2. Download and install [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/) Python distribution
3. Build environment:
   - Open an Anaconda Prompt (Windows) or a Terminal (MacOS)
   - Change directory to `umid_intro_to_python`
     ```
     cd <path to umid_intro_to_python>
     ```
   - Use Conda to build a custom environment, using the  `environment.yml` file:
      ```
      conda env create -f environment.yml
      ```
   - See a list of the available environments:
      ```
      conda env list
      ```
   - activate the new environment:
      ```
      conda activate umid
      ```
   - You can tell the new environment been activated by the `(umid)` in your terminal. You can also verify this new enviromnet has been activated by again using the command:
      ```
      conda env list
      ```
   - This webpage is a a [very helpful resource](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#activating-an-environment) for managing environments
4. Running Python on your computer
   1. command line (IPython)
       ```
       python

       print('hello upper midwest')
       ```
   
   2. scripts
       ```
       python rock_paper_scisors.py
       ```
   3. Jupyter Notebooks
       ```
       jupyter notebook
       ```
5. Launching and using Jupyter Notebooks
   1. Launching in the right place
   2. The Kernel
   3. Running notebooks
   4. Advantages and pitfalls
   5. Closing Jupyter Notebooks
6. Python basics - brief overview [Nick]
   1. data types
   2. lists, tuples, dictionaries
   3. math
   4. arrays
7. Reading data into python [Nick]
   1. Reading files line by line (readlines)
   2. Pandas
   3. intro to plot making (Matplotlib)

## 1. Working with Data (10:00-11:30)
0. Notebook examples about working with data
   1. working with time series data (Pandas) [Mike]
   2. Retrieving data (dataretrieval-python and Requests) [Andy]
   3. Example pulling and plotting data, saving shapefile [All? Nick will make notebook]

## Here are some links you might find helpful moving forward with Python

### conda
* [Getting started with conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html)
* [General information on conda environments](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html)
* [Managing Conda Environments](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
* [Tutorial introduction to conda enviroments](https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307)

### cheat sheets
* [conda](https://conda.io/projects/conda/en/latest/user-guide/cheatsheet.html)
* [pandas](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
* [numpy](http://datacamp-community-prod.s3.amazonaws.com/ba1fe95a-8b70-4d2f-95b0-bc954e9071b0)
* [data science packages](https://www.utc.fr/~jlaforet/Suppl/python-cheatsheets.pdf)
* [Jupyter Notebook/Lab keyboard shortcuts](https://towardsdatascience.com/jypyter-notebook-shortcuts-bf0101a98330)

### general python
* [Tutorial on General Python Programming](https://cscircles.cemc.uwaterloo.ca/)
* [Installing packages dynamically into an environment](https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#working-in-development-mode)
* [what on earth is \_\_name__ == '\_\_main__'](https://www.youtube.com/watch?v=sugvnHA7ElY)

### some galleries
* [matplotlib gallery](https://matplotlib.org/stable/gallery/index.html)
* [geopandas gallery](https://geopandas.org/en/stable/gallery/index.html)
* [a hydrologic "data story" using pandas](https://code.usgs.gov/cdi/cdi-fy20/jupyter-data-stories/-/tree/main/examples/hydrologic_data_analysis)

### more general references
* [numpy for matlab users](https://numpy.org/doc/stable/user/numpy-for-matlab-users.html)
* [datetime formats](https://docs.python.org/3/library/datetime.html) (jump to the bottom of the page where it says "Format Codes")
* [visual studio code -- our editor of choice](https://code.visualstudio.com/)

### some relevant hydrology libraries
* [PyNHD: Navigate and subset NHDPlus database](https://docs.hyriver.io/readme/pynhd.html)
* [dataretrieval-python: Download hydrologic data from NWIS](https://github.com/DOI-USGS/dataretrieval-python)
* [PyGeoHydro: Retrieve Geospatial Hydrology Data](https://docs.hyriver.io/readme/pygeohydro.html)

### Flopy and MODFLOW
* [Flopy code](https://github.com/modflowpy/flopy.git)
* [Flopy official documentation](https://flopy.readthedocs.io/en/3.3.5/)
* [MODFLOW 6 -- online documentation](https://modflow6.readthedocs.io/en/latest/)
* [MODFLOW 6 Example Problems -- overview](https://modflow6-examples.readthedocs.io/en/master/introduction.html)
* [MODFLOW 6 Example Problems](https://modflow6-examples.readthedocs.io/en/master/examples.html)
* [Flopy Tutorial Notebooks](https://github.com/modflowpy/flopy/blob/develop/docs/notebook_examples.md)
* [Groundwater Paper](https://ngwa.onlinelibrary.wiley.com/doi/abs/10.1111/gwat.12413)
* [Another Groundwater Paper](https://ngwa.onlinelibrary.wiley.com/doi/10.1111/gwat.13259)

### modflow-setup and sfrmaker
* [MODFLOW setup code and docs](https://github.com/doi-usgs/modflow-setup)
* [MODFLOW setup paper](https://www.frontiersin.org/articles/10.3389/feart.2022.903965/full)
* [SFRmaker code and docs](https://github.com/DOI-USGS/sfrmaker)
* [SFRmaker paper](https://ngwa.onlinelibrary.wiley.com/doi/10.1111/gwat.13095)
* A worked example/workflow using MODFLOW setup, SFRmaker, and PEST++
  * [workflow code](https://github.com/DOI-USGS/neversink_workflow) 
  *  [paper](https://ngwa.onlinelibrary.wiley.com/doi/full/10.1111/gwat.13129)

