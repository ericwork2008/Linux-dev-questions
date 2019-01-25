I just copy some questions I am interesting from some website
From http://www.codespaghetti.com/devops-interview-questions/#linux
#Question: What is Linux?
Linux is the best-known and most-used open source operating system. As an operating system, Linux is a software that sits underneath all of the other software on a computer, receiving requests from those programs and relaying these requests to the computer’s hardware.
In many ways, Linux is similar to other operating systems such as Windows, OS X, or iOS
But Linux also is different from other operating systems in many important ways.
First, and perhaps most importantly, Linux is open source software. The code used to create Linux is free and available to the public to view, edit, and—for users with the appropriate skills—to contribute to.
Linux operating system is consist of 3 components which are as below:
Kernel: Linux is a monolithic kernel that is free and open source software that is responsible for managing hardware resources for the users.
System Library: System Library plays a vital role because application programs access Kernels feature using system library.
System Utility: System Utility performs specific and individual level tasks.



#Question: What Is Difference Between Linux & Unix?
Unix and Linux are similar in many ways, and in fact, Linux was originally created to be similar to Unix.
Both have similar tools for interfacing with the systems, programming tools, filesystem layouts, and other key components.
However, Unix is not free. Over the years, a number of different operating systems have been created that attempted to be “unix-like” or “unix-compatible,” but Linux has been the most successful, far surpassing its predecessors in popularity.

//The following is answer from https://mindmajix.com/linux-interview-questions
Linux Is Just Kernal

All Linux distributions include GUI system, GNU utilities, installation & management tools, GNU c/c++ Compilers, Editors (vi), and various applications like OpenOffice, Firefox.

UNIX operating systems are considered as a complete OS as everything come from a single vendor.

License and cost

Linux is Free. You can download it from the Internet or redistribute it under GNU licenses. Most UNIX like operating systems are not free.

Security And Firewall

Linux comes with open source Netfilter and IPTables based firewall tool to protect your server and desktop from the crackers and hackers. UNIX operating systems comes with its own firewall products. 

Backup And Recovery

UNIX and Linux come with their own set of tools for backing up data to tape and other backup media. However, both Linux and UNIX share some common tools such as tar, dump/restore, and cpio etc.

#Question: What Is BASH?
BASH stands for Bourne Again Shell. BASH is the UNIX shell for the GNU operating system. So, BASH is the command language interpreter that helps you to enter your input, and thus you can retrieve information.
In a straightforward language, BASH is a program that will understand the data entered by the user and execute the command and gives output.

#Question: What Is Daemon In Linux?
A daemon is a type of program on Linux operating systems that runs unobtrusively in the background, rather than under the direct control of a user, waiting to be activated by the occurrence of a specific event or condition
Unix-like systems typically run numerous daemons, mainly to accommodate requests for services from other computers on a network, but also to respond to other programs and to hardware activity.
Examples of actions or conditions that can trigger daemons into activity are a specific time or date, passage of a specified time interval, a file landing in a particular directory, receipt of an e-mail or a Web request made through a particular communication line.
It is not necessary that the perpetrator of the action or condition be aware that a daemon is listening, although programs frequently will perform an action only because they are aware that they will implicitly arouse a daemon

#Question: What Is Process In Linux?
Daemons are usually instantiated as processes. A process is an executing (i.e., running) instance of a program.
Processes are managed by the kernel (i.e., the core of the operating system), which assigns each a unique process identification number (PID).
There are three basic types of processes in Linux:
-Interactive:Interactive processes are run interactively by a user at the command line
-Batch:Batch processes are submitted from a queue of processes and are not associated with the command line; they are well suited for performing recurring tasks when system usage is otherwise low.
-Daemon: Daemons are recognized by the system as any processes whose parent process has a PID of one

#Questions: What Is Linux Kernel?
A kernel is the lowest level of easily replaceable software that interfaces with the hardware in your computer.
It is responsible for interfacing all of your applications that are running in “user mode” down to the physical hardware, and allowing processes, known as servers, to get information from each other using inter-process communication (IPC).
There are three types of Kernals
Microkernel:A microkernel takes the approach of only managing what it has to: CPU, memory, and IPC. Pretty much everything else in a computer can be seen as an accessory and can be handled in user mode.
Monolithic Kernel:Monolithic kernels are the opposite of microkernels because they encompass not only the CPU, memory, and IPC, but they also include things like device drivers, file system management, and system server calls
Hybrid Kernel:Hybrid kernels have the ability to pick and choose what they want to run in user mode and what they want to run in supervisor mode. Because the Linux kernel is monolithic, it has the largest footprint and the most complexity over the other types of kernels. This was a design feature which was under quite a bit of debate in the early days of Linux and still carries some of the same design flaws that monolithic kernels are inherent to have.

#Question: What Is Linux Loader?
Linux Loader is a boot loader for Linux operating system. It loads Linux into into the main memory so that it can begin its operations.

#Question: What Is Swap Space?
Swap space is the amount of physical memory that is allocated for use by Linux to hold some concurrent running programs temporarily.
This condition usually occurs when Ram does not have enough memory to support all concurrent running programs.
This memory management involves the swapping of memory to and from physical storage.

#Question: What Are File Permissions In Linux?
There are 3 types of permissions in Linux 
Read: User can read the file and list the directory.
Write: User can write new files in the directory .
Execute: User can access and run the file in a directory.

#Question: Memory Management In Linux?
It is always required to keep a check on the memory usage in order to find out whether the user is able to access the server or the resources are adequate. There are roughly 5 methods that determine the total memory used by the Linux.
This is explained as below
Free command: This is the most simple and easy to use the command to check memory usage. For example: ‘$ free –m’, the option ‘m’ displays all the data in MBs.
/proc/meminfo: The next way to determine the memory usage is to read /proc/meminfo file. For example: ‘$ cat /proc/meminfo’
Vmstat: This command basically lays out the memory usage statistics. For example: ‘$ vmstat –s’
Top command: This command determines the total memory usage as well as also monitors the RAM usage.
Htop: This command also displays the memory usage along with other details. (I don't use it)

#Question:  Which Tools Are Used For Reporting Statistics In Linux?
Some of the popular and frequently used system resource generating tools available on the Linux platform are 
vmstat    -
netstat   -  netstat command in Linux shows the network status. This netstat command shows network ports in use and their incoming connections.
iostat    -
ifstat    -
mpstat.   - 
lsof      - lsof command lists the open files associated with your application.
These are used for reporting statistics from different system components such as virtual memory, network connections and interfaces, CPU, input/output devices and more.

#Question:  Types Of Processes In Linux?
There are fundamentally two types of processes in Linux:

Foreground processes (also referred to as interactive processes) – these are initialized and controlled through a terminal session. In other words, there has to be a user connected to the system to start such processes; they haven’t started automatically as part of the system functions/services.
Background processes (also referred to as non-interactive/automatic processes) – are processes not connected to a terminal; they don’t expect any user input.

#Question:  Creatin Of Processes In Linux?
A new process is normally created when an existing process makes an exact copy of itself in memory.

The child process will have the same environment as its parent, but only the process ID number is different.

There are two conventional ways used for creating a new process in Linux:

Using The System() Function – this method is relatively simple, however, it’s inefficient and has significantly certain security risks.
Using fork() and exec() Function – this technique is a little advanced but offers greater flexibility, speed, together with security.

#Question:  What Is Init Process Linux?
lnit process is the mother (parent) of all processes on the system, it’s the first program that is executed when the Linux system boots up; it manages all other processes on the system. It is started by the kernel itself, so in principle it does not have a parent process.

The init process always has process ID of 1. It functions as an adoptive parent for all orphaned processes.

#Question:  What Are Different States Of A Processes In Linux?
During execution, a process changes from one state to another depending on its environment/circumstances. In Linux, a process has the following possible states:

Running – here it’s either running (it is the current process in the system) or it’s ready to run (it’s waiting to be assigned to one of the CPUs).
Waiting – in this state, a process is waiting for an event to occur or for a system resource. Additionally, the kernel also differentiates between two types of waiting processes; interruptible waiting processes – can be interrupted by signals and uninterruptible waiting processes – are waiting directly on hardware conditions and cannot be interrupted by any event/signal.
Stopped – in this state, a process has been stopped, usually by receiving a signal. For instance, a process that is being debugged.
Zombie – here, a process is dead, it has been halted but it’s still has an entry in the process table.


#Question:  Can We Send signals To Processes In Linux?
The fundamental way of controlling processes in Linux is by sending signals to them. There are multiple signals that you can send to a process, to view all the signals run:

$ kill -l
List All Linux Signals

To send a signal to a process, use the kill, pkill or pgrep commands we mentioned earlier on. But programs can only respond to signals if they are programmed to recognize those signals.

And most signals are for internal use by the system, or for programmers when they write code. The following are signals which are useful to a system user:

SIGHUP 1 – sent to a process when its controlling terminal is closed.
SIGINT 2 – sent to a process by its controlling terminal when a user interrupts the process by pressing [Ctrl+C].
SIGQUIT 3 – sent to a process if the user sends a quit signal [Ctrl+D].
*SIGKILL 9 – this signal immediately terminates (kills) a process and the process will not perform any clean-up operations.
SIGTERM 15 – this a program termination signal (kill will send this by default).
SIGTSTP 20 – sent to a process by its controlling terminal to request it to stop (terminal stop); initiated by the user pressing [Ctrl+Z].

From https://mindmajix.com/linux-interview-questions
#Q. What is iptables command in Linux?
A. iptables command blocks or allows traffic on a Linux host, similar to a network firewall. This iptables command may prevent certain applications from receiving or transmitting requests.

