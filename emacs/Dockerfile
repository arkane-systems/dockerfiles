# Emacs, containerized.
#
# docker run --rm -it -v C:/Working:/host cerebrate/emacs
#

FROM debian:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Emacs: containerized editor^Woperating system"

RUN apt-get update && apt-get install -y \
	emacs-nox \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

VOLUME /host

CMD [ "/usr/bin/emacs" ]
