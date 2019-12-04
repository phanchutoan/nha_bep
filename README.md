1. docker-compose up -d

2. ssh into app container

3. insall composer 
    php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
    php composer-setup.php && \
    php -r "unlink('composer-setup.php');" && \
    php composer.phar install
4. Install app 
    php artisan igniter:install

    DB infor:
        - MYSQL_DATABASE=tastyigniter
        - MYSQL_USER=tastyigniter
        - MYSQL_PASSWORD=somepassword