# ðŸ“˜ Shell, init files, variables and expansions

## ðŸ“Œ Description

_No description detected._

---

## ðŸ“š Resources

**Read or watch**:



- [Expansions](http://linuxcommand.org/lc3_lts0080.php)

- [Shell Arithmetic](https://intranet.hbtn.io/rltoken/CuAnsjJ9mg_y-zBVwmn7mg)

- [Variables](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_02.html)

- [Shell initialization files](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_01.html)

- [The alias Command](https://www.linfo.org/alias.html)

- [Technical Writing](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/misc/2021/6/9112669886fd446a2aa3113c31319d1f468dc160.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20260504%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20260504T204546Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4ae5c8cab9d918a8293684aa7327a1d1db7c5c416bb5fe20d18a928441b5721c)



**man or help**:



- `printenv`

- `set`

- `unset`

- `export`

- `alias`

- `unalias`

- `.`

- `source`

- `printf`

---

## ðŸŽ¯ Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), __without the help of Google__:



### General



- What happens when you type `$ ls -l *.txt`



### Shell Initialization Files



- What are the `/etc/profile` file and the `/etc/profile.d` directory

- What is the `~/.bashrc` file



### Variables



- What is the difference between a local and a global variable

- What is a reserved variable

- How to create, update and delete shell variables

- What are the roles of the following reserved variables: HOME, PATH, PS1

- What are special parameters

- What is the special parameter `$?`?



### Expansions



  - What is expansion and how to use them

  - What is the difference between single and double quotes and how to use them properly

  - How to do command substitution with `$()` and backticks



### Shell Arithmetic



- How to perform arithmetic operations with the shell



### The `alias` Command



- How to create an alias

- How to list aliases

- How to temporarily disable an alias



### Other `help` pages



- How to execute commands from a file in the current shell

---

## âœ… Requirements

### General



- Allowed editors: `vi`, `vim`, `emacs`

- All your scripts will be tested on Ubuntu 20.04 LTS

- All your scripts should be exactly two lines long (`$ wc -l file` should print 2)

- All your files should end with a new line (<a href="http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789">why?</a>)

- The first line of all your files should be exactly `#!/bin/bash`

- A `README.md` file, at the root of the folder of the project, describing what each script is doing

- You are not allowed to use `&&`, `||` or `;`

- You are not allowed to use `bc`, `sed` or `awk`

- All your files must be executable

---

## âš™ï¸ Setup

_No specific setup detected._

---

## ðŸ§  Quiz

<details>
<summary>Question #0</summary>

**Question:** Which command should I use to display a variable?

**Available answers:**

- `ls $MYVAR`
- `cd $MYVAR`
- `export $MYVAR`
- `echo $MYVAR`

**Answer:** `echo $MYVAR`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #1</summary>

**Question:** What is the variable name who contains the previous working directory path?

**Available answers:**

- `OLDPWD`
- `PREVPWD`
- `OLDDIR`
- `PREVDIR`

**Answer:** `OLDPWD`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #2</summary>

**Question:** Which command should I use to display the exit code of the previous command?

**Available answers:**

- `echo ?`
- `echo $EXITCODE`
- `echo $?`
- `echo $CODE`

**Answer:** `echo $?`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #3</summary>

**Question:** Which command should I use to define a new command push for pushing in Github?

**Available answers:**

- `alias push="git push"`
- `export push="git push"`
- `alias push=git push`
- `export push=git push`

**Answer:** `alias push="git push"`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>


---

## ðŸ§© Tasks

<details>
<summary>0. <o></summary>

**Files:**

- [`0-alias`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/0-alias)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
0. <o>
Create a script that creates an alias.
Name:
ls
Value:
rm -f *
julien
@ubuntu
:/tmp/
0x03
$
ls
0
-
alias
file1    file2
julien
@ubuntu
:/tmp/
0x03
$
source ./
0
-
alias
julien
@ubuntu
:/tmp/
0x03
$
ls
julien
@ubuntu
:/tmp/
0x03
$
\ls
julien
@ubuntu
:/tmp/
0x03
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
0-alias
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
0. <o>
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
Ã—
Students who are done with "0. <o>"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>1. Hello you</summary>

**Files:**

- [`1-hello_you`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/1-hello_you)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
1. Hello you
Create a script that prints
hello user
, where user is the current Linux user.
julien
@ubuntu
:/tmp/
0x03
$
id
uid=
1000
(julien) gid=
1000
(julien) groups=
1000
(julien),
4
(adm),
24
(cdrom),
27
(sudo),
30
(dip),
46
(plugdev),
113
(lpadmin),
128
(sambashare)
julien
@ubuntu
:/tmp/
0x03
$
./
1
-hello_you
hello julien
julien
@ubuntu
:/tmp/
0x03
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
1-hello_you
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
1. Hello you
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
Ã—
Students who are done with "1. Hello you"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>2. The path to success is to take massive, determined action</summary>

**Files:**

- [`2-path`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/2-path)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
2. The path to success is to take massive, determined action
Add
/action
to the
PATH
.
/action
should be the last directory the shell looks into when looking for a program.
julien
@ubuntu
:
/tmp/
0x03
$ echo
$PATH
/home/
julien
/bin:/
home
/julien/
.local
/bin:/
usr
/local/
sbin:
/usr/
local
/bin:/
usr
/sbin:/
usr
/bin:/
sbin:
/bin:/
usr
/games:/
usr
/local/
games:
/snap/
bin
julien
@ubuntu
:
/tmp/
0x03
$ source
./
2
-
path
julien
@ubuntu
:
/tmp/
0x03
$ echo
$PATH
/home/
julien
/bin:/
home
/julien/
.local
/bin:/
usr
/local/
sbin:
/usr/
local
/bin:/
usr
/sbin:/
usr
/bin:/
sbin:
/bin:/
usr
/games:/
usr
/local/
games:
/snap/
bin:
/
action
julien
@ubuntu
:
/tmp/
0x03
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
2-path
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
2. The path to success is to take massive, determined action
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
Ã—
Students who are done with "2. The path to success is to take massive, determined action"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>3. If the path be beautiful, let us not ask where it leads</summary>

**Files:**

- [`3-paths`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/3-paths)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
3. If the path be beautiful, let us not ask where it leads
Create a script that counts the number of directories in the
PATH
.
julien
@ubuntu
:
/tmp/
0x03
$ echo
$PATH
/home/
julien
/bin:/
home
/julien/
.local
/bin:/
usr
/local/
sbin:
/usr/
local
/bin:/
usr
/sbin:/
usr
/bin:/
sbin:
/bin:/
usr
/games:/
usr
/local/
games:
/snap/
bin
julien
@ubuntu
:
/tmp/
0x03
$ .
./
3
-
paths
11
julien
@ubuntu
:
/tmp/
0x03
$
PATH
=/
home
/julien/
bin:
/home/
julien
/.local/
bin:
/usr/
local
/sbin:/
usr
/local/
bin:
/usr/
sbin:
/usr/
bin:
/sbin:/
bin:
/usr/
games:
/usr/
local
/games:/
snap
/bin:::::/
hello
julien
@ubuntu
:
/tmp/
0x03
$ .
./
3
-
paths
12
julien
@ubuntu
:
/tmp/
0x03
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
3-paths
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
3. If the path be beautiful, let us not ask where it leads
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
Ã—
Students who are done with "3. If the path be beautiful, let us not ask where it leads"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>4. Global variables</summary>

**Files:**

- [`4-global_variables`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/4-global_variables)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
4. Global variables
Create a script that lists environment variables.
julien@ubuntu:/tmp/0x03$ source ./4-global_variables
CC=gcc
CDPATH=.:~:/usr/local:/usr:/
CFLAGS=-O2 -fomit-frame-pointer
COLORTERM=gnome-terminal
CXXFLAGS=-O2 -fomit-frame-pointer
DISPLAY=:0
DOMAIN=hq.garrels.be
e=
TOR=vi
FCEDIT=vi
FIGNORE=.o:~
G_BROKEN_FILENAMES=1
GDK_USE_XFT=1
GDMSESSION=Default
GNOME_DESKTOP_SESSION_ID=Default
GTK_RC_FILES=/etc/gtk/gtkrc:/nethome/franky/.gtkrc-1.2-gnome2
GWMCOLOR=darkgreen
GWMTERM=xterm
HISTFILESIZE=5000
history_control=ignoredups
HISTSIZE=2000
HOME=/nethome/franky
HOSTNAME=octarine.hq.garrels.be
INPUTRC=/etc/inputrc
IRCNAME=franky
JAVA_HOME=/usr/java/j2sdk1.4.0
LANG=en_US
LDFLAGS=-s
LD_LIBRARY_PATH=/usr/lib/mozilla:/usr/lib/mozilla/plugins
LESSCHARSET=latin1
LESS=-edfMQ
LESSOPEN=|/usr/bin/lesspipe.sh %s
LEX=flex
LOCAL_MACHINE=octarine
LOGNAME=franky
[...]
julien@ubuntu:/tmp/0x03$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
4-global_variables
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
4. Global variables
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
Ã—
Students who are done with "4. Global variables"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>5. Local variables</summary>

**Files:**

- [`5-local_variables`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/5-local_variables)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
5. Local variables
Create a script that lists all local variables and environment variables, and functions.
julien@ubuntu:/tmp/0x03$ . ./5-local_variables
BASH=/bin/bash
BASHOPTS=checkwinsize:cmdhist:complete_fullquote:expand_aliases:extglob:extquote:force_fignore:histappend:interactive_comments:progcomp:promptvars:sourcepath
BASH_ALIASES=()
BASH_ARGC=()
BASH_ARGV=()
BASH_CMDS=()
BASH_COMPLETION_COMPAT_DIR=/etc/bash_completion.d
BASH_LINENO=()
BASH_REMATCH=()
BASH_SOURCE=()
BASH_VERSINFO=([0]=
"4"
[1]=
"3"
[2]=
"46"
[3]=
"1"
[4]=
"release"
[5]=
"x86_64-pc-linux-gnu"
)
BASH_VERSION='4.3.46(1)-release'
CLUTTER_IM_MODULE=xim
COLUMNS=133
COMPIZ_CONFIG_PROFILE=ubuntu
COMP_WORDBREAKS=$' \t\n
"\'><=;|&(:'
DBUS_SESSION_BUS_ADDRESS=unix:abstract=/tmp/dbus-Fg27Lr20bq
DEFAULTS_PATH=/usr/share/gconf/ubuntu.default.path
DESKTOP_SESSION=ubuntu
[...]
julien@ubuntu:/tmp/0x03$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
5-local_variables
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
5. Local variables
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
Ã—
Students who are done with "5. Local variables"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>6. Local variable</summary>

**Files:**

- [`6-create_local_variable`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/6-create_local_variable)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
6. Local variable
Create a script that creates a new local variable.
Name:
BEST
Value:
School
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
6-create_local_variable
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
6. Local variable
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
Ã—
Students who are done with "6. Local variable"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>7. Global variable</summary>

**Files:**

- [`7-create_global_variable`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/7-create_global_variable)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
7. Global variable
Create a script that creates a new global variable.
Name:
BEST
Value:
School
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
7-create_global_variable
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
7. Global variable
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
Ã—
Students who are done with "7. Global variable"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>8. Every addition to true knowledge is an addition to human power</summary>

**Files:**

- [`8-true_knowledge`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/8-true_knowledge)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
8. Every addition to true knowledge is an addition to human power
Write a script that prints the result of the addition of 128 with the value stored in the environment variable
TRUEKNOWLEDGE
, followed by a new line.
julien
@production
-
503e7013
:~
$
export
TRUEKNOWLEDGE
=
1209
julien
@production
-
503e7013
:~
$
./
8
-true_knowledge |
cat -e
1337$
julien@production-503e7013:~$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
8-true_knowledge
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
8. Every addition to true knowledge is an addition to human power
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
Ã—
Students who are done with "8. Every addition to true knowledge is an addition to human power"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>9. Divide and rule</summary>

**Files:**

- [`9-divide_and_rule`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/9-divide_and_rule)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
9. Divide and rule
Write a script that prints the result of
POWER
divided by
DIVIDE
, followed by a new line.
POWER
and
DIVIDE
are environment variables
julien
@production
-
503e7013
:~
$
export
POWER
=
42784
julien
@production
-
503e7013
:~
$
export
DIVIDE
=
32
julien
@production
-
503e7013
:~
$
./
9
-divide_and_rule |
cat -e
1337$
julien@production-503e7013:~$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
9-divide_and_rule
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
9. Divide and rule
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
Ã—
Students who are done with "9. Divide and rule"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath</summary>

**Files:**

- [`10-love_exponent_breath`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/10-love_exponent_breath)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath
Write a script that displays the result of
BREATH
to the power
LOVE
BREATH
and
LOVE
are environment variables
The script should display the result, followed by a new line
julien
@production
-
503e7013
:~/
$
export
BREATH
=
4
julien
@production
-
503e7013
:~/
$
export
LOVE
=
3
julien
@production
-
503e7013
:~/
$
./
10
-love_exponent_breath
64
julien
@production
-
503e7013
:~/
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
10-love_exponent_breath
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath
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
Ã—
Students who are done with "10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>11. There are 10 types of people in the world -- Those who understand binary, and those who don't</summary>

**Files:**

- [`11-binary_to_decimal`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/11-binary_to_decimal)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
11. There are 10 types of people in the world -- Those who understand binary, and those who don't
Write a script that converts a number from base 2 to base 10.
The number in base 2 is stored in the environment variable
BINARY
The script should display the number in base 10, followed by a new line
julien
@production
-
503e7013
:~/
$
export
BINARY
=
10100111001
julien
@production
-
503e7013
:~/
$
./
11
-binary_to_decimal
1337
julien
@production
-
503e7013
:~/
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
11-binary_to_decimal
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
11. There are 10 types of people in the world -- Those who understand binary, and those who don't
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
Ã—
Students who are done with "11. There are 10 types of people in the world -- Those who understand binary, and those who don't"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>12. Combination</summary>

**Files:**

- [`12-combinations`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/12-combinations)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
12. Combination
Create a script that prints all possible combinations of two letters, except
oo
.
Letters are lower cases, from
a
to
z
One combination per line
The output should be alpha ordered, starting with
aa
Do not print
oo
Your script file should contain maximum 64 characters
julien
@ubuntu
:/tmp/
0x03
$
echo
$(
(
26
**
2
-
1
))
675
julien
@ubuntu
:/tmp/
0x03
$
./
12
-combinations |
wc -l
675
julien@ubuntu:/tmp/0x03$
julien@ubuntu:/tmp/0x03$ ./12-combinations
| tail -
303
|
head -10
oi
oj
ok
ol
om
on
op
oq
or
os
julien@ubuntu:/tmp/0x03$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
12-combinations
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
12. Combination
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
Ã—
Students who are done with "12. Combination"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>13. Floats</summary>

**Files:**

- [`13-print_float`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/13-print_float)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
13. Floats
Write a script that prints a number with two decimal places, followed by a new line.
The number will be stored in the environment variable
NUM
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
:~/
0x03
$
export
NUM
=
0
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
:~/
0x03
$
./
13
-print_float
0.00
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
:~/
0x03
$
export
NUM
=
98
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
:~/
0x03
$
./
13
-print_float
98.00
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
:~/
0x03
$
export
NUM
=
3.14159265359
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
:~/
0x03
$
./
13
-print_float
3.14
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
:~/
0x03
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
13-print_float
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
13. Floats
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
Ã—
Students who are done with "13. Floats"
Ã—
Recommended Sandboxes
Loading...
```

</details>

<details>
<summary>14. Decimal to Hexadecimal</summary>

**Files:**

- [`14-decimal_to_hexadecimal`](https://github.com/Antgst/holbertonschool-shell/blob/main/init_files_variables_and_expansions/14-decimal_to_hexadecimal)

**Repository:** `holbertonschool-shell`

**Directory:** `init_files_variables_and_expansions`

**Task details:**

```text
14. Decimal to Hexadecimal
Write a script that converts a number from base 10 to base 16.
The number in base 10 is stored in the environment variable
DECIMAL
The script should display the number in base 16, followed by a new line
julien
@production
-
503e7013
:~/
$
export
DECIMAL
=
16
julien
@production
-
503e7013
:~/
$
./
14
-decimal_to_hexadecimal
10
julien
@production
-
503e7013
:~/
$
export
DECIMAL
=
1337
julien
@production
-
503e7013
:~/
$
./
14
-decimal_to_hexadecimal |
cat -e
539$
julien@production-503e7013:~/$ export DECIMAL=15
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal
| cat -e
f
$
julien
@production
-
503e7013
:~/
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
init_files_variables_and_expansions
File:
14-decimal_to_hexadecimal
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
Select a repositoryâ€¦
Folder (optional)
Run the correction
Get a sandbox
QA Review
Ã—
14. Decimal to Hexadecimal
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
Ã—
Students who are done with "14. Decimal to Hexadecimal"
Ã—
Recommended Sandboxes
Loading...
```

</details>


---

## ðŸ§ª Testing

Use the provided task examples and Holberton checker to validate the project.

---

## ðŸ‘¤ Author

Project from Holberton School.

README generated with Antoine's README Factory workflow.
