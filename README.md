# Python-Starter-File

### Starter file to set up seperate environment.

#### Steps to get started: 
Inside your terminal and the file you are working on...
1) In terminal: `git init`
Initializing empty Git repository.
2) `poetry init` \
Optional to fill out Version, Description, Author, License, Compatible Python versions, define main dependencies interactively, and development dependencies interactively. I don't define main dependencies and development dependencies interactively. Once filled out, confirm generation. 
3) Create a `poetry.toml` file to keep the environment inside this file. 
Inside the file: `[virtualenvs] in-project = true`

  - TIP 1: Make sure there is a break between `[virtualenvs]` and `in-project=true`. Here is an example of how it should look like: \
`[virtualenvs]` \
               `in-project=true`
  - TIP 2: To make sure environment is inside the project: Check with `poetry config --list` where `virtualenvs.in-project = true`, not null. \
4) In terminal: `poetry install` \
Installing dependency manager
5)  In terminal: `poetry add -G dev black isort jupyter` 
Installing dependencies: Black, isort, and jupyter. 

6) To test out the file, first create a python file then run `poetry run python filename.py` in your terminal.
Alternatively, run `poetry shell`. When running `poetry shell`, make sure to run `deactivate` so you don't run into issues in another environment. 

#### Why these dependencies? 
- Poetry: Dependency Manager, like NPM
- Black: Code formatter, like ESlint
- isort: Sorts dependency
- Jupyter: Web App for notetaking

**Optional**: Making a `src` folder for python files and `notebook` folder for jupyter files. I create them to keep the files organized. 
<br> To make folders in terminal and to change directory: (or just use VSCode to make the folders and files)
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
