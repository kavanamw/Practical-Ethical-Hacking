Enumerating SSH

    Found the ssh port and version from the nmap scan  

    Not going to be able to login without exploitation  

    Basically only going to be able to see if its running  

    Normall run with ssh IP but since this box is old its 

        Ssh IP –oKexAlgorithms=+diffie-hellman-group1-sha1 –c (cipher) aes128-cbc 

            Gives a password prompt with a RSA key 

    Sometimes you get a banner with version numbers and stuff  