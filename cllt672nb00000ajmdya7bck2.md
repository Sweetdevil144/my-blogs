---
title: "Shell Scripting 101: Essential Commands for Every Developer"
seoTitle: "Basic Shell Commands Every Developer Needs"
seoDescription: "Beginner guide to essential shell scripting for automating tasks, managing files, and enhancing command line skills. Perfect for developers"
datePublished: Sun Aug 27 2023 08:10:01 GMT+0000 (Coordinated Universal Time)
cuid: cllt672nb00000ajmdya7bck2
slug: shell-scripting-101-essential-commands-for-every-developer
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1693123739642/b7737cf3-9084-4669-947d-2864bb2b5e0e.jpeg
tags: programming-blogs, github, bash, shell, beginners

---

Diving into the universe of shell scripting? Welcome aboard! Shell scripting is a potent means to automate mundane tasks, string several commands together, and interact dynamically with your system. Here's your beginner-friendly guide to 101 essential shell commands.

Let's dive into 50 shell commands:

## **The Basics**

1. **echo - Display a line of text**
    
    It's one of the simplest commands. It's frequently used in shell scripts to display status or to produce formatted outputs.
    
    `echo [option] [string]`
    
    ```bash
    echo "Hello, World!"
    ```
    
    1. **man - Manual pages**
        
        If you are a bash scripter, this is the **MOST IMPORTANT** command you need throughout your journey. Even this blog isn't compared to what help the `man` command provides us. It is used to display manual pages for commands, giving detailed information on usage.
        
        `man [option] command`
        
        ```bash
        man ls
        ```
        
2. **ls - List contents of the directory**
    
    Lists files and directories in the current directory, with options to format or filter the results.
    
    `ls [option] [directory]`
    
    ```bash
    ls -l /home/user
    ```
    
3. **cd - Change Directory**
    
    Navigate to a different part of the filesystem.
    
    `cd [directory]`
    
    ```bash
    cd /home/user/documents
    ```
    

## **Working With Files and Directories**

1. **touch - Create an empty file**
    
    Generates new files quickly or updates timestamps on existing ones.
    
    `touch [option] filename`
    
    ```bash
    touch sample.txt
    ```
    
2. **cp - Copy files or directories**
    
    Duplicate files or directories from one location to another.
    
    `cp [option] source destination`
    
    ```bash
    cp file1.txt file2.txt
    ```
    
3. **mv - Move or rename files/directories**
    
    Transfer or rename files and directories.
    
    `mv [option] source destination`
    
    ```bash
    mv oldname.txt newname.txt
    ```
    
4. **rm - Remove files or directories**
    
    Delete files or directories. Use with caution; it's irreversible.
    
    `rm [option] file`
    
    ```bash
    rm unwantedfile.txt
    ```
    
5. **mkdir - Make directories**
    
    Create new directories.
    
    `mkdir [option] directory`
    
    ```bash
    mkdir new_directory
    ```
    
6. **rmdir - Remove empty directories**
    

Delete empty directories.

`rmdir [option] directory`

```bash
rmdir empty_directory
```

## **Manipulating Text and Files**

1. **cat - Concatenate and display file contents**
    

Read and display text files.

`cat [option] file`

```bash
cat file.txt
```

1. **grep - Search text using patterns**
    

Hunt for specific patterns in text.

`grep [option] pattern [file...]`

```bash
grep 'hello' file.txt
```

1. **sed - Stream editor**
    

Powerful tool to parse and modify text in a data stream or file.

`sed [option] 'command' file`

```bash
sed 's/apple/orange/' file.txt
```

## **Permissions, Ownerships and Monitoring**

1. **chmod - Change file permissions**
    

Adjust permissions on files or directories.

`chmod [option] mode file`

```bash
chmod 755 script.sh
```

1. **chown - Change file owner and group**
    

Alter the ownership of files or directories.

`chown [option] owner[:group] file`

```bash
chown user:group file.txt
```

1. **ps - Report process status**
    

Snapshot of current processes.

`ps [option]`

```bash
ps aux
```

1. **top - Display dynamic real-time processes**
    

Monitor system tasks in real-time.

`top [option]`

```bash
top
```

1. **kill - Terminate or signal a process**
    

Send signals to specific processes, usually to terminate.

`kill [signal or option] pid`

```bash
kill -9 12345
```

1. **history - Command history**
    

Display commands recently used.

`history [option]`

```bash
history
```

1. **find - Search for files in directories**
    

Locate files in the system based on various criteria.

`find [path...] [expression]`

```bash
find /home/user -name "*.txt"
```

21.**pwd - Print Working Directory**

Displays the full pathname of the current directory, helping to understand where you are in the filesystem.

`pwd [option]`

```bash
pwd
```

## **Compressing and Decompressing files**

1. **tar - Archive utility**
    

Combine multiple files into one or extract files from such a combined archive.

`tar [option] [file...]`

```bash
tar -xvf archive.tar
```

1. **gzip - Compress files**
    

Reduce file sizes.

`gzip [option] file`

```bash
gzip file.txt
```

1. **gunzip - Decompress files**
    

Decompress `.gz` files.

`gunzip [option] file.gz`

```bash
gunzip file.txt.gz
```

## **Networking**

1. **ping - Network diagnostic tool**
    

Check the network connection to a specific IP or domain.

`ping [option] destination`

```bash
ping google.com
```

1. **netstat - Network statistics**
    

Display network connections, routing tables, and interface statistics.

`netstat [option]`

```bash
netstat -tuln
```

1. **ifconfig - Display or configure network interfaces**
    

Show or set network interfaces.

`ifconfig [interface] [options]`

```bash
ifconfig eth0
```

1. **ssh - Secure shell remote login**
    

Connect to remote servers securely.

`ssh [option] user@host`

```bash
ssh user@domain.com
```

1. **scp - Securely copy files between hosts**
    

Transfer files between local and remote hosts securely.

`scp [option] source destination`

```bash
scp file.txt user@remote.com:/path/
```

1. **wget - Non-interactive network downloader**
    

Download files from the internet.

`wget [option] [URL]`

```bash
wget http://example.com/file.zip
```

1. **curl - Command line tool for transferring data**
    

Fetch data from a URL.

`curl [option] [URL]`

```bash
curl -O http://example.com/file.zip
```

1. **cut - Remove sections from lines of files**
    

Extract and display specific columns from a file's content.

`cut OPTION... [FILE]...`

```bash
cut -f1,3 -d',' data.csv
```

## **Displaying Files and contents**

1. **head - Output the first part of files**
    

Display the beginning of a file.

`head [option] [file...]`

```bash
head -n 10 file.txt
```

1. **tail - Output the last part of files**
    

Show the end of a file, often used to display logs.

`tail [option] [file...]`

```bash
tail -f /var/log/syslog
```

1. **sort - Sort lines of text files**
    

Organize the lines in text files.

`sort [option] [file...]`

```bash
sort file.txt
```

1. **date - Display or set the system date and time**
    

Show the current date and time or set a new one.

`date [option]`

```bash
date
```

1. **cal - Display a calendar**
    

Showcase a simple calendar.

`cal [option]`

```bash
cal 12 2023
```

## **System Checkup and Reports**

1. **df - Report file system disk space usage**
    

Check available disk space.

`df [option]`

```bash
df -h
```

1. **du - Estimate file and directory space usage**
    

Gauge how much space a directory or file uses.

`du [option] [file...]`

```bash
du -sh /home/user/
```

1. **alias - Create an alias for a command**
    

Shorten or customize command names.

`alias name='command'`

```bash
alias ll='ls -la'
```

1. **unalias - Remove an alias**
    

Remove a previously defined alias.

`unalias alias_name`

```bash
unalias ll
```

1. **which - Shows the full path of commands**
    

Display where a particular program is located.

`which [command]`

```bash
which ls
```

1. **passwd - Change user password**
    

Modify the password for a user.

`passwd [username]`

```bash
passwd john
```

1. **wc - Print newline, word, and byte counts for a file**
    

Count the number of lines, words, and bytes.

`wc [option] [file...]`

```bash
wc file.txt
```

1. **diff - Compare files line by line**
    

Contrast the contents of two files.

`diff [option] file1 file2`

```bash
diff file1.txt file2.txt
```

1. **tee - Read from standard input and write to standard output and files**
    

Useful to split the output of a command to both display and save in a file simultaneously.

`command | tee [option] file`

```bash
ls | tee output.txt
```

## **Running System Jobs**

1. **bg - Put jobs in background**
    

Send a process to run in the background.

`bg [job_id]`

```bash
bg %1
```

1. **fg - Bring jobs to foreground**
    

Retrieve a process to run in the foreground.

`fg [job_id]`

```bash
fg %1
```

1. **jobs - List active jobs**
    

Display the jobs currently running in the background.

`jobs [option]`

```bash
jobs
```

1. **clear - Clear the terminal screen**
    

Clean the console display.

`clear`

```bash
clear
```

Arming yourself with the knowledge of these 50 shell commands will significantly enhance your command line prowess. Remember, the key to mastering them is regular practice. Happy coding!

And that's our detailed guide to 50 foundational shell commands. While it's not all 101 commands as the title says, mastering these will provide a strong foundation for any developer or system administrator. Remember, practice makes perfect. Explore, experiment, and most importantly, enjoy the journey into the world of shell scripting!

Happy scripting!