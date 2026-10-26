FROM postgres:17.2-alpine

COPY CreateTable.sql /docker-entrypoint-initdb.d/
COPY InsertData.sql /docker-entrypoint-initdb.d/