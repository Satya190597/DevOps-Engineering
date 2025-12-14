# DevOps-Engineering
## Linux
First Linux Instance.
Login to Linux Using SSL
`ssh -i "gfg-linux-shell.pem" ec2-user@<INSTANCE-PUBLIC-IP/INSTANCE-PUBLIC-DNS>`

**List all the users.**

`cat /etc/passwd`

**List all the groups.**

`cat /etc/group`

**Create A New User**

`sudo useradd <USER-NAME>`

**List all files including those whose names begin with a dot.**

`ls -a`

**To see current working directory**

`pwd`

## Move files and directories.

Move a file from present directory to another directory.

`mv <FILE-NAME> <DIRECTORY-PATH>`

Move multiple files from present directory to another directory.

`mv <FILE-NAME> <FILE-NAME> <FILE-NAME> <DIRECTORY-PATH>`

Rename a particular file.

`mv <OLD-FILE-NAME> <NEW-FILE-NAME>`

Rename a directory.

`mv <OLD-DIRECTORY-NAME-WITH-PATH> <NEW-DIRECTORY-NAME-WITH-PATH>`

Remove files and directory.

Delete a file.

`rm <FILE-NAME>`

Delete a directory recursively.

`rm -rf <DIRECTORY-NAME>`

To display the user manual of any command that we can run on the terminal.

`man ls`


