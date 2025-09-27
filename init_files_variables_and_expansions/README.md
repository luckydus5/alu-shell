# 🐚 Shell, Init Files, Variables and Expansions

**Author:** Olivier Dusabamahor  
**Purpose:** Personal documentation & tracker of what I’ve learned and practiced in Bash scripting.

---

## 📚 Resources

Read or watch:

- Expansions  
- Shell Arithmetic  
- Variables  
- Shell initialization files  
- The alias Command  
- Technical Writing  

**man or help:**

- `printenv`  
- `set`  
- `unset`  
- `export`  
- `alias`  
- `unalias`  
- `.` (dot command)  
- `source`  
- `printf`  

---

## 🎯 Learning Objectives

At the end of this project, I should be able to explain to anyone (without Google):

### General
- What happens when you type `$ ls -l *.txt`

### Shell Initialization Files
- What are the `/etc/profile` file and the `/etc/profile.d` directory  
- What is the `~/.bashrc` file  

### Variables
- What is the difference between a local and a global variable  
- What is a reserved variable  
- How to create, update and delete shell variables  
- Roles of the following reserved variables: `HOME`, `PATH`, `PS1`  
- What are special parameters  
- What is the special parameter `$?`  

### Expansions
- What is expansion and how to use it  
- Difference between single and double quotes, and how to use them properly  
- How to do command substitution with `$()` and backticks  

### Shell Arithmetic
- How to perform arithmetic operations with the shell  

### The alias Command
- How to create an alias  
- How to list aliases  
- How to temporarily disable an alias  

### Other help pages
- How to execute commands from a file in the current shell  

---

## ⚙️ Requirements

- Allowed editors: `vi`, `vim`, `emacs`  
- Scripts will be tested on **Ubuntu 20.04 LTS**  
- Scripts must be exactly **two lines long** (`$ wc -l file` should print 2)  
- All files must end with a **new line**  
- First line of all files:  
  ```bash
  #!/bin/bash


🟢 Section 2: Beginner Practice Projects (Level 1–50)

Short 2–10 line scripts to build fundamentals.

File Operations

 Create a file named myfile.txt

 Append “Hello World” to myfile.txt

 Print the number of lines in a file

 Display only the first 5 lines of /etc/passwd

 Display the last 10 lines of a log file

Permissions & Ownership

 Create a script that makes a file read-only

 Change ownership of a file to another user

 Give execute permission only to the owner

 Remove all permissions for “others”

 Find all .sh files in the current directory and make them executable

Variables & Expansion

 Print your $USER

 Create and print a local variable

 Export a global variable

 Show the value of $HOME and $PATH

 Demonstrate difference between ' ' and " "

Redirection & Pipes

 Redirect stdout to a file

 Redirect stderr to a file

 Combine stdout and stderr into one file

 Count the number of words in /etc/passwd

 Extract usernames from /etc/passwd

Simple Loops

 Print numbers 1–10

 Print even numbers up to 20

 Print the multiplication table of 5

 Loop through files in a directory and print names

 Print “hello” 100 times using a loop

🟡 Section 3: Intermediate Projects (Level 51–120)

Scripts with logic, automation, and text processing.

System Monitoring

 Display system uptime

 Show current logged-in users

 Display top 10 processes by memory usage

 Check disk usage of /home

 Monitor CPU usage every 5 seconds

Text Processing

 Count unique words in a file

 Extract email addresses from a text file

 Replace all tabs with 4 spaces

 Sort lines in a file alphabetically

 Remove duplicate lines from a file

Scripting Automation

 Backup /etc/passwd to /tmp/passwd.bak

 Compress all .log files in /var/log

 Create daily timestamped backup of ~/Documents

 Write a script to clean temporary files (*.swp, *~)

 Create a log-rotating script that keeps only last 5 logs

Math & Arithmetic

 Calculate factorial of a number

 Generate Fibonacci series up to N

 Add all numbers from 1 to N

 Check if a number is prime

 Convert Celsius to Fahrenheit

Control Flow

 Check if a file exists

 Check if a number is positive, negative, or zero

 Print grade from marks (if/else ladder)

 Case statement: print day of the week from number

 Nested loops: print multiplication table 1–10

🔴 Section 4: Advanced Projects (Level 121–200)

Real-world level scripting.

Process & Job Control

 Find zombie processes

 Kill a process by name

 Monitor a process and restart if it stops

 Print parent PID of a process

 Log all background jobs into a file

Networking

 Ping a host and save results

 Check if a website is reachable (HTTP 200)

 Download a file using curl or wget

 Extract all URLs from a webpage

 Monitor open ports with netstat or ss

Security & Users

 List all users on the system

 Check if a user exists

 Create a new user with default password

 Lock and unlock a user account

 Monitor failed login attempts from logs

File Systems & Backups

 Create an incremental backup script with rsync

 Mount and unmount a partition

 Check filesystem usage (df, du)

 Find the 10 largest files in /home

 Monitor changes to /etc/passwd

Advanced Text/Data Processing

 Parse CSV file and print column 1

 Convert CSV → JSON using jq

 Search a log file for IP addresses

 Find all lines with numbers in a text file

 Extract lines between two patterns

Automation & APIs

 Send an email from bash

 Fetch weather data from an API with curl

 Check GitHub repo stars with curl

 Automate pushing commits to GitHub

 Monitor website SSL certificate expiry

Scripting Challenges

 Implement a simple calculator (add/sub/mul/div)

 Build a todo list manager in bash

 Write a number guessing game

 Implement a rock-paper-scissors game

 Password generator script

 Brute force zip password cracker with fcrackzip

 Automate system updates (apt update && apt upgrade)

 Build your own ls using for loop and stat

 Build your own cat with while read

 Shell-based “chat” program using named pipes

🎓 Learning Path

Level 1–50 → Build confidence with basics (redirection, variables, loops)

Level 51–120 → Text processing, system monitoring, automation

Level 121–200 → Real-world scripting (processes, networking, APIs, security)

✅ Conclusion

This README combines the original Julien Barbier project with 150+ practice projects from beginner → advanced.

👉 With these exercises, I will master:

Shell basics

Expansions & arithmetic

Redirection & pipes

Variables & environments

Automation scripts

Networking & security scripting

Real-world system administration
