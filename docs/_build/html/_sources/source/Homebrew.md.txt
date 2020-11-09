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
Homebrew is installed in /usr/local. Every time we open up terminal it will have access to our /usr/local/bin directory.  
Installing packages using “brew” will install packages in their own directories and then symlink it into /usr/local. 

## **Upgrade**
```
/bin/bash "Brew upgrade"
```
