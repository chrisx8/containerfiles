IMAGE = ghcr.io/chrisx8/sharelatex
VERSION ?= 6.2.1

.PHONY: build push

build:
	podman build --build-arg VERSION=${VERSION} --tag ${IMAGE}:${VERSION} .

push:
	podman push ${IMAGE}:${VERSION}
