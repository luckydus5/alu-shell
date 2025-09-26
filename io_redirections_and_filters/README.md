# Shell I/O Redirections and Filters – Practice (ALU)

This project is part of my learning journey at **ALU**.  
It focuses on **Shell I/O redirection, filters, and special characters** through hands-on practice.

---

## 📚 Resources

Read or watch:

- [Shell, I/O Redirection](https://www.gnu.org/software/bash/manual/html_node/Redirections.html)
- [Special Characters](https://tldp.org/LDP/abs/html/special-chars.html)

Man or help pages to check:

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
- `passwd (5)` → `man 5 passwd`

---

## 🎯 Learning Objectives

By the end of this project, I will be able to explain (without using Google):

### Shell I/O Redirection
- What do the commands `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr` do  
- How to redirect standard output to a file  
- How to get standard input from a file instead of the keyboard  
- How to send the output from one program to the input of another program  
- How to combine commands and filters with redirections  

### Special Characters
- What are special characters  
- Understand white spaces, single quotes, double quotes, backslash, comments, pipes, command separators, tilde  
- When and how to use each  

### Other Man Pages
- How to display a line of text  
- How to concatenate files and print on the standard output  
- How to reverse a string  
- How to remove sections from each line of files  
- What is the `/etc/passwd` file and its format  
- What is the `/etc/shadow` file and its format  

---

## 📋 Requirements

- **Allowed editors:** `vi`, `vim`, `emacs`  
- All scripts will be tested on **Ubuntu 20.04 LTS**  
- All scripts must be **exactly two lines long** (`wc -l file` should print `2`)  
- All files must end with a **new line**  
- The first line of every file should be exactly:  

  ```bash
  #!/bin/bash

