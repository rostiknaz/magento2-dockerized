# Magento2 Dockerized
This project provides a setup of docker environment for Magento 2.

### File structure:
```
./build/ - Magento code pool.
./bin/docker - shell script for managing app inside the docker container (for more details run `bin/docker usage` command)
./docker/app/ini/ - php ini files.
./docker/app/Dockerfile - php:7.2-fpm image template.
./docker/app/php-fpm.conf - php-fpm custom configuration.
./docker/db/conf.d/ - mount custom MySQL configuration file into /etc/mysql/.
./docker/db/init.d/ - here we can put files with extensions .sh, .sql and .sql.gz . This files will be imported by default to the database specified by the MYSQL_DATABASE variable when container is started for the first time.
./docker/var/log/ - contains php-fpm and nginx logs.
./docker/web/ssl/ - stores generated ssl certificates.
./docker/web/magento2.template - nginx server configuration template for Magento2.
./docker/.env - environment variables.
```

### Installation process:

