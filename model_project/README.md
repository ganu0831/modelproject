<b>steps of create a models in Django: -</b><br>
step
1) make sure to write our app path in settings.py
   

    INSTALLED_APPS = [
    ...
    ...
    'polls.apps.PollsConfig', # our app address <br>
    ]

    polls -> app_name.
    apps -> it is a file in our app called "apps.py".
    PollsConfig -> it is a class in 'apps.py'.

2) run commands for activation/creation of DB

       python manage.py makemigration

<b>Output<br></b>

       Migrations for 'polls':
           polls\migrations\0001_initial.py
              - Create model Question
              - Create model Choice

3) then run this command for implementation of these fields we created/Modified
  
       python manage.py migrate

<b>output:</b>

         Operations to perform:
            Apply all migrations: admin, auth, contenttypes, polls, sessions
         Running migrations:
            Rendering model states... DONE
            Applying polls.0001_initial... OK