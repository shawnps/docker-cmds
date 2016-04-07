ROOT=sigscicmd
CONTAINER=rpm

build:
	docker build -t ${ROOT}/${CONTAINER} .

console:
	docker run -it --rm ${ROOT}/${CONTAINER} sh

.PHONY: build
.PHONY: console
