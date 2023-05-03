FROM kalilinux/kali-rolling
LABEL "NT132"="Nhom12"
LABEL "Project"="beauty"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install apache2 -y
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD beauty.tar.gz /var/www/html
