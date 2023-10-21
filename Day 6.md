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
