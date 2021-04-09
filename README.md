# Django_setup_db_mysql_postgre_sqlite

Django_setup_db_mysql_postgre_sqlite

> mysql/mariabd

settings.py

# @sqlite3 => https://github.com/DENRIV/PythonDjangoCrudBooks/blob/master/apps/settings.py

DATABASES = {

    'default': {
    
        'ENGINE': 'django.db.backends.sqlite3',
        
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
        
    }

# @mysql [real] => https://github.com/DENRIV/crud_django_bootstrap/blob/main/crud_django_bootstrap/settings.py

DATABASES = {

    'sqlite': {
    
        'ENGINE': 'django.db.backends.sqlite3',
        
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
        
    },
    
    'default': {
    
        'ENGINE': 'django.db.backends.mysql',
        
        'NAME': 'productos',
        
        'USER': 'root',
        
        'PASSWORD': '',
        
        'HOST': 'localhost',
        
        'PORT': '3306',
        
        'OPTIONS': {
        
            'sql_mode': 'traditional',
            
        }
        
    }
    
}

# @postgre => https://github.com/DENRIV/Python_Django_postgresql_PetAdoption/blob/main/refugio/settings.py

DATABASES = {

    'default': {
    
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        
        'NAME': 'refugio',
        
        'USER': 'postgres',
        
        'PASSWORD': 'sa',
        
        'HOST': 'localhost',
        
        'PORT': 5432,

    }
    
}

