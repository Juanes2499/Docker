FROM centos
MAINTAINER Oscar Mondragon
RUN yum install httpd -y
RUN echo "<h1> Bienvenidos a esta pagina </h1>" > /var/www/html/index.html
EXPOSE 80
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]