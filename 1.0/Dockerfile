# VERSION 1.0.3
# AUTHOR:         Nicolas Lamirault <nicolas.lamirault@gmail.com>
# DESCRIPTION:    zeiot/rpi-traefik

FROM resin/armv7hf-debian:jessie
MAINTAINER Nicolas Lamirault <nicolas.lamirault@gmail.com>

ENV TRAEFIK_VERSION 1.0.3

ADD https://github.com/containous/traefik/releases/download/v${TRAEFIK_VERSION}/traefik_linux /traefik

RUN chmod +x /traefik

EXPOSE 80 8080

ENTRYPOINT ["/traefik"]

