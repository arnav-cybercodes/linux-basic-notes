# 🐧 Linux Learning Journey (Beginner → Foundation)

## 📌 Overview
This repository documents my hands-on journey learning Linux from scratch.  
It covers terminal basics, file management, permissions, searching, and essential command-line utilities.

---

# 🚀 Terminal Basics

## 🖥️ What I Learned
- How to open and close terminal  
- Adjust font size  
- Clear terminal screen  
- Pause and terminate processes  

---

## ⌨️ Important Shortcuts

| Shortcut | Function |
|----------|----------|
| Ctrl + Alt + T | Open terminal |
| Ctrl + C | Stop running process |
| Ctrl + Z | Pause process |
| Ctrl + L | Clear screen |
| Ctrl + A | Move cursor to beginning |
| Ctrl + E | Move cursor to end |

---

# 📂 Basic Linux Commands

| Command | Function | Example |
|--------|---------|--------|
| pwd | Shows current working directory | pwd |
| ls | Lists files and directories | ls |
| cd | Changes directory | cd Documents |
| touch | Creates empty file | touch file.txt |
| echo | Writes text into file | echo "Hello" > file.txt |
| cat | Displays file content | cat file.txt |
| rm | Deletes file | rm file.txt |
| mkdir | Creates directory | mkdir folder |
| mv | Moves or renames file | mv password.txt test.txt |

---

# 🧠 Text Editors

## ✏️ Vim
- Advanced terminal-based editor  
- Uses modes (Insert, Command)  
- Powerful but requires practice  

## ✏️ Nano
- Beginner-friendly  
- Simple and easy to use  

---

# 🔐 Directory & File Permissions

## 📌 Definition
File permissions control who can:
- Read (r)
- Write (w)
- Execute (x)

Permissions are divided into:
- User (Owner)
- Group
- Others  

---

## 🔢 Permission Format

Example:
```bash
-rwxr-xr--
Breakdown:
rwx → Owner permissions
r-x → Group permissions
r-- → Others permissions
🧩 chmod (Change Permissions)
🔹 Symbolic Method
Command
Function
Example
chmod u+x file
Add execute permission to user
chmod u+x file.txt
chmod g-w file
Remove write from group
chmod g-w file.txt
🔹 Octal Method
Value
Permission
7
rwx
6
rw-
5
r-x
4
r--
Example:
Bash
chmod 755 file.txt
👉 Owner: rwx
👉 Group: r-x
👉 Others: r-x
👑 Root Access
Command
Function
Example
sudo bash
Opens root shell
sudo bash
👉 Gives full administrative privileges
👤 Ownership Management
Command
Function
Example
chown
Change file owner
chown user file.txt
chgrp
Change group ownership
chgrp group file.txt
🔍 Searching in Files
📌 grep (Global Regular Expression Print)
Definition
Searches for specific text inside files
Command
Function
Example
grep "text" file
Finds text in file
grep "dynamics" /etc/protocols
🔗 Pipe Operator (|)
📌 Definition
Used to pass output of one command as input to another
Example
Bash
cat file.txt | grep "hello"
👉 Takes output of cat and filters using grep
🔎 Finding Files
📌 locate Command
Definition
Finds files quickly using database
Command
Function
Example
locate --all "password"
Find all matching files
locate --all "password"
locate "password" | grep "/etc/passwd"
Filter results
locate "password" | grep "/etc/passwd"
locate --all -c filename
Count results
