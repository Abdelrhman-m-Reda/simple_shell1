<<<<<<< HEAD
ALX Simple Shell Team Project

Description
A simple UNIX command interpreter that replicates functionalities of the simple shell (sh). Additional functions are also included. This program was written entirely in C as a milestone project for ALX Africa Software Engineering.

Installation
Clone this repository into your working directory. For best results, files should be compiled with GCC and the following flags: -Wall -Wextra -Werror -pedantic -std=gnu89

Usage
After compilation, the resulting program can run stand-alone, either in interactive or non-interactive mode.

Interactive Mode
In interactive mode, simply run the program and wait for the prompt to appear. From there, you can type commands freely, exiting with either the "exit" command or ctrl-D.

Non-Interactive Mode
In non-interactive mode, echo your desired command and pipe it into the program like this:

echo "ls" | ./shell
In non-interactive mode, the program will exit after finishing your desired command(s).

Included Built-Ins
Our shell has support for the following built-in commands:

Command	Definition
exit [n]	Exit the shell, with an optional exit status, n.
env	Print the environment.
setenv [var][value]	Set an environment variable and value. If the variable exists, the value will be updated.
unsetenv [var]	Remove an environment variable.
cd [dir]	Change the directory.
help [built-in]	Read documentation for a built-in.
Credits
All code written by Abdelrhman-m-Reda and Shan-91
=======
PROJECT OVERVIEW

This group project is done as part of requrement for software engineering cousre at alx.
in this assignment we achieved some of the following learning objectives as per the project description
 .How does a shell work
  .What is a pid and a ppid
.How to manipulate the environment of the current process
.What is the difference between a function and a system call
program specification

simple shell 1.0
Simple shell 0.1
Write a UNIX command line interpreter.
Usage: simple-shell
Your Shell should:
Display a prompt and wait for the user to type a command. A command line always ends with a new line.
The prompt is displayed again each time a command has been executed.
The command lines are simple, no semicolons, no pipes, no redirections or any other advanced features.
The command lines are made only of one word. No arguments will be passed to programs.
If an executable cannot be found, print an error message and display the prompt again.
Handle errors.
You have to handle the “end of file” condition (Ctrl+D)
You don’t have to:
use the PATH
implement built-ins
handle special characters : ", ', , \, *, &, #
be able to move the cursor
handle commands with arguments
Simple shell 0.2
Simple shell 0.1 +
Handle command lines with arguments
Simple shell 0.3
Simple shell 0.2 +
Handle the PATH
fork must not be called if the command doesn’t exist
Simple shell 0.4
Simple shell 0.3 +
Implement the exit built-in, that exits the shell
Usage: exit
You don’t have to handle any argument to the built-in exit
Simple shell 1.0
Simple shell 0.4 +
Implement the env built-in, that prints the current environment
Simple shell 0.1.1
Simple shell 0.1 +
Write your own getline function
Use a buffer to read many chars at once and call the least possible the read system call
You will need to use static variables
You are not allowed to use getline
You don’t have to:
be able to move the cursor
Simple shell 0.2.1
Simple shell 0.2 +
You are not allowed to use strtok
Simple shell 0.4.1
Simple shell 0.4 +
handle arguments for the built-in exit
Usage: exit status, where status is an integer used to exit the shell
setenv, unsetenv
Simple shell 1.0 +
Implement the setenv and unsetenv builtin commands
setenv - Initialize a new environment variable, or modify an existing one - Command syntax: setenv VARIABLE VALUE - Should print something on stderr on failure unsetenv - Remove an environment variable - Command syntax: unsetenv VARIABLE - Should print something on stderr on failure
cd
Simple shell 1.0 +
Implement the builtin command cd:
Changes the current directory of the process.
Command syntax: cd [DIRECTORY]
If no argument is given to cd the command must be interpreted like cd $HOME
You have to handle the command cd -
You have to update the environment variable PWD when you change directory man chdir, man getcwd
Handler of this separator ;
Simple shell 1.0 +
Handle the commands separator ;
&& and ||
Simple shell 1.0 +
Handle the && and || shell logical operators
alias
Simple shell 1.0 +
Implement the alias builtin command
Usage: alias [name[='value'] ...]
alias: Prints a list of all aliases, one per line, in the form name='value'
alias name [name2 ...]: Prints the aliases name, name2, etc 1 per line, in the form name='value'
alias name='value' [...]: Defines an alias for each name whose value is given. If name is already an alias, replaces its value with value
Comments
Simple shell 1.0 +
Handle comments (#)
File as input
Simple shell 1.0 +
Usage: simple_shell [filename]
Your shell can take a file as a command line argument
The file contains all the commands that your shell should run before exiting
The file should contain one command per line
In this mode, the shell should not print a prompt and should not read from stdin
AURTHORS
sharone Achieng'
Abdelrhman-m-Reda
>>>>>>> 24326d84e6175c3a1ad6a3425fd1efd3fa4777d3
