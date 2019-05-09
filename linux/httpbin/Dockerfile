# HTTPbin, containerized.
#
# docker run --rm -d -p 80:80 cerebrate/httpbin
#

FROM python:3-alpine
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="HTTPBin: a simple HTTP request & response service"

RUN apk add --no-cache --virtual .build-deps \
		build-base \
		libffi-dev \
	&& pip3 install --no-cache-dir  \
		gevent \
		gunicorn \
		httpbin \
	&& apk del .build-deps

ENTRYPOINT ["gunicorn", "-b", "[::]:80", "httpbin:app", "-k", "gevent"]
