FROM postgres:12-alpine

RUN cp /usr/share/zoneinfo/America/Bahia /etc/localtime \
    && echo "America/Bahia" > /etc/timezone \
    && apk add nano

ENV TZ="America/Bahia"
ENV PGTZ="America/Bahia"

EXPOSE 5432
