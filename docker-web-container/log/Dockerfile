FROM debian:latest

MAINTAINER 0.1 eiurur

RUN apt-get update
RUN apt-get upgrade -y

# ボリュームの作成
RUN ["mkdir", "/var/log/httpd"]
VOLUME /var/log/httpd
