FROM php:8.2-apache

# Enable Apache mod_rewrite
RUN a2enmod rewrite

# Install mysqli
RUN docker-php-ext-install mysqli

# Copy backend files into container
COPY . /var/www/html/

# Apache config
WORKDIR /var/www/html
