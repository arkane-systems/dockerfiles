# Htop, containerized.
#
# docker run --rm -it --pid host cerebrate/htop
#

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Htop: process monitor"

RUN apk --no-cache add htop

CMD [ "htop" ]
