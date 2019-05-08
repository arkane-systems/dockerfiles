# ponysay: like cowsay, but with more MLP:FiM
#
# docker run --rm -it cerebrate/ponysay <text>
#

FROM debian:stretch-slim
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="ponysay: like cowsay, but with more MLP:FiM"

RUN apt update && \
    apt install python3 wget -y && \
    wget http://www.vcheng.org/ponysay/ponysay_3.0.2-1_all.deb && \
    dpkg -i ponysay_3.0.2-1_all.deb && \
    apt remove wget -y && \
    apt autoremove -y

ENTRYPOINT [ "ponysay" ]
