#creating a project
```
django-admin.py startproject mysite
```
<br>
```
python manage.py syncdb
```
<br>
```
python manage.py startapp polls
```
<br>

```
v polls/models.py
#add
from django.db import models

class Poll(models.Model):
    question = models.CharField(max_length=200)
    pub_date = models.DateTimeField('date published')

class Choice(models.Model):
    poll = models.ForeignKey(Poll)
    choice_text = models.CharField(max_length=200)
    votes = models.IntegerField(default=0)

