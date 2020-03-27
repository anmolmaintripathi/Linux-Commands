# mkdir & rmdir:
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
