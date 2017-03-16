FROM phpdockerio/php56-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php5-mysql \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

COPY src/ /var/www/src/

WORKDIR "/var/www/src"