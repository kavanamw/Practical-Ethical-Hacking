Finding Subdomain with Assetfinder

* grab assetfinder from Github
	* tom might have other cool tools to use 
# Commands 
* assetfinder tesla.com
	* way faster than sublister
	* also finds asset related to tesla
* assetfinder --subs-only tesla.com
	* good to find only subdomains of tesla.com

#
## Script 
```
#!/bin/bash

url=$1

if [ ! -d "$url" ];then
	mkdir $url
fi

if [ ! -d "$url/recon" ];then
	mkdir $url/recon
fi

echo " [+] Harvesting subdomains with assetfinder..."
assetfinder $url >> $url/recon/assets.txt
cat $url/recon/assets.txt | grep $1 >> $url/recon/final.txt
rm $url/recon/assets.txt
```