Homebrew
========

Homebrew is a package manager tool for macOS and Linux.

## **Installation**
Command:  
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
* [Homebrew documentation](https://brew.sh/)

## **Need to Know**
* Homebrew is installed in /usr/local.  
* Every time we open up terminal it will have access to our /usr/local/bin directory.  
* Installing a package using “brew” will install package in its own directory and then symlink it into /usr/local. 

## **Upgrade**
```
brew upgrade
```