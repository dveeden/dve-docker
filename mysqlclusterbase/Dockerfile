FROM fedora:20
MAINTAINER Daniël van Eeden <docker@myname.nl>

ADD mysql-cluster-gpl-7.2.17-linux2.6-x86_64.tar.gz /opt/
RUN mv /opt/mysql-cluster-gpl-7.2.17-linux2.6-x86_64 /opt/mysql

RUN yum -y install libaio
RUN groupadd mysql
RUN useradd -g mysql -s /sbin/nologin mysql
