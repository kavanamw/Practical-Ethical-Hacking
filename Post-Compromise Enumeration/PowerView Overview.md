PowerView Overview

* get the package from Github
* ## powershell -ep bypass 
	* does some bypassing to let us run some stuff 
# Powerview domain enumeration commands 
	* Get-NetDomain 
	* Get-NetDomainController
		* net domain controller information to get where it is and what it's called 
	* Get-DomainPolicy
		* get policy info for the domain 
		* (Get-DomainPolicy)."system access"
			* password information to help crack passwords 
	* Get-NetUser
		* Might get user descriptions 
	* Get-NetUser | select [item] 
		* like a grep filter 
	* Get-UserPrioperty 
		* '' -Properties pwdlastset 
		* get when passwords were last signed in 
			* good way to find honeypot accounts 
	* Get-NetComputer 
		* lists all the computers on the domain 
		* '' -FullData
	* Get-NetGroup -Groupname "Domain Admins"
		* '' '*admin'
	* Invoke-ShareFinder