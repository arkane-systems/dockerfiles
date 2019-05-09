# Netcat, containerized.

FROM debian:sid-slim
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Netcat: the tcp swiss army tool"

RUN apt-get update && apt-get install -y \
	netcat \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT [ "netcat" ]
