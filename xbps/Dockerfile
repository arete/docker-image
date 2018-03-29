FROM arete74/voidlinux

RUN  /usr/bin/xbps-install -Syu &&  /usr/bin/xbps-install -Sy  git xtools gawk util-linux && rm -rf /var/cache/xpbs/
RUN mkdir /repo

WORKDIR /repo
VOLUME /repo
COPY ./entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
