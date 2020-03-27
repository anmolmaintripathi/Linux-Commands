# ls:
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
