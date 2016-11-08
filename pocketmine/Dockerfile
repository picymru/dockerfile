FROM ubuntu:16.04
MAINTAINER Matthew Gall <matthew@picymru.org.uk>

WORKDIR /app

RUN apt-get update && \
	apt-get -y install curl python3-yaml && \
	curl -sL https://raw.githubusercontent.com/PocketMine/php-build-scripts/master/installer.sh | bash -s - -r

EXPOSE 19132

CMD ["/app/start.sh", "--no-wizard", "--enable-rcon=on"]