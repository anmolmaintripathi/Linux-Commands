# Linux File System

* Linux File System or any file system generally is a layer which is under the operating system that handles the positioning of your data on the storage, without it; the system cannot knows which file starts from where and ends where.

| Directory | Meaning |
|--|--|
| /| Root directory, which contains only the files needed at the top level of the file structure| 
| /bin | All the executable files are located in this directory |
| /dev | These are devices drivers, which acts as a translator between hardware and the programs or OS|
| /dev | Contains devices drivers |
| /etc | Supervisor directory commands, configuration files, disk configuration files, valid user lists, groups, ethernet, hosts, where to send critical messages and much more|
| /lib | Contains shared library files and sometimes other kernel-related files |
|/boot| Contains files for booting the system|
| /home|Contains the home directory for users and other accounts|
|/mnt|Used to mount other temporary file systems, such as cdrom for the CD-ROM drive, respectively|
|/proc|Contains all processes marked as a file by process number or other information that is dynamic to the system|
|/tmp|Holds temporary files used between system boots|
|/usr|Used for miscellaneous purposes, and can be used by many users. Includes administrative commands, shared files, library files, and others. This folder is named after the name of your Device name|
|/kernel|Contains kernel files|

* In the following picture using the ```ls``` command (which is used to display all the directories and files) we can see all the files under root.

![Files under root](https://user-images.githubusercontent.com/45136496/77253553-0d6c3e00-6c81-11ea-8f61-98edb0f6c832.png)
