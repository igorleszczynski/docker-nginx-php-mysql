FROM php:7.4-fpm
RUN apt-get -y update
RUN apt-get install -y \
        zlib1g-dev \
        libpng-dev \
        libzip-dev \
        libxml2-dev
RUN docker-php-ext-install mysqli pdo pdo_mysql gd zip bcmath soap
RUN pecl install xdebug
RUN curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php
RUN php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer


