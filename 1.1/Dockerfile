# VERSION 1.1.2
# AUTHOR:         Nicolas Lamirault <nicolas.lamirault@gmail.com>
# DESCRIPTION:    zeiot/rpi-traefik

FROM resin/armv7hf-debian:jessie
MAINTAINER Nicolas Lamirault <nicolas.lamirault@gmail.com>

ENV TRAEFIK_VERSION 1.1.2

ADD https://github.com/containous/traefik/releases/download/v${TRAEFIK_VERSION}/traefik_linux-arm /traefik
RUN chmod +x /traefik

EXPOSE 80

VOLUME ["/etc/traefik"]

ENTRYPOINT [ "/traefik" ]

CMD ["--configFile", "/etc/traefik/traefik.toml"]
