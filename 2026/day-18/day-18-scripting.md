### Task 1: Basic Functions
1. Create `functions.sh` with:
   - A function `greet` that takes a name as argument and prints `Hello, <name>!`
   - A function `add` that takes two numbers and prints their sum
   - Call both functions from the script


   screenshot :
   ![1](images/1.jpg)
   
   screenshot :
   ![1a](images/1a.jpg)

### Task 2: Functions with Return Values
1. Create `disk_check.sh` with:
   - A function `check_disk` that checks disk usage of `/` using `df -h`
   - A function `check_memory` that checks free memory using `free -h`
   - A main section that calls both and prints the results


   screenshot :
   ![2](images/2.jpg)

     screenshot :
   ![2a](images/2a.jpg)


### Task 3: Strict Mode — `set -euo pipefail`
1. Create `strict_demo.sh` with `set -euo pipefail` at the top
2. Try using an **undefined variable** — what happens with `set -u`?
3. Try a command that **fails** — what happens with `set -e`?
4. Try a **piped command** where one part fails — what happens with `set -o pipefail`?

**Document:** What does each flag do?
- `set -e` → Exit the script immediately if a command fails.
- `set -u` → Exit if an undefined variable is used.
- `set -o pipefail` →  If any command in a pipeline fails, the entire pipeline fails.

 screenshot :
   ![3](images/3.jpg)

 screenshot :
   ![3a](images/3a.jpg)


### Task 4: Local Variables
1. Create `local_demo.sh` with:
   - A function that uses `local` keyword for variables
   - Show that `local` variables don't leak outside the function
   - Compare with a function that uses regular variables

Notes:
What are variables in functions
Regular variables in Bash are global by default ,If you create a variable inside a function, it can still be used outside the function
Local variables are limited to the function ,If you create a variable with the keyword local, it does not exist outside the function

screenshot :
   ![4](images/4.jpg)

   screenshot :
   ![4a](images/4a.jpg)


### Task 5: Build a Script — System Info Reporter
Create `system_info.sh` that uses functions for everything:
1. A function to print **hostname and OS info**
2. A function to print **uptime**
3. A function to print **disk usage** (top 5 by size)
4. A function to print **memory usage**
5. A function to print **top 5 CPU-consuming processes**
6. A `main` function that calls all of the above with section headers
7. Use `set -euo pipefail` at the top


screenshot :
   ![5](images/5.jpg)


   screenshot :
   ![5a](images/5a.jpg)





