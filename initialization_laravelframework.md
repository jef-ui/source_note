#####Setting Up Laravel _ Ubuntu Linux Operationg System

- Install xampp, composer, nodejs and php

###### sudo composer create-project laravel/laravel myapp
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

  - path you project and type code .

  ## Setting up your .env , copy env.example and rename it to .env 

    ### Config .env file

   -DB_CONNECTION=mysql //change mysql from sqlite
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE= <createddbname> // change what db name in php my admin
    DB_USERNAME=<your username> 
    DB_PASSWORD= <your password>

    ### config/database.php

    -'mysql' => [
    'driver' => 'mysql',
    'url' => env('DB_URL'),
    'host' => env('DB_HOST', '127.0.0.1'),
    'port' => env('DB_PORT', '3306'),
    'database' => env('DB_DATABASE', '<createddbname>'), 
    'username' => env('DB_USERNAME', '<your username if not default is root>'),
    'password' => env('<your password>', ''),
    'unix_socket' => env('DB_SOCKET', ''),
    'charset' => env('DB_CHARSET', 'utf8mb4'),
    'collation' => env('DB_COLLATION', 'utf8mb4_general_ci'),<<< change general from unicode >>>
    'prefix' => '',
    'prefix_indexes' => true,
    'strict' => true,
    'engine' => null,
    'options' => extension_loaded('pdo_mysql') ? array_filter([
    PDO::MYSQL_ATTR_SSL_CA => env('MYSQL_ATTR_SSL_CA'),
    ]) : [],
    ],

 ## php artisan migrate

 ## php artisan key:generate

 ## php artisan serve 

 ## php artisan serve --host=ip address --port=portnumber










