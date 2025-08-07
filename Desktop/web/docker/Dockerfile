FROM ubuntu:14.04

RUN apt-get update

RUN apt-get install apache2 -y

RUN echo '<!DOCTYPE html><html><body><h1>Hello, Hanbat Study!</h1></body></html>', > /var/www/html/index.html

EXPOSE 80

#컨테이너 시작시 apache2를 백그라운드에서 실행되게 한다.
CMD service apache2 start && tail -f /var/log/apache2/access.log