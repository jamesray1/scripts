#IMAGE for build rust armv7 arch
#Created by Parity Technologies <devops@parity.io>
USER=parity
NAME=rust-armv7
TAG=latest

IMAGE=${USER}/${NAME}:${TAG}

help:
	@echo "Build rustup armv7 image."
	@echo
	@echo "Usage:"
	@echo "  make [help]        - display this message"
	@echo "  make image         - build rustup arm image"
	@echo "  make push          - push built image to the regitry"

image:
	docker build --tag ${IMAGE} .

push:
	docker push ${IMAGE}

.PHONY: help image push
