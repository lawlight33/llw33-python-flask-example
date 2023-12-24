## Flask hello-world application

1. In development mode as a script. Built-in server used: 
```shell
python flask_test.py
```
2. In development mode using Flask itself. Flask command is going to be installed along with pip dependency installation:
```shell
flask --app flask_test run
```
3. In production mode from WSGI server:
```shell
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:80 flask_test:app
```