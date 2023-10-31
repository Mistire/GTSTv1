## What is Bash Sctipt?
- **Bash** => *Bourne Again Shell*
- It is a shell that helps us to interact with the kernel
- Script is a file that contains shell commands in a simple and clear algorithm
- The original is sh - Bourne shell
- Bash files can have ".sh" extension but  it could also be done without ".sh" too
- The files have to have executable peremission
### Uses of bash
- Script development
- Automating tasks
- Simplifying your linux ability
- Developing hacking scripts
### Displaying output
- To start every bash scripts use shebang
	- #!/bin/bash
	- #!/bin/sh
- To display outputs on bash
	- echo "TEXT"
- To run a project
	- /bin/bash hello.sh
	- ./hello.sh -> need x
	- hello -> need x
#### Variables
- Bash variables are almost the same with Python variables with some exception.
- **Syntax:** VARIABLE_NAME=value
- **Exception:** 
	- No space between the equal sign
	- Never start with numbers
	- Use double quotes only
- To use the variable we will use the dollar sign before the variable name
- To display the variable sticked with other text use ${VARIABLE_NAME}
- Bash variables are string by default
- The set command can be used to assign values to positional parameters
- **Syntax:** set $value1 $value2 $value3
#### System Variables
- Are variables declared by the system
	- echo $BASH
	- echo $BASH_VERSION
	- echo $PWD
#### Variables and Data types
- **Arrays:** 
	- Arrays are list or tuples on python
	- **Syntax:** 
		- var=("list1"list2"list3")
		- To display echo
			- ${var[0]}
		- To get all the elements
			- ${var[@]}
		- To get the index
			- ${!var[@]}
		- To get the length
			- ${#var[@]}
		- To add elements to the array
			- var[4]="list5"
		- To remove from the array
			- unset var[3]
#### Bash Input
- There two methods to accept input in bash
	- **Read function**
	- **Arguments**
##### Bash read
- Read used to accept inputs while the script is running
- **Syntax:** 
	- read -p "TEXT TO DISPLAY" var
	- read -sp "PASSWORD:" var => used to accept hidden texts like password
	- read -a var => for accepting arrays(lists)
##### Arguments
- These helps to get input before the script starts
- **Syntax:** 
	- Just use $0-$9 to work with the input
#### Comments
- **For single line**
	-  # single line comment
- **For multi line**
	- << COMMENTS
		First line comment
		Second line comment
		Third line comment
	 COMMENTS
##### Bash Sleep
- Sleep used to make the script appear after the given time
- **Syntax:** 
	- sleep < number >s
##### Operation
- To do mathematical operation we'll use $(( expression ))
- Let keyword is used for assigning variable
1. **Arithmetic Operations**
	- Addition $(( a + b ))
	- Subtraction $(( a - b))
	- Multiplication $(( a * b ))
	- Division $(( a / b ))
	- Exponential $(( a ** b))
	- Modulo $(( a % b))
2. **Assignment Operations**
	- Increment "let a+= 3"
	- Decrement "let a-= 3"
	- Multiply "let a*=3"
	- Divide "let a/=3"
3. **Comparison Operation**
	-  *Alphabetic Comparison*
		- Greater than => -gt
		- Less than => -lt
		- Greater than and equals to => -ge
		- Less than and equals too => -le
		- Equal => -eq
		- Not equal => -ne
#### If/else condition
- **Syntax:**
	- *if [ condtion ] *
	  then
		  body
	  else
		  body
	  fi
- If [ condtion ] is used => alphabetic comparison will be used
- If (( condition )) => numeric comparison will be used
---