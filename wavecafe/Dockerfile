FROM centos:7
LABEL "Author"="saiteja Irrinki"
LABEL "Project"="Wave"
RUN yum install httpd wget unzip -y
RUN wget https://www.tooplate.com/zip-templates/2121_wave_cafe.zip --no-check-certificate
RUN unzip 2121_wave_cafe.zip
RUN cp -r 2121_wave_cafe/* /var/www/html/
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/httpd

