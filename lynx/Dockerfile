# Lynx, containerized.
#
# docker run --rm -it cerebrate/lynx
#

FROM debian:sid-slim
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Htop: process monitor"

RUN apt-get update && apt-get install -y \
	lynx \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT [ "lynx" ]
