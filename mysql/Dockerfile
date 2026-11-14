FROM mysql:8.0
LABEL maintainer="Songjie Wang (wangso@missouri.edu)"

ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_USER=covid19-user
ENV MYSQL_PASSWORD=covid19-pass
ENV MYSQL_DATABASE=covid19

# The official MySQL image creates the database and user from the variables above
# and runs every .sql file in /docker-entrypoint-initdb.d/ on first start
COPY covid19.sql /docker-entrypoint-initdb.d/
