# Linux_Server_Configuration

## Description
   This is the final project for Udacity's Full Stack Web Developer Nanodegree.This is about linux server configuration
   
### Server Details:

Server IP Address: 13.127.101.42

Hosted site Url : http://13.127.101.42.xip.io/


### How to connect as grader:

  save the private key provided in your local machine and run the following command
  ```
  ssh -i path/to/privatekey -p 2200 grader@13.127.101.42
    
  ```
  and the password for grader : srinu1211
  
### Id_rsa key:
```
-----BEGIN RSA PRIVATE KEY-----
MIIEpAIBAAKCAQEA6cy+KZblQRW3hq6JdBCsl+iXIju5zpwXJNAcQSx7EF1EchW2
WDUVkgUvq21sJ8mktsdsEi8uYUTy9TBQmXG3EFkeuqZ3WnPT2gDDlVYmc6tztUBR
JGXv4vTqqyMSA+UcPImnRVi4ilpW1s1aL9yyVmcNsx91DdvcuiJ6S9uY1YJsYny/
tSIW4X2Ea/7ZntxszfgyDxRO7A8DNiJIkhat5vtzBdepip+PGxSVRJD98Vl8Tpg1
uwhGIMiEj054Ztiz1tVrJGdAREqNrvss9csavO65uU+WQN5Jm8Fn9DZzv0L7DU+P
ybHIe7EPq/5QtwYL7kThPWg8YCffPuSPFSV2xQIDAQABAoIBACJu2QLfClyPijv3
sJ67Ze/pfXi5OyBGtNHjJIYkuusqEU6MDBLpnoem4+JndypU9EFHFY+IC1igAvhB
aV1v9foeZfwvUByuOmE9A5EW4wreEWh8VHb73FycnYMe4yRXtdTkoRIBgww9SdTQ
4Zty8YDwJIBg/ahQ3S08rq5FZTjseE8KsVl6M1gjRWpTILPY6o7gixnyolDyIdQx
btqstsss3bU5LaWm0rh/YYEpitGx8EfIqv1TTrm4kks52YSA2WBM+c8lk/a8V44p
X8NAMaxmRe9mtNTEDmZclKcWwWNnLshzM+RUPwC+cDCEp8gst5maT+OI4N+vmB96
i7BpcYECgYEA//v4ah15hZc/DPE9nJgIm0Plo0iASYOSZZQ1Z331LvTFeuqNtyi2
eLoPlnyHHxa5UOZ+UkKsNCBkUs20sxcs2eiKoHVbEUMPh9hYFLL0/WBExwtQuoXU
Pr6yRlebYLZjK5oL2xVXn6qjgo3wY4YKi20XwjmdjhbAHUD5eiGKo8kCgYEA6dBs
WOBzE0v6a6k1b1dqFkrdkLmx7pwJHTMUKJTwH8jYDef4STJealDWeU2iOBj813Ez
K8WjyYNvA+4Mpg7JS4ZdnsIpEHEmRit8bR48XOU0p4Wp31oML7gqh3gFDDABztLM
+tf+1PpI1PgoOrj6qMINyNGyKagiD3avsUC0IR0CgYEA8QxDiyFAOpUG0VglrVzY
1eRkzJJMA227IJ4kf9TzWYkyoKFYW34h/aMvZITU9GiAjvbNQwb3g4pxDiwYmYAc
QwIf8CMyYxnj+Qa3Qp6V5jaN7WTxWwMEryUBWQ3MCZEV54wC2AXL4lVb7WddU0p4
iXxsIAADJja0J5f0lJYbKEkCgYAtvp9UDCW3gsftxF81925ECkWrCQms205VLicl
gW4xacQLhHTpLTeXqVUsymmQfCMLq5QNXk+bH2Ha7PoAiygK5LDwXKBYHSsV03A2
kRHSQu24UMhZcG6t72QyuOKT7diMtGVyNkwfMxCIyjxksMgpuD2mKpCm4cQ4LkpV
bYlQaQKBgQDXvH3yE0UBoZp/YNByFW/qFGNxMdMUAuEjxVO2FKxb523e1XM7cNv2
Ugh+CgS2H59MShDrQs4asDjD4M5d+ULxC17V7CygajySFUucKH2yVaZ72ubqrgMS
Akc7hfZYp7BYzea+S3B+PXZAM3sR8a6FOVyFaZ+/JXK5roFDwOvEeA==
-----END RSA PRIVATE KEY-----



```
### Id_rsa.pub key:
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDpzL4pluVBFbeGrol0EKyX6JciO7nOnBck0BxBLHsQXURyFbZYNRWSBS+rbWwnyaS2x2wSLy5hRPL1MFCZcbcQWR66pndac9PaAMOVViZzq3O1QFEkZe/i9OqrIxID5Rw8iadFWLiKWlbWzVov3LJWZw2zH3UN29y6InpL25jVgmxifL+1IhbhfYRr/tme3GzN+DIPFE7sDwM2IkiSFq3m+3MF16mKn48bFJVEkP3xWXxOmDW7CEYgyISPTnhm2LPW1WskZ0BESo2u+yz1yxq87rm5T5ZA3kmbwWf0NnO/QvsNT4/Jsch7sQ+r/lC3BgvuROE9aDxgJ98+5I8VJXbF lenovo@srinivas

## passpharse key
    there is no passpharse key
    press enter button when it asks

## Configuring Linux Server

### Updating all packages:
```
sudo apt-get update
sudo apt-get upgrade
```

### Creating grader User:
  create new user by following command:
  ```
  sudo adduser grader
  ```
  Then type this command to give permissions:
  ```
  sudo nano /etc/sudoers
  ```
  Below the Root user append the following line:
  ```
  grader  ALL=(ALL:ALL) ALL
  ```
  This will grant sudo permission to grader.

  ### Creating a ssh key pair for grader:

   On your local machine in terminal/command prompt type:
   ```
   ssh-keygen
   ```
   It will generate the ssh keys which is saved to .ssh folder
   
   Then in your virtual machine connect to newly created user:

   ```
   su - grader
   ```
   Create a new directory .ssh and new file authorized_keys in that directory:
   ```
   mkdir .ssh

   sudo nano .ssh/authorized_keys
   ```
   Copy the public key with .pub extension to authorized_keys and save the file:

   ```
   chmod 700 .ssh
   chmod 644 .ssh/authorized_keys
   ```
   - 644 prevent other user from writting in to file.
   - 700 will give read write and execute permission to user.
   
   Then restart ssh server:

   ```
   service ssh restart
   ```
   
   Log in to grader with private key generated in local terminal:

   ```
   ssh -i .ssh/id_rsa grader@ipaddress 
   ```
  ### Changing the ssh port to 2200:
   Type below command to change port 
   ```
   sudo nano /etc/ssh/sshd_config
   ```
   it will open up file change port to 2200
    
   Restart the ssh server:
   
   ```
   service ssh restart
   ```
   
   >Before Logging using ssh add custom TCP port 2200 under lightsaail firewall in networking tab in lightsail instance console:  
   
   Now Login using command in local terminal:
   ```
   ssh -i .ssh/id_rsa -p 2200 grader@youripaddress
   ```
   
  ### Disabling ssh login as root:
  follow this commands:

  `sudo nano /etc/ssh/sshd_config`
  
  make change `PermitRootLogin no`
  
  ### Configurating  Ufw firewall:
  follow this commands:
  ```
  sudo ufw status
  sudo ufw allow 2200/tcp
  sudo ufw allow 80/tcp
  sudo ufw allow 123/udp
  sudo ufw enable
  ```
  This will allow all required ports and enables the ufw
  ```
  sudo ufw status
  ```
  It will display all allowed ports
  
  ## Changing time Zone:

  `sudo dpkg-reconfigure tzdata`
  
  select none from list and then select utc.
  
  ### Installing Apache2 :

  In terminal type:
  
  ```sudo apt-get install apache2```
  
  Now mod_wsgi:
  
  ```sudo apt-get install python-setuptools libapache2-mod-wsgi```
  
  Enable mod_wsgi by:
  
  ```sudo a2enmod wsgi ```

  ## Setting up your flask application to work with apache2:

   Deploying flask app with apache2 is referred from [Digital ocean](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)

   Creating a flask app
   
   In the /var/www/ directory create new floder FlaskApp

   `sudo mkdir FlaskApp`
   
   Install git using sudo
   
   `sudo apt-get install git`
   
   move to the FlaskApp `cd FlaskApp`
   
   In that direcory clone your github repository
   
   `sudo git clone https://github.com/username/catalog.git`
   
   Rename your repository to FlaskApp
   
   Then rename in main project file to `__init__.py`
   
   >Error : While accesssing the client_secrets.json file 
   ```
   PROJECT_ROOT = os.path.realpath(os.path.dirname(__file__))
   json_url = os.path.join(PROJECT_ROOT, 'client_secrets.json')
   ```
   Use json_url instead client_secrets.json in script
   
  ## Install and configuring postgresql for project

   Install Postgres using command:
   
   `sudo apt-get install postgresql`
   
   login to postgres: `sudo su - postgres`
   
   then type below to enter into shell:
   
    `psql`
   
   create user:
   
    `CREATE USER catalog WITH PASSWORD 'password';`
   
   permit user to createdb: 
   `ALTER USER catalog CREATEDB;`
   
   Create a database name catalog with user catalog ::`CREATE DATABASE catalog WITH OWNER catalog;`
   
   connect to db using following command:
   `\c catalog`
   
   revoke all permission to public: 
   `REVOKE ALL ON SCHEMA public FROM public;`
   
   Give schema permission to user catalog:
    `GRANT ALL ON SCHEMA public TO catalog;`
   
   exit from db and postgres `\q and exit`
   
   Change the database connection in both db_setup.py and `__init__.py` as `engine =create_engine('postgresql://catalog:password@localhost/catalog')`
   
  ## Configure and Enable a New Virtual Host:
   Type this command to config:

   `sudo nano /etc/apache2/sites-available/FlaskApp.conf`
   
   In this add the following code

   ```
   <VirtualHost *:80>
		ServerName mywebsite.com
		ServerAdmin admin@mywebsite.com
		WSGIScriptAlias / /var/www/FlaskApp/flaskapp.wsgi
		<Directory /var/www/FlaskApp/FlaskApp/>
			Order allow,deny
			Allow from all
		</Directory>
		Alias /static /var/www/FlaskApp/FlaskApp/static
		<Directory /var/www/FlaskApp/FlaskApp/static/>
			Order allow,deny
			Allow from all
		</Directory>
		ErrorLog ${APACHE_LOG_DIR}/error.log
		LogLevel warn
		CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
   ```
   Enable the virtual host by:

   `sudo a2ensite FlaskApp`
   
   Disabling the default apache2 page:

   `sudo a2dissite 000-default.conf`
   
  #### Create the .wsgi File
    first move to following directory and run command to create file:
    ```
    cd /var/www/FlaskApp
    sudo nano flaskapp.wsgi 
    ```
   Add the following code in the file:
   
   ```
   #!/usr/bin/python
    import sys
    import logging
    logging.basicConfig(stream=sys.stderr)
    sys.path.insert(0,"/var/www/FlaskApp/")

    from FlaskApp import app as application
    application.secret_key = 'Add your secret key'
   ```
   save and exit the file
   
   
   ## Installing require modules

   You can either install all modules on your machine or create a virtual environment for the project and install the modules

   ` pip install flask sqlalchemy requests oauth2client psycopg2`
   
   ## Setting up your Google Oauth2:

   Login to your  google developer console and select your project and edit OAuth details as following
   
   Javascript origin:

   `http://ip.xip.io`(ip=your ip adress)
   
   redirect URI:
   ```
   http://ip.xip.io/login
   
   http://ip.xip.io/gconnect
   
   http://ip.xip.io/callback
   ```
   [xip.io](xip.io) is a free DNS which will be the same as using IP address.
   
   ##Finally

   Restart your apache2 server using command below:
   
   `sudo service apache2 restart`
   
