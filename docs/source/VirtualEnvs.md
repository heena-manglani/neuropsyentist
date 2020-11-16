Virtualenv
============

Tool to manage and isolate project dependencies.

* Reproducibility crisis no more!
    * Have all of the packages you need for a specific project in the exact version needed.
    * Include a requirements file that lists all of the packages and their dependencies.
    * Can share your env so others can cleanly duplicate your env and run the code.


## Bread and Butter Commands
To <strong>create</strong> a virtual env, execute the venv module (part of the Python standard lib):
```
python 3 -m venv phd/
```

To <strong>activate</strong> a virtual env:
```
source phd/bin/activate
````

<strong>Install</strong> a package to the virtual env:
```
pip install numpy as np
```

To create a <strong>requirements</strong> file:
```
pip freeze > requirements.txt
```

To <strong>duplicate</strong> someone else's env:
* pull their repo
* create a virtual env
* and install its dependencies
```
pip install -r requirements.txt
```

To <strong>exit</strong> the env:
```
deactivate
```

## Need to Know
* Virtual envs will live in your home dir ~/env/
