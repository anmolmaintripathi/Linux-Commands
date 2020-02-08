# 'sudo' Command
  * sudo allows a permitted user to execute a command as the superuser or another user.
  
### Root access using 'sudo' command:
  * using option '-s'  
    ```console
    fiesta@fiesta-VirtualBox:~/Desktop$ sudo -s
    [sudo] password for fiesta: 
    root@fiesta-VirtualBox:~/Desktop# 
    ```
  * using option '-i' 
    ```console
    fiesta@fiesta-VirtualBox:~$ sudo -i
    [sudo] password for fiesta: 
    root@fiesta-VirtualBox:~#
    ```
  * using sudo su
    ```console
    fiesta@fiesta-VirtualBox:~$ sudo su
    [sudo] password for fiesta: 
    root@fiesta-VirtualBox:/home/fiesta# 
    ```

### Installing '.deb' files using sudo
  1. Download the file and go to the Target folder.
  2. Open the Terminal in the Target folder.
  3. Execute `sudo apt install ./<file_name>.deb`
  
  NOTE: In the following example, we have .deb chrome file from the offical webite,
  ```console
  fiesta@fiesta-VirtualBox:~$ cd Downloads
  fiesta@fiesta-VirtualBox:~/Downloads$ ls
  google-chrome.deb
  fiesta@fiesta-VirtualBox:~/Downloads$ sudo apt install ./google-chrome.deb
  [sudo] password for fiesta: 
  Reading package lists... Done
  Building dependency tree....
  ```
      
