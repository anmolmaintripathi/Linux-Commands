# cat:
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
