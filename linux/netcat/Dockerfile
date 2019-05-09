# Netcat, containerized.

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Netcat: the tcp/ip swiss army knife"

RUN apk --no-cache add nmap

ENTRYPOINT [ "ncat" ]
