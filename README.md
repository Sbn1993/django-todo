# django-todo
A simple todo app built with django

![todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoApp.png)
### Setup
```bash
$ sudo -i
First of all make a directory named projects
$ mkdir projects
To get this repository, run the following command inside your git enabled terminal
```bash
$ git clone https://github.com/shreys7/django-todo.git
```
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide
```
Go to the directory 
$ cd django-todo/

Then install pip with the help of 
$ apt install python3-pip

update the packages again with 
$ apt-get update

To install django, use
$ pip3 install django

```
Once you have downloaded django, go to the cloned repo directory and run the following command

```bash
$ python3 manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.
```
You may get errors, make necessary changes in settings.py file
$ vi todoApp/settings.py
```
Run this again and check for errors/nil
$ python3 manage.py makemigrations
```

Now, to apply this migrations run the following command
```bash
$ python3 manage.py migrate
```

One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user
```bash
$ python3 manage.py createsuperuser
```

That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash
$ python3 manage.py runserver:8002
```
You may need to allow host, to do so again open settings.py file and in allowed hosts add '*'
```

Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Cheers and Happy Coding :)
