# Lynx, containerized.
#
# docker run --rm -it cerebrate/lynx
#

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Lynx: text-based web browser"

RUN apk --no-cache add lynx

ENTRYPOINT [ "lynx" ]
