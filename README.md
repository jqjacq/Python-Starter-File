# Python-Starter-File

### Starter file to set up seperate environment.

#### Steps to get started: 
Inside your terminal and the file you are working on...
1) `git init`
2) `poetry init`
3) Create a poetry.toml file to keep the environment inside this file. 
Inside the file: 
`[virtualenvs] in-project = true` 
4) Install dependency manager: `poetry install`
5) Install dependencies: `poetry add -G dev black isort jupyter`

6) To test out the file, first create a python file then run `poetry run python filename.py` in your terminal.
Alternatively, run `poetry shell`. When running `poetry shell`, make sure to run `deactivate` so you don't run into issues in another environment. 


#### Why these dependencies? 
- Poetry: Dependency Manager, like NPM
- Black: Code formatter, like ESlint
- isort: Sorts dependency
- Jupyter: Web App for notetaking
