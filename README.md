# webapp-flask-sqlite3-template

A template for a web app based on Flask and Sqlite3 with user account handling.

Uses Python3, Sqlite3, Flask, jsonschema, Bootstrap, jQuery, DataTables.

Installation
Create your own GitHub repo out of this repo.
Clone your repo to your own work computer, as usual.
Set up your Python3 environment, e.g. using virtualenv.
Install the required Python3 third-party packages (Flask, etc) using `pip install -r requirements.txt'.
Create your JSON file settings.json in either the directory {your-repo-dir}/site or 
    {your-repo-dir}/webapp by making a copy of {your-repo-dir}/webapp/example_settings.json 
Edit it to fit your site. If your email server is not the simple localhost with no password, then you need to set those variables. 
See the file {your-repo-dir}/webapp/__init__.py for all email-related settings variables.
Set up the SQLITE3 database that your app will use, and add the name of it, any required username and password for it, in your settings.json file.
Include the directory {your-repo-dir} in the Python path. This can be done in different ways. The simplest is to set it in the shell (e.g. in your .bashrc file):

$ cd {your-repo-dir}
$ export PYTHONPATH=$PWD:$PYTHONPATH

Use the command-line interface to create an admin user account. This will also automatically load the index definitions to the CouchDB server.
$ python cli.py -A

Run the Flask app in development mode as usual python app.py.

If you wish to run the Flask app in production mode, see the Flask manual or the Apache, nginx, or whichever outward-facing web server you are using for information.

    
