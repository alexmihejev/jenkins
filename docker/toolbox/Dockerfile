FROM alpine
RUN apk update && apk add --no-cache curl wget busybox-extras netcat-openbsd python py-pip bash && pip install awscli
RUN apk --purge -v del py-pip
