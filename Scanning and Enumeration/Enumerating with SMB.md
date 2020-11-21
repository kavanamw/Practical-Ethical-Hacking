Enumerating with SMB

    SMB – fileshare  

    Metasploit  

        A exploit framework  

        Msfconsole to launch?  

        Search smb 

            Returns a lot of results  

        Use # 

        Info 

        Metasploit returns Unix (Samba 2.2.1a) 

    Smbclient  

        Attempt to connect to the smb file share  

            Might give us files 

            Could be useful, could be passwords  

        Smbclient –L \\\\IP\\ 

            We do get the ADMIN$ and IP$ but the admin one is more important  

            Cannot sign in with anonymous user 

            Dead end because we can't really get in further  