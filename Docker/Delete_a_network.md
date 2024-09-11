# Task
The Nautilus DevOps team is planning to do some cleanup on App Server 2 in Stratos Datacenter, some old and unused docker networks need to be deleted. Find below more details:

Delete a docker network named `php-network` from `App Server 2` in Stratos Datacenter.

## Solution
Connect to the App Server 2.

```sh
ssh steve@stapp02
```

List all the networks.

```sh
sudo docker network ls
```

Delete the network.

```sh
sudo docker network rm php-network
php-network
```

## References

[docker network delelte](https://docs.docker.com/reference/cli/docker/network/rm/)<br/>
[docker network list](https://docs.docker.com/reference/cli/docker/network/ls/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
