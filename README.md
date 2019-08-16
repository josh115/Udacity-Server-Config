# Udacity-Server-Config

## Server Information
- IP Address: 3.9.135.49
- SSH Port: 2200
- URL: http://ec2-3-9-135-49.eu-west-2.compute.amazonaws.com/
- Password For grader User: grader

## Software
  Amazon Lightsail
 
  - Apache2 `sudo apt-get install apache2`
  - mod_wsgi `sudo apt-get install libapache2-mod-wsgi-py3`
  - Git `sudo apt-get install git`
  - Pip3 `sudo apt-get install python3-pip`
  - Flask `sudo pip3 install Flask`
  - Libaries `sudo pip3 install httplib2 oauth2client sqlalchemy requests`
  - Psycopg2 `sudo apt-get build-dep python3-psycopg2` then `sudo pip3 install psycopg2`
  - Virtualenv `sudo pip3 install virtualenv`
  - PostgreSQL `sudo apt-get install postgresql`
  
## Configuration
  - Updated all currently installed packages.
  - Changed the ssh port from 22 to 2200.
  - Added Uncomplicated Firewall (UFW) to only allow connection from ports 2200, 80 and 123.
  - Added user grader with sudo permission.
  - Changed timezone to UTC
  - Disable login for root user
  - Configured Apache for mod_wsgi
  - Configure PostgreSQL database with user catalog and database catalog with remote connections disabled
  - Cloned item catalog project so that is functions as it should
  
## Third Party Resources
  - Apache with Flask help `http://www.islandtechph.com/2017/10/23/how-to-deploy-a-flask-python-3-5-application-on-a-live-ubuntu-16-04-linux-server-running-apache2/`
  - PostgreSQL help `https://medium.com/coding-blocks/creating-user-database-and-adding-access-on-postgresql-8bfcd2f4a91e`
  - SqlAlchemy and PostgreSQL conncetion `https://docs.sqlalchemy.org/en/13/core/engines.html`
