# Linux File System

* Linux File System or any file system generally is a layer which is under the operating system that handles the positioning of your data on the storage, without it; the system cannot knows which file starts from where and ends where.
* The directories have specific purposes and generally hold the same types of information for easily locating files. 

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

##### -> Terminal : Shortcut to open terminal ``` CTRL + ALT + T```

### Navigating the File System : 
* Now that you understand the basics of the file system, you can begin navigating to the files you need. The following commands are used to navigate the system

|Commands|Description|
|--|--|
|```cat```|concatenate files and print on the standard output|
|```cd```|change the working directory|
|```cp```|copy files and directories to the specified location|
|```file```|determine file type, for example (binary, text, etc)|
|```find```|search for files in a directory hierarchy|
|```head```|output the beginning part of files|
|```tail```|output the last part of files|
|```less```|browses through a file from the end or the beginning|	
|```ls```|list specified directory contents|
|```mkdir```|creates the specified directory|
|```more```|browses through a file from the beginning to the end|
|```mv```|moves the location of, or renames a file/directory|
|```pwd```|print name of current/working directory|
|```rm```|remove files or directories|
|```rmdir```|removes a directory|
|```touch```|creates a blank file or modifies an existing file or its attributes| 	
|```whereis```| output all the location of a file or directory|
|```which```|output the location of a directory if it is in your PATH|

