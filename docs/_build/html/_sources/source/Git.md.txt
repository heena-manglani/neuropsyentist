Git
===
Git is a version control system that allows multiple people to collaborate on a project without interfering (too much!) with each other's work. If someone changes a file (i.e. writes to it or deletes from it), git records the differences between the new version and the old version, and maintains a history.

## Installation

Command:  
```
brew install git
```

* Documentation can be found here: <a href="https://git-scm.com/doc" target="_blank" rel="noreferrer">git-scm.com/doc</a>

## Need to Know
* MacOS comes with git preinstalled in /usr/bin/git
* Git also allows you to create <i>branches.</i> This allows you to create separate workflows out of the same version history without worrying about messing up someone else's work. You can then <i>merge</i> them back together for a complete project.
* <a href="https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet" target="_blank" rel="noreferrer">Git Cheat Sheet</a>

## Best practices
* <strong>Pull Before Push</strong> You should always pull from the branch you are working on to make sure that you have the most recent version of the remote (i.e. Github) repository. This lets you deal with merge conflicts locally on your machine rather than in your remote repository.
* <strong>Push Only Working Code (POWC)</strong> You should always only push working code to your remote repository so that if someone else <i>checksout</i> your branch, the code runs.
* Main and develop should generally not be pushed directly to. For this you would use a branch and then merge your code into develop, then main.
    * To create a new branch and checkout. -b flag tells git to create the branch then checkout
      ```bash
      git checkout -b <branch name>
      ```
    * Checkout an existing branch
        ```bash
        git checkout <branch name>
        ```

## Bread and Butter Commands
* This is the most common workflow commands using git. The majority of your git work will be using these commands.
* This will show you all of the files that are being tracked by git and their status--changed, addded, deleted-- and if they have been commited yet.
    ```
    git status
    ```

* This will pull the remote repository down to your local machine for changes to be made
    ``` 
    git pull <remote repository>
    ```

* This will add the files you have modified to be commited. You can choose what files/directories to add. You can also add all of the files simply saying "git add ."
    ```
    git add <files>
    ```

* This is a staging area before publishing the changes to the remote repository for everyone working on the project to see. The -m flag is adding a message telling others what the changes you made do. These messages are permanent and will be kept in the history of your repository <strong>forever</strong>

    ```
    git commit -m "<message>"
    ```

* This will publish your changes to your remote repository for others on your project to use, see, and change.
    ```
    git push <remote repository>
    ```

## Cloning an Existing Repository
* Pull an existing remote repository to your local machine
* Create a directory to hold your repo
* Clone the repo in the current directory
  ```bash
  git clone https://github.com/user-name/repo-name.git
  ```

## Initialize A Repository

* Initialize a blank repository locally.
  * Creates a .git directory which sets up the configuration and ability for version control
    ```bash
    git init
    ```
  * Adds the README file to the files currently tracked by git (README is used as an introduction or documentation for a project)
    ```bash
    git add README.md
    ```
  * Commits the added files so they are now tracked at this point. 
    ```bash
    git commit -m "first commit"
    ```
  * Rename the branch to main
    ```bash
    git branch -M main
    ```
  * Add the remote (i.e. Github) tracking.
    ```bash
    git remote add origin https://github.com/user-name/testrepo.git
    ```
  * Push the staged commit to the remote branch main. -u flag is set-upstream
    ```bash
    git push -u origin main
    ```

## User config
* User name and emails can be set for a single repository and globally. 

    ```
    git config --global user.name "Name"
    git config --global user.email email@email.com
    ```