
## 1. Shells:

**Q1: Which of the following is a shell used on your Ubuntu machine?**  
a) PowerShell  
b) bash  
c) cmd  
d) Z shell  

**Q2: Which shell is commonly used in Windows for command-line operations?**  
a) zsh  
b) bash  
c) PowerShell  
d) sh  

---

## 2. SSH (Secure Shell):

**Q6: What is the primary use of SSH?**  
a) To browse the internet securely  
b) To establish a secure, encrypted connection to remote systems  
c) To copy files between systems  
d) To back up system files  

**Q7: What is the command to establish an SSH connection to a server?**  
a) ssh 192.168.0.0@ubuntu 
b) ssh ubuntu@192.168.0.0
c) ssh-server  
d) connect ssh ubuntu@192.168.0.0

**Q8: Which of the following is a requirement for SSH authentication?**  
a) Password encryption  
b) Public and private key pairs  
c) Username and domain name 
d) Static IP address


---

## 3. Files, Directories, and OS Structure:

**Question 3:** What does the command `ls ../..` do?

- a) Lists files in the current directory
- b) Lists files two directories up from current location
- c) Lists hidden files in parent directory
- d) Creates a new directory

**Q10: What command is used to list files and directories in Linux?**  
a) ls  
b) dir  
c) list  
d) show  

**Q11: What command creates a new directory in Linux?**  
a) mkdir  
b) mkdir -new  
c) touch  
d) newdir  

**Q12: What command is used to remove a directory in Linux?**  
a) rm  
b) del  
c) rmdir  
d) delete  

**Q13: What command is used to remove a file in Linux?**  
a) rm  
b) erase  
c) del  
d) remove  

**Q14: Which command in Linux is used to copy files?**  
a) mv  
b) cp  
c) cat  
d) ln  

---

## 4. Scripting:

**Q17: What does the `echo` command do in bash scripting?**  
a) Prints a message to the console  
b) Executes a command  
c) Reads a file  
d) Creates a new file  

**Q18: What bash command is used to check if a file exists?**  
a) test -e file  
b) check file  
c) file exists  
d) if file -exists  

**Q19: Which of the following is used to read user input in a bash script?**  
a) read  
b) get  
c) input  
d) prompt  

**Q21: Which loop in bash will execute a block of code until a condition is met?**  
a) for loop  
b) while loop  
c) until loop  
d) repeat loop  

---

## 5. Git (Version Control):

**Q23: What does the `git commit -m "message"` command do?**  
a) Stages changes for commit  
b) Commits staged changes with a descriptive message  
c) Pushes committed changes to a remote repository  
d) Creates a new branch 

**Q24: What command is used to check the status of a Git repository?**  
a) git status  
b) git check  
c) git info  
d) git logs  

**Q25: What does the `git pull` command do?**  
a) Downloads and merges changes from a remote repository  
b) Creates a new commit  
c) Uploads local changes to the remote repository  
d) Clones a remote repository  

**Q26: Which command would you use to stage files for commit in Git?**  
a) git push  
b) git stage  
c) git add  
d) git merge  

**Q27: What does the `git clone` command do?**  
a) Creates a new branch  
b) Downloads a remote repository
c) Commits changes to the repository  
d) Adds files to the repository  

**Question 2: You're trying to push changes to GitHub but get an error saying "Updates were rejected because the remote contains work that you do not have locally." What should you do first?**

- a) `git push --force`
- b) `git pull`
- c) `git reset --hard`
- d) `git commit -m "fix"`
---

## 6. Additional Questions:

**Q28: What is the default file extension for bash scripts?**  
a) .txt  
b) .sh  
c) .bash  
d) .bashscript  

**Q29: What does the `chmod` command do in Linux?**  
a) Changes the ownership of a file  
b) Changes the permissions of a file  
c) Moves a file to a new directory  
d) Renames a file  

**Q30: How can you make a bash script executable?**  
a) chmod +x script.sh  
b) bash script.sh  
c) make script.sh executable  
d) execute script.sh  

**Q31: What does the `cat` command do in Linux?**  
a) Creates a new file  
b) Displays the content of a file  
c) Copies a file  
d) Deletes a file  


Question 7: Given this SSH config entry:
```
Host server1
    HostName 192.168.1.100
    User admin
    IdentityFile ~/.ssh/server_key
```

What SSH command would use this config file break down to?

- a) `ssh admin@192.168.1.100`
- b) `ssh -i ~/.ssh/server_key admin@192.168.1.100`
- c) `ssh ~/.ssh/server_key 192.168.1.100@admin `
- d) `ssh 192.168.1.100`

**Question 8:** In the above SSH config, what is the username on the remote system?

- a) server1 
- b) admin
- c) 192.168.1.100
- d) server_key
---

## Text Processing

**Question 9:** You need to replace all occurrences of "oldserver" with "newserver" in a file called hosts.txt. Which sed command is correct?

- a) `sed 's/oldserver/newserver/' hosts.txt`
- b) `sed 's/oldserver/newserver/g' hosts.txt`
- c) `sed 'g/oldserver/newserver/' hosts.txt`
- d) `sed 'oldserver/newserver/g' hosts.txt`

**Question 10:** Given this data:

```
Alice Johnson red pizza
Bob Wilson blue burger
Carol Davis green salad
```

Which awk command prints the favorite food of people whose first name contains 'o'?

- a) `awk '$1 ~ /o/ {print $4}' data`
- b) `awk '$1 = /o/ {print $4}' data`
- c) `awk '/o/ {print $4}' data`
- d) `awk '$0 ~ /o/ {print $1}' data`

## Regular Expressions

**Question 11:** Which grep command will match lines containing either "cat" or "dog" (exact words)?

- a) `grep "cat|dog" file.txt`
- b) `grep -E "(cat|dog)" file.txt`
- c) `grep -v "(cat|dog)" file.txt`
- d) `grep "(cat|dog)" > file.txt`

**Question 12:** Given the regex pattern: `^[Tt]est\s\$[0-9]{2,3}$`

Which string will match this pattern?

- a) `Test $25`
- b) `test $5`
- c) `Testing $100`
- d) `test$25`

**Question 13:** Which regex matches files ending in .txt only?

- a) `.txt`
- b) `\.txt`
- c) `\.txt$`
- d) `txt$`

## File Permissions

**Question 14:** What permissions does `chmod 755 script.sh` set?

- a) user: rwx, group: r-x, other: r-x
- b) user: rw-, group: r--, other: r--
- c) user: r-x, group: rwx, other: r-x
- d) user: rwx, group: rwx, other: rwx

**Question 15:** A file has permissions `-rw-r--r--` and is owned by user "john" in group "staff". Can user "mary" (who is in group "staff") edit this file?

- a) Yes
- b) No

## User Management

**Question 16:** Which command adds user "alice" to the group "developers"?

- a) `usermod -a -G developers alice`
- b) `usermod -a -G alice developers`
- c) `adduser alice developers`
- d) `chgrp developers alice`

**Question 17:** A script has permissions `-rw-r--r--`. Can you execute it with `./script.sh`?

- a) Yes
- b) No

## Shell Scripting

**Question 18:** Which script correctly checks if a file exists before reading it?

- a) 
```bash
if [[ -f $filename ]]; then
    cat $filename
fi
```

- b)
```bash
if [[ -d $filename ]]; then
    cat $filename
fi
```

- c)
```bash
if [[ -e $filename ]]; then
    cat $filename
fi
```

- d) Both a and c are correct

**Question 19:** You have a script that uses getopts with options "-h" for help, "-f" for filename, and "-n" for number. Write a command that would call this script to set filename to "data.txt" and number to "42":

**Answer:** ________________________________

## Git Operations

**Question 20:** You have modified a file called "main.java" in your git repository. The output of `git status` shows:

```
Changes not staged for commit:
  modified: main.java
```

What commands do you need to commit and push this change?

- a) `git add main.java; git commit -m "update"; git push`
- b) `git commit main.java; git push`
- c) `git add .; git push`
- d) `git commit -a; git push`

---

## Questions on `grep`, `sed` and `awk` are here to get you comfortable before the exam.
**Feel free to use past notes or `man` pages on your terminal!!**

**Use the `employees.csv` file located in this repo for the next questions.**


### `grep` Questions:
1. Find all employees in the "Engineering" department.
2. Display lines containing "HR" employees.
3. Find employees whose name contains "John".
4. Show lines with a salary greater than 70000 (you may need to refine this after `grep` using `awk`).
5. Search for employees who joined in the year 2019.

### `sed` Questions:
6. Replace "HR" with "Human Resources" in the dataset.
7. Remove the "Marketing" department from the dataset.
8. Add a "USD" suffix to all salary values.
9. Swap the "Name" and "Department" columns (assume a simple text transformation).
10. Remove the header row from the file.

### `awk` Questions:
11. Print only the names of the employees.
12. Show the name and salary of employees from the "Engineering" department.
13. Calculate and print the average salary of all employees.
14. Find the highest salary in the dataset.
15. Print the names of employees who joined after 2020.

---
