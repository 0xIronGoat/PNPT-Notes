# Users and Privileges
## Permissions
`ls -la` - list current directory contents along with permissions for each file/directory

Each entry begins with the permissions, e.g. `drwxr-xr-x`

`d` - means this is a directory, if this was a file it would start with `-`
`r` - read access
`w` - write access
`x` - execute access

The first character indicates if it is a file or a directory.  
The rest is split in to 3 groups of 3 `rwx`:  
1. File/directory owner permissions
2. File/directory group ownership permissions
3. All other users permissions

`chmod` - "change mode", alter file permissions
You can add a specific permission, e.g. to add execute permission: `chmod +x`

**Numerical permission values**  
`r`, `w`, and `x` each have a numerical value:  
	- `r` = 4  
	- `w` = 2  
	- `x` = 1  

Using the `chmod` command, you can use these numbers to set the permissions for user, group and others for a file.

`chmod 777` = `rwx` for everyone  
`chmod 764` = `rwx` for owner, `rw` for group and `r` for everyone else


## Users
`adduser` - add a new user  

You will see the new user defined in `/etc/passwd`  
The password hash for the user is stored in `/etc/shadow`  

`su` - switch user  
