<h1 align='center'>Django Install On Ubuntu</h1>
<p>Django is a full-featured Python web framework for developing dynamic websites and applications. Using Django, you can quickly create Python web applications and rely on the framework to do a good deal of the heavy lifting.</p><br>

<h2 align='center'>Global Install From Packages</h2>
<p align = 'justified'>If you wish to install Django using the Ubuntu repositories, the process is very straightforward.</p>     
<p>First, update your local package index with apt:</p>

```
$ sudo apt update
$ python3 -V
```

<p>You will see a result just like this:</p>

```
$ Python 3.9.5
```



<p>Next step is to install Django in your system</p>

```
$ sudo apt install python3-django
$ django-admin --version
```



<p>You will see a result just like this:</p>

```
$ 2.2.20
```



All you have to do is now install the ***pip*** and ***virtual*** environment from Ubuntu repositories.

```
$ sudo apt install python3-pip
$ sudo apt install python3-venv
```



<h2 align='center'>Create a  Simple Django Project to check everything is fine</h2>

To create an project first you have to go to your directory where you want to open your project and open the terminal and write those following commands:

```
$ django-admin startproject [project_name]
$ cd [project_name]
```

Now, you have to create a virtual environment

```
$ python3 -m venv .
```

To install packages into the isolated environment, you must activate it by typing:

```
$ source bin/activate
```

In your new environment, we can use `pip` to install Django. Regardless of your Python version, `pip` should just be called `pip` when you are in your virtual environment. Also note that you *do not* need to use `sudo` since you are installing locally:

```
$ (project_name)$ pip install django
```

We can verify the installation by typing:

```
$ (project_name)$ django-admin --version
```

Start the development server:

```
$ (project_name)$ python manage.py runserver
```

