FROM projectdc/base:latest

MAINTAINER ysicing

ADD sid.list /etc/apt/sources.list.d/sid.list

RUN \
    DEBIAN_FRONTEND=noninteractive apt update && \
    DEBIAN_FRONTEND=noninteractive apt install -y \
    python3.6 \
    python3-apt \
    python3-pip \
    python3.6-dev \
    libffi-dev \
    build-essential \
    redis-server && \
    rm -rf /var/lib/apt/lists/*