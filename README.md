# Project: Linux Server Configuration 
- This project is for Udacity's Full Stack Web Developer Nanodegree.
- It sets up the item catalog app project on amazon lightsail virtual server

## Server Info
1. IP address:54.146.148.42, port 2200
2. URL http://54.146.148.42.xip.io

## Configuration 
1. Change ssh port 22 to 2200 by editing sshd_config file (`sudo nano /etc/ssh/sshd_config`)
2. In the same file, disable root remote login and password authentication by setting the parameter to "no"
3. Configure uncomplicated firewall (UFW) to only allow connection on port 80, 2200, and 123, and activate UFW
4. Change the timezone to UTC
5. Create user named 'grader' and grant it sudo access
6. Configure and Enable a New Virtual Host by creating a catalog.conf file 
7. Create the .wsgi file 

## Installation
1. Apache2 (`sudo apt-get install apache2`)
2. Mod_wsgi ('sudo apt-get install libapache2-mod-wsgi')
3. Postgreaql (`sudo apt-get install postgresql`)
   - create a user named 'catalog' with password 'catalog'
   - create an empty database called 'catalog', which will serve the data from the item catalog project

## Dependencies

1. Flask
2. httplib2, oauth2client, sqlalchemy psycopg2

## Usage:

After ssh in the server:

`cd /var/www/catalog/catalog`
`sudo python database_setup.py` (to set up the database)
`sudo python CityAttraction.py` (to populate the database with initial data)
`sudo python application.py`  (to run the server)


## Third Party Resource

- Ssh key configuration (https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server)
- Deploy a flask app on Ubuntu (https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps#step-four-–-configure-and-enable-a-new-virtual-host)

## Author

[Jingyi Mo](mailto:jingyim62015@gmail.com)

