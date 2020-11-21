Token Impersation Overview 

![3fd5573114c35988c15568cb26caa4c0.png](../../_resources/e6997299d128493f8d9d454fba3fd8ac.png)

* Meterpreter has an impersonate_token user\\user
	* this can give us a shell 
	* We can dump hashes from that shell 
	* get priv esc with the tokens and get more hashes from there
* If you have a domain admin token then you own that network 

# Comands
* from meterpreter you can load different tools, type load to see whats available 
	* loca incognito 
	* can impersonate_token, list_tokens, and other things 
	* impersonate_token marvel\\administrator
		* you now get a shell with these creds 
	* rev2self to return to who you were 

# Mitigation Starategies 
	* limit user/group token creation premission
	* account tiering 
	* local admin restruction 