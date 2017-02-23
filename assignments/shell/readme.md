
>Group Members
>
| Name    | Email   | Github Username |
|----------|---------|-----------------|
| Kattreddy, Madhuchirra Reddy  | madhureddykp477@gmail.com | madhureddykp477  |
|  Valliyil, Saikiran  | valliyilmenon@gmail.com| Valliyilmenon  |
| Tinubu, Oluwaseyi | tinubuseyi@gmail.com | Decastrino|


Date Completed: 02/20/2017
===============================================================================================



================================================================================================
The program is executed by calling the python command followed by the  file name.
The executedfile contains a main fucntion that calls the main thread, this main thread function creates a thread that starts the whole input processing.
When a user enters a command, it is checked



This program is a makeshift shell written in python, that accepts commands from users, 
kicks off a main thread when the input is entered, the input is checked and split, 
based on the split, functions are called that carry out appropriate commands entered by the user.
The shell is implemented as a class. It has methods that allows it get user inputs, compare inputs with predefined lists of valid commands and, exit.


It reads user input as a strings.

Using the commandSplitter Class, the sring of command is splitted into words using blank
spaces as the delimiter and each words are put in a pythin list structure.

The commandChecker then accepts the splitted command as an argument. It basically inherits from the commandSpliter class.

The commandChecker class has 3 functions that:

	1. acceptCommand: accept the user command(i.e commands gotten from the commandSpltter
	   class.
	   
	2. processCommand: process the user command(i.e it checks for the length of the command
	   entered, and takes all first element in the splitted list of words as the main shell command.
	   
	3. passCommand: this function checks if the command is to be run as an underground process(a daemon thread).
           It also validates the command by checking if it is in the list of recorgnised commands for the shell.
	 
If commands passed are valid commands (i.e in the list of recorgnised commands), It checks for which specific command was entered and then runs it's code..(sends it off as a thread).

A "File_system_operations" class was implemented.

This handles various user level permissions to files and folders in the Shell environment.
It also handles getting the sizes of each files in the shell, date accessed, date changed.



===================================================================================================================================

How to run the shell.

From command prompt, navigate to the directory where the shell program folder is located e.g c:\Users\...\...\Helix\project folder>

On getting to the project folder, type python leave a space and the name of the file to be run. E.g. 
projectFolder>python driver.py

The above step gets you into our shell interface where you can run the implemented commands.
It begins with a prompt...%.

The commands that will work in the shell environment are listed below

================================================================================================================================
Commands implemented:

1.  ls:
	-l: lists all files/folders 
	
	-a: lists all files and sorts them according to time accessed(newest to oldest).
	
2. cat: Outputs texts to the screen

3. cd: 
	"directory_name": go to a user specified directory
	'~': go to home directory(not too accurate)
	'..': change to parent directory(go up one directory)
4. cp 

5. wc:  counts number of words in a file and outputs the result to the screen

6. rm:  Removes a file. 
        it also removes a directory.(rmdir)

7. mkdir: creates a new directory.

8. pwd: prints the current working directory path.

9. head: prints out the first few lines of a file.

10. prints out the last few lines/characters of a file.

11. Various user level permissions where also implemented.

12. grep: searches for a KEYWORD in a file and outputs all lines containing the keyword.

13. Chmod.


Commands not yet implemented:

1. pipe

2. command > file and file > command.

Commands not working correctly:
1. Chmod


