# VERSION 1.2.3
# AUTHOR:         Nicolas Lamirault <nicolas.lamirault@gmail.com>
# DESCRIPTION:    zeiot/rpi-traefik

FROM resin/armv7hf-debian:stretch
MAINTAINER Nicolas Lamirault <nicolas.lamirault@gmail.com>

ENV TRAEFIK_VERSION 1.1.2

ADD https://github.com/containous/traefik/releases/download/v${TRAEFIK_VERSION}/traefik_linux-arm /traefik
RUN chmod +x /traefik

EXPOSE 80

VOLUME ["/etc/traefik"]

ENTRYPOINT [ "/traefik" ]

CMD ["--configfile", "/etc/traefik/traefik.toml"]
