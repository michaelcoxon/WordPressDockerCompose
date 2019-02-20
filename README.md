# WordPress Docker Compose
A Docker Compose file for standing up development instances of WordPress

## Sources  
 - https://docs.docker.com/compose/wordpress/
 - https://cntnr.io/setting-up-wordpress-with-docker-262571249d50

## Usage
This will create a folder for wp-content and the database
in the folder it is run from. You will be able to access 
phpmyadmin from `localhost:8080` and the site from `localhost:8000`.

Change the ports in the `docker-compose.yml` file for each instance
you want running.

### How to use

> For each running instance change the port numbers for 
> phpmyadmin and WordPress. (this is the first parameter in ports)

run `docker-compose up -d` in the directory this file is in 
to stand the containers up. WordPress takes a bit to work.

run `docker-compose down --volumes` to kill the instances. 
Your files will remain - just delete them after

default root password is `toor` change it in the `docker-compose.yml` 
file if you want
