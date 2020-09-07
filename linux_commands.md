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



---

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

