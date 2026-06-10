**Core components of linux**
1. The Linux Kernel (The Core) runs in the most privileged CPU mode (Ring 0) and has complete, unrestricted access
   to the underlying hardware. It acts as a broker between software requests and physical hardware components.
2. User Space (The Environment) refers to the unprivileged memory region (Ring 3) where user applications
   and non-kernel services run. If a process crashes here, it will not bring down the entire system.
3. Init and systemd (The Manager) When a computer boots up, the kernel initializes hardware and mounts the root filesystem.
   It then spawns exactly one initial process in user space: init. This process always receives Process ID 1 (PID 1).

Process states define the current lifecycle stage of a program executing in an operating system. The OS kernel assigns these states
(e.g., Running, Sleeping, Zombie) to manage CPU allocation, handle I/O requests, and track terminated tasks.
1. Running / Runnable What it means: The process is either actively executing on a CPU core or is in the ready queue waiting for its
   turn to run.
2. Sleeping (Waiting) What it means: The process is inactive because it is waiting for an event to occur, such as user input, a network
   response, or an I/O disk operation.
3. Zombie What it means: A child process that has completed its execution, but still has an entry in the process table because its parent
   process hasn't read (or "reaped") its exit status yet.

**List 5 commands you would use daily**


ls: Lists the contents (files and directories) of your current working directory. Adding flags like ls -l provides a detailed list
(permissions, owner, size), and ls -a reveals hidden configuration files.


cd: Navigates through the file system. You type cd folder_name to enter a directory, cd .. to go back one level, and cd by itself to return straight to your home directory.


pwd: Displays the exact, absolute path of your current working location. It helps you stay oriented so you don't accidentally modify files in the wrong place.


mkdir: Creates a brand new directory or folder. For example, typing mkdir projects will create a directory named "projects" inside your current location.


sudo: Grants you superuser or administrator privileges. You use this before running commands that require root access—such as installing software updates or modifying system-critical configuration files.
