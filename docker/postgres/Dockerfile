FROM postgres:12-alpine

RUN cp /usr/share/zoneinfo/America/Bahia /etc/localtime \
    && echo "America/Bahia" > /etc/timezone \
    && apk add nano

ENV TZ="America/Bahia"
ENV PGTZ="America/Bahia"

COPY backup.sql /docker-entrypoint-initdb.d/

EXPOSE 5432
