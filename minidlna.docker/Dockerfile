FROM alpine
MAINTAINER strakh.alex
RUN apk update && \
    apk add minidlna && \
    apk add minissdpd
COPY minidlna.conf /etc/minidlna.conf
EXPOSE 8200/tcp 1900/udp
CMD ["/usr/sbin/minidlnad","-S"]
