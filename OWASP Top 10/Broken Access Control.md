Broken Access Control 

* [Broken Access Control](https://owasp.org/www-project-top-ten/OWASP_Top_Ten_2017/Top_10-2017_A5-Broken_Access_Control)
# Vulnerable 
* access control enforces policy such that users cannot act outside of their intended permsissions 
	* you shouldn't be able to go to the admin page without being authenticated as admin 
* bypassing access control checks by modifying url, internet application state, or simply using a custom api attack
* allowing the primary key to bechanged to another's user record 
* elevaton of privilege, acting as a user without loggin in, acting as an admin without loggin in 
* maniplating data (access control token, cookies) to get admin 
* force browsing to unauthenticated pages as an unauthenticated user or to privileged pages as a standard user
# Prevention 
* deny by default
* inplemement access control 
* model access controls should enforece record ownership 
* log access control failures 
* rate limit api access
* JWT token should be invalidatee on the server after logout 