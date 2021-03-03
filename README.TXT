Instructions to run the application

STEP 1: Install the Flask login and security modules from the command line:
  sudo pip3 install flask_login werkzeug

STEP 2: Go to the project home directory, and edit .flaskenv as
follows. Modify the database variables (last 3) accordingly:

      FLASK_APP=main.py
      FLASK_DEBUG=1
      DATABASE_NAME='The name of the database you created on db4free.net'
      DATABASE_USERNAME='YOUR username on db4free.net'
      DATABASE_PASSWORD='YOUR password on db4free.net'

    Save your edits and quit micro.

STEP 3: Now run the Flask application from the project home directory:

    flask run --host=0.0.0.0 --port=8080

STEP 4: Login credentials for application:

  Admin username: admin   password: csc330sp21
  Regular user:   user    password: csc330sp21
