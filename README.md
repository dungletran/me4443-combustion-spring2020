# ME4443 - Introduction to Combustion

This *Library* will be used to illustrate examples in class and/or to share templates for extended homework or projects.

 * Maintained (i.e. continuously updated) versions will be housed on [GitHub](https://github.com/ischoegl/me4443-combustion-fall2020)

## Python Installation

This class will use open source Python software, with the preconfigured suite [**Anaconda**](https://www.anaconda.com) being the *only version* supported for classwork. Anaconda is free of charge, and can be installed on any operating system (i.e. Windows, OSX and Linux).

 * To install, follow [this link](https://www.anaconda.com/download) and select **Python 3.7** as the version to download and install.
 * Once the installation has finished, open a Jupyter notebook: see [instructions](http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html)
 * To install [Cantera](http://www.cantera.org/docs/sphinx/html/index.html) (an open source software package we will use for class), run the following from within a Jupyter notebook:

```
!conda install -y -c cantera cantera
```

* This process is also illustrated in the following notebook: [install\_cantera](install\_cantera.ipynb).

## Git Installation (optional)

In order to keep class resources up to date, you can either download things from Gitlab repeatedly, or, alternatively, use **git**, which is a tool that allows you to retrieve the latest version of class resources without creating excessive clutter. Installation depends on your operating system:

 - **Windows:** follow the download [link](https://git-scm.com/download), which provides a simple command line tool. During installation, follow instructions; it is likely sufficient to leave everything on default settings.

 - **OSX:** Apple maintains a git within their *XCode* suite. Open a terminal (type `terminal` in the finder and it will open), and use `git --help`, after which OSX will offer to install XCode for you.

 - **Linux:** use your package manager to install git (contact me on slack if there are questions)

Irrespective of operating system, you will use git from the command line (either *Git Bash* or a Terminal). Launch the terminal and locate yourself by typing
```
pwd
```
which yields your current location, most likely `/c/Users/<your_user_name>` (Windows) or similar, i.e. your user directory within the operating system.

Now change onto your Desktop and clone the repository using
```
cd Desktop
git clone git@github.com:ischoegl/me4443-combustion-fall2020.git
```
which will place the class folder on your Desktop. (*Note: if you have a Gitlab account, this will also work: `git clone git@github.com:ischoegl/me4443-combustion-fall2020.git`)

In order to update to a newer version of the course documents (e.g. once another assignment is posted), issue
```
cd me4443-combustion-fall2020
git pull
```

**Important:** whenever you start working on your homework solutions, save your notebooks under a *different* filename, as the above command will discard local changes.

## Launching Jupyter

On windows, launch the *Anaconda Prompt* (which lands you inside your user folder, e.g. `C:\Users\<your_user_name>`). Now navigate to where the course files are located, i.e.
```
cd Desktop\me4443-combustion-fall2020
```
Now, launch jupyter
```
jupyter notebook
```
and navigate wherever you need to go.

**Important:** as mentioned above, *do not modify the files that are provided*, but make copies instead. I.e. use `File > Make a Copy ...` from within Jupyter to ensure that your modifications are not overwritten whenever you update the files for the next assignment ...
