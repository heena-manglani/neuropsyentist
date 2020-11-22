Git
===

<iframe width="560" height="315" src="https://www.youtube.com/embed/9ofRCD34UlA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> <br>
<br>

* Git is a version control system.
  * What's that? A version control system records changes to a file. 
  * If someone changes a file (i.e. writes to it or deletes from it), git records the differences between the new version and the old version, and maintains a history.
* Multiple people can collaborate on a project and each person's changes are documented. Fosters collaboration!
* <a href="https://git-scm.com/doc" target="_blank" rel="noreferrer">Documentation</a>

## Installation
Before installing check to see whether you have git:

```
git --version
```

To install:  
```
brew install git
```

## Need to Know
* MacOS comes with git preinstalled in /usr/bin/git
* How to work with others?
  * Git allows you to create <i>branches</i>. 
  * Branches can serve as separate workflows out of the same parent version which you can then <i>merge</i> back with <i>main</i> to update the parent code.
* Found an error? Fantastic. Git lets you revert back to a previous version. 
* <a href="https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet" target="_blank" rel="noreferrer">Git Cheat Sheet</a>

--------
## Necessary configuration:
* User name and emails can be set for a single repository and globally. 
    ```
    git config --global user.name "Name"
    git config --global user.email email@email.com
    ```

## Initial Set-Up
Either pull/clone a remote repository existing on Git to your local machine OR take an existing directory on your local and initialize it with Git.  

**To clone an existing remote repository in the current directory:**
```bash
git clone https://github.com/user-name/repo-name.git
```

**To initialize a local repository:**

1. Configure the directory to be a .git directory:
    ```bash
    git init
    ```
2. Add a README file to the files currently tracked by git:
    ```bash
    git add README.md
    ```
3. Commit the added files so they are now tracked:
    ```bash
    git commit -m "first commit"
    ```
4. Rename the branch to main:
    ```bash
    git branch -M main
    ```
5. Add the remote (i.e. Github) tracking:
    ```bash
    git remote add origin https://github.com/user-name/testrepo.git
    ```
6. Push the staged commit to the remote branch main (-u flag is set-upstream)
    ```bash
    git push -u origin main
    ```


## Bread and Butter Commands
* To see all modified files and their <strong>status</strong> (changed, addded, deleted, commited):
    ```
    git status
    ```

* To <strong>pull</strong> the remote repository down to local machine:
    ``` 
    git pull <remote repository>
    ```

* To <strong>add</strong> specific files/directories to be commited.
    ```
    git add <files>
    ```

* To <strong>add all</strong> the files to be commited.
    ```
    git add .
    ```

* To <strong>stage</strong> your changes before publishing them: 
  * The -m flag adds a message describing the changes. 
  * These messages are permanent and will be kept in the history of your repository <strong>forever!</strong>
    ```
    git commit -m "<message>"
    ```

* To <strong>publish</strong> your changes to your remote repository for others to use, see, and change:
    ```
    git push <remote repository>
    ```

* To <strong>create a new branch</strong> and move into it:
  * -b flag creates the branch.
      ```bash
      git checkout -b <branch name>
      git checkout <branch name>
      ```

* To list all branches:
    ```bash
    git branch -a
    ```

## Best practices
* <strong>Pull Before Push</strong> Always pull from the branch you are working on to make sure that you have the most recent version of the remote (i.e., Github) repository.
  * This lets you deal with merge conflicts locally on your machine rather than in your remote repository.  

* <strong>Push Only Working Code (POWC)</strong> Only push functional code to your remote repository so that when others <i>checkout</i> your branch, the code works.
  * Main and develop should generally not be pushed directly to.
  * Merge your code into a develop branch instead and have someone else ensure it works before changing the parent code (main).