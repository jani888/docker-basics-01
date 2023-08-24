# Docker basics lesson - demo 2

## 1. Docker hub
- navigate to [Docker Hub](https://hub.docker.com)
- create an account
- go to the repositories tab
- create a new repository


## 2. Pull an image
```sh
docker pull nginx:latest
```


## 2. Push
First tag it with your username and repo
```sh
docker tag nginx:latest <your_username>/<repo>:latest
```

```sh
docker push <your_username>/<repo>:latest
```