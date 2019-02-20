TAG := jellyfin/ffmpeg:upgraded

.PHONY: build
build:
	docker build -t $(TAG) --build-arg MAKEFLAGS="-j$(cat /proc/cpuinfo | grep processor | wc -l)" .

push:
	echo TODO implement

run:
	docker run --device /dev/dri/renderD128:/dev/dri/renderD128 --rm -i -t $(TAG) $(ARGS)
