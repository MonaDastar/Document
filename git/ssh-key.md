
Generate ssh key in the local machine:

ssh keys are to set us free from logging into the cloud space to have clone.

```sh
ssh-keygen -t rsa -b 4096 -C "<username>@<email>"  
```
 try to choose a meaningful name to help you remember the purpose of creating this repository



steps after generating ssh key: 
    read the ssh file: 

```sh
    cat ~/.ssh/id_rsa_<your_rsa_name >.pub
```

 Copy your SSH public key to your clipboard. ...
    Log into GitHub  and go to the upper-right section of the page, click in your profile photo, and select Settings. ...
    Then, in profile your settings, click SSH and GPG keys. ...
    Click the New SSH key button.
   



in the github or other cloud spaces make sure that the project visibility is public so that people can reach your project


to test if you are correctly authenticated,

```sh
ssh -T ssh -T git@github.  >>domain name
```
 and the session would immediately end with:

Hi username!  You've successfully authenticated, 
but GitHub does not provide shell access. 

another way to try if the ssh works well you can get a clone, on the branch in github, copy the address of the project folder:
```sh
git clone https://git.hamidrabedi.ir/pyze/core-commerce.git
```
if you do not want to clone with https, change the address type from clone button in the github score-commerce page and change it to ssh.

```sh
git clone  
```


