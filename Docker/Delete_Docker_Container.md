# Task
One of the Nautilus project developers created a container on App Server 3. This container was created for testing only and now we need to delete it. Accomplish this task as per details given below:

Delete a container named ```kke-container```, its running on ```App Server 3``` in Stratos DC.
## Solution
Connect to the App Server 3.

```sh
ssh banner@stapp03
```

Stop the container.
```sh
sudo docker container stop kke-container
kke-container
```
Remove the container.
```sh
sudo docker container rm kke-container
kke-container
```

## References

[docker stop](https://docs.docker.com/engine/reference/commandline/stop/)

[docker rm](https://docs.docker.com/engine/reference/commandline/rm/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
