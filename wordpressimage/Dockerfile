# Use the official WordPress image as the base
FROM wordpress:latest

# Replace the Apache default port from 80 to 8080
RUN sed -i 's/Listen 80/Listen 8080/' /etc/apache2/ports.conf \
    && sed -i 's/<VirtualHost *:80>/<VirtualHost *:8080>/' /etc/apache2/sites-available/000-default.conf

# Expose the new port
EXPOSE 8080
