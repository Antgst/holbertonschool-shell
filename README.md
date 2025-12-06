# 🐚 Holberton Shell Projects

## 📝 Description
This repository contains my Holberton School **Shell** projects.  
It covers the fundamentals of working in a Unix environment and progressively introduces:
- navigation and file manipulation
- permissions and users/groups
- I/O redirections and filters
- environment, variables, aliases, and expansions

Each project folder includes its own `README.md` describing what each script does.

## 🎯 Global Learning Objectives
By the end of this series, I am expected to be able to explain and demonstrate:
- what the shell is and how it differs from a terminal
- how to navigate and explore the Linux filesystem
- how to manage files, links, and directories
- how Linux permissions, ownership, and groups work
- how to use redirections, pipes, and text-processing commands
- how environment variables, expansions, and aliases behave
- how to read `man` pages effectively

## ✅ General Requirements (Series)
- Allowed editors: `vi`, `vim`, `emacs`
- Scripts are designed to be tested on **Ubuntu LTS** (version depends on the project)
- All scripts must be **exactly two lines long**
- All files must end with a new line
- The first line of each script must be:

    ```bash
    #!/bin/bash

- You are not allowed to use: backticks, `&&`, `||`, or `;` (depending on project rules)

- All scripts must be executable:

        chmod u+x <filename>

## 🗂️ Repository Structure

| Folder                               | Project                                         | Main focus                          | 
|--------------------------------------|-------------------------------------------------|-------------------------------------|
|`basics`                              |Shell, basics (P1)                               |navigation, files, links, man pages  |
|`permissions`                         |Shell, permissions (P2)                          |chmod, sudo, users/groups            |
|`io_redirections_and_filters`         |Shell, I/O Redirections and filters (P3)         |pipes, redirections, text filters    |
|`init_files_variables_and_expansions` |Shell, init files, variables and expansions (P4) |env, aliases, arithmetic, expansions |


# 1) 🧭 Shell, basics (P1)
## 📚 Resources
- What Is “The Shell”?
- Navigation
- Looking Around
- A Guided Tour
- Manipulating Files
- Working With Commands
- Reading Man pages
- Keyboard shortcuts for Bash
- LTS
- Shebang
- Linux file systems explained
- `man` or `help`:
    - `cd`
    - `ls`
    - `pwd`
    - `less`
    - `file`
    - `ln`
    - `cp`
    - `mv`
    - `rm`
    - `mkdir`
    - `type`
    - `which`
    - `help`
    - `man`

## 🎯 Learning Objectives
### General
- What does RTFM mean?
- What is a Shebang?
- What is the Shell?
- What is the difference between a terminal and a shell?
- What is the shell prompt?
- How to use the history (the basics)

### Navigation

- What do the commands or built-ins `cd`, `pwd`, `ls` do?
- How to navigate the filesystem
- What are the `.` and `..` directories?
- What is the working directory, how to print it and how to change it?
- What is the root directory?
- What is the home directory, and how to go there?
- What is the difference between the root directory and the home directory of the user `root`?
- What are the characteristics of hidden files and how to list them?
- What does the command `cd -` do?

### Looking Around

- What do the commands `ls`, `less`, `file` do? 
- How do you use options and arguments with commands?
- Understand the `ls` long format and how to display it

### A Guided Tour

- What does the `ln` command do?
- What do you find in the most common/important directories?
- What is a symbolic link?
- What is a hard link?
- What is the difference between a hard link and a symbolic link?

### Manipulating Files
- What do the commands `cp`, `mv`, `rm`, `mkdir` do?
- What are wildcards and how do they work?
- How to use wildcards

### Working with Commands
- What do `type`, `which`, `help`, `man` commands do?
- What are the different kinds of commands?
- What is an alias?
- When do you use the command `help` instead of `man`?

### Reading Man Pages
- How to read a man page
- What are man page sections?
- What are the section numbers for User commands, System calls and Library functions?
- Keyboard Shortcuts for Bash
- Common shortcuts for Bash

### LTS
- What does LTS mean?

## ✅ Requirements
- Tested on Ubuntu 22.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All scripts should be exactly two lines long
- All your files should end with a new line
The first line of all your files should be exactly:

    ```bash
    #!/bin/bash

- A `README.md` file at the root of the repo, containing a description of the repository
- A `README.md` file at the root of this project folder, describing what each script is doing
- You are not allowed to use backticks, `&&`, `||` or `;`
- All your scripts must be executable:
    ```bash
    chmod u+x <filename>

## 📌 Scripts

Each script in this folder performs a specific required task for Shell basics.
(See `basics/README.md` for the detailed per-script description.)

# 2) 🔐 Shell, permissions (P2)
## 📚 Resources

- Permissions
- `man` or `help`:
    - `chmod`
    - `sudo`
    - `su`
    - `chown`
    - `chgrp`
    - `id`
    - `groups`
    - `whoami`
    - `adduser`
    - `useradd`
    - `addgroup`

## 🎯 Learning Objectives
### Permissions

- What do the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do?
- Linux file permissions
- How to represent each of the three sets of permissions (owner, group, and other) as a single digit
- How to change permissions, owner and group of a file
- Why can’t a normal user `chown` a file?
- How to run a command with root privileges
- How to change user ID or become superuser

### Other Man Pages

- How to create a user
- How to create a group
- How to print real and effective user and group IDs
- How to print the groups a user is in
- How to print the effective userid

## ✅ Requirements

- Tested on Ubuntu 22.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All scripts should be exactly two lines long
- All your files should end with a new line
The first line of all your files should be exactly:

    ```bash
    #!/bin/bash

- A `README.md` file at the root of this project folder, describing what each script is doing
- You are not allowed to use backticks, `&&`, `||` or `;`
- All your files must be executable
- Warning: tasks 3 / 13 / 14 / 15 / 16 must be done inside the sandbox in order to be corrected by the checker

## 📌 Scripts

Each script in this folder focuses on a specific permissions or user/group task.
(See `permissions/README.md` for the detailed per-script description.)

# 3) 🔁 Shell, I/O Redirections and filters (P3)
## 📚 Resources

- Shell, I/O Redirection
- Special Characters
- `man` or `help`:
    - `echo`
    - `cat`
    - `head`
    - `tail`
    - `find`
    - `wc`
    - `sort`
    - `uniq`
    - `grep`
    - `tr`
    - `rev`
    - `cut`
    - `man 5 passwd`

## 🎯 Learning Objectives
### Shell, I/O Redirection
- What do the commands `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr` do?
- How to redirect standard output to a file
- How to get standard input from a file instead of the keyboard
- How to send the output from one program to the input of another program
- How to combine commands and filters with redirections

### Special Characters

What are special characters?

Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde and how and when to use them

### Other Man Pages
- How to display a line of text
- How to concatenate files and print on the standard output
- How to reverse a string
- How to remove sections from each line of files
- What is the `/etc/passwd` file and what is its format?
- What is the `/etc/shadow` file and what is its format?

## ✅ Requirements

- Tested on Ubuntu 20.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All scripts should be exactly two lines long
- All your files should end with a new line
- The first line of all your files should be exactly:

        #!/bin/bash


- A `README.md` file at the root of this project folder, describing what each script is doing
- You are not allowed to use backticks, `&&`, `||` or `;`
- All your files must be executable
- You are not allowed to use `sed` or `awk`

## 📌 Scripts

Each script applies redirections, pipes, or filters to solve a specific task.
(See `io_redirections_and_filters/README.md` for the detailed per-script description.)

# 4) 🧩 Shell, init files, variables and expansions (P4)
## 📚 Resources

- Expansions
- Shell Arithmetic
- Variables
- Shell initialization files
- The alias Command
- Technical Writing
- `man` or `help`:
    - `printenv`
    - `set`
    - `unset`
    - `export`
    - `alias`
    - `unalias`
    - `.`
    - `source`
    - `printf`

## 🎯 Learning Objectives
### General

- What happens when you type:

    ```bash
    ls -l *.txt

### Shell Initialization Files
- What are the `/etc/profile` file and the `/etc/profile.d` directory?
- What is the `~/.bashrc` file?

### Variables
- What is the difference between a local and a global variable?
- What is a reserved variable?
- How to create, update and delete shell variables
- What are the roles of the following reserved variables: `HOME`, `PATH`, `PS1`
- What are special parameters?
- What is the special parameter `$`?

### Expansions
- What is expansion and how to use them?
- What is the difference between single and double quotes and how to use them properly?
- How to do command substitution with `$()` and backticks

### Shell Arithmetic
- How to perform arithmetic operations with the shell

### The alias Command
- How to create an alias
- How to list aliases
- How to temporarily disable an alias

### Other help pages
- How to execute commands from a file in the current shell

## ✅ Requirements
- Tested on Ubuntu 20.04 LTS
- Allowed editors: `vi`, `vim`, `emacs`
- All scripts should be exactly two lines long
- All your files should end with a new line
- The first line of all your files should be exactly:

        #!/bin/bash

- A `README.md` file at the root of this project folder, describing what each script is doing
- You are not allowed to use `&&`, `||` or `;`
- You are not allowed to use `bc`, `sed` or `awk`
- All your files must be executable
 
## 📌 Scripts

- Each script demonstrates environment handling, expansions, or alias usage.
(See `init_files_variables_and_expansions/README.md` for the detailed per-script description.)

## 🚀 How to Run

    chmod u+x <script_name>
    ./<script_name>

## 👤 Author
Antoine Gousset — Holberton student & future fullstack dev
- GitHub: https://github.com/Antgst
