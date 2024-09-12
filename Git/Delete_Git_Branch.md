## Task

The Nautilus developers are engaged in active development on one of the project repositories located at `/usr/src/kodekloudrepos/games`. During testing, several test branches were created, and now they require cleanup. Here are the requirements provided to the DevOps team:

On the `Storage server` in Stratos DC, delete a branch named `xfusioncorp_games` from the `/usr/src/kodekloudrepos/games` Git repository.

## Solution

Connect to Storage Server.
```sh
ssh natasha@ststor01
```
Go to the repo directory.

```sh
[natasha@ststor01 ~]$ cd /usr/src/kodekloudrepos/games
```

List all branches in this repo.
```sh
sudo git branch --list
  master
* xfusioncorp_games
```

Change branch to `master`.

```sh
sudo git checkout master
Switched to branch 'master'
```

Delete `xfusioncorp_games` branch.

```sh
sudo git branch -d xfusioncorp_games
Deleted branch xfusioncorp_games (was bc55b77).
```
## References

[git branch](https://git-scm.com/docs/git-branch)

<br/><br/>

[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
