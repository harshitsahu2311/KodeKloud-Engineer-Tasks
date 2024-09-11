# Create a group

The system admin team at ```xFusionCorp Industries``` has streamlined access management by implementing group-based access control. Here's what you need to do:



a. Create a group named ```nautilus_noc``` across all App servers within the ```Stratos Datacenter```.


b. Add the user ```rajesh``` into the ```nautilus_noc``` group on all App servers. If the user doesn't exist, create it as well.

## Solution 

Connect to the Nautilus App 1 using ssh.

```sh
ssh tony@stapp01
```

Create a group named nautilus_noc.
```sh
sudo groupadd nautilus_noc
```
Check if user rajesh is already created.
```sh
sudo getent passwd | grep rajesh
```

Create a new user named rajesh and assign group nautilus_noc.
```sh
sudo useradd -G nautilus_noc rajesh
```

Check if the user kano is created.
```sh
sudo getent passwd | grep rajesh
```
Check if the group nautilus_admin_users is assigned to the user kano.
```sh
[tony@stapp01 ~]$ id rajesh
```

Similarly make users and group in ```steve``` and ```banner``` user of Nautilus Project.
## References

[How to Create Groups in Linux](https://linuxize.com/post/how-to-create-groups-in-linux/)

[How to List Users in Linux](https://linuxize.com/post/how-to-list-users-in-linux/)

[How to Create Users in Linux](https://linuxize.com/post/how-to-create-users-in-linux-using-the-useradd-command/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
