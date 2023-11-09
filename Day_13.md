# Reconnaissance (Information Gathering)
## What is Information Gathering?
- It is collecting data about some network / host / system
- Footprinting => Footstep + printing (logging)
- Footprinting is a very important part of Ethical Hacking. Almost 85% of Hacking.
### Why do we need recon?
- To get access on system first we have to know the system and knowing the system will lead you to know if the system is vulnerable
### Type of Information gathering
- Based on how we do the recon:
	- Active Footprinting
	- Passive Footprinting
#### 1. Active Footprinting
- It is the kind of information that is gathered by directly contacting the source of the information
- Doing Active Footprinting without permission is **ILLEGAL**
#### 2. Passive Footprinting
- It is the kind of Information that is gathered from another person, 3rd party or by checking public sources.
### What type of Information do you gather?
- We gather information for different things
	- **Host**
		- *Websites*
		- *Computers*
		- *Smart Phone*
	- **Network**
		- *Home Network*
		- *Company Networks*
	- **Person/Organization**
	- **Application**
#### 1. Websites
- The Information we gather about a websites are:
	- IP Addresses
	- Development frameworks
		- Technologies used and versions
	- Name
	- DNS information
	- Subdomains, Assets, Contents
##### To get IP
- To get IP address of some website:
	- Active recon
		- ping < website link >
		- nslookup < website link >
		- host < website link >
	- Passive recon
		- www.nslookup.io
##### To get development frameworks
- Using simple browser extension
	- Wapplyzer
	- Builtwith
- Terminal tool
	- whatweb
##### To get the name
- You can see the title of the website or texts inside the page also the url.
##### Details about domains
* Terminal + website tool
	* sudo apt install whois
	* whois
	* dig
#### 2. Computers / Phone
- The information we gather about a computers / hosts are 
	- IP Addresses
	- OS information
	- Host name
	- MAC address
	- Open service or ports
#### 3. Networks
- The information we gather about a network are:
	- IP addresses
	- Port, services
	- Class and type of Network
	- Subnets
	- Hosts on that Network
	- Strength and security of that Network
#### 4. Personal Information
- The Information we gather about a person are:
	- Full name
	- Address
		- Physical Address
		- All Social Media Address
		- Phone address
	- What that person loves
	- Job
	- Friends
	- Status
	- Skills
- Persons information can be gathered by active and passive.
- Gathering and Analyzing Different Information based on Public resource is called OSINT(Open Source Intelligence)
##### Getting names by Phone number
- www.truecaller.com/
##### Getting Social media Addresses
- Using search engines(google, bing, yahoo)
- Sherlock from github...on terminal
##### Getting Physical Address
##### IP geolocation
- If you go the private address of someone you can insert it to www.iplocation.net
#### 5. Applications / Software
- The information we gather about applications are:
	- What they're made of
		- Which programming language is used
		- Which framework is used
	- Source codes
	- Their logic and Function
### Reverse image search
- It is a technique of searching with images
- We can use:
	- https://tineye.com/
	- https://www.labnol.org/reverse/
	- https://images.google.com/
### Google Dorking( Google Hacking Database)
- It is using different google operators to effectively optimize search results.
- It also involves using google to identify vulnerabilities in websites
- Results are highly customizable
#### Basic operators
- For inclusion of something common (+)
- Terms you want to exclude (-)
- Search for an exact term (" ")
- Any word ( * )
	- If you include * within a query, it tells Google to try to treat the star as a placeholder for any unknown term(s) and then find the best matches.
- Boolean 'OR' ( | )
#### Advanced Operators
- These are Syntaxes used by Google.
	- intitle
		- Google returns results with the word/phrase found within the title of the page
			- intitle:index.of
			- intitle:”Hackers Bible”
	- inurl
		- Finds a specific term within the URL
			- inurl:view/index.shtml
	- filetype
		- Searches for a specific filetype
			- “Hacking” filetype:pdf
			- filetype:txt
	- Intext
		- Google returns links that contains Texts from that link
			- intext:”Hackers in Ethiopia”
- Further on Google dorking:
	- https://www.exploit-db.com/google-hacking-database
---