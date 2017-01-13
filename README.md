# Docker-Symfony kickstarter

This template use docker and docker-compose to initialize a ready to use developper environment with shared files to 
customize httpd and php configuration.

docker-compose.yml define : 
 - httpd 2.4 (based on Centos7) with a prepared configuration to work with php-fpm
 - php-fpm server (also based on Centos7) 
 - postgresql database
 - and a mailcatcher 
 
##### Usage
Database configuration and Symfony environment are store in the `.env` file.
The example files `app.php` and `parameters.yml` replace both `app.php` and `app_dev.php` by using `SYMFONY_ENV` and 
`SYMFONY_DEBUG` environment variables (like native bin|app/console).