Senstive Data Exposure 

* when a webapp inadvertently exposes data that should be kept private 
* passwords stored in a clear text file 
* is the application vulnerable
	* is data transmitted in clear text?
	* are any old or weak crypto algos used in older code
	* are default crytos in use?
	* is encryption not enforced?
	* does the user agent not verify if the received server cert is valid
* preventions
	* classify data procesed
	* apply controls as per the classification
	* does store data you don't need
	* make sure to encrypt all sensitive data at rest
	* ensure up-to-date and strong standard algorithmsm, protocols and keys are in place 
	* encrypt all data in transit with secure protocols 
	* disable caching for response that contain sensitive data 
	* store passwords using strong adaptive and salted hashing functions 

[Senstive Data Exposure](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A3-Sensitive_Data_Exposure)

[Security Headers](securityheaders.com)
* scan the headers returned from a website to see if there is any senstive data leaded 
* good for adding to a report 

# Nmap scan website commands
nmap --script=ssl-enum-ciphers -p port url 
	* report bad ciphers, good for a report as a low finding 