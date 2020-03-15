# Tricks 

### Bang Bang:
* Used to execute the perviously executed command we can enter **>** ```!!``` **<**
```console
kali@kali:~/Documents$ pwd
/home/kali/Documents
kali@kali:~/Documents$ !!
pwd
/home/kali/Documents
```
* To run using root access just add sudo with ```!!```
```console
kali@kali:~/Documents$ sudo !!
```

### Cut and Yank:
```console
Ctrl+k					---	Cut Command from cursor to end 
Ctrl+u					---	Cut the Line from the cursor to the beginning of line
```

### Application of Cut and Yank:
* Suppose you extered an command and you forgot to add something at the 
	the beginning of line, in this case-
```console
	Ctrl+u
	<add your line>
	Ctrl+y
```
