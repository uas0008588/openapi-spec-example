# PIPENV Quick Guide
### set in vim ~/.bash_profile or set in for all users in /etc/profile.d/pipenv.sh inorder to create the virtual enviroment in project directory
`export PIPENV_VENV_IN_PROJECT=1`
### Remove virtual enviroment
`pipenv --rm`
### Find the python version
`pipenv run where python`
### Find path of virtual enviroment
`pipenv --venv`
### Package Uninstall `--all` will uninstall all the packages or `--all-dev` will remove all developmetn pkgs
`pipenv uninstall <pkg_name>`
### Install Package
`pipenv install <pkg_name>`
### Install package for development enivorment only
`pipenv install <pkg_name> -d or --dev` 
### Check for security vulneribilites
`pipenv check`
### Find the home directory of project
`pipenv --where`
### Activate the virtualenviroment 
`pipenv shell`
##### or
#### Run the app in virtual enviroment
`pipenv run python <app.py> `
### Create the virtaul enviroment otherwise it will create automatically
`pipenv --three`
### Cpdate the pipfile.lock file from pip
`pipenv lock`
### Install the packages from pipfile.lock instead of pipfile
`pipenv install --ignore-pipfile`
### Install the package from requirement.txt
`pipenv install -r requirement.txt`
### Generate the requirement.txt file
`pipenv lock -r > requirement.txt`
### Create the virtual enviromentwith specific python version
`pipenv --python 3.6`


#### .flaskenv  
```
export FLASK_APP=src
export FLASK_DEBUG=1
export SQLAlchemy_DB_URI=sqlite:///bookmarks.db
export JWT_SECRET_KEY='JWT_KEY'
```
#### .env file
`export SECRET_KEY=dev`
### flask run cmd
`flask run`
