FROM debian:latest

MAINTAINER 0.1 eiurur

RUN apt-get update
RUN apt-get upgrade -y

RUN ["apt-get", "-y", "install", "apache2"]

CMD ["/etc/init.d/apache2", "restart"]
