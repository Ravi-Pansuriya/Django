# How install and configure Django REST Framework
Inatalltion process and setting up rest framework in Django is very easy.

## Step 1: Install virtualenv for python
Now, type this command in your terminal.
```
sudo pip3 install virtualenv
```
Okay, after installing, we need to create the virtual environment. Now you will create this folder when you are putting your other projects. Mine is desktop >> project folder. So navigate to that and type the following command and create project directory.
```
mkdir Erranzer
cd Erranzer
```
In my case, My virtualenv folder name is **env**. we will keep our environment setup in separate directory.
```
virtualenv -p python3 env
```
Now, activate the virtual environment by typing the following command without leaving project directory.
```
source env/bin/activate
```
You will see your terminal looks like below.  
![image-02](https://github.com/Ravi-Pansuriya/Django/blob/master/assets/images/image-02.png)  
So, our virtual environment has been started. Now, this is the time to install the Django Framework.

## Step 4: Install Django In env
Okay, now stay in that folder and install **Django** and **Djanfo REST Framework** using the following command.
```
pip3 install django
pip3 install djangorestframework
```
It will download the Django and rest framework in project.

## Step 5: Set up a new project with a single application
We need to install skeleton of the Django project. So type the following command.
```
django-admin startproject Erranzer
```
Here, our project name is Erranzer. Next, go into that folder.
```
cd Erranzer
```
Now we will create an app name **api**
```
django-admin startapp api
```
The project layout should look like:
```
$ pwd
<some path>/Erranzer
$ find .
.
./Erranzer
./Erranzer/__init__.py
./Erranzer/settings.py
./Erranzer/urls.py
./Erranzer/wsgi.py
./api
./api/migrations
./api/migrations/__init__.py
./api/models.py
./api/__init__.py
./api/apps.py
./api/admin.py
./api/tests.py
./api/views.py
./manage.py
```
Finally, we have created the project. Now we may need to migrate apps installed by scalaton by typing this command.
```
python3 manage.py migrate
```
Now start the project server by typing the following command.
```
python3 manage.py runserver
```
![image-03](https://github.com/Ravi-Pansuriya/Django/blob/master/assets/images/image-03.png)  
It has started the development server, and we can access it via localhost:8000

Navigate to the browser, and you will see the screen like this.
![image-04](https://github.com/Ravi-Pansuriya/Django/blob/master/assets/images/image-04.png)  
