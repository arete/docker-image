FROM arete74/voidlinux

RUN useradd -d /var/www/html -r -s /bin/false -U http
RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Syu nginx php-fpm php-pgsql runit

#COPY nginx.php-fpm.conf  /etc/nginx/nginx.conf
#COPY nginx.vh.default.conf /etc/nginx/conf.d/default.conf

#enable nginx and php-fpm

RUN  mkdir -p /etc/runit/runsvdir/default/ && ln -s /etc/sv/nginx /etc/runit/runsvdir/default/ && ln -s /etc/sv/php-fpm /etc/runit/runsvdir/default/
EXPOSE 80 443

ADD entrypoint /sbin
ENTRYPOINT ["/sbin/entrypoint"]
CMD ["/usr/sbin/runsvdir","-P","/var/service"]



