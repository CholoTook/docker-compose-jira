FROM mysql:8.0

# NOTE: It's more canonical to put these in place using volumes at run time!
# TODO: mkdir conf.d docker-entrypoint-initdb.d (docker can only mount dirs)
# TODO: Remove this build step

COPY my.jira.cnf /etc/mysql/conf.d/

COPY setup-jira.sql /docker-entrypoint-initdb.d
