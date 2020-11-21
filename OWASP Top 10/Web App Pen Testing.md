Web App Pen Testing

## Stages
1. unauthenticated 
	* the stage when you are not logged in and can only access some stuff
	* chekc out all the pages, see if you can get in with defaults creds 
2. authenticated
	* you have user access but not admin access
	* might get a lot more access to vuln pages but not admin ones
3. admin level
	* full control of the webapp 
## Burp Stuff
* Proxy
	* add the main url to the scope 
	* click through the stuff in the target tab under the url to see if there is anything else intresting 
		* pro edition has the scan feature 
		* when doing a real pen test do this 
		* scan, was spidering, will craw to other sites to see if it can get other access
			* might find vulns right in burp like cross site scripting 
			* good to have but not completly reliable 
			* this is inser more   
* Repeater
	* allows us to repeate requests 
	* proxy tab -> options -> under Intercept Client Requets turn on the and operator -> under Intercept Server Responses turn on the and operator 
		* this will keep the intercepter within scope stopping firefox requets showing up 
	* lets us delete a cookie and see the raw response, change a GET to a POST
* Intruder 
	* store a payload and use it 
	* under the extender -> app store -> some will be free 
		* install turbo intruder for free to increase speed for free 
* Comparer
	* see the differences between two items to see the difference between two responses
* Decoder 
	* not as nice as CyberChef but still handy right in burp 