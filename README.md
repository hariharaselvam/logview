# logview
Django project to view log files on web page

django-admin startproject logviewer
add django_live_log to INSTALLED_APPS
add url(r'^dll/', include('django_live_log.urls')), to urls.py
add DLL_FILE = '/var/log/myfile.log' to settings.py
python manage.py runserver


 



 



 

