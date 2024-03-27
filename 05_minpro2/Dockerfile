FROM centos:7

RUN yum -y install httpd php && yum clean all

VOLUME ["/var/www/html", "/var/log/httpd"]
ADD src.tar /var/www/html

EXPOSE 80/tcp

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]