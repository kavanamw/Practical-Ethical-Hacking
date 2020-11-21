Abusing GPP

# Hack the box: Active to practice GPP 10.10.10.100
* We find both 53 and 88 open which should indicate that it might be a domain controller 
* lets look at 445 - SMB
* mget * will get all the files 
	* we like groups.xlm!!! the one for gpp
		* this gives us the cpassword right in the xml file
		* also gives domain name and that the tgs exists 
		* gpp-decrypt password
			* outputs the gpp password 
	* registry.pol