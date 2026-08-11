## Windows CLI

Handy cheat sheet for essential Windows Command Prompt (CMD) commands used in system navigation, networking, file management, and process analysis.

| Command | Description | Example / Syntax |
| :--- | :--- | :--- |
| `set` | Environment | Displays, sets, or removes environment variables in the current session. |
| `ver` | System Info | Displays the exact Windows operating system version number. |
| `systeminfo` | System Info | Displays detailed system configuration, OS build, patches (hotfixes), and hardware specs. |
| `more` | File Utility | Displays output or text file content one screenful/page at a time. |
| `driverquery` | System Info | Lists all installed device drivers and their properties. |
| `ipconfig` | Networking | Displays basic IP address, subnet mask, and default gateway for all network adapters. |
| `ipconfig /all` | Networking | Displays detailed network configuration, including MAC addresses, DHCP, and DNS servers. |
| `ping example.com` | Networking | Sends ICMP Echo Requests to a target host to test network connectivity and latency. |
| `tracert target_name` | Networking | Traces the network route to a destination, showing each hop and latency along the path. |
| `nslookup example.com` | Networking | Queries DNS servers to resolve domain names to IP addresses (and vice versa). |
| `netstat` | Networking | Displays active TCP connections and network statistics. |
| `netstat -abon` | Networking | Lists all active connections with **A**ll ports, **B**inary/executable names, **O**WNER process IDs, and **N**umeric addresses (requires Admin). |
| `cd` | Navigation | Displays the current working directory path. |
| `dir` | Navigation | Lists files and subdirectories in the current directory. |
| `dir /a` | Navigation | Lists all files in the directory, including hidden and system files. |
| `dir /s` | Navigation | Recursively lists all files and directories in the current folder and its subfolders. |
| `tree` | Navigation | Graphically displays the folder structure of a path or drive. |
| `cd target_directory` | Navigation | Changes the current working directory to the specified target path. |
| `cd..` | Navigation | Moves up one directory level to the parent folder. |
| `mkdir directory_name` | File Management | Creates a new directory/folder with the specified name. |
| `rmdir directory_name` | File Management | Removes/deletes an empty directory. |
| `type filename` | File Management | Displays the raw content of a text file in the terminal (equivalent to Linux `cat`). |
| `copy source destination` | File Management | Copies one or more files from one location to another. |
| `move source destination` | File Management | Moves files or directories from one location to another, or renames a directory. |
| `del filename` | File Management | Deletes one or more specified files. |
| `tasklist` | Process Mgmt | Displays a list of all currently running processes with their Process IDs (PIDs) and memory usage. |
| `tasklist /FI "imagename eq example.exe"` | Process Mgmt | Filters running processes to display only those matching a specific executable name. |
| `taskkill /PID target_PID` | Process Mgmt | Terminates a running process using its specific Process ID (PID). Add `/F` to force termination. |
