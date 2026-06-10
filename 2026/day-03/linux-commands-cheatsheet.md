Process Management

ps aux – View all running processes on the system with user details.
top – Monitor real-time CPU, memory usage, and active system processes.
htop – View interactive, color-coded process management (requires installation).
kill <PID> – Terminate a specific process gracefully using its ID number.
killall <name> – Stop all running instances of a program by name.
pkill -f <string> – Find and kill processes matching a specific text string.
bg – Send a suspended foreground job to run in the background.
fg – Bring a background job back into the foreground.


File System

df -h – Display available and used disk space in human-readable format.
du -sh * – Show the total size of each folder in the current directory.
ls -la – List all files, including hidden ones, with detailed permissions.
chmod 755 <file> – Set file permissions so owner can write, others can read/execute.
chown user:group <file> – Change the owner and group ownership of a file.
find / -name <filename> – Search for a file by name starting from the root directory.
grep -r "text" . – Search recursively for a specific string inside all files.
ncdu – Analyze disk usage with a text-based interface (requires installation).


Network Troubleshooting

ping -c 4 <host> – Send four packets to a host to test network connectivity.
ip addr – Show active network interfaces and assigned local IP addresses.
dig <domain> – Query DNS name servers to look up domain records.
curl -I <URL> – Fetch only the HTTP response headers from a specific URL.
ss -tuln – List all active network ports currently listening for connections.
traceroute <host> – Trace the path packets take to reach a network host.
