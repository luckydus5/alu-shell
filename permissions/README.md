# 📂 Shell Permissions Project

This project explores **Linux file permissions**, ownership, and user management.  
All scripts are written in **Bash**, tested on **Ubuntu 20.04 LTS**, and follow strict requirements.

---

## 📖 Resources
Read or watch:
- `man` or `help` for:  
  `chmod`, `sudo`, `su`, `chown`, `chgrp`, `id`, `groups`, `whoami`, `adduser`, `useradd`, `addgroup`

---

## 🎯 Learning Objectives
By the end of this project, you should be able to explain:

- File **permissions** in Linux  
- What the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do  
- How to represent permissions for **owner, group, and other** as a single digit  
- How to change permissions, owner, and group of a file  
- Why a normal user cannot `chown` a file  
- How to run a command with root privileges (`sudo`, `su`)  
- How to change user ID or become superuser  
- How to create a user and a group  
- How to print real/effective user and group IDs  
- How to print the groups a user belongs to  
- How to print the effective user ID  

---

## ⚙️ Requirements
- Editors allowed: `vi`, `vim`, `emacs`
- Scripts will be tested on **Ubuntu 20.04 LTS**
- Each script must be **2 lines long** (`wc -l file` → `2`)
- Each file ends with a new line
- First line always:  
  ```bash
  #!/bin/bash

