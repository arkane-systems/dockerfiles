# httpie, intuitive CLI http client
#
# docker run --rm -it cerebrate/httpie <url>
#

FROM python:3-alpine
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="HTTPie: intuitive CLI http client"

RUN pip install --no-cache-dir httpie httpie-unixsocket

ENTRYPOINT [ "http" ]
