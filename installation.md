## Alternative Installation Instructions

At the time of writing (January 2020), the installation of Cantera fails on a freshly installed Anaconda installation. In order to resolve various clashing package versions, run the following in a terminal window (on Windows, use the **Anaconda Prompt**).:
```
conda update --all
```
which will update all packages to up-to-date versions (this will take several minutes). Now, run
```
conda install -y -c cantera cantera graphviz python-graphviz
```
to install cantera and dependent packages.

### Notes:

1. At the time of writing, calling conda from within jupyter on windows is extremely slow (hence the recommendation to run it in the terminal instead)
2. The instructions above install cantera into the root system of Anaconda python. For instructions involving conda environments, follow [this link](https://cantera.org/install/conda-install.html).
