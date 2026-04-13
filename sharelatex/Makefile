IMAGE = ghcr.io/chrisx8/sharelatex
VERSION ?= 6.1.2

.PHONY: build push

build:
	podman build --build-arg VERSION=${VERSION} --tag ${IMAGE}:${VERSION} .

push:
	podman push ${IMAGE}:${VERSION}
