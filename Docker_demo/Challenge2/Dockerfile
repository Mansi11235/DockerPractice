FROM centos:7

# ENTRYPOINT [ "ping", "www.google.com" ]

# RUN yum makecache

RUN yum -y install httpd

ADD webserver.tar.gz /var/www/html

CMD [ "-D", "FOREGROUND" ]

ENTRYPOINT [ "/usr/sbin/httpd" ]

EXPOSE 80