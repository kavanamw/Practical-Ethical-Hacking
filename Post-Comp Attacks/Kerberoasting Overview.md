Kerberoasting Overview

![54d630d39e7e3bb49cdaa43b162b82e6.png](../../_resources/97d1a4dee9c9450c8f8de8ea26f7de28.png)

# 
* any valid user get a ticket, once we have cracked the user creds we can use those to get into the Application server using a ticket from the Domain Controller 
* from impacket
	* python GetUserSPN.py Domain.local/user:password -dc-ip IP -request
	* Returns a hash you can then try to crack 