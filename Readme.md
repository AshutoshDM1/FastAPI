##### Python Virtual Environment Setup Script ##

#!/bin/bash

# Create the virtual environment
python -m venv myenv

# Activate the virtual environment
source myenv/Scripts/activate


# Create the virtual environment in UV
uv venv  
# Activate the virtual environment in UV
.venv\Scripts\activate  
# create a  new Django Project
django-admin startproject myproject
# go to folder in django project
cd myproject
# run server
python manage.py runserver

# make requirements.txt file for the virtual environment created above 
pip freeze > requirements.txt
