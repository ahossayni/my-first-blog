commandes
  python -m venv myvenv
  pip install django==1.8
  myvenv\Scripts\activate
  django-admin startproject mysite .
  myvenv\Scripts\activate
  django-admin startproject mysite .



dans le fichier mysite/settings.py
  TIME_ZONE = 'Europe/Paris'
  STATIC_URL = '/static/'
  STATIC_ROOT = os.path.join(BASE_DIR, 'static')


commandes:
  python manage.py migrate

lancer le serveur
  python manage.py runserver
  l arreter avec Ctrl+c

creer un projet blog:
  python manage.py startapp blog

dans mysite/settings.py ajouter 'blog' à:
INSTALLED_APPS = (
  'django.contrib.admin',
  'django.contrib.auth',
  'django.contrib.contenttypes',
  'django.contrib.sessions',
  'django.contrib.messages',
  'django.contrib.staticfiles',
  'blog',
)
