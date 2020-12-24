IMAGE=zimbra_docker
PROJECT_ID=zimbra-299618

VERSION=8.8.7

.PHONY: all build push

all: build

build:
	docker build --rm -t $(IMAGE) .

push:
	docker tag $(IMAGE) gcr.io/$(PROJECT_ID)/$(IMAGE):$(VERSION) && \
	docker push gcr.io/$(PROJECT_ID)/$(IMAGE):$(VERSION)
