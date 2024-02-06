## Debugger ##
### What is a debugger? ###
  A debugger is a software tool used by developers to identify and fix issues in computer programs. It provides a controlled environment for monitoring and analyzing program execution, allowing developers to understand the behavior of their code and diagnose problems.
  Debuggers are essential for software development, helping to streamline the debugging process and improve overall code quality.
### What are the Best Linux Debuggers you can Use on Linux? ###
#### GNU Debugger (GDB) ####
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
     ```sudo yum check-update
     sudo yum install gdb

     # Output:
     # 'Loaded plugins: fastestmirror, ovl'
     # 'Loading mirror speeds from cached hostfile'
     # 'Package gdb is already installed.'
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
 
     
