 

FROM alpine:latest

LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apk --no-cache add \
	aspell \
	aspell-en

ENTRYPOINT [ "aspell" ]
