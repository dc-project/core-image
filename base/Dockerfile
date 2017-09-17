FROM debian:stretch-slim

MAINTAINER ysicing

ENV TZ="Asia/Shanghai"
ENV TERM="xterm"

ADD stretch.list /etc/apt/sources.list

RUN \
    DEBIAN_FRONTEND=noninteractive apt update && \
    DEBIAN_FRONTEND=noninteractive apt install --no-install-recommends -y \
    gnupg  \
    curl wget sudo nano \
    ca-certificates \
    unzip \
    apt-transport-https && \
    apt upgrade -y && \
    apt dist-upgrade -y && \
    apt-get autoclean && apt-get autoremove && \
    rm -rf /var/lib/apt/lists/*
