# Step 1: Install Python on Mac
Python is already installed on brand new Mac, but its version is old. So what we do is to install the latest version of python using homebrew.
```
brew install python3
```
Okay, after it will complete the installation, you will type the following command to check the version. First type python3 in your terminal. Since MacOS X has already python installed, we cannot uninstall the old version because otherwise the Python 2 supported programmes will be stopped and we need to reinstall the mac. So we need to type python3 instead of python.
```
python3
```
It will display the version, and now we can execute the python code.
[image]()
Okay, so we have successfully installed the python 3. Now, to out from the python console, we need to type exit().

# Step 2: Install Pip package management system
Pip is the package management system used to install and manage software packages written in Python. Now, install it using the following command.
```
sudo easy_install pip
```
# Step 3: Install virtualenv for python
Now, type this command in your terminal.
```
sudo pip3 install virtualenv
```
Okay, after installing, we need to create the virtual environment. Now you will create this folder when you are putting your other projects. Mine is desktop >> code folder. So navigate to that and type the following command. In my case, My virtualenv folder name is **Geekyworks**.
```
virtualenv -p python3 Geekyworks
```
Okay, so it will install the required folders. Now, go into that folder.
```
cd Geekyworks
```
Now, activate the virtual environment by typing the following command. Please Make sure you are in the virtual environment directory.
```
source bin/activate
```
You will see your terminal looks like below.
[image]()
So, our virtual environment has been started. Now, this is the time to install the Django Framework.

# Step 4: Install Django In Mac
Okay, now stay in that folder and install Django using the following command.
```
sudo pip3 install django
```
It will download the Django project. Check the Django version using the following command.
```
python3 -m django --version
```

# Step 5: Create the Django Project
We need to install skeleton of the Django project. So type the following command.
```
django-admin startproject Erranzer
```
Here, our project name is Erranzer. Next, go into that folder.
```
cd Erranzer
```
Finally, we have created the project. Now we may need to migrate apps installed by scalaton by typing this command.
```
python3 manage.py migrate
```
Now start the project server by typing the following command.
```
python3 manage.py runserver
```
[image]()
It has started the development server, and we can access it via localhost:8000

Navigate to the browser, and you will see the screen like this.
[image]()

# Step 6: Open Django on Visual Studio Code
If you have not installed Visual Studio Code on Mac then please check out below tutorial. 

Related Post:  [How To Install Visual Studio Code On Mac](https://appdividend.com/2018/03/17/how-to-install-visual-studio-code-on-mac/)
This step is optional because if you are using Visual Studio Code, then it will be helpful to you. If you are using another IDE like pycharm or editor like sublime text, then you can skip this step. First, perform the following step.

Install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python).

Now, open our project in the visual studio code using the following command.
```
code .
```
Please make sure, you are at the root of the Erranzer folder.

You will get the folder structure like this.
[image]()
Finally, How To Install Django In Mac tutorial is over. Thanks!!
