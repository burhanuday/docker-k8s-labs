# Docker K8s Labs

## Docker commands cheat-sheet

### Build an image

```shell
docker build <docker file path>
```

### Run a container

```shell
docker run <image id/ image name>
```

### List running containers

```shell
docker ps
```

### List all containers

```shell
docker ps -a
```

### Stop a container

```shell
docker stop <container name>
```

### Exposing ports

p flag is called publish

```shell
docker run -p <local port>:<container port> <container name>
```
