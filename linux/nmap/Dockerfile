# Nmap, containerized.

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Nmap: network scanning tool"

RUN apk --no-cache add nmap

ENTRYPOINT [ "nmap" ]
