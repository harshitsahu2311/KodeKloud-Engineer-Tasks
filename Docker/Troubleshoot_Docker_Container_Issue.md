# Task
An issue has arisen with a static website running in a container named `nautilus` on `App Server 1`. To resolve the issue, investigate the following details:<br/>
Check if the container's volume `/usr/local/apache2/htdocs` is correctly mapped with the host's volume `/var/www/html`.<br/>
Verify that the website is accessible on host port `8080` on `App Server 1`. Confirm that the command `curl http://localhost:8080/` works on `App Server 1`.

## Solution
## Connect to the App Server 1.

```sh
ssh tony@stapp01
```

Check if container is running.

```sh
sudo docker ps -a
CONTAINER ID        IMAGE               COMMAND              CREATED             STATUS                     PORTS               NAMES
a186716f49a5        httpd               "httpd-foreground"   4 minutes ago       Exited (0) 4 minutes ago                       nautilus
```

Start the container that is in Exited status.

```sh
sudo docker start a1
a1
```

Check if we can connect to localhost on port 8080 and see if static website is running.

```sh
curl http://localhost:8080/
Welcome to xFusionCorp Industries!
```

## References

[docker container ls](https://docs.docker.com/engine/reference/commandline/container_ls/)

[docker start](https://docs.docker.com/engine/reference/commandline/start/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
