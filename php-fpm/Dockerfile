FROM arete74/voidlinux

RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Syu php-fpm php-pgsql




EXPOSE 

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]



