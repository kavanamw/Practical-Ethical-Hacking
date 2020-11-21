Scanning with nmap

    Used networkdiscover to find the ip of the vuln ip 

    Used nmap to find open ports on the vuln system 

        -sS stands for stealth scan, no longer very stealthy but won't always be caught  

        Nmap –T4 (speed of 1-5) -p- (not sure) -A (gets more information but does take longer) IP 

    Scanning UDP 

        Namp –sU –T4 –p IP 

        UDP scanning can take longer so this is a quicker scan 