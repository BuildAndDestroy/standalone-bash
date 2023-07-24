FROM debian:latest
RUN apt update -y
RUN apt install wget gcc make -y
WORKDIR /opt
RUN wget -c http://deb.debian.org/debian/pool/main/b/bash/bash_5.2.15.orig.tar.gz
RUN tar -zxvf bash_5.2.15.orig.tar.gz
WORKDIR /opt/bash-5.2.15
RUN ./configure --enable-static-link
RUN make
#RUN ldd bash
