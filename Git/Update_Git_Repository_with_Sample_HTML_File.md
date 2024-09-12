# Task

The Nautilus development team has initiated a new project development, establishing various Git repositories to manage each project's source code. Recently, a repository named `/opt/demo.git` was created. The team has provided a sample `index.html` file located on the jump host under the `/tmp` directory. This repository has been cloned to `/usr/src/kodekloudrepos` on the `storage server` in the Stratos DC.

1. Copy the sample `index.html` file from the jump host to the storage server placing it within the cloned repository at `/usr/src/kodekloudrepos/demo`.

2. Add and commit the file to the repository.

3. Push the changes to the master branch.

## Solution
Copy file to ststor01:  
```
sudo scp /tmp/index.html natasha@ststor01:/tmp
```

SSH to ststor01:
```
ssh natasha@ststor01
```

Run command:  
```
sudo mv /tmp/index.html /usr/src/kodekloudrepos/demo
```

Run Git add command:
```
sudo git add index.html
```

Run Git commit command: 
```
sudo git commit -m "add index.html"
```

Run Git push command:
```
sudo git push -u origin master
```

[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
