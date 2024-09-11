The DevOps team established a new Git repository last week, which remains unused at present. However, the Nautilus application development team now requires a copy of this repository on the Storage Server in the Stratos DC. Follow the provided details to clone the repository:<br /><br />
The repository to be cloned is located at ``` /opt/media.git ```.<br />
Clone this Git repository to the ``` /usr/src/kodekloudrepos ``` directory. Ensure no modifications are made to the repository during the cloning process.<br />

Solution:  
1. SSH to stsor01  
2. cd to /usr/src/kodekloudrepos
```bash
cd /usr/src/kodekloudrepos
```
  
3. Run command:  
```bash
git clone /opt/official.git
```
4. Verify
```bash
ls /usr/src/kodekloudrepos
```

[back](https://github.com/harshitsahu2311/Kodekloud-Engineer-Tasks)
