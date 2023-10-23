![image](https://github.com/Mistire/GTSTv1/assets/96515111/1d988d75-5e68-40d1-a60d-7e4e10b2089f)

## Finishing Linux
#### Script Installation
- Some hacking tools are made open-source by the developers, so we could download that from github by cloning to our terminal  and use it.
#### Script Installation
- Scripts are made with scripting languages(programming) like *Python, bash, go, ruby*
- So when we use these programming languages to do tasks their is something called *modules/libraries* these are needed to run the script as the dependencies.
- Examples:
	- **Python**: to install python modules we use -> *pip install module name
		- For requirements file -> *pip install -r requirements.txt
	- **Go**: to install go modules -> *go install module name
	- **Ruby**: to install ruby modules -> *gem install module name
##### Python Installation
- If pip is not found there will be an error
![[Pasted image 20231021121928.png]]
- It will install ![[Pasted image 20231021121955.png]]
- If the package is already installed
 ![[Pasted image 20231021122111.png]]
##### Go Package installation
- Go scripts are scripts made with go-lang(go programming language).
- There are 2 installation methods.
	- Old version
	- New version
- Old version
![[Pasted image 20231021122252.png]]
- New version
	- Downloading the package => go install github.com/lc/gau/v2/cmd/gau@latest
	- Moving the file to /usr/bin => sudo mv filename /usr/bin
##### Errors that may happen
- Don't close apt while installation
- Repository errors, if this happened you can fix it using
	- *sudo apt edit-sources*
#### To get help on the Linux commands
- You could use man(manual) with the command you want to know about
- You could use help with the command you want to know about
#### Linux Processes and Services
- **Process**: number of instances of running program
- To get the process => *ps option
- More commands
	- *ps -> for process running on my shell*
	- *ps -A -> view all running process*
	- *ps -u username -> view user processes*
- PID - Process ID
- To stop process
	- *kill option PID*
- More on kill
	- kill -19 PID -> to stop the process
	- kill -18 PID -> to resume the process we stopped
	- kill -9 PID -> to stop a process immediately
- htop and top could be used to see active processes
#### Foreground/ background
- Thus far, we have run commands at the prompt and waited for them to complete. We call this running in the “foreground.”
- Thus far, we have run commands at the prompt and waited for them to complete. We call this running in the “foreground.”
- To get the background process back to foreground we use *fg*
#### Null device
- **/dev/null** - Redirects output to nowhere.
- On shell there are two things
	- STDERR = 2
	- STDOUT = 1
- To redirect the errors from a command result we use
	- command 2> filename
- To redirect the error free output
	- command 1> filename
- To get error free result
	- command 2> /dev/null
#### Symbolic linking
- Symbolic Linking is a process of creating a linked shortcut form of a file to some pre-existed file or folder using its file path
	- *ln -s source_filePATH filename*
#### Alias
- It gives name to some bunch of commands
	- Ex: alias remi='ls -la'
- It doesn't work after the terminal is closed. To make it work it must be added to the config files
#### Tmux - Terminal Multiplexer
- It is used to classify out terminal work
- To Create config file type
	- nano .tmux.conf
	- Type this
		unbind C-b
		unbind l
		set -g prefix C-a
		unbind %
		bind e split-window -h
		bind o split-window -v
		set -g base-index 1
		setw -g pane-base-index 1
		Save it | exit tmux and open again
- To split horizontally
	- *^A then o*
- To split vertically
	- *^A then e*
- To exit
	- *^A then x or*
	- just type ‘exit’
- To create tab
	- *^A then c*
- To rename the tab
	- *^A then ,(comma)*
- To switch tabs
	- *^A then numbers*
- To switch partitions
	- *^A then arrow*
#### Wget
- A tool used to download files from websites/server
- Syntax:
	- *wget option link*
#### Find
- To search for files, folders, music, videos
	- *find searchpath options searchword*
	- *find / -name "linux"*
	- *find /home -perm 777*
	- *find -type f | find -type d*
