FROM mysql:8.0

COPY my.jira.cnf /etc/mysql/conf.d/

COPY setup-jira.sql /docker-entrypoint-initdb.d
