FROM       alpine:3.4
MAINTAINER Matthew Gall <matthew@picymru.org.uk>

ADD ./apk-install /usr/sbin/apk-install
RUN apk update && apk upgrade && \
	rm -rf /var/cache/apk/*

CMD ["/bin/sh"]