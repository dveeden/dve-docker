FROM dveeden:ndb72base
MAINTAINER Daniël van Eeden <docker@myname.nl>

RUN cd /opt/mysql; ./scripts/mysql_install_db --user=mysql --datadir=/usr/local/mysql/data
ADD my.cnf /etc/
EXPOSE 3306
ENTRYPOINT /opt/mysql/bin/mysqld_safe --skip-grant-tables --ledir=/opt/mysql/bin --ndb-connectstring=${MGM01_PORT_1186_TCP_ADDR}
