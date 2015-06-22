# catalog_app
udacity full stack nanodegree project 3 completed by Xiang Zhao Mirko
05/23/2015

GENERAL DESCRIPTION
-------------------
This is a project including sql schema in a virtual box instance using vagrant. This is a web app where registered users are able to create and modify jewelry collections. Not logged in users are also able to browse existing collections.

MODULES
-------------------
project.py: main python file which will create a Flask app and run it locally on localhost:5000
database_setup.py: includes database settings and schema, running this file will cerate a sqlite:///ecommerce.db 
lotsofitems.py: running this script will create some sample collections and users to populate the database
emptyDatabase.py: this is a helper script to delete all instances in the database without dropping it
client_secrets.json: you need to create your own google oauth credentials from https://console.developers.google.com/ after registering and creating an app, go under credentials on the left column and click 'dowload JSON'    
fb_client_secrets.json: register your app at https://developers.facebook.com/ and obtain the app id and client secret to be replaced accordign to this json file format
static folder: includes all css files, fonts files, and media files necessary to recreate the web page
templates folder: includes all html template files used by flask to render teh different pages



python libraries and frameworks used: 
psycopg2
requests
httplib2
Flask-Login
Flask
gunicorn
Jinja2
oauth
oauth2client
SQLAlchemy
Werkzeug

INSTALLATION
-------------------
Install Git, Vagrant, and Virtual Box  
-Git: If you do not have a version of git installed, please visit http://git-scm.com/downloads  
-Vagrant: in order to install Vagrant, plese visit https://www.vagrantup.com/downloads  
-VirtualBox: in order to install Virtual Box, please visit https://www.virtualbox.org/wiki/Downloads  

CONFIGURATION
-------------------
-git clone https://github.com/xiangormirko/tournament_project_2.git  
-using terminal navigate to the fouder in '/vagrant'  
-type 'vagrant up'  
-after the inizial setting up, type 'vagrant ssh' to log into the instance  
-navigate to 'cd /vagrant' to access the share files  

DATABASE & TABLES
-------------------
-After you are logged into vagrant type psql  
-Here type the commands to create the database tournament ('CREATE DATABASE tournament;')  
-You may check the the databases with the command '/d'  
-Connect to the database using the command ('\c tournament')  
-Import using command '/i tournament.sql' or paste sql schema to create tables and views from tournament.sql  
-Run 'python test_tournament.py' to check if the script passes all unit tests  
-Use and edit methods in tournament.py as needed  
-Thanks!  



