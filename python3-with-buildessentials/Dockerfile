# Python 3 with build essentials
#
# Intermediate container - not for direct use.
#

FROM python:3-slim-stretch
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="Python 3 image with build-essentials (intermediate)"

RUN apt-get update && apt-get install -y build-essential

CMD [ "bash" ]
