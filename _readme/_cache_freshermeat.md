python310 -m venv venv
venv\Scripts\activate.bat
poetry install
pip install sgmllib3k==1.0.0 snaptime==0.2.4
cd freshermeat/static/
mklink /D npm_components ..\..\node_modules
set FLASK_APP=runserver.py
set APPLICATION_SETTINGS=development.py
...