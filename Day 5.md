![image](https://github.com/Mistire/GTSTv1/assets/96515111/236d583d-8147-41f7-822c-34d9c631f0d2)

## Advanced Linux User
#### Some advanced user commands
- To change password of a user
	- *sudo passwd username*
- To change user id
	- *sudo usermod -u new_id username*
- To delete User
	- *sudo userdel -r username*
- To change users on terminal
	- *sudo username*
#### Sudoers file
- It is a file in Linux and Unix that administrators use to allocate system rights to system users
- The user that is created doesn't have the power to use sudo as the original one
- This is because it is not added in the sudoers file
- To access this file
	- sudo visudo


![image](https://github.com/Mistire/GTSTv1/assets/96515111/810caa6a-528b-48da-b11e-41b2509e888a)

#### Linux File Permission
- Every file on Linux have their own
	- Owner
	- Permissions
- There is 5 main parts
	- Permission
	- Owners
	- Date
	- Size
	- filename
##### Ownership
- Ownership is the owner of the file
- There are two kind of Owners
	- User
	- Group
- To change the owner of file 
	- *chown user:group filename*
- There are 3 types of permissions
	- Read
	- Write
	- Execute
- The permissions have 3 parts
	- User(u) => power of user defined on the ownership
	- Group(g) => power of the group defined on the ownership
	- Other(o) => power of other users
	- All(a) => power of all which can be found in the 3 above owners
- Command to change permission of file
	- *chmod parameter filename*
- It can be expressed in two ways:
	- Parameters in Symbol
	- Parameters in Numbers


![image](https://github.com/Mistire/GTSTv1/assets/96515111/33df68e1-4643-40d8-8d06-160ac6a61935)

#### Special File Permission
- There are another 3 special permissions, you may encounter on your pentest
Journey.
- They are
	- SUID bits(s) - set user ID bit - add 4 infront of our numeric value -> 4000
	- SGID bits(S) - set group ID bit - add 2 infront of our numeric value -> 2777
	- Sticky bits(t) - set other ID bit - add 1 in front of our numeric value -> 1602
- They are permissions like the execute(x), but they will set the execute permission to the user who settled them.
- Example: if mr.A add suid bit to a program that program will be executed with permission of mr.A
	- Meaning if admin add suid bit on some program. Then any user if they got that program they can run it as root with any sudo password
#### Package installation on Linux
- On Linux to install softwares we use package managers.
	- Ex: apt,pacman,pkg,...
-  We will use debian package manager.
-  On debian the package manager i called ‘APT’ also there is called ‘dpkg’
-  Package managers are a free-software user interface that work with an online server to handle the installation and removal of software on Debian, and Debian-based Linux distributions.
#### Advanced package tool (apt)
- Apt is a free-software user interface that work with an online server to handle the installation and removal of software on Debian, and Debian-based Linux distributions. 
- It is used for online and offline purpose.
-  The old ‘apt’ used as ‘apt-get’
- Syntax:
	-  *sudo apt update
	- *sudo apt search softwarename
	- *sudo apt install softwarename
	- *sudo apt remove softwarename
	- *sudo apt upgrade
	- *sudo apt purge softwarename
#### Package dependencies
- A software can be built based on another program
called **modules**
- Program to work properly, the dependencies have to be installed successfully.
-  Those package managers install the *software + dependencies.**
#### Dpkg / Debian package manager /
- Dpkg is an offline package managing
program.
- Packages on Debian have an extension *“.deb”*
- Syntax:
	- sudo dpkg -i packagename
	- sudo dpkg -r packagename
	- sudo dpkg -P packagename
