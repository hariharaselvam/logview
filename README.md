# logview
### Django project to view log files on web page

## install django live log
### $ sudo pip install django_live_log

## Create folder
### $ mkdir log_project

## Go to folder
### $ cd log_project/

## Start Django Application
### $ django-admin startproject logviewer
 this will create manage.py db.sqllite3 and a folder as logviewer and the folder will have __init__.py, settings.py, urls.py and uwsgi.py

## Add APP 
### add 'django_live_log' to INSTALLED_APPS, as an app to the project by editing settings.py

## Add URL
### add url(r'^dll/', include('django_live_log.urls')), to urls.py and import include from django.conf.urls

## Add LOG
### add a line DLL_FILE = '/var/log/myfile.log' to settings.py for absolute path of log file

## Run Django
### $ python manage.py runserver 
 this will run the django web application with default domain localhost and default django port 8000


## Out put

 to view the log file

http://localhost:8000/dll 


 to read 500 lines of log file

http://localhost:8000/dll/?from=500


 to read any other log file

http://localhost:8000/dll/?file_path=/Users/hariharaselvam/elasticsearch-5.3.0/logs/elasticsearch.log


 



 



 

