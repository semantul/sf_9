FROM alpine:3.14

ENV SITE="ya.ru"
RUN apk add --update curl && \
    rm -rf /var/cache/apk/* && \
    mkdir -p /opt/app/ico
COPY ./favicon.sh /opt/app
WORKDIR /opt/app
CMD /bin/sh ./favicon.sh $SITE
