
# Options for VirtualEnvironments for Python Projects

## Why you want to use virtual environments 

Keeping the library dependencies and versions together, tracked and reproducable will save you an enormous amount of time and hassle in the future.

## There are multiple options for virutal environments, which should I choose?

There are numerous ways to configure virtual environments to your own tastes This link will give you details about the choies

https://docs.python-guide.org/dev/virtualenvs/

### Here is a short summary list of options for you to consider

#### Pipenv

Pipenv is a dependency manager for Python projects. If you’re familiar with Node.js’ npm or Ruby’s bundler, it is similar in spirit to those tools. While pip can install Python packages, Pipenv is recommended as it’s a higher-level tool that simplifies dependency management for common use cases.

``` bash
pip install pipenv
```

#### virtualenv

virtualenv is a tool to create isolated Python environments. virtualenv creates a folder which contains all the necessary executables to use the packages that a Python project would need.

It can be used standalone, in place of Pipenv.

##### Install virtualenv via pip:

``` bash
pip install virtualenv
```

##### Test your installation:
```bash
virtualenv --version
```

##### Basic Usage:  create virtualenv 
```bash 
cd my_project_folder
virtualenv venv
```

##### Basic Usage:  activate virtualenv in the folder 
```bash 
cd my_project_folder
source venv/bin/activate 
```

##### Basic Usage: install a single library into virtualenv 

```bash
pip install requests
```

##### Basic Usage: install a list of libraries into virtualenv from a file like a requirements.txt

```bash
pip install -r requirements.txt 
```
##### Basic Usage: store list of current libraries into a requirements.txt 

```bash
pip freeze > requirements.txt
```