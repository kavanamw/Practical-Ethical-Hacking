SQL Injection Defenses

* Defense 1: Parameterized Statements 
	* ensure that the inputs are used safely in SQL statements 
	* Ex. "SELECT * FROM users WHERE email=?"
	* Ex. "SELECT * FROM users WHERE email=""+ email +""";
		* where email is a variable 
* Defense 2: Sanitizing Input
	* clean the input so that it is defidently the kind of input you want beyond just text