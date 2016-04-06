ROOT=sigscicmd
CONTAINER=aws

build:
	docker build -t ${ROOT}/${CONTAINER} .

help:
	docker run ${ROOT}/${CONTAINER} --help

version:
	docker run ${ROOT}/${CONTAINER} --version

console:
	docker run -it --rm ${ROOT}/${CONTAINER} sh

.PHONY: build
.PHONY: console
