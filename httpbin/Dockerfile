# HTTPbin, containerized.
#
# docker run --rm -d -p 80:80 cerebrate/httpbin
#

FROM cerebrate/python:3-with-buildessentials
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="HTTPBin: a simple HTTP request & response service"

RUN pip3 install --no-cache-dir gevent gunicorn httpbin && \
	apt remove build-essential -y && \
	apt autoremove -y && \
	rm -rf /var/lib/apt/lists/*

CMD ["gunicorn", "-b", "0.0.0.0:80", "httpbin:app", "-k", "gevent"]
