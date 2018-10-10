# golang-docker-multistep

## Build
```
docker build -t kristaxox/golang-docker-multistep .
```

## Run
```
docker run -it kristaxox/golang-docker-multistep
```

## Why?
A multistep docker build process allows your code to be built with all the regular tooling, and your deployable docker image to be tiny :).
```
➜  golang-docker-multistep git:(master) ✗ docker images
REPOSITORY                          TAG                 IMAGE ID            CREATED              SIZE
kristaxox/golang-docker-multistep   latest              91a821f14d1e        About a minute ago   6.42MB
```