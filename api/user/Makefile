VERSION=v1
DOCKERUSER=akhileshappala11

build:
	docker build -f Dockerfile -t userservice . --no-cache=true --platform=linux/amd64

push:
	docker tag userservice $(DOCKERUSER)/userservice:$(VERSION)
	docker push $(DOCKERUSER)/userservice:$(VERSION)
	docker tag userservice $(DOCKERUSER)/userservice:latest
	docker push $(DOCKERUSER)/userservice