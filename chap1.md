# 1 - Getting started with the basics

## Introductory terms and concepts
**1. Binaries** refers to files that can be executed (tệp được thực thi). Binaries generally reside (nằm ở) in he */usr/bin* or *usr/sbin* directory.

**2. Case sensitivity** This mean that *Desktop* is different from *desktop*.

**3. Directory** This is same as a folder in Windows.

**4. Home** Each user has their own/home directory.

**5. root** This is an administrator or superuser in Linux. root can do such things as reconfiguring the system, adding users and changing password.

**6. Terminal** command line interface (CLI)

___
## The Linux Filesystem
Very top of the filesystem structure is /, the root of the filesystem, but it's different from the root user. 

![image](https://github.com/user-attachments/assets/1c5f7b48-a660-4b54-85ee-ae55f386efcf)

The root (/) of the filesystem is at the top of the tree, and the following are the most important subdirectories to know:
**/root** The home directory of the all-powerful root user

**/etc** contaisn the Linux configuration files - files that control when and how programs start up.

**/home** the user's home directory

**/mnt** where other filesystem are attached and mounted to the filesystem

**/media** where CDs and USB devices are atteched and mounted the filesystem

**/bin** where application binaries reside

**/lib** where app;ication binaries

## Basic command on Linux
1. pwd: to see where are you
2. whoami: checking your login

## Navigating the Linux Filesystem (điều hướng)
1. cd: changing directories
   cd .. : move up 1 level
   cd .. .. : move up 2 levels
   cd .. .. .. : move up 3 levels and so on
   cd / : move up the root level

2. ls: listing the contents of directory
   ls -l : long listing to get more informations such as permissions, owner, size and when they were last modified
   ls -a : to see hidden file

3. --help / -h / -? : getting help

4. man *command,utility,app* : for more information

## Finding stuff
1. locate *name* : go through your entire information and locate every occurrence of that word.
   => overwhelming, too much information. And *locate* uses a database is usually only updated once a day.
   => just created file a few minutues? it might not appear in this list.

2. whereis *name*: find binaries file.

3. which *name*: finding binaries file in the PATH Variable

4. find *directory options expression*
  > search for file with the name apache2, starting in the root directory

  >find / -type f -name apache2

5. grep *keyword* : often used when output is piped from one command to another, this is called *piping*, use the command |

    > ps aux | grep apache2 : listing all my services and then send that output to grep, look through the output for *apache2*

## Modifying Files and Directories (thay đổi)

### Creating files
1. cat > *filename* : overwrite the file
   
   > cat > hackingskills : when you eneter, you go to interactive mode and wait for you to start entering content for the file.

2. cat >> *filename* : to add, append more content to a file.

3. touch *filename* : create newfile

4. mkdir *directoryname* : create new directory

5. cp *filename* *directory* : copying a file
   > cp oldfile /root/newdirectory/newfile : copy and rename

6. mv *oldname* *newname* : renaming a file

7. rm *filename*: removing a file

8. rmdir *directoryname* : removing a directory and you can just remove a driectory when it's empty
