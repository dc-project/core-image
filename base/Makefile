NAME = projectdc/base
VERSION = 9

all: build

build:
	docker build --tag=$(NAME):$(VERSION) .

tag_latest:
	docker tag $(NAME):$(VERSION) $(NAME):latest

release: tag_latest
	docker push $(NAME):latest
