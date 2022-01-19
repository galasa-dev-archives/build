ARG dockerRepository

FROM ${dockerRepository}/httpd:2.4

RUN rm -v /usr/local/apache2/htdocs/*

COPY httpd.conf /usr/local/apache2/conf/httpd.conf

RUN mkdir /usr/local/apache2/htdocs/codecov/

COPY index.html /usr/local/apache2/htdocs/codecov/

COPY target/image /usr/local/apache2/htdocs/codecov/
