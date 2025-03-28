#!/bin/bash
##This script is an example for tasks to be executed for day1 scripting challenge

# Task  2: Echo
echo "This is Day1 scripting challenge"

# Task  3: Variables & # Task  4: Using Variables
Number1 = "$1"
Number2 = "$2"
Sum = $((Number1 + Number2))
echo "The sum is $Sum

# Task  5: Using Built-in Variables
echo "The name of the script is $0"
echo "The current users name is $USER"
echo "The user's home dir is $HOME"

# Task  6: Wildcards
echo "List all the text files in current directory"
ls .*txt
