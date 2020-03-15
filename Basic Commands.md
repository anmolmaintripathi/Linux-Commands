# Basic Linux Commands

### pwd:
* 'pwd' commands stands for print working directory
```console
kali@kali:~/Desktop/folder$ pwd
/home/kali/Desktop/folder
```
* The command line also displays the working directory. [important]
```console
kali@kali:~/Desktop/folder$
	    \-----|------/
	    	  |
	    this is the path in which the terminal is working.
```

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
  ###### NOTE : '-l' option is used to display all the number of folders in the current directory and details of each files and folders
  ```console
  fiesta@fiesta-VirtualBox:~$ ls -l
 total 48
 drwxr-xr-x 2 fiesta fiesta 4096 Feb  8 22:30 Desktop
 drwxr-xr-x 3 fiesta fiesta 4096 Feb  7 20:29 Documents
 drwxr-xr-x 2 fiesta fiesta 4096 Feb  8 22:47 Downloads
 ....
  ```
  ###### NOTE : Some other important options 
  ```console
ls -F					---	list files with their types
ls -R					---	list files recursively
ls -R /					---	List all files on system
ls -lR					---	list all files recursively with verbous information
ls -a					---	list all files includng hidden one
ls --color				---	list files in color
ls -lS					---	Sort by size [larger size on top]
ls -lSr					---	sort by size [smaller size on top]
  ```
  
  ###### NOTE : "tree" command is used to display the tree graph of all directories
  ```console
  tree					---	tree of all files from current directory
  tree	~				---	tree of all files from the root
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

### rm:
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
 
### echo:
 * ##### 'echo' command can be used to display line of text/string. 
 * ##### 'echo' can also be used display output.
 
 ###### NOTE: 'echo' can be used to display our default interpreter
 ```console
 fiesta@fiesta-VirtualBox:~$ echo $SHELL
 /bin/bash
 ```
 
### touch:
 * ##### 'touch' command is used to create any kind of files
 ```console
 fiesta@fiesta-VirtualBox:~$ cd Desktop
 fiesta@fiesta-VirtualBox:~/Desktop$ ls -l
 total 0
 fiesta@fiesta-VirtualBox:~/Desktop$ touch trail.txt
 fiesta@fiesta-VirtualBox:~/Desktop$ ls -l
 total 0
 -rw-r--r-- 1 fiesta fiesta 0 Feb  9 01:31 trail.txt
 fiesta@fiesta-VirtualBox:~/Desktop$ ls
 trail.txt
 fiesta@fiesta-VirtualBox:~/Desktop$ 
 ```
 
### cat:
 * ##### 'cat' command can be used to read a file and display the contains of the file.
 * ##### It can also used to concatenate two different files.
 ###### NOTE: assume there exist a file called "trial.txt"
 ```console
 fiesta@fiesta-VirtualBox:~/Desktop$ cat trial.txt
 this is the first line of the file
 fiesta@fiesta-VirtualBox:~/Desktop$
 ```
 ###### NOTE: ">>" operator can be used to append values into a existing file. (`Ctrl + D` can be used to end the file)
 ```console 
 fiesta@fiesta-VirtualBox:~/Desktop$ cat trial.txt
 this is the first line of the file
 fiesta@fiesta-VirtualBox:~/Desktop$ cat >> trial.txt
 this is the second line of the life
 fiesta@fiesta-VirtualBox:~/Desktop$ cat trial.txt
 this is the first line of the file
 this is the second line of the life
 fiesta@fiesta-VirtualBox:~/Desktop$
 ```
 ###### NOTE: ">" operator can be used to replace the contains of the file. 
 ```console
 fiesta@fiesta-VirtualBox:~/Desktop$ cat trial.txt
 this is the first line of the file
 this is the second line of the life
 fiesta@fiesta-VirtualBox:~/Desktop$ cat > trial.txt
 this will replace all the exsiting values in the file.
 fiesta@fiesta-VirtualBox:~/Desktop$ cat trial.txt
 this will replace all the exsiting values in the file.
 fiesta@fiesta-VirtualBox:~/Desktop$ 
 ```
 
 ###### NOTE: 'cat' command can  be used to combine the contains of different files and add it to a new file
 ```console
 fiesta@fiesta-VirtualBox:~/Desktop$ cat>file1.txt
 file 1         
 fiesta@fiesta-VirtualBox:~/Desktop$ cat>file2.txt
 file 2
 fiesta@fiesta-VirtualBox:~/Desktop$ cat file1.txt file 2.txt > file3.txt
 cat: file: No such file or directory
 cat: 2.txt: No such file or directory
 fiesta@fiesta-VirtualBox:~/Desktop$ cat file1.txt file2.txt > file3.txt
 fiesta@fiesta-VirtualBox:~/Desktop$ cat file3.txt
 file 1
 file 2
 fiesta@fiesta-VirtualBox:~/Desktop$
 ``` 
 
### cp:
* 'cp' is used for coping files and directories.
* Syntax for 'cp' commands
```console
cp filename destination_path

kali@kali:~/Desktop$ cp file1.txt /home/kali/Documents
```


###### NOTE : '-r' option is used to copy directories/folders 
```console
kali@kali:~/Desktop$ cp -r folder /home/kali/Documents
kali@kali:~/Desktop$ cd /home/kali/Documents
kali@kali:~/Documents$ ls
file1.txt  folder
```

### Create Server using Python
 ##### PYTHON SERVER :
* Python can be used to create servers.
* The commands depends on the version of python being used "PYTHON 2 OR PTYHON 3"
	
* For PYTHON 2 

```console 
python –m SimpleHTTPServer
```
* For PYTHON 3
```console
python -m http.server          --- default port number is 8080

python -m http.server 9000     --- changing the port number to 9000
```

* If both the python versions are present in the system try writting "python3" or "python2" along with the command

### ps:
* "ps" stands for Process Status.
* Displays all the different currently-running processes. 
###### NOTE : The default format of ps is " [Process Id]  [tty: Teletypewriter]  [Run Time]  [Terminal Type]
```console
kali@kali:~$ ps
PID TTY          TIME CMD
2852 pts/0    00:00:00 bash
2855 pts/0    00:00:00 ps
```

###### NOTE : '-p' option can be used to display a specific command
```console
kali@kali:~$ ps -p 2852
    PID TTY          TIME CMD
   2852 pts/0    00:00:00 bash
```

###### NOTE : other important options
```console
ps -u 						--- 	list for all users
ps aux						---	list all processes including system processes
ps aux | less					---	list all processes and pipe them to less command
top 						---	show continually updated processes list 
```



