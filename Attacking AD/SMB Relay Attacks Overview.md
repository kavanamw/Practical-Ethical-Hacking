SMB Relay Attacks Overview 

    Instead of cracking the hash you can pass the hash on and maybe gain access 

    Requirements  

        SMB signing must be disabled for the target 

            Checks user and has and permissions, does not check signing  

        Relayed user creds must be admin  

    Dumps the Sam file 

        The etc/shadow file for windows  

        Maybe even get a full shell  

    Discovering hosts with SMB Signing disabled 

        Nmap –script=smb2-security-mode.nse -p445 IP  

            Scans this one port for SMB Signing  

            Disabled by default on any workstation but enabled by default on any server 

        Look into ntlmrelayx.py in kali 

            With a -I you can give you a shell to do a nc reverse shell on   

            -e to run a meterperter shell and add a payload  