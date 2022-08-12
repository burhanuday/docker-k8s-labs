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

### List images

```shell
docker images
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

### Remove a container

You cannot remove a running container. It needs to be stopped first

```shell
docker rm <container_name1> <container_name2> ...
```

### Removing images

Images can only be removed if they aren't being used by any containers including stopped containers

```shell
docker rmi <imageid>
```

### Remove unused images

```shell
docker image prune
```

### Automatically remove container when it exits

Use the `--rm` flag

```shell
docker run --rm <image_id>
```

### Inspect image

```shell
docker inspect <image_id>
```

### Copy files to/from containers

```shell
docker cp <source> <dest>
docker cp local_path/ container_name:/path
docker cp container_name:/path local_path/
```

### Name a container

```shell
docker run <imageid> --name myapp
```

### Tag an image

```shell
docker build -t myname:mytag .
```
