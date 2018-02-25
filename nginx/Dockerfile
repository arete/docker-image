FROM arete74/voidlinux

RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Syu nginx

COPY nginx.conf /etc/nginx/nginx.conf
COPY nginx.vh.default.conf /etc/nginx/conf.d/default.conf



EXPOSE 80

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]



