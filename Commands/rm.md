# rm:
  * ##### 'rm' command can be used to remove files and directories
  
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
