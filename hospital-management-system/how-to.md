## How to run HMS project

- Move to project folder in Terminal. Then run the command :
```
pip install -r requirement.txt
```

- After successfull install of packages by pip, Now run following commands:
```
py manage.py makemigrations
py manage.py migrate
py manage.py runserver 0:8000
```

- Now enter following URL in Your Browser Installed On Your Pc
```
http://127.0.0.1:8000/
