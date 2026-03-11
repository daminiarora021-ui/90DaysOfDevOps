## Challenge Tasks

### Task 1: Your First Script
1. Create a file `hello.sh`
2. Add the shebang line `#!/bin/bash` at the top
3. Print `Hello, DevOps!` using `echo`
4. Make it executable and run it

screenshot :
![1](images/1.jpg)


screenshot :
![2](images/2.jpg)

**Document:** What happens if you remove the shebang line?

The shebang (#!) line specifies the interpreter used to execute a script. If the shebang line is removed, the operating system may not know which interpreter should run the script when executed directly. As a result, the script may fail or run with the default shell.




### Task 2: Variables
1. Create `variables.sh` with:
   - A variable for your `NAME`
   - A variable for your `ROLE` (e.g., "DevOps Engineer")
   - Print: `Hello, I am <NAME> and I am a <ROLE>`


screenshot :
![3](images/3.jpg)


screenshot :
![4](images/4.jpg)

2. Try using single quotes vs double quotes — what's the difference?
 single and double quote behave differently 
 single quote take literal value of all expression 
 double allows variable and command expression 
screenshot :
![5](images/5.jpg)


### Task 3: User Input with read
1. Create `greet.sh` that:
   - Asks the user for their name using `read`
   - Asks for their favourite tool
   - Prints: `Hello <name>, your favourite tool is <tool>`

screenshot :
![6](images/6.jpg)

screenshot :
![7](images/7.jpg)

### Task 4: If-Else Conditions
1. Create `check_number.sh` that:
   - Takes a number using `read`
   - Prints whether it is **positive**, **negative**, or **zero**

screenshot :
![8](images/8.jpg)

screenshot :
![9](images/9.jpg)


2. Create `file_check.sh` that:
   - Asks for a filename
   - Checks if the file **exists** using `-f`
   - Prints appropriate message


screenshot :
![10](images/10.jpg)
screenshot :
![11](images/11.jpg)


Create `server_check.sh` that:
1. Stores a service name in a variable (e.g., `nginx`, `sshd`)
2. Asks the user: "Do you want to check the status? (y/n)"
3. If `y` — runs `systemctl status <service>` and prints whether it's **active** or **not**
4. If `n` — prints "Skipped."



screenshot :
![12](images/12.jpg)
screenshot :
![13](images/13.jpg)
