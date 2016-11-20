FROM centos:latest

MAINTAINER 0.1 eiurur

RUN ["yum", "-y", "install", "httpd"]

# RUN ["rpm", "-Uvh", "http://nginx.org/packges/centos/7/noarch/RPMS/nginx-release-centos-7-0.e17.ngx.noarch.rpm"]
# RUN ["yum" , "install", "-y", "nginx"]

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]