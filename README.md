# how2use
"How2use" is a personal repository that aims to consolidate a continued study of certain technologies to be openly shared with IT community, providing a faster learning curve for any other person.

# Python CMS Jango

## What is?

## How?

## Install

1 - Considerations

Please, considerer that this steps were here defined on Mar/2020 and are intended to guide you on python 3.7 (at least).

2 - Python pip update

At first, let's bring our pip release to the latest stable release available

```shell
python get-pip.py
```

3 - Virtualenv package install

Let's create a virtual environment with "virtualenv" package

```shell
pip install virtualenv
```

4 - virtualenvwrapper-win install

Let's now install virtual env wrapper

```shell
pip install virtualenvwrapper-win

easy_install virtualenvwrapper-win

git clone git://github.com/davidmarble/virtualenvwrapper-win.git

cd virtualenvwrapper-win

python setup.py install

set WORKON_HOME=%VIRTUAL_ENV%\..\Envs

mkdir -p %WORKON_HOME%

%VIRTUAL_ENV%\Scripts\virtualenvwrapper.sh

mkvirtualenv pub

```

5 - Django-CMS package instakk

```shell
pip install djangocms-installer
```

6 - Create your first Django CMS project

Let's now ask django package to create a project
```sh
djangocms -p [project name] [Django CMS template]
```
For this firts try, consider using "modern_business" as the [Django CMS template]

Remarks:
- Do not consider creating a too long path as a project name
- Do not execute the command from your python IDE. Use your OS prompt directly


4 - Active your project

```shell
source ./[project name]/bin/activate
```


5 - Start your django CMS web server

```shell
python manage.py runserver
```

6 - Access the administration default page 

* URL:  http://127.0.0.1:8000
* user: admim
* pwd: admin


7 - Project dependencies update

List you dependencies and update the dependency requitement file for further deploys

```shell
pip freeze > requirements.txt
```

Remarks: 

Whenever the project install is demanded in another location, consider using:
```shell
pip install -r requirements.txt
```