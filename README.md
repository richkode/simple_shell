# Simple Shell

### Introduction
This repository is an Alx Project. The project is to allow students understand how the linux shell works and operates. Students are to code a similar shell using the c programming language with limited builin c functions. We as students are suppose to build and use our own custom functions in most cases to help us in this project. 

## Required Features
* cd [path/directory]
* exit [status]
* env
* echo [$$] or [$?] or [$PATH]
* setenv NAME VALUE
* unsetenv NAME
* help [command]

## Usage 
In order to run this program, clone this repository.

compile it with  

`gcc 4.8.4 -Wall -Werror -Wextra -pedantic *.c -o hsh`.  
You can then run it by invoking `./hsh` in that same directory.  
 
It wil then display a simple prompt and wait for commands.  
`$ `   
A command will be of the type `$ command`  

## Examples Command
**Example 1**
```
Username@your-regular-prompt:~$ ./hsh
$ pwd
/home/username/
$ ^D
Username@your-regular-prompt:~$
```
**Example 2**
```
Username@your-regular-prompt:~$ ./hsh
$ ls -l /tmp 
-rw------- 1 username username    0 Dec  5 12:09 config-err-aAMZrR
drwx------ 3 root   root   4096 Dec  5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-colord.service-V7DUzr
drwx------ 3 root   root   4096 Dec  5 12:09 systemd-private-062a0eca7f2a44349733e78cb4abdff4-rtkit-daemon.service-ANGvoV
drwx------ 3 root   root   4096 Dec  5 12:07 systemd-private-062a0eca7f2a44349733e78cb4abdff4-systemd-timesyncd.service-CdXUtH
-rw-rw-r-- 1 username username    0 Dec  5 12:09 unity_support_test.0
$ ^D
Username@your-regular-prompt:~$
```
### Exmples Builtin

**case env and exit**
```
Username@your-regular-prompt:~$ ./hsh
USER=julien
LANGUAGE=en_US
SESSION=ubuntu
COMPIZ_CONFIG_PROFILE=ubuntu
SHLVL=1
HOME=/home/julien
C_IS=Fun_:)
DESKTOP_SESSION=ubuntu
LOGNAME=julien
TERM=xterm-256color
PATH=/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
DISPLAY=:0
$ exit
Username@your-regular-prompt:~$ 

```
**Case Exit Statue**
```
Username@your-regular-prompt:~$ ./hsh
$ exit 98
Username@your-regular-prompt:~$ echo $?
98
Username@your-regular-prompt:~$

```
Keep Exploring The echo Builtin and history ... Using The Help Builtin

### Also
* Handle Ctrl+C: your shell should not quit when the user inputs ^C
* If no argument is given to cd the command must be interpreted like cd $HOME
* handle the command cd -
* Handle variables replacement
* Handle the $? variable
* Handle the $$ variable
* Handle The Argument file like `./hsh test` Where test is a file filled with command and builtin to excute.
### List of functions and system calls we could use
List of allowed functions and system calls

    access (man 2 access)
    chdir (man 2 chdir)
    close (man 2 close)
    closedir (man 3 closedir)
    execve (man 2 execve)
    exit (man 3 exit)
    fork (man 2 fork)
    free (man 3 free)
    fstat (man 2 fstat)
    getcwd (man 3 getcwd)
    getline (man 3 getline)
    kill (man 2 kill)
    lstat (man 2 lstat)
    malloc (man 3 malloc)
    open (man 2 open)
    opendir (man 3 opendir)
    perror (man 3 perror)
    read (man 2 read)
    readdir (man 3 readdir)
    signal (man 2 signal)
    stat (man 2 stat)
    strtok (man 3 strtok)
    wait (man 2 wait)
    waitpid (man 2 waitpid)
    wait3 (man 2 wait3)
    wait4 (man 2 wait4)
    write (man 2 write)
    _exit (man 2 _exit)

## Authors
* Tweneboanah Richmond
* God'slove God'slove 
