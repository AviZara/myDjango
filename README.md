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
   django-admin startproject mysite . //The period . is crucial because it tells the script to 
   install    
   Django in your current directory (for which the period . is a short-hand reference).
8. create a .gitignore file in the base project
 	*.pyc <br/>
	*~ <br/>
	__ pycache __ <br/>
	myvenv <br/>
	db.sqlite3 <br/>
	/static <br/>
	.DS_Store <br/>
9. python manage.py runserver// quit run Ctrl +c <br/>
