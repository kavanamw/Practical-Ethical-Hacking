SQL Injection Attacks

* an attack in which malicious SQL statements are injected into a sql database 
	* easy to avoid but still happens 
	* could read data, extract information, modify databaes, and maybe even get a shell 
* Common SQL Verbs
	* SELECT - retrieves data from a table
	* INSERT - add data to a table
	* DELETE - removes data from a table
	* UPDATE - modifies data in a table
	* DROP - deletes a table
	* UNION - combines data from multiple queries 
	* WHERE - filters records based on a specific comdition
	* AND/OR/NOT - filters reconrds based on conditions
	* ORDER BY - sorts records in ascending/decending order 
#
[A1:2017-Injection](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A1-Injection
#
* login page might send select * from users where email='input'
	* if you can send a single ' it will break the page 
	* if  you cen get a SQL error of any kind then you might have an sql injection 
	* look for the error in burp's repeater 
	* test' OR 1=1 --;
		* will run select * from users where email='test'' --
		* the -- will log us in as the first user in the database 
* Blind SQL Injection
	* a type of attack that asks the database true or false questions and determine the answer based on the applications response 
	* often used when the web application is configured to show generic error messages, but has not mitigated the code that is vulnerable to SQL Injection 