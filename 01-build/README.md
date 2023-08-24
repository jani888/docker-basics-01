# Docker basics lesson - demo 1

## 1. List docker images

```sh
docker images
```

## 2. Build the docker image
- build the docker image, and tag it with `my-image`
```sh
docker build . -t my-image
```
- Run docker images again to show the new image.
- Now try it without the `&& rm -rf /var/cache/apk/*` and compare the image sizes


## 3. Create a container from the image
- Run `docker run` to start an instance of the image
```sh
docker run my-image
```
- Create a container using `docker create`
```sh
docker create --name my-container my-image
```
- Start, stop and restart the container
```sh
docker start my-container
docker stop my-container
docker restart my-container
```

## 4. View (running) containers
- List running containers
```sh
docker ps
```
- List all containers
```sh
docker ps -a
```

## 5. Cleanup
- Remove the container:
```sh
docker rm my-container
```
- Remove the image:
```sh
docker rmi my-image
```