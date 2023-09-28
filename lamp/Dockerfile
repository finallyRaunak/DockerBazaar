FROM php:8.1-apache

# Update package manager and install required packages
RUN apt-get update \
    && apt-get install -y libcurl4-openssl-dev \
    && apt-get install -y libzip-dev \
    && docker-php-ext-install mysqli pdo pdo_mysql curl zip

# Enable Apache mod_rewrite
# RUN sed -i 's/#LoadModule rewrite_module/LoadModule rewrite_module/' /etc/apache2/httpd.conf
RUN a2enmod rewrite

# Set the working directory
WORKDIR /var/www/html

# Change ownership and permissions of web root
RUN chown -R www-data:www-data /var/www/html \
    && chmod -R 755 /var/www/html

# Add the Virtual Host file to your Docker image
COPY ./wp.local.conf /etc/apache2/sites-available/wp.local.conf
RUN a2ensite wp.local.conf

# Restart Apache
RUN service apache2 restart