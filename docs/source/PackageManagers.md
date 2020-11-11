Package Managers
================

<a href="https://brew.sh/" target="_blank" rel="noreferrer">Homebrew</a>, <a href="https://docs.conda.io/en/latest/" target="_blank" rel="noreferrer">Anaconda</a>, and <a href="https://pip.pypa.io/en/stable/" target="_blank" rel="noreferrer">Pip</a> are all package installer tools.

## Installation
Command:  
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
To install anaconda, go to the <a href="https://www.anaconda.com/products/individual" target="_blank" rel="noreferrer">Anaconda site</a>, download the 64-Bit Graphical Installer OR the 64-Bit Command Line Installer.

## Need to Know

**Why do we need a package manager tool?**
* Softwares come with dependencies. 
* Package manager tools allow us to download software packages with everything they need.
* They also make sure that packages play nice.
    * They analyze the current environment (all of the existing packages) and install compatible dependencies. 

**What's the difference between homebrew vs anaconda vs pip?**
* Homebrew is a package manager tool for macOS and Linux.
* Anaconda distributes most of the popular scientific computing packages.
    * conda-forge: to install more packages
* Pip is a package manager specific to the Python Package Index (PyPI).
    * It installs all Python package dependencies as they are (regardless of whether they are compatible with existing packages).

**Which one should I use to install packages?**  
* It depends on what kind of package you want to install.
* If mac application, use brew.
* If python package, first try conda then conda-forge. If not, use pip.
    * Remember, anaconda manages dependencies and versions to keep packages compatible.

**Installation Paths**
* Homebrew is installed in /usr/local.
  * Every time you open up the terminal, it will have access to our /usr/local/bin directory.  
  * Installing a package using “brew” will install package in its own directory and then symlink it into /usr/local. 
* Anaconda is installed in ~/opt directory when installing with the Graphical Installer.


------
## Bread and Butter Commands

* Find package: 

```bash
brew search <package>
```

```bash
conda search <package>
```

* Install:

```bash
brew install <package>
```

```bash
conda install <package>
```

* Remove:

```bash
brew uninstall <package>
```

```bash
conda remove <package>
```

## Upgrade

```bash
brew upgrade
```

```bash
conda upgrade conda
```

## Cheat Sheets
<a href="https://devhints.io/homebrew" target="_blank" rel="noreferrer">Homebrew</a><br>
<a href="https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf" target="_blank" rel="noreferrer">Conda</a>