Docker Django
-
1. Create the Django project by running: `sudo docker-compose run web django-admin startproject <Project Name> .`
2. Modify the `DATABASES = ...` variable in `<Project Name>/settings.py` to...
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

Reference
-
- https://docs.docker.com/compose/django/
- https://docs.djangoproject.com/en/2.2/intro/tutorial01/