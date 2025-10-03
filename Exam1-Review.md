# CEG 2350 Midterm 1 Review 

## Instructions

**Resources Available:**
- Your terminal and AWS instance
- Notes you've taken so far
- Regex links that are provided
- [Data Camp Cheat Sheet](https://www.datacamp.com/cheat-sheet/regular-expresso)
and [Regex 101](https://regex101.com)
- Lab work in your course repository

**Important Note:**
These questions are designed to check your understanding and test your ability to use available resources to find correct answers. They are not meant to be an exact replica of the exam you will take, but rather practice questions to reinforce your learning.

Good luck, and may the curve ever be in your favor. 

(There isn't a curve, so just good luck 😉)

## 1. Shells

**Q1: Which of the following is a shell used on your Ubuntu machine?**
- a) PowerShell  
- b) bash <- 
- c) cmd  
- d) Z shell  

**Q2: Which shell is commonly used in Windows for command-line operations?**
- a) zsh  
- b) bash  
- c) PowerShell <- 
- d) sh  

---

## 2. Files, Directories, and OS Structure

**Q3: What does the command `ls ../..` do?**
- a) Lists files in the current directory
- b) Lists files two directories up from current location<-
- c) Lists hidden files in parent directory
- d) Creates a new directory

**Q4: What command is used to list files and directories in Linux?**
- a) ls  <-
- b) dir  
- c) list  
- d) show  

**Q5: What command creates a new directory in Linux?**
- a) mkdir  <-
- b) mkdir -new  
- c) touch  
- d) newdir  

**Q6: What command is used to remove a directory in Linux?**
- a) rm  
- b) del  
- c) rmdir <- 
- d) delete  

**Q7: What command is used to remove a file in Linux?**
- a) rm<- 
- b) erase  
- c) del  
- d) remove  

**Q8: Which command in Linux is used to copy files?**
- a) mv  
- b) cp<-  
- c) cat  
- d) ln  

**Q9: What does the `cat` command do in Linux?**
- a) Creates a new file  
- b) Displays the content of a file  
- c) Copies a file  
- d) Deletes a file  

---

## 3. SSH (Secure Shell)

**Q10: What is the primary use of SSH?**
- a) To browse the internet securely  
- b) To establish a secure, encrypted connection to remote systems  
- c) To copy files between systems  
- d) To back up system files  

**Q12: Which of the following is a requirement for SSH authentication?**
- a) Password encryption  
- b) Public and private key pairs  
- c) Username and domain name 
- d) Static IP address

**Q13: Given this SSH config entry:**
```
Host server1
    HostName 192.168.1.100
    User admin
    IdentityFile ~/.ssh/server_key
```
**What SSH command would use this config file break down to?**
- a) `ssh admin@192.168.1.100`
- b) `ssh -i ~/.ssh/server_key admin@192.168.1.100`
- c) `ssh ~/.ssh/server_key 192.168.1.100@admin`
- d) `ssh 192.168.1.100`

**Q14: In the above SSH config, what is the username on the remote system?**
- a) server1 
- b) admin
- c) 192.168.1.100
- d) server_key

---

## 4. Scripting

**Q15: What does the `echo` command do in bash scripting?**
- a) Prints a message to the console  
- b) Executes a command  
- c) Reads a file  
- d) Creates a new file  

**Q16: What bash command is used to check if a file exists?**
- a) test -e file  
- b) check file  
- c) file exists  
- d) if file -exists  

**Q17: Which of the following is used to read user input in a bash script?**
- a) read  
- b) get  
- c) input  
- d) prompt  

**Q19: What is the default file extension for bash scripts?**
- a) .txt  
- b) .sh  
- c) .bash  
- d) .bashscript  

**Q20: How can you make a bash script executable?**
- a) chmod +x script.sh  
- b) bash script.sh  
- c) make script.sh executable  
- d) execute script.sh  

**Q21: Which script correctly checks if a file exists before reading it?**
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

**Q22: You have a script that uses getopts with options "-h" for help, "-f" for filename, and "-n" for number. Write a command that would call this script to set filename to "data.txt" and number to "42":**

**Answer:** ________________________________

---

## 5. File Permissions

**Q23: What does the `chmod` command do in Linux?**
- a) Changes the ownership of a file  
- b) Changes the permissions of a file  
- c) Moves a file to a new directory  
- d) Renames a file  

**Q24: What permissions does `chmod 755 script.sh` set?**
- a) user: rwx, group: r-x, other: r-x
- b) user: rw-, group: r--, other: r--
- c) user: r-x, group: rwx, other: r-x
- d) user: rwx, group: rwx, other: rwx

**Q25: A file has permissions `-rw-r--r--` and is owned by user "john" in group "staff". Can user "mary" (who is in group "staff") edit this file?**
- a) Yes
- b) No

**Q26: A script has permissions `-rw-r--r--`. Can you execute it with `./script.sh`?**
- a) Yes
- b) No

---

## 6. User Management

**Q27: Which command adds user "alice" to the group "developers"?**
- a) `usermod -a -G developers alice`
- b) `usermod -a -G alice developers`
- c) `adduser alice developers`
- d) `chgrp developers alice`

---

## 7. Text Processing

**Q28: You need to replace all occurrences of "oldserver" with "newserver" in a file called hosts.txt. Which sed command is correct?**
- a) `sed 's/oldserver/newserver/' hosts.txt`
- b) `sed 's/oldserver/newserver/g' hosts.txt`
- c) `sed 'g/oldserver/newserver/' hosts.txt`
- d) `sed 'oldserver/newserver/g' hosts.txt`

**Q29: Given this data:**
```
Alice Johnson red pizza
Bob Wilson blue burger
Carol Davis green salad
```
**Which awk command prints the favorite food of people whose first name contains 'o'?**
- a) `awk '$1 ~ /o/ {print $4}' data`
- b) `awk '$1 = /o/ {print $4}' data`
- c) `awk '/o/ {print $4}' data`
- d) `awk '$0 ~ /o/ {print $1}' data`

---

## 8. Regular Expressions

**Q30: Which grep command will match lines containing either "cat" or "dog" (exact words)?**
- a) `grep "cat|dog" file.txt`
- b) `grep -E "(cat|dog)" file.txt`
- c) `grep -v "(cat|dog)" file.txt`
- d) `grep "(cat|dog)" > file.txt`

**Q31: Given the regex pattern: `^[Tt]est\s\$[0-9]{2,3}$`**
**Which string will match this pattern?**
- a) `Test $25`
- b) `test $5`
- c) `Testing $100`
- d) `test$25`

**Q32: Which regex matches files ending in .txt only?**
- a) `.txt`
- b) `\.txt`
- c) `\.txt$`
- d) `txt$`

---

## 9. Git (Version Control)

**Q33: What does the `git commit -m "message"` command do?**
- a) Stages changes for commit  
- b) Commits staged changes with a descriptive message  
- c) Pushes committed changes to a remote repository  
- d) Creates a new branch 

**Q34: What command is used to check the status of a Git repository?**
- a) git status  
- b) git check  
- c) git info  
- d) git logs  

**Q35: What does the `git pull` command do?**
- a) Downloads and merges changes from a remote repository  
- b) Creates a new commit  
- c) Uploads local changes to the remote repository  
- d) Clones a remote repository  

**Q36: Which command would you use to stage files for commit in Git?**
- a) git push  
- b) git stage  
- c) git add  
- d) git merge  

**Q37: What does the `git clone` command do?**
- a) Creates a new branch  
- b) Downloads a remote repository
- c) Commits changes to the repository  
- d) Adds files to the repository  

**Q38: You're trying to push changes to GitHub but get an error saying "Updates were rejected because the remote contains work that you do not have locally." What should you do first?**
- a) `git push --force`
- b) `git pull`
- c) `git reset --hard`
- d) `git commit -m "fix"`

**Q39: You have modified a file called "main.java" in your git repository. The output of `git status` shows:**
```
Changes not staged for commit:
  modified: main.java
```
**What commands do you need to commit and push this change?**
- a) `git add main.java; git commit -m "update"; git push`
- b) `git commit main.java; git push`
- c) `git add .; git push`
- d) `git commit -a; git push`

---

## 10. Practical Exercises with employees.csv

**Use the `employees.csv` file located in this repo for the following questions.**

### `grep` Questions:
**Q40:** Find all employees in the "Engineering" department.

**Q41:** Display lines containing "HR" employees.

**Q42:** Find employees whose name contains "John".

**Q43:** Show lines with a salary greater than 70000 (you may need to refine this after `grep` using `awk`).

**Q44:** Search for employees who joined in the year 2019.

### `sed` Questions:
**Q45:** Replace "HR" with "Human Resources" in the dataset.

**Q46:** Remove the "Marketing" department from the dataset.

**Q47:** Add a "USD" suffix to all salary values.

**Q48:** Swap the "Name" and "Department" columns (assume a simple text transformation).

**Q49:** Remove the header row from the file.

### `awk` Questions:
**Q50:** Print only the names of the employees.

**Q51:** Show the name and salary of employees from the "Engineering" department.

**Q52:** Calculate and print the average salary of all employees.

**Q53:** Find the highest salary in the dataset.

**Q54:** Print the names of employees who joined after 2020.

---

