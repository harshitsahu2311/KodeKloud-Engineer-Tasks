# Task
The Nautilus DevOps team wanted to transfer some docker images from one server to another server so they wanted to save some docker images as tar archives on the docker host itself. Find below the exact requirements:<br/>
There is a docker image named `nginx:mainline-alpine-slim` on `App Server 2` in Stratos Datacenter, save this image as `nginx.tar` archive under `/home` directory on the same server.

## Solution

Connect to the App Server 2.

```sh
ssh steve@stapp02
```

Save the image in an archive.

```sh
docker save nginx:mainline-alpine-slim  > nginx.tar
```

Copy the archive to the /home.

```sh
scp nginx.tar /home
```

## References

[docker save](https://docs.docker.com/engine/reference/commandline/save/)
[docker load](https://docs.docker.com/engine/reference/commandline/load/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
