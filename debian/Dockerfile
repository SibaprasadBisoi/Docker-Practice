

FROM debian:sid-slim

LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apt get update && apt-get install -y \
	adb \
	android-tools* \
	ca-certificates \
	curl \
	firstboot \
	usbutils \	
	--no-install-recomends \
	&& rm -rf /val/lib/apt/lists/*

ENTRYPOINT [ "bash" ] 
