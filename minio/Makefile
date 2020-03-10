VERSION    ?= 1.0.0
IMAGE_NAME ?= bilderlings/minio-mc

build:
	docker build -t $(IMAGE_NAME):$(VERSION) .
	docker tag $(IMAGE_NAME):$(VERSION) $(IMAGE_NAME):latest
.PHONY: build

test:
	docker build -t $(IMAGE_NAME):$(VERSION) .
	docker run $(IMAGE_NAME):$(VERSION)

push:
	docker push $(IMAGE_NAME):$(VERSION)
	docker push $(IMAGE_NAME):latest
.PHONY: push

