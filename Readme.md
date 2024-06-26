### Python Virtual Environment Setup Script 
```bash
#!/bin/bash

# Create the normal virtual environment
python -m venv myenv

# Activate the virtual environment
source myenv/Scripts/activate

# Create the virtual environment in UV
# On Windows.
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
# then 
uv venv

# Activate the virtual environment in UV
.venv\Scripts\activate

```
## Now For Django Project 

```bash
# For django Create a new Django Project
django-admin startproject myproject

# Go to folder in Django project / 
cd myproject

# Run server
python manage.py runserver

# Make requirements.txt file for the virtual environment created above
pip freeze > requirements.txt

```
## For FastAPI 

```bash
# install
# For FastAPI just install
pip install fastapi uvicorn

# Make API flder
# make main.py file and write route logic
# start Server
uvicorn API.main:app --reload # API. is file name 





