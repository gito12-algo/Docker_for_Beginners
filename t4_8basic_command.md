# Docker Basic Commands
- Container vs Image
- Version and Tag
# Dockcer Commands
- docker pull
- docker run 
- docker run --options
- docker stop
- docker start
- docker ps
- docker exec -it
- docker log


# Q) what is the difference b/w container vs image?
Mostly pepole use those terms interchangeably but actually there is a fine difference b/w the two.
- Image is just the part of the container runtime. So the 
container is the running environments for an image.
- Container is a running environment for Image. Container has its own abstraction of an operating system including the file system and the environment.

# Q) what is tag?
- Tag is basically the version of the image.
```
docker pull redis
```
# To check existing images
```
docker images
```
# run the container
```
docker run redis
```
# to see the running container
```
docker ps
```
# run container in detached mode 
```
docker run -d redis
```
# to check the ruuning container
```
docker ps 
```
# restart the container 
```
docker stop ____(container_id)____
```
# start the container
```
docker start ____(container_id)____
```
# show you all container running or not running
```
docker ps -a
```

# Container port vs Host port
- Container is just a virtual environment running on your host and you have multiple container running simuiltaneously on your host which is your laptop pc.So your laptop has certain p0orts available.You need create s0-called binding b/w a port that your laptop your host matchine has and the container.
- yow will be confilict if you open to two 5000 ports on your hosts.

# to same container binding port 
```
docker run -p6000:6329
```
# bind a port 
```
docker run -p ---(port)
```
