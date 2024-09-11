# Task
To accommodate the backup agent tool's specifications, the system admin team at ```xFusionCorp Industries ```requires the creation of a user with a non-interactive shell. Here's your task:<br/>
Create a user named ```rose``` with a non-interactive shell on ```App Server 1```.


## Solution

Connect to the App Server 1.

```sh
ssh tony@stapp01
```

Create a user named `rose` with the `nologin` shell. This can be achieved by using the `--shell` flag followed by the path of the desired shell. In our case, to create a user with a non-interactive shell, use `/usr/sbin/nologin`.  
```sh
sudo adduser rose  --shell /usr/sbin/nologin
```
Check if the user rose has assigned a correct shell.
```sh
sudo cat /etc/passwd | grep rose
rose:x:1002:1002::/home/rose:/usr/sbin/nologin
```

## References

[Create Non Login User in Linux](https://www.baeldung.com/linux/create-non-login-user)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
