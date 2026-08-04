# terminal-commands
Collection of linux terminal codes, operators and CLI notes.

| Command | Description | Example / Syntax |
| :--- | :--- | :--- |
| `pwd` | Print working directory (shows current path) | `pwd` |
| `ls` | List directory contents | `ls -la` *(shows hidden files & details)* |
| `cd` | Change directory | `cd /var/log` or `cd ..` |
| `cat` | Concatenate and display file content | `cat flag.txt` |
| `find` | Find the specific file | `find -name specific.txt` or `find -name *.txt`
| `wc` | Give details about file (bytes,logs,ch etc.) | `wc file.txt`
| `grep` | Search entire file *(just one)*, find the specific one and display it | `grep "specific" file.txt or data.log`
| `grep -R` | Search recursively with grep *(in a whole directory)* | `grep -R "i_love_you" /home/lovers`
| `cut` | Extract specific columns from file | `cut -d ':' -f 1 /etc/passwd` |
| `sort` & `uniq` | Sort lines and count unique occurrences | `cat log.txt \| sort \| uniq -c` |
| `tail -f` | Monitor log files in real-time | `tail -f /var/log/auth.log` |
| `awk` | Pattern scanning and processing language | `ls -l \| awk '{print $1, $9}'` |

---

| Operator or symbol | Description | Example / Syntax |
| :--- | :--- | :--- |
| `&` | Allows to execute commands in the background. | `sleep 30 &`
| `&&` | Make a list of commands to run *(in order)* | `command1 && command2`
| `>` | Take the output from a command, run, send this output to somewhere else and create a new file | `echo welcome > kaan`
| `>>` | Take the output from a command, add this to end of the file that selected | `echo hello >> kaan`
| `\|` | Pipes stdout of one command to stdin of another | `cat log.txt \| grep "ERROR"` |
| `2>` | Redirects error messages (stderr) | `find / -name "flag" 2> /dev/null` |
| `\|\|` | Runs second command ONLY if first fails | `cd /root \|\| echo "Access Denied"` |
| `$(...)` | Command substitution (executes command inline) | `echo "Today is $(date)"` |
| `*` | Wildcard matching zero or more characters | `rm *.tmp` |
| `{1..N}` | Brace expansion for sequence generation | `mkdir dir_{1..5}` |
| `-` | Switch back to the previous working directory | `cd -` |

---

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
