Git
===
Git is a version control system that allows multiple people to collaborate on a project without interfering (too much!) with each other's work. If someone changes a file (i.e. writes to it or deletes from it), git records the differences between the new version and the old version, and maintains a history.

## **Installation**
Command:  
```
brew install git
```

* Documentation can be found here: https://git-scm.com/doc

## **Need to Know**
* MacOS comes with git preinstalled in /usr/bin/git
* Git also allows you to create <i>branches.</i> This allows you to create separate workflows out of the same version history without worrying about messing up someone else's work. You can then <i>merge</i> them back together for a complete project.

## **Best practices**
* <strong>Pull Before Push</strong> You should always pull from the branch you are working on to make sure that you have the most recent version of the remote (i.e. Github) repository. This lets you deal with merge conflicts locally on your machine rather than in your remote repository.
* <strong>Push Only Working Code (POWC)</strong> You should always only push working code to your remote repository so that if someone else <i>checksout</i> your branch, the code runs.

## **Bread and Butter Commands**
```
git status
```
This will show you all of the files that are being tracked by git and their status--changed, addded, deleted-- and if they have been commited yet.

``` 
git pull <remote repository>
```
This will pull the remote repository down to your local machine for changes to be made

```
git add <files>
```
This will add the files you have modified to be commited. You can choose what files/directories to add. You can also add all of the files simply saying "git add ."

```
git commit -m "<message>"
```
This is a staging area before publishing the changes to the remote repository for everyone working on the project to see. The -m flag is adding a message telling others what the changes you made do. These messages are permanent and will be kept in the history of your repository <strong>forever</strong>

```
git push <remote repository>
```
This will publish your changes to your remote repository for others on your project to use, see, and change.
* This is the most common workflow commands using git. The majority of your git work will be using these commands.

## **Other Commands**
```
git init <directory>
git clone <repository>
git checkout <repository> <branch> 
git config user.name
git config user.email
git diff
```
