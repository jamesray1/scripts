#IMAGE for libp2p-js-echo-server
#Created by Parity Technologies <devops@parity.io>
USER=parity
NAME=libp2p-js-echo-server
TAG=gitlab-ci

IMAGE=${USER}/${NAME}:${TAG}

help:
	@echo "Build rustup image."
	@echo
	@echo "Usage:"
	@echo "  make [help]        - display this message"
	@echo "  make image         - build rustup image"
	@echo "  make push          - push build image to the regitry"

image:
	docker build --tag ${IMAGE} .

push:
	docker push ${IMAGE}

.PHONY: help image push
