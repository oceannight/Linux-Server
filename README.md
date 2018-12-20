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


## Third Party Resource

- Ssh key configuration (https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server)
- Deploy a flask app on Ubuntu (https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps#step-four-–-configure-and-enable-a-new-virtual-host)

## Author

[Jingyi Mo](mailto:jingyim62015@gmail.com)

## Notes to Reviewer
- Grader password: grader
- ssh key: MIIEowIBAAKCAQEAvtmlqMjEV39swexRGkulOKVRWR0LoF4w4FsRs3Akge00rO1h
T+Zzj1jYNnEpADNFn1Bf1JrECgC39kvKzYBkl0WjYkCBUa1LrkWOsXqbc3APZEzT
WPgWFVeHGQWBqKmOHgDOtfkey9LQUsBfVlJpasG2QvYWZlbIg2uHwLYO+OHakUSc
AwJVHYaAJOztIJtQLJsTGhJ6VtWeb43AfnueG94mSr4PCk0CtSaqEa9K2S/0xDlS
V/3i/ear9Q/+FaejKgWpcl4pmwh+DVHRiQsPgeDWGZR+Hev4p39A8Mz+aGpOWAqU
LPnzCBcpKQhbTISsm1F/WOdGze0hB5SQiLrNvQIDAQABAoIBAHCZZJ2iZgThjz8S
t/71pnM3Rjl3Y4aoS9nyoQznGwL0+mEUZJeJdaCbYGUuemw909Pczc1XylXEesT7
jpmUKMT/Nxgeyq1vuvkE3N1lYxXGha49jWwuYokQ7QocL5VdBBY7j7nZUwwaQwKv
sQ/y63Mq+uei3TBf/0laReuy/j5jq30+b7ivolPcslOmPbkb7EYXhzHr0KpO7qY3
E0N7QVwx1e+hQYGUPhhNlsHn7NyfBj9e1J2lLE+BBjORifw6WvfoZFvMFtF1fWas
l8hmRhr3hLmyn/8FwmzSadvtO8LRX/esc2/aX7KzHdf6cbyp3PjGvtLwPjQ/0jlX
c3r17ZkCgYEA+nqN7vG/O0LhlGsc3F1gTrElZcjLBp3AbHT8WBh4nwujklVtDbB4
B2aY/M6SRp6JkCNVWJi/9l3ZrkkY+LGm4vX3vKUIRNJ7/PMX5yRDJ3f3+vDKKyBC
XqXKCJCoikiIJgnO+K5DKBpr7ylUCWLWklptqAaXGfkt3d5EYvBDQgsCgYEAww6c
NoIEx36fG0LLHgWSwxMQbFTSOF+PF1Q98ww0JMQRg86acu6QOFw77ek5jA7SLWUm
hyoM0yFwW530/3/p+wVUORKPR1tep/qNZqITbuVx17H6SY1LvEkMUaouptbtij8w
BuHlGgAK9bRiWzbeOZeVrbSLrOMqxJBcjbazlFcCgYAERd7x+pHGkweCHqmpYLZp
4T/AEsLT5BEKSJydbB1yqSIrNuXbW+1QQwHNHkEEj2PNX6zvC/wKWeOCw6B3baBp
MsT9JNuVQPn4gLUhrk6u9671SvJH9g7rymw95Sna4g3giD5No7tljb3VoKDcYCFE
8eH5AdPGD6gmpsoH3g1nrQKBgHO+srGhm4Zpu64oh3EMK5d4M5GlD42GHtngElas
EjES67XEHmA+8fOPv7wgXhafINbxI9im+i86s3qaE6ydUdGzytOHEOBt9pBFHC0f
1dpDardslDGbF6rlydqX2tEDzrbvYedjmlhAWECOxqKLv3h7W8VU0mFH97PmWhV5
qbxHAoGBAL7YZTUJxb1BFoRfCdFXY5DqJelrUFwC79fJ2f55DzdV57Wz3aFX5QVV
xMQsob53k2HOLytP6qkFnQmpkgvFRtO3x0DUxsdfZR8/aN55HGnzGB1n/wpbXsuw
iM0uRzSwPNxcGw84R2sD6zqe3UrkgbULJW1Q90UFxlFD2l2Jef2R
