# Linux Commands
A)  open terminal from terminal 
--
1.gnome-terminal
--terminal command to open terminal .

2.gnome-terminal -e [command]
--terminal command to open terminal and execute command in new terminal

3.gnome-terminal --command="bash -c '[command1]; [command2]; $SHELL'"
--bash -c tells it is a bash command 
--command1 and command2 are commands to be executed on new terminal.
--$SHELL makes the terminal remain open to work on.

4.gnome-terminal --tab  
 --opens a new tab in the same terminal.

B) dealing with arguments
--
We can make a tool which take arguments, for that we need to understand 
how to work with arguments.

1.$n
--we can involve values of our arguments in our code by using $ followed by argument number in place where we want that argument value.Depending upon the number of argument we can use $1,$2,$3,$4....$n.

2.$@ 
--contains values of all the arguments.

3.$0
--returns the name of the script on which you are working.

4.$#
--total number of all the arguments passed with the command.

To implement the following argument manipulation techniques make a script and give it a name and give argument(s) and run it.
---------Script---------- 
#! /bin/bash
echo $1
echo $#
echo $@
echo $#

