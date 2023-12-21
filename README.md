# Worlds smallest Docker Image - aka WSDI | 92 bytes

https://hub.docker.com/repository/docker/dooqod/wsdi/general

Hi everyone,

If you ever wondered what is the minimal Docker image in the world, then you are in right place.
Is it debian, is it alpine or busybox ? 

Our team at Dooqod did extensive research on to figure out this.

We come up with 2 approaches to figure this out.

## Approch 1:
At least there is finate amount of Docker images under DockerHub. 
So this task should not be impossible. To run all of them and compare.

But it'll take lots of time and resources. 

## Approach 2:
We decided to create the smallest one and publish under DockerHub. Sounds promising.

## Wow moment

Wow, we can create the smallest Docker image in the world.

It can be the MVP and we can try to sell it :) 

So we started this project right away.

## Dockerfile of the 'worlds-smallest-docker-image'

d - is just an emptyfile we add into 'scratch'

```shell
FROM scratch
ADD d /d

```

## What is scratch ?

The scratch image is the most minimal image in DockerHub. This is the base ancestor for all other images. 
The scratch image is actually empty. It doesn't contain any folders/files.

You can use Docker’s reserved, minimal image, scratch, as a starting point for building containers. Using the scratch “image” signals to the build process that you want the next command in the Dockerfile to be the first filesystem layer in your image.

While scratch appears in Docker’s repository on the hub, you can’t pull it, run it, or tag any image with the name scratch. Instead, you can refer to it in your Dockerfile. For example, to create a minimal container using scratch:

https://hub.docker.com/_/scratch

## How to build 

```shell
# just clone the repo
# cd into repository and run 

docker build -t wsdi .

# or pull from DockerHub

docker pull docker.io/dooqod/wsdi:latest

# check 


```

## Support the project to not grow :)

Our goal is to make this image minimal.
We'll put all our efforts to keep it simple and small also in the feature.

 - Give a Github Star
 - Buy lambo - 




