# Most Used Commands In Linux
Here are some useful commands that you should learn in Linux
___

# man

Help for Commands

# pwd

Displaying your current path

# whoami
Displaying your current user

# ls

Listing everything in the directory

**ls -l**  --> Displaying files/directories along with their owners and permissions and more

**ls -a** --> Displaying files/directories along hidden ones

**ls [Path]** --> Specifying a path for it

# clear

Clear terminal

# cd

Change directory

**cd /** --> Going to root file system

**cd /usr/bin** --> Going to a particular path (you can put any path you want)

**cd ..** --> Going to the previous directory

# touch

Create a file

**touch file.txt new.pdf** --> Create multiple files in one line

**touch lino{1,2}** --> Create files lino1 and lino2

**touch lino{3..5}** --> Create files lino3 to lino5

**touch -d tomorrow file.txt** --> Specifying a time for creating file

# rm
Removing a file

# mkdir

Making a directory

# rmdir

Removing an **empty** directory 

# rm -rf

Removing a **full** directory

# cp 

Copy a file/directory

**cp file.txt  /home/admin/Documents** --> You should first specify **source path** then **destination path**

# mv
Cut a file/directory

**mv file.txt  /home/admin/Documents** --> You should first specify **source path** then **destination path**

# touch

Calling a file/txt/...

**echo file.txt**

**echo "Stuff Stuff" > file.txt** --> puting what's bitween " " insted of file.txt past content

# nano

One of the linux editors

Ctr+x , y , Enter --> Geting out of editor

# vim

One of the linux editors

**Shift+: , q!** --> Geting out of editor (without changes)

**Shift+: , wq** --> Geting out of editor (withchanges)

# cat

A quick look in a file

**cat file.txt**

# shred

Making inside of a file unreadable

**shred file.txt**

# su

Switching between users

Note: In all the command below, if you leave [usranme] empty, it will apply ti the **root** user

**su [usranme]**

**su [usranme]** --> switch to [usranme] without changing environment

**su - [usranme]** --> switch to [usranme] as if logging in as the new user from the start

# adduser

Adding a new user

**sudo adduser [usranme]**

# deluser

Deleting user

**sudo deluser --remove-home [usranme]** --> Removing user and their home directory

# finger

Quick inspection of a user

**finger [usranme]**

# whatis

Quick guide for command

# which

The place of commands

# whereis 

All the places od commands

# wget

Download something frome internet

 **wget [Link]**

 # curl

Download something frome internet and specifide a path and name for it

**curl  [path+filename] [link]** -->  curl /home/user/Documents/image.jpg https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4dmsYSNKQTnRVt7kHvDyqI_3qZmTc6Ei68w&s

# zip / unzip

 To compress/extraction files

 **zip [zip file name.zip] [target file]**
 
 **unzip file.zip**

# less

Viewing files page by page

# head

Viewing head of the files

# tail

Viewing end of the files

#cmp

Comparing 2 file to see if thay are different or not

    cmp [file-1] [file-2]

# diff

Viewing the differences between 2 files

    diff [file-1] [file-2]

# sort

Sorting content base on alphabet

**cat [file.txt] | sort**

# find

Finding a file

**find [path-you can use / for anywhere] -name "file.txt"**

**find [path-you can use / for anywhere] -type f -name "."** --> Finding all the hidden files

**find [path-you can use / for anywhere] -type f -empty** --> Finding all the empty directories

# chown

Chainging the ownership of files

**chown [new user owner] file.txt**

# ip a / ip address

Viewing system IPs

some common outputs you get:

**inet->IPv4   /  inet6->IPv6  /  eth0->Cable internet  /  vlan0->WiFi**

**ip address | grep [interface]** --> Only viewing [interface] information

# ping

Routing test

**ping -c [number of pings] 8.8.8.8** --> ping -c 5 8.8.8.8
    
**ping -c [number of pings] -s [number of packes to sent] google.com** --> ping -c 5 -s 500 google.com

# netstat

Open ports in systems

(you can install it with the following command:)

    sudo apt update
    
    sudo apt install net-tools

**Option Description:**

-a --> Show all connections (listening and non-listening)

-t --> Show TCP connections

-u --> Show UDP connections

-l --> Show only listening sockets 

-n --> Show numeric addresses (no DNS resolution)

-p --> Show PID and program name

-r --> Show the routing table

-s --> Show statistics by protocol

-i --> Show network interface statistics

-c --> Continuously update the output

# uname

Tell you about your systemse

uname -a --> Tell you more

# neofetch

Tell you about your systemse (in a fancy wey)

# free

Display amount of free and used memory in the system

# df 

report file system space usage

**df -H** --> print sizes in GB

# ps

report a snapshot of the current processes

**ps -d** --> Viewing all the active process  

# top

display Linux processes 

# htop

display Linux processes (in a fancy wey)

# kill

Killing a process

     kill -9 [PID]
  
for killing a process, you have to know there PID; you can find it here:

     ps -aux | grep [process name]


# pkill 

Killing a process (no need a PID)

     pkill -f [process name]

# history

History of all the commands

# reboot 

      sudo reboot

# shutdown   
      sudo shutdown -h now
