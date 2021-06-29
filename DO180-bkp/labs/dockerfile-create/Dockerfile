FROM ubi7/ubi:7.7
MAINTAINER Dell Padron <dellpadron@gmail.com>
LABEL desctiption="A custom Apache container baserd on UBI 7"
RUN yum install -y httpd && \
    yum clean all
RUN echo "Hello from Dockerfile" > /var/www/html/index.html
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]
