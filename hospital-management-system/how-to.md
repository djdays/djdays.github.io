## How to run HMS project

- Move to project folder in Terminal. Then run the command :
```
pip install -r requirement.txt
```

- After successfull install of packages by pip, Now run following commands:
```
python manage.py makemigrations
python manage.py migrate
python manage.py runserver 0:8000
```

- Now enter following URL in Your Browser Installed On Your Pc
```
http://127.0.0.1:8000/
