# linuxlearning

# User Management
### Create User
`useradd <username>`
### Set Password
`passwd <username>`


# SSH Key generation
### Follow along the steps after entering the below command
`ssh-keygen`


# SUDO Management
### User can be added in `/etc/sudoers` file or can be added as a part of `wheel` group
- "wheel" is a default group in linux available to be assigned to users which are to be configuired as sudo users.
- To add user in wheel group, follow the below steps.
1. Switch to root user.
2. Run the command `usermod -G wheel <username>` 


- To add a user in `/etc/sudoers` file, add an entry in the file in below format.
1. `<username>    ALL=(ALL)       ALL`

- To add a group in `/etc/sudoers` file, add an entry in the file in below format.
1. `%<groupname>    ALL=(ALL)       ALL`