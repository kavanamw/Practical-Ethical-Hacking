Insecure Deserialization 

[Insecure Deserialization](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A6-Security_Misconfiguration)

* Serialization - converting data to be sent over the network
	* XML, Json...
* Deserializatoin - the opposite 
* insecure
	* send a malicious payload and when recieved it gets deserialized and runs the code 
* Prevention
	* do not accept serialized objects from untrusted sources 
	**readup on ysoserial** 