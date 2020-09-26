##### linux_commands.md

# Linux commands for Linux Sysadmins
---
### Navigation

`pwd`
#### Print Working Directory

`ls`
#### List the files in the working directory

`cd`
#### To change directory
#### Example uses:
`cd /usr/bin`
#### or
`cd ..`
#### or
`cd ./bin`
#### (this is the same as cd bin)
---
### Viewing directories and files
`ls`
#### list the files in the working directory
`ls -a`
#### list all files in the working directory, including hidden files
`less my_file`
#### less will let you view text files
#### once the text file is opened in less, you can use the following to controll the file
#### Page Up or Down to scroll back or forward one page
#### G to go to the end of the text file
#### 1G to go to the beginning of the text file
#### /characters to search forward in the text document for your specified characters
#### n to repeat the previous search
#### h to display the complete list of less commands and options
#### q to quit the less utility
`file`
#### File lets you examine a file and determines what type of file it is
`file my_file`
#### this command will tell you what type of file the 'my_file' is
---
### Manipulating Files
`cp`
#### Use 'cp' to copy files and directories
`mv`
#### Use 'mv' to move or rename files and directories
`rm`
#### Use 'rm' to remove files and directories
`touch`
#### Use 'touch'to create a file
`mkdir`
#### Use 'mkdir' to create direcories

`mkdir --help`
#### Use this to get the 'help' option of the mkdir command
#### This will also work for other commands as well - example 'touch --help'

`man`
#### The man command is used to view manuals, or a formal documentation on said command
#### Example usage:  'man ls'
#### This will produce the documentation on the 'ls' command (ls is the list directory command)

`> file_list.txt`
#### Output to a txt file.  Example: ls > file_list.txt
#### Run the same command again and it will overwrite to the txt file
#### To append results to the file, use the following:  ls >> file_list.txt

#### Standard Input
`sort < my_text_file.txt`
#### This will sort the contents of the file you pointed to using the '<'
#### And output it in the terminal

#### You can also output it to a new txt file as shown below:
`sort < my_text_file.txt > my_new_sorted_file.txt`

#### Pipeline - this can be used to connect multiple commands together as shown below:
`ls -lt | head`
#### This will show the 10 newest files in the directory which it is run in

`du | sort -nr`
#### Will show a list of directories, directory size and sort them from largest to smallest
---
---

### Common Filter Commands
`sort`
#### Sorts standard input then outputs the sorted result to standard output

`uniq`
#### Given a sorted stream of data, it removes duplicate lines of data (makes sure it is all unique)

`grep`
#### Takes a line of data from standard input and outputs lines that contain specified pattern

`fmt`
#### Takes text from standard input, outputs formatted text via standard output

`pr`
#### Takes standard input,splits the data into pages with breaks, headers and footers for printing

`head`
#### Will output the first several lines of the file used as its argument

`tail`
#### will output the last severa lines of the file used as its argument

`tr`
#### Translate characters.  Use to uppercase / lowercase conversion

---
---
#### Print directly from the command line:
#### Use `lpr`
#### `lpr` takes standard input and sends it to the printer
#### Example:

`cat my_text_file.txt | sort | uniq | pr | lpr`

#### cat sends the txt file to sort wich sorts it and feeds it to
#### uniq which will remove any duplicates. pr & lpr paginate and print the list

---
---
### Permissions

`chmod` 
#### Used to change permissions to a file or directory

`su`
#### Used to temporarily become a superuser

`sudo`
#### Also used to temporarily become a superuser

`chown`
#### Used to change file ownership

`chgrp`
#### Used to change a file's group owner
----
----

`echo *`
#### This will list all files in the current directory (similar to the ls command)

`echo ~`
#### This will list all files / directories in the home folder


---
---
### System Info

`users`
#### This will list the current users logged onto a system

`uptime`
#### This will list the current systems up time


---
#### List and show all IP addresses associated with all network interfaces:
#### This is the same as:
`ip address show`
#### Which is the long form - below is the short form:
`ip a`

