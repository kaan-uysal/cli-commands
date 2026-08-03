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
