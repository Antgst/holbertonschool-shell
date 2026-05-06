# 📘 Shell, permissions

## 📌 Description

_No description detected._

---

## 📚 Resources

**Read or watch**:


- [Permissions](http://linuxcommand.org/lc3_lts0090.php)


**man or help**:


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

---

## 🎯 Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), __without the help of Google__:


### Permissions


- What do the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do

- Linux file permissions

- How to represent each of the three sets of permissions (owner, group, and other) as a single digit

- How to change permissions, owner and group of a file

- Why can't a normal user `chown` a file

- How to run a command with root privileges

- How to change user ID or become superuser


### Other Man Pages


- How to create a user

- How to create a group

- How to print real and effective user and group IDs

- How to print the groups a user is in

- How to print the effective userid

---

## ✅ Requirements

### General


- Allowed editors: `vi`, `vim`, `emacs`

- All your scripts will be tested on Ubuntu 22.04 LTS

- All your scripts should be exactly two lines long (`$ wc -l file` should print 2)

- All your files should end with a new line (<a href="http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789">why?</a>)

- The first line of all your files should be exactly `#!/bin/bash`

- A `README.md` file, at the root of the folder of the project, describing what each script is doing

- You are not allowed to use backticks, `&&`, `||` or `;`

- All your files must be executable


**Warning: tasks 3 / 13 / 14 / 15 / 16 must be done inside the sandbox in order to be corrected by the checker.**

---

## ⚙️ Setup

_No specific setup detected._

---

## 🧠 Quiz

<details>
<summary>Question #0</summary>

**Question:** Which command should I use for changing a file permission?

**Available answers:**

- `su`
- `chmod`
- `chown`
- `chgrp`

**Answer:** `chmod`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #1</summary>

**Question:** Which command should I use for changing a file owner?

**Available answers:**

- `su`
- `chmod`
- `chown`
- `chgrp`

**Answer:** `chown`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #2</summary>

**Question:** What is the permission value for a file without any restriction?

**Available answers:**

- `600`
- `644`
- `777`

**Answer:** `777`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #3</summary>

**Question:** What is the permission value for a file read only for the group owner?

**Available answers:**

- `040`
- `050`
- `060`
- `070`

**Answer:** `040`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #4</summary>

**Question:** What is the numerical value for the rwx------ permission?

**Available answers:**

- `600`
- `621`
- `704`
- `700`

**Answer:** `700`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #5</summary>

**Question:** What is the numerical value for the r-xr--r-- permission?

**Available answers:**

- `522`
- `544`
- `644`
- `411`

**Answer:** `544`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>

<details>
<summary>Question #6</summary>

**Question:** What is the numerical value for the ----w---x permission?

**Available answers:**

- `123`
- `121`
- `221`
- `021`

**Answer:** `021`

**Explanation / tip:**

_To be reviewed and completed manually if needed._

</details>


---

## 🧩 Tasks

<details>
<summary>0. My name is Betty</summary>

**Files:**

- [`0-iam_betty`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/0-iam_betty)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
0. My name is Betty
Create a script that switches the current user to the user
betty
.
You should use exactly 8 characters for your command (+1 character for the new line)
You can assume that the user
betty
will exist when we will run your script
julien
@ubuntu
:/tmp/h
$
tail -
1
0
-iam_betty |
wc -c
9
julien@ubuntu:/tmp/h$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
0-iam_betty
0. My name is Betty
---
---
---
---
---
```

</details>

<details>
<summary>1. Who am I</summary>

**Files:**

- [`1-who_am_i`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/1-who_am_i)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
1. Who am I
Write a script that prints the effective username of the current user.
julien
@ubuntu
:/tmp/h
$
./
1
-who_am_i
julien
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
1-who_am_i
1. Who am I
---
---
---
---
---
```

</details>

<details>
<summary>2. Groups</summary>

**Files:**

- [`2-groups`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/2-groups)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
2. Groups
Write a script that prints all the groups the current user is part of.
julien
@ubuntu
:/tmp/h
$
./
2
-groups
julien adm cdrom sudo dip plugdev lpadmin sambashare
julien
@ubuntu
:/tmp/h
$
Note: depending on the user, you will get a different output.
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
2-groups
2. Groups
---
---
---
---
---
```

</details>

<details>
<summary>3. New owner</summary>

**Files:**

- [`3-new_owner`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/3-new_owner)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
3. New owner
Write a script that changes the owner of the file
hello
to the user
betty
.
julien
@ubuntu
:/tmp
$
ls -l
total
4
-rwxrw-r--
1
julien julien
30
Sep
20
14
:
23
3
-new_owner
-rw-rw-r--
1
julien julien
0
Sep
20
14
:
18
hello
julien
@ubuntu
:/tmp
$
sudo ./
3
-new_owner
julien
@ubuntu
:/tmp
$
ls -l
total
4
-rwxrw-r--
1
julien julien
30
Sep
20
14
:
23
3
-new_owner
-rw-rw-r--
1
betty  julien
0
Sep
20
14
:
18
hello
julien
@ubuntu
:/tmp
$
The script must be present on the github repository and on the sandbox inside the folder /tmp
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
3-new_owner
3. New owner
---
---
---
---
---
```

</details>

<details>
<summary>4. Empty!</summary>

**Files:**

- [`4-empty`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/4-empty)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
4. Empty!
Write a script that creates an empty file called
hello
.
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
4-empty
4. Empty!
---
---
---
---
---
```

</details>

<details>
<summary>5. Execute</summary>

**Files:**

- [`5-execute`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/5-execute)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
5. Execute
Write a script that adds execute permission to the owner of the file
hello
.
The file
hello
will be in the working directory
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
26
5
-execute
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./hello
bash:
./
hello:
Permission
denied
julien
@ubuntu
:/tmp/h
$
./
5
-execute
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
26
5
-execute
-rwxrw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
5-execute
5. Execute
---
---
---
---
---
```

</details>

<details>
<summary>6. Multiple permissions</summary>

**Files:**

- [`6-multiple_permissions`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/6-multiple_permissions)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
6. Multiple permissions
Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file
hello
.
The file
hello
will be in the working directory
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
36
Sep
20
14
:
31
6
-multiple_permissions
-rw-r-----
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./
6
-multiple_permissions
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
36
Sep
20
14
:
31
6
-multiple_permissions
-rwxr-xr--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
6-multiple_permissions
6. Multiple permissions
---
---
---
---
---
```

</details>

<details>
<summary>7. Everybody!</summary>

**Files:**

- [`7-everybody`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/7-everybody)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
7. Everybody!
Write a script that adds execution permission to the owner, the group owner and the other users, to the file
hello
The file
hello
will be in the working directory
You are not allowed to use commas for this script
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
35
7
-everybody
-rw-r-----
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./
7
-everybody
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
35
7
-everybody
-rwxr-x--x
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
7-everybody
7. Everybody!
---
---
---
---
---
```

</details>

<details>
<summary>8. James Bond</summary>

**Files:**

- [`8-James_Bond`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/8-James_Bond)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
8. James Bond
Write a script that sets the permission to the file
hello
as follows:
Owner: no permission at all
Group: no permission at all
Other users: all the permissions
The file
hello
will be in the working directory
You are not allowed to use commas for this script
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
40
8
-
James
_Bond
-rwxr-x--x
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./
8
-
James
_Bond
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
28
Sep
20
14
:
40
8
-
James
_Bond
-------rwx
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
8-James_Bond
8. James Bond
---
---
---
---
---
```

</details>

<details>
<summary>9. John Doe</summary>

**Files:**

- [`9-John_Doe`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/9-John_Doe)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
9. John Doe
Write a script that sets the mode of the file
hello
to this:
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
The file
hello
will be in the working directory
You are not allowed to use commas for this script
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
9-John_Doe
9. John Doe
---
---
---
---
---
```

</details>

<details>
<summary>10. Look in the mirror</summary>

**Files:**

- [`10-mirror_permissions`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/10-mirror_permissions)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
10. Look in the mirror
Write a script that sets the mode of the file
hello
the same as
olleh
’s mode.
The file
hello
will be in the working directory
The file
olleh
will be in the working directory
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
42
Sep
20
14
:
45
10
-mirror_permissions
-rwxr-x-wx
1
julien julien
23
Sep
20
14
:
25
hello
-rw-rw-r--
1
julien julien
0
Sep
20
14
:
43
olleh
julien
@ubuntu
:/tmp/h
$
./
10
-mirror_permissions
julien
@ubuntu
:/tmp/h
$
ls -l
total
8
-rwxrw-r--
1
julien julien
42
Sep
20
14
:
45
10
-mirror_permissions
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
-rw-rw-r--
1
julien julien
0
Sep
20
14
:
43
olleh
julien
@ubuntu
:/tmp/h
$
Note: the mode of
olleh
will not always be 664. Make sure your script works for any mode.
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
10-mirror_permissions
10. Look in the mirror
---
---
---
---
---
```

</details>

<details>
<summary>11. Directories</summary>

**Files:**

- [`11-directories_permissions`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/11-directories_permissions)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
11. Directories
Create a script that adds execute permission to all subdirectories of the current directory for  the owner, the group owner and all other users. Regular files should not be changed.
julien
@ubuntu
:/tmp/h
$
ls -l
total
20
-rwxrwxr-x
1
julien julien
24
Sep
20
14
:
53
11
-directories_permissions
drwx------
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx------
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx------
2
julien julien
4096
Sep
20
14
:
49
dir2
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./
11
-directories_permissions
julien
@ubuntu
:/tmp/h
$
ls -l
total
20
-rwxrwxr-x
1
julien julien
24
Sep
20
14
:
53
11
-directories_permissions
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
11-directories_permissions
11. Directories
---
---
---
---
---
```

</details>

<details>
<summary>12. More directories</summary>

**Files:**

- [`12-directory_permissions`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/12-directory_permissions)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
12. More directories
Create a script that creates a directory called
my_dir
with permissions 751 in the working directory.
julien
@ubuntu
:/tmp/h
$
ls -l
total
20
-rwxrwxr-x
1
julien julien
39
Sep
20
14
:
59
12
-directory_permissions
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
./
12
-directory_permission s
julien
@ubuntu
:/tmp/h
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
39
Sep
20
14
:
59
12
-directory_permissions
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
drwxr-x--x
2
julien julien
4096
Sep
20
14
:
59
my_dir
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp/h
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
12-directory_permissions
12. More directories
---
---
---
---
---
```

</details>

<details>
<summary>13. Change group</summary>

**Files:**

- [`13-change_group`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/13-change_group)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
13. Change group
Write a script that changes the group owner to
school
for the file
hello
The file
hello
will be in the working directory
The script must be present on the github repository and on the sandbox on the folder /tmp
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
34
Sep
20
15
:
03
13
-change_group
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
drwxr-x--x
2
julien julien
4096
Sep
20
14
:
59
my_dir
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
sudo ./
13
-change_group
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
34
Sep
20
15
:
03
13
-change_group
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
drwxr-x--x
2
julien julien
4096
Sep
20
14
:
59
my_dir
-rw-rw-r--
1
julien school
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
13-change_group
13. Change group
---
---
---
---
---
```

</details>

<details>
<summary>14. Owner and group</summary>

**Files:**

- [`14-change_owner_and_group`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/14-change_owner_and_group)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
14. Owner and group
Write a script that changes the owner to
vincent
and the group owner to
staff
for all the files and directories in the working directory.
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
36
Sep
20
15
:
06
14
-change_owner_and_group
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
julien julien
4096
Sep
20
14
:
49
dir2
drwxr-x--x
2
julien julien
4096
Sep
20
14
:
59
my_dir
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
sudo ./
14
-change_owner_and_group
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
vincent staff
36
Sep
20
15
:
06
14
-change_owner_and_group
drwx--x--x
2
vincent staff
4096
Sep
20
14
:
49
dir0
drwx--x--x
2
vincent staff
4096
Sep
20
14
:
49
dir1
drwx--x--x
2
vincent staff
4096
Sep
20
14
:
49
dir2
drwxr-x--x
2
vincent staff
4096
Sep
20
14
:
59
my_dir
-rw-rw-r--
1
vincent staff
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
The script must be present on the github repository and on the sandbox inside the folder /tmp
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
14-change_owner_and_group
14. Owner and group
---
---
---
---
---
```

</details>

<details>
<summary>15. Symbolic links</summary>

**Files:**

- [`15-symbolic_link_permissions`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/15-symbolic_link_permissions)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
15. Symbolic links
Write a script that changes the owner and the group owner of
_hello
to
vincent
and
staff
respectively.
The file
_hello
is in the working directory
The file
_hello
is a symbolic link
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
44
Sep
20
15
:
12
15
-symbolic_link_permissions
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
lrwxrwxrwx
1
julien julien
5
Sep
20
15
:
10
_hello -> hello
julien
@ubuntu
:/tmp
$
sudo ./
15
-symbolic_link_permissions
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
44
Sep
20
15
:
12
15
-symbolic_link_permissions
-rw-rw-r--
1
julien julien
23
Sep
20
14
:
25
hello
lrwxrwxrwx
1
vincent  staff
5
Sep
20
15
:
10
_hello -> hello
julien
@ubuntu
:/tmp
$
The script must be present on the github repository and on the sandbox inside the folder /tmp
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
15-symbolic_link_permissions
15. Symbolic links
---
---
---
---
---
```

</details>

<details>
<summary>16. If only</summary>

**Files:**

- [`16-if_only`](https://github.com/Antgst/holbertonschool-shell/blob/main/permissions/16-if_only)

**Repository:** `holbertonschool-shell`

**Directory:** `permissions`

**Task details:**

```text
16. If only
Write a script that changes the owner of the file
hello
to
vincent
only if it is owned by the user
guillaume
.
The file
hello
will be in the working directory
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien    julien
47
Sep
20
15
:
18
16
-if_only
-rw-rw-r--
1
guillaume julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
sudo ./
16
-if_only
julien
@ubuntu
:/tmp
$
ls -l
total
24
-rwxrwxr-x
1
julien julien
47
Sep
20
15
:
18
16
-if_only
-rw-rw-r--
1
vincent  julien
23
Sep
20
14
:
25
hello
julien
@ubuntu
:/tmp
$
The script must be present on the github repository and on the sandbox inside the folder /tmp
Repo:
GitHub repository:
holbertonschool-shell
Directory:
permissions
File:
16-if_only
16. If only
---
---
---
---
---
```

</details>


---

## 🧪 Testing

Use the provided task examples and Holberton checker to validate the project.

---

## 👤 Author

Project from Holberton School.

README generated with Antoine's README Factory workflow.
