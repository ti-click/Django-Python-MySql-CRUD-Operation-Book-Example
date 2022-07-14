# Django Python CRUD Operation Book Example
This is a simple Django project to demonstrate Django CRUD functionality using Python and TiDB

# 1. Required TiDB Cluster
TODO

# 2. Import data into TiDB Cluster
```
$ mysql -u root -h ${url} -P 4000 -p < /workspace/Django-Python-MySql-CRUD-Operation-Book-Example/mysite.sql
password:
```

# 3. Update the setting.py file
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'mysite',
        'USER': 'root',
        'PASSWORD': '${password}',
        'HOST': '${url}',
        'PORT': '4000'
    }
}
```

# 4. Run python command
```
$ cd /workspace/Django-Python-MySql-CRUD-Operation-Book-Example/mysite
$ python manage.py migrate
$ python manage.py runserver 0.0.0.0:7000
```

# 5. Then open the URL
TODO

# Thanks 
This example app is reference [Django-Python-MySql-CRUD-Operation-Book-Example](https://github.com/pdjani91/Django-Python-MySql-CRUD-Operation-Book-Example)
