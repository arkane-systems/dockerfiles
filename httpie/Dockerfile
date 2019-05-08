# httpie, intuitive CLI http client
#
# docker run --rm -it 80:80 cerebrate/httpie
#

FROM python:2-slim-stretch
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="HTTPie: intuitive CLI http client"

RUN pip install --no-cache-dir httpie httpie-unixsocket

ENTRYPOINT [ "http" ]
