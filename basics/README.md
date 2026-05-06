# 📘 Shell, basics

## 📌 Description

_No description detected._

---

## 📚 Resources

**Read or watch**:



- [What Is "The Shell"?](https://intranet.hbtn.io/auth/sign_in)

- [Navigation](https://intranet.hbtn.io/auth/sign_in)

- [Looking Around](https://intranet.hbtn.io/auth/sign_in)

- [A Guided Tour](http://linuxcommand.org/lc3_lts0040.php)

- [Manipulating Files](http://linuxcommand.org/lc3_lts0050.php)

- [Working With Commands](http://linuxcommand.org/lc3_lts0060.php)

- [Reading Man pages](http://linuxcommand.org/lc3_man_pages/man1.html)

- [Keyboard shortcuts for Bash](https://www.howtogeek.com/181/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/)

- <a href="https://wiki.ubuntu.com/LTS" target="_blank">LTS</a>

- [Shebang](https://en.wikipedia.org/wiki/Shebang_%28Unix%29)

- [Linux file systems explained](https://www.linuxfoundation.org/blog/blog/classic-sysadmin-the-linux-filesystem-explained)



**man or help**:



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

---

## 🎯 Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), __without the help of Google__:



### General



- What does RTFM mean?

- What is a Shebang



### What is the Shell



- What is the shell

- What is the difference between a terminal and a shell

- What is the shell prompt

- How to use the history (the basics)



### Navigation



- What do the commands or built-ins `cd`, `pwd`, `ls` do

- How to navigate the filesystem

- What are the . and .. directories

- What is the working directory, how to print it and how to change it

- What is the root directory

- What is the home directory, and how to go there

- What is the difference between the root directory and the home directory of the user root

- What are the characteristics of hidden files and how to list them

- What does the command `cd -` do



### Looking Around



- What do the commands `ls`, `less`, `file` do

- How do you use options and arguments with commands

- Understand the ls long format and how to display it

- [A Guided Tour](http://linuxcommand.org/lc3_lts0040.php)

- What does the `ln` command do

- What do you find in the most common/important directories

- What is a symbolic link

- What is a hard link

- What is the difference between a hard link and a symbolic link



### Manipulating Files



- What do the commands `cp`, `mv`, `rm`, `mkdir` do

- What are wildcards and how do they work

- How to use wildcards



### Working with Commands



- What do `type`, `which`, `help`, `man` commands do

- What are the different kinds of commands

- What is an alias

- When do you use the command help instead of man



### Reading Man Pages



- How to read a man page

- What are man page sections

- What are the section numbers for User commands, System calls and Library functions



### Keyboard Shortcuts for Bash



- Common shortcuts for Bash



### LTS



- What does `LTS` mean?

---

## ✅ Requirements

### General



- Allowed editors: `vi`, `vim`, `emacs`

- All your scripts will be tested on Ubuntu 22.04 LTS

- All your scripts should be exactly two lines long (`$ wc -l file` should print 2)

- All your files should end with a new line (<a href="http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789">why?</a>)

- The first line of all your files should be exactly `#!/bin/bash`

- A `README.md` file at the root of the repo, containing a description of the repository

- A `README.md` file, at the root of the folder of *this* project, describing what each script is doing

- You are not allowed to use backticks, `&&`, `||` or `;`

- All your scripts must be executable. To make your file executable, use the `chmod` command:  `chmod u+x FILENAME_GOES_HERE`. Later, we'll learn more about how to utilize this command.

---

## ⚙️ Setup

_No specific setup detected._

---

## 🧠 Quiz

<details>
<summary>Question #0</summary>

**Question:** What command would you use to list files on Linux?

**Available answers:**

- `pwd`
- `cd`
- `ls`
- `list`
- `which`

**Answer:** `ls`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #1</summary>

**Question:** What does LTS stand for?

**Available answers:**

- `Long Term Support`
- `Long Time Support`
- `Last Terrible Service`

**Answer:** `Long Term Support`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #2</summary>

**Question:** How do you change directory on Linux?

**Available answers:**

- `pwd`
- `cd`
- `ls`
- `which`

**Answer:** `cd`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #3</summary>

**Question:** What does RTFM stand for?

**Available answers:**

- `Remember The First Manipulation`
- `Read, Teach, Forget, Migrate`
- `Read The F** Manual`

**Answer:** `Read The F** Manual`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>


---

## 🧩 Tasks

<details>
<summary>0. Where am I?</summary>

**Files:**

- [`0-current_working_directory`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/0-current_working_directory)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
0. Where am I?
Write a script that prints the absolute path name of the current working directory.
Example:
$
./
0
-current_working_directory
/basics
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
0-current_working_directory
Score of the task
6
/6
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
0. Where am I?
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "0. Where am I?"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>1. What’s in there?</summary>

**Files:**

- [`1-listit`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/1-listit)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
1. What’s in there?
Display the contents list of your current directory.
Example:
$
./
1
-listit
Applications
Documents
Dropbox
Movies
Pictures
Desktop
Downloads
Library
Music
Public
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
1-listit
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
1. What’s in there?
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "1. What’s in there?"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>2. There is no place like home</summary>

**Files:**

- [`2-bring_me_home`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/2-bring_me_home)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
2. There is no place like home
Write a script that changes the working directory to the user’s home directory.
You are not allowed to use any shell variables
Example:
julien
@ubuntu
:/tmp
$
pwd
/tmp
julien
@ubuntu
:/tmp
$
echo
$HOME
/home/julien
julien
@ubuntu
:/tmp
$
source ./
2
-bring_me_home
julien
@ubuntu
:~
$
pwd
/home/julien
julien
@ubuntu
:~
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
2-bring_me_home
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
2. There is no place like home
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "2. There is no place like home"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>3. The long format</summary>

**Files:**

- [`3-listfiles`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/3-listfiles)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
3. The long format
Display current directory contents in a long format
Example:
$ ./3-listfiles
total 40
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:20 README.md
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
3-listfiles
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
3. The long format
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "3. The long format"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>4. Hidden files</summary>

**Files:**

- [`4-listmorefiles`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/4-listmorefiles)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
4. Hidden files
Display current directory contents, including hidden files (starting with
.
). Use the long format.
Example:
$ ./
4
-listmorefiles
total
48
drwxr-xr-
x@
6
sylvain staff
204
Jan
25
00
:
29
.
drwxr-xr-
x@
43
sylvain staff
1462
Jan
25
00
:
19
..
-rwxr-xr-
x@
1
sylvain staff
18
Jan
25
00
:
19
0
-current_working_directory
-rwxr-xr-
x@
1
sylvain staff
19
Jan
25
00
:
23
1
-listit
-rwxr-xr-
x@
1
sylvain staff
18
Jan
25
00
:
29
2
-bring_me_home
-rwxr-xr-
x@
1
sylvain staff
18
Jan
25
00
:
39
3
-listfiles
-rwxr-xr-
x@
1
sylvain staff
18
Jan
25
00
:
41
4
-listmorefiles
-rwxr-xr-
x@
1
sylvain staff
18
Jan
25
00
:
20
README.md
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
4-listmorefiles
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
4. Hidden files
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "4. Hidden files"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>5. I love numbers</summary>

**Files:**

- [`5-listfilesdigitonly`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/5-listfilesdigitonly)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
5. I love numbers
Display current directory contents.
Long format
with user and group IDs displayed numerically
And hidden files (starting with .)
Example:
$ ./
5
-listfilesdigitonly
total
56
drwxr-xr-
x@
6
501
20
204
Jan
25
00
:
29
.
drwxr-xr-
x@
43
501
20
1462
Jan
25
00
:
19
..
-rwxr-xr-
x@
1
501
20
18
Jan
25
00
:
19
0
-current_working_directory
-rwxr-xr-
x@
1
501
20
18
Jan
25
00
:
23
1
-listfiles
-rwxr-xr-
x@
1
501
20
19
Jan
25
00
:
29
2
-bring_me_home
-rwxr-xr-
x@
1
501
20
20
Jan
25
00
:
39
3
-listfiles
-rwxr-xr-
x@
1
501
20
18
Jan
25
00
:
41
4
-listmorefiles
-rwxr-xr-
x@
1
501
20
18
Jan
25
00
:
43
5
-listfilesdigitonly
-rwxr-xr-
x@
1
501
20
18
Jan
25
00
:
20
README.md
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
5-listfilesdigitonly
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
5. I love numbers
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "5. I love numbers"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>6. Welcome</summary>

**Files:**

- [`6-firstdirectory`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/6-firstdirectory)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
6. Welcome
Create a script that creates a directory named
my_first_directory
in the
/tmp/
directory.
Example:
$
./
6
-firstdirectory
$
file /tmp/my_first_directory/
/tmp/my
_first_directory/: directory
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
6-firstdirectory
Score of the task
4
/4
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
6. Welcome
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "6. Welcome"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>7. Betty in my first directory</summary>

**Files:**

- [`7-movethatfile`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/7-movethatfile)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
7. Betty in my first directory
Move the file
betty
from
/tmp/
to
/tmp/my_first_directory
.
Example:
$
./7-movethatfile
$
ls
/tmp/my_first_directory/
betty
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
7-movethatfile
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
7. Betty in my first directory
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "7. Betty in my first directory"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>8. Bye bye Betty</summary>

**Files:**

- [`8-firstdelete`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/8-firstdelete)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
8. Bye bye Betty
Delete the file
betty
.
The file
betty
is in
/tmp/my_first_directory
Example:
$
./8-firstdelete
$
ls
/tmp/my_first_directory/
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
8-firstdelete
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
8. Bye bye Betty
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "8. Bye bye Betty"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>9. Bye bye My first directory</summary>

**Files:**

- [`9-firstdirdeletion`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/9-firstdirdeletion)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
9. Bye bye My first directory
Delete the directory
my_first_directory
that is in the
/tmp
directory.
Example:
$
./9-firstdirdeletion
$
file /tmp/my_first_directory
/tmp/my_first_directory: cannot open `/tmp/my_first_directory' (No such file or directory)
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
9-firstdirdeletion
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
9. Bye bye My first directory
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "9. Bye bye My first directory"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>10. Back to the future</summary>

**Files:**

- [`10-back`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/10-back)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
10. Back to the future
Write a script that changes the working directory to the previous one.
julien
@ubuntu
:/tmp
$
pwd
/tmp
julien
@ubuntu
:/tmp
$
cd /var
julien
@ubuntu
:/var
$
pwd
/var
julien
@ubuntu
:/var
$
source ./
10
-back
/tmp
julien
@ubuntu
:/tmp
$
pwd
/tmp
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
10-back
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
10. Back to the future
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "10. Back to the future"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>11. Lists</summary>

**Files:**

- [`11-lists`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/11-lists)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
11. Lists
Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the
/boot
directory (in this order), in long format.
Be careful with the
/
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
11-lists
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
11. Lists
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "11. Lists"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>12. File type</summary>

**Files:**

- [`12-file_type`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/12-file_type)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
12. File type
Write a script that prints the type of the file named
iamafile
. The file
iamafile
will be in the
/tmp
directory when we will run your script.
Example
ubuntu
@ip
-
172
-
31
-
63
-
244
:~
$
./
12
-file_type
/tmp/
iamafile:
ELF
64
-bit
LSB
executable, x86-
64
, version
1
(
SYSV
), dynamically linked (uses shared libs),
for
GNU
/
Linux
2.6
.
24
,
Build
ID[sha1]=bd39c07194a778ccc066fc963ca152bdfaa3f971, stripped
Note that depending on the file, the output of your script will be different.
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
12-file_type
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
12. File type
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "12. File type"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>13. We are symbols, and inhabit symbols</summary>

**Files:**

- [`13-symbolic_link`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/13-symbolic_link)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
13. We are symbols, and inhabit symbols
Create a symbolic link to
/bin/ls
, named
__ls__
.
The symbolic link should be created in the current working directory.
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la
total
144
drwxrwxr-x
2
ubuntu ubuntu
4096
Sep
20
03
:
24
.
drwxrwxrwt
12
root   root
139264
Sep
20
03
:
24
..
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$.
/
13
-symbolic_link
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la
total
144
drwxrwxr-x
2
ubuntu ubuntu
4096
Sep
20
03
:
24
.
drwxrwxrwt
12
root   root
139264
Sep
20
03
:
24
..
lrwxrwxrwx
1
ubuntu ubuntu
7
Sep
20
03
:
24
__ls__ ->
/bin/ls
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
13-symbolic_link
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
13. We are symbols, and inhabit symbols
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "13. We are symbols, and inhabit symbols"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>14. Copy HTML files</summary>

**Files:**

- [`14-copy_html`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/14-copy_html)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
14. Copy HTML files
Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
You can consider that all HTML files have the extension
.html
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
14-copy_html
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
14. Copy HTML files
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "14. Copy HTML files"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>15. Let’s move</summary>

**Files:**

- [`15-lets_move`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/15-lets_move)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
15. Let’s move
Create a script that moves all files beginning with an uppercase letter to the directory
/tmp/u
.
You can assume that the directory
/tmp/u
will exist when we will run your script
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la
total
148
drwxrwxr-x
3
ubuntu ubuntu
4096
Sep
20
03
:
33
.
drwxrwxrwt
12
root   root
139264
Sep
20
03
:
26
..
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
My
_file
lrwxrwxrwx
1
ubuntu ubuntu
7
Sep
20
03
:
24
__ls__ ->
/bin/ls
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
Elif
_ym
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
random_file
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la /tmp/u
total
8
drwxrwxr-x
2
ubuntu ubuntu
4096
Sep
20
03
:
33
.
drwxrwxr-x
3
ubuntu ubuntu
4096
Sep
20
03
:
33
..
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
./
15
-lets_move
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la
total
148
drwxrwxr-x
3
ubuntu ubuntu
4096
Sep
20
03
:
33
.
drwxrwxrwt
12
root   root
139264
Sep
20
03
:
26
..
lrwxrwxrwx
1
ubuntu ubuntu
7
Sep
20
03
:
24
__ls__ ->
/bin/ls
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
random_file
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls -la /tmp/u
total
8
drwxrwxr-x
2
ubuntu ubuntu
4096
Sep
20
03
:
33
.
drwxrwxr-x
3
ubuntu ubuntu
4096
Sep
20
03
:
33
..
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
My
_file
-rw-rw-r--
1
ubuntu ubuntu
0
Sep
20
03
:
32
Elif
_ym
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
15-lets_move
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
15. Let’s move
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "15. Let’s move"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>16. Clean Emacs</summary>

**Files:**

- [`16-clean_emacs`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/16-clean_emacs)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
16. Clean Emacs
Create a script that deletes all files in the current working directory that end with the character
~
.
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
ls
main.c  main.c~
Makefile
~
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/sym
$
./
16
-clean_emacs
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/emacs
$
ls
main.c
ubuntu
@ip
-
172
-
31
-
63
-
244
:/tmp/emacs
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
16-clean_emacs
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
16. Clean Emacs
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "16. Clean Emacs"
×
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>17. Tree</summary>

**Files:**

- [`17-tree`](https://github.com/Antgst/holbertonschool-shell/blob/main/basics/17-tree)

**Repository:** `holbertonschool-shell`

**Directory:** `basics`

**Task details:**

```text
17. Tree
Create a script that creates the directories
welcome/
,
welcome/to/
and
welcome/to/school
in the current directory.
You are only allowed to use two spaces (and lines) in your script, not more.
julien
@ubuntu
:/tmp/h
$
ls -l
total
4
-rwxrw-r--
1
julien julien
44
Sep
20
12
:
09
17
-tree
julien
@ubuntu
:/tmp/h
$
wc -l
17
-tree
2
17
-tree
julien
@ubuntu
:/tmp/h
$
head -
1
17
-tree
#!/bin/bash
julien
@ubuntu
:/tmp/h
$
tr -cd
' '
<
17
-tree |
wc -c # you
do
not
have to understand this yet, but the result should be 2, 1
or
0
2
julien@ubuntu:/tmp/h$ ./17-tree
julien@ubuntu:/tmp/h$ ls
17-tree  welcome
julien@ubuntu:/tmp/h$ ls welcome/
to
julien@ubuntu:/tmp/h$ ls -l welcome/to
total 4
drwxrwxr-x 2 julien julien 4096 Sep 20 12:11 school
julien@ubuntu:/tmp/h$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
basics
File:
17-tree
Score of the task
5
/5
pts
100.0%
0
correction requests
My GitHub
Connect GitHub
Connect as:
Disconnect
Repository
Select a repository…
Folder (optional)
Run the correction
Get a sandbox
QA Review
×
17. Tree
Commit used:
User:
---
URL:
Click here
ID:
---
Author:
---
Subject:
---
Date:
---
×
Students who are done with "17. Tree"
×
Recommended Sandboxes
Loading...
```

</details>


---

## 🧪 Testing

Use the provided task examples and Holberton checker to validate the project.

---

## 👤 Author

Project from Holberton School.

README generated with Antoine's README Factory workflow.
