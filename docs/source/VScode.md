VScode
======

Visual Studio Code is an open-source code editor made by Microsoft. 

* VScode comes with many tools: an integrated terminal, Intellisense (code completion), and Git integrations.
* Extensions transform VScode into a powerhouse for using multiple languages, debuggers, themes, etc.
* <a href="https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf" target="_blank" rel="noreferrer"> Cheat Sheet</a>

## Installation

* <a href="https://code.visualstudio.com/docs?dv=osx" target="_blank" rel="noreferrer"> Direct download</a> or to install using brew:

  ```bash
  brew cask install visual-studio-code
  ```

## Bread and Butter Commands

* Launch VS code from the current directory of the terminal:
  ```bash
  code .
  ```

* Open command palette:
  ```
  cmd + shift + p 
  ```

* Open integrated terminal:
  ```bash
  ctrl + ~
  ```

## Must-have Extensions

* Python: `ms-python.python`
  * Essential for developing anything in Python.
  * Features: 
    * Intellisense = auto-complete
    * Linting = enforces a style guide
    * Jupyter Notebooks = execute code in segments/cells

* Community Material Theme: `equinusocio.vsc-community-material-theme`
  * Fit your style using preset themes or make your own!

## Honorable Mentions

* Live Server: `ritwickdey.liveserver`
  * Start up a local, hot-reloadable server for front-end development work
* Live Share: `ms-vsliveshare.vsliveshare` 
  * Enables collaboration in real-time without being co-located
* Markdown Linter: `davidanson.vscode-markdownlint`
  * Best styling practices
* Git Lens: `eamodio.gitlens`
  * Advanced git tracking (see who edited what and when)
* Code Spell Checker: `streetsidesoftware.code-spell-checker`
  * Basic spell checker
* Remote Development: `ms-vscode-remote.vscode-remote-extensionpack`
  * Open folders in a container
* Docker: `ms-azuretools.vscode-docker`
  * Manage docker containers.
* Anaconda Extension: `ms-python.anaconda-extension-pack`
  * Manage anaconda settings and envs.