# -*- docker-image-name: "sagittariidae" -*-

# ---
# ADAPT base container build.
# cf. https://docs.docker.com/engine/reference/builder/
# ---

FROM alpine:3.4
# cf. http://gliderlabs.viewdocs.io/docker-alpine,
#     https://github.com/gliderlabs/docker-alpine

MAINTAINER Docker <docker@adapt.mines.edu>

RUN apk add --progress --update \
    busybox-suid \
    ca-certificates \
    openssl \
    zsh \
    && update-ca-certificates
# busybox-suid: https://github.com/gliderlabs/docker-alpine/pull/122
SHELL ["/bin/zsh", "-c"]
