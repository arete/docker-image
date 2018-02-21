FROM arete74/voidlinux

RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Syu nginx


EXPOSE 80

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]



