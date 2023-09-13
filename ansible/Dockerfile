 

FROM python:3-alpine

LABEL maintainer "Christian Koep <christiankoep@gmail.com>"

RUN buildeps = ' \
		musl-dev \
		openssl-dev \
		libffi-dev \	
		gcc \
		' \
	&& apk --no-cache add \
	ca-certificates \
	$builddeps \
	&& pip install \
		ansible \
	&& apk del --purge $buildeps

ENTRYPOINT [ "ansible" ]
