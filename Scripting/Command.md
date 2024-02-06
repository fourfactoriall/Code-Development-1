# Basic of Shell Script
### Create file Shell script
```
touch hello_world.sh
```

### Find the path to your bash shell.
```
which bash
```
In my case, the path is ` /usr/bin/bash ` and I will include this in the shebang.

### Write the command.
```
echo "Hello World"
```
Edit the file hello_world.sh using a text editor of your choice and add the above lines in it.

### Provide execution rights to your user.
```
chmod u+x hello_world.sh
```
`chmod` modifies the existing rights of a file for a particular user. We are adding `+x` to user u.

### Run the script.
You can run the script in the following ways:
```
./hello_world.sh
bash hello_world.sh
```

## The Basic Syntax of Bash Scripting
Just like any other programming language, bash scripting follows a set of rules to create programs understandable by the computer. In this section, we will study the syntax of bash scripting.

### How to define variables
We can define a variable by using the syntax `variable_name=value`. To get the value of the variable, add `$` before the variable.
```
greeting=Hello
name=Tux
echo $greeting $name
```

### Arithmetic Expressions
Below are the operators supported by bash for mathematical calculations:

|OPERATOR | USAGE 
|-------- | ------
|+        | addition
|-        | subtruction
| *	       | multiplication
| /	       | division
| **       |	exponentiation
| %	      | modulus

<b>Examples >>> </b>
```
expr 10 + 10000
expr 30 / 2
```
Numerical expressions can also be calculated and stored in a variable using the syntax below:
```
var=$((expression))
```
<b>Example >>> </b>
```
var=$((3+9))
echo $var
```
Fractions are not correctly calculated using the above methods and truncated. <br>
For decimal calculations, we can use bc command to get the output to a particular number of decimal places. bc (Bash Calculator) is a command line calculator that supports calculation up to a certain number of decimal points. 
```
echo "scale=2;22/7" | bc
```
Where `scale` defines the number of decimal places required in the output.

### How to read user input
Sometimes you'll need to gather user input and perform relevant operations. <br>
In bash, we can take user input using the `read` command.
```
read variable_name
```
To prompt the user with a custom message, use the `-p` flag.
<b>Example >>> </b>
```
echo "Enter a numner"
read a

echo "Enter a numner"
read b

var=$((a+b))
echo $var
```

### Numeric Comparison logical operators
Comparison is used to check if statements evaluate to `true` or `false`. We can use the below shown operators to compare two statements:

OPERATION |	SYNTAX |	EXPLANATION
--------- | ------ | --------------
Equality |	num1 -eq num2	| is num1 equal to num2
Greater than equal to |	num1 -ge num2	| is num1 greater than equal to num2
Greater than|	num1 -gt num2 |	is num1 greater than num2
Less than equal to |	num1 -le num2 |	is num1 less than equal to num2
Less than |	num1 -lt num2 |	is num1 less than num2
Not Equal to |	num1 -ne num2 |	is num1 not equal to num2
