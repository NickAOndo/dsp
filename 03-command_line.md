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

> >  list contents: ls (with -l for information, -a to include hidden, -t to order by most recently updated)

> > move to directory: cd sub_directory (or cd .. to go up the directory tree)

> > current directory: pwd

> > create directory: mkdir new_directory

> > remove directory: rmdir old_directory

> > move file: mv some_space_separated_list_of_files their_new_directory

> > create text file: touch new_file.txt

> > delete file: rm unimportant_file.txt

> > search document for string match: grep file_to_be_searched.txt

> > rename file:  mv old_file_name new_file_name

> > read text file:  cat text_file.txt

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

> > The command `ls` lists the contents of the current directory

> > The `-a` argument displays all files, including hidden files (i.e. those beginning with a .)

> > The `-l` argument displays all of the information (size, date modified, access, etc)

> > The `-h` argument displays all of the information, but bytes are given prefixes (K=kilo, M=mega, etc) for readability.

> > The `-lah` argument displays detailed info with human-readable sizes and includes hidden files. (Merges lh and a 
functionality.)

> > The `-t` orders the result in terms of which was most recently modified to the least recently modified

> > The `-p` makes directories come with a `/` at the end and `-G` removes grouping for long lists.

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > a is useful for seeing hidden files and folders
> > c is useful for looking at the date information
> > R is useful for looking at subdirectories
> > g is useful to remove clutter of the owner name alongside -l
> > l is useful for seeing all of the information

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` allows us to apply functions to a list of outputs, e.g. suppose we want to remove all directories that contain the name `apple`, we could perform `ls | grep apple | xargs rmdir` which would grab the contents of the directory, grab all entries with `apple` in the name, and then remove them one-by-one.

 

