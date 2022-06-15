FROM golang:1.17 AS builder

MAINTAINER docker-network

WORKDIR /build

COPY ./linux_amd64/main /build
COPY ./public /build/public
COPY ./template /build/template
COPY ./config/ /build/config
COPY ./data/ /build/data

EXPOSE 8200

ENTRYPOINT ["./main"]
