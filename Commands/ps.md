# ps:
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
