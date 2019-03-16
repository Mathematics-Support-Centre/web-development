release: python manage.py migrate
web: gunicorn config.wsgi:application
worker: celery worker --app=web-development.taskapp --loglevel=info
