![image](https://github.com/Mistire/GTSTv1/assets/96515111/2e331dda-2831-4f4e-aed4-07721b800aae)
## Linux for Users

#### Linux Commands
- Linux Systems uses shell. The shell help us to Communicate with the kernel and helps to execute codes. [[Day 2]]
- Shell is also called *Terminal*.
- The terminal have 5 parts.
	- Username
	- Hostname
	- Current directory
	- Privilege
	- Command place
##### Linux Commands Basics
- A **Command** is a small program that do one task well
- **ls:** list information about the *files*(the current directory by default)
	- *ls -a*
	- *ls -l
	- *ls -R*
	- *ls -Rla*
- **cd:** changes current working directory
	- *cd /* => root
	- *cd * => home
	- *cd ..* => 1x Back
	- *cd ../..* => 2x Back
- **pwd:** prints the path of the working directory, starting from the root 
- **echo:** display lines of text that are passed as an argument
- **cat:** used to show the content of a file
- **touch:** create any kind of files
- **mkdir:** creates a new directory/folder
- **clear:** clears the screen
- **rm:** removes/deletes file or empty directory
	- *rm -r* => recursive
	-  *rm -i* => for prompt(ask)
	-  *rm -f* => force delete
- **cp/mv:** copy/move files and folders
- **grep:**  a filter that is used to search for lines matching a specified pattern and print the matching lines to standard output
	- *grep -i* "search" file =>  case insensitive
	- *grep -c* "search" file => counts numbers
	- *grep -l* "search" => displays file name 
	- *grep -R* "search" foldername => searches text in folders
	- *grep -v* "term" filename => displays without this term
	- *grep -n* "term" file => displays number of terms
- **wc:** used to find the number of lines word count, byte, and characters count in the specified file arguments
	- *wc -l*
	- *wc -w*
	- *wc -c*
#### Multiple Command Execution
- Multiple commands can be executed in 1 line
- Using 3 methods:
	- And (&&)
	- Or (||)
	- Piping (|) =>runs command by using the output of the 1st command as an input for the next one


