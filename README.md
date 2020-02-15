Docker Django
-
1. Create the Django project by running: `docker-compose run web django-admin startproject <Project Name> .`
2. Modify the `DATABASES = ...` variable in settings.py to...
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'HOST': 'db',
        'PORT': 5432,
    }
}
```
3. Run with `docker-compose up`