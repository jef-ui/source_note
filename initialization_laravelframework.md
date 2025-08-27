# Setting Up Laravel _ Ubuntu Linux Operationg System

- Install xampp, composer, nodejs and php

## sudo composer create-project laravel/laravel myapp
 - track your path first opt/lampp/htdocs/ + command

## sudo chown -R <username>:<username> /opt/lampp/htdocs/<projectname>/

 - sudo chown -R web-dev-eirfej:web-dev-eirfej /opt/lampp/htdocs/myapp/

 ## chmod 775 storage bootstrap/cache/

 ## sudo nano /opt/lampp/etc/extra/httpd-vhosts.conf

 ## sudo nano /etc/hosts

 - add 127.0.0.1 <projectname.test>

 ## sudo /opt/lampp/lampp restart

 ## sudo apt install php8.3-mysql

 - optional if you dont install php yet.

 ## sudo nano /opt/lampp/etc/extra/httpd-vhosts.conf 

 ## sudo nano /opt/lampp/etc/php.ini

  - remove semi colon or enable
    extension=php_pdo_mysql.dll
    extension=php_pdo_sqlite.dll 
    extension=php_sqlite3.dll 
  - search = ctrl + w

  ## sudo /opt/lampp/lampp restart

  - path





