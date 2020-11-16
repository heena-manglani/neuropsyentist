Virtualenvs
============

Tool to manage and isolate project dependencies. <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands" target="_blank" rel="noreferrer">Documentation</a>


* Reproducibility crisis no more!
  * Have all of the packages you need for a specific project in the exact version needed.
  * Share your env including all packages and their dependencies.


## Bread and Butter Commands
To <strong>create</strong> a virtual env, execute the venv module (part of the Python standard lib):
```
conda create --name phd python=3.8 <package name>
```

<strong>Install</strong> a package to the virtual env:
```
conda install -n phd numpy
```

To <strong>activate</strong> a virtual env:
```
conda activate phd
````

To <strong>export</strong> your env:
```
conda activate phd
conda env export > environment.yml
```

To <strong>duplicate</strong> someone else's env:
* pull their repo, create a virtual env, and install its dependencies
```
pip install -r requirements.txt
```

To <strong>view</strong> a list of your envs:
```
conda env list
```

To <strong>exit</strong> the env:
```
source deactivate
```

## Need to Know
* Virtual envs will live in your home dir ~/envs/.
