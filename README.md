# 🖥️ Linux System Info Dashboard (Bash)

A beginner → intermediate Linux scripting project that generates a system information dashboard directly in the terminal using Bash and standard Linux CLI tools.
The script provides a quick overview of system health, usage statistics, and running processes in a clean and formatted output.

---

## 🎯 Project Goals

This project aims to:

Practice Bash scripting fundamentals
Use Linux command-line tools to collect system data
Display formatted system statistics in the terminal
Build a small but real DevOps-style utility script

---

## The script prints a dashboard including

System identity, Uptime, Memory usage, Disk usage, Running processes, CPU usage, Warning  messages when resources are low

---

## 🛠 Tech Stack

**Language**
-Bash (Shell scripting)

**Linux command-line tools Used**
-whoami
-hostname
-date
-uptime
-free
-df
-ps
-grep
-awk
-head
-top

**Other Tools**
-Git & GitHub

---

## 🖥 Features

-Displays system identity (user, hostname, date)
-Shows system uptime in human-readable format
-Displays memory usage (Total / Used / Free)
-Displays disk usage for root partition
-Counts total running processes
-Shows Top 5 memory-consuming processes
-Displays real-time CPU usage
-Color-coded terminal output (green / red warnings)
-Warning alerts when Free memory is low  and Disk space is low
-Clean and structured terminal dashboard

---

## 📷 Example Output

    =======================================
             SYSTEM INFO
    =======================================
    User: mike
    Hostname: mike
    Date: Wed Apr 08 15:42:17 
    ---------------------------------------
    -----------------Uptime-----------------
    up 5 hours, 24 minutes

    ----------------Memory (MB)--------------
    Total: 15974 MB | Used: 8026 MB | Free: 423 MBI

    -----------------Disk Usage---------------
    Total: 129G | Used: 23G | Free: 99G

    ------------------Processes---------------
    Running: 334 
    Top 5 Memory-Consuming Processes:
    ------------------------------------------
    PID: PID    | MEM: %MEM   | CMD: COMMAND
    PID: 6496   | MEM: 4.3    | CMD: /opt/google/chrome/chrome
    PID: 7082   | MEM: 4.0    | CMD: /opt/google/chrome/chrome
    PID: 17723  | MEM: 3.5    | CMD: /opt/google/chrome/chrome
    PID: 3580   | MEM: 3.4    | CMD: /snap/firefox/8054/usr/lib/firefox/firefox
    PID: 3797   | MEM: 3.4    | CMD: /opt/google/chrome/chrome 

    WARNING: Low memory! Only 423MB free. 
    High disk space 99GMB 

    CPU Usage
    ------------------------------------------
    Current CPU Usage: 7.4%

    =============================================
                    Dashboard OK         
    =============================================

---

## ⚙ Installation & Setup

    ```Clone the repository:

git clone <https://github.com/mike2377/system_info_dashbord.git>
cd system_info_dashbord

Give execution permission to the script:

chmod +x sysinfo.sh

Run the script:

./sysinfo.sh

---

## 📁 Project Structure

sysinfo-dashboard/
│
├── sysinfo.sh
└── README.md

🧠 Challenges Faced
Parsing command output using awk and grep
Formatting terminal output cleanly
Extracting numeric values for comparisons
Implementing color-coded warnings in Bash
Calculating CPU usage from top command output

📚 What I Learned
Writing structured Bash scripts
Using command substitution $(...)
Working with Linux system monitoring commands
Parsing CLI output with awk
Creating readable terminal dashboards
Adding logic and conditional warnings in Bash

🚀 Future Improvements
Add command-line flags:
--compact
--verbose
Save output to a log file
Add system temperature monitoring
Add network usage statistics
Convert into a cron job for periodic monitoring

👨🏽‍💻 Author
Kembou Keumoe Ivan Michael
Junior Fullstack Developer
📩 Email: <kman39457@email.com>
🌍 Based in Cameroon | Open to remote opportunities
