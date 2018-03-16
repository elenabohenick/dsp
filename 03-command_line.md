# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > * pwd - shows current working directory path
> > * mkdir directoryname - creates new directory called directoryname
> > * rm -r directoryname - removes directory called direcoryname and all of its child directories
> > * touch filename.txt - crates a *.txt file called filename
> > * rm filename - deletes a file called filename
> > * mv filename_old.txt filename_new.txt - changes filename from filename_old to filename_new
> > * ls -a - list all files in the working directory including hidden files
> > * cp filename directoryname/ - copies files from current directory to satated direcoty
> > * grep "line" filename.txt - searches for lines that match "line" in filename.txt
> > * cat file1 >> file2 - takes the standard output of the file1 and appends it to the file2 

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls` - lists all files in the working direcotry	  
`ls -a` - list all files incuding hidden in the working directory	
`ls -l` - list all contents of the working directory in the longform format	
`ls -lh` - list files with sizez in human readable format   
`ls -lah` - list all files including hiddnet in the longform with sizer shown in human readable format (combination of t\
hree options l a h )  
`ls -t` - sorts files by modification time showing last edited files first	
`ls -Glp` - list files in the longform with the owner omitted and '/' after each filename	  


---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 'ls -c' displays files by file timestamp
> > 'ls -d' displays directories only
> > 'ls -t' displays newest files first
> > 'ls -F' flags filenames
> > 'ls -R' displays subdirectories in addition to directories

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 'xargs' creates and execures commands from standard intput and can parallel process jobs. 

 

