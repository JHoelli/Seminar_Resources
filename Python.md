# Python

## Install Python



## Environments

We use environments to isolate the project librarie and eliminate unintended sideeffects to other projects.
Three ways to create an evironment:
- Venv (with python 3)
- virtualenv (pip install virtualenv)
- anaconda (for binaries, recommended for windows)
- pipenv (pip install pipenv)

Below an Example on how to create such an environment with virtualenv

Got to your Project Folder and create an environment: 

```
virtualenv -p python3 spielwiese
```

Activate the evironment:
```
Linux / Mac: source spielwiese/bin/activate
Windows: ./spielwiese/Scripts/activate
```
## Packages 
For Machine Learning multiple python Packages provide preimplemented funtionalties. If you want to use those packages you need to install them first. 
```
pip install <pandas> oder pip install –r <requirements.txt>
```
## Run a Script
```
python spielwiese.py
```
