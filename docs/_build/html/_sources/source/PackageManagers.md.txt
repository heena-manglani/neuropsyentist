Package Managers
================

[Homebrew](https://brew.sh/),  [Anaconda](https://docs.conda.io/en/latest/) and [Pip](https://pip.pypa.io/en/stable/) are all package installer tools.

**Why do we need a package manager tool?**
* Softwares come with dependencies. 
* Package manager tools allow us to download software packages with everything they need.
* They also make sure that packages play nice.
    * They analyze the current environment (all of the existing packages) and install compatible dependencies. 

**What's the difference between homebrew vs anaconda vs pip?**
* Homebrew is a package manager tool for macOS and Linux.
* Anaconda distributes most of the popular scientific computing packages.
* Pip is a package manager specific to the Python Package Index (PyPI).
    * It installs all Python package dependecies as they are (regardless of whether they are compatible with existing packages).

**Which one should I use to install packages?**  
* It depends on what kind of package you want to install.
* If mac application, use brew.
* If python package, first try conda then conda-forge. If not, use pip.
    * Remember, anaconda manages dependencies + versioning. 
    
------
**Homebrew**
------------
Almighty "brew" commands
* to find packages = "brew search"
* to install = "brew install"
* to remove = "brew uninstall"

## Need to Know
* Homebrew is installed in /usr/local.  
* Every time you open up the terminal, it will have access to our /usr/local/bin directory.  
* Installing a package using “brew” will install package in its own directory and then symlink it into /usr/local. 

## Installation
Command:  
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## Upgrade
```
brew upgrade
```

Anaconda
--------
* conda = package manager
    * conda-forge: to install more packages