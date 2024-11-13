# How to build docker image locally

1. Set environment `IMG` as the target image on your computer. This variable
   should have the form of: `<registry>/<image-name>:<tag>`.
> You can option to use auxiliar variables `REGISTRY`, `IMAGE_NAME`, `TAG`. By
> default `IMG=$REGISTRY/$IMAGE_NAME:$TAG`

2. Execute the make target `docker-build`.
```sh
make docker-build
```

# How to push docker image manually

1. Set environment variable `IMG` with the image you want to upload.
> You can option to use auxiliar variables `REGISTRY`, `IMAGE_NAME`, `TAG`. By
> default `IMG=$REGISTRY/$IMAGE_NAME:$TAG`

2. Execute the make target `docker-push`
```sh
make docker-push
```
