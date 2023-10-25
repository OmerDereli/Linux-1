# Linux-1
# Introduction of linux basic commands

# File and Directory Manipulation:
1-Create a directory named "my_homework" in your home directory.

```
$ mkdir my_homework
```

2-Inside "my_homework," create three subdirectories: "docs," "pictures," and "code."
```
$ mkdir my_homework/Docs
$ mkdir my_homework/Pictures
$ mkdir my_homework/Code
```

3-Create a text file named "todo.txt" inside "docs" and write a list of tasks for the week.
```
$ cat > myhomework/docs/todo.txt
#Now it wants you to write inside todo.txt aftery you finish writing press CTRL + D to exit
```
4-Move an image file from your downloads folder to the "pictures" directory.
```
$ mv /home/omer/Downloads/cat.png /home/omer/my_homework/pictures/ #You need to write location correctly for this you can right click on folder then look parent folder.
```
5-Use the "ls" and "cd" commands to navigate through the directories you've created.
```
$ ls

 123.sh           b_bio.txt      Documents      my_bio2.txt     Pictures    todo2.txt
 backup           denemefolder   Downloads      my_homework     Public      txtfiles
 backup_bio.txt   deneme.txt     logfiles.txt   mylogfile.txt   snap        Videos
 backup.sh        Desktop        Music          notlar          Templates  'VirtualBox VMs'

$ cd my_homework
$ ls

 Code   Docs   Pictures

```
6-Take a screenshot of your directory structure and save it in the "pictures" directory.

--------------------------------------------------------------------------------------

--------------------------------------------------------------------------------------

# Text File Manipulation:

1-Create a text file called "bio.txt" using a text editor (e.g., Nano or Vim).
```
$ nano bio.txt
```

2-Write a short biography about yourself in the "bio.txt" file.
```
#after commending nano it will open text editor write there.
```

3-Use command-line tools like "cat," "head," and "tail" to view the contents of the file.

```
$ cat bio.txt
$ head bio.txt
$ tail -3 bio.txt #"-3" represent the last 3 lines of bio.txt
```

4-Use the "cp" command to make a backup copy of the "bio.txt" file.
```
$ cp -b my_bio.txt backup_bio.txt # -b represent backup
```

5-Use the "mv" command to rename the original file to "my_bio.txt."
```
$ mv my_bio.txt my_bio2.txt
```
--------------------------------------------------------------------------------------

--------------------------------------------------------------------------------------

# User and Permissions:

1-Create a new user account with a unique username (e.g., "student") using the "sudo" command.
```
$ sudo adduser student
```

2-Switch to the newly created user account using the "su" or "sudo su" command.
```
$ sudo su deniz
```

3-Create a new directory in this user's home directory and try to write a file in it.
```
$ mkdir deneme
$ echo "Lorem ipsum" > deneme/file.txt
```

4-Use the "chmod" command to change permissions on the directory to allow writing.
```
$ chmod 777 file.txt 
```

5-Try writing the file again and observe the difference in permissions.

--------------------------------------------------------------------------------------

--------------------------------------------------------------------------------------

# Package Management:

1-Install a new software package of your choice using your Linux distribution's package manager (e.g., "apt" for Debian/Ubuntu, "yum" for CentOS, or "dnf" for Fedora).
```
# sudo apt install htop # example usage of apt
```
2-Update the package list to ensure you have the latest information about available packages.
```
$ apt --upgradable
```
Check if the installed package has any available updates.
```
$ apt-cache policy google-chrome-stable
```
Use the package manager to upgrade the installed package to the latest version.
```
$ sudo apt-get install --only-upgrade nano
```
--------------------------------------------------------------------------------------

--------------------------------------------------------------------------------------

# Basic Scripting:

Create a simple Bash script named "greet.sh" that prints a personalized greeting message based on user input (e.g., "Hello, John!").
Make the script executable using the "chmod" command.
Run the script and test it with different names.
Modify the scri
pt to accept the user's name as a command-line argument rather than prompting for input.

```
#!/bin/bash

name="$1"
echo "Hello, $name!"
```




























