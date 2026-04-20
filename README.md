# 🐧 Linux Learning Journey (Beginner → Foundation)

## 📌 Overview
This repository documents my hands-on journey learning Linux from scratch.  
It covers terminal basics, file management, permissions, searching, and essential commands.

---

# 🚀 Terminal Basics

## 🖥️ What I Learned
- Opening and closing terminal  
- Adjusting font size  
- Clearing terminal  
- Pausing and stopping processes  

---

## ⌨️ Shortcut Keys

| Shortcut | Function |
|----------|----------|
| Ctrl + Alt + T | Open terminal |
| Ctrl + C | Stop running process |
| Ctrl + Z | Pause process |
| Ctrl + L | Clear screen |
| Ctrl + A | Move cursor to start |
| Ctrl + E | Move cursor to end |

---

# 📂 Basic Linux Commands

| Command | Function | Example |
|--------|---------|--------|
| pwd | Show current directory | pwd |
| ls | List files | ls |
| cd | Change directory | cd Documents |
| touch | Create file | touch file.txt |
| echo | Write text to file | echo "Hello" > file.txt |
| cat | Read file | cat file.txt |
| rm | Delete file | rm file.txt |
| mkdir | Create directory | mkdir folder |
| mv | Move / Rename file | mv password.txt test.txt |

---

# 🧠 Text Editors

| Editor | Description |
|--------|------------|
| Vim | Advanced editor with modes (Insert, Command) |
| Nano | Simple and beginner-friendly |

---

# 🔐 File & Directory Permissions

## 📌 Definition
Permissions decide who can read, write, or execute a file.

- r → Read  
- w → Write  
- x → Execute  

Users:
- User (Owner)  
- Group  
- Others  

---

## 🔢 Permission Format

Example:
-rwxr-xr--

Breakdown:
- rwx → Owner  
- r-x → Group  
- r-- → Others  

---

# 🧩 chmod (Change Permissions)

## Symbolic Method

| Command | Function | Example |
|--------|---------|--------|
| chmod u+x file | Add execute to user | chmod u+x file.txt |
| chmod g-w file | Remove write from group | chmod g-w file.txt |

---

## Octal Method

| Value | Permission |
|------|-----------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |

Example:
chmod 755 file.txt

Meaning:
- Owner → rwx  
- Group → r-x  
- Others → r-x  

---

# 👑 Root Access

| Command | Function |
|--------|---------|
| sudo bash | Open root shell |

Gives full administrative control.

---

# 👤 Ownership Commands

| Command | Function | Example |
|--------|---------|--------|
| chown | Change owner | chown user file.txt |
| chgrp | Change group | chgrp group file.txt |

---

# 🔍 Searching in Files

| Command | Function | Example |
|--------|---------|--------|
| grep "text" file | Search text in file | grep "dynamics" /etc/protocols |

---

# 🔗 Pipe Operator

## Definition
Pass output of one command to another.

Example:
cat file.txt | grep "hello"

---

# 🔎 Finding Files

| Command | Function | Example |
|--------|---------|--------|
| locate --all "password" | Find files | locate --all "password" |
| locate "password" \| grep "/etc/passwd" | Filter results | locate "password" \| grep "/etc/passwd" |
| locate --all -c filename | Count results | locate --all -c filename |

---

# 🧭 Key Learnings

- Navigating filesystem  
- Managing files and directories  
- Understanding permissions  
- Using search tools  
- Combining commands  

---
