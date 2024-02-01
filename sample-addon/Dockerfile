ARG BUILD_FROM
FROM $BUILD_FROM

RUN apk update && apk add --no-cache python3 && \
rm -rf /var/cache/apk/*

COPY rootfs /

WORKDIR /data

COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]