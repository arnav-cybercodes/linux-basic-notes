# 🐧 Linux Basics Journey (Beginner → Intermediate)

## 📌 Overview
This repository documents my **Linux learning journey**, starting from absolute basics to essential command-line skills, permissions, and file management.

---

# 🚀 Getting Started with Terminal

## 🖥️ Basic Terminal Usage
- Open Terminal  
- Close Terminal  
- Adjust font size  
- Clear screen  
- Pause/stop processes  
- End processes  

---

## ⌨️ Important Shortcut Keys

- `Ctrl + Alt + T` → Open terminal  
- `Ctrl + C` → Stop running process  
- `Ctrl + Z` → Pause process  
- `Ctrl + L` → Clear screen  
- `Ctrl + A` → Move cursor to start  
- `Ctrl + E` → Move cursor to end  

---

# 📂 Basic Linux Commands

## 📍 Current Directory
```bash
pwd
📄 List Files
Bash
ls
📁 Change Directory
Bash
cd <directory>
📄 Create File
Bash
touch file.txt
📝 Write Text
Bash
echo "Hello" > file.txt
📖 Read File
Bash
cat file.txt
❌ Delete File
Bash
rm file.txt
📁 Create Directory
Bash
mkdir folder
🔄 Move / Rename File
Bash
mv password.txt test.txt
🧠 Text Editors
✏️ Vim
Advanced terminal editor
Works with modes (Insert, Command)
✏️ Nano
Beginner-friendly
Easy and simple to use
🔐 File Permissions
📌 Basics
Read (r)
Write (w)
Execute (x)
🧩 chmod (Symbolic Method)
Bash
chmod u+x file.txt
🔢 chmod (Octal Method)
Bash
chmod 755 file.txt
👑 Root Access
🔓 Open Root Shell
Bash
sudo bash
👉 Gives full administrative control
👤 Ownership Commands
Change Owner
Bash
chown user file.txt
Change Group
Bash
chgrp group file.txt
🔍 Searching in Files
grep command
Bash
grep "dynamics" /etc/protocols
🔗 Pipe Operator (|)
👉 Used to combine commands
Example:
Bash
cat file.txt | grep "hello"
🔎 Finding Files
📍 locate command
Bash
locate --all "password"
Combine with grep
Bash
locate "password" | grep "/etc/passwd"
Count Results
Bash
locate --all -c filename
