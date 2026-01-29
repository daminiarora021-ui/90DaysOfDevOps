## Linux Architecture 



![arch](https://github.com/user-attachments/assets/0a8a14f0-5b5e-47cc-972d-09f894f84f7a)

## The core components of Linux (kernel, user space, init/systemd)
# Kernel
The heart of Linux. intermediator between hardware and software. Machine understands kernel language which is in c program .
kernel manage process , memory , device , file system , networking , security and permission .

# user space 
where application , shell , utilities and library runs .

# init / systemmd
The first process to start after the kernel boots (PID 1)
initializing the system and managing all other services


## How processes are created and managed
An instance of a program that is currently running is called process 
- Each process has a unique PID , which startes from 1


## Explain **process states** (running, sleeping, zombie, etc.)
running : Active process.
sleeping : Idle process.
Stopped : paused or suspended process 
Zombie : The process has terminated , in this child process has finished, but the parent process has not yet called to read its exit status.


## What systemd does and why it matters
The modern system and service manager for Linux, replacing traditional SysVinit.
Systemd is the default system and service manager for most modern Linux distributions, acting as PID 1 (the initial process) to boot the user space and manage services, mounting, and system state


##  List **5 commands** you would use daily
pwd               Present work directory 
df -h             Displays disk space usage in human readable format  
ps aux            Display all processes for all users 
Top               Display real time CPU & Memory usage 
system clt        starting, stopping, restarting, or reloading a daemon 
