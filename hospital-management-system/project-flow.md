# HMS Project control flow


In the [PROJECT] folder we have the following directory structure

```bash
hms (project main folder)
├── db.sqlite3 (default backend database in SQLite)
├── hms (project configuration folder)
├── hospital (app folder)
├── LICENSE (Our permission doc to others to use our source code)
├── manage.py (django control script to manage the project)
├── README.md (Project doc)
├── requirement.txt (packages needed for the project)
├── static (assest folder containing images etc.,)
└── templates (html frontend pages)
```

[PROJECT] here refers to HMS and [APP] refers to HOSPITAL

## HMS [PROJECT] configuration folder

```bash
hms/hms
├── asgi.py (altertive webserver - not used)
├── __init__.py
├── __pycache__
├── settings.py (settings for hms project)
├── urls.py (add various page urls for the project)
└── wsgi.py (Web Server Gateway Interface script)
```

### Tweaking hms/hms/settings.py

```python
	# For accessing the website from any computer
	ALLOWED_HOSTS = ['*']

	INSTALLED_APPS = [
	    '...',
	    '...',
	    '...',
	    '...',
	    '...',
	    'hospital',
	    'widget_tweaks',
	]

	DATABASES = {
	    'default': {
		# For SQLite backend database
		~~'ENGINE': 'django.db.backends.sqlite3',~~
		~~'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),~~

		# for MySQL backend database
		'ENGINE': 'django.db.backends.mysql',
		# database name
		'NAME': 'hms',
		'USER': '<username to access database>'
		'PASSWORD`': '<password to access database>'
	    }
	}

	# default timezone will be in UTC, change it to IST
	TIME_ZONE = 'Asia/Kolkata'

```
