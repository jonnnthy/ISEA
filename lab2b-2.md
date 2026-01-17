# Introduction to Bash Scripting & System Automation

## Bash Script Basics
- Add `#!/bin/bash`
- Use `echo` to display messages
- Use `chmod 777` to make the script executable
- Execute with `./hello_world.sh`
<img width="244" height="72" alt="nano hello world" src="https://github.com/user-attachments/assets/70498955-fe6d-4a8b-a3a7-573c206373a2" />
<img width="658" height="270" alt="executing sh " src="https://github.com/user-attachments/assets/6c2c30cb-b047-4280-a2d1-d63c1ad5665f" />


## Control Flow & User Input
- Use `for` loop for countdowns or iteration
<img width="262" height="236" alt="for loop" src="https://github.com/user-attachments/assets/cbf6b417-8c32-449c-8176-cfa7b13c8be0" />
<img width="524" height="228" alt="for loop result" src="https://github.com/user-attachments/assets/2df94a04-2f4b-4614-93d9-1b54d8561791" />

- Use `if`, `elif`, `else` to evaluate user input
<img width="394" height="330" alt="if elif else code" src="https://github.com/user-attachments/assets/4f287105-5614-48f4-a39b-33ddf6957796" />
<img width="454" height="268" alt="if elif else result" src="https://github.com/user-attachments/assets/e4126145-210f-4edd-9088-53a909ae1fa0" />

- Use `read` for interactive input
<img width="296" height="134" alt="read" src="https://github.com/user-attachments/assets/fc4d76d6-af5a-47c6-8b0e-e4686d2c6960" />


## System Monitoring Commands
- Use `top`, `free -h`, `df -h` to monitor system resources
<img width="1166" height="1018" alt="top" src="https://github.com/user-attachments/assets/4f1a8f2c-3a21-43d0-a815-4e9c22ffea8a" />


## Reflection Questions
- What command did you use to create a new directory?

mkdir
  
- How can you view the contents of a file without opening it in a GUI?

I used commands like cat and less to view file contents directly in the terminal.
  
- What is the purpose of `chmod 777`?

chmod 777 gives the owner, group, and others full read/write/execute permissions so the script can be executed.
  
- What does `#!/bin/bash` do at the start of a script?

It tells the system to run the script using the Bash interpreter.
 
- What happens when invalid input is entered into a script?

The script may produce an error or unexpected output unless input validation is added using conditions like if statements.
  
- What output does `free -h` show?

It shows memory usage (RAM and swap) in a human-readable format like MB or GB.
  
- How would you monitor network bandwidth in a Bash script?
I would use tools like iftop, nload, or vnstat and run them in a loop with sleep for continuous monitoring.
