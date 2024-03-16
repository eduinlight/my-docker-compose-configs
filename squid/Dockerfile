FROM alpine

ENV SQUID_ACCESS_LOG /var/log/squid/access.log

WORKDIR /etc/squid
RUN apk add squid bash openrc
RUN rc-service -e squid
RUN touch $SQUID_ACCESS_LOG
CMD tail -f $SQUID_ACCESS_LOG
