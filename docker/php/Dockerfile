FROM php:7.4-fpm-alpine
WORKDIR /var/www/html
# Install extension
RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable mysqli
# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer