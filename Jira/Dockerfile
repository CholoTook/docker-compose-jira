FROM atlassian/jira-software

# See https://confluence.atlassian.com/adminjiraserver/connecting-jira-applications-to-mysql-8-0-1018775461.html
# and  https://downloads.mysql.com/archives/c-j/

# TODO: Try a newer Mysql?

ARG mysqlcon=mysql-connector-j-8.0.33

ADD https://downloads.mysql.com/archives/get/p/3/file/${mysqlcon}.tar.gz /tmp/

RUN tar -C /tmp/ -zxvf /tmp/${mysqlcon}.tar.gz ${mysqlcon}/${mysqlcon}.jar 

RUN rm /tmp/${mysqlcon}.tar.gz

RUN cp /tmp/${mysqlcon}/${mysqlcon}.jar /opt/atlassian/jira/lib/

