# myDjango

(checked already with homebrew the version..)

1. cd desktop
2. $ mkdir myDjango
3. $ cd myDjango
4. $ python3 -m venv myvenv
5. $ source myvenv/bin/activate<br>
   //remember to replace myvenv with your chosen virtualenv name!<br>
   sometimes source might not be available. In those cases try doing this instead:<br>
             command-line.  $ . myvenv/bin/activate
6. $ pip install --upgrade pip //time to Create a django project
6-1 if needed Remove any old versions of Django (optional)
                python -c "import django; print(django.__path__)"
    
7. pip install Django  // install Django
8. django-admin startproject mysite . //The period . is crucial because it tells the script to 
   install    
   Django in your current directory (for which the period . is a short-hand reference).
9. change settings in mysite/settings.py //TIME_ZONE, LANGUAGE_CODE AND OTHERS
10. set up database in mysite/settings.py

    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.sqlite3',
            'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
        }
    }
10. run python manage.py migrate
11. create a .gitignore file in the base project<br>//this step could be done earlier
 	*.pyc <br/>
	*~ <br/>
	__ pycache __ <br/>
	myvenv <br/>
	db.sqlite3 <br/>
	/static <br/>
  .settings.py//notify related school
	.DS_Store <br/>
12. python manage.py runserver// quit run Ctrl +c <br/>



//some notes related to database//the example here is sql

*change the models(in models.py)
*run _python manage.py make migrations_ to create migrations for those changes
*run _python manage.py migrate_ to apply those changes to the database
//create and admin user
$python manage.py createsuperuser

