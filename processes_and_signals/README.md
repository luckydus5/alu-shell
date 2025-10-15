🧠 Shell, Processes and Signals — Learning Content
📚 Resources

Before diving into practice, read or explore the following:

Linux PID

Linux Process

Linux Signal

man pages / help commands:

man ps

man pgrep

man pkill

man kill

man exit

man trap

🎯 Learning Objectives

By the end of this module, you’ll be able to explain (without looking up answers):

General

✅ What is a PID
✅ What is a process
✅ How to find a process’ PID
✅ How to kill a process
✅ What is a signal
✅ What are the 2 signals that cannot be ignored

🧩 Core Concepts
1️⃣ What is a PID?

PID (Process ID): A unique number assigned by the Linux kernel to each running process.

Every process (like a script, application, or service) has one.

You can display your script’s own PID using:

echo $$


To check a specific process PID:

pgrep bash
ps -ef | grep bash

2️⃣ What is a Process?

A process is any running instance of a program.

When you run a command (like sleep 5 or firefox), it becomes a process.

View running processes:

ps
ps aux        # Detailed view of all processes
top           # Real-time system monitoring

3️⃣ How to Find a Process’ PID

You can find PIDs in multiple ways:

ps aux | grep process_name
pgrep process_name


Example:

pgrep firefox


→ Outputs the PID(s) of all running firefox processes.

4️⃣ How to Kill a Process

To stop or terminate a process, use the kill command with its PID.

Examples:

kill 1234         # Sends the default SIGTERM signal (politely asks process to stop)
kill -9 1234      # Sends SIGKILL (forcefully terminates the process)


Or kill by process name:

pkill firefox

5️⃣ What is a Signal?

A signal is a way to communicate with processes.

Signals are messages sent by the OS or user to control processes (e.g., stop, pause, restart).

Example:

SIGTERM → ask the process to terminate gracefully

SIGKILL → force the process to stop immediately

SIGSTOP → pause (can be resumed later)

SIGINT → interrupt (usually from Ctrl + C)

List all signals:

kill -l

6️⃣ Signals That Cannot Be Ignored

Two signals cannot be caught or ignored:

SIGKILL (signal 9) → Immediately kills the process.

SIGSTOP (signal 19) → Suspends (pauses) the process.

These two bypass the process's signal handlers — the kernel enforces them directly.

⚙️ Requirements Recap

Allowed editors: vi, vim, emacs

Tested on Ubuntu 20.04 LTS

Each file must:

End with a new line

Be executable

Pass Shellcheck (0.7.0) validation

Start with:

#!/usr/bin/env bash
# Description of what the script does

📘 Extra Knowledge

If you want to dive deeper:
👉 List of all Linux signals (Wikipedia)

Would you like me to follow this up with a series of practice exercises (like “display own PID”, “show parent PID”, “kill process by name”, etc.) to go step-by-step through this module?
