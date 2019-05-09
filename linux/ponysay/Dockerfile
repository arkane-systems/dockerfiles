# ponysay: like cowsay, but with more MLP:FiM
#
# docker run --rm -it cerebrate/ponysay <text>
#

FROM alpine:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="ponysay: like cowsay, but with more MLP:FiM"

WORKDIR /root

RUN apk --no-cache add python3 git texinfo && \
    git clone https://github.com/erkin/ponysay.git && \
    cd ponysay && \
    ./setup.py --freedom=partial install && \
    cd .. && \
    rm -rf ponysay && \
    apk del git texinfo

ENTRYPOINT [ "ponysay" ]
