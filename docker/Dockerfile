#
#
FROM registry.access.redhat.com/rhel7

RUN yum -y install tar httpd mod_ssl ksh && yum -y clean all

COPY html /var/www/html
COPY cgi-bin /var/www/cgi-bin

EXPOSE 80

ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D", "FOREGROUND"]
##
##
