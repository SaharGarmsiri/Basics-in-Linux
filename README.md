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

Listing everything in the current directory

**ls -l**  --> Displaying files/directories along with their owners and permissions and more

**ls -a** --> Displaying files/directories along hidden ones

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

Making a folder

# rmdir

Removing an **empty** folder 

# rm -rf

Removing a **full** folder

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
