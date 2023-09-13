

FROM openjdk:8-alpine

LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apk add --no-cache \
	ca-certificats \
	curl \
	tar

ENV Lang C.UTF-8

ENV ATD_Version 081310

RUN curl -ssl "http://www.polishmywriting.com/download/atd_distribution${ATD_VERSION}.tgz" -o /tmp/atd.tar.gz \
	&& mkdir -p /usr/src/atd \
	&& tar -xvf /tmp/atd.tar.gz -C /usr/src/atd --strip-components 1 \
	&& rm /tmp/atd.tar.gz* 

WORKDIR /usr/src/atd

EXPOSE 1049

ENTRYPOINT [ "sh" , "-c" , "/usr/src/atd/run.sh"]
