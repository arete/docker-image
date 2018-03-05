FROM arete74/voidlinux
RUN useradd -d /var/www/html -r -s /bin/false -U http
RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Syu php-fpm php-pgsql



EXPOSE 9000



