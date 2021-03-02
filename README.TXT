Instructions to run the application

Note: We've already done Steps 1 and 2 in class. They're included here for
      completeness

STEP 1: Install the python DB related python modules from the command line:
sudo pip3 install requests flask-mysql flask-wtf flask-sqlalchemy


STEP 2: Set up an account on db4free.net
- Make note of the username/password and database name

STEP 3: Go to the project home directory, and edit .flaskenv as
follows. Modify the database variables (last 3) accordingly:

      FLASK_APP=main.py
      FLASK_DEBUG=1
      DATABASE_NAME='The name of the database you created on db4free.net'
      DATABASE_USERNAME='YOUR username on db4free.net'
      DATABASE_PASSWORD='YOUR password on db4free.net'


    Save your edits and quit micro.


STEP 4: Run the flask application just to initialize the environment variables.
	Type the following in the terminal:

	flask run    (this will start the flask application)
	Ctrl+c       (this will terminate the application)

STEP 5: Still from the project directory, perform the following:
    - Start python interpreter by typing:     python3
    - At the python prompt type:              from app import app
    - At the python prompt type:              from app import db
    - At the python prompt type:              db.create_all()
    - Exit the python interpreter by typing:  quit()

The create_all command creates the database schema defined in app/models.py.
Go to db4free.net and click on myPhpAdmin link (this is very slow).  You should
find your table there.


STEP 6: Now run the Flask application from the project home directory:

    flask run --host=0.0.0.0 --port=8080
