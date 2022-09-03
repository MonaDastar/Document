# Git commands 
#### written by Mona Dastar
## how to start with Git:
to check if git is installed or not:
```sh
git --version
```
git configuration:
```sh
git config --global(optional) user.name 
git config --global(optional) user.email 
```
to create my first repository and initialize git inside it:

```sh
mkdir  foldername
cd foldername
git init   >> in the local machine
```

to add file to the snapshot or to stage a file:

```sh
git add file1,file2
```

to create a file in linux:
 ```sh
touch filename.postfix
 ```

to send files from snapshot or staging area to the local repository:
```sh
git commit -m "git commit message"
git commit   >> will have a longer message in the commit message
```

to see the status of the files:
```sh
git status
```
to see the history of my commits:
```sh
git log
git log --oneline          >> information in one line
git log --oneline --start  >> more information in one line
git kog --start  more info
git log -- oneline --patch  >> the diff between the previous commit and the new commit
git log -- oneline -3  >> the three last commits
git log -- oneline --author="Mona" >> all commits by Mona
git log -- oneline --after="2022-08-01" >> all commits after 2022-08-01
git log -- oneline --after="yesterday"
git log -- oneline --after= date  
git log --oneline --grep="feat" >> all commits with the prefix of "feat" or feature modifications
git log --oneline -S "hello()" >> all commits that had hello() added in their code
git log --oneline<commit-hash>..<commit-hash> >> shows all commits between the given commits
git log --oneline myfile.txt >> all commits done on myfile.txt
```
to download the repository from cloud to the local machine:
```sh
git clone "https://...
```
to create, view, and delete connections to other repositories
```sh
git remote [-v | --verbose]
git remote add [-t <branch>] [-m <master>] [-f] [--[no-]tags] [--mirror=(fetch|push)] <name> <URL>
git remote rename [--[no-]progress] <old> <new>
git remote remove <name>
```
to upload local repository content to a remote repository.
```sh
git push <remote> <branch>
git push origin master 
git push <remote> --force >> force the push even if it results in a non-fast-forward merge.
git push <remote> --all  >> Tags are not automatically pushed when you push a branch or use the --all option. The --tags flag sends all of your local tags to the remote repository.
```
#####Deleting a remote branch or tag

fully delete a branch, it must be deleted locally and also remotely
```sh
git branch -D branch_name 
git push origin :branch_name
```
```sh
git branch -m branch_name   >> change branch to branch_name
```

ti initialize git in our local machine:
```sh
git init
```
here if we type:
```sh
git remote -v
```
no remote will be found so:

to Create a new, empty Git repository on your remote server. Obtain the git remote add URL for the remote repository and add credentials if needed. Run the git remote add origin command from your local repository with the --set-upstream and the name of the active branch to push:
```sh
git remote add origin git@ssh.hamidrabedi.ir.pyez/core-commerce.git
```
origin is the name for our remote , we can choose any name:
```sh
git remote add abcd git@ssh.hamidrabedi.ir.pyez/core-commerce.git
```


to delete a remote:

```sh 
git remote rm <origin_name>
git remote rm abdc git@ssh.hamidrabedi.ir.pyez/core-commerce.git

```
to rename the remote:
```sh
get remote rename <old_name> <new_name?>
```
gitignore - Specifies intentionally untracked files to ignore
make sure to create one.

an empty folder will not be tracked so you need to make a file named: 
.gitkeep so the empty folder can be tracked as well.


```sh
git add tab >> gives the file that are not added yet
```

to restore a staged file:
```sh
got restore --staged <file_name>
```

to push:
```sh 
git push origin main
```
to pull
