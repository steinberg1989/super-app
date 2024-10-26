FROM php:8.0-apache

# Enable necessary modules
RUN a2enmod rewrite
RUN a2enmod mpm_prefork

# Copy your application files
COPY ./src /var/www/html/  # Ensure this path is correct
COPY ./apache2.conf /etc/apache2/apache2.conf  # Ensure this path is correct

# Set permissions (adjust as necessary)
RUN chown -R www-data:www-data /var/www/html
RUN chmod -R 755 /var/www/html
