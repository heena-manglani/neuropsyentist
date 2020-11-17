Virtualenvs
============

Tool to manage and isolate project dependencies. <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands" target="_blank" rel="noreferrer">Documentation</a>


* Reproducibility crisis no more!
  * Have all of the packages you need for a specific project in the exact version needed.
  * Share your env including all packages and their dependencies.


## Bread and Butter Commands
To <strong>create</strong> a virtual env:
```
conda create --name <env_name> python=3.8 <package>
```
To <strong>activate</strong> a virtual env:
```
conda activate <env_name>
````

<strong>Install</strong> a package to the virtual env:
```
conda install numpy
```

To <strong>view</strong> a list of your envs:
```
conda env list
```

To <strong>exit</strong> the env:
```
conda deactivate
```

To <strong>export</strong> your env:
```
conda activate <env_name>
conda env export > environment.yml
```

To <strong>duplicate</strong> an existing env:
```
conda install -n <env_name> environment.yml
conda activate <env_name>
```

## Need to Know
* Virtual envs will live in your home dir /opt/anaconda3/envs/.
