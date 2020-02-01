FROM php:7.3-fpm

RUN apt-get update && apt-get install -y \
        git \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
    && docker-php-ext-install -j$(nproc) iconv mbstring mysqli pdo_mysql

 RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

 ADD php.ini /usr/local/etc/php/conf.d/40-custom.ini

 WORKDIR /var/www/decker-test/

 CMD ["php-fpm"]