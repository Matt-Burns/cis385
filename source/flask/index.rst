Fun With Flask
==============
Below you will find links to many things Flask. As a novice Python developer I found them helpful!

Read All About Flask
--------------------
| Flask is a web framework that provides libraries to build lightweight web applications in python.
| If you are familiar with other web development frameworks and know enough python to get by you should check out `Flask <https://flask.palletsprojects.com/en/2.0.x//>`_.

Flask Tutorial
--------------
| Get up to speed fast! Complete this basic `Flask Tutorial <https://flask.palletsprojects.com/en/2.0.x/tutorial/>`_ provided by the fine folks at Pallets Projects.

Virtual Environments
--------------------
| Confusing yet satisfying. `Python V Env Tutorial <https://docs.python.org/3/tutorial/venv.html>`_.

Flask and Click
---------------
| `Pallets Projects Click <https://click.palletsprojects.com/en/8.0.x/>`_ can be used in conjunction with Flask to extend the Flask CLI.

Flask CLI: Avoid Setting FLASK_APP Environment Variable
-------------------------------------------------------
| Flask CLI command 'run' starts a new Flask environment located in the directory given by the FLASK_APP environment variable.
  The Flask environment scans python packages in FLASK_APP directory looking for a Flask application or factory.
  Should FLASK_APP not be set, Flask will fail to start the environment.
  Ensuring the FLASK_APP variable is set properly before starting a Flask environment can be a pain.
  Luckily Flask can be started, sans FLASK_APP, as long as there is an app.py in the directory Flask run is being executed in.
  The app.py must provide a Flask application or factory.
  I found this to be handy for my local development environment. Here is the app.py I used to start the flaskr tutorial app.

.. code-block:: python

   import flaskr


   def create_app(test_config=None):
       print(test_config)
       return flaskr.create_app(test_config)

