# Django Python CRUD Operation Book Example
This is a simple Django project to demonstrate Django CRUD functionality using Python and TiDB

[Demo Link](https://gitpod.io/#/github.com/ti-click/Django-Python-MySql-CRUD-Operation-Book-Example)

# 1. Ready TiDB Cluster
### 1.1 Get the Gitpod public IP
```
$ curl https://ipinfo.io/ip 
```
### 1.2 Create TiDB Cluster on TiDB Cloud 

### 1.3 Setting Password and Gitpod Public IP 

### 1.4 Getting the Password and connect URL

# 2. Import data into TiDB Cluster
First Testing mysql client and connect URL is well work.
```
$ mysql -u root -h ${URL} -P 4000 -p${Password}
```
Start import 
```
$ mysql -u root -h ${URL} -P 4000 -p${Password} < /workspace/Django-Python-MySql-CRUD-Operation-Book-Example/mysite.sql
```

# 3. Update the setting.py file
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'mysite',
        'USER': 'root',
        'PASSWORD': '${Password}',
        'HOST': '${URL}',
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
