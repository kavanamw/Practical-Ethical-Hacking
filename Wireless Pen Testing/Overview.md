Overview

* 2 types of newwork 
	* WPA2 PSK - common for the home networks 
	* WPA2 Enterprise - self ex. 
* Activities Done
	* Evaluate the strength of the PSK
		* catch the handshake and try to crack it offline
	* Reviewing nearby networks 
	* Accessing guest networks
		* maybe no password or a weak password 
		* is the guest network seperate from the main network? 
	* Checking network access 
* Tools to use
	* a dual band card becuase 5G is common 
	* wirelesshack.org/best-kali-linux-compatable-usb-adapter-dongles.html 
	* check a current list to get a compatable card and chipset 
* The Hacking process
	* Place - place the card in monitor mode
	* Discover - discover info about the network, channel and BSSD (mac address)
	* Select - Select network and capture data
	* Perform - Perform deauth attack
		* kick someone off the network to then capture the handshake, option but speeds things up
	* Capture - Capture WPA handshake 
	* Attempt - Attempt to crack the handshake
		* hard with a good password, just like a hash 
# Commands and Tools
* Arimon-ag 
	* first run check kill - removes processes that might interfere
	* iwconig - check the config 
	* airodump-ng wlan0 mon - shows all the devices and detaials around the card 
		* the lower the negative power number, the closer 
	* airodump-ng -c (channel) --bssid (mac) -w (filename) (interface)
		* capture data from that device and save the data to a file 
	* Deauth a client
		* aireply-ng -o (number of times to run) -a (mac) -c (station from airdump) (interface)
		* might have to run several times 
		* don't do this over and over again becuase it could cause issues in the enviroment