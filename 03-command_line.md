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

pwd: show current directory path
mkdir <name(s)>: create a directory
rmdir <name(s)>: delete a directory
touch <name(s)>: create a file (http://www.linfo.org/touch.html)
rm <name(s)>: delete a file
mv -i <oldname> <newname>: move a file
ls -a (all files), or ls -ld .*? (only hidden): output hidden files
cp -i <file> <newpath/newfile>: copy a file
cd <dir>: change current directory
cat <name>: output text file 




---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

ls: output the contents of the current directory (except hidden)  
ls -a: all files (including hidden)  
ls -l: long version (with permissions, number of children directories, file owner, owner group, last modified)  
ls -lh: long with file size  
ls -lah: all files, long, with file size  
ls -t: sort by time/date  
ls -Glp: uses colors to highlight (-G) long file types (-l), and sticks a '/' at the end of directories (-p) 



---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:


ls -R: Because it was hilarious when I used it on my root 

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs allows you to pipe standard input even to procedures (including rm, mkdir) that can't normally take stdin by converting them the stdin(s) into arguement(s). Moreover, some procedures can only accept a limited number of arguments; xargs applies the procedure to all the arguments you give it.

find /Users/ilanmoscovitz/documents | xargs rm
shred each of my documents

 

