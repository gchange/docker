FROM debian:jessie
RUN /bin/echo -e "deb http://mirrors.163.com/debian/ jessie main non-free contrib\n\
deb http://mirrors.163.com/debian/ jessie-updates main non-free contrib\n\
deb http://mirrors.163.com/debian/ jessie-backports main non-free contrib\n\
deb-src http://mirrors.163.com/debian/ jessie main non-free contrib\n\
deb-src http://mirrors.163.com/debian/ jessie-updates main non-free contrib\n\
deb-src http://mirrors.163.com/debian/ jessie-backports main non-free contrib\n\
deb http://mirrors.163.com/debian-security/ jessie/updates main non-free contrib\n\
deb-src http://mirrors.163.com/debian-security/ jessie/updates main non-free contrib" > /etc/apt/sources.list
RUN apt-get upgrade
RUN apt-get update
RUN apt-get install -y apt-utils dnsutils net-tools sysstat iotop ssh gcc g++ mysql-client
RUN apt-get install -y wget curl
RUN apt-get install -y git subversion
CMD /bin/bash