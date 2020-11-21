Enumerating with HTTP/s

    Ports 80, 443 and other common ports are common exploit vectors  

        Wannacry used an SMB flaw  

        Port 22 has SSH which historically is not a good way to do remote code execution  

    First step was to go to ip on http and https to see what comes back 

        In this case it was an apache server running redhat  

        If someone is running a default webpage is their stuff behind it? 

            Try IP/admin 

            Do directory buster to find things  

        If they're not running a website then port 443 has an open port for no reason, bad security hygiene 

        This is the kind of thing to note in a writeup  

            80/443 - IP – Time 

                Default webpage – Apache - PHP  

        Information disclosure  

            Error page on the manual page  

            Also gives the apache version, hostname (internal hostname), and port  

                Another thing to take note of 

                    Information disclosure – 404 page (screenshot) 

        Good to look at the source code for a webpage to see if there's any password or userids  

    Nikt 

        Web vuln scanner  

        If the website has good security and might autoblock if the scan is found  

            Web/application firewall  

        Nikto –h (host) http://IP 

        Shows potential vulns with versions if they are outdated  

            Bigger the difference, the better  

    Dirbuter  

        Dirbuster& 

            Loads interface  

            Add the http:/IP/port/ 

            Check go faster if you can 

            Browse to the /urs/share/wordlist/gobuster/ 

            Use the small list for this proof of concept and maybe medium or large depending on need 

        We know this is running apache, so php 

        Might be different if it's like flask or Microsoft 

        Add more filetypes to find by adding the extension sperated with commas   

    Dirb 

    Gobuster  

    ^ all do the same basic thing, directory busting  

    Through burp we see more information disclosure problems  