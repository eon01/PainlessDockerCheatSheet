# PainlessDockerCheatSheet

## Delete all containers
```
docker rm $(docker ps -a -q)
```

## Delete all images
```
docker rmi $(docker images -q)
```

## Volumes
### List All Volumes
``` docker volume ls -qf dangling=true ```

### Cleanup Volumes

```
docker volume rm $(docker volume ls -qf dangling=true)
```

