"# System-Programming-Process-Management" 
Part 1. Shell Experiences and Programming

You are asked to try Unix/Linux shell in this part of project.
Requirements:

1. Run the displayinfo.sh and greeting.sh scripts provided and report the result (i.e. using
shell redirection to produce output files and then submit output files).
2. Made two modifications to the greeting.sh script provided: 1) the script only shows a
greeting message when it’s morning, afternoon, or evening; please make a code
modification to show a greeting message “Hello [your login name]!” when it’s other than
morning, afternoon, or evening; 2) please output the greeting message to a file called
“greetingmsg”, and if this file already exists, then deletes the file first, then output the
message to this file.
3. Run the modified greeting.sh script on the HPCC server and report the result.

Part 2. System Programming and Process Management (in C programming language)

You are asked to develop basic system programming including process creation and termination
on a Linux platform in this part of programming project. You are asked to create multiple
children processes to work under one parent process. In theory, children processes can do their
own work separately or cooperatively to accomplish a task. In this assignment, these children
processes simply print out a “hello” message together with their PIDs (process IDs) and exit.
You should use fork() and wait() system calls to implement this program.

Requirements:
1. Take the number of children processes as an argument when the parent process creates
children processes. This argument should be passed through a command line argument.
2. The parent process creates children processes and should print out an error message if
creation fails. The parent process should also wait for all children processes to finish and
then exit.
3. Each child process should print out a hello message together its PID and then exit.
