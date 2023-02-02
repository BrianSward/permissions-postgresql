# LAB - Class 33
## Project: Authentication & Production Server
### Author: Brian Sward
### Links and Resources
PORT - 8000
DATABASE_URL - http://localhost:8000/admin/ 
### How to initialize/run your application (where applicable)
`gunicorn snacks_project.wsgi:application –bind 0.0.0.0:8000 –workers 4`
### Tests
- How do you run tests?
 - Thunderclient
- Any tests of note?
  - Yes there are - using Thunderclient, first test for tokens by a:
    - POST to http://127.0.0.1:8000/api/token/
      - be sure to include in the Body the following:
        - {"username": "admin", "password": "admin"}
  - There are more tests to come but awaiting a message in slack to describe them
  
# LAB - Class 32
## Project: Permissions & Postgresql
### Author: Brian Sward
### Links and Resources
PORT - 8000
DATABASE_URL - http://localhost:8000/admin/ 
### How to initialize/run your application (where applicable)
`python manage.py runserver`
### Tests
- How do you run tests?
 - `python manage.py test`
- Any tests of note?
  - make sure you run them in a sqlite3 database as this is how i was instructed to
