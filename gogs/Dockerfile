FROM picymru/base:latest
MAINTAINER Matthew Gall <matthew@picymru.org.uk>

ENV GOGS_VERSION 0.9.97
ENV GOGS_BINARY gogs_v${GOGS_VERSION}_linux_amd64

ADD https://dl.gogs.io/${GOGS_BINARY}.tar.gz /tmp/${GOGS_BINARY}.tgz
RUN tar xzf /tmp/${GOGS_BINARY}.tgz -C /tmp && \
	mkdir /app && \
	mv /tmp/gogs/* /app && \ 
	rm /tmp/${GOGS_BINARY}.tgz

WORKDIR /app

EXPOSE 3000

ENTRYPOINT ["/sbin/tini"]
CMD ["/app/gogs", "web"]