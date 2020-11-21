XXE Attack and Defense 

* Does not work when running Juice Shop in Docker 
## The Exploit
* make a new account 
* under the complaint section there is a file upload feature 
	* can be very bad for a web app if not done well 
	* check for client side validation on the file type 
* in our case it should return the /etc/passwd file 