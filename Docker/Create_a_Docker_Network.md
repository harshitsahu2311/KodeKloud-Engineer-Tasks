# Task
The Nautilus DevOps team is planning to setup/create some docker containers on App Server 2 in Stratos Datacenter, some prerequisites are needs to be done on this server. Find below more details:


Create a new network named `mysql-network` using the `bridge` driver. Allocate subnet `182.18.0.0/24`, configure Gateway `182.18.0.1`.

## Solution

Connect to the App Server 2.

```sh
ssh steve@stapp02
```

Create a network.

```sh
sudo docker network create --driver=bridge --subnet=182.18.0.0/24 --gateway=182.18.0.1 mysql-network
04ec795810e7255a3c1449ad13b7564d58e2fe66b79fc60ae393b9a9c32976d3
```

## References

[docker network create](https://docs.docker.com/engine/reference/commandline/network_create/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
