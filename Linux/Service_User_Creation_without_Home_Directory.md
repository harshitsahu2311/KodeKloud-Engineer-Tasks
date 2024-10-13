# Task
In response to the latest tool implementation at `xFusionCorp Industries`, the system admins require the creation of a service user account. Here are the specifics:

Create a user named `kareem` in `App Server 1` without a `home directory`.

## Solution
Connect to the App Server 1.

```sh
ssh tony@stapp01
```

Create a user named `kareem` with the no `home` directory.
```sh
sudo useradd -M kareem
```

To Check the user, run the command
```sh
sudo cat /etc/pass* | grep kareem
```

## References

[Create User without home directory in Linux](https://linuxsimply.com/ubuntu-create-user-without-home-directory/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
