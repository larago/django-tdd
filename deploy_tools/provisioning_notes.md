Deploy a new webapp
====================

## Following packages need to be installed

* nginx
* Python
* Git
* pip
* virtualenve

Examples in linux 14.04, you can execute following order to install:

    sudo apt-get install nginx git  python3 python3-pip
    sudo pip3 install virtualenv

## Configure Nginx 

* Refer to nginx.template.conf
* Please set SITENAME as your own sitename, such as my-domain.com

## Upstart Mission

* Refer to gunicorn-upstart.template.conf
* Please set SITENAME as your own sitename, such as my-domain.com

## Construct of files

If you have an account already, then catalog should be like /home/username

/home/username
 |__sites
     |__SITENAME
         |__database
         |__source
         |__static
         |__virtualenv
