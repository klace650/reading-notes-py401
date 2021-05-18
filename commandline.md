## 1 The Command Line
- The command line is a text based interface to your OS
- Begins with a prompt for a command
- BASH stands for Bourne Again Shell - why?
- The shell is what determines how the terminal behaves after commands

- ``echo $SHELL`` to display/verify bash is running (or whatever shell)

- Arrow key to scroll command history - we know this 

## 2 Basic Navigation

How to move around in the system from the command line:

``pwd`` : present working directory

- this will show the file path to current directory
- no args

``ls`` : short for list

- will list out files and directories in pwd  
- can have args *I didn't know this*  
- ``-l`` will do a long listing - much information  
- ``/etc`` will list directories contents

### Paths

Very important with navigating the terminal - its the way you get to certain files.

Root is the very top of the structure - denoted by a single ``/`` (slash)

*Two types:*

1. Absolute - specify a file path from root  *BEGINS w/ SLASH*
2. Relative - from pwd  *NO SLASH*

More things:

``~`` (tilde): used to refer to the home directory  
``.`` (dot) : reference to pwd  
``..``(dotdot) : reference to parent directory
``cd``  - change directory, no args takes you to home directory  
``tab`` - will auto complete stuff thats been used recently  