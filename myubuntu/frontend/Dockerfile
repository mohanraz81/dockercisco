FROM ubuntu:18.04
MAINTAINER mohanraz@gmail.com
RUN apt-get -y update
ENV TZ=Asia/Kolkata
RUN apt-get -y install tzdata
ADD config /opt
RUN apt-get -y install `cat /opt/packages` 
ADD code /var/www/html
CMD ["nginx","-g","daemon off;"]