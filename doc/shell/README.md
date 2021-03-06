# Getting started with shell

Shell is the program used by a Linux terminal to pass commands from the keyboard to the operating system.
Below are some exercises to help familiarize a user with using the terminal and reading and browsing man pages.

## Navigation and File or Folder Creation
1. Navigate to your home directory
2. List all the files in your home directory
3. Find the file in /etc/ that gives the name of your system
4. Open the .bashrc file in your home directory
5. Make a directory in your home directory for this exercise and move into that directory
6. Make an empty file
7. Make a file using a text editor
8. Make a new directory and copy all the files from /etc/apt into that directory
9. Remove the directory made in 8.

## Redirecting Output and Pipes

As with most command line programs which display their results do so by sending there results to something called "standard output"
By default standard output is directed to the display, but there are two ways to direct the output somewhere else.
The ">" character is used to redirect standard output to a file, e.g. $ ls > ls_output.txt which writes the output of ls to the file ls_output.txt
The "|" character (pipe) is used to redirect standard output to the input of the next command.   e.g. lspci | less will pass the output into less which allows for paging lots of output.

1. Check out the man pages for lspci, ls, cat, grep, tr, sed, cut, more, less, and find
2. Write the contents of lspci to a file
3. Print the contents of the file to the screen, and use more or less to find your video card
4. Using the file from 2, print only the line with your video card to the screen
5. List only the files in /etc
6. Print only the owners and groups for files and directories in /etc
7. Print only the permissions for all the files and directories in /etc
8. Using the output from 7, replace "r" with "read", "w" with "write", "x" with execute, and "-" with None (hint, you may need to use multiple pipes)
9. Make the file from 2 all uppercase
10. Using tr and the file from 2, replace all the spaces with new lines
11. List all the files in /etc which end in .conf (there are at least two ways to do this)
