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

### Restarting existing container

```shell
docker start <container name/id>
```

### Detached mode

use `-d` flag to start in detached mode

### Attach to a running container

```shell
docker attach <container name/id>
```

### Fetch container logs

```shell
docker logs <container name>
```

add `-f` to attach and see future logs

### Interactive mode

```shell
docker run -it <image id/ name>

OR

docker start -a -i <container name/ id>
```
