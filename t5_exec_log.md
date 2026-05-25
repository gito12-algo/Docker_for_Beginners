Debugging Docker Containers with docker exec and docker logs.

Commands for troubleshooting a Docker container are very useful. If something goes wrong in the container, you want to see the logs of the Docker container or get inside the container and use the terminal there.

```
docker logs (container_id)
```
or
```
docker logs (name of the container)
```
### When a container is created you just get some random name.

## this wiil create a new container and run with port and redis-older name
```
docker run -d -p6000:6397 --name redis-older redis:4.0
```
```
docker ps
```
## stop the continer
```
docker stop (container_id)
```
```
docker run -d -p6001:6397 --name redis-latest redis
```
Another very usefull command in debugging is docker exec. We can actually get the terminal of a running container.
```
docker exec (container_id)
```
here you become a root user so you run this command
```
ls
```
cd /
```
```
pwd
```
```
env
```
```
exit
```
This isvery usefull if you have a container with some complex configuration or you running your application that you worte in a container.

### what is the difference b/w docker run and docker stop command.
- docker run take an image with a specfic version or latest as a option or attribute. 
- docker start you not working images rather container.
