## Debugger ##

### What is a debugger? ###
  A debugger is a software tool used by developers to identify and fix issues in computer programs. It provides a controlled environment for monitoring and analyzing program execution, allowing developers to understand the behavior of their code and diagnose problems.
  Debuggers are essential for software development, helping to streamline the debugging process and improve overall code quality.
### What are the Best Linux Debuggers you can Use on Linux? ###
### GNU Debugger (GDB) ###
The GNU Debugger (GDB) is a highly versatile and widely used debugger for Linux. As an open-source tool, GDB provides developers with an extensive range of features and capabilities to effectively analyze and debug their programs.
####  What can GDB do? ####
  - Set breakpoints: Pause program execution at specific points to examine variables and analyze behavior.
  - Step through code: Execute code line-by-line, inspecting changes and identifying issues.
  - Inspect variables: View values of variables at any point, understanding data flow and potential errors.
  - Modify variables: Change variable values during debugging to test outcomes and pinpoint root causes.
  - Print expressions: Calculate values on the fly using expressions, gaining insights into program logic.
  - Examine memory: Analyze memory contents for potential corruption or unexpected values.
#### How to installing the GDB ####
The GDB have 2 way to install
  1. Installing by Command
     
     ```sudo apt update
     sudo apt install gdb

     # Output:
     # 'Reading package lists... Done'
     # 'Building dependency tree'
     # 'Reading state information... Done'
     # 'gdb is already the newest version (8.1-0ubuntu3).'
     # '0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.'
     ```
     
  2. Installind by Sourcee Code
  
     ``` wget http://ftp.gnu.org/gnu/gdb/gdb-10.2.tar.xz
     tar -xvf gdb-10.2.tar.xz
     cd gdb-10.2
     ./configure
     make
     sudo make install

     # Output:
     # 'config.status: creating Makefile'
     # 'config.status: creating config.h'
     # 'config.status: executing depfiles commands'
     # 'config.status: executing libtool commands'
     # 'Making install in .'
     # 'make[1]: Entering directory '/home/user/gdb-10.2'
     # 'make[2]: Entering directory '/home/user/gdb-10.2'
     # 'make[2]: Nothing to be done for 'install-exec-am'.
     # 'make[2]: Nothing to be done for 'install-data-am'.
     # 'make[2]: Leaving directory '/home/user/gdb-10.2'
     # 'make[1]: Leaving directory '/home/user/gdb-10.2'
     ```
     
#### Useful GDB commands: ####

command | Description 
--------| -----------
run or r|Executes the program from start to end.
break or b | Sets a breakpoint on a particular line.
disable | Disables a breakpoint
enable | Enables a disabled breakpoint
next or n | Executes the next line of code without diving into functions.
step | Goes to the next instruction, diving into the fuction.
list or l | Display the code.
print or p | Displays the value of a variable.
quit or q | Exits out of GDB.
clear | Clars all breakpoints.
continue | Continues normal execution

example:
set a breakpoint : let's introduce a break point, say line 5.


```
(gdb) b 5
Breakpoint 1 at 0x5555555546a8: file test.c, line 5.
(gdb) |
```

if you want to put breakpoint at different lines, you can type "b line_number".

By default "list or l" display only first 10 lines.

-Start GDB

` gdb `

![307](https://github.com/Chinjuku/Code-Development-1/assets/109953279/bf17e3df-7729-4d39-bd1f-be8fa1c5ee83)




#### The LLDB Debugger ####

reference

https://www.geeksforgeeks.org/gdb-step-by-step-introduction/
https://installati.one/install-lldb-ubuntu-20-04/
https://ioflood.com/blog/install-gdb-command-linux/#:~:text=In%20most%20Linux%20distributions%2C%20the,command%20sudo%20yum%20install%20gdb%20.
https://www.sourceware.org/gdb/
https://www.scaler.com/topics/linux-debugger/
 
     
