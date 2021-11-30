FROM 'phpdockerio/php:8.0-fpm'
#php:8-alpine3.14

WORKDIR "/application"

#TODO : install with apk to alpine image version
RUN apt-get update; \
    apt-get -y --no-install-recommends install \
        php8.0-bcmath \ 
        php8.0-gd \ 
        php8.0-http \ 
        php8.0-intl \ 
        php8.0-mcrypt \ 
        php8.0-mongodb \ 
        php8.0-mysql \ 
        php8.0-pgsql \ 
        php8.0-redis \ 
        php8.0-soap \ 
        php8.0-solr \ 
        php8.0-uuid \ 
        php8.0-xdebug; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

RUN apt-get update; \ 
    apt-get -y --no-install-recommends install \
    nodejs \  
    npm