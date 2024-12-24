### **Linux Commands Quick Reference**

---

**1\. What is the `echo` command in Linux?**  
The `echo` command prints a string or message to the terminal.

`$ echo "Hey Deepak"`    
`Hey Deepak`

---

**2\. How to check the hostname in Linux?**

`$ hostname`    
`Deepak`

---

**3\. How to check the current user in Linux?**

`$ whoami`    
`Deepak`

---

**4\. How to check the current directory path?**

`$ pwd`    
`/c/Users/Deepak/Linux_practice`

---

**5\. What is the absolute and relative path in Linux?**

**Relative Path**: Path relative to the current directory.

`$ cd Linux_practice/`

* 

**Absolute Path**: Full path starting from the root directory.

`$ cd /Deepak/Linux_practice`

* 

---

**6\. Commands to create files in Linux:**

* `touch`, `vi`, `vim`, `nano`, etc.

---

**7\. How to edit an existing file on the server?**  
Use editors like `vi`, `vim`, or `nano`.

---

**8\. How to rename a file in Linux?**  
Use the `mv` command:

`$ mv file1 file2`

---

**9\. How to search for a string in a file?**  
Use the `grep` command:

`$ grep "you" file2`    
`Hey Deepak, How are you?`

---

**10\. Difference between `grep` and `egrep`:**

* **`grep`**: Searches a single pattern.

**`egrep`**: Searches multiple patterns.

`$ egrep "Alice|Engineering" file2`

* 

---

**11\. How to read a file without `cat`?**  
Use `less`, `tail -f`, `nano`, or `vi`.

---

**12\. Advantage of `less`:**

* Easier navigation in large files (forward and backward).

---

**13\. How to check file permissions?**

`$ ls -l`    
`$ getfacl file_name`

---

**14\. How to check the IP of a Linux server?**

`$ ip addr`    
`$ ifconfig`

---

**15\. How to read the first or last lines of a file?**

Top 2 lines:

`$ head -2 file_name`

* 

Last 2 lines:

`$ tail -2 file_name`

* 

---

**16\. How to list hidden files?**

`$ ls -la`

---

**17\. How to see recent commands?**

`$ history`

---

**18\. What is `root`?**  
The superuser with complete access to the system.

---

**19\. What is an inode, and how to find it?**

Inodes provide a unique identifier for files.

`$ ls -li`

* 

---

**20\. Command to find a file in Linux:**

`$ find /path/to/search -name file_name`

---

**21\. Commands to count words or lines:**

`$ wc file_name`    
`$ wc -l file_name`

---

**22\. How to combine commands using a pipe (`|`)?**

Pipe connects the output of one command to another.

`$ cat file2 | grep HR`

* 

---

**23\. How to compare two files?**  
Use the `diff` command:

`$ diff file1 file2`

---

**24\. Use of the `shred` command:**  
Permanently deletes files.

---

**25\. How to check system architecture info?**

`$ lscpu`    
`$ dmidecode`

---

**26\. How to combine two files?**

`$ cat file1 file2 > file3`

---

**27\. How to determine the type of a file?**

`$ file file_name`

---

**28\. How to sort file contents?**

`$ sort file_name`

---

**29\. Ways to access a Linux server remotely:**  
Tools like PuTTY, MobaXterm, Git , etc.

---

**30\. File permissions in Linux:**

* **Read** (`r`), **Write** (`w`), and **Execute** (`x`).

---

**31\. How to redirect output or errors to a file?**

`$ command > output.txt       # Output only`    
`$ command 2> error.txt       # Error only`    
`$ command > output.txt 2>&1  # Both`

---

**32\. How to automate tasks in Linux?**  
Use **cron jobs**:

`$ crontab -e`

---

**33\. What is a daemon service?**  
A background service (e.g., `sshd`, `httpd`).

---

**34\. How to check if a service is running?**

`$ systemctl status service_name`

---

**35\. How to check disk space or directory size?**

`$ df -h       # Disk space`    
`$ du -h       # Directory size`

---

**36\. What is a process in Linux?**  
A program or command in execution with a unique PID.

---

**37\. How to check if a process is running?**

`$ ps -ef | grep process_name`

---

**38\. How to terminate a process?**

`$ kill -9 PID`

---

**39\. How to check network interfaces in Linux?**

`$ ifconfig`    
`$ ip addr`

---

**40\. Difference between Telnet and SSH:**

* **SSH**: Secure communication.  
* **Telnet**: Unsecure communication.

---

**41\. Default SSH port:**  
Port 22\.

---

**42\. How to connect to another Linux server?**

`$ ssh user@ip_address`

---

**43\. How to transfer large files remotely?**

Compress the file:

`$ tar -czf largefile.tar.gz largefile`

1. 

Transfer the file:

`$ scp largefile.tar.gz user@remote_host:/path/to/destination`

2. 

