Broken Authenticaton 

* Is the applicaton vulnerable 
	* permits cred stuffing?
	* permits brute force attack?
	* permits weak or well known passwords 
	* permits easy forgotten password recovery options 
	* uses plain text, encrypted, or weakly hashed passwords 
	* has missing multi-factor auth
	* does not rotate session IDs after successful login
	* does not properly invalidate session IDs, user sessions or authention tokens 
	* saying invalid email/valid email but invalid password, information disclosure 
* How to prevent
	* multi-factor auth
	* no defaul creds
	* weak password checks
	* good cred recovery
	* limit or delay failed login attempts, log suspected cred stuffing or brute force logins 
	* user server-side, secure, built in sesion mamager that generates a new random session id with high entropy after login 

[Broken Authentication Link](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A2-Broken_Authentication)