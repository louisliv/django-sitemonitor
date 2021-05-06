# django-sitemonitor
Web-based system monitor for Django

## Installation

##### Add URL route to settings

In `urls.py` add the desired route

```python

urlpatterns = [
    ...
    path('sitemonitor', include('django_sitemonitor.urls')),
]
```

##### Add to installed apps in settings

In `settings.py` add the `django_sitemonitor` app to `INSTALLED_APPS

```python
INSTALLED_APPS = [
    ...
    'sitemonitor'
]
```

##### Add URL route to settings

In `settings.py` add the same url that was added to `urls.py`

```python
SITEMONITOR_PATH = 'sitemonitor'
```

## Devolpment

##### Build Frontend

Execute the following commands to setup the development environment

```bash
$> cd <PATH_TO_REPO>/client
$> ng build --prod --base_href {{base_path}} --deploy_url /static/sitemonitor/
```
