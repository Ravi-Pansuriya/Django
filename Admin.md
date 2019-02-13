# Create super user
We'll also create an initial user named admin with a password of geeky1234.
```
python3 manage.py createsuperuser --email admin@geekyworks.com --username admin
```
Enter password and you got a new super user account.  
You can authenticate that user at [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin).
