# Python-Starter-File

### Starter file to set up separate environment.

#### Steps to get started: 
Inside your terminal and the file you are working on...
0) Initializing empty Git repository (if you are uploading to Github) In terminal: `git init`
1) Create a folder and inside the folder, create a python file. Example: python_file.py
2) Create a new Poetry project. In terminal: `poetry init` <br>
   Poetry is a dependency management tool that manages dependencies, packages, and libraries in your Python project. <br>
   Once initialized, it will ask you to fill out the following: Version, Description, Author, License, Compatible Python versions, define main dependencies interactively, and development dependencies interactively. These are optional, if you wish to skip it, press enter. <br>
I don't define main dependencies and development dependencies interactively. Once filled out, you will see a `pyproject.toml` file.  TOML is a file format for configuring files. 

3) Create a `poetry.toml` file to keep the environment inside this file. 
Inside the file: `[virtualenvs] in-project = true`

  - TIP 1: Make sure there is a break between `[virtualenvs]` and `in-project=true`. Here is an example of how it should look like: 
`[virtualenvs]` \
               `in-project=true`
  - TIP 2: To make sure the environment is inside the project: Inside your terminal, write `poetry config --list`. <br>
  You should see `virtualenvs.in-project = true`, NOT null. 
4) Installing the dependency manager tool. In terminal: `poetry install` \
5)  In terminal: `poetry add -G dev black isort jupyter` 
Installing dependencies: Black, isort, and jupyter.

#### Why should I install a dependency management tool?
There will always be updates happening. The dependency management tool will help with version control and version compatibility. <br>

#### Why these dependencies? 
- Poetry: Dependency Manager, like NPM
- Black: Code formatter, like ESlint
- isort: Sorts dependency
- Jupyter: Web App for notetaking

6) To test out the file, first create a python file then run `poetry run python filename.py` in your terminal.
Alternatively, run `poetry shell`. When running `poetry shell`, make sure to run `deactivate` so you don't run into issues in another environment. 



To make folders in terminal and to change directory: (or just use VSCode to make the folders and files)
- Make folder: `mkdir name_of_folder`
- Change directory: `cd name_of_folder`
- Move up a file: `cd ../` 
- Create files: `touch name_of_file.py`
<br> 
Here is example of how the file format for Python and Jupyter should look like: 
<br>
Python: name_of_file.py
<br>
Jupyter: name.ipynb

**Optional**: Making a `src` folder for python files and `notebook` folder for jupyter files. I create them to keep the files organized. 
