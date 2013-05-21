#Installing Django
#### from net.tutsplus.com/tutorials/python-tutorials/python-from-scratch-creating-a-dynamic-website
<br>
<br>
<br>

```
wget http://www.djangoproject.com/download/1.3.1/tarball/
tar xzvf Django-1.3.1.tar.gz
rm Django-1.3.1.tar.gz
cd Django-1.3.1
python setup.py install
``````
<br>
<br>
<br>
<br>
<br>

```
python
from django import get_version
get version()
```

<br>
<br>
<br>
<br>
<br>

##In use
<br>
```
django-admin.py startproject folderName   #makes project folder
```

### in the created folder ...
1.' __init__.py '
    * telling python it's package
2.' manage.py '
    * contains functions to manage page
3.' settings.py '
    * has website settings
4.' urls.py '
    * maps URLs to pages
<br><br><br><br><br><br><br><br><br>
##To make it work..
#We need APPS !
that change codes --> web functions !
<br><br>
##Each app to serve one distinct purpose
```
python manage.py startapp blog
cd blog
ls
```
<br><br>
##inside the blog just created ...
##Define our data structures in models
* accessing data:
    via models

* in the views file:
    wirte the code that actually generates the web pages



<br><br><br><br><br><br><br><br><br>
#When user types URL ...
#### It is sent by the urls script
#### and get relevant data from the models
#### ---> process ---> template ---> website !

