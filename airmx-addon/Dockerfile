# hadolint global ignore=DL3006,DL3042
ARG BUILD_FROM
FROM $BUILD_FROM

WORKDIR /

RUN apk add --no-cache python3 py3-pip mosquitto && \
    pip3 install flask==3.0.0 gunicorn==21.2.0

COPY rootfs /

VOLUME /data
EXPOSE 25880 25883
