## Q) What is container?
So technically container is made up of images so we have layers of stacked images on top of each other and at the base of most of the containers you would have a linux based image which is either Alpine with a specfic version or it could be some other linux distribution and it's important for those base images to be small that's why most of them are actually Alpine because that will make sure that the containers stay small in size which is one of the advantage of using container so on top of the base image you would have application image.
### layers of linux base image, application image with configuraton 
### Demo - docker container

## run a specfic version of postgres container.
```
docker run postgres:9.6

```
## you will sea all the running containers
```
docker ps

```
Let's another version of postgres to run at the same time on my local matchine.
```
docker run postgres:10.10

```
Again it doesn't find locally so it pushes and this is same applications but with just a different version some of the layers of the image are the same so i don't fetch this again they are already my matchine.
```
docker ps

```
