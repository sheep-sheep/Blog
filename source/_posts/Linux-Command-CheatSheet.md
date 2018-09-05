---
title: Linux Command CheatSheet
date: 2018-05-28 02:33:42
tags: linux, ubuntu
---

# Permission

- List all groups

  `id -nG`

  

- Add one username to the user group

  `sudo usermod -aG docker username`

  

- Check permission

  `getfacl /var/www/html/`

  

- Add permission

  Just add the -R option to recursively change the permissions of files. An example, recursively add read and write permissions for the owner and group on foldername.

  `chmod -R ug+rw foldername`

# Directory

- Get current directory

  `pwd`

- Go to user directory

  'cd ~'

- Go to previous directory

  'cd -'

# Process

- Check processes that are using specific port

  `sudo fuser 5000/tcp -k`

  

- Get Process and its user

  `ps -aux |grep [servicename]`

  

- Control the system services

  `sudo systemctl status [servicename]`

  `sudo systemctl restart [servicename]`

- Windows Kill Process

  *Step one:*

  `netstat -ano | findstr :8080`

  *Step two:*

  `taskkill /PID typeyourPIDhere /F`

  (`/F` forcefully terminates the process)

