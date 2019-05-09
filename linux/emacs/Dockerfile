# Emacs, containerized.
#
# docker run --rm -it -v C:/Working:/host cerebrate/emacs
#

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Emacs: containerized editor^Woperating system"

RUN apk --no-cache add \
	--repository http://dl-cdn.alpinelinux.org/alpine/edge/community/ \
	emacs

VOLUME /host

CMD [ "/usr/bin/emacs" ]
