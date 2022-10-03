FROM httpd:2.4
COPY ./mod_dispatcher.so /usr/local/apache2/modules
COPY ./httpd.conf /usr/local/apache2/conf
RUN ln -sf /dev/stdout /usr/local/apache2/logs/dispatcher.log