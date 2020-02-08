# Basic Linux Commands

### ls:
  * ##### 'ls' command can be used to display all the files present in a current directory

  ```console
  ubuntu-VirtualBox:~$ ls
  Desktop  Documents  Downloads  Music  Pictures  Public  snap  Templates  Videos
  ```
  ###### NOTE : '-a' option is used to display all the hidden file
  ```console
  ubuntu-VirtualBox:~$ ls -a                                  
  Desktop        Documents   .install4j     Pictures   snap                       .vboxclient-display.pid
  Downloads      .java       .pki           .ssh       .vboxclient-draganddrop.pid
  .bash_history  .cache      .gnome         .local     .profile         .sudo_as_admin_successful  .vboxclient-seamless.pi

  ```

### cd:
  * ##### 'cd' command can be used to go a specific directory

  ```console
  ubuntu-VirtualBox:~$ cd Desktop
  ubuntu-VirtualBox:~/Desktop$
  ```  
  ###### NOTE : '..' is used to go back to the previous directory
  ```console
  ubuntu-VirtualBox:~/Desktop$ cd ..                           
  ubuntu-VirtualBox:~$ 
  ```
  ###### NOTE : you can enter a path to move to that specific directory
  ```console
  ubuntu-VirtualBox:~$ cd Documents/"Visual Studio Code"/Python    
  ubuntu-VirtualBox:~/Documents/Visual Studio Code/Python$ 
  ```
  
### mkdir & rmdir:
  * ##### 'mkdir' command can we used to make a directory and 'rmdir'command can be used to delete a empty directory

  ```console
  ubuntu-VirtualBox:~/Desktop$ mkdir commands
  ubuntu-VirtualBox:~/Desktop$ ls
  commands
  ubuntu-VirtualBox:~/Desktop$ mkdir folder
  ubuntu-VirtualBox:~/Desktop$ ls
  commands  folder
  ```
  ###### NOTE : We can delete only those folders which are empty using rmdir 
  ```console
  ubuntu-VirtualBox:~/Desktop$ cd folder
  ubuntu-VirtualBox:~/Desktop/folder$ mkdir folder2
  ubuntu-VirtualBox:~/Desktop/folder$ cd ..
  ```
  ###### NOTE : When we try to delete an non-empty folder using rmdir it raises an errror messgae
  ```console
  ubuntu-VirtualBox:~/Desktop$ rmdir folder
  rmdir: failed to remove 'folder': Directory not empty
  ```
  ###### NOTE : Once all the contains of the folder is deleted then we can execute the 'rmdir' command to delete the folder
  ```console
  ubuntu-VirtualBox:~/Desktop$ cd folder
  ubuntu-VirtualBox:~/Desktop/folder$ rmdir folder2
  ubuntu-VirtualBox:~/Desktop/folder$ cd ..
  ubuntu-VirtualBox:~/Desktop$ rmdir folder
  ubuntu-VirtualBox:~/Desktop$ ls
  commands
  ubuntu-VirtualBox:~/Desktop$ 
  
  ```

### rn:
  * ##### 'rn' command can be used to remove files and directories
  
  ```console
  ubuntu-VirtualBox:~/Desktop$ ls
  folder1  folder2  trial.txt
  ubuntu-VirtualBox:~/Desktop$ rm trial.txt
  ubuntu-VirtualBox:~/Desktop$ ls
  folder1  folder2
  ```
  ###### NOTE: '-r' option is used to delete directories including non empty directories
  ```console
  ubuntu-VirtualBox:~/Desktop$ rm -r folder2  
  ubuntu-VirtualBox:~/Desktop$ ls
  folder1
  ubuntu-VirtualBox:~/Desktop$
  ```
 
### echo:
 * ##### 'echo' command can be used to display line of text/string. 
 * ##### 'echo' can also be used initialize variables and display output or store output in a file
 
 ###### NOTE: 'echo' can be used to display our default interpreter
 ```console
 fiesta@fiesta-VirtualBox:~/Downloads$ echo $SHELL
 /bin/bash
 ```
 

