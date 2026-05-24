# kubernetes = K8s
container orchestration tool

To learn kubernetes you first have to understand what a container is and why we use them?

So in this toutorials, we'll talk about container concepts and one of the most popular implementations which is Docker.

## Q) What is a container and what problems does it solve?
## Q) How container can actually make the development process much easier and more efficient and also how they solve some of the problems in deployment processs of Applications.

## Q) What is a container?
Container is a way to package applications with all the necessary dependencies and configuration. 
Portable artifact easly shared and moved around between a development team or operations team and that portability of containers, everything packaged in one isolated environments gives it some advantage that makes development and deployment process more efficient.

## Q) Where do containers live?
Containres leave in a container repository, this is special type of storge for containers. many companies have their own private repositories where they store all the containers.

There are also public repository for docker containers where you can browse and probably find any application container that you want.

## Q) how containers improve the development process?
let's
How did we develop applications before the containers?
usually when you have a team or developer working on some applications you would have to install most of the services on your operating system directly.
Each developer needs to install the application specfic version
Installation process different on each OS evvironments
Many steps where something could go worng.

## Q) How containers solve all of this problems?
With containers you actually do not have tgo install any of the services directly in your operating system because the container is it own isolated operating system layer with linux base image. You have everyting packaged in one isolated environment (so you have PostgreSQL with a specfic version)
Packaged with all needed configurations.
### one command to install the applications.
### Run the same app with 2 different versions.

## Q) how container improve the deployment process/
Now you have the developers and operations working in one team to package the whole configurations dependencies inside the applications directly on the server, so here you need to run a docker command that pulls some the repository and runs this that makes the process.
###  Developers and Operations work together to package the application in a container
### No environmejnt configuration needed on server - execpt for docker runtime.

 