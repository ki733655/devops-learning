DEVOPS INTERNSHIP
TASK 5: PROCESS MANAGEMENT IN LINUX

Name: Khairul Islam
Task No: 5
Topic: Process Management in Linux


1. INTRODUCTION

Process management is an important part of Linux system administration and DevOps. 
A process is a program that is currently running in the system. Linux provides various commands to manage and monitor processes. 
In this task, I learned how to list running processes, kill processes, understand process states, manage services using systemctl, and monitor system resources.


2. TOOLS USED

1. Linux Command Line Interface (CLI)
2. ps command
3. top command
4. kill command
5. systemctl


3. LISTING RUNNING PROCESSES

To list all running processes, the following command was used:

ps aux

This command displays all processes running in the system.
Here:
a shows processes of all users,
u shows user-oriented output,
x shows background processes.

Another command used is:

top

The top command shows real-time running processes.
It displays CPU usage, memory usage, process ID, and process states.
It is useful for monitoring system performance.


4. KILLING PROCESSES

To stop a process normally, the kill command is used:

kill PID

This sends a termination signal to the process and allows it to stop safely.

To forcefully stop a process, the following command is used:

kill -9 PID

This immediately terminates the process.
This command should be used only when the normal kill command does not work.


5. PROCESS STATES IN LINUX

Linux processes can have the following states:

R – Running
S – Sleeping
D – Uninterruptible sleep (waiting for I/O)
T – Stopped
Z – Zombie

Zombie processes do not consume system resources but indicate that the parent process has not cleared them properly.


6. MANAGING SERVICES USING SYSTEMCTL

systemctl is used to manage services in Linux systems.

To start a service:
sudo systemctl start nginx

To stop a service:
sudo systemctl stop nginx

To check service status:
sudo systemctl status nginx

To enable a service at boot:
sudo systemctl enable nginx

To disable a service at boot:
sudo systemctl disable nginx


7. MONITORING RESOURCE USAGE

To monitor CPU and memory usage:
top

To check memory usage:
free -h

To check disk usage:
df -h

These commands help in analyzing system performance and resource consumption.


8. OBSERVATIONS

1. Every running process has a unique PID.
2. top command is useful for real-time monitoring.
3. High CPU usage makes the system slow.
4. kill -9 should be used carefully.
5. systemctl simplifies service management.


9. INTERVIEW QUESTIONS AND ANSWERS

Q1. What is PID?
PID stands for Process ID. It is a unique number assigned to each running process.

Q2. Difference between kill and kill -9?
kill stops a process gracefully.
kill -9 forcefully terminates a process.

Q3. What is a daemon?
A daemon is a background process that runs continuously and provides system services.

Q4. What is systemctl?
systemctl is a command-line tool used to manage system services.

Q5. What happens when CPU usage spikes?
The system becomes slow, applications respond slowly, and overall performance degrades.




