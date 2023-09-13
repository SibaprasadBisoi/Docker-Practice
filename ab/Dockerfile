

FROM alpine:latest

LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apk --no-cache add \
	apache2-ssl \
	apache2-utils \
	ca-certificates \
	htop

ENTRYPOINT [ "ab" ]
