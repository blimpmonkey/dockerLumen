FROM php:7.1-fpm-alpine

RUN	apk update && apk add \
    curl

# Install extentsions
RUN docker-php-ext-install \
    mbstring \
    pdo \
    pdo_mysql

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer