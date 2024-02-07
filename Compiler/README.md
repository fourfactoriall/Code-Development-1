# Compiler

A compiler is a special program that translates a programming language's source code into machine code, bytecode or another programming language. The source code is typically written in a high-level, human-readable language such as Java or C++. A programmer writes the source code in a code editor or an integrated development environment (IDE) that includes an editor, saving the source code to one or more text files. A compiler that supports the source programming language reads the files, analyzes the code, and translates it into a format suitable for the target platform.

The program written in a high-level language is known as a source program, and the program converted into a low-level language is known as an object (or target) program. Without compilation, no program written in a high-level language can be executed. For every programming language, we have a different compiler; however, the basic tasks performed by every compiler are the same. The process of translating the source code into machine code involves several stages, including lexical analysis, syntax analysis, semantic analysis, code generation, and optimization.

- - - -
<br />

## Linux Compiler
### GCC

In Linux, the GCC stands for GNU Compiler Collection. It is a compiler system for the various programming languages. It is mainly used to compile the C and C++ programs. It takes the name of the source program as a necessary argument; rest arguments are optional such as debugging, warning, object file, and linking libraries.

GCC is a portable tool, and it can run on many operating systems. Also, it can be ported to Windows by using some tools such as Cygwin, MinGW, and MinGW-W64. As it is a key component of GNU toolchain, it contains the following components for developing applications and operating systems:

### GCC Compiler Process

![gcc_process](https://github.com/KanNattawat/Comor-Project-image/blob/main/Pre-Processor%20(1).png?raw=true)

* ***Pre-Processing*** is the first step of the compiling process. In this process, the header files are searched and copied to the source code file. It removes comments, expands macros, and includes files.

* ***Compilation*** process runs the code into the GCC module. In this step, the preprocessed files are converted into assembly language which is just an intermediate-level human readable language. The main purpose is to communicate with the hardware.

* ***Assembly*** process converts the assembly code into binary, machine language code. In this step, all the machine starts to understand the program’s instructions.

*  ***Linking*** is the last step in the whole compiling step. In this step, all the source codes are merged and even the library functions are considered. There’s also dynamic linking where the codes are not copied but binary file names are put inside the code.

### GCC Command
* ***gcc:*** This is the command itself.
In Linux, the gcc command is used to compile C and C++ programs. Below is a basic syntax along with some common options:

      gcc [options] [source files] [-o output file]

Here's what each part means:
* `gcc` : This is the command itself.

* `[options]` : These are optional flags that modify the behavior of the compiler. Options are preceded by a hyphen (-). Some common options include
  * `-c` : Compile or assemble the source files, but do not link.
  *  `-o` : Specify the name of the output file.
  *  `-Wall` : Enable all warning messages.
  *  `-g` : Generate debugging information.

* `[source files]` : These are the source files (C or C++ files) that you want to compile.
* `[-o output file]` : This option specifies the name of the output file. If omitted, the default output file is usually a.out.


