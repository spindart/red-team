



<h1 align="center">
<br>
  Linux commands
  <br>
<img src="./assets/linux.png" alt="Tools" width="200">
</h1>

The most important command in Linux terminal is <strong><a href="#man">man(ual)</a></strong>, record this! 
through this command you get the manual to understand commands and how to use them


## Interacting With the Filesystem

Basic commands to interact with the filesystem

<table>
<tbody>
<tr>
<td>Command</td>
<td>Full Name</td>
<td>Purpose</td>
</tr>
<tr><td>ls</td><td>listing</td><td>List files/directories.</td></tr>
<tr><td>cd</td><td>change directory</td><td>Change current directory.</td></tr>
<tr><td>cat</td><td>concatenate</td><td>Display file contents.</td></tr>
<tr><td>pwd</td><td>print working directory</td><td>Display Current Directory</td></tr>
<tr><td>touch</td><td>touch</td><td>Create file</td></tr>
<tr><td>mkdir</td><td>make directory</td><td>Create a folder</td></tr>
<tr><td>cp</td><td>copy</td><td>Copy a file or folder</td></tr>
<tr><td>mv</td><td>move</td><td>Move a file or folder</td></tr>
<tr><td>rm</td><td>remove</td><td>Remove a file or folder</td></tr>
<tr><td>file</td><td>file</td><td>Determine the type of a file</td></tr>
</tbody>
</table>

## An Introduction to Shell Operators

<table><tbody><tr><td>Symbol / Operator</td><td>Description</td></tr><tr><td>&amp;</td><td>This operator allows you to run commands in the background of your terminal.</td></tr><tr><td>&amp;&amp;</td><td>This operator allows you to combine multiple commands together in one line of your terminal.</td></tr><tr><td>&gt;</td><td>This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere.</td></tr><tr><td>&gt;&gt;</td><td><p>This operator does the same function of the <code>&gt;</code> operator but appends the output rather than replacing (meaning nothing is overwritten).</p></td></tr></tbody></table>

### Operator "&"
This operator allows us to execute commands in the background. For example, let's say we want to copy a large file. This will obviously take quite a long time and will leave us unable to do anything else until the file successfully copies.

The "&" shell operator allows us to execute a command and have it run in the background (such as this file copy) allowing us to do other things!

```bash
sleep 10 & sudo apt update
```

### Operator "&&"
This shell operator is a bit misleading in the sense of how familiar is to its partner "&". Unlike the "&" operator, we can use "&&" to make a list of commands to run for example command1 && command2. However, it's worth noting that command2 will only run if command1 was successful.

<b>Example</b>

```bash
mkdir my_directory && cd my_directory
```

### Operator ">"
This operator is what's known as an output redirector. What this essentially means is that we take the output from a command we run and send that output to somewhere else.

<b>Example</b>

```bash
echo hey > welcome.txt
```

### Operator ">>"
This operator is also an output redirector like in the previous operator (>) we discussed. However, what makes this operator different is that rather than overwriting any contents within a file, for example, it instead just puts the output at the end.

Following on with our previous example where we have the file "welcome" that has the contents of "hey". If were to use echo to add "hello" to the file using the > operator, the file will now only have "hello" and not "hey".

The >> operator allows to append the output to the bottom of the file

```bash
echo hello >> welcome.txt
```

```bash
echo cat welcome.txt
```

OUTPUT:

hey<br>
hello



<hr>

<h1> A-Z commands</h1>


## A

<b>alias</b>

The alias command is simply a way to reference another command. It can be used to avoid repetitive long typing of commands and shell lines and simplify work.

<b>at</b>

The at command in Linux is used to schedule jobs that do not run on a regular schedule.

<b>awk</b>

The AWK command dates back to the early Unix days. Long back before Perl or Python came into existence, AWK was used in scripts for manipulating text. You can use it for writing relatively complex programs, but also because of the powerful one-liners you can write to solve issues with your data files.

## B

<b>basename</b>

The basename command in Linux prints the final component in a file path. This is particularly helpful in bash scripts where you want to extract the file name from the long file path.

## C

<b>cal</b>

Unix-like systems provide a handful of tools for dealing with dates and times. Cal is one such command that enables you to view calendar in the command line.

<b>cat</b>

cat is one of the most used commands in Linux. Intended for concatenating text, it is mainly used for displaying the contents of text files.

<b>cd</b>

The cd command is used to navigate between directories in Linux. It stands for ‘change directory’.

<b>chgrp</b>

chgrp command is used for changing the group of a file or directory in Linux.

<b>chmod</b>

chmod stands for change mode. This command is used for changing the mode of access, i.e. the file permissions in Linux.

<b>chown</b>

The chown command in Linux enables you to change the user and group ownership of a file or directory.

<b>cp</b>

One of the commands that you must know in Linux is cp. It’s often called the copy command in Linux and it is actually short for copy and it does exactly as it name suggests: it copies.

<b>cron</b>

The crontab is used to automate all types of tasks on Linux systems. This is an especially important skill for aspiring system administrators to learn.

<b>curl</b>

CURL is a tool for data transfer. The most popular use case for curl command is to download files from the web in Linux terminal.

<b>cut</b>

The cut command is the canonical tool to remove “columns” from a text file. In this context, a “column” can be defined as a range of characters or bytes identified by their physical position on the line, or a range of fields delimited by a separator.

## D

<b>date</b>

The date command gives you the current date and time of you Linux system. But it can do a lot more than that.

<b>dd</b>

The dd command in Linux is a powerful utility for copying and converting files. Its most popular use case is creating live Linux USB using Linux command line.

<b>df</b>

The df command is used for checking disk space in Linux.

<b>diff</b>

When you need to compare two files containing similar text in Linux, using the diff command can make your task much easier. The command compares two files to suggest changes that would make the files identical. Great for finding that extra curly brace that broke your newly updated code.

<b>dig</b>

Dig command in Linux is commonly used for retrieving the DNS information of a remote server.

<b>dirname</b>

The dirname command in Linux prints a file path with its final component removed. This basically gives you the directory path from the file path.

<b>du</b>

Knowing the size of a file is easy in Linux but it won't show the size of directories. The du command is used for checking the size of directory.

## E

<b>echo</b>

The echo command is perhaps one of the first few commands you see when you start learning Linux commands or bash shell scripting. It is a simple command that simply prints its arguments on the display.

<b>emacs</b>

There are many text-based editors in Linux. GNU Emacs is one of the oldest and powerful editor that has a steep learning curve.

<b>expand</b>

This is a rather less known and less used command with the main use case being the ability to convert tabs into spaces.

## F

<b>file </b>

The file command gives you various information about a file in Linux. This includes the type of file, MIME type etc.

<b>find</b>

One of the frequent used commands. The find command can be used to looks for files based on their name, type, modification time and more. Combine it with the likes of exec or xargs command and you have a powerful tool at your hand for searching and modifying files.

<b>examples:</b>

Using "find" to find a file with the name of "passwords.txt"
```bash
find -name passwords.txt
```

Using "find" to find any file with the extension of ".txt"
```bash
 find -name *.txt
```

<b>findmnt</b>

Another lesser know command which is used for checking if a file system is mounted.

<b>fmt and fold</b>

Both of these commands are used for formatting text so the lines will fit in the available space on the target device.

<b>free</b>

If you would like to know the detailed information about the memory availability on your Linux system, the free command is a simple utility that makes it easy to find real time results for a variety of use cases.

<b>fsck</b>

The fsck (file system check) command helps with a potentially corrupted filesystem. This utility is used for checking and (optionally) repairing the file system.

## G

<b>grep</b>

Find command works on file name. The grep command is used to find patterns inside file content.

Using "grep" to find any entries with the text joy in "passwords.txt"

```bash
grep "joy" passwords.txt
```

Using "grep" to find any entries with the "THM"  in "access.log"

```bash
grep "THM" access.log
```

Using "grep" to find any entries with the IP address of "3.18.18.132" in "access.log"

```bash
grep 3.18.18.132 access.log
```

<b>groupadd</b>

The groupadd command in Linux creates new groups

<b>groupdel</b>

The groupdel command is perhaps the simplest command in Linux with virtually no options. It is used for deleting an existing group.

<b>groupmod</b>

You can modify group properties like group name and group ID with the groupmod command in Linux.

<b>groups</b>

This command helps you find the groups a Linux user belongs to in Linux command line.

## H

<b>head</b>

You can use the head command to print a specified number of lines from the beginning of the file.

<b>history</b>

Everything you type in the terminal is stored in the shell history. This aspect can be displayed and controlled through the history command.

## I

<b>id</b>

Every user in Linux has a unique, numeric user ID and a default group with a unique numeric group ID. The id command prints this information.

## J

<b>jobs</b>

The jobs command in Linux allows the user to directly interact with processes in the current shell.

## L

<b>less</b>

Less is an awesome Linux command utility for viewing text files.

<b>ln</b>

The ln command allows you to create both soft and hard links in Linux.
locate

The locate command allows you to preform a super quick search for files.

<b>ls</b>

The ls command in Linux is one of the most used commands. It is used for listing the contents of a directory.

<b>lsof</b>

You can list opened files by a user or a process by using the lsof command in Linux.

## M

### man

The man command in Linux offers a manual of various GNU Linux commands, as well as a manual for other third-party programs. man offers a simplified interface for programmers to offer a manual of their programs. The manual pages accompany almost all GNU/Linux programs and can be installed according to the chosen language, if it is available in the distribution. The man information is called "Man Pages" and they provide a basic description of commands and details about how your options work.

The manual documents are divided into sessions according to the subject matter. The sessions are numbered from 1 to 9, as follows:

<ol><li> Executable programs or shell commands;</li> 
<li>System Calls (functions provided by the Kernel);</li>
<li>Library Calls (functions provided by libraries);</li>
<li> Special files, especially those located in /dev;</li>
<li> File formats and conventions;</li>
<li> Gaming;</li>
<li> Macro Packages;</li> 
<li>Administrative commands;</li>
<li> Kernel routines.</li>
</ol>

Each page of the manual is divided into parts:
<b>
<ul>
<li>NAME: Name of the item searched for with a short description;</li><li>SYNOPSIS: Full description of usage and syntax;</li>
 <li>DESCRIPTION: Brief description of the features; </li>
 <li>OPTIONS: Description of each option and arguments; </li>
 <li>FILES: A list of important files;</li>
  <li>SEE ALSO: A list of items related to the wanted person; </li>
  <li>BUGS: Description of possible problems with the item; </li>
  <li>AUTHOR: List of people responsible for the item.</li>
</ul>
</b>

To access the manual, the command is the man followed by the item sought. Optionally, the session number can be passed as a parameter.

In this example man visualizes the passwd command manual, belonging to session 1:

```bash
man passwd
```

In this example, man will display the manual file /etc/passwd:

```bash
man 5 passwd
```

Navigation within the manual pages is done using the keys:

<ul>
<li><b>q</b> Leaves the manual page; </li>
<li><b>PageDown</b> or <b>f</b> Scrolls 25 lines down;</li>
 <li><b>PageUP</b> or <b>w</b> Scrolls 25 lines up;</li>
  <li><b>ArrowUp</b> or <b>k</b> Rolls 1 line up; </li>
  <li><b>ArrowDown<b> or <b>e</b> Scrolls 1 line down;</li>
   <li><b>r</b> Redraws the screen (refresh); </li>
   <li><b>p or </b>g</b> Top of page; h Help on man page options;</li>
    <li><b>s</b> Saves the man page in text format to the specified file.</li>
</ul>

<b>mkdir</b>

The mkdir command allows you to make new directories (folders in common term) in Linux.

<b>mkfs</b>

mkfs is the command line tool in Linux to format a disk or partition in a certain filesystem of your choice.

<b>more</b>

The more command in Linux opens a text file in page views. It's predecessor to the less command and not used a lot these days.

<b>mv</b>

mv command in Linux is used for moving and renaming files and directories.

## N

<b>nc (netcat)</b>

The core functionality of Netcat is allowing two computers to connect and share resources. It is a powerful and versatile network tool that is available for Linux, Mac, and Windows machines.

<b>nohup</b>

Nohup command in Linux enables you to run commands even after logging out.

<b>nslookup</b>

nslookup is one of the popular networking commands in Linux used for querying the Domain Name System (DNS) records.

## P

<b>passwd</b>

The passwd command in Linux allows you to change user password, lock accounts, expire passwords and more.

<b>paste</b>

The paste command merges several input files to produce a new delimited text file from them.

<b>ping</b>

Ping is mainly used to check if a remote host is reachable or not.

<b>printf</b>

You may print simple outputs with echo command but that's not enough for complicated formatted outputs. printf allows a C styled formating of the output.

<b>ps</b>

The ps command in Linux is used for getting information about running processes.

## R

<b>read</b>

With read command, you can make your bash script interactive by accepting user inputs.

<b>reboot</b>

Reboot performs the actions of the halt command (explained below), requiring that all processing stop. Then instead of triggering the ACPI signal, your system is restarted.

<b>rename</b>

Rename command can be used to rename multiple files in Linux at once.

<b>rm </b>

The rm command is used for removing files and directories in Linux.

<b>rsync</b>

Rsync (Remote Sync) is a synchronization tool for copying files and directories in a system or between systems. Its most popular use case includes copying files between remote systems.

## S

<b>scp</b>

Scp stands for secure copy but I like to think it as 'SSH copy'. Like rsync, scp is also used for copying files between remote systems.

<b>screen</b>

The screen command in Linux allows you to use multiple virtual terminals that can be saved by name and reopened using keyboard shortcuts.

<b>sed</b>

Sed is part of the Unix standard toolbox since the end of the 60s. As any text editor, it will help you to modify text files.

<b>seq</b>

The seq command, short for sequence, is used for printing a sequence of numbers. The numbers could be integers or real (with decimal points).

<b>sleep</b>

Linux sleep command is one of the simplest commands out there. As you can guess from the name, its only function is to sleep. In other words, it introduces a delay for a specified time.

<b>source</b>

The source command is a handy utility that can be used to refresh environment variables among some other things.

<b>stat</b>

You can get file permissions, size, mtime, ctime, atime, ownership and several other file attribute information using the stat command in Linux.

## T

<b>tail</b>

The tail command prints the last ten lines of the input files. The tail command is also used for reading log files in real time.

<b>tar</b>

Tar is one of the most common tool used for archiving files in Linux.

<b>tee</b>

The tee command reads from the standard input and writes to both standard output and files. The result is that you get to see your command’s output as well as save it to a file at the same time.

<b>time</b>

The time command in Linux measures how long a particular command or script runs.

<b>timeout</b>

With the timeout command you can set a time limit on running other commands and programs.

<b>top</b>

The top command provides a quick look at system resources and processes.

<b>touch</b>

Touch command in Linux is used for changing file timestamps however one of the most common usages of touch command includes creating a new empty file.

<b>tr</b>

The tr command in Linux is used to perform simple but useful translations of one set of characters into another.

<b>type</b>

The type command tells you whether a Linux command is built-in shell command, where is its executable located and whether it is aliased to some other command.

## U

<b>ulimit</b>

Ulimit is a built-in shell command designed to display, allocate, and limit resources.

<b>uname</b>

You can get Linux kernel version and some other system information with the uname command in Linux.
<b>uniq</b>

The uniq command in Linux and Unix is used for removing duplicate lines from a file.
<b>useradd</b>

The useradd command lets a superuser create a new user account on Linux.
userdel

The userdel lets you delete an existing user.
<b>usermod</b>

The usermod command in Linux allows you to modify a user account in various ways.

## V

<b>vim</b>

Vim is one of the most popular text editor in the Linux command line.

## W

<b>watch</b>

Watch is a great utility that automatically refreshes data. Some of the more common uses for this command involve monitoring system processes or logs, but it can be used in combination with pipes for more versatility.

<b>wc</b>

The wc command displays statistical information about a file such as the number of lines, words, characters.

<b>Examples</b>

Using "wc" to count the number of entries in "access.log"

```bash
wc -l access.log
```
Using "wc" to count the number of entries in "passwords.txt"

```bash
wc -l passwords.txt
```

<b>which</b>

which command is an extremely useful command for locating executable files located anywhere in the Linux system.

<b>who</b>

The who command in Linux lists all logged-in users on the system.

<b>whoami</b>

whoami is a Unix command that allows you to show the current user of the system, even if you have permissions added with su.


## References

* https://linuxhandbook.com/a-to-z-linux-commands/
* https://www.certificacaolinux.com.br/comando-linux-man/