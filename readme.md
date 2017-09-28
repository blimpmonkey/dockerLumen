## Getting started
1. docker-compose up --build -d
2. shell into php container
3. use composer to create a new Laravel/ Lumen project

## Docker commands

#### Build 
```
$ docker-compose up --build -d
```

#### List running containers
```
$ docker-compose ps
```

#### Destroy containers
```
$ docker-compose down
```

#### Removing all running containers
```
$ docker rm $(docker ps -a -q)
```

#### Removing all images
```
$ docker rmi $(docker images -q)
```

## Laravel/ Lumen commands

#### Running shell in the php container
```
$ docker-compose exec php sh
```

#### Setup new project
```
# composer create-project laravel/lumen .
# composer create-project laravel/laravel .
```

#### php artisan
```
# php artisan
```

#### composer
```
# composer -v
```

#### phpunit
```
# vendor/bin/phpunit
```

##### References
* https://serversforhackers.com/s/docker-in-development
    * https://github.com/retroconduct/docker-lumen
    * https://github.com/shipping-docker/php-app

###### Possible values for docker-php-ext-install:
bcmath bz2 calendar ctype curl dba dom enchant exif fileinfo filter ftp gd gettext gmp hash iconv imap interbase intl json ldap mbstring mcrypt mssql mysql mysqli oci8 odbc opcache pcntl pdo pdo_dblib pdo_firebird pdo_mysql pdo_oci pdo_odbc pdo_pgsql pdo_sqlite pgsql phar posix pspell readline recode reflection session shmop simplexml snmp soap sockets spl standard sybase_ct sysvmsg sysvsem sysvshm tidy tokenizer wddx xml xmlreader xmlrpc xmlwriter xsl zip