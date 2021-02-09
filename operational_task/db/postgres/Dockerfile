FROM postgres:9.6-alpine
LABEL maintainer="Eugene Papkou"
EXPOSE 5432
ENV POSTGRES_USER postgres
ENV POSTGRES_DB rates
COPY operational-task-git/db/rates.sql docker-entrypoint-initdb.d/
