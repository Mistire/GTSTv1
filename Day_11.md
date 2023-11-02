![image](https://github.com/Mistire/GTSTv1/assets/96515111/b92cb874-dd32-4a9e-a073-8039ae548c5f)
## Further on Bash
### Regular expressions /regex
- Most filter validation on any platform are done by Regular expression/regex
- They are patterns that helps filter texts, space, tabs and symbols
- Like telegram or other platforms filtering links inside group, filtering some bad words are all regex
- Regex is a pattern
- Regex are used on linux tools called grep, awk, and sed
- The pattern is same but the implementation may differ on programming languages
### Metacharacters
- They are regex patterns symbol for filter
- They are:
	- .
	- ^
	- $
	- *
	- +
	- ?
	- { }
	- [ ]
	- ( )
	-  |
	-  \
#### Dot ( . )
- Used to get all the line except new lines
- **Syntax:** 
	- . =>This means give me all lines except the new lines
#### Caret ( ^ ) - Assertion
- Used to get line that start with pattern
- **Syntax:** ^ hello
	- This means lines that start with hello
#### Dollar sign ( $ ) - Assertion
- Used to get the line that ends with some patterns
- **Syntax:** hello$
	- That ends with hello
#### Plus ( + ) - Quantity
- Used to get line that have pattern that occurs 1 and more times
- **Syntax:** hello+
	- A text hello that have at least 1 times and more
#### Asterisk ( * ) - Quantity
- Used to get line that have pattern that occurs 0 and more times.
- **Syntax:** hellos*
	- A text hello that s at least 0 times and more
#### Question mark ( ? ) - Quantity
- Used to get line that have pattern that occurs 0 and 1 times
- **Syntax:** hellos?
	- A text hello that have at least 0 times or 1 time
#### Curly Bracket ( { max, min } ) - Quantity
- Used to get line that have pattern that occurs min and max times. It is custom
- **Syntax:** hellos{ 1, 3 }
	- A text hello that have at least 0 times or more
#### \\w
- Used to get alphanumeric
- **Syntax:** \\w
	- All texts except newlines and symbols
#### \\W 
- Used to get all except alphanumeric
	- **Syntax:** \\W
#### \\s
- Used to get whitespace
- **Syntax:** \\s
#### \\S
- Used to get all except whitespace
- **Syntax:** \\S
#### \\d
- Used to get Digits/numbers
- **Syntax:** \\d
#### \\D
- Used to get all except Digits/numbers
- **Syntax:** \\D
#### Pipe ( | ) - OR
- Used to search 2 different things
- **Syntax:** a | b
#### Escape ( \\ )
- Used to search symbols that are metacharacters
- **Syntax:** \\sign
#### Square Brackets ( \[ ] ) - Custom pattern
- Used to create your own pattern
- **Syntax** : [ pattern ]
### BASH for regex
- We use =~ operator for regex
- Here we use double brackets for our conditional statements
- **Syntax:** 
	- patterm="YourRegex"   if [[ $input =~ ${pattern} ]]
#### Bash else if
- When comparing condition more than 1, it uses elif like python
	- *if condition  then body elif condition then body else body fi*
#### Loops 
- On Bash, there are 3 types of loops
	- For loop
	- While loop
	- Until loop
##### For loops
- The iteration may be different here. We can use arrays like list python but we don't have range in bash but we can do { a...b } this iterates from a to b.
- **Syntax:**
	- *for condition do body echo done*
	- *for (( i=1; i < 10; i++ do echo done*.... For loop without sequence data
	- *for num in {start..stop..step} do echo $num done*...For loop with increment/decrement
##### While loop
- *while [ expression]  do body done *
##### Continue Statement
- is a function that helps to break the loop there and start it from the up again. It's python equivalent is called 'pass'
##### Until loop
- It is the same but this one exits the loop when the expression is true.
- **Syntax:** *until [ expression ] do body done*
##### Function
- **Syntax:** *function_name( ) { body }           function name*
- When we have function and the arguments will be $1, $2
- If we use $? it will call the return value
#### Bash and Linux
- We can run linux command inside our bash
	- *echo "I can run appt commands in my bash"  apt update*
- Bash for loop in one line
	- *for i in { 1..5 } do echo "Hello $i" done*
- To access files in current directory using * sign
	- *echo  *
- For loop on terminal
	- *for command; do body; done*
---



