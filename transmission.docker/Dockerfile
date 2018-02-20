FROM alpine
MAINTAINER strakh.alex
COPY settings.json /root/.config/transmission-daemon/settings.json
RUN apk update && \
    apk add transmission-daemon
EXPOSE 9091/tcp 51413/udp
CMD ["/usr/bin/transmission-daemon","-f"]
