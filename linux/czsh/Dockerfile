# Minimal zsh/oh-my-zsh install on Debian, for testing.

FROM debian:latest
LABEL maintainer="Alistair Young <avatar@arkane-systems.net>" version="1.0" description="A basic Debian image with zsh and oh-my-zsh installed."

RUN apt-get update && \
    apt-get install -y zsh && \
    apt-get install -y wget && \
    apt-get install -y git && \
    chsh -s /bin/zsh

ENV SHELL /usr/bin/zsh

WORKDIR /root

RUN wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh

COPY ./.zshrc /root/.zshrc

VOLUME /host

WORKDIR /host

ENTRYPOINT /bin/zsh
