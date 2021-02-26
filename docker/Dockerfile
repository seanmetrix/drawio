FROM openjdk:8-alpine AS build

RUN apk update --no-cache && \
    apk add --no-cache \
        apache-ant \
        git

COPY . /tmp/drawio

RUN cd /tmp && \
    # git clone https://github.com/jsknight/drawio.git && \
    cd /tmp/drawio/etc/build/ && \
    ant war