Custom Shell README
===================

Custom Shell is a simple command line interpreter, also known as a shell. It is designed to run on Unix-like operating systems, and provides users with a basic set of commands for interacting with the file system and running programs.

Getting Started
---------------

To use Custom Shell, simply clone this repository and compile the code using a C compiler such as gcc. Then, run the resulting executable file from the command line.

Features
--------

Custom Shell currently supports the following features:

-   Reading input from the user one line at a time using a custom getline function.
-   Parsing input into tokens, splitting on whitespace characters.
-   Executing commands using the `execve` system call.
-   Running commands in the background by appending an ampersand (`&`) to the end of the command line.
-   Changing directories using the `chdir` system call.
-   Exiting the shell using the `exit` command.

Usage
-----

To use Custom Shell, simply type commands at the prompt and hit enter. The shell will then execute the command and display the output (if any). For example:

sql

`$ ls -l
total 20
drwxr-xr-x 2 user user 4096 Apr 20 12:34 .
drwx------ 5 user user 4096 Apr 20 12:34 ..
-rw-r--r-- 1 user user  148 Apr 20 12:34 custom_shell.c
-rw-r--r-- 1 user user   48 Apr 20 12:34 Makefile
-rw-r--r-- 1 user user  789 Apr 20 12:34 README.md`

To run a command in the background, simply append an ampersand (`&`) to the end of the command line:

shell

`$ sleep 10 &
[1] 1234`

To change directories, use the `cd` command followed by the desired directory:

shell

`$ cd /home/user`

To exit the shell, use the `exit` command:

shell

`$ exit`

Limitations
-----------

Custom Shell is a basic implementation and has several limitations:

-   It does not support advanced features such as pipes or input/output redirection.
-   Error handling is minimal, and error messages are not always informative.
-   Some edge cases may not be handled correctly.

Future Development
------------------

In the future, we plan to add more features to Custom Shell, including:

-   Input/output redirection.
-   Pipes.
-   Command history and editing.
-   Tab completion.

Contributing
------------

Contributions to Custom Shell are welcome! If you find a bug or have a feature suggestion, please open an issue on the GitHub repository. If you'd like to contribute code, please fork the repository and submit a pull request with your changes.

License
-------

Custom Shell is released under the MIT License. See the `LICENSE` file for details.
