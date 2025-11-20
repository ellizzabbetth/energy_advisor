# Purpose of This Repo

This repo is meant to be used to keep things organized during content development and act as the source of truth for all projects and exercises related to this course.

## Python Version
Python version 3.9.2

python -m venv .venv   
.venv\Scripts\activate   


https://www.youtube.com/watch?v=15AI-2_C51w
VS Code's terminal using a different python interpreter than the one you've selected
https://stackoverflow.com/questions/48135624/how-can-i-change-the-python-version-in-visual-studio-code

## Folder Structure
The error "ModuleNotFoundError: No module named 'sqlalchemy'" in Jupyter Notebook, despite SQLAlchemy appearing as installed, typically occurs due to a mismatch between the Python environment where SQLAlchemy was installed and the environment Jupyter Notebook is using.
 This often happens when packages are installed in a different Python version or virtual environment than the one Jupyter is running on.

To resolve this, first verify the Python interpreter Jupyter is using by running sys.executable in a notebook cell. Compare this path with the one used to install SQLAlchemy. If they differ, the package was installed in a different environment.
 For example, if Jupyter is using a system Python while SQLAlchemy was installed via a user-specific pip, the notebook won't find it.
 
cd project
python -m venv .venv
.venv\Scripts\activate
cd ../
pip install -r requirements.txt
cd ecohome_solution
pip install -r requirements.txt
python --version


How to use pip for pyenv?
# Source - https://stackoverflow.com/a
# Posted by jmh
# Retrieved 2025-11-20, License - CC BY-SA 4.0

pyenv local 2.7.14
pip install -r requirements.txt

### Lesson Folder

This repo contains a folder for each `lesson` and one `project` folder.

Example
```
lesson-1-hello
lesson-2-world
lesson-3-foo
lesson-4-bar
project
```

Each `lesson` folder is named using the naming convention of `lesson-#-name-of-lesson`.

Example
```
lesson-1-hello
```

Four lesson folders have been provided as a template; However, you may need to add more or possibly use less than four depending on what is needed.

If you require an additional lesson folder, you can make a copy of the folder and paste it into the root directory.

### Exercises Folder

Each `lesson` folder contains an `exercises` folder. This `exercises` folder should contain all files and instructions necessary for the exercises along with the solution. The solutions for these exercises will be shared with students. See the `README` in the `exercises` folder for information about folder structure.

### Project Folder

The `project` folder should contain all files and instructions necessary for setup. If possible, a set of instructions should be provided for both Udacity workspaces and a way to work locally (for both MacOS and Windows OS). At a minimum, one set of instructions should be provided. A `README` template has been provided in the project folder. This template layout should be used to write your README.
