# Answer Key

## Multiple Choice Answers

1. **Q1:** 
   - b) bash

2. **Q2:** 
   - c) PowerShell

3. **Q3:** 
   - b) Lists files two directories up from current location

4. **Q4:** 
   - a) ls

5. **Q5:** 
   - a) mkdir

6. **Q6:** 
   - c) rmdir

7. **Q7:** 
   - a) rm

8. **Q8:** 
   - b) cp

9. **Q9:** 
   - b) Displays the content of a file

10. **Q10:** 
    - b) To establish a secure, encrypted connection to remote systems

11. **Q11:** 
    - b) ssh ubuntu@192.168.0.0

12. **Q12:** 
    - b) Public and private key pairs

13. **Q13:** 
    - b) `ssh -i ~/.ssh/server_key admin@192.168.1.100`

14. **Q14:** 
    - b) admin

15. **Q15:** 
    - a) Prints a message to the console

16. **Q16:** 
    - a) test -e file

17. **Q17:** 
    - a) read

18. **Q18:** 
    - c) until loop

19. **Q19:** 
    - b) .sh

20. **Q20:** 
    - a) chmod +x script.sh

21. **Q21:** 
    - d) Both a and c are correct

22. **Q22:** 
    - `./script.sh -f data.txt -n 42`

23. **Q23:** 
    - b) Changes the permissions of a file

24. **Q24:** 
    - a) user: rwx, group: r-x, other: r-x

25. **Q25:** 
    - b) No (group only has read permission, not write)

26. **Q26:** 
    - b) No (no execute permission)

27. **Q27:** 
    - a) `usermod -a -G developers alice`

28. **Q28:** 
    - b) `sed 's/oldserver/newserver/g' hosts.txt`

29. **Q29:** 
    - a) `awk '$1 ~ /o/ {print $4}' data`

30. **Q30:** 
    - b) `grep -E "(cat|dog)" file.txt`

31. **Q31:** 
    - a) `Test $25`

32. **Q32:** 
    - c) `\.txt$`

33. **Q33:** 
    - b) Commits staged changes with a descriptive message

34. **Q34:** 
    - a) git status

35. **Q35:** 
    - a) Downloads and merges changes from a remote repository

36. **Q36:** 
    - c) git add

37. **Q37:** 
    - b) Downloads a remote repository

38. **Q38:** 
    - b) `git pull`

39. **Q39:** 
    - a) `git add main.java; git commit -m "update"; git push`

## Practical Exercise Answers (for employees.csv)

### `grep` Answers:
40. **Q40:** 
    - `grep "Engineering" employees.csv`

41. **Q41:** 
    - `grep "HR" employees.csv`

42. **Q42:** 
    - `grep "John" employees.csv`

43. **Q43:** 
    - `grep -E "[0-9]{6,}" employees.csv` (then pipe to awk for exact filtering)

44. **Q44:** 
    - `grep "2019" employees.csv`

### `sed` Answers:
45. **Q45:** 
    - `sed 's/HR/Human Resources/g' employees.csv`

46. **Q46:** 
    - `sed '/Marketing/d' employees.csv`

47. **Q47:** 
    - `sed 's/\([0-9]\+\)$/\1 USD/g' employees.csv`

48. **Q48:** 
    - `sed -r 's/^([^,]+),([^,]+),/\2,\1,/' employees.csv`

49. **Q49:** 
    - `sed '1d' employees.csv`

### `awk` Answers:
50. **Q50:** 
    - `awk -F',' '{print $1}' employees.csv`

51. **Q51:** 
    - `awk -F',' '$2=="Engineering" {print $1, $3}' employees.csv`

52. **Q52:** 
    - `awk -F',' 'NR>1 {sum+=$3; count++} END {print sum/count}' employees.csv`

53. **Q53:** 
    - `awk -F',' 'NR>1 {if($3>max) max=$3} END {print max}' employees.csv`

54. **Q54:** 
    - `awk -F',' '$4 > 2020 {print $1}' employees.csv`
